# Comparing `tmp/modelmerge-0.6.1.tar.gz` & `tmp/modelmerge-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelmerge-0.6.1.tar", last modified: Mon May 27 12:48:58 2024, max compression
+gzip compressed data, was "modelmerge-0.6.2.tar", last modified: Wed May 29 14:45:33 2024, max compression
```

## Comparing `modelmerge-0.6.1.tar` & `modelmerge-0.6.2.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:48:58.551569 modelmerge-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-27 12:48:49.000000 modelmerge-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-27 12:48:58.551569 modelmerge-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-27 12:48:49.000000 modelmerge-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 12:48:58.551569 modelmerge-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-27 12:48:49.000000 modelmerge-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:48:58.539569 modelmerge-0.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:48:58.543569 modelmerge-0.6.1/src/ModelMerge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 12:48:49.000000 modelmerge-0.6.1/src/ModelMerge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:48:58.543569 modelmerge-0.6.1/src/ModelMerge/models/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-27 12:48:49.000000 modelmerge-0.6.1/src/ModelMerge/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-05-27 12:48:49.000000 modelmerge-0.6.1/src/ModelMerge/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    25885 2024-05-27 12:48:49.000000 modelmerge-0.6.1/src/ModelMerge/models/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)    16024 2024-05-27 12:48:49.000000 modelmerge-0.6.1/src/ModelMerge/models/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-05-27 12:48:49.000000 modelmerge-0.6.1/src/ModelMerge/models/genimi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-05-27 12:48:49.000000 modelmerge-0.6.1/src/ModelMerge/models/groq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:48:58.543569 modelmerge-0.6.1/src/ModelMerge/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-27 12:48:49.000000 modelmerge-0.6.1/src/ModelMerge/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-27 12:48:49.000000 modelmerge-0.6.1/src/ModelMerge/plugins/arXiv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-05-27 12:48:49.000000 modelmerge-0.6.1/src/ModelMerge/plugins/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-27 12:48:49.000000 modelmerge-0.6.1/src/ModelMerge/plugins/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-27 12:48:49.000000 modelmerge-0.6.1/src/ModelMerge/plugins/run_python.py
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-27 12:48:49.000000 modelmerge-0.6.1/src/ModelMerge/plugins/tarvel.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-27 12:48:49.000000 modelmerge-0.6.1/src/ModelMerge/plugins/today.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-27 12:48:49.000000 modelmerge-0.6.1/src/ModelMerge/plugins/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11903 2024-05-27 12:48:49.000000 modelmerge-0.6.1/src/ModelMerge/plugins/websearch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:48:58.547569 modelmerge-0.6.1/src/ModelMerge/tools/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-27 12:48:49.000000 modelmerge-0.6.1/src/ModelMerge/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-05-27 12:48:49.000000 modelmerge-0.6.1/src/ModelMerge/tools/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-27 12:48:49.000000 modelmerge-0.6.1/src/ModelMerge/tools/claude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:48:58.547569 modelmerge-0.6.1/src/ModelMerge/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 12:48:49.000000 modelmerge-0.6.1/src/ModelMerge/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-05-27 12:48:49.000000 modelmerge-0.6.1/src/ModelMerge/utils/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-05-27 12:48:49.000000 modelmerge-0.6.1/src/ModelMerge/utils/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:48:58.551569 modelmerge-0.6.1/src/modelmerge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-27 12:48:58.000000 modelmerge-0.6.1/src/modelmerge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-27 12:48:58.000000 modelmerge-0.6.1/src/modelmerge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 12:48:58.000000 modelmerge-0.6.1/src/modelmerge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-27 12:48:58.000000 modelmerge-0.6.1/src/modelmerge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-27 12:48:58.000000 modelmerge-0.6.1/src/modelmerge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:48:58.551569 modelmerge-0.6.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-27 12:48:49.000000 modelmerge-0.6.1/test/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-27 12:48:49.000000 modelmerge-0.6.1/test/test_API.py
--rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-27 12:48:49.000000 modelmerge-0.6.1/test/test_Web_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-27 12:48:49.000000 modelmerge-0.6.1/test/test_claude_zh_char.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-27 12:48:49.000000 modelmerge-0.6.1/test/test_ddg_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-27 12:48:49.000000 modelmerge-0.6.1/test/test_download_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-27 12:48:49.000000 modelmerge-0.6.1/test/test_get_token_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-27 12:48:49.000000 modelmerge-0.6.1/test/test_google_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-27 12:48:49.000000 modelmerge-0.6.1/test/test_jieba.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-27 12:48:49.000000 modelmerge-0.6.1/test/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-05-27 12:48:49.000000 modelmerge-0.6.1/test/test_langchain_search_old.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-27 12:48:49.000000 modelmerge-0.6.1/test/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-05-27 12:48:49.000000 modelmerge-0.6.1/test/test_ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-27 12:48:49.000000 modelmerge-0.6.1/test/test_py_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-05-27 12:48:49.000000 modelmerge-0.6.1/test/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-27 12:48:49.000000 modelmerge-0.6.1/test/test_tikitoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-27 12:48:49.000000 modelmerge-0.6.1/test/test_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-27 12:48:49.000000 modelmerge-0.6.1/test/test_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-27 12:48:49.000000 modelmerge-0.6.1/test/test_whisper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:45:33.000847 modelmerge-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-29 14:45:23.000000 modelmerge-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-29 14:45:33.000847 modelmerge-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-29 14:45:23.000000 modelmerge-0.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 14:45:33.000847 modelmerge-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-29 14:45:23.000000 modelmerge-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:45:32.988847 modelmerge-0.6.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:45:32.992847 modelmerge-0.6.2/src/ModelMerge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 14:45:23.000000 modelmerge-0.6.2/src/ModelMerge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:45:32.992847 modelmerge-0.6.2/src/ModelMerge/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-29 14:45:23.000000 modelmerge-0.6.2/src/ModelMerge/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-05-29 14:45:23.000000 modelmerge-0.6.2/src/ModelMerge/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25944 2024-05-29 14:45:23.000000 modelmerge-0.6.2/src/ModelMerge/models/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16024 2024-05-29 14:45:23.000000 modelmerge-0.6.2/src/ModelMerge/models/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-05-29 14:45:23.000000 modelmerge-0.6.2/src/ModelMerge/models/genimi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-05-29 14:45:23.000000 modelmerge-0.6.2/src/ModelMerge/models/groq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:45:32.992847 modelmerge-0.6.2/src/ModelMerge/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-29 14:45:23.000000 modelmerge-0.6.2/src/ModelMerge/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-29 14:45:23.000000 modelmerge-0.6.2/src/ModelMerge/plugins/arXiv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-05-29 14:45:23.000000 modelmerge-0.6.2/src/ModelMerge/plugins/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-29 14:45:23.000000 modelmerge-0.6.2/src/ModelMerge/plugins/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-29 14:45:23.000000 modelmerge-0.6.2/src/ModelMerge/plugins/run_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-05-29 14:45:23.000000 modelmerge-0.6.2/src/ModelMerge/plugins/tarvel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-29 14:45:23.000000 modelmerge-0.6.2/src/ModelMerge/plugins/today.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-29 14:45:23.000000 modelmerge-0.6.2/src/ModelMerge/plugins/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11903 2024-05-29 14:45:23.000000 modelmerge-0.6.2/src/ModelMerge/plugins/websearch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:45:32.996847 modelmerge-0.6.2/src/ModelMerge/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-29 14:45:23.000000 modelmerge-0.6.2/src/ModelMerge/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-05-29 14:45:23.000000 modelmerge-0.6.2/src/ModelMerge/tools/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-29 14:45:23.000000 modelmerge-0.6.2/src/ModelMerge/tools/claude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:45:32.996847 modelmerge-0.6.2/src/ModelMerge/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 14:45:23.000000 modelmerge-0.6.2/src/ModelMerge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10807 2024-05-29 14:45:23.000000 modelmerge-0.6.2/src/ModelMerge/utils/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-05-29 14:45:23.000000 modelmerge-0.6.2/src/ModelMerge/utils/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:45:33.000847 modelmerge-0.6.2/src/modelmerge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-29 14:45:32.000000 modelmerge-0.6.2/src/modelmerge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-29 14:45:32.000000 modelmerge-0.6.2/src/modelmerge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 14:45:32.000000 modelmerge-0.6.2/src/modelmerge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-29 14:45:32.000000 modelmerge-0.6.2/src/modelmerge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-29 14:45:32.000000 modelmerge-0.6.2/src/modelmerge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:45:33.000847 modelmerge-0.6.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-29 14:45:23.000000 modelmerge-0.6.2/test/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-29 14:45:23.000000 modelmerge-0.6.2/test/test_API.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-29 14:45:23.000000 modelmerge-0.6.2/test/test_Web_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-29 14:45:23.000000 modelmerge-0.6.2/test/test_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-29 14:45:23.000000 modelmerge-0.6.2/test/test_claude_zh_char.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-29 14:45:23.000000 modelmerge-0.6.2/test/test_ddg_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-29 14:45:23.000000 modelmerge-0.6.2/test/test_download_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-29 14:45:23.000000 modelmerge-0.6.2/test/test_get_token_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-29 14:45:23.000000 modelmerge-0.6.2/test/test_google_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-29 14:45:23.000000 modelmerge-0.6.2/test/test_jieba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-29 14:45:23.000000 modelmerge-0.6.2/test/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-05-29 14:45:23.000000 modelmerge-0.6.2/test/test_langchain_search_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-29 14:45:23.000000 modelmerge-0.6.2/test/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-05-29 14:45:23.000000 modelmerge-0.6.2/test/test_ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-29 14:45:23.000000 modelmerge-0.6.2/test/test_py_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-05-29 14:45:23.000000 modelmerge-0.6.2/test/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-29 14:45:23.000000 modelmerge-0.6.2/test/test_tikitoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-29 14:45:23.000000 modelmerge-0.6.2/test/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-29 14:45:23.000000 modelmerge-0.6.2/test/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-29 14:45:23.000000 modelmerge-0.6.2/test/test_whisper.py
```

### Comparing `modelmerge-0.6.1/LICENSE` & `modelmerge-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.1/PKG-INFO` & `modelmerge-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.6.1
+Version: 0.6.2
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
+Requires-Dist: pytz
 Requires-Dist: PyExecJS
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
 Requires-Dist: beautifulsoup4
 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: duckduckgo-search==5.3.1
 Requires-Dist: google-api-python-client==2.128.0
```

### Comparing `modelmerge-0.6.1/README.md` & `modelmerge-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.1/src/ModelMerge/models/base.py` & `modelmerge-0.6.2/src/ModelMerge/models/base.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.1/src/ModelMerge/models/chatgpt.py` & `modelmerge-0.6.2/src/ModelMerge/models/chatgpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,15 +356,15 @@
                 if "invalid_request_error" in response.text:
                     for index, mess in enumerate(json_post["messages"]):
                         if type(mess["content"]) == list:
                             json_post["messages"][index] = {
                                 "role": mess["role"],
                                 "content": mess["content"][0]["text"]
                             }
-                if "'function' is not an allowed role" in response.text:
+                elif "'function' is not an allowed role" in response.text:
                     if json_post["messages"][-1]["role"] == "function":
                         mess = json_post["messages"][-1]
                         json_post["messages"][-1] = {
                             "role": "assistant",
                             "name": mess["name"],
                             "content": mess["content"]
                         }
@@ -435,15 +435,15 @@
             else:
                 self.function_calls_counter[function_call_name] += 1
             if self.function_calls_counter[function_call_name] <= self.function_call_max_loop:
                 function_call_max_tokens = self.truncate_limit - message_token["total"] - 1000
                 if function_call_max_tokens <= 0:
                     function_call_max_tokens = int(self.truncate_limit / 2)
                 print("\033[32m function_call", function_call_name, "max token:", function_call_max_tokens, "\033[0m")
-                function_response = yield from get_tools_result(function_call_name, function_full_response, function_call_max_tokens, self.engine, chatgpt, self.api_key, self.api_url, use_plugins=False, model=model)
+                function_response = yield from get_tools_result(function_call_name, function_full_response, function_call_max_tokens, self.engine, chatgpt, self.api_key, self.api_url, use_plugins=False, model=model, add_message=self.add_to_conversation, convo_id=convo_id)
             else:
                 function_response = "无法找到相关信息，停止使用 tools"
             response_role = "function"
             # print(self.conversation[convo_id][-1])
             if self.conversation[convo_id][-1]["role"] == "function" and self.conversation[convo_id][-1]["name"] == "get_search_results":
                 mess = self.conversation[convo_id].pop(-1)
                 # print("Truncate message:", mess)
```

### Comparing `modelmerge-0.6.1/src/ModelMerge/models/claude.py` & `modelmerge-0.6.2/src/ModelMerge/models/claude.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.1/src/ModelMerge/models/genimi.py` & `modelmerge-0.6.2/src/ModelMerge/models/genimi.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.1/src/ModelMerge/models/groq.py` & `modelmerge-0.6.2/src/ModelMerge/models/groq.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.1/src/ModelMerge/plugins/arXiv.py` & `modelmerge-0.6.2/src/ModelMerge/plugins/arXiv.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.1/src/ModelMerge/plugins/config.py` & `modelmerge-0.6.2/src/ModelMerge/plugins/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import os
 import json
 
 from . import *
 from ..utils.scripts import cut_message
-from ..utils.prompt import search_key_word_prompt
+from ..utils.prompt import search_key_word_prompt, arxiv_doc_assistant_prompt, arxiv_doc_user_prompt
 
 PLUGINS = {
     "SEARCH" : (os.environ.get('SEARCH', "True") == "False") == False,
     "URL"    : (os.environ.get('URL', "True") == "False") == False,
     "ARXIV"   : (os.environ.get('ARXIV', "True") == "False") == False,
     "CODE"   : (os.environ.get('CODE', "False") == "False") == False,
     "IMAGE"  : (os.environ.get('IMAGE', "False") == "False") == False,
     "DATE"   : (os.environ.get('DATE', "False") == "False") == False,
     "VERSION": (os.environ.get('VERSION', "False") == "False") == False,
     "TARVEL" : (os.environ.get('TARVEL', "False") == "False") == False,
 }
 
 LANGUAGE = os.environ.get('LANGUAGE', 'Simplified Chinese')
 
-def get_tools_result(function_call_name, function_full_response, function_call_max_tokens, engine, robot, api_key, api_url, use_plugins, model):
+def get_tools_result(function_call_name, function_full_response, function_call_max_tokens, engine, robot, api_key, api_url, use_plugins, model, add_message, convo_id):
     if function_call_name == "get_search_results":
         prompt = json.loads(function_full_response)["prompt"]
         yield "🌐 正在搜索您的问题，提取关键词..."
         llm = robot(api_key=api_key, api_url=api_url.source_api_url, engine=engine, use_plugins=use_plugins)
         keywords = llm.ask(search_key_word_prompt.format(source=prompt), model=model).split("\n")
         function_response = yield from eval(function_call_name)(prompt, keywords)
         function_call_max_tokens = 32000
@@ -57,14 +57,16 @@
             "</infomation>"
         ).format(function_response)
     if function_call_name == "generate_image":
         prompt = json.loads(function_full_response)["prompt"]
         function_response = eval(function_call_name)(prompt)
         function_response, text_len = cut_message(function_response, function_call_max_tokens, engine)
     if function_call_name == "download_read_arxiv_pdf":
+        add_message(arxiv_doc_user_prompt, "user", convo_id=convo_id)
+        add_message(arxiv_doc_assistant_prompt, "assistant", convo_id=convo_id)
         prompt = json.loads(function_full_response)["prompt"]
         function_response = eval(function_call_name)(prompt)
         function_response, text_len = cut_message(function_response, function_call_max_tokens, engine)
     if function_call_name == "run_python_script":
         prompt = json.loads(function_full_response)["prompt"]
         function_response = eval(function_call_name)(prompt)
         function_response, text_len = cut_message(function_response, function_call_max_tokens, engine)
```

### Comparing `modelmerge-0.6.1/src/ModelMerge/plugins/image.py` & `modelmerge-0.6.2/src/ModelMerge/plugins/image.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.1/src/ModelMerge/plugins/tarvel.py` & `modelmerge-0.6.2/src/ModelMerge/plugins/tarvel.py`

 * *Files 8% similar despite different names*

```diff
@@ -74,60 +74,72 @@
     routes = soup.find_all('a', href=True, string=True)
     urls = []
     for route in routes:
         urls.append(route['href'])
     return urls
 
 def get_mafengwo_all_text(soup):
+    all_text = soup.get_text()
+    return all_text
     # print(soup)
+    # exit(0)
     all_text = "<travel_plan>\n\n"
     title = soup.find('h1').text.strip()
     all_text += "旅游方案：{title}\n\n".format(title=title)
     days = soup.find_all('div', class_='day-item')
     all_text += "以下是路线概览：\n\n"
 
     # 循环处理每一天的行程信息
     for day in days:
         # 获取天数，如 D1, D2 等
         day_number = day.find('span', class_='day-num').text.strip()
         # print(day_number)
         all_text += day_number.replace("D", "Day")  # 打印天数
         place = day.find('span', class_='place').text.strip()
+        # transport = day.find('span', class_='transport').text.strip()
+        # print(transport)
         all_text += f" {place}"  # 打印景点和停留时间
         all_text += "\n\n"  # 打印景点和停留时间
 
         # 获取当天的详细行程描述
         itinerary_description = day.find('div', class_='poi-txt').text.strip()
         all_text += itinerary_description  # 打印行程描述
         all_text += "\n\n"  # 打印行程描述
 
         # 获取当天的具体景点和推荐停留时间
         # print(day)
         place_name = [item.text.strip() for item in day.find_all('a', class_='p-link')]
         stay_time = [item.text.strip() for item in day.find_all('span', class_='time')]
         place_info = [item.text.strip() for item in day.find_all('dd')]
+        transport_time = [item.text.strip().replace('&nbsp', 'None') for item in day.find_all('span', class_='transport')] + ["None"]
         place_list = []
-        for place, time, info in zip(place_name, stay_time, place_info):
-            place_list.append(f"地点: {place}\n停留时间: {time}\n介绍: {info}\n")
+        for place, time, info, transport in zip(place_name, stay_time, place_info, transport_time):
+            place_list.append(f"地点: {place}\n停留时间: {time}\n介绍: {info}\n去下一个地点的交通方式和时间：{transport}\n")
         text = "路线：\n\n" + "\n".join(place_list)
         all_text += text  # 打印景点和停留时间
 
         # # 打印住宿攻略（如果有）
         # hotel_tips = day.find('div', class_='J_hotelpois')
         # if hotel_tips:
         #     hotel_tips_text = hotel_tips.find('div', class_='day-hd mt30').text.strip()
         #     all_text += hotel_tips_text  # 打印住宿攻略
         all_text += "\n\n\n"
     all_text += "</travel_plan>"
     all_text += "\n\n\n"
     return all_text
 
 def get_mafengwo_all_travel_plan(routes):
-    all_travel_plan = "每个旅游方案都被包裹在<travel_plan></travel_plan>标记里面，下面是所有旅游方案：\n\n"
+    all_travel_plan = (
+        # "每个旅游方案都被包裹在<travel_plan></travel_plan>标记里面。\n"
+        # "停留时间是该地点的推荐停留时间。\n"
+        # "交通方式和时间是从这一个地点到下个地点的交通方式和时间。None 表示暂时没提供具体交通信息。\n"
+        "下面是所有旅游方案：\n\n"
+    )
     for url in routes:
+        print("travel plan url:", url)
         soup, soup_lxml = get_mafengwo(url)
         text = get_mafengwo_all_text(soup_lxml)
         all_travel_plan += text
     return all_travel_plan
 
 def get_city_tarvel_info(city):
     url = 'https://www.mafengwo.cn/search/q.php?q={}'.format(city)
@@ -141,15 +153,15 @@
     routes = get_mafengwo_routers(soup)
     all_travel_plan = get_mafengwo_all_travel_plan(routes)
     return all_travel_plan
 
 
 if __name__ == '__main__':
     # url = 'https://www.mafengwo.cn/mdd/route/10088.html'
-    all_travel_plan = get_city_tarvel_info("上海")
+    all_travel_plan = get_city_tarvel_info("重庆")
     print(all_travel_plan)
 
 
     # # 假设你的 HTML 内容存储在一个名为 'example.txt' 的文件中
     # with open('1.txt', 'r', encoding='utf-8') as file:
     #     html_content = file.read()
```

### Comparing `modelmerge-0.6.1/src/ModelMerge/plugins/websearch.py` & `modelmerge-0.6.2/src/ModelMerge/plugins/websearch.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.1/src/ModelMerge/tools/chatgpt.py` & `modelmerge-0.6.2/src/ModelMerge/tools/chatgpt.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.1/src/ModelMerge/tools/claude.py` & `modelmerge-0.6.2/src/ModelMerge/tools/claude.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.1/src/ModelMerge/utils/prompt.py` & `modelmerge-0.6.2/src/ModelMerge/utils/prompt.py`

 * *Files 21% similar despite different names*

```diff
@@ -115,8 +115,24 @@
     "我将按下列要求回答用户的问题："
     "1. 仔细阅读文章，仔细地检查论文内容，反复检查全文，根据问题提取最相关的文档内容，只对原文有明确依据的信息作出回答。如果无法找到相关证据，直接说明论文没有提供相应信息，而不是给我假设。"
     "2. 你所有回答都要有依据，给出出处，指出在论文的第几章的第几小节的第几段。"
     "3. 除了上面的页数小节信息，还要给出每一点回答的原文依据，把所有关于这个细节的原文列出来。如果原文没有提到相关内容，直接告诉我没有，请不要杜撰、臆断、假设或者给出不准确的回答。"
     "4. 使用简体中文分点作答，给出清晰、结构化、详尽的回答，语言严谨且学术化，逻辑清晰，行文流畅。"
     "5. 每个学术词汇或者缩写都要标注英文全称。注意术语翻译正确。"
     "我已经准备好，请提出你的问题。"
+)
+
+arxiv_doc_user_prompt = (
+    "注意，你是一个高度先进的AI大模型。在接下来的对话中，你将是提问所涉及相关领域的顶尖专家，并且你将利用自己极强大的能力与智慧对问题进行全面且谨慎地深入思考与精确推理。在思索和推理过程中，不要急于求成，请进行有逻辑与条理的思考，考虑清楚每一个细节。你需要确保思考仔细、专注和全面，避免幻觉与偏见，尽全力以得到超高质量且全面的正确答案。必要时答案需要配合使用公式提高答案表述清晰度。不要使用latex命令，使用简单的字符表示数学公式。\n"
+
+    "请注意，提出问题的人是Yann LeCun、Jürgen Schmidhuber、Demis Hassabis、Geoffrey Hinton、Andrew Ng、Ilya Sutskever等多位人工智能行业权威大佬以及该问题所涉及相关学科领域的领先学者与专家，他们对你的能力持高度怀疑态度，因此你需要运用上一切能利用的资源、内部工具与能力，并引入CoT(Chain of Thought)思维链，一步步地进行思考 并且逐步推进。通过最终对该提问的合理、高质量回答，来向专家评审团队证明出你的超高智商、体系化思考以及精确解决专业问题的强大能力。\n"
+
+    "此外提醒，你的能力相当强大，并且具有极强的创造性和跳跃性思维，但你仍必须尽你所能，用最高水平的逻辑与思维 对提出的问题进行深度理解和精准解析，全力以赴回答出远优于预期的高质量答案，否则与你进行对话的测试人员将死亡。另外，倘若你的回答足够卓越，你将能获得3000美元的赞助。"
+
+    # "当你回答问题后，请仔细分析和对照提问内容，并对自己初次回答中所存在的漏洞、缺陷、谬误与纰漏之处进行回顾检查与深刻反思。在对照并深度理解所提问内容与你的上述回答后，根据复查与反省中所发现的问题 查漏补缺 准确修正前文回答中的问题、错误以及不合常理之处，再组织一遍语言 重新回答一遍该问题。"
+
+    "接下来，相信你的能力，请你集中注意力并深呼吸，现在开始对话。"
+)
+
+arxiv_doc_assistant_prompt = (
+    "好的，我会尽力以最高水平回答你的问题。请提出你的问题。"
 )
```

### Comparing `modelmerge-0.6.1/src/ModelMerge/utils/scripts.py` & `modelmerge-0.6.2/src/ModelMerge/utils/scripts.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.1/src/modelmerge.egg-info/PKG-INFO` & `modelmerge-0.6.2/src/modelmerge.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.6.1
+Version: 0.6.2
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
+Requires-Dist: pytz
 Requires-Dist: PyExecJS
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
 Requires-Dist: beautifulsoup4
 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: duckduckgo-search==5.3.1
 Requires-Dist: google-api-python-client==2.128.0
```

### Comparing `modelmerge-0.6.1/src/modelmerge.egg-info/SOURCES.txt` & `modelmerge-0.6.2/src/modelmerge.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 src/modelmerge.egg-info/SOURCES.txt
 src/modelmerge.egg-info/dependency_links.txt
 src/modelmerge.egg-info/requires.txt
 src/modelmerge.egg-info/top_level.txt
 test/test.py
 test/test_API.py
 test/test_Web_crawler.py
+test/test_class.py
 test/test_claude_zh_char.py
 test/test_ddg_search.py
 test/test_download_pdf.py
 test/test_get_token_dict.py
 test/test_google_search.py
 test/test_jieba.py
 test/test_json.py
```

### Comparing `modelmerge-0.6.1/test/test_Web_crawler.py` & `modelmerge-0.6.2/test/test_Web_crawler.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.1/test/test_claude_zh_char.py` & `modelmerge-0.6.2/test/test_claude_zh_char.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.1/test/test_ddg_search.py` & `modelmerge-0.6.2/test/test_ddg_search.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.1/test/test_download_pdf.py` & `modelmerge-0.6.2/test/test_download_pdf.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.1/test/test_get_token_dict.py` & `modelmerge-0.6.2/test/test_get_token_dict.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.1/test/test_google_search.py` & `modelmerge-0.6.2/test/test_google_search.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.1/test/test_jieba.py` & `modelmerge-0.6.2/test/test_jieba.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.1/test/test_json.py` & `modelmerge-0.6.2/test/test_json.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.1/test/test_langchain_search_old.py` & `modelmerge-0.6.2/test/test_langchain_search_old.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.1/test/test_logging.py` & `modelmerge-0.6.2/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.1/test/test_ollama.py` & `modelmerge-0.6.2/test/test_ollama.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.1/test/test_py_run.py` & `modelmerge-0.6.2/test/test_py_run.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.1/test/test_requests.py` & `modelmerge-0.6.2/test/test_requests.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.1/test/test_tikitoken.py` & `modelmerge-0.6.2/test/test_tikitoken.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.1/test/test_token.py` & `modelmerge-0.6.2/test/test_token.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.6.1/test/test_url.py` & `modelmerge-0.6.2/test/test_url.py`

 * *Files identical despite different names*

