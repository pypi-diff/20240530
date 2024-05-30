# Comparing `tmp/message-local-0.0.98.tar.gz` & `tmp/message-local-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "message-local-0.0.98.tar", last modified: Sun Feb 11 02:45:11 2024, max compression
+gzip compressed data, was "message-local-0.0.99.tar", last modified: Wed Feb 14 06:25:43 2024, max compression
```

## Comparing `message-local-0.0.98.tar` & `message-local-0.0.99.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 02:45:11.631105 message-local-0.0.98/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-02-11 02:45:11.631105 message-local-0.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-02-11 02:44:34.000000 message-local-0.0.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 02:45:11.631105 message-local-0.0.98/message_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 02:45:11.631105 message-local-0.0.98/message_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-02-11 02:44:34.000000 message-local-0.0.98/message_local/src/ChannelProviderConstants.py
--rw-r--r--   0 runner    (1001) docker     (127)    13107 2024-02-11 02:44:34.000000 message-local-0.0.98/message_local/src/CompoundMessage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-02-11 02:44:34.000000 message-local-0.0.98/message_local/src/GetTestIds.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-02-11 02:44:34.000000 message-local-0.0.98/message_local/src/MessageChannels.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-02-11 02:44:34.000000 message-local-0.0.98/message_local/src/MessageConstants.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-11 02:44:34.000000 message-local-0.0.98/message_local/src/MessageImportance.py
--rw-r--r--   0 runner    (1001) docker     (127)    16285 2024-02-11 02:44:34.000000 message-local-0.0.98/message_local/src/MessageLocal.py
--rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-02-11 02:44:34.000000 message-local-0.0.98/message_local/src/MessageTemplates.py
--rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-02-11 02:44:34.000000 message-local-0.0.98/message_local/src/Recipient.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-02-11 02:44:34.000000 message-local-0.0.98/message_local/src/SmsMessageLocal.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-11 02:44:34.000000 message-local-0.0.98/message_local/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 02:45:11.631105 message-local-0.0.98/message_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-02-11 02:45:11.000000 message-local-0.0.98/message_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-02-11 02:45:11.000000 message-local-0.0.98/message_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-11 02:45:11.000000 message-local-0.0.98/message_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-11 02:45:11.000000 message-local-0.0.98/message_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-11 02:45:11.000000 message-local-0.0.98/message_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-02-11 02:44:34.000000 message-local-0.0.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-11 02:45:11.635105 message-local-0.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-02-11 02:44:34.000000 message-local-0.0.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 06:25:43.289775 message-local-0.0.99/
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-02-14 06:25:43.289775 message-local-0.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-02-14 06:25:09.000000 message-local-0.0.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 06:25:43.285775 message-local-0.0.99/message_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 06:25:43.289775 message-local-0.0.99/message_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-02-14 06:25:09.000000 message-local-0.0.99/message_local/src/ChannelProviderConstants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14357 2024-02-14 06:25:09.000000 message-local-0.0.99/message_local/src/CompoundMessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-02-14 06:25:09.000000 message-local-0.0.99/message_local/src/GetTestIds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-02-14 06:25:09.000000 message-local-0.0.99/message_local/src/MessageChannels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-02-14 06:25:09.000000 message-local-0.0.99/message_local/src/MessageConstants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-14 06:25:09.000000 message-local-0.0.99/message_local/src/MessageImportance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15347 2024-02-14 06:25:09.000000 message-local-0.0.99/message_local/src/MessageLocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9494 2024-02-14 06:25:09.000000 message-local-0.0.99/message_local/src/MessageTemplates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-02-14 06:25:09.000000 message-local-0.0.99/message_local/src/Recipient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-02-14 06:25:09.000000 message-local-0.0.99/message_local/src/SmsMessageLocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 06:25:09.000000 message-local-0.0.99/message_local/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 06:25:43.289775 message-local-0.0.99/message_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-02-14 06:25:43.000000 message-local-0.0.99/message_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-02-14 06:25:43.000000 message-local-0.0.99/message_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 06:25:43.000000 message-local-0.0.99/message_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-02-14 06:25:43.000000 message-local-0.0.99/message_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-14 06:25:43.000000 message-local-0.0.99/message_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-02-14 06:25:09.000000 message-local-0.0.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-14 06:25:43.289775 message-local-0.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-02-14 06:25:09.000000 message-local-0.0.99/setup.py
```

### Comparing `message-local-0.0.98/PKG-INFO` & `message-local-0.0.99/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: message-local
-Version: 0.0.98
+Version: 0.0.99
 Home-page: https://github.com/circles-zone/message-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -12,9 +12,10 @@
 Requires-Dist: api-management-local>=0.0.39
 Requires-Dist: language-local
 Requires-Dist: variable-local
 Requires-Dist: logger-local
 Requires-Dist: database-mysql-local>=0.0.199
 Requires-Dist: star-local
 Requires-Dist: profiles-local>=0.0.50
+Requires-Dist: phones-local
 
 message-local
```

### Comparing `message-local-0.0.98/README.md` & `message-local-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `message-local-0.0.98/message_local/src/CompoundMessage.py` & `message-local-0.0.99/message_local/src/CompoundMessage.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,95 +8,113 @@
 from variable_local.template import ReplaceFieldsWithValues
 
 from .MessageChannels import MessageChannel
 from .MessageConstants import object_message
 from .MessageTemplates import MessageTemplates
 from .Recipient import Recipient
 
-
-
 lang_code_cache = {}
+JSON_VERSION = "240214"  # TODO: make it generic
+
 
 class CompoundMessage(GenericCRUD, metaclass=MetaLogger, object=object_message):
     def __init__(self, campaign_id: int = None, message_template_id: int = None, body: str = None, subject: str = None,
-                 recipients: list[Recipient] = None, message_id: int = None, is_test_data: bool = False, ui_schema=None,schema=None,field_id=None):
-        self.user_context=UserContext.login_using_user_identification_and_password()
+                 recipients: list[Recipient] = None, message_id: int = None, is_test_data: bool = False, ui_schema=None,
+                 schema=None, field_id=None):
+        self.user_context = UserContext()
         super().__init__(default_schema_name="message", default_table_name="message_table",
                          default_view_table_name="message_view", default_id_column_name="message_id",
                          is_test_data=is_test_data)
 
         self.campaign_id = campaign_id
         self.message_template_id = message_template_id
         self.body = body
         self.subject = subject
         self.recipients = recipients
         self.message_id = message_id
         self.__compound_message = {}
-        self.ui_schema=ui_schema
-        self.schema=schema
-        self.field_id=field_id
+        self.ui_schema = ui_schema
+        self.schema = schema
+        self.field_id = field_id
         self.profile_local = ProfilesLocal()
         self.message_template = MessageTemplates()
         self.set_compound_message_after_text_template()
-        
 
     def _get_template_ids_by_campaign(self, campaign_id: int) -> list[int]:
         """Returns a random template id from the campaign"""
 
         possible_template_ids = self.select_multi_tuple_by_id(
             schema_name="campaign", view_table_name="campaign_view",
             id_column_name="campaign_id", id_column_value=campaign_id,
             select_clause_value="message_template_id")
 
-        possible_template_ids = [message_template_id[0] for message_template_id in possible_template_ids]
-
-        return possible_template_ids
+        return [message_template_id[0] for message_template_id in possible_template_ids]
 
+    # TODO: {
+    #   "json_version": ...,
+    #   "data": {
+    #     "formId": ...,
+    #     "formName": ...,
+    #     "messageTemplates": [
+    #     {
+    #         "messageTemplateId": ...,
+    #         "compoundMessages": [...]
     def set_compound_message_after_text_template(
             self, campaign_id: int = None, message_template_id: int = None, body: str = None, subject: str = None,
             recipients: list[Recipient] = None, message_id: int = None) -> None:
-        """ Sets the compound message in the instance and in the database using the following structure:
-    {
-    'json_version': '110224',
-    'data': {
-        'DEFAULT': {
-            'bodyBlocks': [{
-                'blockId': ...,
-                'blockTypeId': ...,
-                'blockTypeName': ...,
-                'questionId': ...,
-                'questionTypeId': ...,
-                'questionTitle': ...,
-                'questionTypeName': ...,
-                'profileBlocks': [{'profileId': ..., 'template': ..., 'processedTemplate': ...}, ...]
-            }, ...],
-
-            'subjuctBlocks': [{...}]  // same as body
-        },
-
-        'EMAIL': {...},  // same as default
-        'SMS': {...},
-        'WHATSAPP': {...}
-        }
-    }
-        """
+        """ Sets the compound message in the instance and in the database using the following structure:"""
+
+        #     {
+        #         # "compoundMessageId": ...,
+        #         "DEFAULT": {
+        #             "bodyBlocks": [
+        #                 {
+        #                     "blockId": ...,
+        #                     "blockTypeId": ...,
+        #                     "blockTypeName": ...,
+        #                     "questionTitle": ...,
+        #                     "questionTypeName": ...,
+        #                     "questionId": ...,
+        #                     "questionTypeId": ...,
+        #                     "answerExpirationDays": ...,
+        #                     "tableId": ...,
+        #                     "variableId": ...,
+        #                     "whereStatement": ...,
+        #                     "isVisible": ...,
+        #                     "isRequired": ...,
+        #                     "defaultValue": ...,
+        #                     "labelQuestionId": ...,
+        #                     "template": ...,
+        #                     "profileBlocks": [
+        #                         {"profileId": ..., "processedTemplate": ...},
+        #                         {"profileId": ..., "processedTemplate": ...},
+        #                     ]
+        #                 },
+        #                 {"blockId": ...}
+        #             ],
+        #             "subjectBlock": {"blockId": ...}  # same structure as one bodyBlock
+        #         },
+        #         "EMAIL": {"bodyBlocks": [...], "subjectBlock": {...}},  # same structure as DEFAULT
+        #         "SMS": {},
+        #         "WHATSAPP": {}
+        #     }
 
         # Allow overiding instance vars
         campaign_id = campaign_id or self.campaign_id
         message_template_id = message_template_id or self.message_template_id
         body = body or self.body
         subject = subject or self.subject
         recipients = recipients or self.recipients or []
         message_id = message_id or self.message_id
 
-        data = {"DEFAULT": {},
-                "WEB": {},
-                "EMAIL": {},
-                "SMS": {},
-                "WHATSAPP": {}
+        data = {"DEFAULT": {"bodyBlocks": [], "subjectBlock": {}},
+                "WEB": {"bodyBlocks": [], "subjectBlock": {}},
+                "EMAIL": {"bodyBlocks": [], "subjectBlock": {}},
+                "SMS": {"bodyBlocks": [], "subjectBlock": {}},
+                "WHATSAPP": {"bodyBlocks": [], "subjectBlock": {}}
                 }
 
         channels_mapping = {
             MessageChannel.SMS.name: {"body": "sms_body_template", "subject": None},
             MessageChannel.EMAIL.name: {"body": "email_body_html_template", "subject": "email_subject_template"},
             MessageChannel.WHATSAPP.name: {"body": "whatsapp_body_template", "subject": None},
             "DEFAULT": {"body": "default_body_template", "subject": "default_subject_template"},
@@ -121,21 +139,29 @@
             criteria_json, recipients)
         self.logger.info(object={"textblocks_and_attributes": textblocks_and_attributes,
                                  "criteria_json": criteria_json})
 
         for message_template_textblock_and_attributes in textblocks_and_attributes:
             for message_channel, template_header in channels_mapping.items():
                 for part in ("body", "subject"):
-                    if f"{part}Blocks" not in data[message_channel]:
-                        data[message_channel][f"{part}Blocks"] = []
+                    templates = [x for x in (message_template_textblock_and_attributes.get(template_header[part]),
+                                             message_template_textblock_and_attributes.get("questionTitle"))
+                                 if x]
+
+                    message_template = " ".join(templates)
+                    if not message_template:
+                        self.logger.warning("message_template is empty", object={
+                            "message_template_textblock_and_attributes": message_template_textblock_and_attributes})
+                        continue
 
                     block = {
                         "blockId": message_template_textblock_and_attributes.get("blockId"),
                         "blockTypeId": message_template_textblock_and_attributes.get("blockTypeId"),
                         "blockTypeName": message_template_textblock_and_attributes.get("blockTypeName"),
+                        "template": message_template,
                         "questionTitle": message_template_textblock_and_attributes.get("questionTitle"),
                         "questionTypeName": message_template_textblock_and_attributes.get("questionTypeName"),
                         # from question_view:
                         "questionId": message_template_textblock_and_attributes.get("questionId"),
                         "questionTypeId": message_template_textblock_and_attributes.get("questionTypeId"),
                         "answerExpirationDays": message_template_textblock_and_attributes.get("answerExpirationDays"),
                         "tableId": message_template_textblock_and_attributes.get("tableId"),
@@ -143,114 +169,99 @@
                         "whereStatement": message_template_textblock_and_attributes.get("whereStatement"),
                         "isVisible": message_template_textblock_and_attributes.get("isVisible"),
                         "isRequired": message_template_textblock_and_attributes.get("isRequired"),
                         "defaultValue": message_template_textblock_and_attributes.get("defaultValue"),
                         "labelQuestionId": message_template_textblock_and_attributes.get("labelQuestionId"),
                         "profileBlocks": []
                     }
-                    templates = [x for x in (message_template_textblock_and_attributes.get(template_header[part]),
-                                             message_template_textblock_and_attributes.get("questionTitle"))
-                                 if x]
 
-                    message_template = " ".join(templates)
-                    if not message_template:
-                        self.logger.warning("message_template is empty", object={
-                            "message_template_textblock_and_attributes": message_template_textblock_and_attributes})
-                        continue
                     for recipient in recipients:
                         if recipient.get_profile_id() not in lang_code_cache:
                             lang_code_cache[
                                 recipient.get_profile_id()] = self.profile_local.get_preferred_lang_code_by_profile_id(
                                 recipient.get_profile_id()).value
-                        # TODO: critiria doesn't match the recipient
+                        # TODO: The test critiria doesn't match the recipient
                         if 1 or (any(recipient.get_profile_id() == potential_recipient["profile_id"]
                                      for potential_recipient in potentials_recipients)
                                  # TODO recipient_preferred_lang_code_str
-                                 and lang_code_cache[
-                                     recipient.get_profile_id()] == message_template_textblock_and_attributes.get(
-                                    "langCode")):
+                                 and (lang_code_cache[recipient.get_profile_id()] ==
+                                      message_template_textblock_and_attributes.get("langCode"))):
                             block["profileBlocks"].append(
                                 # each profile has its own template, because of the language
                                 {"profileId": recipient.get_profile_id(),
-                                 "template": message_template,
                                  "processedTemplate": self._process_text_block(message_template, recipient=recipient),
                                  })
-                    data[message_channel][f"{part}Blocks"].append(block)
+                    if part == "subject":
+                        # ignore if already set
+                        data[message_channel]["subjectBlock"] = data[message_channel]["subjectBlock"] or block
+                    else:
+                        data[message_channel][f"{part}Blocks"].append(block)
 
-        # TODO: make it generic
-        compound_message = {"json_version": "110224", "data": data}
+        compound_message = {"json_version": JSON_VERSION, "data": data}
         # save in message table
         if message_id:
             self.update_by_id(id_column_value=message_id,
                               data_json={"compound_message_json": json.dumps(compound_message),
                                          "compound_message": json.dumps(compound_message)})
         else:
             self.message_id = self.insert(data_json={"compound_message_json": json.dumps(compound_message),
                                                      "compound_message": json.dumps(compound_message)})
 
         self.__compound_message = compound_message
+        self.logger.debug(object=locals())
 
     def _process_text_block(self, text_block_body: str, recipient: Recipient) -> str:
-
         template = ReplaceFieldsWithValues(message=text_block_body,
                                            # TODO language -> lang_code_str ?
                                            language=recipient.get_preferred_lang_code_str(),
                                            variable=recipient.get_profile_variables())
         processed_text_block = template.get_variable_values_and_chosen_option(
             profile_id=self.user_context.get_effective_profile_id(),
             # TODO profile_id -> effective_profile_id
             kwargs={"recipient.first_name": recipient.get_first_name(),
-                    # TODO real -> effective
+                    # TODO: effective -> real in user_context
                     "sender.first_name": self.user_context.get_real_first_name(),
                     "message_id": self.message_id
                     })
         return processed_text_block
 
     def get_compound_message_dict(self, channel: MessageChannel = None) -> dict:
-
-        compound_message = {}
         if channel is None:
-            compound_message = self.__compound_message["data"]
+            return self.__compound_message["data"]
         else:
-            compound_message["DEFAULT"] = self.__compound_message["data"]["DEFAULT"]
-            compound_message[channel.name] = self.__compound_message["data"][channel.name]
-
-        return compound_message
+            return {"DEFAULT": self.__compound_message["data"]["DEFAULT"],
+                    channel.name: self.__compound_message["data"][channel.name]}
 
     def get_compound_message_str(self, channel: MessageChannel = None) -> str:
         return json.dumps(self.get_compound_message_dict(channel=channel))
 
     def get_profile_block(self, profile_id: int, channel: MessageChannel, part: str = "body") -> dict:
         """Returns a dict with the following keys:
         profileId, template, processedTemplate, blockId, blockTypeId, blockTypeName, questionId,
             questionTypeId, questionTitle, questionTypeName
         """
 
         assert part in ("body", "subject")
-        blocks = self.__compound_message["data"].get(channel.name, {}).get(f"{part}Blocks", [])
+        key = "bodyBlocks" if part == "body" else "subjectBlock"
+        blocks = self.__compound_message["data"].get(channel.name, {}).get(key, [])
         for block in blocks:
             for _profile_block in block.get("profileBlocks", []):
                 if _profile_block.get("profileId") == profile_id:
-                    profile_block = {**_profile_block, **{k: v for k, v in block.items()
-                                                          if k != "profileBlocks"}}
-
-                    return profile_block
-
+                    return {**_profile_block, **{k: v for k, v in block.items() if k != "profileBlocks"}}
         return {}
 
     def get_message_fields(self) -> dict:
         if self.recipients:
             recipients_mapping = {recipient.get_profile_id(): recipient.to_json() for recipient in self.recipients}
         else:
             recipients_mapping = {}
-        obj = {
+        return {
             "campaign_id": self.campaign_id,
             "body": self.body,
             "subject": self.subject,
             "message_id": self.message_id,
             "ui_schema": self.ui_schema,
             "schema": self.schema,
             "field_id": self.field_id,
             "recipients": recipients_mapping,
-            "json_version": 3,
+            "json_version": JSON_VERSION,
         }
-        return obj
```

### Comparing `message-local-0.0.98/message_local/src/GetTestIds.py` & `message-local-0.0.99/message_local/src/GetTestIds.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,17 +9,17 @@
     def __init__(self):
         super().__init__(default_schema_name="message", default_table_name="message_table",
                          default_view_table_name="message_outbox_view", default_id_column_name="message_id")
 
     def insert_message(self, **kwargs) -> int:
         """Inserts a message into the database"""
         data_json = {}
-        for arg in kwargs.items():
-            if arg[1] is not None:
-                data_json[arg[0]] = arg[1]
+        for key, value in kwargs.items():
+            if value is not None:
+                data_json[key] = value
 
         message_id = self.insert(schema_name="message", data_json=data_json)
         return message_id
 
     def get_test_message_id(self) -> int:
         return self.get_test_entity_id(entity_name="message",
                                        insert_function=self.insert_message)
```

### Comparing `message-local-0.0.98/message_local/src/MessageConstants.py` & `message-local-0.0.99/message_local/src/MessageConstants.py`

 * *Files identical despite different names*

### Comparing `message-local-0.0.98/message_local/src/MessageLocal.py` & `message-local-0.0.99/message_local/src/MessageLocal.py`

 * *Files 8% similar despite different names*

```diff
@@ -115,16 +115,16 @@
             return self.channel_ids_per_recipient[recipient.get_profile_id()]
         else:
             return self.get_msg_type(recipient)
 
     @staticmethod
     def get_message_provider_id(message_channel_id: MessageChannel, recipient: Recipient) -> int:
         """return message provider"""
-
-        if message_channel_id == MessageChannel.SMS and recipient.get_normizalied_phone().startswith("972"):
+        # TODO: implement the logic for the provider_id (remove +972, etc.)
+        if message_channel_id == MessageChannel.SMS and recipient.get_normizalied_phone().startswith("+972"):
             provider_id = AWS_SNS_SMS_MESSAGE_PROVIDER_ID
         elif message_channel_id == MessageChannel.EMAIL:
             provider_id = AWS_SES_EMAIL_MESSAGE_PROVIDER_ID
         elif message_channel_id == MessageChannel.WHATSAPP:
             # TODO: or vonage
             provider_id = INFORU_MESSAGE_PROVIDER_ID
         else:
@@ -133,14 +133,15 @@
         return provider_id
 
     def get_body_after_text_template(self, recipient: Recipient,
                                      message_channel: MessageChannel = None) -> str:
         # TODO: is this the right way to do it?
         if message_channel is None:
             message_channel = self.get_message_channel(recipient)
+            self.logger.debug("message_channel: " + str(message_channel))
 
         body = ""
         for block in self.get_compound_message_dict(message_channel)[message_channel.name]["bodyBlocks"]:
             for profile_block in block["profileBlocks"]:
                 if profile_block["profileId"] == recipient.get_profile_id():
                     body += profile_block["processedTemplate"] + "\n"
         return body
@@ -220,15 +221,14 @@
             )
             if arr is None:
                 self.__used_cache = False
                 if api_check == APILimitStatus.BETWEEN_SOFT_LIMIT_AND_HARD_LIMIT:
                     self.logger.warn("You passed the soft limit")
                 if api_check != APILimitStatus.GREATER_THAN_HARD_LIMIT:
                     try:
-                        # user = user_context.login_using_user_identification_and_password(outgoing_body)
                         http_status_code = http.HTTPStatus.OK.value
                     except Exception as exception:
                         self.logger.exception(object=exception)
                         http_status_code = http.HTTPStatus.BAD_REQUEST.value
                 else:
                     self.logger.info("You passed the hard limit")
                     x = self.api_management_manager.seconds_to_sleep_after_passing_the_hard_limit(
@@ -294,27 +294,7 @@
 
     def get_importance(self) -> MessageImportance:
         """get method"""
         return self.importance
 
     def get_recipients(self) -> List[Recipient]:
         return self.__recipients
-
-    # def get_message_template_dict_by_campaign_id(self, campaign_id: int) -> dict:
-    #     """Returns [lang_code (such as 'en'):
-    #                 {'sms_body_template': ..., 'email_subject_template': ...,
-    #                     'email_body_html_template': ..., 'whatsapp_body_template': ...
-    #                 }, ...
-    #                ]"""
-    #     
-    #     if campaign_id is None:
-    #         return {}
-    #     query = "SELECT * FROM campaign_message_template.campaign_message_template_table " \
-    #             "JOIN message_template.message_template_ml_table" \
-    #             "WHERE campaign_id = %s"
-    #     query_parameters = (campaign_id,)
-    #     self.cursor.execute(query, query_parameters)
-    #     columns = [column[0] for column in self.cursor.description]
-    #     results = [dict(zip(columns, row)) for row in self.cursor.fetchall()]
-    #     results = {row["lang_code"]: row for row in results}
-    #     
-    #     return results
```

### Comparing `message-local-0.0.98/message_local/src/MessageTemplates.py` & `message-local-0.0.99/message_local/src/MessageTemplates.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from logger_local.MetaLogger import MetaLogger
 
 from .MessageConstants import object_message
 from .Recipient import Recipient
 
 cache = {}
 
-
 class MessageTemplates(GenericCRUDML, metaclass=MetaLogger, object=object_message):
     def __init__(self):
         super().__init__(default_schema_name="field", default_table_name="field_table")
 
     def get_potentials_recipients(self, criteria_json: dict, recipients: list[Recipient] = None) -> list[dict]:
         where = self.get_where_by_criteria_json(criteria_json)
         if recipients:
@@ -19,20 +18,18 @@
         query_for_potentials_recipients = f"""
 SELECT DISTINCT user_id, person_id, user_main_email_address, user.profile_id AS profile_id, 
    profile_phone_full_number_normalized, profile_preferred_lang_code
  FROM user.user_general_view AS user
     JOIN group_profile.group_profile_view AS group_profile on group_profile.profile_id = user.profile_id
   WHERE {where} 
 """
-        if "get_potential_receipients" not in cache:
-            columns = ("user_id, person_id, user_main_email_address, profile_id,"
-                       "profile_phone_full_number_normalized, profile_preferred_lang_code")
-            self.cursor.execute(query_for_potentials_recipients)
-            cache["get_potential_receipients"] = [self.convert_to_dict(row, columns) for row in self.cursor.fetchall()]
-        return cache["get_potential_receipients"]
+        columns = ("user_id, person_id, user_main_email_address, profile_id,"
+                   "profile_phone_full_number_normalized, profile_preferred_lang_code")
+        self.cursor.execute(query_for_potentials_recipients)
+        return [self.convert_to_dict(row, columns) for row in self.cursor.fetchall()]
 
     def get_where_by_criteria_json(self, criteria_json: dict) -> str:
         # TODO add support to user_external_id in criteria_json
         min_age = criteria_json.get("min_age")
         max_age = criteria_json.get("max_age")
         gender_list_id = criteria_json.get("gender_list_id")
         group_list_id = criteria_json.get("group_list_id")
```

### Comparing `message-local-0.0.98/message_local/src/Recipient.py` & `message-local-0.0.99/message_local/src/Recipient.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 from enum import Enum, auto
 
-from user_context_remote.user_context import UserContext
+from phones_local.phones_local import PhonesLocal
 from variable_local.variable import VariablesLocal
 
 
 # TODO Each of them has field_id value in field.field_table, shall we use it?
 #   (I didn't find it there)
 class ReferenceType(Enum):
     PERSON_ID = auto()
@@ -33,15 +33,14 @@
         self.__telephone_number = telephone_number
         self.__preferred_lang_code_str = preferred_lang_code_str
         self.__first_name = first_name
         for key, value in self.to_json().items():
             if not key.endswith("id") and key.upper() in RecipientType.__members__:
                 self._recipient_type = RecipientType[key.upper()]  # remove the first underscore
 
-        self.user = UserContext()
         self.__variable_local: VariablesLocal | None = None  # To improve performance, we will get it only when needed.
 
     def get_profile_variables(self) -> VariablesLocal:
         if self.__variable_local is not None:
             return self.__variable_local
         self.__variable_local = VariablesLocal()
         # TODO: make sure those are stored on the effective_profile_id (using global user_context or sending the user_context).
@@ -80,31 +79,21 @@
     def get_telephone_address(self):
         return self.__telephone_number is not None
 
     def get_preferred_lang_code_str(self):
         return self.__preferred_lang_code_str
 
     # TODO Is there a package/library for this that we can use?
-    def get_normizalied_phone(self):
+    def get_normizalied_phone(self, region: str = "IL"):
         """ normalized/canonical phone, telephone number """
         # TODO I think this function does not cover all cases - I believe we can find one on the internet - I think Sahar found one.
         if self.__telephone_number is None:
             return None
-        if self.__telephone_number.startswith("+"):
-            country_code = ""
-        else:
-            # TODO county_code and country_id are two different things
-            country_code = self.user.get_country_code()
+        return PhonesLocal.normalize_phone_number(self.__telephone_number, region)['full_number_normalized']
 
-        # Remove non-numeric characters from the telephone number and leading zeroes
-        cleaned_number = int(''.join(char for char in self.__telephone_number if char.isdigit()))
-
-        cleaned_number = f"{country_code}{cleaned_number}"
-
-        return cleaned_number
 
     def to_json(self):
         init_args = ("contact_id", "person_id", "user_id", "profile_id", "telephone_number",
                      "email_address_str", "preferred_lang_code_str", "first_name")
         return {k.replace("_Recipient__", ""): v for k, v in self.__dict__.items()
                 if v is not None and k.replace("_Recipient__", "") in init_args}
```

### Comparing `message-local-0.0.98/message_local.egg-info/PKG-INFO` & `message-local-0.0.99/message_local.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: message-local
-Version: 0.0.98
+Version: 0.0.99
 Home-page: https://github.com/circles-zone/message-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -12,9 +12,10 @@
 Requires-Dist: api-management-local>=0.0.39
 Requires-Dist: language-local
 Requires-Dist: variable-local
 Requires-Dist: logger-local
 Requires-Dist: database-mysql-local>=0.0.199
 Requires-Dist: star-local
 Requires-Dist: profiles-local>=0.0.50
+Requires-Dist: phones-local
 
 message-local
```

### Comparing `message-local-0.0.98/message_local.egg-info/SOURCES.txt` & `message-local-0.0.99/message_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `message-local-0.0.98/pyproject.toml` & `message-local-0.0.99/pyproject.toml`

 * *Files identical despite different names*

### Comparing `message-local-0.0.98/setup.py` & `message-local-0.0.99/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "message-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/message-local
-    version='0.0.98',
+    version='0.0.99',
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="message-local",
@@ -23,9 +23,10 @@
                       "api-management-local>=0.0.39",  # https://pypi.org/project/api-management-local/
                       "language-local",
                       "variable-local",
                       "logger-local",
                       "database-mysql-local>=0.0.199",
                       "star-local",
                       "profiles-local>=0.0.50",
+                      "phones-local"
                       ]
 )
```

