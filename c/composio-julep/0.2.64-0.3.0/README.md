# Comparing `tmp/composio_julep-0.2.64.tar.gz` & `tmp/composio_julep-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_julep-0.2.64.tar", last modified: Thu May 23 12:24:02 2024, max compression
+gzip compressed data, was "composio_julep-0.3.0.tar", last modified: Thu May 30 03:55:06 2024, max compression
```

## Comparing `composio_julep-0.2.64.tar` & `composio_julep-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-05-23 12:24:02.166130 composio_julep-0.2.64/
--rw-r--r--   0 utkarsh    (501) staff       (20)     4463 2024-05-23 12:24:02.165925 composio_julep-0.2.64/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)     3933 2024-05-23 11:16:37.000000 composio_julep-0.2.64/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-05-23 12:24:02.164600 composio_julep-0.2.64/composio_julep/
--rw-r--r--   0 utkarsh    (501) staff       (20)      158 2024-05-23 11:22:34.000000 composio_julep-0.2.64/composio_julep/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     1397 2024-05-23 11:22:34.000000 composio_julep-0.2.64/composio_julep/julep_toolspec.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-05-23 12:24:02.165642 composio_julep-0.2.64/composio_julep.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)     4463 2024-05-23 12:24:02.000000 composio_julep-0.2.64/composio_julep.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      267 2024-05-23 12:24:02.000000 composio_julep-0.2.64/composio_julep.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-05-23 12:24:02.000000 composio_julep-0.2.64/composio_julep.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-05-23 12:24:02.000000 composio_julep-0.2.64/composio_julep.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       15 2024-05-23 12:24:02.000000 composio_julep-0.2.64/composio_julep.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-05-23 12:24:02.166170 composio_julep-0.2.64/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)      820 2024-05-23 12:23:43.000000 composio_julep-0.2.64/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:55:06.114544 composio_julep-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-05-30 03:55:06.114544 composio_julep-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-30 03:54:44.000000 composio_julep-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:55:06.114544 composio_julep-0.3.0/composio_julep/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-30 03:54:44.000000 composio_julep-0.3.0/composio_julep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-30 03:54:44.000000 composio_julep-0.3.0/composio_julep/toolset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:55:06.114544 composio_julep-0.3.0/composio_julep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-05-30 03:55:06.000000 composio_julep-0.3.0/composio_julep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-30 03:55:06.000000 composio_julep-0.3.0/composio_julep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 03:55:06.000000 composio_julep-0.3.0/composio_julep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-30 03:55:06.000000 composio_julep-0.3.0/composio_julep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-30 03:55:06.000000 composio_julep-0.3.0/composio_julep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 03:55:06.114544 composio_julep-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-30 03:54:44.000000 composio_julep-0.3.0/setup.py
```

### Comparing `composio_julep-0.2.64/PKG-INFO` & `composio_julep-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_julep
-Version: 0.2.64
+Version: 0.3.0
 Summary: Use Composio to get an array of tools with your Julep wokflow.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_openai===0.2.64
+Requires-Dist: composio_openai===0.3.0
 Requires-Dist: julep>=0.3.2
 
 ## 🚀🔗 Integrating Composio with Julep
 
 Streamline the integration of Composio within the Julep agentic framework to enhance the interaction capabilities of Julep agents with external applications, significantly extending their operational range and efficiency.
 
 ### Objective
```

### Comparing `composio_julep-0.2.64/README.md` & `composio_julep-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `composio_julep-0.2.64/composio_julep.egg-info/PKG-INFO` & `composio_julep-0.3.0/composio_julep.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_julep
-Version: 0.2.64
+Version: 0.3.0
 Summary: Use Composio to get an array of tools with your Julep wokflow.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_openai===0.2.64
+Requires-Dist: composio_openai===0.3.0
 Requires-Dist: julep>=0.3.2
 
 ## 🚀🔗 Integrating Composio with Julep
 
 Streamline the integration of Composio within the Julep agentic framework to enhance the interaction capabilities of Julep agents with external applications, significantly extending their operational range and efficiency.
 
 ### Objective
```

### Comparing `composio_julep-0.2.64/setup.py` & `composio_julep-0.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 from pathlib import Path
 
 from setuptools import setup
 
 
 setup(
     name="composio_julep",
-    version="0.2.64",
+    version="0.3.0",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Julep wokflow.",
     long_description=(Path(__file__).parent / "README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.9,<4",
-    install_requires=["composio_openai===0.2.64", "julep>=0.3.2"],
+    install_requires=["composio_openai===0.3.0", "julep>=0.3.2"],
     include_package_data=True,
 )
```

