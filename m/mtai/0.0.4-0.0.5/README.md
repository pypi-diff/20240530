# Comparing `tmp/mtai-0.0.4.tar.gz` & `tmp/mtai-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtai-0.0.4.tar", last modified: Sun May 26 10:24:45 2024, max compression
+gzip compressed data, was "mtai-0.0.5.tar", last modified: Thu May 30 11:00:30 2024, max compression
```

## Comparing `mtai-0.0.4.tar` & `mtai-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:24:45.440832 mtai-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-26 10:24:19.000000 mtai-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-26 10:24:45.440832 mtai-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-26 10:24:19.000000 mtai-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:24:45.440832 mtai-0.0.4/mtai/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-26 10:24:19.000000 mtai-0.0.4/mtai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-26 10:24:19.000000 mtai-0.0.4/mtai/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-26 10:24:19.000000 mtai-0.0.4/mtai/mt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-26 10:24:19.000000 mtai-0.0.4/mtai/prompts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-26 10:24:19.000000 mtai-0.0.4/mtai/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:24:45.440832 mtai-0.0.4/mtai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-26 10:24:45.000000 mtai-0.0.4/mtai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-26 10:24:45.000000 mtai-0.0.4/mtai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 10:24:45.000000 mtai-0.0.4/mtai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-26 10:24:45.000000 mtai-0.0.4/mtai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-26 10:24:45.000000 mtai-0.0.4/mtai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 10:24:45.440832 mtai-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-26 10:24:19.000000 mtai-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:00:30.181835 mtai-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-30 11:00:10.000000 mtai-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-30 11:00:30.181835 mtai-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-30 11:00:10.000000 mtai-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:00:30.181835 mtai-0.0.5/mtai/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-30 11:00:10.000000 mtai-0.0.5/mtai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-30 11:00:10.000000 mtai-0.0.5/mtai/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-30 11:00:10.000000 mtai-0.0.5/mtai/mt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-30 11:00:10.000000 mtai-0.0.5/mtai/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-30 11:00:10.000000 mtai-0.0.5/mtai/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:00:30.181835 mtai-0.0.5/mtai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-30 11:00:30.000000 mtai-0.0.5/mtai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-30 11:00:30.000000 mtai-0.0.5/mtai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 11:00:30.000000 mtai-0.0.5/mtai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-30 11:00:30.000000 mtai-0.0.5/mtai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-30 11:00:30.000000 mtai-0.0.5/mtai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 11:00:30.181835 mtai-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-30 11:00:10.000000 mtai-0.0.5/setup.py
```

### Comparing `mtai-0.0.4/LICENSE` & `mtai-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mtai-0.0.4/PKG-INFO` & `mtai-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtai
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python library to consume meditranscribe ai API
 Home-page: https://github.com/mediatranscribe/mt-ai-python
 Author: KtechHub
 Author-email: pypi@ktechhub.com
 License: MIT
 Keywords: mtai mediatranscribe mtaiapi python library
 Classifier: Intended Audience :: Developers
@@ -31,15 +31,15 @@
 ```python
 from mtai.mt import MT
 secret_key = "secret_key_here"
 mt = MT(secret_key=secret_key)
 print(mt.tags.list())
 print(mt.tags.create_from_title(title="Python Programming Language"))
 print(mt.tags.create_from_title_summary("Python", "Python is a programming language"))
-print(mt.tags.get_tab_by_id("664e033837511b57fa93dd2e"))
+print(mt.tags.get_tag_by_id("664e033837511b57fa93dd2e"))
 print(mt.tags.delete_tag_by_id("664e033837511b57fa93dd2e"))
 ```
 
 ### Tags Static Use
 To start using the MTAI Python API, you need to start by setting your secret key.
 
 You can set your secret key in your environment by running:
```

### Comparing `mtai-0.0.4/README.md` & `mtai-0.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 ```python
 from mtai.mt import MT
 secret_key = "secret_key_here"
 mt = MT(secret_key=secret_key)
 print(mt.tags.list())
 print(mt.tags.create_from_title(title="Python Programming Language"))
 print(mt.tags.create_from_title_summary("Python", "Python is a programming language"))
-print(mt.tags.get_tab_by_id("664e033837511b57fa93dd2e"))
+print(mt.tags.get_tag_by_id("664e033837511b57fa93dd2e"))
 print(mt.tags.delete_tag_by_id("664e033837511b57fa93dd2e"))
 ```
 
 ### Tags Static Use
 To start using the MTAI Python API, you need to start by setting your secret key.
 
 You can set your secret key in your environment by running:
```

### Comparing `mtai-0.0.4/mtai/base.py` & `mtai-0.0.5/mtai/base.py`

 * *Files identical despite different names*

### Comparing `mtai-0.0.4/mtai/prompts.py` & `mtai-0.0.5/mtai/prompts.py`

 * *Files identical despite different names*

### Comparing `mtai-0.0.4/mtai/tags.py` & `mtai-0.0.5/mtai/tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         """
         return cls().requests.post(
             "/tags/create-tags-from-title-summary",
             data={"title": title, "summary": summary, "count": count},
         )
 
     @classmethod
-    def get_tab_by_id(cls, tag_id):
+    def get_tag_by_id(cls, tag_id):
         """
         Get a tag by id.
         Args:
             tag_id: str
         Returns:
             JSON Response
         """
```

### Comparing `mtai-0.0.4/mtai.egg-info/PKG-INFO` & `mtai-0.0.5/mtai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtai
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python library to consume meditranscribe ai API
 Home-page: https://github.com/mediatranscribe/mt-ai-python
 Author: KtechHub
 Author-email: pypi@ktechhub.com
 License: MIT
 Keywords: mtai mediatranscribe mtaiapi python library
 Classifier: Intended Audience :: Developers
@@ -31,15 +31,15 @@
 ```python
 from mtai.mt import MT
 secret_key = "secret_key_here"
 mt = MT(secret_key=secret_key)
 print(mt.tags.list())
 print(mt.tags.create_from_title(title="Python Programming Language"))
 print(mt.tags.create_from_title_summary("Python", "Python is a programming language"))
-print(mt.tags.get_tab_by_id("664e033837511b57fa93dd2e"))
+print(mt.tags.get_tag_by_id("664e033837511b57fa93dd2e"))
 print(mt.tags.delete_tag_by_id("664e033837511b57fa93dd2e"))
 ```
 
 ### Tags Static Use
 To start using the MTAI Python API, you need to start by setting your secret key.
 
 You can set your secret key in your environment by running:
```

### Comparing `mtai-0.0.4/setup.py` & `mtai-0.0.5/setup.py`

 * *Files identical despite different names*

