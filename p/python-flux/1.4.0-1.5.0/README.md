# Comparing `tmp/python_flux-1.4.0.tar.gz` & `tmp/python_flux-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_flux-1.4.0.tar", max compression
+gzip compressed data, was "python_flux-1.5.0.tar", max compression
```

## Comparing `python_flux-1.4.0.tar` & `python_flux-1.5.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     8872 2024-04-26 12:27:05.738836 python_flux-1.4.0/README.rst
--rw-r--r--   0        0        0      741 2024-05-28 04:58:20.786898 python_flux-1.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-07-20 21:55:18.000000 python_flux-1.4.0/python_flux/__init__.py
--rw-r--r--   0        0        0    24446 2024-05-28 04:58:20.449426 python_flux-1.4.0/python_flux/flux.py
--rw-r--r--   0        0        0      759 2024-04-25 04:03:40.583703 python_flux-1.4.0/python_flux/flux_utilis.py
--rw-r--r--   0        0        0     1905 2024-05-28 04:58:20.449885 python_flux-1.4.0/python_flux/producers.py
--rw-r--r--   0        0        0     1641 2024-04-18 05:35:27.173689 python_flux-1.4.0/python_flux/subscribers.py
--rw-r--r--   0        0        0     9603 1970-01-01 00:00:00.000000 python_flux-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     8872 2024-05-28 05:50:27.650264 python_flux-1.5.0/README.rst
+-rw-r--r--   0        0        0      741 2024-05-30 03:56:50.339511 python_flux-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-07-20 21:55:18.000000 python_flux-1.5.0/python_flux/__init__.py
+-rw-r--r--   0        0        0    25539 2024-05-30 03:54:21.005003 python_flux-1.5.0/python_flux/flux.py
+-rw-r--r--   0        0        0      849 2024-05-30 03:10:11.597706 python_flux-1.5.0/python_flux/flux_utilis.py
+-rw-r--r--   0        0        0     1905 2024-05-28 05:50:27.652881 python_flux-1.5.0/python_flux/producers.py
+-rw-r--r--   0        0        0     1641 2024-04-18 05:35:27.173689 python_flux-1.5.0/python_flux/subscribers.py
+-rw-r--r--   0        0        0     9603 1970-01-01 00:00:00.000000 python_flux-1.5.0/PKG-INFO
```

### Comparing `python_flux-1.4.0/README.rst` & `python_flux-1.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `python_flux-1.4.0/python_flux/flux.py` & `python_flux-1.5.0/python_flux/flux.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import logging
 import threading
 import types
 import time
+import concurrent.futures as cr
 from datetime import timedelta, datetime
 from functools import partial
+from statistics import mean
+
 from jsonmerge import merge
 from python_flux.flux_utilis import FluxUtils as fu
 from python_flux.subscribers import SSubscribe
 
 
 class Flux(object):
 
@@ -79,14 +82,27 @@
         se procesarán sus elementos.
 
         :param delay_ms: Delay en milisegundos que se retrasará el procesamiento de los elementos del flujo
         :param predicate: Si es verdadero se aplica el delay establecido
         """
         return FDelayMs(delay_ms, predicate, self)
 
+    def rate(self, rate, must_apply=fu.default_predicate):
+        """
+        Fuerza un flujo constante de procesamiento de elementos en el stream.
+        Para esto una vez fijado el rate de procesamiento en RPS, se mide el tiempo de producción
+        de cada elemento y si este es inerior al indicado por el rate se espera el tiempo suficiente para asegurar
+        el rate configurado.
+        Si el tiempo de procesamiento es superior a lo indicado por el rate se procesa si espera el mensaje.
+
+        :param rate: Delay en milisegundos que se retrasará el procesamiento de los elementos del flujo
+        :param must_apply: Si es verdadero se aplica el delay establecido
+        """
+        return FRateRPS(self, rate=rate, must_apply=must_apply)
+
     def chunks(self, n):
         """
         Emite un valor construido como una lista de como máximo n valores obtenidos del flujo padre.
         Si algún valor mientras se construye el chunk da error se emiten los elementos recolectados
         y luego se propaga el error.
 
         :param n: Cantidad de elementos recolectados antes de emitir el evento de lista.
@@ -390,106 +406,118 @@
         if e is not None:
             return value, e, ctx
         if valid:
             time.sleep(self.delay / 1000)
         return value, e, ctx
 
 
+class FRateRPS(Stream):
+    def __init__(self, rate, must_apply, flux):
+        super().__init__(flux)
+        self.rate = rate
+        self.predicate = must_apply
+
+    def next(self, context):
+        start_time = time.monotonic()
+        value, e, ctx = super(FRateRPS, self).next(context)
+        if e is not None:
+            return value, e, ctx
+        end_time = time.monotonic()
+
+        valid, e = fu.try_or(partial(self.predicate), value, ctx)
+        if e is not None:
+            return value, e, ctx
+        if valid:
+            delay = (1 / self.rate) - (end_time - start_time)
+            if delay > 0:
+                time.sleep(delay)
+        return value, e, ctx
+
+
 class _Register:
 
     def __init__(self):
         self.value = None
         self.e = None
-        self.start_ctx = None
-        self.end_ctx = None
-        self.thread = None
+        self.ctx = None
         self.elapsed_time = 0
 
-    def execute(self, sup):
-        t = time.process_time_ns()
+    def execute(self, sup, context):
+        t = time.monotonic()
         sup.prepare_next()
-        self.value, self.e, self.end_ctx = sup.next(self.start_ctx)
-        self.elapsed_time = (time.process_time_ns() - t) / 1000000
-
-    def set_thread(self, t):
-        self.thread = t
-
-    def set_start_context(self, ctx):
-        self.start_ctx = ctx
+        self.value, self.e, ctx = sup.next(context)
+        self.ctx = merge(context, ctx)
+        self.elapsed_time = (time.monotonic() - t)
+        return self
 
 
 class FParallel(Stream):
     def __init__(self, pool_size, join_timeout, metric_func, metric_rate, metric_buffer_size, flux):
         super().__init__(flux)
         self.pool_size = pool_size
+        self.join_timeout = join_timeout
         self.metric_func = metric_func
         self.metric_rate = metric_rate
         self.metric_buffer_size = metric_buffer_size
-        self.join_timeout = join_timeout
-        self.pool = []
+        self.executor = cr.ThreadPoolExecutor(max_workers=pool_size)
+        self.semaphore = threading.BoundedSemaphore(pool_size)
+        self.futures = []
         self.buffer_metrics = []
-        self.last_metric_execution = 0
+        self.last_metric_execution = time.monotonic()
         self.waiting_to_stop = False
 
-    def show_metrics(self, now, ctx):
+    def show_metrics(self, elapsed_time, ctx):
         if self.metric_func is not None:
+            now = time.monotonic()
+            self.buffer_metrics.append((len(self.futures), elapsed_time, now))
             len_buffer = len(self.buffer_metrics)
+            if len_buffer >= self.metric_buffer_size:
+                self.buffer_metrics.pop(0)
+
             if len_buffer > 0:
                 diff_time = max(map(lambda p: p[2], self.buffer_metrics)) - min(map(lambda p: p[2], self.buffer_metrics))
                 metrics = {
                     'pool_size': self.pool_size,
-                    'used_pool': len(self.pool),
-                    'avg_used_pool': sum(map(lambda p: p[0], self.buffer_metrics)) / len_buffer if len_buffer > 0 else 0.0,
-                    'avg_task_time_ms': sum(map(lambda p: p[1], self.buffer_metrics)) / len_buffer if len_buffer > 0 else 0.0,
-                    'rate_rps': round(1000 * len(self.buffer_metrics) / diff_time if len_buffer > 0 and diff_time > 0 else 0.0, 2)
+                    'used_pool': len(self.futures),
+                    'avg_used_pool': round(mean(map(lambda p: p[0], self.buffer_metrics)), 2),
+                    'avg_task_time_ms': round(mean(map(lambda p: p[1], self.buffer_metrics)) * 1000, 2),
+                    'rate_rps': round(len(self.buffer_metrics) / diff_time if diff_time > 0 else 0.0, 2)
                 }
-                if self.metric_rate is None or (now - self.last_metric_execution) > (1000 / self.metric_rate):
+                if self.metric_rate is None or (now - self.last_metric_execution) > (1 / self.metric_rate):
                     self.metric_func(metrics, ctx)
                     self.last_metric_execution = now
+        self.last_metric_execution = now
 
     def next(self, context):
-        ctx = context
-        while True:
+        while not self.waiting_to_stop or len(self.futures) > 0:
             if not self.waiting_to_stop:
-                if len(self.pool) < self.pool_size:
-                    reg = _Register()
-                    t = threading.Thread(target=reg.execute, args=[super(FParallel, self)])
-                    reg.set_thread(t)
-                    reg.set_start_context(ctx)
-                    self.pool.append(reg)
-                    t.start()
-            pools = self.pool.copy()
-            for r in pools:
+                self.semaphore.acquire()
                 try:
-                    now = time.process_time_ns() / 1000000
-                    self.show_metrics(now, ctx)
-                    r.thread.join(self.join_timeout)
-                    if r.thread.is_alive():
-                        continue
-                    else:
-                        self.pool.remove(r)
-                        self.buffer_metrics.append((len(self.pool), r.elapsed_time, now))
-                        if len(self.buffer_metrics) >= self.metric_buffer_size:
-                            self.buffer_metrics.pop(0)
-                        if r.end_ctx is not None:
-                            ctx = merge(ctx, r.end_ctx)
-                        if isinstance(r.e, StopIteration):
-                            self.waiting_to_stop = True
-                            if len(self.pool) == 0:
-                                self.show_metrics(now, ctx)
-                                return None, StopIteration(), ctx
-                            else:
-                                continue
-                        if self.waiting_to_stop:
-                            if len(self.pool) == 0:
-                                self.show_metrics(now, ctx)
-                                return None, StopIteration(), ctx
-                        return r.value, r.e, ctx
-                except Exception as e:
-                    return None, e, ctx
+                    future = self.executor.submit(_Register().execute, super(FParallel, self), context)
+                    self.futures.append(future)
+                except:
+                    self.semaphore.release()
+                    raise
+                else:
+                    future.add_done_callback(lambda x: self.semaphore.release())
+            try:
+                futures = self.futures.copy()
+                for future in cr.as_completed(futures, timeout=self.join_timeout):
+                    self.futures.remove(future)
+                    r = future.result()
+                    self.show_metrics(r.elapsed_time, r.ctx)
+                    if not self.waiting_to_stop and r.e is not None and isinstance(r.e, StopIteration):
+                        self.waiting_to_stop = True
+                        self.executor.shutdown(wait=True)
+                        break
+                    if r.e is None or not isinstance(r.e, StopIteration):
+                        return r.value, r.e, r.ctx
+            except TimeoutError:
+                pass
+        return None, StopIteration(), {}
 
 
 class FMap(Stream):
     def __init__(self, func, flux):
         super().__init__(flux)
         self.function = func
```

### Comparing `python_flux-1.4.0/python_flux/producers.py` & `python_flux-1.5.0/python_flux/producers.py`

 * *Files identical despite different names*

### Comparing `python_flux-1.4.0/python_flux/subscribers.py` & `python_flux-1.5.0/python_flux/subscribers.py`

 * *Files identical despite different names*

### Comparing `python_flux-1.4.0/PKG-INFO` & `python_flux-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-flux
-Version: 1.4.0
+Version: 1.5.0
 Summary: Librería que utiliza generadores de python para simular procesamiento de flujo de datos
 License: GPL-3.0-or-later
 Author: Juan Pablo Bochard
 Author-email: jbochard@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

