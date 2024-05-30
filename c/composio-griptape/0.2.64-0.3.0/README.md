# Comparing `tmp/composio_griptape-0.2.64.tar.gz` & `tmp/composio_griptape-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_griptape-0.2.64.tar", last modified: Thu May 23 12:23:59 2024, max compression
+gzip compressed data, was "composio_griptape-0.3.0.tar", last modified: Thu May 30 03:54:11 2024, max compression
```

## Comparing `composio_griptape-0.2.64.tar` & `composio_griptape-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-05-23 12:23:59.694748 composio_griptape-0.2.64/
--rw-r--r--   0 utkarsh    (501) staff       (20)     2389 2024-05-23 12:23:59.694549 composio_griptape-0.2.64/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)     1851 2024-05-16 16:34:56.000000 composio_griptape-0.2.64/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-05-23 12:23:59.693158 composio_griptape-0.2.64/composio_griptape/
--rw-r--r--   0 utkarsh    (501) staff       (20)      161 2024-05-16 16:34:56.000000 composio_griptape-0.2.64/composio_griptape/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     5101 2024-05-23 11:22:34.000000 composio_griptape-0.2.64/composio_griptape/griptape_toolspec.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-05-23 12:23:59.694313 composio_griptape-0.2.64/composio_griptape.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)     2389 2024-05-23 12:23:59.000000 composio_griptape-0.2.64/composio_griptape.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      291 2024-05-23 12:23:59.000000 composio_griptape-0.2.64/composio_griptape.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-05-23 12:23:59.000000 composio_griptape-0.2.64/composio_griptape.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       40 2024-05-23 12:23:59.000000 composio_griptape-0.2.64/composio_griptape.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       18 2024-05-23 12:23:59.000000 composio_griptape-0.2.64/composio_griptape.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-05-23 12:23:59.694784 composio_griptape-0.2.64/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)      831 2024-05-23 12:23:43.000000 composio_griptape-0.2.64/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:54:11.654971 composio_griptape-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-05-30 03:54:11.654971 composio_griptape-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-30 03:53:49.000000 composio_griptape-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:54:11.654971 composio_griptape-0.3.0/composio_griptape/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-30 03:53:49.000000 composio_griptape-0.3.0/composio_griptape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-05-30 03:53:49.000000 composio_griptape-0.3.0/composio_griptape/toolset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:54:11.654971 composio_griptape-0.3.0/composio_griptape.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-05-30 03:54:11.000000 composio_griptape-0.3.0/composio_griptape.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-30 03:54:11.000000 composio_griptape-0.3.0/composio_griptape.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 03:54:11.000000 composio_griptape-0.3.0/composio_griptape.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-30 03:54:11.000000 composio_griptape-0.3.0/composio_griptape.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 03:54:11.000000 composio_griptape-0.3.0/composio_griptape.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 03:54:11.654971 composio_griptape-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-30 03:53:49.000000 composio_griptape-0.3.0/setup.py
```

### Comparing `composio_griptape-0.2.64/PKG-INFO` & `composio_griptape-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_griptape
-Version: 0.2.64
+Version: 0.3.0
 Summary: Use Composio to get an array of tools with your Griptape wokflow.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.2.64
+Requires-Dist: composio_core===0.3.0
 Requires-Dist: griptape>=0.24.2
 
 ## 🚀🔗 Integrating Composio with Griptape
 
 Streamline the integration of Composio within the Griptape agentic framework to enhance the interaction capabilities of Griptape agents with external applications, significantly extending their operational range and efficiency.
 
 ### Objective
```

### Comparing `composio_griptape-0.2.64/README.md` & `composio_griptape-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `composio_griptape-0.2.64/composio_griptape.egg-info/PKG-INFO` & `composio_griptape-0.3.0/composio_griptape.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_griptape
-Version: 0.2.64
+Version: 0.3.0
 Summary: Use Composio to get an array of tools with your Griptape wokflow.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.2.64
+Requires-Dist: composio_core===0.3.0
 Requires-Dist: griptape>=0.24.2
 
 ## 🚀🔗 Integrating Composio with Griptape
 
 Streamline the integration of Composio within the Griptape agentic framework to enhance the interaction capabilities of Griptape agents with external applications, significantly extending their operational range and efficiency.
 
 ### Objective
```

### Comparing `composio_griptape-0.2.64/setup.py` & `composio_griptape-0.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 from pathlib import Path
 
 from setuptools import setup
 
 
 setup(
     name="composio_griptape",
-    version="0.2.64",
+    version="0.3.0",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Griptape wokflow.",
     long_description=(Path(__file__).parent / "README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.9,<4",
-    install_requires=["composio_core===0.2.64", "griptape>=0.24.2"],
+    install_requires=["composio_core===0.3.0", "griptape>=0.24.2"],
     include_package_data=True,
 )
```

