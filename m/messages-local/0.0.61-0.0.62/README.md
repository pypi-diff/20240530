# Comparing `tmp/messages_local-0.0.61.tar.gz` & `tmp/messages_local-0.0.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "messages_local-0.0.61.tar", last modified: Tue May 28 07:22:43 2024, max compression
+gzip compressed data, was "messages_local-0.0.62.tar", last modified: Wed May 29 10:44:57 2024, max compression
```

## Comparing `messages_local-0.0.61.tar` & `messages_local-0.0.62.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:22:43.028712 messages_local-0.0.61/
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-28 07:22:43.028712 messages_local-0.0.61/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-28 07:21:57.000000 messages_local-0.0.61/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:22:43.024712 messages_local-0.0.61/messages_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:22:43.028712 messages_local-0.0.61/messages_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-05-28 07:21:57.000000 messages_local-0.0.61/messages_local/src/MessagesLocal.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 07:21:57.000000 messages_local-0.0.61/messages_local/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:22:43.028712 messages_local-0.0.61/messages_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-28 07:22:43.000000 messages_local-0.0.61/messages_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-28 07:22:43.000000 messages_local-0.0.61/messages_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 07:22:43.000000 messages_local-0.0.61/messages_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-28 07:22:43.000000 messages_local-0.0.61/messages_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-28 07:22:43.000000 messages_local-0.0.61/messages_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-28 07:22:04.000000 messages_local-0.0.61/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 07:22:43.028712 messages_local-0.0.61/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-28 07:21:57.000000 messages_local-0.0.61/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:44:57.755840 messages_local-0.0.62/
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-29 10:44:57.755840 messages_local-0.0.62/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-29 10:44:19.000000 messages_local-0.0.62/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:44:57.751840 messages_local-0.0.62/messages_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:44:57.755840 messages_local-0.0.62/messages_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    12323 2024-05-29 10:44:19.000000 messages_local-0.0.62/messages_local/src/MessagesLocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 10:44:19.000000 messages_local-0.0.62/messages_local/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:44:57.755840 messages_local-0.0.62/messages_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-29 10:44:57.000000 messages_local-0.0.62/messages_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-29 10:44:57.000000 messages_local-0.0.62/messages_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 10:44:57.000000 messages_local-0.0.62/messages_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-29 10:44:57.000000 messages_local-0.0.62/messages_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-29 10:44:57.000000 messages_local-0.0.62/messages_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-29 10:44:26.000000 messages_local-0.0.62/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 10:44:57.755840 messages_local-0.0.62/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-29 10:44:19.000000 messages_local-0.0.62/setup.py
```

### Comparing `messages_local-0.0.61/PKG-INFO` & `messages_local-0.0.62/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: messages-local
-Version: 0.0.61
+Version: 0.0.62
 Home-page: https://github.com/circles-zone/messages-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `messages_local-0.0.61/README.md` & `messages_local-0.0.62/README.md`

 * *Files identical despite different names*

### Comparing `messages_local-0.0.61/messages_local/src/MessagesLocal.py` & `messages_local-0.0.62/messages_local/src/MessagesLocal.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         return self.queue_worker
 
     @staticmethod
     def __send(recipient: Recipient, message_local: MessageLocal, importance: MessageImportance,
                campaign_id: int) -> list[int]:
         message_recipient_channel = message_local.get_message_channel(recipient)
         message_recipient_provider_id = message_local.get_message_provider_id(
-            message_channel_id=message_recipient_channel, recipient=recipient)
+            message_channel=message_recipient_channel, recipient=recipient)
         body = message_local.get_body_text_after_template_processing(recipient=recipient, message_channel=message_recipient_channel)
         if not body:
             return []
         init_kwargs = {}
         send_kwargs = {"body": body, "recipients": [recipient],
                        "compound_message_dict": message_local.get_compound_message_dict(channel=message_recipient_channel)}
         if (message_recipient_channel == MessageChannel.SMS and
```

### Comparing `messages_local-0.0.61/messages_local.egg-info/PKG-INFO` & `messages_local-0.0.62/messages_local.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: messages-local
-Version: 0.0.61
+Version: 0.0.62
 Home-page: https://github.com/circles-zone/messages-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `messages_local-0.0.61/setup.py` & `messages_local-0.0.62/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PACKAGE_NAME = "messages-local"
 
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.61',  # https://pypi.org/project/messages-local
+    version='0.0.62',  # https://pypi.org/project/messages-local
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="messages-local",
```

