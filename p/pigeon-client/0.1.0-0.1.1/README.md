# Comparing `tmp/pigeon_client-0.1.0.tar.gz` & `tmp/pigeon_client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pigeon_client-0.1.0.tar", last modified: Thu May 30 14:52:08 2024, max compression
+gzip compressed data, was "pigeon_client-0.1.1.tar", last modified: Thu May 30 17:02:46 2024, max compression
```

## Comparing `pigeon_client-0.1.0.tar` & `pigeon_client-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 cameron   (1000) cameron   (1000)        0 2024-05-30 14:52:08.507588 pigeon_client-0.1.0/
--rw-rw-r--   0 cameron   (1000) cameron   (1000)     1463 2024-05-30 14:20:44.000000 pigeon_client-0.1.0/LICENSE
--rw-r--r--   0 cameron   (1000) cameron   (1000)     1475 2024-05-30 14:52:08.507588 pigeon_client-0.1.0/PKG-INFO
--rw-rw-r--   0 cameron   (1000) cameron   (1000)      606 2024-05-30 14:51:53.000000 pigeon_client-0.1.0/README.md
-drwxrwxr-x   0 cameron   (1000) cameron   (1000)        0 2024-05-30 14:52:08.503588 pigeon_client-0.1.0/pigeon/
--rw-rw-r--   0 cameron   (1000) cameron   (1000)       60 2024-05-29 20:52:40.000000 pigeon_client-0.1.0/pigeon/__init__.py
--rw-rw-r--   0 cameron   (1000) cameron   (1000)     2059 2024-05-29 20:53:19.000000 pigeon_client-0.1.0/pigeon/__main__.py
--rw-rw-r--   0 cameron   (1000) cameron   (1000)      260 2024-05-24 22:16:38.000000 pigeon_client-0.1.0/pigeon/base_msg.py
--rw-rw-r--   0 cameron   (1000) cameron   (1000)     5498 2024-05-29 20:52:52.000000 pigeon_client-0.1.0/pigeon/client.py
--rw-rw-r--   0 cameron   (1000) cameron   (1000)      101 2024-05-24 22:09:05.000000 pigeon_client-0.1.0/pigeon/exceptions.py
--rw-rw-r--   0 cameron   (1000) cameron   (1000)      387 2024-05-24 22:09:05.000000 pigeon_client-0.1.0/pigeon/logging.py
-drwxrwxr-x   0 cameron   (1000) cameron   (1000)        0 2024-05-30 14:52:08.507588 pigeon_client-0.1.0/pigeon_client.egg-info/
--rw-r--r--   0 cameron   (1000) cameron   (1000)     1475 2024-05-30 14:52:08.000000 pigeon_client-0.1.0/pigeon_client.egg-info/PKG-INFO
--rw-rw-r--   0 cameron   (1000) cameron   (1000)      417 2024-05-30 14:52:08.000000 pigeon_client-0.1.0/pigeon_client.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron   (1000) cameron   (1000)        1 2024-05-30 14:52:08.000000 pigeon_client-0.1.0/pigeon_client.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron   (1000) cameron   (1000)       48 2024-05-30 14:52:08.000000 pigeon_client-0.1.0/pigeon_client.egg-info/entry_points.txt
--rw-rw-r--   0 cameron   (1000) cameron   (1000)       25 2024-05-30 14:52:08.000000 pigeon_client-0.1.0/pigeon_client.egg-info/requires.txt
--rw-rw-r--   0 cameron   (1000) cameron   (1000)        7 2024-05-30 14:52:08.000000 pigeon_client-0.1.0/pigeon_client.egg-info/top_level.txt
--rw-rw-r--   0 cameron   (1000) cameron   (1000)      859 2024-05-30 14:50:43.000000 pigeon_client-0.1.0/pyproject.toml
--rw-rw-r--   0 cameron   (1000) cameron   (1000)       38 2024-05-30 14:52:08.507588 pigeon_client-0.1.0/setup.cfg
-drwxrwxr-x   0 cameron   (1000) cameron   (1000)        0 2024-05-30 14:52:08.503588 pigeon_client-0.1.0/tests/
--rw-rw-r--   0 cameron   (1000) cameron   (1000)      794 2024-05-29 20:56:31.000000 pigeon_client-0.1.0/tests/test_base_message.py
--rw-rw-r--   0 cameron   (1000) cameron   (1000)     5209 2024-05-29 20:56:21.000000 pigeon_client-0.1.0/tests/test_client.py
+drwxrwxr-x   0 cameron   (1000) cameron   (1000)        0 2024-05-30 17:02:46.293723 pigeon_client-0.1.1/
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)     1463 2024-05-30 14:20:44.000000 pigeon_client-0.1.1/LICENSE
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1475 2024-05-30 17:02:46.293723 pigeon_client-0.1.1/PKG-INFO
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)      606 2024-05-30 14:51:53.000000 pigeon_client-0.1.1/README.md
+drwxrwxr-x   0 cameron   (1000) cameron   (1000)        0 2024-05-30 17:02:46.293723 pigeon_client-0.1.1/pigeon/
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)       60 2024-05-29 20:52:40.000000 pigeon_client-0.1.1/pigeon/__init__.py
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)     2059 2024-05-29 20:53:19.000000 pigeon_client-0.1.1/pigeon/__main__.py
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)      260 2024-05-24 22:16:38.000000 pigeon_client-0.1.1/pigeon/base_msg.py
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)     5495 2024-05-30 17:00:47.000000 pigeon_client-0.1.1/pigeon/client.py
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)      101 2024-05-24 22:09:05.000000 pigeon_client-0.1.1/pigeon/exceptions.py
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)      387 2024-05-24 22:09:05.000000 pigeon_client-0.1.1/pigeon/logging.py
+drwxrwxr-x   0 cameron   (1000) cameron   (1000)        0 2024-05-30 17:02:46.293723 pigeon_client-0.1.1/pigeon_client.egg-info/
+-rw-r--r--   0 cameron   (1000) cameron   (1000)     1475 2024-05-30 17:02:46.000000 pigeon_client-0.1.1/pigeon_client.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)      434 2024-05-30 17:02:46.000000 pigeon_client-0.1.1/pigeon_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)        1 2024-05-30 17:02:46.000000 pigeon_client-0.1.1/pigeon_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)       48 2024-05-30 17:02:46.000000 pigeon_client-0.1.1/pigeon_client.egg-info/entry_points.txt
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)       25 2024-05-30 17:02:46.000000 pigeon_client-0.1.1/pigeon_client.egg-info/requires.txt
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)        7 2024-05-30 17:02:46.000000 pigeon_client-0.1.1/pigeon_client.egg-info/top_level.txt
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)      901 2024-05-30 17:01:37.000000 pigeon_client-0.1.1/pyproject.toml
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)       24 2024-05-30 16:39:16.000000 pigeon_client-0.1.1/requirements.txt
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)       38 2024-05-30 17:02:46.293723 pigeon_client-0.1.1/setup.cfg
+drwxrwxr-x   0 cameron   (1000) cameron   (1000)        0 2024-05-30 17:02:46.293723 pigeon_client-0.1.1/tests/
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)      794 2024-05-29 20:56:31.000000 pigeon_client-0.1.1/tests/test_base_message.py
+-rw-rw-r--   0 cameron   (1000) cameron   (1000)     5209 2024-05-29 20:56:21.000000 pigeon_client-0.1.1/tests/test_client.py
```

### Comparing `pigeon_client-0.1.0/LICENSE` & `pigeon_client-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pigeon_client-0.1.0/PKG-INFO` & `pigeon_client-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pigeon-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: A STOMP client with message definitions via Pydantic
 Author-email: Cameron Devine <cameron.devine@alleninstitute.org>
 License: BSD 3 Clause
 Project-URL: Homepage, https://github.com/AllenInstitute/pigeon
 Project-URL: Documentation, http://pigeon.readthedocs.io/
 Project-URL: Repository, https://github.com/AllenInstitute/pigeon
 Project-URL: Issues, https://github.com/AllenInstitute/pigeon/issues
```

### Comparing `pigeon_client-0.1.0/README.md` & `pigeon_client-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pigeon_client-0.1.0/pigeon/__main__.py` & `pigeon_client-0.1.1/pigeon/__main__.py`

 * *Files identical despite different names*

### Comparing `pigeon_client-0.1.0/pigeon/client.py` & `pigeon_client-0.1.1/pigeon/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     @staticmethod
     def _configure_logging() -> logging.Logger:
         logger = logging.getLogger(__name__)
         logger.setLevel(logging.INFO)
         return logger
 
     def _load_topics(self):
-        for entrypoint in entry_points(group="emarfarap.msgs"):
+        for entrypoint in entry_points(group="pigeon.msgs"):
             self.register_topics(*entrypoint.load())
 
     def register_topics(self, topics: Dict[str, Callable], version: str):
         self._topics.update(topics)
         self._msg_versions.update({ topic:version for topic in topics })
 
     def register_topic(self, topic: str, msg_class: Callable, version: str):
```

### Comparing `pigeon_client-0.1.0/pigeon_client.egg-info/PKG-INFO` & `pigeon_client-0.1.1/pigeon_client.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pigeon-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: A STOMP client with message definitions via Pydantic
 Author-email: Cameron Devine <cameron.devine@alleninstitute.org>
 License: BSD 3 Clause
 Project-URL: Homepage, https://github.com/AllenInstitute/pigeon
 Project-URL: Documentation, http://pigeon.readthedocs.io/
 Project-URL: Repository, https://github.com/AllenInstitute/pigeon
 Project-URL: Issues, https://github.com/AllenInstitute/pigeon/issues
```

### Comparing `pigeon_client-0.1.0/pyproject.toml` & `pigeon_client-0.1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 [project]
 name = "pigeon-client"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Cameron Devine", email="cameron.devine@alleninstitute.org" },
 ]
 description = "A STOMP client with message definitions via Pydantic"
 readme = "README.md"
 requires-python = ">=3.10"
-dependencies=[
-  "pydantic",
-  "stomp-py",
-  "pyyaml",
-]
 license = {text = "BSD 3 Clause"}
 classifiers = [
   "Intended Audience :: Developers",
   "License :: OSI Approved :: BSD License",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
+dynamic = ["dependencies"]
 
 [project.scripts]
 pigeon = "pigeon.__main__:main"
 
 [project.urls]
 Homepage = "https://github.com/AllenInstitute/pigeon"
 Documentation = "http://pigeon.readthedocs.io/"
 Repository = "https://github.com/AllenInstitute/pigeon"
-Issues = "https://github.com/AllenInstitute/pigeon/issues"
+Issues = "https://github.com/AllenInstitute/pigeon/issues"
+
+[tool.setuptools.dynamic]
+dependencies = {file = ["requirements.txt"]}
```

### Comparing `pigeon_client-0.1.0/tests/test_base_message.py` & `pigeon_client-0.1.1/tests/test_base_message.py`

 * *Files identical despite different names*

### Comparing `pigeon_client-0.1.0/tests/test_client.py` & `pigeon_client-0.1.1/tests/test_client.py`

 * *Files identical despite different names*

