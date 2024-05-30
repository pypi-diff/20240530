# Comparing `tmp/lunary-1.0.8.tar.gz` & `tmp/lunary-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lunary-1.0.8.tar", max compression
+gzip compressed data, was "lunary-1.0.9.tar", max compression
```

## Comparing `lunary-1.0.8.tar` & `lunary-1.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      604 2024-02-24 01:43:56.000000 lunary-1.0.8/README.md
--rw-r--r--   0        0        0    61354 2024-05-03 16:08:13.152703 lunary-1.0.8/lunary/__init__.py
--rw-r--r--   0        0        0     2221 2024-03-27 12:45:10.024740 lunary-1.0.8/lunary/consumer.py
--rw-r--r--   0        0        0      607 2024-03-09 04:19:24.000000 lunary-1.0.8/lunary/event_queue.py
--rw-r--r--   0        0        0     2384 2024-02-23 21:19:34.000000 lunary-1.0.8/lunary/openai_utils.py
--rw-r--r--   0        0        0      670 2024-04-09 13:37:22.854858 lunary-1.0.8/lunary/parent.py
--rw-r--r--   0        0        0     1071 2024-04-09 13:37:22.855410 lunary-1.0.8/lunary/parsers.py
--rw-r--r--   0        0        0      425 2024-04-09 13:37:16.108314 lunary-1.0.8/lunary/project.py
--rw-r--r--   0        0        0      378 2024-03-27 12:45:06.573143 lunary-1.0.8/lunary/tags.py
--rw-r--r--   0        0        0     1164 2024-04-25 09:32:12.975713 lunary-1.0.8/lunary/thread.py
--rw-r--r--   0        0        0      573 2024-02-23 21:19:34.000000 lunary-1.0.8/lunary/users.py
--rw-r--r--   0        0        0      762 2024-05-03 16:08:48.542692 lunary-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     1723 1970-01-01 00:00:00.000000 lunary-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0      604 2024-02-24 01:43:56.000000 lunary-1.0.9/README.md
+-rw-r--r--   0        0        0    61235 2024-05-03 16:11:56.710425 lunary-1.0.9/lunary/__init__.py
+-rw-r--r--   0        0        0     2221 2024-03-27 12:45:10.024740 lunary-1.0.9/lunary/consumer.py
+-rw-r--r--   0        0        0      607 2024-03-09 04:19:24.000000 lunary-1.0.9/lunary/event_queue.py
+-rw-r--r--   0        0        0     2384 2024-02-23 21:19:34.000000 lunary-1.0.9/lunary/openai_utils.py
+-rw-r--r--   0        0        0      670 2024-04-09 13:37:22.854858 lunary-1.0.9/lunary/parent.py
+-rw-r--r--   0        0        0     1071 2024-04-09 13:37:22.855410 lunary-1.0.9/lunary/parsers.py
+-rw-r--r--   0        0        0      425 2024-04-09 13:37:16.108314 lunary-1.0.9/lunary/project.py
+-rw-r--r--   0        0        0      378 2024-03-27 12:45:06.573143 lunary-1.0.9/lunary/tags.py
+-rw-r--r--   0        0        0     1164 2024-04-25 09:32:12.975713 lunary-1.0.9/lunary/thread.py
+-rw-r--r--   0        0        0      573 2024-02-23 21:19:34.000000 lunary-1.0.9/lunary/users.py
+-rw-r--r--   0        0        0      762 2024-05-03 16:12:07.717663 lunary-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1723 1970-01-01 00:00:00.000000 lunary-1.0.9/PKG-INFO
```

### Comparing `lunary-1.0.8/README.md` & `lunary-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `lunary-1.0.8/lunary/__init__.py` & `lunary-1.0.9/lunary/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -375,15 +375,14 @@
                         "user_id", None) or user_ctx.get() or user_id,
                     user_props=kwargs.pop("user_props", None)
                     or user_props
                     or user_props_ctx.get(),
                     params=params,
                     metadata=metadata,
                     tags=kwargs.pop("tags", None) or tags or tags_ctx.get(),
-                    params=kwargs.get("extra", None),
                     template_id=kwargs.get("extra_headers", {}).get("Template-Id", None),
                     is_openai=True
                 )
             except Exception as e:
                 handle_internal_error(e)
 
             if kwargs.get("stream") == True:
@@ -464,15 +463,14 @@
                         ) or user_ctx.get() or user_id,
                         user_props=kwargs.pop("user_props", None)
                                    or user_props
                                    or user_props_ctx.get(),
                         params=params,
                         metadata=metadata,
                         tags=kwargs.pop("tags", None) or tags or tags_ctx.get(),
-                        params=parsed_input.get("extra", None),
                         template_id=kwargs.get("extra_headers", {}).get("Template-Id", None),
                     )
                 except Exception as e:
                     handle_internal_error(e)
 
                 try:
                     output = await fn(*args, **kwargs)
@@ -706,15 +704,14 @@
         "tools",
         "tool_choice",
         "response_format",
         "max_tokens",
         "logit_bias",
     ]
 
-
     class UserContextManager:
         """Context manager for Lunary user context."""
 
         def __init__(self, user_id: str, user_props: Any = None) -> None:
             user_ctx.set(user_id)
             user_props_ctx.set(user_props)
```

### Comparing `lunary-1.0.8/lunary/consumer.py` & `lunary-1.0.9/lunary/consumer.py`

 * *Files identical despite different names*

### Comparing `lunary-1.0.8/lunary/event_queue.py` & `lunary-1.0.9/lunary/event_queue.py`

 * *Files identical despite different names*

### Comparing `lunary-1.0.8/lunary/openai_utils.py` & `lunary-1.0.9/lunary/openai_utils.py`

 * *Files identical despite different names*

### Comparing `lunary-1.0.8/lunary/parent.py` & `lunary-1.0.9/lunary/parent.py`

 * *Files identical despite different names*

### Comparing `lunary-1.0.8/lunary/parsers.py` & `lunary-1.0.9/lunary/parsers.py`

 * *Files identical despite different names*

### Comparing `lunary-1.0.8/lunary/thread.py` & `lunary-1.0.9/lunary/thread.py`

 * *Files identical despite different names*

### Comparing `lunary-1.0.8/lunary/users.py` & `lunary-1.0.9/lunary/users.py`

 * *Files identical despite different names*

### Comparing `lunary-1.0.8/pyproject.toml` & `lunary-1.0.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lunary"
-version = "1.0.8"
+version = "1.0.9"
 description = "Observability, analytics and evaluations for AI agents and chatbots."
 authors = ["lunary <hello@lunary.ai>"]
 readme = "README.md"
 repository = "https://github.com/lunary-ai/lunary-py"
 documentation = "https://lunary.ai/docs/py"
 keywords = ["Lunary", "lunary.ai", "Langchain", "AI", "Analytics", "Monitoring"]
```

### Comparing `lunary-1.0.8/PKG-INFO` & `lunary-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lunary
-Version: 1.0.8
+Version: 1.0.9
 Summary: Observability, analytics and evaluations for AI agents and chatbots.
 Home-page: https://github.com/lunary-ai/lunary-py
 Keywords: Lunary,lunary.ai,Langchain,AI,Analytics,Monitoring
 Author: lunary
 Author-email: hello@lunary.ai
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
```

