# Comparing `tmp/sirji-agents-0.0.8.tar.gz` & `tmp/sirji-agents-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sirji-agents-0.0.8.tar", last modified: Fri Apr  5 13:25:47 2024, max compression
+gzip compressed data, was "sirji-agents-0.0.9.tar", last modified: Fri Apr  5 16:17:35 2024, max compression
```

## Comparing `sirji-agents-0.0.8.tar` & `sirji-agents-0.0.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 13:25:47.587227 sirji-agents-0.0.8/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1069 2024-04-05 13:25:43.000000 sirji-agents-0.0.8/LICENSE
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       15 2024-04-05 13:25:43.000000 sirji-agents-0.0.8/MANIFEST.in
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3436 2024-04-05 13:25:47.585115 sirji-agents-0.0.8/PKG-INFO
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3060 2024-04-05 13:25:43.000000 sirji-agents-0.0.8/README.md
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       38 2024-04-05 13:25:47.587534 sirji-agents-0.0.8/setup.cfg
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      684 2024-04-05 13:25:43.000000 sirji-agents-0.0.8/setup.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 13:25:47.569756 sirji-agents-0.0.8/sirji_agents/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      188 2024-04-05 13:25:43.000000 sirji-agents-0.0.8/sirji_agents/__init__.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 13:25:47.574743 sirji-agents-0.0.8/sirji_agents/llm/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 13:25:43.000000 sirji-agents-0.0.8/sirji_agents/llm/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2545 2024-04-05 13:25:43.000000 sirji-agents-0.0.8/sirji_agents/llm/base.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      228 2024-04-05 13:25:43.000000 sirji-agents-0.0.8/sirji_agents/llm/coder.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      232 2024-04-05 13:25:43.000000 sirji-agents-0.0.8/sirji_agents/llm/planner.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 13:25:47.575730 sirji-agents-0.0.8/sirji_agents/researcher/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       67 2024-04-05 13:25:43.000000 sirji-agents-0.0.8/sirji_agents/researcher/__init__.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 13:25:47.578370 sirji-agents-0.0.8/sirji_agents/researcher/embeddings/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 13:25:43.000000 sirji-agents-0.0.8/sirji_agents/researcher/embeddings/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      385 2024-04-05 13:25:43.000000 sirji-agents-0.0.8/sirji_agents/researcher/embeddings/base.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      342 2024-04-05 13:25:43.000000 sirji-agents-0.0.8/sirji_agents/researcher/embeddings/factory.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     5844 2024-04-05 13:25:43.000000 sirji-agents-0.0.8/sirji_agents/researcher/embeddings/openai_assistant.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 13:25:47.581852 sirji-agents-0.0.8/sirji_agents/researcher/inferer/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 13:25:43.000000 sirji-agents-0.0.8/sirji_agents/researcher/inferer/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1075 2024-04-05 13:25:43.000000 sirji-agents-0.0.8/sirji_agents/researcher/inferer/base.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      324 2024-04-05 13:25:43.000000 sirji-agents-0.0.8/sirji_agents/researcher/inferer/factory.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     4364 2024-04-05 13:25:43.000000 sirji-agents-0.0.8/sirji_agents/researcher/inferer/openai_assistant.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     4705 2024-04-05 13:25:43.000000 sirji-agents-0.0.8/sirji_agents/researcher/researcher.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 13:25:47.583593 sirji-agents-0.0.8/sirji_agents.egg-info/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3436 2024-04-05 13:25:47.000000 sirji-agents-0.0.8/sirji_agents.egg-info/PKG-INFO
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      794 2024-04-05 13:25:47.000000 sirji-agents-0.0.8/sirji_agents.egg-info/SOURCES.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        1 2024-04-05 13:25:47.000000 sirji-agents-0.0.8/sirji_agents.egg-info/dependency_links.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       56 2024-04-05 13:25:47.000000 sirji-agents-0.0.8/sirji_agents.egg-info/requires.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       13 2024-04-05 13:25:47.000000 sirji-agents-0.0.8/sirji_agents.egg-info/top_level.txt
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 16:17:35.516390 sirji-agents-0.0.9/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1069 2024-04-05 16:17:31.000000 sirji-agents-0.0.9/LICENSE
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       15 2024-04-05 16:17:31.000000 sirji-agents-0.0.9/MANIFEST.in
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     5748 2024-04-05 16:17:35.515978 sirji-agents-0.0.9/PKG-INFO
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     5372 2024-04-05 16:17:31.000000 sirji-agents-0.0.9/README.md
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       38 2024-04-05 16:17:35.516478 sirji-agents-0.0.9/setup.cfg
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      684 2024-04-05 16:17:31.000000 sirji-agents-0.0.9/setup.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 16:17:35.507888 sirji-agents-0.0.9/sirji_agents/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      188 2024-04-05 16:17:31.000000 sirji-agents-0.0.9/sirji_agents/__init__.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 16:17:35.511094 sirji-agents-0.0.9/sirji_agents/llm/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 16:17:31.000000 sirji-agents-0.0.9/sirji_agents/llm/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2545 2024-04-05 16:17:31.000000 sirji-agents-0.0.9/sirji_agents/llm/base.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      228 2024-04-05 16:17:31.000000 sirji-agents-0.0.9/sirji_agents/llm/coder.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      232 2024-04-05 16:17:31.000000 sirji-agents-0.0.9/sirji_agents/llm/planner.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 16:17:35.511933 sirji-agents-0.0.9/sirji_agents/researcher/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       67 2024-04-05 16:17:31.000000 sirji-agents-0.0.9/sirji_agents/researcher/__init__.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 16:17:35.513309 sirji-agents-0.0.9/sirji_agents/researcher/embeddings/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 16:17:31.000000 sirji-agents-0.0.9/sirji_agents/researcher/embeddings/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      385 2024-04-05 16:17:31.000000 sirji-agents-0.0.9/sirji_agents/researcher/embeddings/base.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      342 2024-04-05 16:17:31.000000 sirji-agents-0.0.9/sirji_agents/researcher/embeddings/factory.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     5844 2024-04-05 16:17:31.000000 sirji-agents-0.0.9/sirji_agents/researcher/embeddings/openai_assistant.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 16:17:35.514922 sirji-agents-0.0.9/sirji_agents/researcher/inferer/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 16:17:31.000000 sirji-agents-0.0.9/sirji_agents/researcher/inferer/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1075 2024-04-05 16:17:31.000000 sirji-agents-0.0.9/sirji_agents/researcher/inferer/base.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      324 2024-04-05 16:17:31.000000 sirji-agents-0.0.9/sirji_agents/researcher/inferer/factory.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     4364 2024-04-05 16:17:31.000000 sirji-agents-0.0.9/sirji_agents/researcher/inferer/openai_assistant.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     4705 2024-04-05 16:17:31.000000 sirji-agents-0.0.9/sirji_agents/researcher/researcher.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 16:17:35.515453 sirji-agents-0.0.9/sirji_agents.egg-info/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     5748 2024-04-05 16:17:35.000000 sirji-agents-0.0.9/sirji_agents.egg-info/PKG-INFO
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      794 2024-04-05 16:17:35.000000 sirji-agents-0.0.9/sirji_agents.egg-info/SOURCES.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        1 2024-04-05 16:17:35.000000 sirji-agents-0.0.9/sirji_agents.egg-info/dependency_links.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       56 2024-04-05 16:17:35.000000 sirji-agents-0.0.9/sirji_agents.egg-info/requires.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       13 2024-04-05 16:17:35.000000 sirji-agents-0.0.9/sirji_agents.egg-info/top_level.txt
```

### Comparing `sirji-agents-0.0.8/LICENSE` & `sirji-agents-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sirji-agents-0.0.8/setup.py` & `sirji-agents-0.0.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sirji-agents',
-    version='0.0.8',
+    version='0.0.9',
     author='Sirji',
     description='Research, Coding and Planning agents used by Sirji.',
     license='MIT',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/sirji-ai/sirji',
     packages=find_packages(),
```

### Comparing `sirji-agents-0.0.8/sirji_agents/llm/base.py` & `sirji-agents-0.0.9/sirji_agents/llm/base.py`

 * *Files identical despite different names*

### Comparing `sirji-agents-0.0.8/sirji_agents/researcher/embeddings/openai_assistant.py` & `sirji-agents-0.0.9/sirji_agents/researcher/embeddings/openai_assistant.py`

 * *Files identical despite different names*

### Comparing `sirji-agents-0.0.8/sirji_agents/researcher/inferer/base.py` & `sirji-agents-0.0.9/sirji_agents/researcher/inferer/base.py`

 * *Files identical despite different names*

### Comparing `sirji-agents-0.0.8/sirji_agents/researcher/inferer/openai_assistant.py` & `sirji-agents-0.0.9/sirji_agents/researcher/inferer/openai_assistant.py`

 * *Files identical despite different names*

### Comparing `sirji-agents-0.0.8/sirji_agents/researcher/researcher.py` & `sirji-agents-0.0.9/sirji_agents/researcher/researcher.py`

 * *Files identical despite different names*

### Comparing `sirji-agents-0.0.8/sirji_agents.egg-info/SOURCES.txt` & `sirji-agents-0.0.9/sirji_agents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

