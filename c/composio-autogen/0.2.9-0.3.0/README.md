# Comparing `tmp/composio_autogen-0.2.9.tar.gz` & `tmp/composio_autogen-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_autogen-0.2.9.tar", last modified: Thu Apr 18 18:49:59 2024, max compression
+gzip compressed data, was "composio_autogen-0.3.0.tar", last modified: Thu May 30 03:51:31 2024, max compression
```

## Comparing `composio_autogen-0.2.9.tar` & `composio_autogen-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:49:59.117014 composio_autogen-0.2.9/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3306 2024-04-18 18:49:59.116839 composio_autogen-0.2.9/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2776 2024-04-15 07:39:40.000000 composio_autogen-0.2.9/README.md
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:49:59.115550 composio_autogen-0.2.9/composio_autogen/
--rw-r--r--   0 karanvaidya   (501) staff       (20)      100 2024-04-15 07:39:40.000000 composio_autogen-0.2.9/composio_autogen/__init__.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     8535 2024-04-16 16:08:42.000000 composio_autogen-0.2.9/composio_autogen/autogen_toolspec.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:49:59.116643 composio_autogen-0.2.9/composio_autogen.egg-info/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3306 2024-04-18 18:49:59.000000 composio_autogen-0.2.9/composio_autogen.egg-info/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      298 2024-04-18 18:49:59.000000 composio_autogen-0.2.9/composio_autogen.egg-info/SOURCES.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-18 18:49:59.000000 composio_autogen-0.2.9/composio_autogen.egg-info/dependency_links.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       40 2024-04-18 18:49:59.000000 composio_autogen-0.2.9/composio_autogen.egg-info/requires.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       17 2024-04-18 18:49:59.000000 composio_autogen-0.2.9/composio_autogen.egg-info/top_level.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)      296 2024-04-18 18:47:29.000000 composio_autogen-0.2.9/pyproject.toml
--rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-18 18:49:59.117136 composio_autogen-0.2.9/setup.cfg
--rw-r--r--   0 karanvaidya   (501) staff       (20)      840 2024-04-18 18:44:03.000000 composio_autogen-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:51:31.703913 composio_autogen-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-30 03:51:31.703913 composio_autogen-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-30 03:51:10.000000 composio_autogen-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:51:31.703913 composio_autogen-0.3.0/composio_autogen/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-30 03:51:10.000000 composio_autogen-0.3.0/composio_autogen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5967 2024-05-30 03:51:10.000000 composio_autogen-0.3.0/composio_autogen/toolset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:51:31.703913 composio_autogen-0.3.0/composio_autogen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-30 03:51:31.000000 composio_autogen-0.3.0/composio_autogen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-30 03:51:31.000000 composio_autogen-0.3.0/composio_autogen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 03:51:31.000000 composio_autogen-0.3.0/composio_autogen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-30 03:51:31.000000 composio_autogen-0.3.0/composio_autogen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-30 03:51:31.000000 composio_autogen-0.3.0/composio_autogen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 03:51:31.703913 composio_autogen-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-30 03:51:10.000000 composio_autogen-0.3.0/setup.py
```

### Comparing `composio_autogen-0.2.9/PKG-INFO` & `composio_autogen-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.2.9
+Version: 0.3.0
 Summary: Use Composio to get an array of tools with your Autogen agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.2.9
-Requires-Dist: pyautogen>=0.2.29
+Requires-Dist: composio_core===0.3.0
+Requires-Dist: pyautogen>=0.2.19
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
 
 ### Goal
```

### Comparing `composio_autogen-0.2.9/README.md` & `composio_autogen-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `composio_autogen-0.2.9/composio_autogen.egg-info/PKG-INFO` & `composio_autogen-0.3.0/composio_autogen.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.2.9
+Version: 0.3.0
 Summary: Use Composio to get an array of tools with your Autogen agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.2.9
-Requires-Dist: pyautogen>=0.2.29
+Requires-Dist: composio_core===0.3.0
+Requires-Dist: pyautogen>=0.2.19
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
 
 ### Goal
```

### Comparing `composio_autogen-0.2.9/setup.py` & `composio_autogen-0.3.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,27 @@
-from setuptools import setup
-import os
-
-
-def get_current_dir():
-    return os.path.dirname(os.path.realpath(__file__))
+"""
+Setup configuration for Composio Autogen plugin
+"""
 
+from pathlib import Path
 
-def resolve_paths(*paths):
-    return os.path.join(*paths)
-
+from setuptools import setup
 
-readme_path = resolve_paths(get_current_dir(), "README.md")
 
 setup(
     name="composio_autogen",
-    version="0.2.9",
+    version="0.3.0",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Autogen agent.",
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
+    install_requires=["composio_core===0.3.0", "pyautogen>=0.2.19"],
     include_package_data=True,
 )
```

