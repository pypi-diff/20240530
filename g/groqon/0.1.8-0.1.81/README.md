# Comparing `tmp/groqon-0.1.8.tar.gz` & `tmp/groqon-0.1.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "groqon-0.1.8.tar", max compression
+gzip compressed data, was "groqon-0.1.81.tar", max compression
```

## Comparing `groqon-0.1.8.tar` & `groqon-0.1.81.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     3492 2024-05-22 13:47:15.279707 groqon-0.1.8/README.md
--rw-r--r--   0        0        0      270 2024-05-29 18:38:37.047706 groqon-0.1.8/groqon/__init__.py
--rw-r--r--   0        0        0        0 2024-05-22 12:01:28.521416 groqon-0.1.8/groqon/async_api/__init__.py
--rw-r--r--   0        0        0    21861 2024-05-30 07:12:34.776702 groqon-0.1.8/groqon/async_api/agroq.py
--rw-r--r--   0        0        0     8365 2024-05-29 18:39:08.757118 groqon-0.1.8/groqon/async_api/agroq_utils.py
--rw-r--r--   0        0        0       53 2024-05-22 13:13:35.662297 groqon-0.1.8/groqon/async_api/experimental/__init__.py
--rw-r--r--   0        0        0     1275 2024-05-22 13:22:45.285100 groqon-0.1.8/groqon/async_api/experimental/mock_api.py
--rw-r--r--   0        0        0     3419 2024-05-30 06:27:02.736663 groqon-0.1.8/groqon/element_selectors.py
--rw-r--r--   0        0        0     1573 2024-05-29 18:38:37.094694 groqon-0.1.8/groqon/groq_config.py
--rw-r--r--   0        0        0     1098 2024-05-29 18:38:37.068701 groqon-0.1.8/groqon/logger.py
--rw-r--r--   0        0        0     2292 2024-05-29 18:38:37.118688 groqon-0.1.8/groqon/parsing.py
--rw-r--r--   0        0        0        0 2024-05-22 12:01:37.983678 groqon-0.1.8/groqon/sync_api/__init__.py
--rw-r--r--   0        0        0     8887 2024-05-22 13:50:34.888728 groqon-0.1.8/groqon/sync_api/groq.py
--rw-r--r--   0        0        0     6976 2024-05-22 17:23:19.949054 groqon-0.1.8/groqon/sync_api/groq_utils.py
--rw-r--r--   0        0        0      154 2024-05-29 18:38:37.067701 groqon-0.1.8/groqon/utils.py
--rw-r--r--   0        0        0      468 2024-05-30 07:17:33.536262 groqon-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3889 1970-01-01 00:00:00.000000 groqon-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     3492 2024-05-22 13:47:15.279707 groqon-0.1.81/README.md
+-rw-r--r--   0        0        0      270 2024-05-29 18:38:37.047706 groqon-0.1.81/groqon/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 12:01:28.521416 groqon-0.1.81/groqon/async_api/__init__.py
+-rw-r--r--   0        0        0    21871 2024-05-30 07:20:21.500385 groqon-0.1.81/groqon/async_api/agroq.py
+-rw-r--r--   0        0        0     8365 2024-05-29 18:39:08.757118 groqon-0.1.81/groqon/async_api/agroq_utils.py
+-rw-r--r--   0        0        0       53 2024-05-22 13:13:35.662297 groqon-0.1.81/groqon/async_api/experimental/__init__.py
+-rw-r--r--   0        0        0     1275 2024-05-22 13:22:45.285100 groqon-0.1.81/groqon/async_api/experimental/mock_api.py
+-rw-r--r--   0        0        0     3419 2024-05-30 06:27:02.736663 groqon-0.1.81/groqon/element_selectors.py
+-rw-r--r--   0        0        0     1573 2024-05-29 18:38:37.094694 groqon-0.1.81/groqon/groq_config.py
+-rw-r--r--   0        0        0     1098 2024-05-29 18:38:37.068701 groqon-0.1.81/groqon/logger.py
+-rw-r--r--   0        0        0     2292 2024-05-29 18:38:37.118688 groqon-0.1.81/groqon/parsing.py
+-rw-r--r--   0        0        0        0 2024-05-22 12:01:37.983678 groqon-0.1.81/groqon/sync_api/__init__.py
+-rw-r--r--   0        0        0     8887 2024-05-22 13:50:34.888728 groqon-0.1.81/groqon/sync_api/groq.py
+-rw-r--r--   0        0        0     6976 2024-05-22 17:23:19.949054 groqon-0.1.81/groqon/sync_api/groq_utils.py
+-rw-r--r--   0        0        0      154 2024-05-29 18:38:37.067701 groqon-0.1.81/groqon/utils.py
+-rw-r--r--   0        0        0      469 2024-05-30 07:21:05.170652 groqon-0.1.81/pyproject.toml
+-rw-r--r--   0        0        0     3890 1970-01-01 00:00:00.000000 groqon-0.1.81/PKG-INFO
```

### Comparing `groqon-0.1.8/README.md` & `groqon-0.1.81/README.md`

 * *Files identical despite different names*

### Comparing `groqon-0.1.8/groqon/async_api/agroq.py` & `groqon-0.1.81/groqon/async_api/agroq.py`

 * *Files 0% similar despite different names*

```diff
@@ -675,21 +675,22 @@
     args = parser.parse_args()
 
     def check_headless(x):
         return x.lower().strip() == "true"
 
     headless = check_headless(args.headless)
 
-    asyncio.run(
+    out = asyncio.run(
         agroq(
             cookie_file=args.cookie_file,
             model_list=args.model,
             headless=headless,
             query_list=args.queries,
             save_dir=args.output_dir,
             system_prompt=args.system_prompt,
             print_output=True,
             temperature=args.temperature,
             max_tokens=args.max_tokens,
             n_workers=args.n_workers,
         )
     )
+
```

### Comparing `groqon-0.1.8/groqon/async_api/agroq_utils.py` & `groqon-0.1.81/groqon/async_api/agroq_utils.py`

 * *Files identical despite different names*

### Comparing `groqon-0.1.8/groqon/async_api/experimental/mock_api.py` & `groqon-0.1.81/groqon/async_api/experimental/mock_api.py`

 * *Files identical despite different names*

### Comparing `groqon-0.1.8/groqon/element_selectors.py` & `groqon-0.1.81/groqon/element_selectors.py`

 * *Files identical despite different names*

### Comparing `groqon-0.1.8/groqon/groq_config.py` & `groqon-0.1.81/groqon/groq_config.py`

 * *Files identical despite different names*

### Comparing `groqon-0.1.8/groqon/logger.py` & `groqon-0.1.81/groqon/logger.py`

 * *Files identical despite different names*

### Comparing `groqon-0.1.8/groqon/parsing.py` & `groqon-0.1.81/groqon/parsing.py`

 * *Files identical despite different names*

### Comparing `groqon-0.1.8/groqon/sync_api/groq.py` & `groqon-0.1.81/groqon/sync_api/groq.py`

 * *Files identical despite different names*

### Comparing `groqon-0.1.8/groqon/sync_api/groq_utils.py` & `groqon-0.1.81/groqon/sync_api/groq_utils.py`

 * *Files identical despite different names*

### Comparing `groqon-0.1.8/PKG-INFO` & `groqon-0.1.81/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: groqon
-Version: 0.1.8
+Version: 0.1.81
 Summary: Use Groq.com as llm
 Author: tikendraw
 Author-email: tikendraksahu1029@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

