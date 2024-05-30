# Comparing `tmp/ebb_events-0.3.5.tar.gz` & `tmp/ebb_events-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebb_events-0.3.5.tar", max compression
+gzip compressed data, was "ebb_events-0.4.0.tar", max compression
```

## Comparing `ebb_events-0.3.5.tar` & `ebb_events-0.4.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1071 2024-05-06 20:14:00.489414 ebb_events-0.3.5/LICENSE
--rw-r--r--   0        0        0     9175 2024-05-28 22:43:36.277500 ebb_events-0.3.5/README.md
--rw-r--r--   0        0        0        0 2024-04-19 21:49:16.587650 ebb_events-0.3.5/ebb_events/__init__.py
--rw-r--r--   0        0        0     8886 2024-05-15 20:31:26.930793 ebb_events-0.3.5/ebb_events/builders/event_builder.py
--rw-r--r--   0        0        0    10777 2024-05-17 17:46:46.038249 ebb_events-0.3.5/ebb_events/consumers/event_consumer.py
--rw-r--r--   0        0        0      174 2024-04-22 19:12:51.110543 ebb_events-0.3.5/ebb_events/enums.py
--rw-r--r--   0        0        0      875 2024-05-20 19:44:17.150314 ebb_events-0.3.5/ebb_events/event_payload_utils.py
--rw-r--r--   0        0        0     3194 2024-05-20 19:44:17.150658 ebb_events-0.3.5/ebb_events/event_schema.py
--rw-r--r--   0        0        0      383 2024-05-06 17:16:47.746622 ebb_events-0.3.5/ebb_events/exceptions.py
--rw-r--r--   0        0        0      263 2024-05-14 16:56:47.898608 ebb_events-0.3.5/ebb_events/field_constants.py
--rw-r--r--   0        0        0      571 2024-05-28 22:43:36.277792 ebb_events-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     9673 1970-01-01 00:00:00.000000 ebb_events-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-06 20:14:00.489414 ebb_events-0.4.0/LICENSE
+-rw-r--r--   0        0        0     9175 2024-05-28 22:43:36.277500 ebb_events-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-19 21:49:16.587650 ebb_events-0.4.0/ebb_events/__init__.py
+-rw-r--r--   0        0        0    10050 2024-05-30 19:53:52.291574 ebb_events-0.4.0/ebb_events/builders/event_builder.py
+-rw-r--r--   0        0        0    10777 2024-05-17 17:46:46.038249 ebb_events-0.4.0/ebb_events/consumers/event_consumer.py
+-rw-r--r--   0        0        0      202 2024-05-30 19:53:52.291964 ebb_events-0.4.0/ebb_events/enums.py
+-rw-r--r--   0        0        0      875 2024-05-20 19:44:17.150314 ebb_events-0.4.0/ebb_events/event_payload_utils.py
+-rw-r--r--   0        0        0     3194 2024-05-20 19:44:17.150658 ebb_events-0.4.0/ebb_events/event_schema.py
+-rw-r--r--   0        0        0      383 2024-05-06 17:16:47.746622 ebb_events-0.4.0/ebb_events/exceptions.py
+-rw-r--r--   0        0        0      263 2024-05-14 16:56:47.898608 ebb_events-0.4.0/ebb_events/field_constants.py
+-rw-r--r--   0        0        0      571 2024-05-30 19:53:52.292335 ebb_events-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     9673 1970-01-01 00:00:00.000000 ebb_events-0.4.0/PKG-INFO
```

### Comparing `ebb_events-0.3.5/LICENSE` & `ebb_events-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ebb_events-0.3.5/README.md` & `ebb_events-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ebb_events-0.3.5/ebb_events/builders/event_builder.py` & `ebb_events-0.4.0/ebb_events/builders/event_builder.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging
 
 from datetime import datetime, timezone
 from marshmallow import ValidationError
 from typing import Optional
 from uuid import uuid4
 
+from ebb_events.enums import EventType
 from ebb_events.field_constants import (
     DATA,
     ID,
     METADATA,
     SOURCE,
     TIME,
     TYPE,
@@ -80,22 +81,26 @@
         if (
             datetime_raw.tzinfo is None
             or datetime_raw.tzinfo.utcoffset(datetime_raw) is None
         ):
             datetime_raw = datetime_raw.replace(tzinfo=timezone.utc)
         return datetime_raw.isoformat()
 
-    def build_event_topic(self) -> str:
+    def build_event_topic(self, is_heartbeat: bool = False) -> str:
         """
         Joins the EventEnvelope fields to form a valid topic string.
         Note: Fields are validated in __init__ so no need to re-validate here.
+
+        args:
+            is_heartbeat (bool): If True, replace event_type section of topic with EventType.HEARTBEAT.
+                                Defaults to False.
         Returns:
             str: _description_
         """
-        topic = f"{self.organization}/{self.system_id}/{self.event_type}/{self.subsystem_id}/{self.device_id}"
+        topic = f"{self.organization}/{self.system_id}/{self.event_type if is_heartbeat is False else EventType.HEARTBEAT.value}/{self.subsystem_id}/{self.device_id}"
         # This should be enforced by the ._validate() call and the EventEnvelopeSchema too
         if len(topic) > 256:
             logging.error(f"Invalid Topic. Topic too long: {topic}.")
             raise TopicFormatException("Topic length cannot exceed 256 characters.")
         return topic
 
     def build_event_payload_dict(
@@ -208,7 +213,31 @@
             message=message,
             serial_number=serial_number,
             metadata=metadata,
             datetime_obj=datetime_obj,
             remove_nones=remove_nones,
         )
         return json.dumps(payload_dict)
+
+    def build_event_heartbeat_payload_json(
+        self,
+        metadata: dict = {},
+    ) -> str:
+        """
+        Build a heartbeat event payload to publish
+
+        Args:
+            metadata (dict, optional): Dictionary containing extra metadata information to be included in the data. Defaults to {}.
+
+        Returns:
+            str: json payload for heartbeat messages to publish
+        """
+        # Build payload with {"alive": True} heartbeat data message
+        payload_dict = self.build_event_payload_dict(
+            message={"alive": True}, metadata=metadata
+        )
+
+        # Overwrite SOURCE and TYPE with heartbeat specific values
+        heartbeat_topic = self.build_event_topic(is_heartbeat=True)
+        payload_dict[SOURCE] = heartbeat_topic
+        payload_dict[TYPE] = EventType.HEARTBEAT.value
+        return json.dumps(payload_dict)
```

### Comparing `ebb_events-0.3.5/ebb_events/consumers/event_consumer.py` & `ebb_events-0.4.0/ebb_events/consumers/event_consumer.py`

 * *Files identical despite different names*

### Comparing `ebb_events-0.3.5/ebb_events/event_payload_utils.py` & `ebb_events-0.4.0/ebb_events/event_payload_utils.py`

 * *Files identical despite different names*

### Comparing `ebb_events-0.3.5/ebb_events/event_schema.py` & `ebb_events-0.4.0/ebb_events/event_schema.py`

 * *Files identical despite different names*

### Comparing `ebb_events-0.3.5/pyproject.toml` & `ebb_events-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ebb-events"
-version = "0.3.5"
+version = "0.4.0"
 description = "Package for building and standardizing MQTT event messages."
 authors = ["Ryan Bloom <ryan.bloom@ebbcarbon.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 marshmallow = "^3.21.1"
```

### Comparing `ebb_events-0.3.5/PKG-INFO` & `ebb_events-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebb-events
-Version: 0.3.5
+Version: 0.4.0
 Summary: Package for building and standardizing MQTT event messages.
 Author: Ryan Bloom
 Author-email: ryan.bloom@ebbcarbon.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

