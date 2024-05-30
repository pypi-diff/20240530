# Comparing `tmp/pyannote-onnx-0.0.7.tar.gz` & `tmp/pyannote-onnx-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyannote-onnx-0.0.7.tar", last modified: Wed May 29 13:27:53 2024, max compression
+gzip compressed data, was "pyannote-onnx-0.0.8.tar", last modified: Wed May 29 13:30:32 2024, max compression
```

## Comparing `pyannote-onnx-0.0.7.tar` & `pyannote-onnx-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:27:53.742340 pyannote-onnx-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 13:27:53.000000 pyannote-onnx-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-29 13:27:53.000000 pyannote-onnx-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-29 13:27:53.742340 pyannote-onnx-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-29 13:27:53.000000 pyannote-onnx-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-29 13:27:53.000000 pyannote-onnx-0.0.7/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:27:53.734341 pyannote-onnx-0.0.7/pyannote_onnx/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-29 13:27:53.000000 pyannote-onnx-0.0.7/pyannote_onnx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-29 13:27:53.000000 pyannote-onnx-0.0.7/pyannote_onnx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-29 13:27:53.000000 pyannote-onnx-0.0.7/pyannote_onnx/inference_session.py
--rw-r--r--   0 runner    (1001) docker     (127)    13938 2024-05-29 13:27:53.000000 pyannote-onnx-0.0.7/pyannote_onnx/pyannote_onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)  5983836 2024-05-29 13:27:53.000000 pyannote-onnx-0.0.7/pyannote_onnx/segmentation-3.0.onnx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:27:53.742340 pyannote-onnx-0.0.7/pyannote_onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-29 13:27:53.000000 pyannote-onnx-0.0.7/pyannote_onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-29 13:27:53.000000 pyannote-onnx-0.0.7/pyannote_onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 13:27:53.000000 pyannote-onnx-0.0.7/pyannote_onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-29 13:27:53.000000 pyannote-onnx-0.0.7/pyannote_onnx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-29 13:27:53.000000 pyannote-onnx-0.0.7/pyannote_onnx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-29 13:27:53.000000 pyannote-onnx-0.0.7/pyannote_onnx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-29 13:27:53.000000 pyannote-onnx-0.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 13:27:53.742340 pyannote-onnx-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-29 13:27:53.000000 pyannote-onnx-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:30:32.052609 pyannote-onnx-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 13:30:30.000000 pyannote-onnx-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-29 13:30:30.000000 pyannote-onnx-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-29 13:30:32.052609 pyannote-onnx-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-29 13:30:30.000000 pyannote-onnx-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-29 13:30:30.000000 pyannote-onnx-0.0.8/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:30:32.044609 pyannote-onnx-0.0.8/pyannote_onnx/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-29 13:30:30.000000 pyannote-onnx-0.0.8/pyannote_onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-29 13:30:30.000000 pyannote-onnx-0.0.8/pyannote_onnx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-29 13:30:30.000000 pyannote-onnx-0.0.8/pyannote_onnx/inference_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13948 2024-05-29 13:30:30.000000 pyannote-onnx-0.0.8/pyannote_onnx/pyannote_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)  5983836 2024-05-29 13:30:30.000000 pyannote-onnx-0.0.8/pyannote_onnx/segmentation-3.0.onnx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:30:32.052609 pyannote-onnx-0.0.8/pyannote_onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-29 13:30:32.000000 pyannote-onnx-0.0.8/pyannote_onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-29 13:30:32.000000 pyannote-onnx-0.0.8/pyannote_onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 13:30:32.000000 pyannote-onnx-0.0.8/pyannote_onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-29 13:30:32.000000 pyannote-onnx-0.0.8/pyannote_onnx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-29 13:30:32.000000 pyannote-onnx-0.0.8/pyannote_onnx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-29 13:30:32.000000 pyannote-onnx-0.0.8/pyannote_onnx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-29 13:30:30.000000 pyannote-onnx-0.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 13:30:32.052609 pyannote-onnx-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-29 13:30:30.000000 pyannote-onnx-0.0.8/setup.py
```

### Comparing `pyannote-onnx-0.0.7/LICENSE` & `pyannote-onnx-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyannote-onnx-0.0.7/PKG-INFO` & `pyannote-onnx-0.0.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyannote-onnx
-Version: 0.0.7
+Version: 0.0.8
 Summary: Pyannote ONNX
 Home-page: https://github.com/pengzhendong/pyannote-onnx
 Author: Zhendong Peng
 Author-email: pzd17@tsinghua.org.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyannote-onnx-0.0.7/README.md` & `pyannote-onnx-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pyannote-onnx-0.0.7/pyannote_onnx/__init__.py` & `pyannote-onnx-0.0.8/pyannote_onnx/__init__.py`

 * *Files identical despite different names*

### Comparing `pyannote-onnx-0.0.7/pyannote_onnx/cli.py` & `pyannote-onnx-0.0.8/pyannote_onnx/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
     num_speakers = vad.get_num_speakers(
         wav_path, threshold=0.5, min_speech_duration_ms=100
     )
     print(num_speakers)
 
     if plot:
-        wav, sr = librosa.load(wav_path, sr=vad.sample_rate)
+        wav, sr = librosa.load(wav_path, sr=vad.vad_sr)
         x1 = np.arange(0, len(wav)) / sr
         outputs = [output for output in vad(wav)]
         x2 = [(i * 270 + 721) / sr for i in range(0, len(outputs))]
 
         plt.plot(x1, wav)
         plt.plot(x2, outputs)
         plt.show()
```

### Comparing `pyannote-onnx-0.0.7/pyannote_onnx/inference_session.py` & `pyannote-onnx-0.0.8/pyannote_onnx/inference_session.py`

 * *Files identical despite different names*

### Comparing `pyannote-onnx-0.0.7/pyannote_onnx/pyannote_onnx.py` & `pyannote-onnx-0.0.8/pyannote_onnx/pyannote_onnx.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,16 +145,16 @@
         wav,
         sample_rate,
         save_path,
         flat_layout,
         speech_pad_samples,
         return_seconds,
     ):
-        segment["start"] = max(segment["start"] - speech_pad_samples, 0)
-        segment["end"] = min(segment["end"] + speech_pad_samples, len(wav))
+        segment["start"] = max(int(segment["start"]) - speech_pad_samples, 0)
+        segment["end"] = min(int(segment["end"]) + speech_pad_samples, len(wav))
         if save_path is not None:
             wav = wav[segment["start"] : segment["end"]]
             if flat_layout:
                 sf.write(str(save_path) + f"_{idx:05d}.wav", wav, sample_rate)
             else:
                 sf.write(str(Path(save_path) / f"{idx:05d}.wav"), wav, sample_rate)
         if return_seconds:
```

### Comparing `pyannote-onnx-0.0.7/pyannote_onnx/segmentation-3.0.onnx` & `pyannote-onnx-0.0.8/pyannote_onnx/segmentation-3.0.onnx`

 * *Files identical despite different names*

### Comparing `pyannote-onnx-0.0.7/pyannote_onnx.egg-info/PKG-INFO` & `pyannote-onnx-0.0.8/pyannote_onnx.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyannote-onnx
-Version: 0.0.7
+Version: 0.0.8
 Summary: Pyannote ONNX
 Home-page: https://github.com/pengzhendong/pyannote-onnx
 Author: Zhendong Peng
 Author-email: pzd17@tsinghua.org.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyannote-onnx-0.0.7/setup.py` & `pyannote-onnx-0.0.8/setup.py`

 * *Files identical despite different names*

