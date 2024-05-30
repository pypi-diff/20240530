# Comparing `tmp/groqon-0.1.7.tar.gz` & `tmp/groqon-0.1.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "groqon-0.1.7.tar", max compression
+gzip compressed data, was "groqon-0.1.71.tar", max compression
```

## Comparing `groqon-0.1.7.tar` & `groqon-0.1.71.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     3492 2024-05-22 13:47:15.279707 groqon-0.1.7/README.md
--rw-r--r--   0        0        0      270 2024-05-29 18:38:37.047706 groqon-0.1.7/groqon/__init__.py
--rw-r--r--   0        0        0        0 2024-05-22 12:01:28.521416 groqon-0.1.7/groqon/async_api/__init__.py
--rw-r--r--   0        0        0    21996 2024-05-30 07:01:41.156774 groqon-0.1.7/groqon/async_api/agroq.py
--rw-r--r--   0        0        0     8365 2024-05-29 18:39:08.757118 groqon-0.1.7/groqon/async_api/agroq_utils.py
--rw-r--r--   0        0        0       53 2024-05-22 13:13:35.662297 groqon-0.1.7/groqon/async_api/experimental/__init__.py
--rw-r--r--   0        0        0     1275 2024-05-22 13:22:45.285100 groqon-0.1.7/groqon/async_api/experimental/mock_api.py
--rw-r--r--   0        0        0     3419 2024-05-30 06:27:02.736663 groqon-0.1.7/groqon/element_selectors.py
--rw-r--r--   0        0        0     1573 2024-05-29 18:38:37.094694 groqon-0.1.7/groqon/groq_config.py
--rw-r--r--   0        0        0     1098 2024-05-29 18:38:37.068701 groqon-0.1.7/groqon/logger.py
--rw-r--r--   0        0        0     2292 2024-05-29 18:38:37.118688 groqon-0.1.7/groqon/parsing.py
--rw-r--r--   0        0        0        0 2024-05-22 12:01:37.983678 groqon-0.1.7/groqon/sync_api/__init__.py
--rw-r--r--   0        0        0     8887 2024-05-22 13:50:34.888728 groqon-0.1.7/groqon/sync_api/groq.py
--rw-r--r--   0        0        0     6976 2024-05-22 17:23:19.949054 groqon-0.1.7/groqon/sync_api/groq_utils.py
--rw-r--r--   0        0        0      154 2024-05-29 18:38:37.067701 groqon-0.1.7/groqon/utils.py
--rw-r--r--   0        0        0      468 2024-05-29 18:40:49.831833 groqon-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3889 1970-01-01 00:00:00.000000 groqon-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     3492 2024-05-22 13:47:15.279707 groqon-0.1.71/README.md
+-rw-r--r--   0        0        0      270 2024-05-29 18:38:37.047706 groqon-0.1.71/groqon/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 12:01:28.521416 groqon-0.1.71/groqon/async_api/__init__.py
+-rw-r--r--   0        0        0    21861 2024-05-30 07:12:34.776702 groqon-0.1.71/groqon/async_api/agroq.py
+-rw-r--r--   0        0        0     8365 2024-05-29 18:39:08.757118 groqon-0.1.71/groqon/async_api/agroq_utils.py
+-rw-r--r--   0        0        0       53 2024-05-22 13:13:35.662297 groqon-0.1.71/groqon/async_api/experimental/__init__.py
+-rw-r--r--   0        0        0     1275 2024-05-22 13:22:45.285100 groqon-0.1.71/groqon/async_api/experimental/mock_api.py
+-rw-r--r--   0        0        0     3419 2024-05-30 06:27:02.736663 groqon-0.1.71/groqon/element_selectors.py
+-rw-r--r--   0        0        0     1573 2024-05-29 18:38:37.094694 groqon-0.1.71/groqon/groq_config.py
+-rw-r--r--   0        0        0     1098 2024-05-29 18:38:37.068701 groqon-0.1.71/groqon/logger.py
+-rw-r--r--   0        0        0     2292 2024-05-29 18:38:37.118688 groqon-0.1.71/groqon/parsing.py
+-rw-r--r--   0        0        0        0 2024-05-22 12:01:37.983678 groqon-0.1.71/groqon/sync_api/__init__.py
+-rw-r--r--   0        0        0     8887 2024-05-22 13:50:34.888728 groqon-0.1.71/groqon/sync_api/groq.py
+-rw-r--r--   0        0        0     6976 2024-05-22 17:23:19.949054 groqon-0.1.71/groqon/sync_api/groq_utils.py
+-rw-r--r--   0        0        0      154 2024-05-29 18:38:37.067701 groqon-0.1.71/groqon/utils.py
+-rw-r--r--   0        0        0      469 2024-05-30 07:14:33.424480 groqon-0.1.71/pyproject.toml
+-rw-r--r--   0        0        0     3890 1970-01-01 00:00:00.000000 groqon-0.1.71/PKG-INFO
```

### Comparing `groqon-0.1.7/README.md` & `groqon-0.1.71/README.md`

 * *Files identical despite different names*

### Comparing `groqon-0.1.7/groqon/async_api/agroq.py` & `groqon-0.1.71/groqon/async_api/agroq.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
 # @profile
 async def check_login(route: Route):
     # ic("in check_login func  : ", now())
     if route.request.url == AUTHENTICATION_URL:
         response = await route.fetch()
 
-        print(colored(f"****: {response.body().decode('utf-8')}", "red"))
+        # print(colored(f"****: {response.body().decode('utf-8')}", "red"))
         await route.continue_()
     else:
         await route.abort()
 
 
 # @profile
 @asynccontextmanager
@@ -245,15 +245,15 @@
             "max_tokens": max_tokens,
             "temperature": temperature,
             "top_p": 1,
             "system_prompt": system_prompt,
         }
 
         await page.goto(URL, timeout=60 * 1000)
-        print("start query: ", now())
+        # print("start query: ", now())
 
         for query in queries:
             user_dict = original_user_dict.copy()
             user_dict["query"] = query
 
             partial_handle.keywords["user_dict"] = user_dict
 
@@ -344,15 +344,15 @@
     print_output: bool = True,
     temperature: float = 0.1,
     max_tokens: int = 2048,
     n_workers: int = 2,
 ) -> List[Dict[str, Any]]:
     """Main function to perform queries and process responses."""
     # ic("in agroq func", now())
-    print("start ", now())
+    # print("start ", now())
     return asyncio.run(
         _agroq(
             query_list=query_list,
             cookie_file=cookie_file,
             model_list=model_list,
             headless=headless,
             save_dir=save_dir,
@@ -589,21 +589,17 @@
                             "Please try to provide useful, helpful and actionable answers.",
                         ),
                         "role": "system",
                     },
                     {"content": user_dict.get("query", "hi"), "role": "user"},
                 ],
             }
-            print("start post data : ", now())
+            # print("start post data : ", now())
 
-            print(
-                colored(
-                    f"***** >>> this is going as post data, {modified_data}", "green"
-                )
-            )
+            # print(colored(f"***** >>> this is going as post data, {modified_data}", "green"))
             await route.continue_(post_data=json.dumps(modified_data))
         else:
             await route.continue_()
     else:
         await route.continue_()
 
     response = await get_query_response(route, user_dict.get("query"))
@@ -632,37 +628,33 @@
         "queries",
         nargs="+",
         help="one or more quoted string like 'what is the purpose of life?' 'why everyone hates meg griffin?'",
     )
     parser.add_argument(
         "--model",
         nargs="+",
-        default="llama3-70b",
+        default=DEFAULT_MODEL,
         help=f"Available models are {' '.join(modelindex)}",
     )
     parser.add_argument(
         "--cookie_file",
         type=str,
         default=GROQ_COOKIE_FILE,
         help="looks in current directory by default for groq_cookie.json. If not found, You will have to login when the browswer opens under 120 seconds. It's one time thing",
     )
     parser.add_argument(
         "--system_prompt",
         type=str,
+        default="Please try to provide useful, helpful and actionable answers.",
         help="System prompt to be given to the llm model. Its like 'you are samuel l jackson as my assistant'. Default is None.",
     )
     parser.add_argument(
         "--headless", type=str, default="True", help="set true to not see the browser"
     )
     parser.add_argument(
-        "--save_output",
-        action="store_true",
-        help="set true to save the groq output with its query name.json",
-    )
-    parser.add_argument(
         "--output_dir",
         default=os.getcwd(),
         help="Path to save the output file. Defaults to current working directory.",
     )
 
     parser.add_argument(
         "--temperature", type=float, default=0.1, help="Temperature value"
```

### Comparing `groqon-0.1.7/groqon/async_api/agroq_utils.py` & `groqon-0.1.71/groqon/async_api/agroq_utils.py`

 * *Files identical despite different names*

### Comparing `groqon-0.1.7/groqon/async_api/experimental/mock_api.py` & `groqon-0.1.71/groqon/async_api/experimental/mock_api.py`

 * *Files identical despite different names*

### Comparing `groqon-0.1.7/groqon/element_selectors.py` & `groqon-0.1.71/groqon/element_selectors.py`

 * *Files identical despite different names*

### Comparing `groqon-0.1.7/groqon/groq_config.py` & `groqon-0.1.71/groqon/groq_config.py`

 * *Files identical despite different names*

### Comparing `groqon-0.1.7/groqon/logger.py` & `groqon-0.1.71/groqon/logger.py`

 * *Files identical despite different names*

### Comparing `groqon-0.1.7/groqon/parsing.py` & `groqon-0.1.71/groqon/parsing.py`

 * *Files identical despite different names*

### Comparing `groqon-0.1.7/groqon/sync_api/groq.py` & `groqon-0.1.71/groqon/sync_api/groq.py`

 * *Files identical despite different names*

### Comparing `groqon-0.1.7/groqon/sync_api/groq_utils.py` & `groqon-0.1.71/groqon/sync_api/groq_utils.py`

 * *Files identical despite different names*

### Comparing `groqon-0.1.7/PKG-INFO` & `groqon-0.1.71/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: groqon
-Version: 0.1.7
+Version: 0.1.71
 Summary: Use Groq.com as llm
 Author: tikendraw
 Author-email: tikendraksahu1029@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

