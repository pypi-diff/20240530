# Comparing `tmp/ovos-dinkum-listener-0.0.3a8.tar.gz` & `tmp/ovos-dinkum-listener-0.0.3a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-dinkum-listener-0.0.3a8.tar", last modified: Thu Sep 14 17:25:13 2023, max compression
+gzip compressed data, was "ovos-dinkum-listener-0.0.3a9.tar", last modified: Sat Sep 16 20:16:40 2023, max compression
```

## Comparing `ovos-dinkum-listener-0.0.3a8.tar` & `ovos-dinkum-listener-0.0.3a9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 17:25:13.733481 ovos-dinkum-listener-0.0.3a8/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2023-09-14 17:25:09.000000 ovos-dinkum-listener-0.0.3a8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9718 2023-09-14 17:25:13.733481 ovos-dinkum-listener-0.0.3a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9332 2023-09-14 17:25:09.000000 ovos-dinkum-listener-0.0.3a8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 17:25:13.733481 ovos-dinkum-listener-0.0.3a8/ovos_dinkum_listener/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2023-09-14 17:25:09.000000 ovos-dinkum-listener-0.0.3a8/ovos_dinkum_listener/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2023-09-14 17:25:09.000000 ovos-dinkum-listener-0.0.3a8/ovos_dinkum_listener/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2023-09-14 17:25:09.000000 ovos-dinkum-listener-0.0.3a8/ovos_dinkum_listener/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 17:25:13.729481 ovos-dinkum-listener-0.0.3a8/ovos_dinkum_listener/res/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 17:25:13.733481 ovos-dinkum-listener-0.0.3a8/ovos_dinkum_listener/res/snd/
--rw-r--r--   0 runner    (1001) docker     (127)     6268 2023-09-14 17:25:09.000000 ovos-dinkum-listener-0.0.3a8/ovos_dinkum_listener/res/snd/acknowledge.mp3
--rw-r--r--   0 runner    (1001) docker     (127)    13290 2023-09-14 17:25:09.000000 ovos-dinkum-listener-0.0.3a8/ovos_dinkum_listener/res/snd/error.mp3
--rw-r--r--   0 runner    (1001) docker     (127)    67090 2023-09-14 17:25:09.000000 ovos-dinkum-listener-0.0.3a8/ovos_dinkum_listener/res/snd/start_listening.wav
--rw-r--r--   0 runner    (1001) docker     (127)    37572 2023-09-14 17:25:09.000000 ovos-dinkum-listener-0.0.3a8/ovos_dinkum_listener/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2023-09-14 17:25:09.000000 ovos-dinkum-listener-0.0.3a8/ovos_dinkum_listener/transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2023-09-14 17:25:09.000000 ovos-dinkum-listener-0.0.3a8/ovos_dinkum_listener/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 17:25:13.733481 ovos-dinkum-listener-0.0.3a8/ovos_dinkum_listener/voice_loop/
--rw-r--r--   0 runner    (1001) docker     (127)      687 2023-09-14 17:25:09.000000 ovos-dinkum-listener-0.0.3a8/ovos_dinkum_listener/voice_loop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12531 2023-09-14 17:25:09.000000 ovos-dinkum-listener-0.0.3a8/ovos_dinkum_listener/voice_loop/hotwords.py
--rw-r--r--   0 runner    (1001) docker     (127)    27134 2023-09-14 17:25:09.000000 ovos-dinkum-listener-0.0.3a8/ovos_dinkum_listener/voice_loop/voice_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 17:25:13.733481 ovos-dinkum-listener-0.0.3a8/ovos_dinkum_listener.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9718 2023-09-14 17:25:13.000000 ovos-dinkum-listener-0.0.3a8/ovos_dinkum_listener.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      762 2023-09-14 17:25:13.000000 ovos-dinkum-listener-0.0.3a8/ovos_dinkum_listener.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-14 17:25:13.000000 ovos-dinkum-listener-0.0.3a8/ovos_dinkum_listener.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-09-14 17:25:13.000000 ovos-dinkum-listener-0.0.3a8/ovos_dinkum_listener.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2023-09-14 17:25:13.000000 ovos-dinkum-listener-0.0.3a8/ovos_dinkum_listener.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-09-14 17:25:13.000000 ovos-dinkum-listener-0.0.3a8/ovos_dinkum_listener.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-14 17:25:13.733481 ovos-dinkum-listener-0.0.3a8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2023-09-14 17:25:09.000000 ovos-dinkum-listener-0.0.3a8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-16 20:16:40.518104 ovos-dinkum-listener-0.0.3a9/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2023-09-16 20:16:36.000000 ovos-dinkum-listener-0.0.3a9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9848 2023-09-16 20:16:40.518104 ovos-dinkum-listener-0.0.3a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9462 2023-09-16 20:16:36.000000 ovos-dinkum-listener-0.0.3a9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-16 20:16:40.514104 ovos-dinkum-listener-0.0.3a9/ovos_dinkum_listener/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2023-09-16 20:16:36.000000 ovos-dinkum-listener-0.0.3a9/ovos_dinkum_listener/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2023-09-16 20:16:36.000000 ovos-dinkum-listener-0.0.3a9/ovos_dinkum_listener/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2023-09-16 20:16:36.000000 ovos-dinkum-listener-0.0.3a9/ovos_dinkum_listener/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-16 20:16:40.514104 ovos-dinkum-listener-0.0.3a9/ovos_dinkum_listener/res/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-16 20:16:40.518104 ovos-dinkum-listener-0.0.3a9/ovos_dinkum_listener/res/snd/
+-rw-r--r--   0 runner    (1001) docker     (127)     6268 2023-09-16 20:16:36.000000 ovos-dinkum-listener-0.0.3a9/ovos_dinkum_listener/res/snd/acknowledge.mp3
+-rw-r--r--   0 runner    (1001) docker     (127)    13290 2023-09-16 20:16:36.000000 ovos-dinkum-listener-0.0.3a9/ovos_dinkum_listener/res/snd/error.mp3
+-rw-r--r--   0 runner    (1001) docker     (127)    67090 2023-09-16 20:16:36.000000 ovos-dinkum-listener-0.0.3a9/ovos_dinkum_listener/res/snd/start_listening.wav
+-rw-r--r--   0 runner    (1001) docker     (127)    37670 2023-09-16 20:16:36.000000 ovos-dinkum-listener-0.0.3a9/ovos_dinkum_listener/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2023-09-16 20:16:36.000000 ovos-dinkum-listener-0.0.3a9/ovos_dinkum_listener/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2023-09-16 20:16:36.000000 ovos-dinkum-listener-0.0.3a9/ovos_dinkum_listener/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-16 20:16:40.518104 ovos-dinkum-listener-0.0.3a9/ovos_dinkum_listener/voice_loop/
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2023-09-16 20:16:36.000000 ovos-dinkum-listener-0.0.3a9/ovos_dinkum_listener/voice_loop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12531 2023-09-16 20:16:36.000000 ovos-dinkum-listener-0.0.3a9/ovos_dinkum_listener/voice_loop/hotwords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27697 2023-09-16 20:16:36.000000 ovos-dinkum-listener-0.0.3a9/ovos_dinkum_listener/voice_loop/voice_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-16 20:16:40.514104 ovos-dinkum-listener-0.0.3a9/ovos_dinkum_listener.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9848 2023-09-16 20:16:40.000000 ovos-dinkum-listener-0.0.3a9/ovos_dinkum_listener.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2023-09-16 20:16:40.000000 ovos-dinkum-listener-0.0.3a9/ovos_dinkum_listener.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-16 20:16:40.000000 ovos-dinkum-listener-0.0.3a9/ovos_dinkum_listener.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2023-09-16 20:16:40.000000 ovos-dinkum-listener-0.0.3a9/ovos_dinkum_listener.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2023-09-16 20:16:40.000000 ovos-dinkum-listener-0.0.3a9/ovos_dinkum_listener.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2023-09-16 20:16:40.000000 ovos-dinkum-listener-0.0.3a9/ovos_dinkum_listener.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-16 20:16:40.518104 ovos-dinkum-listener-0.0.3a9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2023-09-16 20:16:36.000000 ovos-dinkum-listener-0.0.3a9/setup.py
```

### Comparing `ovos-dinkum-listener-0.0.3a8/PKG-INFO` & `ovos-dinkum-listener-0.0.3a9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-dinkum-listener
-Version: 0.0.3a8
+Version: 0.0.3a9
 Summary: ovos-core listener daemon client
 Home-page: https://github.com/OpenVoiceOS/ovos-dinkum-listener
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
@@ -53,14 +53,16 @@
     "speech_begin": 0.1,
     // Seconds of silence before a voice command has finished
     "silence_end": 0.5,
     // Settings used by microphone to set recording timeout with and without speech detected
     "recording_timeout": 10.0,
     // Settings used by microphone to set recording timeout without speech detected.
     "recording_timeout_with_silence": 3.0,
+    // Setting to remove all silence/noise from start and end of recorded speech (only non-streaming)
+    "remove_silence": true,
     // continuous listen is an experimental setting, it removes the need for
     // wake words and uses VAD only, a streaming STT is strongly recommended
     // NOTE: depending on hardware this may cause mycroft to hear its own TTS responses as questions
     "continuous_listen": false,
 
     // hybrid listen is an experimental setting,
     // it will not require a wake word for X seconds after a user interaction
```

### Comparing `ovos-dinkum-listener-0.0.3a8/README.md` & `ovos-dinkum-listener-0.0.3a9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,16 @@
     "speech_begin": 0.1,
     // Seconds of silence before a voice command has finished
     "silence_end": 0.5,
     // Settings used by microphone to set recording timeout with and without speech detected
     "recording_timeout": 10.0,
     // Settings used by microphone to set recording timeout without speech detected.
     "recording_timeout_with_silence": 3.0,
+    // Setting to remove all silence/noise from start and end of recorded speech (only non-streaming)
+    "remove_silence": true,
     // continuous listen is an experimental setting, it removes the need for
     // wake words and uses VAD only, a streaming STT is strongly recommended
     // NOTE: depending on hardware this may cause mycroft to hear its own TTS responses as questions
     "continuous_listen": false,
 
     // hybrid listen is an experimental setting,
     // it will not require a wake word for X seconds after a user interaction
```

### Comparing `ovos-dinkum-listener-0.0.3a8/ovos_dinkum_listener/__init__.py` & `ovos-dinkum-listener-0.0.3a9/ovos_dinkum_listener/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-dinkum-listener-0.0.3a8/ovos_dinkum_listener/__main__.py` & `ovos-dinkum-listener-0.0.3a9/ovos_dinkum_listener/__main__.py`

 * *Files identical despite different names*

### Comparing `ovos-dinkum-listener-0.0.3a8/ovos_dinkum_listener/plugins.py` & `ovos-dinkum-listener-0.0.3a9/ovos_dinkum_listener/plugins.py`

 * *Files identical despite different names*

### Comparing `ovos-dinkum-listener-0.0.3a8/ovos_dinkum_listener/res/snd/acknowledge.mp3` & `ovos-dinkum-listener-0.0.3a9/ovos_dinkum_listener/res/snd/acknowledge.mp3`

 * *Files identical despite different names*

### Comparing `ovos-dinkum-listener-0.0.3a8/ovos_dinkum_listener/res/snd/error.mp3` & `ovos-dinkum-listener-0.0.3a9/ovos_dinkum_listener/res/snd/error.mp3`

 * *Files identical despite different names*

### Comparing `ovos-dinkum-listener-0.0.3a8/ovos_dinkum_listener/res/snd/start_listening.wav` & `ovos-dinkum-listener-0.0.3a9/ovos_dinkum_listener/res/snd/start_listening.wav`

 * *Files identical despite different names*

### Comparing `ovos-dinkum-listener-0.0.3a8/ovos_dinkum_listener/service.py` & `ovos-dinkum-listener-0.0.3a9/ovos_dinkum_listener/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,14 +209,16 @@
                 silence_seconds=listener_config.get("silence_end", 0.7),
                 timeout_seconds=listener_config.get("recording_timeout", 10),
                 timeout_seconds_with_silence=listener_config.get("recording_timeout_with_silence", 5),                
                 num_stt_rewind_chunks=listener_config.get(
                     "utterance_chunks_to_rewind", 2),
                 num_hotword_keep_chunks=listener_config.get(
                     "wakeword_chunks_to_save", 15),
+                remove_silence=listener_config.get(
+                    "remove_silence", False),
                 #
                 wake_callback=self._record_begin,
                 text_callback=self._stt_text,
                 listenword_audio_callback=self._hotword_audio,
                 hotword_audio_callback=self._hotword_audio,
                 stopword_audio_callback=self._hotword_audio,
                 wakeupword_audio_callback=self._hotword_audio,
```

### Comparing `ovos-dinkum-listener-0.0.3a8/ovos_dinkum_listener/transformers.py` & `ovos-dinkum-listener-0.0.3a9/ovos_dinkum_listener/transformers.py`

 * *Files identical despite different names*

### Comparing `ovos-dinkum-listener-0.0.3a8/ovos_dinkum_listener/voice_loop/__init__.py` & `ovos-dinkum-listener-0.0.3a9/ovos_dinkum_listener/voice_loop/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-dinkum-listener-0.0.3a8/ovos_dinkum_listener/voice_loop/hotwords.py` & `ovos-dinkum-listener-0.0.3a9/ovos_dinkum_listener/voice_loop/hotwords.py`

 * *Files identical despite different names*

### Comparing `ovos-dinkum-listener-0.0.3a8/ovos_dinkum_listener/voice_loop/voice_loop.py` & `ovos-dinkum-listener-0.0.3a9/ovos_dinkum_listener/voice_loop/voice_loop.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 from ovos_plugin_manager.vad import VADEngine
 from ovos_utils.log import LOG
 from ovos_bus_client.session import SessionManager
 from ovos_dinkum_listener.transformers import AudioTransformersService
 from ovos_dinkum_listener.voice_loop.hotwords import HotwordContainer, HotwordState, HotWordException
 from ovos_plugin_manager.templates.microphone import Microphone
 
+from ovos_dinkum_listener.plugins import FakeStreamingSTT
+
 
 class ListeningState(str, Enum):
     DETECT_WAKEWORD = "wakeword"
     WAITING_CMD = "continuous"
 
     RECORDING = "recording"
 
@@ -100,14 +102,15 @@
 class DinkumVoiceLoop(VoiceLoop):
     speech_seconds: float = 0.3
     silence_seconds: float = 0.7
     timeout_seconds: float = 10.0
     timeout_seconds_with_silence: float = 5.0    
     num_stt_rewind_chunks: int = 2
     num_hotword_keep_chunks: int = 15
+    remove_silence: bool = False
     skip_next_wake: bool = False
     hotword_chunks: Deque = field(default_factory=deque)
     stt_chunks: Deque = field(default_factory=deque)
     stt_audio_bytes: bytes = bytes()
     last_ww: float = -1.0
     speech_seconds_left: float = 0.0
     silence_seconds_left: float = 0.0
@@ -646,14 +649,23 @@
         recording and transcript. The loop is reset to the appropriate state for
         the next command.
         @param chunk: bytes of audio captured
         """
         # Command has ended, call transformers pipeline before STT
         chunk, stt_context = self.transformers.transform(chunk)
 
+        if isinstance(self.stt, FakeStreamingSTT) and self.remove_silence:
+            # NOTE: This is using the FS-STT buffer directly, not the S-STT queue
+            self.stt.stream.buffer.clear()
+            extracted_speech = self.vad.extract_speech(self.stt_audio_bytes)
+            # only deposit non empty audio
+            if extracted_speech:
+                LOG.debug("removed silence from utterance")
+                self.stt.stream.update(extracted_speech)
+
         text, stt_context = self._get_tx(stt_context)
 
         if text:
             LOG.debug(f"transformers metadata: {stt_context}")
             LOG.info(f"transcribed: {text}")
         else:
             LOG.info("nothing transcribed")
```

### Comparing `ovos-dinkum-listener-0.0.3a8/ovos_dinkum_listener.egg-info/PKG-INFO` & `ovos-dinkum-listener-0.0.3a9/ovos_dinkum_listener.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-dinkum-listener
-Version: 0.0.3a8
+Version: 0.0.3a9
 Summary: ovos-core listener daemon client
 Home-page: https://github.com/OpenVoiceOS/ovos-dinkum-listener
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
@@ -53,14 +53,16 @@
     "speech_begin": 0.1,
     // Seconds of silence before a voice command has finished
     "silence_end": 0.5,
     // Settings used by microphone to set recording timeout with and without speech detected
     "recording_timeout": 10.0,
     // Settings used by microphone to set recording timeout without speech detected.
     "recording_timeout_with_silence": 3.0,
+    // Setting to remove all silence/noise from start and end of recorded speech (only non-streaming)
+    "remove_silence": true,
     // continuous listen is an experimental setting, it removes the need for
     // wake words and uses VAD only, a streaming STT is strongly recommended
     // NOTE: depending on hardware this may cause mycroft to hear its own TTS responses as questions
     "continuous_listen": false,
 
     // hybrid listen is an experimental setting,
     // it will not require a wake word for X seconds after a user interaction
```

### Comparing `ovos-dinkum-listener-0.0.3a8/ovos_dinkum_listener.egg-info/SOURCES.txt` & `ovos-dinkum-listener-0.0.3a9/ovos_dinkum_listener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-dinkum-listener-0.0.3a8/setup.py` & `ovos-dinkum-listener-0.0.3a9/setup.py`

 * *Files identical despite different names*

