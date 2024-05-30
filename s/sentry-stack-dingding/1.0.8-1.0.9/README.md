# Comparing `tmp/sentry-stack-dingding-1.0.8.tar.gz` & `tmp/sentry-stack-dingding-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sentry-stack-dingding-1.0.8.tar", last modified: Mon May 13 06:39:09 2024, max compression
+gzip compressed data, was "dist/sentry-stack-dingding-1.0.9.tar", last modified: Mon May 13 07:07:19 2024, max compression
```

## Comparing `sentry-stack-dingding-1.0.8.tar` & `sentry-stack-dingding-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 wilson    (1000) wilson    (1000)        0 2024-05-13 06:39:09.000000 sentry-stack-dingding-1.0.8/
--rw-rw-r--   0 wilson    (1000) wilson    (1000)       38 2024-05-13 06:39:09.000000 sentry-stack-dingding-1.0.8/setup.cfg
--rw-rw-r--   0 wilson    (1000) wilson    (1000)     1044 2024-05-13 04:26:29.000000 sentry-stack-dingding-1.0.8/setup.py
--rw-rw-r--   0 wilson    (1000) wilson    (1000)      774 2024-05-13 03:32:44.000000 sentry-stack-dingding-1.0.8/README.md
--rw-rw-r--   0 wilson    (1000) wilson    (1000)     1549 2024-05-13 06:39:09.000000 sentry-stack-dingding-1.0.8/PKG-INFO
-drwxrwxr-x   0 wilson    (1000) wilson    (1000)        0 2024-05-13 06:39:09.000000 sentry-stack-dingding-1.0.8/src/
-drwxrwxr-x   0 wilson    (1000) wilson    (1000)        0 2024-05-13 06:39:09.000000 sentry-stack-dingding-1.0.8/src/sentry_stack_dingding.egg-info/
--rw-rw-r--   0 wilson    (1000) wilson    (1000)      453 2024-05-13 06:39:09.000000 sentry-stack-dingding-1.0.8/src/sentry_stack_dingding.egg-info/SOURCES.txt
--rw-rw-r--   0 wilson    (1000) wilson    (1000)       16 2024-05-13 06:39:09.000000 sentry-stack-dingding-1.0.8/src/sentry_stack_dingding.egg-info/top_level.txt
--rw-rw-r--   0 wilson    (1000) wilson    (1000)        1 2024-05-13 06:39:09.000000 sentry-stack-dingding-1.0.8/src/sentry_stack_dingding.egg-info/dependency_links.txt
--rw-rw-r--   0 wilson    (1000) wilson    (1000)     1549 2024-05-13 06:39:09.000000 sentry-stack-dingding-1.0.8/src/sentry_stack_dingding.egg-info/PKG-INFO
--rw-rw-r--   0 wilson    (1000) wilson    (1000)       74 2024-05-13 06:39:09.000000 sentry-stack-dingding-1.0.8/src/sentry_stack_dingding.egg-info/entry_points.txt
--rw-rw-r--   0 wilson    (1000) wilson    (1000)        1 2024-05-13 03:35:14.000000 sentry-stack-dingding-1.0.8/src/sentry_stack_dingding.egg-info/not-zip-safe
--rw-rw-r--   0 wilson    (1000) wilson    (1000)       23 2024-05-13 06:39:09.000000 sentry-stack-dingding-1.0.8/src/sentry_stack_dingding.egg-info/requires.txt
-drwxrwxr-x   0 wilson    (1000) wilson    (1000)        0 2024-05-13 06:39:09.000000 sentry-stack-dingding-1.0.8/src/sentry_dingding/
--rw-rw-r--   0 wilson    (1000) wilson    (1000)     2941 2024-05-13 06:38:59.000000 sentry-stack-dingding-1.0.8/src/sentry_dingding/plugin.py
--rw-rw-r--   0 wilson    (1000) wilson    (1000)       34 2024-05-13 06:39:03.000000 sentry-stack-dingding-1.0.8/src/sentry_dingding/__init__.py
--rw-rw-r--   0 wilson    (1000) wilson    (1000)      320 2024-05-13 02:34:05.000000 sentry-stack-dingding-1.0.8/src/sentry_dingding/forms.py
+drwxrwxr-x   0 wilson    (1000) wilson    (1000)        0 2024-05-13 07:07:19.000000 sentry-stack-dingding-1.0.9/
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)       38 2024-05-13 07:07:19.000000 sentry-stack-dingding-1.0.9/setup.cfg
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)     1044 2024-05-13 04:26:29.000000 sentry-stack-dingding-1.0.9/setup.py
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)      774 2024-05-13 03:32:44.000000 sentry-stack-dingding-1.0.9/README.md
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)     1549 2024-05-13 07:07:19.000000 sentry-stack-dingding-1.0.9/PKG-INFO
+drwxrwxr-x   0 wilson    (1000) wilson    (1000)        0 2024-05-13 07:07:19.000000 sentry-stack-dingding-1.0.9/src/
+drwxrwxr-x   0 wilson    (1000) wilson    (1000)        0 2024-05-13 07:07:19.000000 sentry-stack-dingding-1.0.9/src/sentry_stack_dingding.egg-info/
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)      453 2024-05-13 07:07:19.000000 sentry-stack-dingding-1.0.9/src/sentry_stack_dingding.egg-info/SOURCES.txt
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)       16 2024-05-13 07:07:19.000000 sentry-stack-dingding-1.0.9/src/sentry_stack_dingding.egg-info/top_level.txt
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)        1 2024-05-13 07:07:19.000000 sentry-stack-dingding-1.0.9/src/sentry_stack_dingding.egg-info/dependency_links.txt
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)     1549 2024-05-13 07:07:19.000000 sentry-stack-dingding-1.0.9/src/sentry_stack_dingding.egg-info/PKG-INFO
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)       74 2024-05-13 07:07:19.000000 sentry-stack-dingding-1.0.9/src/sentry_stack_dingding.egg-info/entry_points.txt
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)        1 2024-05-13 03:35:14.000000 sentry-stack-dingding-1.0.9/src/sentry_stack_dingding.egg-info/not-zip-safe
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)       23 2024-05-13 07:07:19.000000 sentry-stack-dingding-1.0.9/src/sentry_stack_dingding.egg-info/requires.txt
+drwxrwxr-x   0 wilson    (1000) wilson    (1000)        0 2024-05-13 07:07:19.000000 sentry-stack-dingding-1.0.9/src/sentry_dingding/
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)     3223 2024-05-13 07:07:01.000000 sentry-stack-dingding-1.0.9/src/sentry_dingding/plugin.py
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)       34 2024-05-13 07:07:11.000000 sentry-stack-dingding-1.0.9/src/sentry_dingding/__init__.py
+-rw-rw-r--   0 wilson    (1000) wilson    (1000)      320 2024-05-13 02:34:05.000000 sentry-stack-dingding-1.0.9/src/sentry_dingding/forms.py
```

### Comparing `sentry-stack-dingding-1.0.8/setup.py` & `sentry-stack-dingding-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `sentry-stack-dingding-1.0.8/README.md` & `sentry-stack-dingding-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `sentry-stack-dingding-1.0.8/PKG-INFO` & `sentry-stack-dingding-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-stack-dingding
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Sentry extension which send errors stats to DingDing
 Home-page: https://github.com/wilsonloo/sentry-stack-dingding.git
 Author: wilson-loo
 Author-email: 614231319@qq.com
 License: MIT
 Description: # Sentry-DingDing
```

### Comparing `sentry-stack-dingding-1.0.8/src/sentry_stack_dingding.egg-info/PKG-INFO` & `sentry-stack-dingding-1.0.9/src/sentry_stack_dingding.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-stack-dingding
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Sentry extension which send errors stats to DingDing
 Home-page: https://github.com/wilsonloo/sentry-stack-dingding.git
 Author: wilson-loo
 Author-email: 614231319@qq.com
 License: MIT
 Description: # Sentry-DingDing
```

### Comparing `sentry-stack-dingding-1.0.8/src/sentry_dingding/plugin.py` & `sentry-stack-dingding-1.0.9/src/sentry_dingding/plugin.py`

 * *Files 14% similar despite different names*

```diff
@@ -58,15 +58,20 @@
         stackDeep=self.get_option('stack_deep', group.project)
         # if event.data:
         #     if event.data["frames"]:
         #         stack = event.data["frames"]
         #     if event.data["stack"]:
         #         stack = event.data["stack"]
 
-        event_keys = vars(event).keys()
+        # project_id, event_id, _snuba_data, _group_id, _groups_cache, _group_ids, _data, _project_cache, interfaces, search_message, _group_cache
+        # event_keys = vars(event).keys()
+        # event_keys_str = ', '.join(event_keys)
+
+        interfaces = event.interfaces
+        event_keys = vars(interfaces).keys()
         event_keys_str = ', '.join(event_keys)
 
         # if stack:
         # # if event.frames and len(event.frames) > 0:
         # #     stack = event.frames[:stackDeep]
         #     stack = json.dumps(stack, indent=2)
```

