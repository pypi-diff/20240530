# Comparing `tmp/messages_local-0.0.62.tar.gz` & `tmp/messages_local-0.0.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "messages_local-0.0.62.tar", last modified: Wed May 29 10:44:57 2024, max compression
+gzip compressed data, was "messages_local-0.0.63.tar", last modified: Thu May 30 08:03:24 2024, max compression
```

## Comparing `messages_local-0.0.62.tar` & `messages_local-0.0.63.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:44:57.755840 messages_local-0.0.62/
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-29 10:44:57.755840 messages_local-0.0.62/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-29 10:44:19.000000 messages_local-0.0.62/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:44:57.751840 messages_local-0.0.62/messages_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:44:57.755840 messages_local-0.0.62/messages_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)    12323 2024-05-29 10:44:19.000000 messages_local-0.0.62/messages_local/src/MessagesLocal.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 10:44:19.000000 messages_local-0.0.62/messages_local/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:44:57.755840 messages_local-0.0.62/messages_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-29 10:44:57.000000 messages_local-0.0.62/messages_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-29 10:44:57.000000 messages_local-0.0.62/messages_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 10:44:57.000000 messages_local-0.0.62/messages_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-29 10:44:57.000000 messages_local-0.0.62/messages_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-29 10:44:57.000000 messages_local-0.0.62/messages_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-29 10:44:26.000000 messages_local-0.0.62/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 10:44:57.755840 messages_local-0.0.62/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-29 10:44:19.000000 messages_local-0.0.62/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:03:24.216506 messages_local-0.0.63/
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-30 08:03:24.216506 messages_local-0.0.63/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-30 08:02:35.000000 messages_local-0.0.63/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:03:24.216506 messages_local-0.0.63/messages_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:03:24.216506 messages_local-0.0.63/messages_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    12527 2024-05-30 08:02:35.000000 messages_local-0.0.63/messages_local/src/MessagesLocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 08:02:35.000000 messages_local-0.0.63/messages_local/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:03:24.216506 messages_local-0.0.63/messages_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-30 08:03:24.000000 messages_local-0.0.63/messages_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-30 08:03:24.000000 messages_local-0.0.63/messages_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 08:03:24.000000 messages_local-0.0.63/messages_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-30 08:03:24.000000 messages_local-0.0.63/messages_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-30 08:03:24.000000 messages_local-0.0.63/messages_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-30 08:02:46.000000 messages_local-0.0.63/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 08:03:24.216506 messages_local-0.0.63/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-30 08:02:35.000000 messages_local-0.0.63/setup.py
```

### Comparing `messages_local-0.0.62/PKG-INFO` & `messages_local-0.0.63/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: messages-local
-Version: 0.0.62
+Version: 0.0.63
 Home-page: https://github.com/circles-zone/messages-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: item-local>=0.0.9
 Requires-Dist: queue-worker-local>=0.0.37
 Requires-Dist: label-message-local>=0.0.4
-Requires-Dist: message-local>=0.0.140
+Requires-Dist: message-local>=0.0.144
 Requires-Dist: whatsapp-message-vonage-local>=0.0.19
 Requires-Dist: whataspp-message-inforu-local>=0.0.12
 Requires-Dist: sms-message-aws-sns-local>=0.0.35
 Requires-Dist: email-message-aws-ses-local>=0.0.13
 
 messages-local
```

### Comparing `messages_local-0.0.62/README.md` & `messages_local-0.0.63/README.md`

 * *Files identical despite different names*

### Comparing `messages_local-0.0.62/messages_local/src/MessagesLocal.py` & `messages_local-0.0.63/messages_local/src/MessagesLocal.py`

 * *Files 5% similar despite different names*

```diff
@@ -118,14 +118,15 @@
                   #  There is start_timestamp, when the message can be sent?
                   start_timestamp: datetime = datetime.now(),
                   importance: int = None,
                   requested_message_type: int = None,
                   sender_profile_id: int = None) -> None:
         """send method"""
 
+        # TODO recipient_list = Recipient.from_dicts(recipient_list_of_dicts or self.recipients) - Three changes
         recipients = Recipient.recipients_from_dicts(recipients or self.recipients)
         importance = MessageImportance(importance or self.default_importance)
         message_local = MessageLocal(message_id=message_id,
                                      original_body=self.default_original_body,
                                      original_subject=self.default_subject,
                                      campaign_id=campaign_id,
                                      recipients=recipients,
@@ -166,14 +167,16 @@
             message_id = message_local.message_id
             if not message_id:
                 raise Exception("Message ID is None")
             function_parameters_json = {
                 # Make sure send_sync accepts all these parameters.
                 "message_id": message_id,
                 "campaign_id": campaign_id,
+                 # TODO Recipient.to_dicts()
+                 # TODO cc_recipients suffix?
                 "cc_recipients": Recipient.recipients_to_dicts(cc_recipients),
                 "bcc_recipients": bcc_recipient.to_dict() if bcc_recipient else None,
                 "request_datetime": str(request_datetime),
                 "importance": importance.value,
                 "requested_message_type": requested_message_type.value if requested_message_type else None,
                 "start_timestamp": str(start_timestamp),
                 "sender_profile_id": sender_profile_id
```

### Comparing `messages_local-0.0.62/messages_local.egg-info/PKG-INFO` & `messages_local-0.0.63/messages_local.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: messages-local
-Version: 0.0.62
+Version: 0.0.63
 Home-page: https://github.com/circles-zone/messages-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: item-local>=0.0.9
 Requires-Dist: queue-worker-local>=0.0.37
 Requires-Dist: label-message-local>=0.0.4
-Requires-Dist: message-local>=0.0.140
+Requires-Dist: message-local>=0.0.144
 Requires-Dist: whatsapp-message-vonage-local>=0.0.19
 Requires-Dist: whataspp-message-inforu-local>=0.0.12
 Requires-Dist: sms-message-aws-sns-local>=0.0.35
 Requires-Dist: email-message-aws-ses-local>=0.0.13
 
 messages-local
```

### Comparing `messages_local-0.0.62/setup.py` & `messages_local-0.0.63/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-import setuptools
+import setuptools 
 
 PACKAGE_NAME = "messages-local"
 
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.62',  # https://pypi.org/project/messages-local
+    version='0.0.63',  # https://pypi.org/project/messages-local
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="messages-local",
@@ -20,14 +20,14 @@
         "License :: Other/Proprietary License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         "item-local>=0.0.9",
         "queue-worker-local>=0.0.37",
         "label-message-local>=0.0.4",
-        "message-local>=0.0.140",
+        "message-local>=0.0.144",
         "whatsapp-message-vonage-local>=0.0.19",
         "whataspp-message-inforu-local>=0.0.12",
         "sms-message-aws-sns-local>=0.0.35",
         "email-message-aws-ses-local>=0.0.13"
     ]
 )
```

