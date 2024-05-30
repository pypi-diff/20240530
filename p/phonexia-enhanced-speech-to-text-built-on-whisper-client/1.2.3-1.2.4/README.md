# Comparing `tmp/phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.3.tar.gz` & `tmp/phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.3.tar", max compression
+gzip compressed data, was "phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.4.tar", max compression
```

## Comparing `phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.3.tar` & `phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.4.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     8232 2024-05-13 11:07:44.890236 phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.3/phonexia_enhanced_speech_to_text_built_on_whisper_client.py
--rw-r--r--   0        0        0     1118 2024-05-13 11:07:44.890236 phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.3/pypi-README.md
--rw-r--r--   0        0        0     2062 2024-05-13 11:08:20.704742 phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0     7954 2024-05-30 13:19:47.154836 phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.4/phonexia_enhanced_speech_to_text_built_on_whisper_client.py
+-rw-r--r--   0        0        0     1118 2024-05-30 13:19:47.154836 phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.4/pypi-README.md
+-rw-r--r--   0        0        0     2072 2024-05-30 13:20:11.263179 phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.4/PKG-INFO
```

### Comparing `phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.3/phonexia_enhanced_speech_to_text_built_on_whisper_client.py` & `phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.4/phonexia_enhanced_speech_to_text_built_on_whisper_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import argparse
+import json
 import logging
 import os
 from enum import Enum
 from typing import Iterator, Optional
 
 import google.protobuf.duration_pb2
 import grpc
+from google.protobuf.json_format import MessageToDict
+
 import phonexia.grpc.technologies.enhanced_speech_to_text_built_on_whisper.v1.enhanced_speech_to_text_built_on_whisper_pb2_grpc as stt_grpc
 from phonexia.grpc.common.core_pb2 import Audio, TimeRange
 from phonexia.grpc.technologies.enhanced_speech_to_text_built_on_whisper.v1.enhanced_speech_to_text_built_on_whisper_pb2 import (
     TranscribeConfig,
     TranscribeRequest,
     TranslateConfig,
     TranslateRequest,
@@ -22,15 +25,15 @@
     transcribe = "transcribe"
     translate = "translate"
 
     def __str__(self):
         return self.value
 
 
-def time_to_duration(time: float) -> google.protobuf.duration_pb2.Duration | None:
+def time_to_duration(time: float) -> Optional[google.protobuf.duration_pb2.Duration]:
     if time is None:
         return None
     duration = google.protobuf.duration_pb2.Duration()
     duration.seconds = int(time)
     duration.nanos = int((time - duration.seconds) * 1e9)
     return duration
 
@@ -107,45 +110,40 @@
                 enable_language_switching=enable_language_switching,
             ),
             metadata=metadata,
         )
     else:
         raise RuntimeError("Unknown task")
 
-    warning_message = []
+    info_message = []
+    response_dict = None
     for _response in response:
+        if not response_dict:
+            response_dict = MessageToDict(_response)
+        else:
+            response_dict["result"]["oneBest"]["segments"] += \
+                MessageToDict(_response)["result"]["oneBest"]["segments"]  # fmt: skip
+
         for segment in _response.result.one_best.segments:
-            print(
-                f"[{segment.start_time.ToJsonString()} -> {segment.end_time.ToJsonString()} "
-                + (
-                    f"{segment.language}"
-                    if task == Task.transcribe
-                    else f"{segment.source_language} -> {segment.language}"
-                )
-                + f"] {segment.text}"
-            )
             if segment.source_language != segment.detected_source_language:
-                warning_message.append(
-                    f"Language '{segment.detected_source_language}' was detected, but the license does not support this language. "
-                    f"Instead the segment was {'transcribed' if task == Task.transcribe else 'translated'} with the "
+                info_message.append(
+                    f"Language '{segment.detected_source_language}' was detected in the audio, but instead "
+                    f"the segment was {'transcribed' if task == Task.transcribe else 'translated'} with the "
                     + (
                         f"closest available source language '{segment.source_language}'"
                         if language is None
-                        else f"language '{language}' that was enforced by argument '--language'"
+                        else f"language '{language}' that was enforced by the '--language' argument"
                     )
-                    + ". For more info on this problem don't hesitate to contact Phonexia."
                 )
-        if _response.HasField("processed_audio_length"):
-            print(f"Processed audio length: {_response.processed_audio_length.ToJsonString()}")
 
-    warning_message = set(warning_message)
-    if len(warning_message) > 0:
-        print()
-        for warning in warning_message:
-            print(f"WARNING: {warning}")
+    print(json.dumps(response_dict, indent=2, ensure_ascii=False))
+    info_message = set(info_message)
+    if len(info_message) > 0:
+        for msg in info_message:
+            logging.info(msg)
 
 
 def main():
     parser = argparse.ArgumentParser(
         description=(
             "Enhanced Speech to Text Built on Whisper gRPC client. Transcribes input audio into segments"
             " with timestamps."
```

### Comparing `phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.3/pypi-README.md` & `phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.4/pypi-README.md`

 * *Files identical despite different names*

### Comparing `phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.3/pyproject.toml` & `phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "phonexia-enhanced-speech-to-text-built-on-whisper-client"
-version = "1.2.3"
+version = "1.2.4"
 description = "Client for communication with Phonexia Enhanced Speech To Text Built On Whisper microservice."
 readme = "pypi-README.md"
 keywords = ["grpc", "transcription", "STT", "ASR", "speech to text", "speech", "language", "microservice"]
 authors = ["Phonexia <info@phonexia.com>"]
 
 [tool.poetry.urls]
 Homepage = "https://phonexia.com"
@@ -13,15 +13,15 @@
 
 [tool.poetry.scripts]
 enhanced_speech_to_text_built_on_whisper_client = 'phonexia_enhanced_speech_to_text_built_on_whisper_client:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 grpcio = "^1.54.0"
-phonexia-grpc = {version="^1.0.0", source="pypi"}
+phonexia-grpc = {version="^2.0.0", source="pypi"}
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.0"
 pytest-cov = "^5.0.0"
 pytest-env = "^1.0.0"
 pytest-random-order = "^1.1.0"
 black = "^24.0.0"
@@ -46,15 +46,15 @@
 target-version = ['py38']
 preview = true
 
 [tool.ruff]
 target-version = "py38"
 line-length = 100
 fix = true
-select = [
+lint.select = [
     # flake8-2020
     "YTT",
     # flake8-bandit
     "S",
     # flake8-bugbear
     "B",
     # flake8-builtins
@@ -78,15 +78,15 @@
     # pyupgrade
     "UP",
     # ruff
     "RUF",
     # tryceratops
     "TRY",
 ]
-ignore = [
+lint.ignore = [
     # LineTooLong
     "E501",
     # DoNotAssignLambda
     "E731",
     # RaiseVanillaArgs aka Avoid specifying long messages outside the exception class
     "TRY003",
 ]
```

### Comparing `phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.3/PKG-INFO` & `phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: phonexia-enhanced-speech-to-text-built-on-whisper-client
-Version: 1.2.3
+Version: 1.2.4
 Summary: Client for communication with Phonexia Enhanced Speech To Text Built On Whisper microservice.
 Keywords: grpc,transcription,STT,ASR,speech to text,speech,language,microservice
 Author: Phonexia
 Author-email: info@phonexia.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: grpcio (>=1.54.0,<2.0.0)
-Requires-Dist: phonexia-grpc (>=1.0.0,<2.0.0)
+Requires-Dist: phonexia-grpc (>=2.0.0,<3.0.0)
 Project-URL: Homepage, https://phonexia.com
 Project-URL: Issues, https://phonexia.atlassian.net/servicedesk/customer/portal/15/group/20/create/40
 Project-URL: protofiles, https://github.com/phonexia/protofiles
 Description-Content-Type: text/markdown
 
 
 ![](https://www.phonexia.com/wp-content/uploads/PHX_logotype_basic_2016_positive_transparent_RGB.png)
```

