# Comparing `tmp/adsputils-1.5.2.tar.gz` & `tmp/adsputils-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adsputils-1.5.2.tar", last modified: Mon Dec 11 06:56:27 2023, max compression
+gzip compressed data, was "adsputils-1.5.3.tar", last modified: Thu May 30 17:33:24 2024, max compression
```

## Comparing `adsputils-1.5.2.tar` & `adsputils-1.5.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 mugdhapolimera   (502) staff       (20)        0 2023-12-11 06:56:27.169720 adsputils-1.5.2/
--rw-r--r--   0 mugdhapolimera   (502) staff       (20)     1069 2023-11-28 16:30:44.000000 adsputils-1.5.2/LICENSE
--rw-r--r--   0 mugdhapolimera   (502) staff       (20)      363 2023-12-11 06:56:27.169551 adsputils-1.5.2/PKG-INFO
--rw-r--r--   0 mugdhapolimera   (502) staff       (20)     1067 2023-11-28 16:30:44.000000 adsputils-1.5.2/README.md
-drwxr-xr-x   0 mugdhapolimera   (502) staff       (20)        0 2023-12-11 06:56:27.166693 adsputils-1.5.2/adsputils/
--rw-r--r--   0 mugdhapolimera   (502) staff       (20)    26427 2023-11-28 16:30:44.000000 adsputils-1.5.2/adsputils/__init__.py
--rw-r--r--   0 mugdhapolimera   (502) staff       (20)      316 2023-11-28 16:30:44.000000 adsputils-1.5.2/adsputils/exceptions.py
--rw-r--r--   0 mugdhapolimera   (502) staff       (20)     1669 2023-11-28 16:30:44.000000 adsputils-1.5.2/adsputils/serializer.py
-drwxr-xr-x   0 mugdhapolimera   (502) staff       (20)        0 2023-12-11 06:56:27.169236 adsputils-1.5.2/adsputils/tests/
--rw-r--r--   0 mugdhapolimera   (502) staff       (20)        0 2023-11-28 16:30:44.000000 adsputils-1.5.2/adsputils/tests/__init__.py
--rw-r--r--   0 mugdhapolimera   (502) staff       (20)       38 2023-11-28 16:30:44.000000 adsputils-1.5.2/adsputils/tests/config_sample.py
--rw-r--r--   0 mugdhapolimera   (502) staff       (20)     2062 2023-11-28 16:30:44.000000 adsputils-1.5.2/adsputils/tests/test_app.py
--rw-r--r--   0 mugdhapolimera   (502) staff       (20)     2084 2023-11-28 16:30:44.000000 adsputils-1.5.2/adsputils/tests/test_init.py
--rw-r--r--   0 mugdhapolimera   (502) staff       (20)     2332 2023-11-28 16:30:44.000000 adsputils-1.5.2/adsputils/tests/test_serializer.py
--rw-r--r--   0 mugdhapolimera   (502) staff       (20)     5163 2023-11-28 16:30:44.000000 adsputils-1.5.2/adsputils/tests/test_utils.py
-drwxr-xr-x   0 mugdhapolimera   (502) staff       (20)        0 2023-12-11 06:56:27.168144 adsputils-1.5.2/adsputils.egg-info/
--rw-r--r--   0 mugdhapolimera   (502) staff       (20)      363 2023-12-11 06:56:27.000000 adsputils-1.5.2/adsputils.egg-info/PKG-INFO
--rw-r--r--   0 mugdhapolimera   (502) staff       (20)      475 2023-12-11 06:56:27.000000 adsputils-1.5.2/adsputils.egg-info/SOURCES.txt
--rw-r--r--   0 mugdhapolimera   (502) staff       (20)        1 2023-12-11 06:56:27.000000 adsputils-1.5.2/adsputils.egg-info/dependency_links.txt
--rw-r--r--   0 mugdhapolimera   (502) staff       (20)        1 2023-11-28 16:48:18.000000 adsputils-1.5.2/adsputils.egg-info/not-zip-safe
--rw-r--r--   0 mugdhapolimera   (502) staff       (20)      208 2023-12-11 06:56:27.000000 adsputils-1.5.2/adsputils.egg-info/requires.txt
--rw-r--r--   0 mugdhapolimera   (502) staff       (20)       10 2023-12-11 06:56:27.000000 adsputils-1.5.2/adsputils.egg-info/top_level.txt
--rw-r--r--   0 mugdhapolimera   (502) staff       (20)       38 2023-12-11 06:56:27.169793 adsputils-1.5.2/setup.cfg
--rw-r--r--   0 mugdhapolimera   (502) staff       (20)     1370 2023-11-28 16:30:44.000000 adsputils-1.5.2/setup.py
+drwxr-xr-x   0 klockhart   (503) staff       (20)        0 2024-05-30 17:33:24.330861 adsputils-1.5.3/
+-rw-r--r--   0 klockhart   (503) staff       (20)     1069 2018-01-04 21:57:55.000000 adsputils-1.5.3/LICENSE
+-rw-r--r--   0 klockhart   (503) staff       (20)      726 2024-05-30 17:33:24.330646 adsputils-1.5.3/PKG-INFO
+-rw-r--r--   0 klockhart   (503) staff       (20)     1067 2024-05-24 19:40:26.000000 adsputils-1.5.3/README.md
+drwxr-xr-x   0 klockhart   (503) staff       (20)        0 2024-05-30 17:33:24.328240 adsputils-1.5.3/adsputils/
+-rw-r--r--   0 klockhart   (503) staff       (20)    26685 2024-05-30 17:33:15.000000 adsputils-1.5.3/adsputils/__init__.py
+-rw-r--r--   0 klockhart   (503) staff       (20)      316 2020-03-16 20:15:13.000000 adsputils-1.5.3/adsputils/exceptions.py
+-rw-r--r--   0 klockhart   (503) staff       (20)     1669 2018-01-04 21:57:55.000000 adsputils-1.5.3/adsputils/serializer.py
+drwxr-xr-x   0 klockhart   (503) staff       (20)        0 2024-05-30 17:33:24.330080 adsputils-1.5.3/adsputils/tests/
+-rw-r--r--   0 klockhart   (503) staff       (20)        0 2018-01-04 21:57:55.000000 adsputils-1.5.3/adsputils/tests/__init__.py
+-rw-r--r--   0 klockhart   (503) staff       (20)       38 2018-01-04 21:57:55.000000 adsputils-1.5.3/adsputils/tests/config_sample.py
+-rw-r--r--   0 klockhart   (503) staff       (20)     2062 2020-04-28 19:59:59.000000 adsputils-1.5.3/adsputils/tests/test_app.py
+-rw-r--r--   0 klockhart   (503) staff       (20)     2084 2020-04-28 19:59:59.000000 adsputils-1.5.3/adsputils/tests/test_init.py
+-rw-r--r--   0 klockhart   (503) staff       (20)     2332 2020-04-28 19:59:59.000000 adsputils-1.5.3/adsputils/tests/test_serializer.py
+-rw-r--r--   0 klockhart   (503) staff       (20)     5163 2020-04-28 19:59:59.000000 adsputils-1.5.3/adsputils/tests/test_utils.py
+drwxr-xr-x   0 klockhart   (503) staff       (20)        0 2024-05-30 17:33:24.330416 adsputils-1.5.3/adsputils.egg-info/
+-rw-r--r--   0 klockhart   (503) staff       (20)      726 2024-05-30 17:33:24.000000 adsputils-1.5.3/adsputils.egg-info/PKG-INFO
+-rw-r--r--   0 klockhart   (503) staff       (20)      475 2024-05-30 17:33:24.000000 adsputils-1.5.3/adsputils.egg-info/SOURCES.txt
+-rw-r--r--   0 klockhart   (503) staff       (20)        1 2024-05-30 17:33:24.000000 adsputils-1.5.3/adsputils.egg-info/dependency_links.txt
+-rw-r--r--   0 klockhart   (503) staff       (20)        1 2020-04-28 20:03:24.000000 adsputils-1.5.3/adsputils.egg-info/not-zip-safe
+-rw-r--r--   0 klockhart   (503) staff       (20)      208 2024-05-30 17:33:24.000000 adsputils-1.5.3/adsputils.egg-info/requires.txt
+-rw-r--r--   0 klockhart   (503) staff       (20)       10 2024-05-30 17:33:24.000000 adsputils-1.5.3/adsputils.egg-info/top_level.txt
+-rw-r--r--   0 klockhart   (503) staff       (20)       38 2024-05-30 17:33:24.330903 adsputils-1.5.3/setup.cfg
+-rw-r--r--   0 klockhart   (503) staff       (20)     1370 2022-09-14 19:19:57.000000 adsputils-1.5.3/setup.py
```

### Comparing `adsputils-1.5.2/LICENSE` & `adsputils-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `adsputils-1.5.2/README.md` & `adsputils-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `adsputils-1.5.2/adsputils/__init__.py` & `adsputils-1.5.3/adsputils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -378,30 +378,15 @@
                              'are you sure CELERY_DEFAULT_EXCHANGE_TYPE is set properly? (%s)',
                              self._config.get('CELERY_DEFAULT_EXCHANGE_TYPE', ''))
 
         self.exchange = Exchange(self._config.get('CELERY_DEFAULT_EXCHANGE', 'ads-pipeline'),
                 type=self._config.get('CELERY_DEFAULT_EXCHANGE_TYPE', 'topic'))
 
         self.forwarding_connection = None
-        if self._config.get('OUTPUT_CELERY_BROKER', None):
-            # kombu connection is lazy loaded, so it's ok to create now
-            self.forwarding_connection = BrokerConnection(self._config['OUTPUT_CELERY_BROKER'])
-
-            if self.conf.get('OUTPUT_TASKNAME', None):
-
-                @self.task(name=self._config['OUTPUT_TASKNAME'],
-                           exchange=self._config.get('OUTPUT_EXCHANGE', 'ads-pipeline'),
-                           queue=self._config.get('OUTPUT_QUEUE', 'update-record'),
-                           routing_key=self._config.get('OUTPUT_QUEUE', 'update-record'))
-                def _forward_message(self, *args, **kwargs):
-                    """A handler that can be used to forward stuff out of our
-                    queue. It does nothing (it doesn't process data)"""
-                    self.logger.error('We should have never been called directly! %s' % \
-                                      (args, kwargs))
-                self._forward_message = _forward_message
+        self._forward_message = None
 
         # HTTP connection pool
         # - The maximum number of retries each connection should attempt: this
         #   applies only to failed DNS lookups, socket connections and connection timeouts,
         #   never to requests where data has made it to the server. By default,
         #   requests does not retry failed connections.
         # http://docs.python-requests.org/en/latest/api/?highlight=max_retries#requests.adapters.HTTPAdapter
@@ -420,20 +405,44 @@
         if 'adsmsg' not in registry.name_to_type:
             register('adsmsg', *register_args)
 
         self.conf['CELERY_ACCEPT_CONTENT'] = ['adsmsg', 'json']
         self.conf['CELERY_TASK_SERIALIZER'] = 'adsmsg'
         self.conf['CELERY_RESULT_SERIALIZER'] = 'adsmsg'
 
-    def forward_message(self, *args, **kwargs):
-        """Class method that is replaced during initializiton with the real
-        implementation (IFF) the OUTPUT_TASKNAME and oother OUTPUT_ parameters
-        are specified."""
-        if not self.forwarding_connection or not self._forward_message:
-            raise NotImplementedError('Sorry, your app is not properly configured.')
+    def forward_message(self, output_taskname=None, output_celery_broker=None, *args, **kwargs):
+        """Class method that sets up the message forwarding handler dynamically based on
+        OUTPUT_TASKNAME and OUTPUT_CELERY_BROKER."""
+
+        # Use OUTPUT_CELERY_BROKER from config if not provided at call time
+        broker = output_celery_broker or self._config.get('OUTPUT_CELERY_BROKER')
+        if broker:
+            # kombu connection is lazy loaded, so it's ok to create now
+            self.forwarding_connection = BrokerConnection(broker)
+
+        if not self.forwarding_connection:
+            raise NotImplementedError('Sorry, your app is not properly configured (no broker).')
+
+        # Use OUTPUT_TASKNAME from config if not provided at call time
+        task_name = output_taskname or self._config.get('OUTPUT_TASKNAME')
+
+        if task_name:
+            @self.task(name=task_name,
+                       exchange=self._config.get('OUTPUT_EXCHANGE', 'ads-pipeline'),
+                       queue=self._config.get('OUTPUT_QUEUE', 'update-record'),
+                       routing_key=self._config.get('OUTPUT_QUEUE', 'update-record'))
+            def _forward_message(*args, **kwargs):
+                """A handler that can be used to forward stuff out of our queue. It does nothing (it doesn't process data)."""
+                self.logger.error('We should have never been called directly! %s' % (args, kwargs))
+
+            self._forward_message = _forward_message
+
+        if not self._forward_message:
+            raise NotImplementedError('Sorry, your app is not properly configured (no task handler).')
+
         self.logger.debug('Forwarding results out to: %s', self.forwarding_connection)
         return self._forward_message.apply_async(args, kwargs,
                                                  connection=self.forwarding_connection)
 
     def _get_callers_module(self):
         frame = inspect.stack()[2]
         m = inspect.getmodule(frame[0])
```

### Comparing `adsputils-1.5.2/adsputils/serializer.py` & `adsputils-1.5.3/adsputils/serializer.py`

 * *Files identical despite different names*

### Comparing `adsputils-1.5.2/adsputils/tests/test_app.py` & `adsputils-1.5.3/adsputils/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `adsputils-1.5.2/adsputils/tests/test_init.py` & `adsputils-1.5.3/adsputils/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `adsputils-1.5.2/adsputils/tests/test_serializer.py` & `adsputils-1.5.3/adsputils/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `adsputils-1.5.2/adsputils/tests/test_utils.py` & `adsputils-1.5.3/adsputils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `adsputils-1.5.2/setup.py` & `adsputils-1.5.3/setup.py`

 * *Files identical despite different names*

