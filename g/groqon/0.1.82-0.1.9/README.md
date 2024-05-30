# Comparing `tmp/groqon-0.1.82.tar.gz` & `tmp/groqon-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "groqon-0.1.82.tar", max compression
+gzip compressed data, was "groqon-0.1.9.tar", max compression
```

## Comparing `groqon-0.1.82.tar` & `groqon-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     3492 2024-05-22 13:47:15.279707 groqon-0.1.82/README.md
--rw-r--r--   0        0        0      270 2024-05-29 18:38:37.047706 groqon-0.1.82/groqon/__init__.py
--rw-r--r--   0        0        0        0 2024-05-22 12:01:28.521416 groqon-0.1.82/groqon/async_api/__init__.py
--rw-r--r--   0        0        0    21845 2024-05-30 07:25:48.542007 groqon-0.1.82/groqon/async_api/agroq.py
--rw-r--r--   0        0        0     8365 2024-05-29 18:39:08.757118 groqon-0.1.82/groqon/async_api/agroq_utils.py
--rw-r--r--   0        0        0       53 2024-05-22 13:13:35.662297 groqon-0.1.82/groqon/async_api/experimental/__init__.py
--rw-r--r--   0        0        0     1275 2024-05-22 13:22:45.285100 groqon-0.1.82/groqon/async_api/experimental/mock_api.py
--rw-r--r--   0        0        0     3419 2024-05-30 06:27:02.736663 groqon-0.1.82/groqon/element_selectors.py
--rw-r--r--   0        0        0     1573 2024-05-29 18:38:37.094694 groqon-0.1.82/groqon/groq_config.py
--rw-r--r--   0        0        0     1098 2024-05-29 18:38:37.068701 groqon-0.1.82/groqon/logger.py
--rw-r--r--   0        0        0     2292 2024-05-29 18:38:37.118688 groqon-0.1.82/groqon/parsing.py
--rw-r--r--   0        0        0        0 2024-05-22 12:01:37.983678 groqon-0.1.82/groqon/sync_api/__init__.py
--rw-r--r--   0        0        0     8887 2024-05-22 13:50:34.888728 groqon-0.1.82/groqon/sync_api/groq.py
--rw-r--r--   0        0        0     6976 2024-05-22 17:23:19.949054 groqon-0.1.82/groqon/sync_api/groq_utils.py
--rw-r--r--   0        0        0      154 2024-05-29 18:38:37.067701 groqon-0.1.82/groqon/utils.py
--rw-r--r--   0        0        0      469 2024-05-30 07:26:08.438687 groqon-0.1.82/pyproject.toml
--rw-r--r--   0        0        0     3890 1970-01-01 00:00:00.000000 groqon-0.1.82/PKG-INFO
+-rw-r--r--   0        0        0     3492 2024-05-22 13:47:15.279707 groqon-0.1.9/README.md
+-rw-r--r--   0        0        0      270 2024-05-29 18:38:37.047706 groqon-0.1.9/groqon/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 12:01:28.521416 groqon-0.1.9/groqon/async_api/__init__.py
+-rw-r--r--   0        0        0    21906 2024-05-30 07:32:22.973746 groqon-0.1.9/groqon/async_api/agroq.py
+-rw-r--r--   0        0        0     8365 2024-05-29 18:39:08.757118 groqon-0.1.9/groqon/async_api/agroq_utils.py
+-rw-r--r--   0        0        0       53 2024-05-22 13:13:35.662297 groqon-0.1.9/groqon/async_api/experimental/__init__.py
+-rw-r--r--   0        0        0     1275 2024-05-22 13:22:45.285100 groqon-0.1.9/groqon/async_api/experimental/mock_api.py
+-rw-r--r--   0        0        0     3419 2024-05-30 06:27:02.736663 groqon-0.1.9/groqon/element_selectors.py
+-rw-r--r--   0        0        0     1573 2024-05-29 18:38:37.094694 groqon-0.1.9/groqon/groq_config.py
+-rw-r--r--   0        0        0     1098 2024-05-29 18:38:37.068701 groqon-0.1.9/groqon/logger.py
+-rw-r--r--   0        0        0     2292 2024-05-29 18:38:37.118688 groqon-0.1.9/groqon/parsing.py
+-rw-r--r--   0        0        0        0 2024-05-22 12:01:37.983678 groqon-0.1.9/groqon/sync_api/__init__.py
+-rw-r--r--   0        0        0     8887 2024-05-22 13:50:34.888728 groqon-0.1.9/groqon/sync_api/groq.py
+-rw-r--r--   0        0        0     6976 2024-05-22 17:23:19.949054 groqon-0.1.9/groqon/sync_api/groq_utils.py
+-rw-r--r--   0        0        0      154 2024-05-29 18:38:37.067701 groqon-0.1.9/groqon/utils.py
+-rw-r--r--   0        0        0      468 2024-05-30 07:33:32.677655 groqon-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3889 1970-01-01 00:00:00.000000 groqon-0.1.9/PKG-INFO
```

### Comparing `groqon-0.1.82/README.md` & `groqon-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `groqon-0.1.82/groqon/async_api/agroq.py` & `groqon-0.1.9/groqon/async_api/agroq.py`

 * *Files 1% similar despite different names*

```diff
@@ -626,18 +626,18 @@
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "queries",
         nargs="+",
         help="one or more quoted string like 'what is the purpose of life?' 'why everyone hates meg griffin?'",
     )
     parser.add_argument(
-        "--model",
+        "--model_list",
         nargs="+",
         default=DEFAULT_MODEL,
-        help=f"Available models are {' '.join(modelindex)}",
+        help=f"Available models are {' '.join(modelindex)}, e.g enter as --model_list 'llama3-8b' 'gemma-7b' ",
     )
     parser.add_argument(
         "--cookie_file",
         type=str,
         default=GROQ_COOKIE_FILE,
         help="looks in current directory by default for groq_cookie.json. If not found, You will have to login when the browswer opens under 120 seconds. It's one time thing",
     )
@@ -677,15 +677,15 @@
     def check_headless(x):
         return x.lower().strip() == "true"
 
     headless = check_headless(args.headless)
 
     out = agroq(
             cookie_file=args.cookie_file,
-            model_list=args.model,
+            model_list=args.model_list,
             headless=headless,
             query_list=args.queries,
             save_dir=args.output_dir,
             system_prompt=args.system_prompt,
             print_output=True,
             temperature=args.temperature,
             max_tokens=args.max_tokens,
```

### Comparing `groqon-0.1.82/groqon/async_api/agroq_utils.py` & `groqon-0.1.9/groqon/async_api/agroq_utils.py`

 * *Files identical despite different names*

### Comparing `groqon-0.1.82/groqon/async_api/experimental/mock_api.py` & `groqon-0.1.9/groqon/async_api/experimental/mock_api.py`

 * *Files identical despite different names*

### Comparing `groqon-0.1.82/groqon/element_selectors.py` & `groqon-0.1.9/groqon/element_selectors.py`

 * *Files identical despite different names*

### Comparing `groqon-0.1.82/groqon/groq_config.py` & `groqon-0.1.9/groqon/groq_config.py`

 * *Files identical despite different names*

### Comparing `groqon-0.1.82/groqon/logger.py` & `groqon-0.1.9/groqon/logger.py`

 * *Files identical despite different names*

### Comparing `groqon-0.1.82/groqon/parsing.py` & `groqon-0.1.9/groqon/parsing.py`

 * *Files identical despite different names*

### Comparing `groqon-0.1.82/groqon/sync_api/groq.py` & `groqon-0.1.9/groqon/sync_api/groq.py`

 * *Files identical despite different names*

### Comparing `groqon-0.1.82/groqon/sync_api/groq_utils.py` & `groqon-0.1.9/groqon/sync_api/groq_utils.py`

 * *Files identical despite different names*

### Comparing `groqon-0.1.82/PKG-INFO` & `groqon-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: groqon
-Version: 0.1.82
+Version: 0.1.9
 Summary: Use Groq.com as llm
 Author: tikendraw
 Author-email: tikendraksahu1029@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

