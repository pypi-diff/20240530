# Comparing `tmp/aily_code_sdk_core-0.1.0b3.tar.gz` & `tmp/aily_code_sdk_core-0.1.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aily_code_sdk_core-0.1.0b3.tar", last modified: Fri May 17 02:39:06 2024, max compression
+gzip compressed data, was "aily_code_sdk_core-0.1.0b4.tar", max compression
```

## Comparing `aily_code_sdk_core-0.1.0b3.tar` & `aily_code_sdk_core-0.1.0b4.tar`

### file list

```diff
@@ -1,48 +1,32 @@
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-17 02:39:06.163182 aily_code_sdk_core-0.1.0b3/
--rw-r--r--   0 bytedance   (501) staff       (20)    10947 2024-05-15 08:04:11.000000 aily_code_sdk_core-0.1.0b3/LICENSE
--rw-r--r--   0 bytedance   (501) staff       (20)    13383 2024-05-17 02:39:06.162827 aily_code_sdk_core-0.1.0b3/PKG-INFO
--rw-r--r--   0 bytedance   (501) staff       (20)      446 2024-05-16 12:44:26.000000 aily_code_sdk_core-0.1.0b3/README.md
--rw-r--r--   0 bytedance   (501) staff       (20)      516 2024-05-17 02:38:32.000000 aily_code_sdk_core-0.1.0b3/pyproject.toml
--rw-r--r--   0 bytedance   (501) staff       (20)       38 2024-05-17 02:39:06.163237 aily_code_sdk_core-0.1.0b3/setup.cfg
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-17 02:39:06.149527 aily_code_sdk_core-0.1.0b3/src/
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-17 02:39:06.151930 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2024-05-13 11:55:38.000000 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-17 02:39:06.154095 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/action/
--rw-r--r--   0 bytedance   (501) staff       (20)       71 2024-05-13 12:16:24.000000 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/action/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1341 2024-05-16 08:25:22.000000 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/action/call_action.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-17 02:39:06.154642 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/common/
--rw-r--r--   0 bytedance   (501) staff       (20)     1260 2024-05-17 02:38:10.000000 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/common/context.py
--rw-r--r--   0 bytedance   (501) staff       (20)      335 2024-05-13 07:28:48.000000 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/common/util.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-17 02:39:06.155382 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/credential/
--rw-r--r--   0 bytedance   (501) staff       (20)       74 2024-05-13 12:16:38.000000 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/credential/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1593 2024-05-16 08:22:26.000000 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/credential/credential.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-17 02:39:06.156146 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/env/
--rw-r--r--   0 bytedance   (501) staff       (20)       74 2024-05-13 12:16:47.000000 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/env/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)      458 2024-05-15 08:39:46.000000 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/env/get_env_info.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-17 02:39:06.156567 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/message/
--rw-r--r--   0 bytedance   (501) staff       (20)      752 2024-05-13 12:20:34.000000 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/message/builder.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-17 02:39:06.162120 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/message/components/
--rw-r--r--   0 bytedance   (501) staff       (20)      682 2024-05-13 12:17:00.000000 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/message/components/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1840 2024-05-13 12:21:51.000000 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/message/components/base_component.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1556 2024-05-11 04:30:30.000000 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/message/components/button.py
--rw-r--r--   0 bytedance   (501) staff       (20)      288 2024-05-11 03:23:07.000000 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/message/components/chart.py
--rw-r--r--   0 bytedance   (501) staff       (20)      362 2024-05-13 12:22:51.000000 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/message/components/code.py
--rw-r--r--   0 bytedance   (501) staff       (20)      266 2024-05-11 04:39:01.000000 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/message/components/col.py
--rw-r--r--   0 bytedance   (501) staff       (20)      441 2024-05-13 12:21:18.000000 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/message/components/color_text.py
--rw-r--r--   0 bytedance   (501) staff       (20)      934 2024-05-13 12:22:32.000000 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/message/components/data_record.py
--rw-r--r--   0 bytedance   (501) staff       (20)      399 2024-05-13 08:09:19.000000 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/message/components/highlight.py
--rw-r--r--   0 bytedance   (501) staff       (20)      337 2024-05-11 03:23:24.000000 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/message/components/image.py
--rw-r--r--   0 bytedance   (501) staff       (20)      354 2024-05-11 03:23:18.000000 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/message/components/item_list.py
--rw-r--r--   0 bytedance   (501) staff       (20)      559 2024-05-13 12:22:14.000000 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/message/components/link.py
--rw-r--r--   0 bytedance   (501) staff       (20)      365 2024-05-11 03:23:18.000000 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/message/components/mention.py
--rw-r--r--   0 bytedance   (501) staff       (20)      389 2024-05-11 08:11:14.000000 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/message/components/note.py
--rw-r--r--   0 bytedance   (501) staff       (20)      491 2024-05-13 12:02:12.000000 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/message/components/ordered_list.py
--rw-r--r--   0 bytedance   (501) staff       (20)      327 2024-05-11 03:23:18.000000 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/message/components/row.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1055 2024-05-11 03:23:18.000000 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/message/components/table.py
--rw-r--r--   0 bytedance   (501) staff       (20)      587 2024-05-11 03:23:17.000000 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/message/components/title.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-17 02:39:06.162419 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core.egg-info/
--rw-r--r--   0 bytedance   (501) staff       (20)    13383 2024-05-17 02:39:06.000000 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core.egg-info/PKG-INFO
--rw-r--r--   0 bytedance   (501) staff       (20)     1632 2024-05-17 02:39:06.000000 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core.egg-info/SOURCES.txt
--rw-r--r--   0 bytedance   (501) staff       (20)        1 2024-05-17 02:39:06.000000 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core.egg-info/dependency_links.txt
--rw-r--r--   0 bytedance   (501) staff       (20)       24 2024-05-17 02:39:06.000000 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core.egg-info/requires.txt
--rw-r--r--   0 bytedance   (501) staff       (20)       19 2024-05-17 02:39:06.000000 aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core.egg-info/top_level.txt
+-rw-r--r--   0        0        0    10947 2024-05-29 05:58:44.305920 aily_code_sdk_core-0.1.0b4/LICENSE
+-rw-r--r--   0        0        0      446 2024-05-29 05:58:44.306203 aily_code_sdk_core-0.1.0b4/README.md
+-rw-r--r--   0        0        0      503 2024-05-30 08:01:01.568120 aily_code_sdk_core-0.1.0b4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-29 05:58:44.306688 aily_code_sdk_core-0.1.0b4/src/aily_code_sdk_core/__init__.py
+-rw-r--r--   0        0        0       71 2024-05-29 05:58:44.307011 aily_code_sdk_core-0.1.0b4/src/aily_code_sdk_core/action/__init__.py
+-rw-r--r--   0        0        0     1787 2024-05-30 04:08:44.777729 aily_code_sdk_core-0.1.0b4/src/aily_code_sdk_core/action/call_action.py
+-rw-r--r--   0        0        0     1390 2024-05-29 06:39:31.368996 aily_code_sdk_core-0.1.0b4/src/aily_code_sdk_core/common/context.py
+-rw-r--r--   0        0        0      541 2024-05-29 09:20:25.222586 aily_code_sdk_core-0.1.0b4/src/aily_code_sdk_core/common/util.py
+-rw-r--r--   0        0        0       74 2024-05-29 05:58:44.308002 aily_code_sdk_core-0.1.0b4/src/aily_code_sdk_core/credential/__init__.py
+-rw-r--r--   0        0        0     1593 2024-05-29 05:58:44.308159 aily_code_sdk_core-0.1.0b4/src/aily_code_sdk_core/credential/credential.py
+-rw-r--r--   0        0        0       74 2024-05-29 05:58:44.308382 aily_code_sdk_core-0.1.0b4/src/aily_code_sdk_core/env/__init__.py
+-rw-r--r--   0        0        0      437 2024-05-29 06:18:31.530058 aily_code_sdk_core-0.1.0b4/src/aily_code_sdk_core/env/get_env_info.py
+-rw-r--r--   0        0        0      752 2024-05-29 05:58:44.308918 aily_code_sdk_core-0.1.0b4/src/aily_code_sdk_core/message/builder.py
+-rw-r--r--   0        0        0      682 2024-05-29 05:58:44.309181 aily_code_sdk_core-0.1.0b4/src/aily_code_sdk_core/message/components/__init__.py
+-rw-r--r--   0        0        0     1840 2024-05-29 05:58:44.309338 aily_code_sdk_core-0.1.0b4/src/aily_code_sdk_core/message/components/base_component.py
+-rw-r--r--   0        0        0     1556 2024-05-29 05:58:44.309521 aily_code_sdk_core-0.1.0b4/src/aily_code_sdk_core/message/components/button.py
+-rw-r--r--   0        0        0      288 2024-05-29 05:58:44.309677 aily_code_sdk_core-0.1.0b4/src/aily_code_sdk_core/message/components/chart.py
+-rw-r--r--   0        0        0      362 2024-05-29 05:58:44.309822 aily_code_sdk_core-0.1.0b4/src/aily_code_sdk_core/message/components/code.py
+-rw-r--r--   0        0        0      266 2024-05-29 05:58:44.309973 aily_code_sdk_core-0.1.0b4/src/aily_code_sdk_core/message/components/col.py
+-rw-r--r--   0        0        0      441 2024-05-29 05:58:44.310106 aily_code_sdk_core-0.1.0b4/src/aily_code_sdk_core/message/components/color_text.py
+-rw-r--r--   0        0        0      934 2024-05-29 05:58:44.310283 aily_code_sdk_core-0.1.0b4/src/aily_code_sdk_core/message/components/data_record.py
+-rw-r--r--   0        0        0      399 2024-05-29 05:58:44.310433 aily_code_sdk_core-0.1.0b4/src/aily_code_sdk_core/message/components/highlight.py
+-rw-r--r--   0        0        0      337 2024-05-29 05:58:44.310584 aily_code_sdk_core-0.1.0b4/src/aily_code_sdk_core/message/components/image.py
+-rw-r--r--   0        0        0      354 2024-05-29 05:58:44.310776 aily_code_sdk_core-0.1.0b4/src/aily_code_sdk_core/message/components/item_list.py
+-rw-r--r--   0        0        0      559 2024-05-29 05:58:44.310921 aily_code_sdk_core-0.1.0b4/src/aily_code_sdk_core/message/components/link.py
+-rw-r--r--   0        0        0      365 2024-05-29 05:58:44.311078 aily_code_sdk_core-0.1.0b4/src/aily_code_sdk_core/message/components/mention.py
+-rw-r--r--   0        0        0      389 2024-05-29 05:58:44.311215 aily_code_sdk_core-0.1.0b4/src/aily_code_sdk_core/message/components/note.py
+-rw-r--r--   0        0        0      491 2024-05-29 05:58:44.311355 aily_code_sdk_core-0.1.0b4/src/aily_code_sdk_core/message/components/ordered_list.py
+-rw-r--r--   0        0        0      327 2024-05-29 05:58:44.311541 aily_code_sdk_core-0.1.0b4/src/aily_code_sdk_core/message/components/row.py
+-rw-r--r--   0        0        0     1055 2024-05-29 05:58:44.311779 aily_code_sdk_core-0.1.0b4/src/aily_code_sdk_core/message/components/table.py
+-rw-r--r--   0        0        0      587 2024-05-29 05:58:44.311902 aily_code_sdk_core-0.1.0b4/src/aily_code_sdk_core/message/components/title.py
+-rw-r--r--   0        0        0     1299 1970-01-01 00:00:00.000000 aily_code_sdk_core-0.1.0b4/PKG-INFO
```

### Comparing `aily_code_sdk_core-0.1.0b3/LICENSE` & `aily_code_sdk_core-0.1.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/common/context.py` & `aily_code_sdk_core-0.1.0b4/src/aily_code_sdk_core/common/context.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 import contextvars
+import logging
 import os
 
 NodeClsKey = "x-apaas-node-cls"
 
 CtxVar = contextvars.ContextVar(NodeClsKey)
 
 try:
     from _sys import CtxVar  # type: ignore
-except Exception:
-    pass
+except Exception as e:
+    logging.info(f'fail to load CtxVar {e}')
 
 
-def Ctx():
+def ctx():
     return contextvars.copy_context()
 
 
 def get_ctx():
     try:
         return CtxVar.get()
     except LookupError:
         CtxVar.set({})
         return CtxVar.get()
 
 
 def get_ctx_key(key):
     try:
         return get_ctx()[key]
-    except Exception:
+    except Exception as err:
+        logging.info(f'key `{key}` not found in context {err}')
         return None
 
 
 def get_from_credential(key: str):
     credential = get_ctx_key("credential")
     if credential is None:
         return ""
@@ -56,11 +58,11 @@
 def get_domain():
     if is_local_dev():
         return os.environ.get("AILY_SDK_DOMAIN")
     return get_from_credential("domain")
 
 
 def get_by_headers(key):
-    headers = get_ctx_key("headers")
+    headers = get_ctx_key("sysHeaders")
     if headers is None:
         return ""
     return headers[key]
```

### Comparing `aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/credential/credential.py` & `aily_code_sdk_core-0.1.0b4/src/aily_code_sdk_core/credential/credential.py`

 * *Files identical despite different names*

### Comparing `aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/message/builder.py` & `aily_code_sdk_core-0.1.0b4/src/aily_code_sdk_core/message/builder.py`

 * *Files identical despite different names*

### Comparing `aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/message/components/__init__.py` & `aily_code_sdk_core-0.1.0b4/src/aily_code_sdk_core/message/components/__init__.py`

 * *Files identical despite different names*

### Comparing `aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/message/components/base_component.py` & `aily_code_sdk_core-0.1.0b4/src/aily_code_sdk_core/message/components/base_component.py`

 * *Files identical despite different names*

### Comparing `aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/message/components/button.py` & `aily_code_sdk_core-0.1.0b4/src/aily_code_sdk_core/message/components/button.py`

 * *Files identical despite different names*

### Comparing `aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/message/components/data_record.py` & `aily_code_sdk_core-0.1.0b4/src/aily_code_sdk_core/message/components/data_record.py`

 * *Files identical despite different names*

### Comparing `aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/message/components/link.py` & `aily_code_sdk_core-0.1.0b4/src/aily_code_sdk_core/message/components/link.py`

 * *Files identical despite different names*

### Comparing `aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/message/components/table.py` & `aily_code_sdk_core-0.1.0b4/src/aily_code_sdk_core/message/components/table.py`

 * *Files identical despite different names*

### Comparing `aily_code_sdk_core-0.1.0b3/src/aily_code_sdk_core/message/components/title.py` & `aily_code_sdk_core-0.1.0b4/src/aily_code_sdk_core/message/components/title.py`

 * *Files identical despite different names*

