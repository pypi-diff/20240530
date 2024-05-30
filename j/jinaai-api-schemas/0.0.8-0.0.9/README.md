# Comparing `tmp/jinaai_api_schemas-0.0.8.tar.gz` & `tmp/jinaai_api_schemas-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinaai_api_schemas-0.0.8.tar", last modified: Mon Dec  4 14:04:54 2023, max compression
+gzip compressed data, was "jinaai_api_schemas-0.0.9.tar", last modified: Tue Dec 19 14:14:23 2023, max compression
```

## Comparing `jinaai_api_schemas-0.0.8.tar` & `jinaai_api_schemas-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 14:04:54.647093 jinaai_api_schemas-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      956 2023-12-04 14:04:54.647093 jinaai_api_schemas-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      122 2023-12-04 14:04:45.000000 jinaai_api_schemas-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 14:04:54.647093 jinaai_api_schemas-0.0.8/api_schemas/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-04 14:04:45.000000 jinaai_api_schemas-0.0.8/api_schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2023-12-04 14:04:45.000000 jinaai_api_schemas-0.0.8/api_schemas/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2023-12-04 14:04:45.000000 jinaai_api_schemas-0.0.8/api_schemas/embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 14:04:54.647093 jinaai_api_schemas-0.0.8/jinaai_api_schemas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      956 2023-12-04 14:04:54.000000 jinaai_api_schemas-0.0.8/jinaai_api_schemas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      352 2023-12-04 14:04:54.000000 jinaai_api_schemas-0.0.8/jinaai_api_schemas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-04 14:04:54.000000 jinaai_api_schemas-0.0.8/jinaai_api_schemas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-04 14:04:54.000000 jinaai_api_schemas-0.0.8/jinaai_api_schemas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-12-04 14:04:54.000000 jinaai_api_schemas-0.0.8/jinaai_api_schemas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-04 14:04:54.000000 jinaai_api_schemas-0.0.8/jinaai_api_schemas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      206 2023-12-04 14:04:45.000000 jinaai_api_schemas-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-04 14:04:54.647093 jinaai_api_schemas-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2023-12-04 14:04:45.000000 jinaai_api_schemas-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 14:14:23.250923 jinaai_api_schemas-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2023-12-19 14:14:23.250923 jinaai_api_schemas-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2023-12-19 14:14:13.000000 jinaai_api_schemas-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 14:14:23.250923 jinaai_api_schemas-0.0.9/api_schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-19 14:14:13.000000 jinaai_api_schemas-0.0.9/api_schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2023-12-19 14:14:13.000000 jinaai_api_schemas-0.0.9/api_schemas/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2023-12-19 14:14:13.000000 jinaai_api_schemas-0.0.9/api_schemas/embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 14:14:23.250923 jinaai_api_schemas-0.0.9/jinaai_api_schemas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2023-12-19 14:14:23.000000 jinaai_api_schemas-0.0.9/jinaai_api_schemas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2023-12-19 14:14:23.000000 jinaai_api_schemas-0.0.9/jinaai_api_schemas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-19 14:14:23.000000 jinaai_api_schemas-0.0.9/jinaai_api_schemas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-19 14:14:23.000000 jinaai_api_schemas-0.0.9/jinaai_api_schemas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2023-12-19 14:14:23.000000 jinaai_api_schemas-0.0.9/jinaai_api_schemas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-19 14:14:23.000000 jinaai_api_schemas-0.0.9/jinaai_api_schemas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2023-12-19 14:14:13.000000 jinaai_api_schemas-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-19 14:14:23.250923 jinaai_api_schemas-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2023-12-19 14:14:13.000000 jinaai_api_schemas-0.0.9/setup.py
```

### Comparing `jinaai_api_schemas-0.0.8/PKG-INFO` & `jinaai_api_schemas-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinaai_api_schemas
-Version: 0.0.8
+Version: 0.0.9
 Summary: The schemas for the Jina Serving API
 Download-URL: https://github.com/jina-ai/embedding-api-schemas/tags
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Proprietary
 Project-URL: Source, https://github.com/jina-ai/embedding-api-schemas.fit/
 Project-URL: Tracker, https://github.com/jina-ai/embedding-api-schemas/issues
```

### Comparing `jinaai_api_schemas-0.0.8/api_schemas/base.py` & `jinaai_api_schemas-0.0.9/api_schemas/base.py`

 * *Files identical despite different names*

### Comparing `jinaai_api_schemas-0.0.8/api_schemas/embedding.py` & `jinaai_api_schemas-0.0.9/api_schemas/embedding.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Union, Optional
 
 from docarray import BaseDoc, DocList
 from docarray.base_doc.doc import BaseDocWithoutId
 from docarray.typing import NdArray
 from docarray.typing.url import ImageUrl
 from docarray.typing.bytes import ImageBytes
-from pydantic import Field, BaseModel, validator
+from pydantic import Field, BaseModel
 
 from api_schemas.base import BaseInputModel
 
 
 class ExecutorUsage(BaseDoc):
     """The usage of the embedding services to report, e.g. number of tokens in case of text input"""
 
@@ -24,20 +24,19 @@
     """Document containing a text field"""
 
     text: str
 
 
 class ImageDoc(BaseDoc):
     url: Optional[ImageUrl] = Field(
-        description='URL to a (potentially remote) image file that needs to be loaded',
-        example='https://github.com/docarray/docarray/blob/main/tests/toydata/image-data/apple.png?raw=true',
+        description='URL of an image file',
         default=None,
     )
     bytes: Optional[ImageBytes] = Field(
-        description='Bytes object of the image which is an instance of `ImageBytes`.',
+        description='Bytes representation of the Image.',
         default=None,
     )
 
 
 ## Model to be imported by the Executor and used by the Universal API to communicate with it
 class EmbeddingDoc(BaseDoc):
     """Document to be returned by the embedding backend, containing the embedding vector and the token usage for the
```

### Comparing `jinaai_api_schemas-0.0.8/jinaai_api_schemas.egg-info/PKG-INFO` & `jinaai_api_schemas-0.0.9/jinaai_api_schemas.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinaai-api-schemas
-Version: 0.0.8
+Version: 0.0.9
 Summary: The schemas for the Jina Serving API
 Download-URL: https://github.com/jina-ai/embedding-api-schemas/tags
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Proprietary
 Project-URL: Source, https://github.com/jina-ai/embedding-api-schemas.fit/
 Project-URL: Tracker, https://github.com/jina-ai/embedding-api-schemas/issues
```

### Comparing `jinaai_api_schemas-0.0.8/setup.py` & `jinaai_api_schemas-0.0.9/setup.py`

 * *Files identical despite different names*

