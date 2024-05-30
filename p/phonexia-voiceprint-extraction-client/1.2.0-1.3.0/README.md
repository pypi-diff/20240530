# Comparing `tmp/phonexia_voiceprint_extraction_client-1.2.0.tar.gz` & `tmp/phonexia_voiceprint_extraction_client-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phonexia_voiceprint_extraction_client-1.2.0.tar", max compression
+gzip compressed data, was "phonexia_voiceprint_extraction_client-1.3.0.tar", max compression
```

## Comparing `phonexia_voiceprint_extraction_client-1.2.0.tar` & `phonexia_voiceprint_extraction_client-1.3.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     4929 2024-02-29 16:19:29.782179 phonexia_voiceprint_extraction_client-1.2.0/phonexia_voiceprint_extraction_client.py
--rw-r--r--   0        0        0      995 2024-02-29 16:19:29.782179 phonexia_voiceprint_extraction_client-1.2.0/pypi-README.md
--rw-r--r--   0        0        0     1966 2024-02-29 16:19:47.049389 phonexia_voiceprint_extraction_client-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1943 1970-01-01 00:00:00.000000 phonexia_voiceprint_extraction_client-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     5317 2024-05-30 11:08:28.887620 phonexia_voiceprint_extraction_client-1.3.0/phonexia_voiceprint_extraction_client.py
+-rw-r--r--   0        0        0      995 2024-05-30 11:08:28.887620 phonexia_voiceprint_extraction_client-1.3.0/pypi-README.md
+-rw-r--r--   0        0        0     1966 2024-05-30 11:08:46.663843 phonexia_voiceprint_extraction_client-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1943 1970-01-01 00:00:00.000000 phonexia_voiceprint_extraction_client-1.3.0/PKG-INFO
```

### Comparing `phonexia_voiceprint_extraction_client-1.2.0/phonexia_voiceprint_extraction_client.py` & `phonexia_voiceprint_extraction_client-1.3.0/phonexia_voiceprint_extraction_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,21 +4,20 @@
 import logging
 import os
 import pathlib
 from typing import Iterator, Optional
 
 import google.protobuf.duration_pb2
 import grpc
-
 import phonexia.grpc.common.core_pb2 as phx_common
 import phonexia.grpc.technologies.speaker_identification.v1.speaker_identification_pb2 as sid
 import phonexia.grpc.technologies.speaker_identification.v1.speaker_identification_pb2_grpc as sid_grpc
 
 
-def time_to_duration(time: float) -> google.protobuf.duration_pb2.Duration | None:
+def time_to_duration(time: float) -> Optional[google.protobuf.duration_pb2.Duration]:
     if time is None:
         return None
     duration = google.protobuf.duration_pb2.Duration()
     duration.seconds = int(time)
     duration.nanos = int((time - duration.seconds) * 1e9)
     return duration
 
@@ -64,18 +63,23 @@
 
 def extract_vp(
     channel: grpc.Channel,
     file: str,
     start: Optional[float],
     end: Optional[float],
     speech_length: Optional[float],
+    metadata: Optional[list],
 ) -> None:
     logging.info(f"Extracting voiceprints from {file}")
     stub = sid_grpc.VoiceprintExtractionStub(channel)
-    write_result(file, stub.Extract(make_request(file, start, end, speech_length)))
+    response = stub.Extract(
+        make_request(file, start, end, speech_length),
+        metadata=metadata,
+    )
+    write_result(file, response)
 
 
 def main():
     parser = argparse.ArgumentParser(
         description=(
             "Voiceprint extraction gRPC client. Extracts voiceprint from an input audio file."
         ),
@@ -90,14 +94,21 @@
     parser.add_argument(
         "-l",
         "--log_level",
         type=str,
         default="error",
         choices=["critical", "error", "warning", "info", "debug"],
     )
+    parser.add_argument(
+        "--metadata",
+        metavar="key=value",
+        nargs="+",
+        type=lambda x: tuple(x.split("=")),
+        help="Custom client metadata",
+    )
     parser.add_argument("--use_ssl", action="store_true", help="Use SSL connection")
     parser.add_argument("--start", type=float, help="Audio start time")
     parser.add_argument("--end", type=float, help="Audio end time")
     parser.add_argument("--speech_length", type=float, help="Maximum amount of speech in seconds")
     parser.add_argument("file", type=str, help="input audio file")
 
     args = parser.parse_args()
@@ -126,18 +137,22 @@
 
     try:
         logging.info(f"Connecting to {args.host}")
         if args.use_ssl:
             with grpc.secure_channel(
                 target=args.host, credentials=grpc.ssl_channel_credentials()
             ) as channel:
-                extract_vp(channel, args.file, args.start, args.end, args.speech_length)
+                extract_vp(
+                    channel, args.file, args.start, args.end, args.speech_length, args.metadata
+                )
         else:
             with grpc.insecure_channel(target=args.host) as channel:
-                extract_vp(channel, args.file, args.start, args.end, args.speech_length)
+                extract_vp(
+                    channel, args.file, args.start, args.end, args.speech_length, args.metadata
+                )
 
     except grpc.RpcError:
         logging.exception("RPC failed")
         exit(1)
     except Exception:
         logging.exception("Unknown error")
         exit(1)
```

### Comparing `phonexia_voiceprint_extraction_client-1.2.0/pypi-README.md` & `phonexia_voiceprint_extraction_client-1.3.0/pypi-README.md`

 * *Files identical despite different names*

### Comparing `phonexia_voiceprint_extraction_client-1.2.0/pyproject.toml` & `phonexia_voiceprint_extraction_client-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "phonexia-voiceprint-extraction-client"
-version = "1.2.0"
+version = "1.3.0"
 description = "Client for communication with Phonexia voiceprint extraction microservice."
 readme = "pypi-README.md"
 keywords = ["grpc", "voice", "voice-biometry", "speech", "language", "identification"]
 authors = ["Phonexia <info@phonexia.com>"]
 
 [tool.poetry.urls]
 Homepage = "https://phonexia.com"
@@ -13,23 +13,23 @@
 
 [tool.poetry.scripts]
 voiceprint_extraction_client = 'phonexia_voiceprint_extraction_client:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 grpcio = "^1.54.0"
-phonexia-grpc = {version="^1.0.0", source="pypi"}
+phonexia-grpc = {version="^2.0.0", source="pypi"}
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.0"
-pytest-cov = "^4.0.0"
+pytest-cov = "^5.0.0"
 pytest-env = "^1.0.0"
 pytest-random-order = "^1.1.0"
 black = "^24.0.0"
-ruff = "^0.2.0"
+ruff = "^0.4.0"
 
 [[tool.poetry.source]]
 name = "gitlab"
 url = "https://gitlab.cloud.phonexia.com/api/v4/groups/39/-/packages/pypi/simple"
 priority = "primary"
```

### Comparing `phonexia_voiceprint_extraction_client-1.2.0/PKG-INFO` & `phonexia_voiceprint_extraction_client-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: phonexia-voiceprint-extraction-client
-Version: 1.2.0
+Version: 1.3.0
 Summary: Client for communication with Phonexia voiceprint extraction microservice.
 Keywords: grpc,voice,voice-biometry,speech,language,identification
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
 
 ![](https://www.phonexia.com/wp-content/uploads/phonexia-logo-transparent-500px.png)
```

