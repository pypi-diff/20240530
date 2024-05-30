# Comparing `tmp/microlearn_llm_factory-0.0.7.tar.gz` & `tmp/microlearn_llm_factory-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microlearn_llm_factory-0.0.7.tar", last modified: Fri Sep 22 06:44:46 2023, max compression
+gzip compressed data, was "microlearn_llm_factory-0.0.9.tar", last modified: Wed Mar  6 07:04:23 2024, max compression
```

## Comparing `microlearn_llm_factory-0.0.7.tar` & `microlearn_llm_factory-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 06:44:46.746015 microlearn_llm_factory-0.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 06:44:46.746015 microlearn_llm_factory-0.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 06:44:46.746015 microlearn_llm_factory-0.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2023-09-22 06:44:36.000000 microlearn_llm_factory-0.0.7/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-09-22 06:44:36.000000 microlearn_llm_factory-0.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      701 2023-09-22 06:44:46.746015 microlearn_llm_factory-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      540 2023-09-22 06:44:36.000000 microlearn_llm_factory-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-09-22 06:44:36.000000 microlearn_llm_factory-0.0.7/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2023-09-22 06:44:36.000000 microlearn_llm_factory-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-09-22 06:44:36.000000 microlearn_llm_factory-0.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      761 2023-09-22 06:44:46.746015 microlearn_llm_factory-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 06:44:46.746015 microlearn_llm_factory-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 06:44:46.746015 microlearn_llm_factory-0.0.7/src/llm_factory/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 06:44:36.000000 microlearn_llm_factory-0.0.7/src/llm_factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2023-09-22 06:44:36.000000 microlearn_llm_factory-0.0.7/src/llm_factory/llm_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2023-09-22 06:44:36.000000 microlearn_llm_factory-0.0.7/src/llm_factory/llm_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2023-09-22 06:44:36.000000 microlearn_llm_factory-0.0.7/src/llm_factory/llm_openai_chat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 06:44:46.746015 microlearn_llm_factory-0.0.7/src/microlearn_llm_factory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2023-09-22 06:44:46.000000 microlearn_llm_factory-0.0.7/src/microlearn_llm_factory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      514 2023-09-22 06:44:46.000000 microlearn_llm_factory-0.0.7/src/microlearn_llm_factory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-22 06:44:46.000000 microlearn_llm_factory-0.0.7/src/microlearn_llm_factory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-09-22 06:44:46.000000 microlearn_llm_factory-0.0.7/src/microlearn_llm_factory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-09-22 06:44:46.000000 microlearn_llm_factory-0.0.7/src/microlearn_llm_factory.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 06:44:46.746015 microlearn_llm_factory-0.0.7/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2023-09-22 06:44:36.000000 microlearn_llm_factory-0.0.7/src/tests/test_llm_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 07:04:23.138795 microlearn_llm_factory-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 07:04:23.134794 microlearn_llm_factory-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 07:04:23.138795 microlearn_llm_factory-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-03-06 07:04:15.000000 microlearn_llm_factory-0.0.9/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-06 07:04:15.000000 microlearn_llm_factory-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-03-06 07:04:23.138795 microlearn_llm_factory-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-03-06 07:04:15.000000 microlearn_llm_factory-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-06 07:04:15.000000 microlearn_llm_factory-0.0.9/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-06 07:04:15.000000 microlearn_llm_factory-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-06 07:04:15.000000 microlearn_llm_factory-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-03-06 07:04:23.138795 microlearn_llm_factory-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 07:04:23.134794 microlearn_llm_factory-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 07:04:23.138795 microlearn_llm_factory-0.0.9/src/llm_factory/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 07:04:15.000000 microlearn_llm_factory-0.0.9/src/llm_factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-06 07:04:15.000000 microlearn_llm_factory-0.0.9/src/llm_factory/llm_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-03-06 07:04:15.000000 microlearn_llm_factory-0.0.9/src/llm_factory/llm_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-03-06 07:04:15.000000 microlearn_llm_factory-0.0.9/src/llm_factory/llm_openai_chat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 07:04:23.138795 microlearn_llm_factory-0.0.9/src/microlearn_llm_factory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-03-06 07:04:23.000000 microlearn_llm_factory-0.0.9/src/microlearn_llm_factory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-06 07:04:23.000000 microlearn_llm_factory-0.0.9/src/microlearn_llm_factory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 07:04:23.000000 microlearn_llm_factory-0.0.9/src/microlearn_llm_factory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-06 07:04:23.000000 microlearn_llm_factory-0.0.9/src/microlearn_llm_factory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-06 07:04:23.000000 microlearn_llm_factory-0.0.9/src/microlearn_llm_factory.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 07:04:23.138795 microlearn_llm_factory-0.0.9/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-03-06 07:04:15.000000 microlearn_llm_factory-0.0.9/src/tests/test_llm_factory.py
```

### Comparing `microlearn_llm_factory-0.0.7/.github/workflows/publish.yml` & `microlearn_llm_factory-0.0.9/.github/workflows/publish.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 name: Python package
 
 on:
   release:
     types: [published]
+  workflow_dispatch:
 
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.8", "3.9", "3.10", "3.11"]
+        python-version: ["3.8", ]
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Setup Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
           cache: "pip"
       - name: Install dependencies
         run: |
           python3 -m pip install --upgrade pip
           pip install pytest
@@ -30,19 +31,19 @@
           OPENAI_API_KEY: ${{ secrets.OPENAI_API_KEY }}
 
   publish:
     needs: test
     runs-on: ubuntu-latest
     steps:
       - name: Checkout
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
         with:
           fetch-depth: 0
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.x"
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install build
       - name: Build package
```

### Comparing `microlearn_llm_factory-0.0.7/PKG-INFO` & `microlearn_llm_factory-0.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: microlearn_llm_factory
-Version: 0.0.7
+Version: 0.0.9
 Summary: A python package for managing microlearn LLM interaction classes
 Home-page: https://github.com/AIprojectflow/llm_factory
 Project-URL: Bug Tracker, https://github.com/AIprojectflow/llm_factory/issues
 Project-URL: Changelog, https://github.com/AIprojectflow/llm_factory/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: langchain<0.1,>=0.0.235
-Requires-Dist: openai<1.0,>=0.27.8
+Requires-Dist: langchain>=0.1.11
+Requires-Dist: langchain-community>=0.0.25
+Requires-Dist: langchain-openai>=0.0.8
+Requires-Dist: openai>=1.13.3
 Requires-Dist: python-dotenv
-Requires-Dist: promptlayer<0.2,>=0.1.95
+Requires-Dist: promptlayer>=0.5.0
```

### Comparing `microlearn_llm_factory-0.0.7/setup.cfg` & `microlearn_llm_factory-0.0.9/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -13,18 +13,20 @@
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.8
 install_requires = 
-	langchain >= 0.0.235, < 0.1
-	openai >= 0.27.8, < 1.0
+	langchain >= 0.1.11
+	langchain-community >= 0.0.25
+	langchain-openai >= 0.0.8
+	openai >= 1.13.3
 	python-dotenv
-	promptlayer >= 0.1.95, < 0.2
+	promptlayer >= 0.5.0
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `microlearn_llm_factory-0.0.7/src/llm_factory/llm_factory.py` & `microlearn_llm_factory-0.0.9/src/llm_factory/llm_factory.py`

 * *Files identical despite different names*

### Comparing `microlearn_llm_factory-0.0.7/src/llm_factory/llm_openai_chat.py` & `microlearn_llm_factory-0.0.9/src/llm_factory/llm_openai_chat.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 LLM wrapper for OpenAI chat model.
 """
 import promptlayer  # Do not remove this line.
-from langchain.callbacks import PromptLayerCallbackHandler
-from langchain.chat_models import ChatOpenAI
+from langchain_community.callbacks import PromptLayerCallbackHandler
+from langchain_openai import ChatOpenAI
 
 from llm_factory.llm_base import LLMBase
 
 
 class LLMOpenAIChat(LLMBase):
     """
     LLM wrapper for OpenAI chat model.
```

### Comparing `microlearn_llm_factory-0.0.7/src/microlearn_llm_factory.egg-info/SOURCES.txt` & `microlearn_llm_factory-0.0.9/src/microlearn_llm_factory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `microlearn_llm_factory-0.0.7/src/tests/test_llm_factory.py` & `microlearn_llm_factory-0.0.9/src/tests/test_llm_factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     pytest src/tests/test_llm_factory.py -v --log-cli-level INFO
 """
 import sys
 from pathlib import Path
 sys.path.insert(0, str(Path(__file__).parent.parent))
 
 from llm_factory.llm_factory import LLMFactory
-from langchain.chat_models import ChatOpenAI
+from langchain_openai import ChatOpenAI
 import pytest
 from dotenv import load_dotenv
 
 
 load_dotenv(override=True)
```

