# Comparing `tmp/composio_crewai-0.2.9.tar.gz` & `tmp/composio_crewai-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_crewai-0.2.9.tar", last modified: Thu Apr 18 18:49:52 2024, max compression
+gzip compressed data, was "composio_crewai-0.3.0.tar", last modified: Thu May 30 03:53:16 2024, max compression
```

## Comparing `composio_crewai-0.2.9.tar` & `composio_crewai-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:49:52.938040 composio_crewai-0.2.9/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3076 2024-04-18 18:49:52.937870 composio_crewai-0.2.9/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2576 2024-04-15 07:39:40.000000 composio_crewai-0.2.9/README.md
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:49:52.936754 composio_crewai-0.2.9/composio_crewai/
--rw-r--r--   0 karanvaidya   (501) staff       (20)      110 2024-04-15 07:39:40.000000 composio_crewai-0.2.9/composio_crewai/__init__.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:49:52.937686 composio_crewai-0.2.9/composio_crewai.egg-info/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3076 2024-04-18 18:49:52.000000 composio_crewai-0.2.9/composio_crewai.egg-info/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      255 2024-04-18 18:49:52.000000 composio_crewai-0.2.9/composio_crewai.egg-info/SOURCES.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-18 18:49:52.000000 composio_crewai-0.2.9/composio_crewai.egg-info/dependency_links.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       27 2024-04-18 18:49:52.000000 composio_crewai-0.2.9/composio_crewai.egg-info/requires.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       16 2024-04-18 18:49:52.000000 composio_crewai-0.2.9/composio_crewai.egg-info/top_level.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)      275 2024-04-18 18:44:03.000000 composio_crewai-0.2.9/pyproject.toml
--rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-18 18:49:52.938080 composio_crewai-0.2.9/setup.cfg
--rw-r--r--   0 karanvaidya   (501) staff       (20)      838 2024-04-18 18:44:03.000000 composio_crewai-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:53:16.326313 composio_crewai-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-30 03:53:16.326313 composio_crewai-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-30 03:53:00.000000 composio_crewai-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:53:16.322313 composio_crewai-0.3.0/composio_crewai/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-30 03:53:00.000000 composio_crewai-0.3.0/composio_crewai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:53:16.326313 composio_crewai-0.3.0/composio_crewai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-30 03:53:16.000000 composio_crewai-0.3.0/composio_crewai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-30 03:53:16.000000 composio_crewai-0.3.0/composio_crewai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 03:53:16.000000 composio_crewai-0.3.0/composio_crewai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-30 03:53:16.000000 composio_crewai-0.3.0/composio_crewai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-30 03:53:16.000000 composio_crewai-0.3.0/composio_crewai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 03:53:16.326313 composio_crewai-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-30 03:53:00.000000 composio_crewai-0.3.0/setup.py
```

### Comparing `composio_crewai-0.2.9/PKG-INFO` & `composio_crewai-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_crewai
-Version: 0.2.9
+Version: 0.3.0
 Summary: Use Composio to get an array of tools with your CrewAI agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Himanshu
 Author-email: himanshu@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_langchain===0.2.9
+Requires-Dist: composio_langchain===0.3.0
 
 # Composio <> CrewAI
 
 ![CrewAI Logo](https://i.imgur.com/jXeNUda.png)
 
 **Composio** enables **CrewAI agents** to connect with numerous tools, making it easy for these agents to interact with external applications seamlessly.
```

### Comparing `composio_crewai-0.2.9/README.md` & `composio_crewai-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `composio_crewai-0.2.9/composio_crewai.egg-info/PKG-INFO` & `composio_crewai-0.3.0/composio_crewai.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_crewai
-Version: 0.2.9
+Version: 0.3.0
 Summary: Use Composio to get an array of tools with your CrewAI agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Himanshu
 Author-email: himanshu@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_langchain===0.2.9
+Requires-Dist: composio_langchain===0.3.0
 
 # Composio <> CrewAI
 
 ![CrewAI Logo](https://i.imgur.com/jXeNUda.png)
 
 **Composio** enables **CrewAI agents** to connect with numerous tools, making it easy for these agents to interact with external applications seamlessly.
```

### Comparing `composio_crewai-0.2.9/setup.py` & `composio_crewai-0.3.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,27 @@
-from setuptools import setup
-import os
-
-
-def get_current_dir():
-    return os.path.dirname(os.path.realpath(__file__))
+"""
+Setup configuration for Composio CrewAI plugin
+"""
 
+from pathlib import Path
 
-def resolve_paths(*paths):
-    return os.path.join(*paths)
-
+from setuptools import setup
 
-readme_path = resolve_paths(get_current_dir(), "README.md")
 
 setup(
     name="composio_crewai",
-    version="0.2.9",
+    version="0.3.0",
     author="Himanshu",
     author_email="himanshu@composio.dev",
     description="Use Composio to get an array of tools with your CrewAI agent.",
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
+    install_requires=["composio_langchain===0.3.0"],
     include_package_data=True,
 )
```

