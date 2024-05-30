# Comparing `tmp/composio_claude-0.2.64.tar.gz` & `tmp/composio_claude-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_claude-0.2.64.tar", last modified: Thu May 23 12:23:55 2024, max compression
+gzip compressed data, was "composio_claude-0.3.0.tar", last modified: Thu May 30 03:52:27 2024, max compression
```

## Comparing `composio_claude-0.2.64.tar` & `composio_claude-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-05-23 12:23:55.167031 composio_claude-0.2.64/
--rw-r--r--   0 utkarsh    (501) staff       (20)     2561 2024-05-23 12:23:55.166824 composio_claude-0.2.64/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)     2027 2024-05-16 16:34:56.000000 composio_claude-0.2.64/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-05-23 12:23:55.165799 composio_claude-0.2.64/composio_claude/
--rw-r--r--   0 utkarsh    (501) staff       (20)      158 2024-05-23 11:22:34.000000 composio_claude-0.2.64/composio_claude/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     1519 2024-05-23 11:22:34.000000 composio_claude-0.2.64/composio_claude/claude_toolset.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-05-23 12:23:55.166643 composio_claude-0.2.64/composio_claude.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)     2561 2024-05-23 12:23:55.000000 composio_claude-0.2.64/composio_claude.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      274 2024-05-23 12:23:55.000000 composio_claude-0.2.64/composio_claude.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-05-23 12:23:55.000000 composio_claude-0.2.64/composio_claude.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       43 2024-05-23 12:23:55.000000 composio_claude-0.2.64/composio_claude.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       16 2024-05-23 12:23:55.000000 composio_claude-0.2.64/composio_claude.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-05-23 12:23:55.167074 composio_claude-0.2.64/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)      825 2024-05-23 12:23:43.000000 composio_claude-0.2.64/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:52:27.198695 composio_claude-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-30 03:52:27.198695 composio_claude-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-30 03:52:07.000000 composio_claude-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:52:27.198695 composio_claude-0.3.0/composio_claude/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-30 03:52:07.000000 composio_claude-0.3.0/composio_claude/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-05-30 03:52:07.000000 composio_claude-0.3.0/composio_claude/toolset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:52:27.198695 composio_claude-0.3.0/composio_claude.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-30 03:52:27.000000 composio_claude-0.3.0/composio_claude.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-30 03:52:27.000000 composio_claude-0.3.0/composio_claude.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 03:52:27.000000 composio_claude-0.3.0/composio_claude.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-30 03:52:27.000000 composio_claude-0.3.0/composio_claude.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-30 03:52:27.000000 composio_claude-0.3.0/composio_claude.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 03:52:27.198695 composio_claude-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-30 03:52:07.000000 composio_claude-0.3.0/setup.py
```

### Comparing `composio_claude-0.2.64/PKG-INFO` & `composio_claude-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_claude
-Version: 0.2.64
+Version: 0.3.0
 Summary: Use Composio to get an array of tools with your Claude LLMs.
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
 Requires-Dist: anthropic>=0.25.7
 
 ## 🚀🔗 Leveraging Claude with Composio
 
 Facilitate the integration of Claude with Composio to empower Claude models to directly interact with external applications, broadening their capabilities and application scope.
 
 ### Objective
```

### Comparing `composio_claude-0.2.64/README.md` & `composio_claude-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `composio_claude-0.2.64/composio_claude.egg-info/PKG-INFO` & `composio_claude-0.3.0/composio_claude.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_claude
-Version: 0.2.64
+Version: 0.3.0
 Summary: Use Composio to get an array of tools with your Claude LLMs.
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
 Requires-Dist: anthropic>=0.25.7
 
 ## 🚀🔗 Leveraging Claude with Composio
 
 Facilitate the integration of Claude with Composio to empower Claude models to directly interact with external applications, broadening their capabilities and application scope.
 
 ### Objective
```

### Comparing `composio_claude-0.2.64/setup.py` & `composio_claude-0.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 from pathlib import Path
 
 from setuptools import setup
 
 
 setup(
     name="composio_claude",
-    version="0.2.64",
+    version="0.3.0",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Claude LLMs.",
     long_description=(Path(__file__).parent / "README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.9,<4",
-    install_requires=["composio_openai===0.2.64", "anthropic>=0.25.7"],
+    install_requires=["composio_openai===0.3.0", "anthropic>=0.25.7"],
     include_package_data=True,
 )
```

