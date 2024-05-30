# Comparing `tmp/phonexia_grpc-2.0.0.tar.gz` & `tmp/phonexia_grpc-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phonexia_grpc-2.0.0.tar", max compression
+gzip compressed data, was "phonexia_grpc-2.1.0.tar", max compression
```

## Comparing `phonexia_grpc-2.0.0.tar` & `phonexia_grpc-2.1.0.tar`

### file list

```diff
@@ -1,25 +1,28 @@
--rw-r--r--   0        0        0    11358 2024-04-25 12:34:14.742177 phonexia_grpc-2.0.0/LICENSE
--rw-r--r--   0        0        0     1910 2024-04-25 12:34:48.610693 phonexia_grpc-2.0.0/phonexia/grpc/common/core_pb2.py
--rw-r--r--   0        0        0     5206 2024-04-25 12:34:48.610693 phonexia_grpc-2.0.0/phonexia/grpc/common/core_pb2.pyi
--rw-r--r--   0        0        0     1145 2024-04-25 12:34:48.610693 phonexia_grpc-2.0.0/phonexia/grpc/common/core_pb2_grpc.py
--rw-r--r--   0        0        0     1941 2024-04-25 12:34:48.610693 phonexia_grpc-2.0.0/phonexia/grpc/common/health_check_pb2.py
--rw-r--r--   0        0        0     3337 2024-04-25 12:34:48.610693 phonexia_grpc-2.0.0/phonexia/grpc/common/health_check_pb2.pyi
--rw-r--r--   0        0        0     5803 2024-04-25 12:34:48.610693 phonexia_grpc-2.0.0/phonexia/grpc/common/health_check_pb2_grpc.py
--rw-r--r--   0        0        0     1849 2024-04-25 12:34:48.610693 phonexia_grpc-2.0.0/phonexia/grpc/common/licensing_pb2.py
--rw-r--r--   0        0        0     3031 2024-04-25 12:34:48.610693 phonexia_grpc-2.0.0/phonexia/grpc/common/licensing_pb2.pyi
--rw-r--r--   0        0        0     3841 2024-04-25 12:34:48.610693 phonexia_grpc-2.0.0/phonexia/grpc/common/licensing_pb2_grpc.py
--rw-r--r--   0        0        0     5828 2024-04-25 12:34:48.610693 phonexia_grpc-2.0.0/phonexia/grpc/technologies/enhanced_speech_to_text_built_on_whisper/v1/enhanced_speech_to_text_built_on_whisper_pb2.py
--rw-r--r--   0        0        0    14876 2024-04-25 12:34:48.610693 phonexia_grpc-2.0.0/phonexia/grpc/technologies/enhanced_speech_to_text_built_on_whisper/v1/enhanced_speech_to_text_built_on_whisper_pb2.pyi
--rw-r--r--   0        0        0    10975 2024-04-25 12:34:48.610693 phonexia_grpc-2.0.0/phonexia/grpc/technologies/enhanced_speech_to_text_built_on_whisper/v1/enhanced_speech_to_text_built_on_whisper_pb2_grpc.py
--rw-r--r--   0        0        0     2517 2024-04-25 12:34:48.611693 phonexia_grpc-2.0.0/phonexia/grpc/technologies/gender_identification/v1/gender_identification_pb2.py
--rw-r--r--   0        0        0     4312 2024-04-25 12:34:48.611693 phonexia_grpc-2.0.0/phonexia/grpc/technologies/gender_identification/v1/gender_identification_pb2.pyi
--rw-r--r--   0        0        0     4677 2024-04-25 12:34:48.611693 phonexia_grpc-2.0.0/phonexia/grpc/technologies/gender_identification/v1/gender_identification_pb2_grpc.py
--rw-r--r--   0        0        0     2907 2024-04-25 12:34:48.611693 phonexia_grpc-2.0.0/phonexia/grpc/technologies/speaker_diarization/v1/speaker_diarization_pb2.py
--rw-r--r--   0        0        0     5753 2024-04-25 12:34:48.611693 phonexia_grpc-2.0.0/phonexia/grpc/technologies/speaker_diarization/v1/speaker_diarization_pb2.pyi
--rw-r--r--   0        0        0     4510 2024-04-25 12:34:48.611693 phonexia_grpc-2.0.0/phonexia/grpc/technologies/speaker_diarization/v1/speaker_diarization_pb2_grpc.py
--rw-r--r--   0        0        0     3682 2024-04-25 12:34:48.611693 phonexia_grpc-2.0.0/phonexia/grpc/technologies/speaker_identification/v1/speaker_identification_pb2.py
--rw-r--r--   0        0        0     7603 2024-04-25 12:34:48.611693 phonexia_grpc-2.0.0/phonexia/grpc/technologies/speaker_identification/v1/speaker_identification_pb2.pyi
--rw-r--r--   0        0        0     7976 2024-04-25 12:34:48.611693 phonexia_grpc-2.0.0/phonexia/grpc/technologies/speaker_identification/v1/speaker_identification_pb2_grpc.py
--rw-r--r--   0        0        0     3259 2024-04-25 12:34:14.742177 phonexia_grpc-2.0.0/pypi-README.md
--rw-r--r--   0        0        0     1564 2024-04-25 12:34:49.016699 phonexia_grpc-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     4467 1970-01-01 00:00:00.000000 phonexia_grpc-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-05-30 06:17:37.611386 phonexia_grpc-2.1.0/LICENSE
+-rw-r--r--   0        0        0     1910 2024-05-30 06:17:55.915646 phonexia_grpc-2.1.0/phonexia/grpc/common/core_pb2.py
+-rw-r--r--   0        0        0     5206 2024-05-30 06:17:55.915646 phonexia_grpc-2.1.0/phonexia/grpc/common/core_pb2.pyi
+-rw-r--r--   0        0        0     1142 2024-05-30 06:17:55.915646 phonexia_grpc-2.1.0/phonexia/grpc/common/core_pb2_grpc.py
+-rw-r--r--   0        0        0     1941 2024-05-30 06:17:55.915646 phonexia_grpc-2.1.0/phonexia/grpc/common/health_check_pb2.py
+-rw-r--r--   0        0        0     3337 2024-05-30 06:17:55.915646 phonexia_grpc-2.1.0/phonexia/grpc/common/health_check_pb2.pyi
+-rw-r--r--   0        0        0     5888 2024-05-30 06:17:55.915646 phonexia_grpc-2.1.0/phonexia/grpc/common/health_check_pb2_grpc.py
+-rw-r--r--   0        0        0     1849 2024-05-30 06:17:55.915646 phonexia_grpc-2.1.0/phonexia/grpc/common/licensing_pb2.py
+-rw-r--r--   0        0        0     3031 2024-05-30 06:17:55.915646 phonexia_grpc-2.1.0/phonexia/grpc/common/licensing_pb2.pyi
+-rw-r--r--   0        0        0     3935 2024-05-30 06:17:55.915646 phonexia_grpc-2.1.0/phonexia/grpc/common/licensing_pb2_grpc.py
+-rw-r--r--   0        0        0     5828 2024-05-30 06:17:55.915646 phonexia_grpc-2.1.0/phonexia/grpc/technologies/enhanced_speech_to_text_built_on_whisper/v1/enhanced_speech_to_text_built_on_whisper_pb2.py
+-rw-r--r--   0        0        0    14876 2024-05-30 06:17:55.915646 phonexia_grpc-2.1.0/phonexia/grpc/technologies/enhanced_speech_to_text_built_on_whisper/v1/enhanced_speech_to_text_built_on_whisper_pb2.pyi
+-rw-r--r--   0        0        0    11122 2024-05-30 06:17:55.915646 phonexia_grpc-2.1.0/phonexia/grpc/technologies/enhanced_speech_to_text_built_on_whisper/v1/enhanced_speech_to_text_built_on_whisper_pb2_grpc.py
+-rw-r--r--   0        0        0     2517 2024-05-30 06:17:55.915646 phonexia_grpc-2.1.0/phonexia/grpc/technologies/gender_identification/v1/gender_identification_pb2.py
+-rw-r--r--   0        0        0     4312 2024-05-30 06:17:55.915646 phonexia_grpc-2.1.0/phonexia/grpc/technologies/gender_identification/v1/gender_identification_pb2.pyi
+-rw-r--r--   0        0        0     4813 2024-05-30 06:17:55.915646 phonexia_grpc-2.1.0/phonexia/grpc/technologies/gender_identification/v1/gender_identification_pb2_grpc.py
+-rw-r--r--   0        0        0     4401 2024-05-30 06:17:55.915646 phonexia_grpc-2.1.0/phonexia/grpc/technologies/language_identification/v1/language_identification_pb2.py
+-rw-r--r--   0        0        0    10570 2024-05-30 06:17:55.915646 phonexia_grpc-2.1.0/phonexia/grpc/technologies/language_identification/v1/language_identification_pb2.pyi
+-rw-r--r--   0        0        0     7460 2024-05-30 06:17:55.915646 phonexia_grpc-2.1.0/phonexia/grpc/technologies/language_identification/v1/language_identification_pb2_grpc.py
+-rw-r--r--   0        0        0     2907 2024-05-30 06:17:55.915646 phonexia_grpc-2.1.0/phonexia/grpc/technologies/speaker_diarization/v1/speaker_diarization_pb2.py
+-rw-r--r--   0        0        0     5753 2024-05-30 06:17:55.915646 phonexia_grpc-2.1.0/phonexia/grpc/technologies/speaker_diarization/v1/speaker_diarization_pb2.pyi
+-rw-r--r--   0        0        0     4642 2024-05-30 06:17:55.915646 phonexia_grpc-2.1.0/phonexia/grpc/technologies/speaker_diarization/v1/speaker_diarization_pb2_grpc.py
+-rw-r--r--   0        0        0     3682 2024-05-30 06:17:55.915646 phonexia_grpc-2.1.0/phonexia/grpc/technologies/speaker_identification/v1/speaker_identification_pb2.py
+-rw-r--r--   0        0        0     7603 2024-05-30 06:17:55.915646 phonexia_grpc-2.1.0/phonexia/grpc/technologies/speaker_identification/v1/speaker_identification_pb2.pyi
+-rw-r--r--   0        0        0     8253 2024-05-30 06:17:55.915646 phonexia_grpc-2.1.0/phonexia/grpc/technologies/speaker_identification/v1/speaker_identification_pb2_grpc.py
+-rw-r--r--   0        0        0     3259 2024-05-30 06:17:37.611386 phonexia_grpc-2.1.0/pypi-README.md
+-rw-r--r--   0        0        0     1564 2024-05-30 06:17:56.337652 phonexia_grpc-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4467 1970-01-01 00:00:00.000000 phonexia_grpc-2.1.0/PKG-INFO
```

### Comparing `phonexia_grpc-2.0.0/LICENSE` & `phonexia_grpc-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `phonexia_grpc-2.0.0/phonexia/grpc/common/core_pb2.py` & `phonexia_grpc-2.1.0/phonexia/grpc/common/core_pb2.py`

 * *Files identical despite different names*

### Comparing `phonexia_grpc-2.0.0/phonexia/grpc/common/core_pb2.pyi` & `phonexia_grpc-2.1.0/phonexia/grpc/common/core_pb2.pyi`

 * *Files identical despite different names*

### Comparing `phonexia_grpc-2.0.0/phonexia/grpc/common/core_pb2_grpc.py` & `phonexia_grpc-2.1.0/phonexia/grpc/common/core_pb2_grpc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 import warnings
 
 
-GRPC_GENERATED_VERSION = '1.63.0rc2'
+GRPC_GENERATED_VERSION = '1.64.0'
 GRPC_VERSION = grpc.__version__
 EXPECTED_ERROR_RELEASE = '1.65.0'
 SCHEDULED_RELEASE_DATE = 'June 25, 2024'
 _version_not_supported = False
 
 try:
     from grpc._utilities import first_version_is_lower
```

### Comparing `phonexia_grpc-2.0.0/phonexia/grpc/common/health_check_pb2.py` & `phonexia_grpc-2.1.0/phonexia/grpc/common/health_check_pb2.py`

 * *Files identical despite different names*

### Comparing `phonexia_grpc-2.0.0/phonexia/grpc/common/health_check_pb2.pyi` & `phonexia_grpc-2.1.0/phonexia/grpc/common/health_check_pb2.pyi`

 * *Files identical despite different names*

### Comparing `phonexia_grpc-2.0.0/phonexia/grpc/common/health_check_pb2_grpc.py` & `phonexia_grpc-2.1.0/phonexia/grpc/common/health_check_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 import warnings
 
 from phonexia.grpc.common import health_check_pb2 as phonexia_dot_grpc_dot_common_dot_health__check__pb2
 
-GRPC_GENERATED_VERSION = '1.63.0rc2'
+GRPC_GENERATED_VERSION = '1.64.0'
 GRPC_VERSION = grpc.__version__
 EXPECTED_ERROR_RELEASE = '1.65.0'
 SCHEDULED_RELEASE_DATE = 'June 25, 2024'
 _version_not_supported = False
 
 try:
     from grpc._utilities import first_version_is_lower
@@ -84,14 +84,15 @@
                     request_deserializer=phonexia_dot_grpc_dot_common_dot_health__check__pb2.HealthCheckRequest.FromString,
                     response_serializer=phonexia_dot_grpc_dot_common_dot_health__check__pb2.HealthCheckResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'grpc.health.v1.Health', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
+    server.add_registered_method_handlers('grpc.health.v1.Health', rpc_method_handlers)
 
 
  # This class is part of an EXPERIMENTAL API.
 class Health(object):
     """Service for checking the health of a service.
     """
```

### Comparing `phonexia_grpc-2.0.0/phonexia/grpc/common/licensing_pb2.py` & `phonexia_grpc-2.1.0/phonexia/grpc/common/licensing_pb2.py`

 * *Files identical despite different names*

### Comparing `phonexia_grpc-2.0.0/phonexia/grpc/common/licensing_pb2.pyi` & `phonexia_grpc-2.1.0/phonexia/grpc/common/licensing_pb2.pyi`

 * *Files identical despite different names*

### Comparing `phonexia_grpc-2.0.0/phonexia/grpc/common/licensing_pb2_grpc.py` & `phonexia_grpc-2.1.0/phonexia/grpc/common/licensing_pb2_grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 import warnings
 
 from phonexia.grpc.common import licensing_pb2 as phonexia_dot_grpc_dot_common_dot_licensing__pb2
 
-GRPC_GENERATED_VERSION = '1.63.0rc2'
+GRPC_GENERATED_VERSION = '1.64.0'
 GRPC_VERSION = grpc.__version__
 EXPECTED_ERROR_RELEASE = '1.65.0'
 SCHEDULED_RELEASE_DATE = 'June 25, 2024'
 _version_not_supported = False
 
 try:
     from grpc._utilities import first_version_is_lower
@@ -66,14 +66,15 @@
                     request_deserializer=phonexia_dot_grpc_dot_common_dot_licensing__pb2.LicensingInfoRequest.FromString,
                     response_serializer=phonexia_dot_grpc_dot_common_dot_licensing__pb2.LicensingInfoResult.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'phonexia.grpc.common.Licensing', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
+    server.add_registered_method_handlers('phonexia.grpc.common.Licensing', rpc_method_handlers)
 
 
  # This class is part of an EXPERIMENTAL API.
 class Licensing(object):
     """Service that implements licensing provider.
     """
```

### Comparing `phonexia_grpc-2.0.0/phonexia/grpc/technologies/enhanced_speech_to_text_built_on_whisper/v1/enhanced_speech_to_text_built_on_whisper_pb2.py` & `phonexia_grpc-2.1.0/phonexia/grpc/technologies/enhanced_speech_to_text_built_on_whisper/v1/enhanced_speech_to_text_built_on_whisper_pb2.py`

 * *Files identical despite different names*

### Comparing `phonexia_grpc-2.0.0/phonexia/grpc/technologies/enhanced_speech_to_text_built_on_whisper/v1/enhanced_speech_to_text_built_on_whisper_pb2.pyi` & `phonexia_grpc-2.1.0/phonexia/grpc/technologies/enhanced_speech_to_text_built_on_whisper/v1/enhanced_speech_to_text_built_on_whisper_pb2.pyi`

 * *Files identical despite different names*

### Comparing `phonexia_grpc-2.0.0/phonexia/grpc/technologies/enhanced_speech_to_text_built_on_whisper/v1/enhanced_speech_to_text_built_on_whisper_pb2_grpc.py` & `phonexia_grpc-2.1.0/phonexia/grpc/technologies/enhanced_speech_to_text_built_on_whisper/v1/enhanced_speech_to_text_built_on_whisper_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 import warnings
 
 from phonexia.grpc.technologies.enhanced_speech_to_text_built_on_whisper.v1 import enhanced_speech_to_text_built_on_whisper_pb2 as phonexia_dot_grpc_dot_technologies_dot_enhanced__speech__to__text__built__on__whisper_dot_v1_dot_enhanced__speech__to__text__built__on__whisper__pb2
 
-GRPC_GENERATED_VERSION = '1.63.0rc2'
+GRPC_GENERATED_VERSION = '1.64.0'
 GRPC_VERSION = grpc.__version__
 EXPECTED_ERROR_RELEASE = '1.65.0'
 SCHEDULED_RELEASE_DATE = 'June 25, 2024'
 _version_not_supported = False
 
 try:
     from grpc._utilities import first_version_is_lower
@@ -107,14 +107,15 @@
                     request_deserializer=phonexia_dot_grpc_dot_technologies_dot_enhanced__speech__to__text__built__on__whisper_dot_v1_dot_enhanced__speech__to__text__built__on__whisper__pb2.ListSupportedLanguagesRequest.FromString,
                     response_serializer=phonexia_dot_grpc_dot_technologies_dot_enhanced__speech__to__text__built__on__whisper_dot_v1_dot_enhanced__speech__to__text__built__on__whisper__pb2.ListSupportedLanguagesResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'phonexia.grpc.technologies.enhanced_speech_to_text_built_on_whisper.v1.SpeechToText', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
+    server.add_registered_method_handlers('phonexia.grpc.technologies.enhanced_speech_to_text_built_on_whisper.v1.SpeechToText', rpc_method_handlers)
 
 
  # This class is part of an EXPERIMENTAL API.
 class SpeechToText(object):
     """Service implementing speech-to-text transcription.
     """
```

### Comparing `phonexia_grpc-2.0.0/phonexia/grpc/technologies/gender_identification/v1/gender_identification_pb2.py` & `phonexia_grpc-2.1.0/phonexia/grpc/technologies/gender_identification/v1/gender_identification_pb2.py`

 * *Files identical despite different names*

### Comparing `phonexia_grpc-2.0.0/phonexia/grpc/technologies/gender_identification/v1/gender_identification_pb2.pyi` & `phonexia_grpc-2.1.0/phonexia/grpc/technologies/gender_identification/v1/gender_identification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `phonexia_grpc-2.0.0/phonexia/grpc/technologies/gender_identification/v1/gender_identification_pb2_grpc.py` & `phonexia_grpc-2.1.0/phonexia/grpc/technologies/gender_identification/v1/gender_identification_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 import warnings
 
 from phonexia.grpc.technologies.gender_identification.v1 import gender_identification_pb2 as phonexia_dot_grpc_dot_technologies_dot_gender__identification_dot_v1_dot_gender__identification__pb2
 
-GRPC_GENERATED_VERSION = '1.63.0rc2'
+GRPC_GENERATED_VERSION = '1.64.0'
 GRPC_VERSION = grpc.__version__
 EXPECTED_ERROR_RELEASE = '1.65.0'
 SCHEDULED_RELEASE_DATE = 'June 25, 2024'
 _version_not_supported = False
 
 try:
     from grpc._utilities import first_version_is_lower
@@ -68,14 +68,15 @@
                     request_deserializer=phonexia_dot_grpc_dot_technologies_dot_gender__identification_dot_v1_dot_gender__identification__pb2.IdentifyRequest.FromString,
                     response_serializer=phonexia_dot_grpc_dot_technologies_dot_gender__identification_dot_v1_dot_gender__identification__pb2.IdentifyResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'phonexia.grpc.technologies.gender_identification.v1.GenderIdentification', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
+    server.add_registered_method_handlers('phonexia.grpc.technologies.gender_identification.v1.GenderIdentification', rpc_method_handlers)
 
 
  # This class is part of an EXPERIMENTAL API.
 class GenderIdentification(object):
     """Service that implements gender identification.
     """
```

### Comparing `phonexia_grpc-2.0.0/phonexia/grpc/technologies/speaker_diarization/v1/speaker_diarization_pb2.py` & `phonexia_grpc-2.1.0/phonexia/grpc/technologies/speaker_diarization/v1/speaker_diarization_pb2.py`

 * *Files identical despite different names*

### Comparing `phonexia_grpc-2.0.0/phonexia/grpc/technologies/speaker_diarization/v1/speaker_diarization_pb2.pyi` & `phonexia_grpc-2.1.0/phonexia/grpc/technologies/speaker_diarization/v1/speaker_diarization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `phonexia_grpc-2.0.0/phonexia/grpc/technologies/speaker_diarization/v1/speaker_diarization_pb2_grpc.py` & `phonexia_grpc-2.1.0/phonexia/grpc/technologies/speaker_diarization/v1/speaker_diarization_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 import warnings
 
 from phonexia.grpc.technologies.speaker_diarization.v1 import speaker_diarization_pb2 as phonexia_dot_grpc_dot_technologies_dot_speaker__diarization_dot_v1_dot_speaker__diarization__pb2
 
-GRPC_GENERATED_VERSION = '1.63.0rc2'
+GRPC_GENERATED_VERSION = '1.64.0'
 GRPC_VERSION = grpc.__version__
 EXPECTED_ERROR_RELEASE = '1.65.0'
 SCHEDULED_RELEASE_DATE = 'June 25, 2024'
 _version_not_supported = False
 
 try:
     from grpc._utilities import first_version_is_lower
@@ -67,14 +67,15 @@
                     request_deserializer=phonexia_dot_grpc_dot_technologies_dot_speaker__diarization_dot_v1_dot_speaker__diarization__pb2.DiarizeRequest.FromString,
                     response_serializer=phonexia_dot_grpc_dot_technologies_dot_speaker__diarization_dot_v1_dot_speaker__diarization__pb2.DiarizeResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'phonexia.grpc.technologies.speaker_diarization.v1.SpeakerDiarization', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
+    server.add_registered_method_handlers('phonexia.grpc.technologies.speaker_diarization.v1.SpeakerDiarization', rpc_method_handlers)
 
 
  # This class is part of an EXPERIMENTAL API.
 class SpeakerDiarization(object):
     """Service implementing speaker diarization.
     """
```

### Comparing `phonexia_grpc-2.0.0/phonexia/grpc/technologies/speaker_identification/v1/speaker_identification_pb2.py` & `phonexia_grpc-2.1.0/phonexia/grpc/technologies/speaker_identification/v1/speaker_identification_pb2.py`

 * *Files identical despite different names*

### Comparing `phonexia_grpc-2.0.0/phonexia/grpc/technologies/speaker_identification/v1/speaker_identification_pb2.pyi` & `phonexia_grpc-2.1.0/phonexia/grpc/technologies/speaker_identification/v1/speaker_identification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `phonexia_grpc-2.0.0/phonexia/grpc/technologies/speaker_identification/v1/speaker_identification_pb2_grpc.py` & `phonexia_grpc-2.1.0/phonexia/grpc/technologies/speaker_identification/v1/speaker_identification_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 import warnings
 
 from phonexia.grpc.technologies.speaker_identification.v1 import speaker_identification_pb2 as phonexia_dot_grpc_dot_technologies_dot_speaker__identification_dot_v1_dot_speaker__identification__pb2
 
-GRPC_GENERATED_VERSION = '1.63.0rc2'
+GRPC_GENERATED_VERSION = '1.64.0'
 GRPC_VERSION = grpc.__version__
 EXPECTED_ERROR_RELEASE = '1.65.0'
 SCHEDULED_RELEASE_DATE = 'June 25, 2024'
 _version_not_supported = False
 
 try:
     from grpc._utilities import first_version_is_lower
@@ -69,14 +69,15 @@
                     request_deserializer=phonexia_dot_grpc_dot_technologies_dot_speaker__identification_dot_v1_dot_speaker__identification__pb2.CompareRequest.FromString,
                     response_serializer=phonexia_dot_grpc_dot_technologies_dot_speaker__identification_dot_v1_dot_speaker__identification__pb2.CompareResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'phonexia.grpc.technologies.speaker_identification.v1.VoiceprintComparison', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
+    server.add_registered_method_handlers('phonexia.grpc.technologies.speaker_identification.v1.VoiceprintComparison', rpc_method_handlers)
 
 
  # This class is part of an EXPERIMENTAL API.
 class VoiceprintComparison(object):
     """Service that implements voiceprint comparison.
     """
 
@@ -145,14 +146,15 @@
                     request_deserializer=phonexia_dot_grpc_dot_technologies_dot_speaker__identification_dot_v1_dot_speaker__identification__pb2.ExtractRequest.FromString,
                     response_serializer=phonexia_dot_grpc_dot_technologies_dot_speaker__identification_dot_v1_dot_speaker__identification__pb2.ExtractResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'phonexia.grpc.technologies.speaker_identification.v1.VoiceprintExtraction', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
+    server.add_registered_method_handlers('phonexia.grpc.technologies.speaker_identification.v1.VoiceprintExtraction', rpc_method_handlers)
 
 
  # This class is part of an EXPERIMENTAL API.
 class VoiceprintExtraction(object):
     """Service that implements voiceprint extraction.
     """
```

### Comparing `phonexia_grpc-2.0.0/pypi-README.md` & `phonexia_grpc-2.1.0/pypi-README.md`

 * *Files identical despite different names*

### Comparing `phonexia_grpc-2.0.0/pyproject.toml` & `phonexia_grpc-2.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "phonexia-grpc"
-version = "2.0.0"
+version = "2.1.0"
 description = "Library for communication with microservices developed by phonexia using grpc application interface."
 readme = "pypi-README.md"
 keywords = ["grpc", "voice", "voice-biometry", "speech", "language", "STT", "whisper"]
 authors = ["Phonexia s.r.o. <info@phonexia.com>"]
 license = "Apache-2.0"
 packages = [
     { include = "phonexia" },
```

### Comparing `phonexia_grpc-2.0.0/PKG-INFO` & `phonexia_grpc-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phonexia-grpc
-Version: 2.0.0
+Version: 2.1.0
 Summary: Library for communication with microservices developed by phonexia using grpc application interface.
 License: Apache-2.0
 Keywords: grpc,voice,voice-biometry,speech,language,STT,whisper
 Author: Phonexia s.r.o.
 Author-email: info@phonexia.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

