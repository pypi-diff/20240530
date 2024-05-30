# Comparing `tmp/microchain_python-0.3.7.tar.gz` & `tmp/microchain_python-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microchain_python-0.3.7.tar", last modified: Sun May 19 10:29:12 2024, max compression
+gzip compressed data, was "microchain_python-0.3.8.tar", last modified: Thu May 30 17:06:20 2024, max compression
```

## Comparing `microchain_python-0.3.7.tar` & `microchain_python-0.3.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 10:29:12.136514 microchain_python-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-05-19 10:29:04.000000 microchain_python-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-19 10:29:12.136514 microchain_python-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-19 10:29:04.000000 microchain_python-0.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 10:29:12.132514 microchain_python-0.3.7/microchain/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-19 10:29:04.000000 microchain_python-0.3.7/microchain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 10:29:12.132514 microchain_python-0.3.7/microchain/engine/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 10:29:04.000000 microchain_python-0.3.7/microchain/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-19 10:29:04.000000 microchain_python-0.3.7/microchain/engine/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-19 10:29:04.000000 microchain_python-0.3.7/microchain/engine/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-19 10:29:04.000000 microchain_python-0.3.7/microchain/engine/function.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-19 10:29:04.000000 microchain_python-0.3.7/microchain/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 10:29:12.132514 microchain_python-0.3.7/microchain/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 10:29:04.000000 microchain_python-0.3.7/microchain/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-05-19 10:29:04.000000 microchain_python-0.3.7/microchain/models/generators.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-19 10:29:04.000000 microchain_python-0.3.7/microchain/models/llm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-19 10:29:04.000000 microchain_python-0.3.7/microchain/models/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 10:29:12.136514 microchain_python-0.3.7/microchain_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-19 10:29:12.000000 microchain_python-0.3.7/microchain_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-19 10:29:12.000000 microchain_python-0.3.7/microchain_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 10:29:12.000000 microchain_python-0.3.7/microchain_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-19 10:29:12.000000 microchain_python-0.3.7/microchain_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-19 10:29:12.000000 microchain_python-0.3.7/microchain_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 10:29:12.136514 microchain_python-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-19 10:29:04.000000 microchain_python-0.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 10:29:12.136514 microchain_python-0.3.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-19 10:29:04.000000 microchain_python-0.3.7/tests/test_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-19 10:29:04.000000 microchain_python-0.3.7/tests/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-19 10:29:04.000000 microchain_python-0.3.7/tests/test_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-19 10:29:04.000000 microchain_python-0.3.7/tests/test_str_args.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:06:20.967702 microchain_python-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-05-30 17:06:12.000000 microchain_python-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-30 17:06:20.967702 microchain_python-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-30 17:06:12.000000 microchain_python-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:06:20.963702 microchain_python-0.3.8/microchain/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-30 17:06:12.000000 microchain_python-0.3.8/microchain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:06:20.963702 microchain_python-0.3.8/microchain/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 17:06:12.000000 microchain_python-0.3.8/microchain/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-30 17:06:12.000000 microchain_python-0.3.8/microchain/engine/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-30 17:06:12.000000 microchain_python-0.3.8/microchain/engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-30 17:06:12.000000 microchain_python-0.3.8/microchain/engine/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-30 17:06:12.000000 microchain_python-0.3.8/microchain/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:06:20.967702 microchain_python-0.3.8/microchain/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 17:06:12.000000 microchain_python-0.3.8/microchain/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-05-30 17:06:12.000000 microchain_python-0.3.8/microchain/models/generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-30 17:06:12.000000 microchain_python-0.3.8/microchain/models/llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-30 17:06:12.000000 microchain_python-0.3.8/microchain/models/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:06:20.967702 microchain_python-0.3.8/microchain_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-30 17:06:20.000000 microchain_python-0.3.8/microchain_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-30 17:06:20.000000 microchain_python-0.3.8/microchain_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 17:06:20.000000 microchain_python-0.3.8/microchain_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-30 17:06:20.000000 microchain_python-0.3.8/microchain_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-30 17:06:20.000000 microchain_python-0.3.8/microchain_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 17:06:20.967702 microchain_python-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-30 17:06:12.000000 microchain_python-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:06:20.967702 microchain_python-0.3.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-30 17:06:12.000000 microchain_python-0.3.8/tests/test_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-30 17:06:12.000000 microchain_python-0.3.8/tests/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-30 17:06:12.000000 microchain_python-0.3.8/tests/test_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-30 17:06:12.000000 microchain_python-0.3.8/tests/test_str_args.py
```

### Comparing `microchain_python-0.3.7/LICENSE` & `microchain_python-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `microchain_python-0.3.7/PKG-INFO` & `microchain_python-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microchain-python
-Version: 0.3.7
+Version: 0.3.8
 Home-page: 
 Author: Federico A. Galatolo
 Author-email: federico.galatolo@unipi.it
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
```

### Comparing `microchain_python-0.3.7/README.md` & `microchain_python-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `microchain_python-0.3.7/microchain/engine/agent.py` & `microchain_python-0.3.8/microchain/engine/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from microchain.engine.function import Function, FunctionResult
 from termcolor import colored
 
 class Agent:
-    def __init__(self, llm, engine, on_iteration_end=None):
+    def __init__(self, llm, engine, on_iteration_end=None, stop_list=["\n"]):
         self.llm = llm
         self.engine = engine
         self.max_tries = 10
         self.prompt = None
         self.bootstrap = []
         self.do_stop = False
         self.on_iteration_end = on_iteration_end
+        self.stop_list = stop_list
 
         self.engine.bind(self)
         self.reset()
 
     def reset(self):
         self.history = []
         self.do_stop = False
@@ -69,15 +70,15 @@
                 break
 
             if tries > self.max_tries:
                 print(colored(f"Tried {self.max_tries} times (agent.max_tries) Aborting", "red"))
                 abort = True
                 break
             
-            reply = self.llm(self.history + temp_messages, stop=["\n"])
+            reply = self.llm(self.history + temp_messages, stop=self.stop_list)
             reply = self.clean_reply(reply)
 
             if len(reply) < 2:
                 print(colored("Error: empty reply, aborting", "red"))
                 abort = True
                 break
```

### Comparing `microchain_python-0.3.7/microchain/engine/engine.py` & `microchain_python-0.3.8/microchain/engine/engine.py`

 * *Files identical despite different names*

### Comparing `microchain_python-0.3.7/microchain/engine/function.py` & `microchain_python-0.3.8/microchain/engine/function.py`

 * *Files identical despite different names*

### Comparing `microchain_python-0.3.7/microchain/functions.py` & `microchain_python-0.3.8/microchain/functions.py`

 * *Files identical despite different names*

### Comparing `microchain_python-0.3.7/microchain/models/generators.py` & `microchain_python-0.3.8/microchain/models/generators.py`

 * *Files identical despite different names*

### Comparing `microchain_python-0.3.7/microchain/models/templates.py` & `microchain_python-0.3.8/microchain/models/templates.py`

 * *Files identical despite different names*

### Comparing `microchain_python-0.3.7/microchain_python.egg-info/PKG-INFO` & `microchain_python-0.3.8/microchain_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microchain-python
-Version: 0.3.7
+Version: 0.3.8
 Home-page: 
 Author: Federico A. Galatolo
 Author-email: federico.galatolo@unipi.it
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
```

### Comparing `microchain_python-0.3.7/microchain_python.egg-info/SOURCES.txt` & `microchain_python-0.3.8/microchain_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `microchain_python-0.3.7/setup.py` & `microchain_python-0.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 with open(os.path.join(os.path.dirname(os.path.realpath(__file__)), "README.md"), "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="microchain-python",
-    version="0.3.7",
+    version="0.3.8",
     author="Federico A. Galatolo",
     author_email="federico.galatolo@unipi.it",
     description="",
     url="",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["microchain", "microchain.models", "microchain.engine"],
```

### Comparing `microchain_python-0.3.7/tests/test_agent.py` & `microchain_python-0.3.8/tests/test_agent.py`

 * *Files identical despite different names*

### Comparing `microchain_python-0.3.7/tests/test_engine.py` & `microchain_python-0.3.8/tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `microchain_python-0.3.7/tests/test_openai.py` & `microchain_python-0.3.8/tests/test_openai.py`

 * *Files identical despite different names*

### Comparing `microchain_python-0.3.7/tests/test_str_args.py` & `microchain_python-0.3.8/tests/test_str_args.py`

 * *Files identical despite different names*

