# Comparing `tmp/composio_lyzr-0.2.9.tar.gz` & `tmp/composio_lyzr-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_lyzr-0.2.9.tar", last modified: Thu Apr 18 18:50:05 2024, max compression
+gzip compressed data, was "composio_lyzr-0.3.0.tar", last modified: Thu May 30 03:56:43 2024, max compression
```

## Comparing `composio_lyzr-0.2.9.tar` & `composio_lyzr-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,14 @@
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:50:05.499118 composio_lyzr-0.2.9/
--rw-r--r--   0 karanvaidya   (501) staff       (20)        0 2024-04-15 07:39:40.000000 composio_lyzr-0.2.9/MANIFEST.in
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2715 2024-04-18 18:50:05.498924 composio_lyzr-0.2.9/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2122 2024-04-15 07:39:40.000000 composio_lyzr-0.2.9/README.md
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:50:05.497656 composio_lyzr-0.2.9/composio_lyzr/
--rw-r--r--   0 karanvaidya   (501) staff       (20)      101 2024-04-15 07:39:40.000000 composio_lyzr-0.2.9/composio_lyzr/__init__.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     5622 2024-04-16 16:08:42.000000 composio_lyzr-0.2.9/composio_lyzr/composio_tool_spec.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2804 2024-04-15 07:39:40.000000 composio_lyzr-0.2.9/composio_lyzr/pydantic_utils.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:50:05.498714 composio_lyzr-0.2.9/composio_lyzr.egg-info/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2715 2024-04-18 18:50:05.000000 composio_lyzr-0.2.9/composio_lyzr.egg-info/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      323 2024-04-18 18:50:05.000000 composio_lyzr-0.2.9/composio_lyzr.egg-info/SOURCES.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-18 18:50:05.000000 composio_lyzr-0.2.9/composio_lyzr.egg-info/dependency_links.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       76 2024-04-18 18:50:05.000000 composio_lyzr-0.2.9/composio_lyzr.egg-info/requires.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       14 2024-04-18 18:50:05.000000 composio_lyzr-0.2.9/composio_lyzr.egg-info/top_level.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)      342 2024-04-18 18:44:03.000000 composio_lyzr-0.2.9/pyproject.toml
--rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-18 18:50:05.499162 composio_lyzr-0.2.9/setup.cfg
--rw-r--r--   0 karanvaidya   (501) staff       (20)      837 2024-04-18 18:44:03.000000 composio_lyzr-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:56:43.732885 composio_lyzr-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-05-30 03:56:43.732885 composio_lyzr-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-30 03:56:24.000000 composio_lyzr-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:56:43.728885 composio_lyzr-0.3.0/composio_lyzr/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-30 03:56:24.000000 composio_lyzr-0.3.0/composio_lyzr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-05-30 03:56:24.000000 composio_lyzr-0.3.0/composio_lyzr/toolset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:56:43.732885 composio_lyzr-0.3.0/composio_lyzr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-05-30 03:56:43.000000 composio_lyzr-0.3.0/composio_lyzr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-30 03:56:43.000000 composio_lyzr-0.3.0/composio_lyzr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 03:56:43.000000 composio_lyzr-0.3.0/composio_lyzr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-30 03:56:43.000000 composio_lyzr-0.3.0/composio_lyzr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-30 03:56:43.000000 composio_lyzr-0.3.0/composio_lyzr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 03:56:43.732885 composio_lyzr-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-30 03:56:24.000000 composio_lyzr-0.3.0/setup.py
```

### Comparing `composio_lyzr-0.2.9/PKG-INFO` & `composio_lyzr-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: composio_lyzr
-Version: 0.2.9
+Version: 0.3.0
 Summary: Use Composio to get an array of tools with your Lyzr workflow.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
 Requires-Dist: lyzr-automata>=0.1.3
 Requires-Dist: pydantic>=2.6.4
-Requires-Dist: composio_core===0.2.9
+Requires-Dist: composio_core===0.3.0
 Requires-Dist: langchain>=0.1.0
 
 ## Using Composio With Lyzr
 
 Integrate Composio with Lyzr agents to allow them to interact seamlessly with external apps, enhancing their functionality and reach.
 
 ### Goal
```

### Comparing `composio_lyzr-0.2.9/README.md` & `composio_lyzr-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `composio_lyzr-0.2.9/composio_lyzr.egg-info/PKG-INFO` & `composio_lyzr-0.3.0/composio_lyzr.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: composio_lyzr
-Version: 0.2.9
+Version: 0.3.0
 Summary: Use Composio to get an array of tools with your Lyzr workflow.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
 Requires-Dist: lyzr-automata>=0.1.3
 Requires-Dist: pydantic>=2.6.4
-Requires-Dist: composio_core===0.2.9
+Requires-Dist: composio_core===0.3.0
 Requires-Dist: langchain>=0.1.0
 
 ## Using Composio With Lyzr
 
 Integrate Composio with Lyzr agents to allow them to interact seamlessly with external apps, enhancing their functionality and reach.
 
 ### Goal
```

### Comparing `composio_lyzr-0.2.9/setup.py` & `composio_lyzr-0.3.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,32 @@
-from setuptools import setup
-import os
-
-
-def get_current_dir():
-    return os.path.dirname(os.path.realpath(__file__))
+"""
+Setup configuration for Composio Lyzr plugin.
+"""
 
+from pathlib import Path
 
-def resolve_paths(*paths):
-    return os.path.join(*paths)
-
+from setuptools import setup
 
-readme_path = resolve_paths(get_current_dir(), "README.md")
 
 setup(
     name="composio_lyzr",
-    version="0.2.9",
+    version="0.3.0",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Lyzr workflow.",
-    long_description=open(readme_path).read(),
+    long_description=(Path(__file__).parent / "README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
-    python_requires=">=3.9",
+    python_requires=">=3.9,<4",
+    install_requires=[
+        "lyzr-automata>=0.1.3",
+        "pydantic>=2.6.4",
+        "composio_core===0.3.0",
+        "langchain>=0.1.0",
+    ],
     include_package_data=True,
 )
```

