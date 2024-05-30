# Comparing `tmp/pyeventengine-0.3.0.post2.tar.gz` & `tmp/pyeventengine-0.3.0.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyeventengine-0.3.0.post2.tar", last modified: Tue May 28 11:03:38 2024, max compression
+gzip compressed data, was "pyeventengine-0.3.0.post3.tar", last modified: Wed May 29 05:33:59 2024, max compression
```

## Comparing `pyeventengine-0.3.0.post2.tar` & `pyeventengine-0.3.0.post3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-28 11:03:38.758236 pyeventengine-0.3.0.post2/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1066 2024-05-28 06:20:25.000000 pyeventengine-0.3.0.post2/LICENSE
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     2112 2024-05-28 11:03:38.755233 pyeventengine-0.3.0.post2/PKG-INFO
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-28 11:03:38.734233 pyeventengine-0.3.0.post2/PyEventEngine.egg-info/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     2112 2024-05-28 11:03:38.000000 pyeventengine-0.3.0.post2/PyEventEngine.egg-info/PKG-INFO
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)      364 2024-05-28 11:03:38.000000 pyeventengine-0.3.0.post2/PyEventEngine.egg-info/SOURCES.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)        1 2024-05-28 11:03:38.000000 pyeventengine-0.3.0.post2/PyEventEngine.egg-info/dependency_links.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       13 2024-05-28 11:03:38.000000 pyeventengine-0.3.0.post2/PyEventEngine.egg-info/top_level.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1510 2024-05-28 11:01:21.000000 pyeventengine-0.3.0.post2/README.md
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-28 11:03:38.493878 pyeventengine-0.3.0.post2/event_engine/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       51 2024-05-28 11:03:19.000000 pyeventengine-0.3.0.post2/event_engine/__init__.py
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-28 11:03:38.507881 pyeventengine-0.3.0.post2/event_engine/cpp/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     9271 2024-05-28 06:20:25.000000 pyeventengine-0.3.0.post2/event_engine/cpp/topic_api.cpp
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-28 11:03:38.615981 pyeventengine-0.3.0.post2/event_engine/native/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     3227 2024-05-28 10:24:33.000000 pyeventengine-0.3.0.post2/event_engine/native/__init__.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)    13778 2024-05-28 10:17:54.000000 pyeventengine-0.3.0.post2/event_engine/native/_event.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     4525 2024-05-28 10:21:19.000000 pyeventengine-0.3.0.post2/event_engine/native/_topic.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     3001 2024-05-28 06:54:14.000000 pyeventengine-0.3.0.post2/event_engine/native/_topic_c.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       79 2024-05-28 11:03:38.760236 pyeventengine-0.3.0.post2/setup.cfg
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1736 2024-05-28 11:01:21.000000 pyeventengine-0.3.0.post2/setup.py
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-29 05:33:59.703257 pyeventengine-0.3.0.post3/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1066 2024-05-28 06:20:25.000000 pyeventengine-0.3.0.post3/LICENSE
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     2112 2024-05-29 05:33:59.701259 pyeventengine-0.3.0.post3/PKG-INFO
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-29 05:33:59.698258 pyeventengine-0.3.0.post3/PyEventEngine.egg-info/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     2112 2024-05-29 05:33:59.000000 pyeventengine-0.3.0.post3/PyEventEngine.egg-info/PKG-INFO
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)      364 2024-05-29 05:33:59.000000 pyeventengine-0.3.0.post3/PyEventEngine.egg-info/SOURCES.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)        1 2024-05-29 05:33:59.000000 pyeventengine-0.3.0.post3/PyEventEngine.egg-info/dependency_links.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       13 2024-05-29 05:33:59.000000 pyeventengine-0.3.0.post3/PyEventEngine.egg-info/top_level.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1510 2024-05-28 11:01:21.000000 pyeventengine-0.3.0.post3/README.md
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-29 05:33:59.624171 pyeventengine-0.3.0.post3/event_engine/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       51 2024-05-29 05:33:10.000000 pyeventengine-0.3.0.post3/event_engine/__init__.py
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-29 05:33:59.631171 pyeventengine-0.3.0.post3/event_engine/cpp/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     9271 2024-05-28 06:20:25.000000 pyeventengine-0.3.0.post3/event_engine/cpp/topic_api.cpp
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-29 05:33:59.689258 pyeventengine-0.3.0.post3/event_engine/native/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     3227 2024-05-28 10:24:33.000000 pyeventengine-0.3.0.post3/event_engine/native/__init__.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    13782 2024-05-29 05:32:38.000000 pyeventengine-0.3.0.post3/event_engine/native/_event.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     4525 2024-05-28 10:21:19.000000 pyeventengine-0.3.0.post3/event_engine/native/_topic.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     3001 2024-05-28 06:54:14.000000 pyeventengine-0.3.0.post3/event_engine/native/_topic_c.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       79 2024-05-29 05:33:59.705258 pyeventengine-0.3.0.post3/setup.cfg
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1736 2024-05-28 11:01:21.000000 pyeventengine-0.3.0.post3/setup.py
```

### Comparing `pyeventengine-0.3.0.post2/LICENSE` & `pyeventengine-0.3.0.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyeventengine-0.3.0.post2/PKG-INFO` & `pyeventengine-0.3.0.post3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyEventEngine
-Version: 0.3.0.post2
+Version: 0.3.0.post3
 Summary: Basic event engine
 Home-page: https://github.com/BolunHan/PyEventEngine.git
 Author: Bolun.Han
 Author-email: Bolun.Han@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyeventengine-0.3.0.post2/PyEventEngine.egg-info/PKG-INFO` & `pyeventengine-0.3.0.post3/PyEventEngine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyEventEngine
-Version: 0.3.0.post2
+Version: 0.3.0.post3
 Summary: Basic event engine
 Home-page: https://github.com/BolunHan/PyEventEngine.git
 Author: Bolun.Han
 Author-email: Bolun.Han@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyeventengine-0.3.0.post2/README.md` & `pyeventengine-0.3.0.post3/README.md`

 * *Files identical despite different names*

### Comparing `pyeventengine-0.3.0.post2/event_engine/cpp/topic_api.cpp` & `pyeventengine-0.3.0.post3/event_engine/cpp/topic_api.cpp`

 * *Files identical despite different names*

### Comparing `pyeventengine-0.3.0.post2/event_engine/native/__init__.py` & `pyeventengine-0.3.0.post3/event_engine/native/__init__.py`

 * *Files identical despite different names*

### Comparing `pyeventengine-0.3.0.post2/event_engine/native/_event.py` & `pyeventengine-0.3.0.post3/event_engine/native/_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
         """
         Get event from queue and then process it.
         """
         while self._active:
             self._get_lock.acquire(blocking=True, timeout=None)
 
             try:
-                event_dict = self._deque.pop()
+                event_dict = self._deque.popleft()
             except IndexError as e:
                 if not self._active:
                     return
                 raise e
 
             topic = event_dict['topic']
             args = event_dict.get('args', ())
```

### Comparing `pyeventengine-0.3.0.post2/event_engine/native/_topic.py` & `pyeventengine-0.3.0.post3/event_engine/native/_topic.py`

 * *Files identical despite different names*

### Comparing `pyeventengine-0.3.0.post2/event_engine/native/_topic_c.py` & `pyeventengine-0.3.0.post3/event_engine/native/_topic_c.py`

 * *Files identical despite different names*

### Comparing `pyeventengine-0.3.0.post2/setup.py` & `pyeventengine-0.3.0.post3/setup.py`

 * *Files identical despite different names*

