# Comparing `tmp/hume-0.6.0rc2.tar.gz` & `tmp/hume-0.6.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hume-0.6.0rc2.tar", max compression
+gzip compressed data, was "hume-0.6.0rc3.tar", max compression
```

## Comparing `hume-0.6.0rc2.tar` & `hume-0.6.0rc3.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0     1070 2024-05-24 20:58:49.224091 hume-0.6.0rc2/LICENSE
--rw-r--r--   0        0        0     2256 2024-05-24 20:58:49.224680 hume-0.6.0rc2/README.md
--rw-r--r--   0        0        0      985 2024-05-24 20:58:49.235357 hume-0.6.0rc2/hume/__init__.py
--rw-r--r--   0        0        0       19 2024-05-24 20:58:49.235561 hume-0.6.0rc2/hume/_common/__init__.py
--rw-r--r--   0        0        0     5027 2024-05-29 08:51:51.161632 hume-0.6.0rc2/hume/_common/client_base.py
--rw-r--r--   0        0        0     1804 2024-05-24 20:58:49.236064 hume-0.6.0rc2/hume/_common/config_base.py
--rw-r--r--   0        0        0      121 2024-05-24 20:58:49.236337 hume-0.6.0rc2/hume/_common/protocol.py
--rw-r--r--   0        0        0       19 2024-05-24 20:58:49.236404 hume-0.6.0rc2/hume/_common/utilities/__init__.py
--rw-r--r--   0        0        0     2320 2024-05-24 20:58:49.236629 hume-0.6.0rc2/hume/_common/utilities/config_utilities.py
--rw-r--r--   0        0        0      291 2024-05-24 20:58:49.236911 hume-0.6.0rc2/hume/_common/utilities/model_utilities.py
--rw-r--r--   0        0        0      215 2024-05-24 20:58:49.237167 hume-0.6.0rc2/hume/_common/utilities/paging_utilities.py
--rw-r--r--   0        0        0     3545 2024-05-24 20:58:49.237327 hume-0.6.0rc2/hume/_common/utilities/retry_utilities.py
--rw-r--r--   0        0        0       58 2024-05-24 20:58:49.237899 hume-0.6.0rc2/hume/_common/utilities/typing_utilities.py
--rw-r--r--   0        0        0       19 2024-05-24 20:58:49.237955 hume-0.6.0rc2/hume/_measurement/__init__.py
--rw-r--r--   0        0        0      573 2024-05-24 20:58:49.238192 hume-0.6.0rc2/hume/_measurement/batch/__init__.py
--rw-r--r--   0        0        0     4387 2024-05-24 20:58:49.238389 hume-0.6.0rc2/hume/_measurement/batch/batch_job.py
--rw-r--r--   0        0        0     6046 2024-05-24 20:58:49.238555 hume-0.6.0rc2/hume/_measurement/batch/batch_job_details.py
--rw-r--r--   0        0        0      643 2024-05-24 20:58:49.238742 hume-0.6.0rc2/hume/_measurement/batch/batch_job_state.py
--rw-r--r--   0        0        0      994 2024-05-24 20:58:49.238927 hume-0.6.0rc2/hume/_measurement/batch/batch_job_status.py
--rw-r--r--   0        0        0    10353 2024-05-24 20:58:49.239255 hume-0.6.0rc2/hume/_measurement/batch/hume_batch_client.py
--rw-r--r--   0        0        0      940 2024-05-24 20:58:49.239412 hume-0.6.0rc2/hume/_measurement/batch/transcription_config.py
--rw-r--r--   0        0        0      216 2024-05-24 20:58:49.239675 hume-0.6.0rc2/hume/_measurement/stream/__init__.py
--rw-r--r--   0        0        0     3288 2024-05-24 20:58:49.239962 hume-0.6.0rc2/hume/_measurement/stream/hume_stream_client.py
--rw-r--r--   0        0        0     9411 2024-05-24 20:58:49.240421 hume-0.6.0rc2/hume/_measurement/stream/stream_socket.py
--rw-r--r--   0        0        0      602 2024-05-24 20:58:49.240584 hume-0.6.0rc2/hume/_voice/__init__.py
--rw-r--r--   0        0        0      429 2024-05-24 20:58:49.240941 hume-0.6.0rc2/hume/_voice/hume_voice_client.py
--rw-r--r--   0        0        0       19 2024-05-24 20:58:49.240993 hume-0.6.0rc2/hume/_voice/microphone/__init__.py
--rw-r--r--   0        0        0     1371 2024-05-24 20:58:49.241753 hume-0.6.0rc2/hume/_voice/microphone/asyncio_utilities.py
--rw-r--r--   0        0        0      728 2024-05-24 20:58:49.242003 hume-0.6.0rc2/hume/_voice/microphone/audio_utilities.py
--rw-r--r--   0        0        0     3652 2024-05-29 15:23:35.830242 hume-0.6.0rc2/hume/_voice/microphone/chat_client.py
--rw-r--r--   0        0        0     3350 2024-05-24 20:58:49.242598 hume-0.6.0rc2/hume/_voice/microphone/microphone.py
--rw-r--r--   0        0        0     1667 2024-05-24 20:58:49.243439 hume-0.6.0rc2/hume/_voice/microphone/microphone_interface.py
--rw-r--r--   0        0        0     2925 2024-05-24 20:58:49.243638 hume-0.6.0rc2/hume/_voice/microphone/microphone_sender.py
--rw-r--r--   0        0        0       19 2024-05-24 20:58:49.243842 hume-0.6.0rc2/hume/_voice/mixins/__init__.py
--rw-r--r--   0        0        0     2464 2024-05-29 17:16:05.235959 hume-0.6.0rc2/hume/_voice/mixins/chat_mixin.py
--rw-r--r--   0        0        0     5995 2024-05-29 17:16:05.236292 hume-0.6.0rc2/hume/_voice/mixins/chats_mixin.py
--rw-r--r--   0        0        0     5378 2024-05-29 17:44:25.929373 hume-0.6.0rc2/hume/_voice/mixins/configs_mixin.py
--rw-r--r--   0        0        0     4289 2024-05-24 20:58:49.245040 hume-0.6.0rc2/hume/_voice/mixins/tools_mixin.py
--rw-r--r--   0        0        0       19 2024-05-24 20:58:49.245104 hume-0.6.0rc2/hume/_voice/models/__init__.py
--rw-r--r--   0        0        0     3669 2024-05-29 17:16:05.236615 hume-0.6.0rc2/hume/_voice/models/chats_models.py
--rw-r--r--   0        0        0     2596 2024-05-29 17:44:25.929783 hume-0.6.0rc2/hume/_voice/models/configs_models.py
--rw-r--r--   0        0        0     1140 2024-05-24 20:58:49.245773 hume-0.6.0rc2/hume/_voice/models/tools_models.py
--rw-r--r--   0        0        0      461 2024-05-24 20:58:49.246706 hume-0.6.0rc2/hume/_voice/session_settings.py
--rw-r--r--   0        0        0     3192 2024-05-24 20:58:49.246918 hume-0.6.0rc2/hume/_voice/voice_socket.py
--rw-r--r--   0        0        0       19 2024-05-24 20:58:49.246982 hume-0.6.0rc2/hume/error/__init__.py
--rw-r--r--   0        0        0      571 2024-05-24 20:58:49.247044 hume-0.6.0rc2/hume/error/hume_client_exception.py
--rw-r--r--   0        0        0       97 2024-05-24 20:58:49.247234 hume-0.6.0rc2/hume/models/__init__.py
--rw-r--r--   0        0        0      588 2024-05-24 20:58:49.247521 hume-0.6.0rc2/hume/models/config/__init__.py
--rw-r--r--   0        0        0      498 2024-05-24 20:58:49.247717 hume-0.6.0rc2/hume/models/config/burst_config.py
--rw-r--r--   0        0        0     2574 2024-05-24 20:58:49.247919 hume-0.6.0rc2/hume/models/config/face_config.py
--rw-r--r--   0        0        0      510 2024-05-24 20:58:49.248127 hume-0.6.0rc2/hume/models/config/facemesh_config.py
--rw-r--r--   0        0        0     2236 2024-05-24 20:58:49.248317 hume-0.6.0rc2/hume/models/config/language_config.py
--rw-r--r--   0        0        0      632 2024-05-24 20:58:49.248526 hume-0.6.0rc2/hume/models/config/model_config_base.py
--rw-r--r--   0        0        0     1001 2024-05-24 20:58:49.248760 hume-0.6.0rc2/hume/models/config/ner_config.py
--rw-r--r--   0        0        0     1786 2024-05-24 20:58:49.248946 hume-0.6.0rc2/hume/models/config/prosody_config.py
--rw-r--r--   0        0        0      805 2024-05-24 20:58:49.249139 hume-0.6.0rc2/hume/models/model_type.py
--rw-r--r--   0        0        0     2640 2024-05-29 17:29:31.885741 hume-0.6.0rc2/pyproject.toml
--rw-r--r--   0        0        0     3655 1970-01-01 00:00:00.000000 hume-0.6.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-24 20:58:49.224091 hume-0.6.0rc3/LICENSE
+-rw-r--r--   0        0        0     2256 2024-05-24 20:58:49.224680 hume-0.6.0rc3/README.md
+-rw-r--r--   0        0        0      985 2024-05-24 20:58:49.235357 hume-0.6.0rc3/hume/__init__.py
+-rw-r--r--   0        0        0       19 2024-05-24 20:58:49.235561 hume-0.6.0rc3/hume/_common/__init__.py
+-rw-r--r--   0        0        0     5027 2024-05-29 08:51:51.161632 hume-0.6.0rc3/hume/_common/client_base.py
+-rw-r--r--   0        0        0     1804 2024-05-24 20:58:49.236064 hume-0.6.0rc3/hume/_common/config_base.py
+-rw-r--r--   0        0        0      121 2024-05-24 20:58:49.236337 hume-0.6.0rc3/hume/_common/protocol.py
+-rw-r--r--   0        0        0       19 2024-05-24 20:58:49.236404 hume-0.6.0rc3/hume/_common/utilities/__init__.py
+-rw-r--r--   0        0        0     2320 2024-05-24 20:58:49.236629 hume-0.6.0rc3/hume/_common/utilities/config_utilities.py
+-rw-r--r--   0        0        0      291 2024-05-24 20:58:49.236911 hume-0.6.0rc3/hume/_common/utilities/model_utilities.py
+-rw-r--r--   0        0        0      215 2024-05-24 20:58:49.237167 hume-0.6.0rc3/hume/_common/utilities/paging_utilities.py
+-rw-r--r--   0        0        0     3545 2024-05-24 20:58:49.237327 hume-0.6.0rc3/hume/_common/utilities/retry_utilities.py
+-rw-r--r--   0        0        0       58 2024-05-24 20:58:49.237899 hume-0.6.0rc3/hume/_common/utilities/typing_utilities.py
+-rw-r--r--   0        0        0       19 2024-05-24 20:58:49.237955 hume-0.6.0rc3/hume/_measurement/__init__.py
+-rw-r--r--   0        0        0      573 2024-05-24 20:58:49.238192 hume-0.6.0rc3/hume/_measurement/batch/__init__.py
+-rw-r--r--   0        0        0     4387 2024-05-24 20:58:49.238389 hume-0.6.0rc3/hume/_measurement/batch/batch_job.py
+-rw-r--r--   0        0        0     6046 2024-05-24 20:58:49.238555 hume-0.6.0rc3/hume/_measurement/batch/batch_job_details.py
+-rw-r--r--   0        0        0      643 2024-05-24 20:58:49.238742 hume-0.6.0rc3/hume/_measurement/batch/batch_job_state.py
+-rw-r--r--   0        0        0      994 2024-05-24 20:58:49.238927 hume-0.6.0rc3/hume/_measurement/batch/batch_job_status.py
+-rw-r--r--   0        0        0    10353 2024-05-24 20:58:49.239255 hume-0.6.0rc3/hume/_measurement/batch/hume_batch_client.py
+-rw-r--r--   0        0        0      940 2024-05-24 20:58:49.239412 hume-0.6.0rc3/hume/_measurement/batch/transcription_config.py
+-rw-r--r--   0        0        0      216 2024-05-24 20:58:49.239675 hume-0.6.0rc3/hume/_measurement/stream/__init__.py
+-rw-r--r--   0        0        0     3288 2024-05-24 20:58:49.239962 hume-0.6.0rc3/hume/_measurement/stream/hume_stream_client.py
+-rw-r--r--   0        0        0     9411 2024-05-24 20:58:49.240421 hume-0.6.0rc3/hume/_measurement/stream/stream_socket.py
+-rw-r--r--   0        0        0      602 2024-05-24 20:58:49.240584 hume-0.6.0rc3/hume/_voice/__init__.py
+-rw-r--r--   0        0        0      429 2024-05-24 20:58:49.240941 hume-0.6.0rc3/hume/_voice/hume_voice_client.py
+-rw-r--r--   0        0        0       19 2024-05-24 20:58:49.240993 hume-0.6.0rc3/hume/_voice/microphone/__init__.py
+-rw-r--r--   0        0        0     1371 2024-05-24 20:58:49.241753 hume-0.6.0rc3/hume/_voice/microphone/asyncio_utilities.py
+-rw-r--r--   0        0        0      728 2024-05-24 20:58:49.242003 hume-0.6.0rc3/hume/_voice/microphone/audio_utilities.py
+-rw-r--r--   0        0        0     3652 2024-05-29 15:23:35.830242 hume-0.6.0rc3/hume/_voice/microphone/chat_client.py
+-rw-r--r--   0        0        0     3350 2024-05-24 20:58:49.242598 hume-0.6.0rc3/hume/_voice/microphone/microphone.py
+-rw-r--r--   0        0        0     1667 2024-05-24 20:58:49.243439 hume-0.6.0rc3/hume/_voice/microphone/microphone_interface.py
+-rw-r--r--   0        0        0     2925 2024-05-24 20:58:49.243638 hume-0.6.0rc3/hume/_voice/microphone/microphone_sender.py
+-rw-r--r--   0        0        0       19 2024-05-24 20:58:49.243842 hume-0.6.0rc3/hume/_voice/mixins/__init__.py
+-rw-r--r--   0        0        0     2530 2024-05-30 16:52:11.959190 hume-0.6.0rc3/hume/_voice/mixins/chat_mixin.py
+-rw-r--r--   0        0        0     5995 2024-05-29 17:16:05.236292 hume-0.6.0rc3/hume/_voice/mixins/chats_mixin.py
+-rw-r--r--   0        0        0     5378 2024-05-29 17:44:25.929373 hume-0.6.0rc3/hume/_voice/mixins/configs_mixin.py
+-rw-r--r--   0        0        0     4289 2024-05-24 20:58:49.245040 hume-0.6.0rc3/hume/_voice/mixins/tools_mixin.py
+-rw-r--r--   0        0        0       19 2024-05-24 20:58:49.245104 hume-0.6.0rc3/hume/_voice/models/__init__.py
+-rw-r--r--   0        0        0     3669 2024-05-29 17:16:05.236615 hume-0.6.0rc3/hume/_voice/models/chats_models.py
+-rw-r--r--   0        0        0     2596 2024-05-29 17:44:25.929783 hume-0.6.0rc3/hume/_voice/models/configs_models.py
+-rw-r--r--   0        0        0     1140 2024-05-24 20:58:49.245773 hume-0.6.0rc3/hume/_voice/models/tools_models.py
+-rw-r--r--   0        0        0      461 2024-05-24 20:58:49.246706 hume-0.6.0rc3/hume/_voice/session_settings.py
+-rw-r--r--   0        0        0     3192 2024-05-24 20:58:49.246918 hume-0.6.0rc3/hume/_voice/voice_socket.py
+-rw-r--r--   0        0        0       19 2024-05-24 20:58:49.246982 hume-0.6.0rc3/hume/error/__init__.py
+-rw-r--r--   0        0        0      571 2024-05-24 20:58:49.247044 hume-0.6.0rc3/hume/error/hume_client_exception.py
+-rw-r--r--   0        0        0       97 2024-05-24 20:58:49.247234 hume-0.6.0rc3/hume/models/__init__.py
+-rw-r--r--   0        0        0      588 2024-05-24 20:58:49.247521 hume-0.6.0rc3/hume/models/config/__init__.py
+-rw-r--r--   0        0        0      498 2024-05-24 20:58:49.247717 hume-0.6.0rc3/hume/models/config/burst_config.py
+-rw-r--r--   0        0        0     2574 2024-05-24 20:58:49.247919 hume-0.6.0rc3/hume/models/config/face_config.py
+-rw-r--r--   0        0        0      510 2024-05-24 20:58:49.248127 hume-0.6.0rc3/hume/models/config/facemesh_config.py
+-rw-r--r--   0        0        0     2236 2024-05-24 20:58:49.248317 hume-0.6.0rc3/hume/models/config/language_config.py
+-rw-r--r--   0        0        0      632 2024-05-24 20:58:49.248526 hume-0.6.0rc3/hume/models/config/model_config_base.py
+-rw-r--r--   0        0        0     1001 2024-05-24 20:58:49.248760 hume-0.6.0rc3/hume/models/config/ner_config.py
+-rw-r--r--   0        0        0     1786 2024-05-24 20:58:49.248946 hume-0.6.0rc3/hume/models/config/prosody_config.py
+-rw-r--r--   0        0        0      805 2024-05-24 20:58:49.249139 hume-0.6.0rc3/hume/models/model_type.py
+-rw-r--r--   0        0        0     2640 2024-05-30 17:11:09.591451 hume-0.6.0rc3/pyproject.toml
+-rw-r--r--   0        0        0     3655 1970-01-01 00:00:00.000000 hume-0.6.0rc3/PKG-INFO
```

### Comparing `hume-0.6.0rc2/LICENSE` & `hume-0.6.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `hume-0.6.0rc2/README.md` & `hume-0.6.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `hume-0.6.0rc2/hume/__init__.py` & `hume-0.6.0rc3/hume/__init__.py`

 * *Files identical despite different names*

### Comparing `hume-0.6.0rc2/hume/_common/client_base.py` & `hume-0.6.0rc3/hume/_common/client_base.py`

 * *Files identical despite different names*

### Comparing `hume-0.6.0rc2/hume/_common/config_base.py` & `hume-0.6.0rc3/hume/_common/config_base.py`

 * *Files identical despite different names*

### Comparing `hume-0.6.0rc2/hume/_common/utilities/config_utilities.py` & `hume-0.6.0rc3/hume/_common/utilities/config_utilities.py`

 * *Files identical despite different names*

### Comparing `hume-0.6.0rc2/hume/_common/utilities/retry_utilities.py` & `hume-0.6.0rc3/hume/_common/utilities/retry_utilities.py`

 * *Files identical despite different names*

### Comparing `hume-0.6.0rc2/hume/_measurement/batch/__init__.py` & `hume-0.6.0rc3/hume/_measurement/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `hume-0.6.0rc2/hume/_measurement/batch/batch_job.py` & `hume-0.6.0rc3/hume/_measurement/batch/batch_job.py`

 * *Files identical despite different names*

### Comparing `hume-0.6.0rc2/hume/_measurement/batch/batch_job_details.py` & `hume-0.6.0rc3/hume/_measurement/batch/batch_job_details.py`

 * *Files identical despite different names*

### Comparing `hume-0.6.0rc2/hume/_measurement/batch/batch_job_state.py` & `hume-0.6.0rc3/hume/_measurement/batch/batch_job_state.py`

 * *Files identical despite different names*

### Comparing `hume-0.6.0rc2/hume/_measurement/batch/batch_job_status.py` & `hume-0.6.0rc3/hume/_measurement/batch/batch_job_status.py`

 * *Files identical despite different names*

### Comparing `hume-0.6.0rc2/hume/_measurement/batch/hume_batch_client.py` & `hume-0.6.0rc3/hume/_measurement/batch/hume_batch_client.py`

 * *Files identical despite different names*

### Comparing `hume-0.6.0rc2/hume/_measurement/batch/transcription_config.py` & `hume-0.6.0rc3/hume/_measurement/batch/transcription_config.py`

 * *Files identical despite different names*

### Comparing `hume-0.6.0rc2/hume/_measurement/stream/hume_stream_client.py` & `hume-0.6.0rc3/hume/_measurement/stream/hume_stream_client.py`

 * *Files identical despite different names*

### Comparing `hume-0.6.0rc2/hume/_measurement/stream/stream_socket.py` & `hume-0.6.0rc3/hume/_measurement/stream/stream_socket.py`

 * *Files identical despite different names*

### Comparing `hume-0.6.0rc2/hume/_voice/__init__.py` & `hume-0.6.0rc3/hume/_voice/__init__.py`

 * *Files identical despite different names*

### Comparing `hume-0.6.0rc2/hume/_voice/microphone/asyncio_utilities.py` & `hume-0.6.0rc3/hume/_voice/microphone/asyncio_utilities.py`

 * *Files identical despite different names*

### Comparing `hume-0.6.0rc2/hume/_voice/microphone/audio_utilities.py` & `hume-0.6.0rc3/hume/_voice/microphone/audio_utilities.py`

 * *Files identical despite different names*

### Comparing `hume-0.6.0rc2/hume/_voice/microphone/chat_client.py` & `hume-0.6.0rc3/hume/_voice/microphone/chat_client.py`

 * *Files identical despite different names*

### Comparing `hume-0.6.0rc2/hume/_voice/microphone/microphone.py` & `hume-0.6.0rc3/hume/_voice/microphone/microphone.py`

 * *Files identical despite different names*

### Comparing `hume-0.6.0rc2/hume/_voice/microphone/microphone_interface.py` & `hume-0.6.0rc3/hume/_voice/microphone/microphone_interface.py`

 * *Files identical despite different names*

### Comparing `hume-0.6.0rc2/hume/_voice/microphone/microphone_sender.py` & `hume-0.6.0rc3/hume/_voice/microphone/microphone_sender.py`

 * *Files identical despite different names*

### Comparing `hume-0.6.0rc2/hume/_voice/mixins/chat_mixin.py` & `hume-0.6.0rc3/hume/_voice/mixins/chat_mixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,28 +25,29 @@
         config_id: Optional[str] = None,
         chat_group_id: Optional[str] = None,
     ) -> AsyncIterator[VoiceSocket]:
         """Connect to the EVI API.
 
         Args:
             config_id (Optional[str]): Config ID.
+            chat_group_id (Optional[str]): Chat group ID.
         """
         uri_base = self._build_endpoint("evi", "chat", Protocol.WS)
 
         if config_id is not None and chat_group_id is not None:
             raise HumeClientException(
                 "If resuming from a chat_group_id you must not provide a config_id. "
                 "The original config for the chat group will be used automatically."
             )
 
         params: Dict[str, Any] = {}
         if config_id is not None:
             params["config_id"] = config_id
         if chat_group_id is not None:
-            params["chat_group_id"] = chat_group_id
+            params["resumed_chat_group_id"] = chat_group_id
 
         encoded_params = urllib.parse.urlencode(params)
         uri = f"{uri_base}?{encoded_params}"
 
         logger.info("Connecting to EVI API at %s", uri)
 
         max_size = self.DEFAULT_MAX_PAYLOAD_SIZE_BYTES
```

### Comparing `hume-0.6.0rc2/hume/_voice/mixins/chats_mixin.py` & `hume-0.6.0rc3/hume/_voice/mixins/chats_mixin.py`

 * *Files identical despite different names*

### Comparing `hume-0.6.0rc2/hume/_voice/mixins/configs_mixin.py` & `hume-0.6.0rc3/hume/_voice/mixins/configs_mixin.py`

 * *Files identical despite different names*

### Comparing `hume-0.6.0rc2/hume/_voice/mixins/tools_mixin.py` & `hume-0.6.0rc3/hume/_voice/mixins/tools_mixin.py`

 * *Files identical despite different names*

### Comparing `hume-0.6.0rc2/hume/_voice/models/chats_models.py` & `hume-0.6.0rc3/hume/_voice/models/chats_models.py`

 * *Files identical despite different names*

### Comparing `hume-0.6.0rc2/hume/_voice/models/configs_models.py` & `hume-0.6.0rc3/hume/_voice/models/configs_models.py`

 * *Files identical despite different names*

### Comparing `hume-0.6.0rc2/hume/_voice/models/tools_models.py` & `hume-0.6.0rc3/hume/_voice/models/tools_models.py`

 * *Files identical despite different names*

### Comparing `hume-0.6.0rc2/hume/_voice/voice_socket.py` & `hume-0.6.0rc3/hume/_voice/voice_socket.py`

 * *Files identical despite different names*

### Comparing `hume-0.6.0rc2/hume/error/hume_client_exception.py` & `hume-0.6.0rc3/hume/error/hume_client_exception.py`

 * *Files identical despite different names*

### Comparing `hume-0.6.0rc2/hume/models/config/__init__.py` & `hume-0.6.0rc3/hume/models/config/__init__.py`

 * *Files identical despite different names*

### Comparing `hume-0.6.0rc2/hume/models/config/face_config.py` & `hume-0.6.0rc3/hume/models/config/face_config.py`

 * *Files identical despite different names*

### Comparing `hume-0.6.0rc2/hume/models/config/language_config.py` & `hume-0.6.0rc3/hume/models/config/language_config.py`

 * *Files identical despite different names*

### Comparing `hume-0.6.0rc2/hume/models/config/model_config_base.py` & `hume-0.6.0rc3/hume/models/config/model_config_base.py`

 * *Files identical despite different names*

### Comparing `hume-0.6.0rc2/hume/models/config/ner_config.py` & `hume-0.6.0rc3/hume/models/config/ner_config.py`

 * *Files identical despite different names*

### Comparing `hume-0.6.0rc2/hume/models/config/prosody_config.py` & `hume-0.6.0rc3/hume/models/config/prosody_config.py`

 * *Files identical despite different names*

### Comparing `hume-0.6.0rc2/hume/models/model_type.py` & `hume-0.6.0rc3/hume/models/model_type.py`

 * *Files identical despite different names*

### Comparing `hume-0.6.0rc2/pyproject.toml` & `hume-0.6.0rc3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
   "communication",
   "learning",
 ]
 license = "Proprietary"
 name = "hume"
 readme = "README.md"
 repository = "https://github.com/HumeAI/hume-python-sdk"
-version = "0.6.0rc2"
+version = "0.6.0rc3"
 
 [tool.poetry.dependencies]
 httpx = { extras = ["http2"], version = "^0.27.0" }
 jupyter = { version = "^1.0.0", optional = true }
 pydantic = "^2.6.4"
 pydub = "^0.25.1"
 python = ">=3.9,<4"
```

### Comparing `hume-0.6.0rc2/PKG-INFO` & `hume-0.6.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hume
-Version: 0.6.0rc2
+Version: 0.6.0rc3
 Summary: Hume AI Python SDK
 Home-page: https://github.com/HumeAI/hume-python-sdk
 License: Proprietary
 Keywords: hume,ai,evi,empathic,multimodal,expression,analysis,sentiment,voice,recognition,detection,emotion,interface,speech,audio,vision,expressive,embeddings,communication,learning
 Author: Hume AI Dev
 Author-email: dev@hume.ai
 Requires-Python: >=3.9,<4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hume Version: 0.6.0rc2 Summary: Hume AI Python SDK
+Metadata-Version: 2.1 Name: hume Version: 0.6.0rc3 Summary: Hume AI Python SDK
 Home-page: https://github.com/HumeAI/hume-python-sdk License: Proprietary
 Keywords:
 hume,ai,evi,empathic,multimodal,expression,analysis,sentiment,voice,recognition,detection,emotion,interface,speech,audio,vision,expressive,embeddings,communication,learning
 Author: Hume AI Dev Author-email: dev@hume.ai Requires-Python: >=3.9,<4
 Classifier: Development Status :: 4 - Beta Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

