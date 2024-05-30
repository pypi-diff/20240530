# Comparing `tmp/flatpack-3.5.8.tar.gz` & `tmp/flatpack-3.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatpack-3.5.8.tar", last modified: Thu May 30 13:08:59 2024, max compression
+gzip compressed data, was "flatpack-3.5.9.tar", last modified: Thu May 30 13:47:37 2024, max compression
```

## Comparing `flatpack-3.5.8.tar` & `flatpack-3.5.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-30 13:08:59.651033 flatpack-3.5.8/
--rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.5.8/LICENSE
--rw-r--r--   0 romlingroup   (501) staff       (20)     5913 2024-05-30 13:08:59.650653 flatpack-3.5.8/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)     5158 2024-05-30 13:08:13.000000 flatpack-3.5.8/README.md
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-30 13:08:59.648027 flatpack-3.5.8/flatpack/
--rw-r--r--   0 romlingroup   (501) staff       (20)      138 2024-05-02 14:39:05.000000 flatpack-3.5.8/flatpack/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     2494 2024-05-02 07:38:12.000000 flatpack-3.5.8/flatpack/agent_manager.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.5.8/flatpack/config.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.5.8/flatpack/datasets.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-30 13:08:59.649405 flatpack-3.5.8/flatpack/engines/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:17:03.000000 flatpack-3.5.8/flatpack/engines/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     3489 2024-05-26 03:22:42.000000 flatpack-3.5.8/flatpack/engines/engine_llama_cpp.py
--rw-rw-r--   0 romlingroup   (501) staff       (20)     1057 2023-09-28 21:46:27.000000 flatpack-3.5.8/flatpack/instructions.py
--rw-r--r--   0 romlingroup   (501) staff       (20)       53 2024-05-29 16:20:58.000000 flatpack-3.5.8/flatpack/load_engines.py
--rw-r--r--   0 romlingroup   (501) staff       (20)       60 2024-05-29 16:21:02.000000 flatpack-3.5.8/flatpack/load_modules.py
--rw-r--r--   0 romlingroup   (501) staff       (20)    36263 2024-05-29 16:04:50.000000 flatpack-3.5.8/flatpack/main.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-30 13:08:59.649938 flatpack-3.5.8/flatpack/modules/
--rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.5.8/flatpack/modules/__init__.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.5.8/flatpack/modules/lstm.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.5.8/flatpack/modules/rnn.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     6983 2024-05-14 17:52:21.000000 flatpack-3.5.8/flatpack/parsers.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      290 2024-04-27 11:31:48.000000 flatpack-3.5.8/flatpack/session_manager.py
--rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.5.8/flatpack/utils.py
--rw-r--r--   0 romlingroup   (501) staff       (20)     8911 2024-05-26 02:17:11.000000 flatpack-3.5.8/flatpack/vector_manager.py
-drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-30 13:08:59.650226 flatpack-3.5.8/flatpack.egg-info/
--rw-r--r--   0 romlingroup   (501) staff       (20)     5913 2024-05-30 13:08:59.000000 flatpack-3.5.8/flatpack.egg-info/PKG-INFO
--rw-r--r--   0 romlingroup   (501) staff       (20)      636 2024-05-30 13:08:59.000000 flatpack-3.5.8/flatpack.egg-info/SOURCES.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-05-30 13:08:59.000000 flatpack-3.5.8/flatpack.egg-info/dependency_links.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-05-30 13:08:59.000000 flatpack-3.5.8/flatpack.egg-info/entry_points.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)      268 2024-05-30 13:08:59.000000 flatpack-3.5.8/flatpack.egg-info/requires.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-05-30 13:08:59.000000 flatpack-3.5.8/flatpack.egg-info/top_level.txt
--rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-05-30 13:08:59.651117 flatpack-3.5.8/setup.cfg
--rw-r--r--   0 romlingroup   (501) staff       (20)     1022 2024-05-30 13:08:21.000000 flatpack-3.5.8/setup.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-30 13:47:37.534948 flatpack-3.5.9/
+-rw-r--r--   0 romlingroup   (501) staff       (20)    11357 2024-01-31 06:56:56.000000 flatpack-3.5.9/LICENSE
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5740 2024-05-30 13:47:37.534611 flatpack-3.5.9/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5019 2024-05-30 13:47:11.000000 flatpack-3.5.9/README.md
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-30 13:47:37.531828 flatpack-3.5.9/flatpack/
+-rw-r--r--   0 romlingroup   (501) staff       (20)      138 2024-05-02 14:39:05.000000 flatpack-3.5.9/flatpack/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     2494 2024-05-02 07:38:12.000000 flatpack-3.5.9/flatpack/agent_manager.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      407 2024-01-31 06:56:56.000000 flatpack-3.5.9/flatpack/config.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     1029 2024-01-31 06:56:56.000000 flatpack-3.5.9/flatpack/datasets.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-30 13:47:37.533498 flatpack-3.5.9/flatpack/engines/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-04-29 23:17:03.000000 flatpack-3.5.9/flatpack/engines/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     3489 2024-05-26 03:22:42.000000 flatpack-3.5.9/flatpack/engines/engine_llama_cpp.py
+-rw-rw-r--   0 romlingroup   (501) staff       (20)     1057 2023-09-28 21:46:27.000000 flatpack-3.5.9/flatpack/instructions.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)       53 2024-05-29 16:20:58.000000 flatpack-3.5.9/flatpack/load_engines.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)       60 2024-05-29 16:21:02.000000 flatpack-3.5.9/flatpack/load_modules.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)    36263 2024-05-29 16:04:50.000000 flatpack-3.5.9/flatpack/main.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-30 13:47:37.533998 flatpack-3.5.9/flatpack/modules/
+-rw-r--r--   0 romlingroup   (501) staff       (20)        0 2024-01-31 06:56:56.000000 flatpack-3.5.9/flatpack/modules/__init__.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4297 2024-01-31 06:56:56.000000 flatpack-3.5.9/flatpack/modules/lstm.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     4292 2024-01-31 06:56:56.000000 flatpack-3.5.9/flatpack/modules/rnn.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     6983 2024-05-14 17:52:21.000000 flatpack-3.5.9/flatpack/parsers.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      290 2024-04-27 11:31:48.000000 flatpack-3.5.9/flatpack/session_manager.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)      184 2024-01-31 06:56:56.000000 flatpack-3.5.9/flatpack/utils.py
+-rw-r--r--   0 romlingroup   (501) staff       (20)     8911 2024-05-26 02:17:11.000000 flatpack-3.5.9/flatpack/vector_manager.py
+drwxr-xr-x   0 romlingroup   (501) staff       (20)        0 2024-05-30 13:47:37.534278 flatpack-3.5.9/flatpack.egg-info/
+-rw-r--r--   0 romlingroup   (501) staff       (20)     5740 2024-05-30 13:47:37.000000 flatpack-3.5.9/flatpack.egg-info/PKG-INFO
+-rw-r--r--   0 romlingroup   (501) staff       (20)      636 2024-05-30 13:47:37.000000 flatpack-3.5.9/flatpack.egg-info/SOURCES.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        1 2024-05-30 13:47:37.000000 flatpack-3.5.9/flatpack.egg-info/dependency_links.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       48 2024-05-30 13:47:37.000000 flatpack-3.5.9/flatpack.egg-info/entry_points.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)      249 2024-05-30 13:47:37.000000 flatpack-3.5.9/flatpack.egg-info/requires.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)        9 2024-05-30 13:47:37.000000 flatpack-3.5.9/flatpack.egg-info/top_level.txt
+-rw-r--r--   0 romlingroup   (501) staff       (20)       38 2024-05-30 13:47:37.535019 flatpack-3.5.9/setup.cfg
+-rw-r--r--   0 romlingroup   (501) staff       (20)      992 2024-05-30 13:47:15.000000 flatpack-3.5.9/setup.py
```

### Comparing `flatpack-3.5.8/LICENSE` & `flatpack-3.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.8/PKG-INFO` & `flatpack-3.5.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.5.8
+Version: 3.5.9
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
@@ -15,15 +15,14 @@
 Requires-Dist: ngrok==1.2.0
 Requires-Dist: nltk==3.8.1
 Requires-Dist: psutil==5.9.5
 Requires-Dist: pydantic==2.7.1
 Requires-Dist: pypdf==4.2.0
 Requires-Dist: requests==2.31.0
 Requires-Dist: sentence-transformers==2.7.0
-Requires-Dist: setuptools==70.0.0
 Requires-Dist: toml==0.10.2
 Requires-Dist: torch==2.3.0
 Requires-Dist: uvicorn==0.29.0
 
 # Flatpack
 
 **NOTE:** Flatpack is currently experimental. Please refrain from using it in production environments.
@@ -115,17 +114,14 @@
 
 - **[requests](https://pypi.org/project/requests/)**\
   Apache Software License (Apache 2.0) ([LICENSE](https://github.com/psf/requests/blob/main/LICENSE))
 
 - **[sentence-transformers](https://pypi.org/project/sentence-transformers/)**\
   Apache Software License (Apache License 2.0) ([LICENSE](https://github.com/UKPLab/sentence-transformers/blob/master/LICENSE))
 
-- **[setuptools](https://pypi.org/project/setuptools/)**\
-  MIT License ([LICENSE](https://github.com/pypa/setuptools/blob/main/LICENSE))
-
 - **[toml](https://pypi.org/project/toml/)**\
   MIT License (MIT) ([LICENSE](https://github.com/uiri/toml/blob/master/LICENSE))
 
 - **[torch](https://pypi.org/project/torch/)**\
   BSD License (BSD-3) ([LICENSE](https://github.com/pytorch/pytorch/blob/main/LICENSE))
 
 - **[uvicorn](https://pypi.org/project/uvicorn/)**\
```

### Comparing `flatpack-3.5.8/README.md` & `flatpack-3.5.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -89,17 +89,14 @@
 
 - **[requests](https://pypi.org/project/requests/)**\
   Apache Software License (Apache 2.0) ([LICENSE](https://github.com/psf/requests/blob/main/LICENSE))
 
 - **[sentence-transformers](https://pypi.org/project/sentence-transformers/)**\
   Apache Software License (Apache License 2.0) ([LICENSE](https://github.com/UKPLab/sentence-transformers/blob/master/LICENSE))
 
-- **[setuptools](https://pypi.org/project/setuptools/)**\
-  MIT License ([LICENSE](https://github.com/pypa/setuptools/blob/main/LICENSE))
-
 - **[toml](https://pypi.org/project/toml/)**\
   MIT License (MIT) ([LICENSE](https://github.com/uiri/toml/blob/master/LICENSE))
 
 - **[torch](https://pypi.org/project/torch/)**\
   BSD License (BSD-3) ([LICENSE](https://github.com/pytorch/pytorch/blob/main/LICENSE))
 
 - **[uvicorn](https://pypi.org/project/uvicorn/)**\
```

### Comparing `flatpack-3.5.8/flatpack/agent_manager.py` & `flatpack-3.5.9/flatpack/agent_manager.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.8/flatpack/datasets.py` & `flatpack-3.5.9/flatpack/datasets.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.8/flatpack/engines/engine_llama_cpp.py` & `flatpack-3.5.9/flatpack/engines/engine_llama_cpp.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.8/flatpack/instructions.py` & `flatpack-3.5.9/flatpack/instructions.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.8/flatpack/main.py` & `flatpack-3.5.9/flatpack/main.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.8/flatpack/modules/lstm.py` & `flatpack-3.5.9/flatpack/modules/lstm.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.8/flatpack/modules/rnn.py` & `flatpack-3.5.9/flatpack/modules/rnn.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.8/flatpack/parsers.py` & `flatpack-3.5.9/flatpack/parsers.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.8/flatpack/vector_manager.py` & `flatpack-3.5.9/flatpack/vector_manager.py`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.8/flatpack.egg-info/PKG-INFO` & `flatpack-3.5.9/flatpack.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatpack
-Version: 3.5.8
+Version: 3.5.9
 Summary: Ready-to-assemble AI
 Author: Romlin Group AB
 Author-email: hello@romlin.com
 License: Apache Software License (Apache-2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
@@ -15,15 +15,14 @@
 Requires-Dist: ngrok==1.2.0
 Requires-Dist: nltk==3.8.1
 Requires-Dist: psutil==5.9.5
 Requires-Dist: pydantic==2.7.1
 Requires-Dist: pypdf==4.2.0
 Requires-Dist: requests==2.31.0
 Requires-Dist: sentence-transformers==2.7.0
-Requires-Dist: setuptools==70.0.0
 Requires-Dist: toml==0.10.2
 Requires-Dist: torch==2.3.0
 Requires-Dist: uvicorn==0.29.0
 
 # Flatpack
 
 **NOTE:** Flatpack is currently experimental. Please refrain from using it in production environments.
@@ -115,17 +114,14 @@
 
 - **[requests](https://pypi.org/project/requests/)**\
   Apache Software License (Apache 2.0) ([LICENSE](https://github.com/psf/requests/blob/main/LICENSE))
 
 - **[sentence-transformers](https://pypi.org/project/sentence-transformers/)**\
   Apache Software License (Apache License 2.0) ([LICENSE](https://github.com/UKPLab/sentence-transformers/blob/master/LICENSE))
 
-- **[setuptools](https://pypi.org/project/setuptools/)**\
-  MIT License ([LICENSE](https://github.com/pypa/setuptools/blob/main/LICENSE))
-
 - **[toml](https://pypi.org/project/toml/)**\
   MIT License (MIT) ([LICENSE](https://github.com/uiri/toml/blob/master/LICENSE))
 
 - **[torch](https://pypi.org/project/torch/)**\
   BSD License (BSD-3) ([LICENSE](https://github.com/pytorch/pytorch/blob/main/LICENSE))
 
 - **[uvicorn](https://pypi.org/project/uvicorn/)**\
```

### Comparing `flatpack-3.5.8/flatpack.egg-info/SOURCES.txt` & `flatpack-3.5.9/flatpack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flatpack-3.5.8/setup.py` & `flatpack-3.5.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="flatpack",
-    version="3.5.8",
+    version="3.5.9",
     license="Apache Software License (Apache-2.0)",
     packages=find_packages(),
     install_requires=[
         "beautifulsoup4==4.12.3",
         "fastapi==0.110.2",
         "hnswlib==0.8.0",
         "httpx==0.27.0",
@@ -17,15 +17,14 @@
         "ngrok==1.2.0",
         "nltk==3.8.1",
         "psutil==5.9.5",
         "pydantic==2.7.1",
         "pypdf==4.2.0",
         "requests==2.31.0",
         "sentence-transformers==2.7.0",
-        "setuptools==70.0.0",
         "toml==0.10.2",
         "torch==2.3.0",
         "uvicorn==0.29.0"
     ],
     author="Romlin Group AB",
     author_email="hello@romlin.com",
     description="Ready-to-assemble AI",
```

