# Comparing `tmp/composio_openai-0.2.64.tar.gz` & `tmp/composio_openai-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_openai-0.2.64.tar", last modified: Thu May 23 12:24:09 2024, max compression
+gzip compressed data, was "composio_openai-0.3.0.tar", last modified: Thu May 30 03:57:37 2024, max compression
```

## Comparing `composio_openai-0.2.64.tar` & `composio_openai-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-05-23 12:24:09.086259 composio_openai-0.2.64/
--rw-r--r--   0 utkarsh    (501) staff       (20)     2615 2024-05-23 12:24:09.086060 composio_openai-0.2.64/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)     2107 2024-05-05 16:54:48.000000 composio_openai-0.2.64/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-05-23 12:24:09.084939 composio_openai-0.2.64/composio_openai/
--rw-r--r--   0 utkarsh    (501) staff       (20)      213 2024-05-23 11:22:34.000000 composio_openai-0.2.64/composio_openai/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     5304 2024-05-23 11:22:34.000000 composio_openai-0.2.64/composio_openai/openai_toolspec.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-05-23 12:24:09.085860 composio_openai-0.2.64/composio_openai.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)     2615 2024-05-23 12:24:09.000000 composio_openai-0.2.64/composio_openai.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      275 2024-05-23 12:24:09.000000 composio_openai-0.2.64/composio_openai.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-05-23 12:24:09.000000 composio_openai-0.2.64/composio_openai.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       23 2024-05-23 12:24:09.000000 composio_openai-0.2.64/composio_openai.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       16 2024-05-23 12:24:09.000000 composio_openai-0.2.64/composio_openai.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-05-23 12:24:09.086297 composio_openai-0.2.64/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)      811 2024-05-23 12:23:43.000000 composio_openai-0.2.64/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:57:37.729429 composio_openai-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-30 03:57:37.729429 composio_openai-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-30 03:57:18.000000 composio_openai-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:57:37.729429 composio_openai-0.3.0/composio_openai/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-30 03:57:18.000000 composio_openai-0.3.0/composio_openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-05-30 03:57:18.000000 composio_openai-0.3.0/composio_openai/toolset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:57:37.729429 composio_openai-0.3.0/composio_openai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-30 03:57:37.000000 composio_openai-0.3.0/composio_openai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-30 03:57:37.000000 composio_openai-0.3.0/composio_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 03:57:37.000000 composio_openai-0.3.0/composio_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 03:57:37.000000 composio_openai-0.3.0/composio_openai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-30 03:57:37.000000 composio_openai-0.3.0/composio_openai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 03:57:37.729429 composio_openai-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-30 03:57:18.000000 composio_openai-0.3.0/setup.py
```

### Comparing `composio_openai-0.2.64/PKG-INFO` & `composio_openai-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_openai
-Version: 0.2.64
+Version: 0.3.0
 Summary: Use Composio to get an array of tools with your OpenAI Function Call.
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
 
 ## 🚀🔗 Leveraging OpenAI with Composio
 
 Facilitate the integration of OpenAI with Composio to empower OpenAI models to directly interact with external applications, broadening their capabilities and application scope.
 
 ### Objective
 
@@ -48,18 +48,18 @@
 openai_client = OpenAI()
 ```
 
 ### Step 2: Integrating GitHub Tools with Composio
 
 This step involves fetching and integrating GitHub tools provided by Composio, enabling enhanced functionality for LangChain operations.
 ```python
-from composio_openai import App, ComposioToolset
+from composio_openai import App, ComposioToolSet
 
 toolset = ComposioToolset()
-actions = toolset.get_tools(tools=App.GITHUB)
+actions = toolset.get_tools(apps=[App.GITHUB])
 ```
 
 ### Step 3: Agent Execution
 
 This step involves configuring and executing the agent to carry out actions, such as starring a GitHub repository.
 
 ```python
```

### Comparing `composio_openai-0.2.64/README.md` & `composio_openai-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -34,18 +34,18 @@
 openai_client = OpenAI()
 ```
 
 ### Step 2: Integrating GitHub Tools with Composio
 
 This step involves fetching and integrating GitHub tools provided by Composio, enabling enhanced functionality for LangChain operations.
 ```python
-from composio_openai import App, ComposioToolset
+from composio_openai import App, ComposioToolSet
 
 toolset = ComposioToolset()
-actions = toolset.get_tools(tools=App.GITHUB)
+actions = toolset.get_tools(apps=[App.GITHUB])
 ```
 
 ### Step 3: Agent Execution
 
 This step involves configuring and executing the agent to carry out actions, such as starring a GitHub repository.
 
 ```python
```

### Comparing `composio_openai-0.2.64/composio_openai.egg-info/PKG-INFO` & `composio_openai-0.3.0/composio_openai.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_openai
-Version: 0.2.64
+Version: 0.3.0
 Summary: Use Composio to get an array of tools with your OpenAI Function Call.
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
 
 ## 🚀🔗 Leveraging OpenAI with Composio
 
 Facilitate the integration of OpenAI with Composio to empower OpenAI models to directly interact with external applications, broadening their capabilities and application scope.
 
 ### Objective
 
@@ -48,18 +48,18 @@
 openai_client = OpenAI()
 ```
 
 ### Step 2: Integrating GitHub Tools with Composio
 
 This step involves fetching and integrating GitHub tools provided by Composio, enabling enhanced functionality for LangChain operations.
 ```python
-from composio_openai import App, ComposioToolset
+from composio_openai import App, ComposioToolSet
 
 toolset = ComposioToolset()
-actions = toolset.get_tools(tools=App.GITHUB)
+actions = toolset.get_tools(apps=[App.GITHUB])
 ```
 
 ### Step 3: Agent Execution
 
 This step involves configuring and executing the agent to carry out actions, such as starring a GitHub repository.
 
 ```python
```

### Comparing `composio_openai-0.2.64/setup.py` & `composio_openai-0.3.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 from pathlib import Path
 
 from setuptools import setup
 
 
 setup(
     name="composio_openai",
-    version="0.2.64",
+    version="0.3.0",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your OpenAI Function Call.",
     long_description=(Path(__file__).parent / "README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.9,<4",
-    install_requires=["composio_core===0.2.64"],
+    install_requires=["composio_core===0.3.0"],
     include_package_data=True,
 )
```

