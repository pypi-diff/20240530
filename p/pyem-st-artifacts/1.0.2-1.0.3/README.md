# Comparing `tmp/pyem_st_artifacts-1.0.2.tar.gz` & `tmp/pyem_st_artifacts-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyem_st_artifacts-1.0.2.tar", last modified: Thu Dec 21 10:16:29 2023, max compression
+gzip compressed data, was "pyem_st_artifacts-1.0.3.tar", last modified: Thu May 30 12:23:15 2024, max compression
```

## Comparing `pyem_st_artifacts-1.0.2.tar` & `pyem_st_artifacts-1.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-12-21 10:16:29.000000 pyem_st_artifacts-1.0.2/
--rw-rw-rw-   0        0        0     1090 2023-08-06 07:52:16.000000 pyem_st_artifacts-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     9762 2023-12-21 10:16:29.000000 pyem_st_artifacts-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     9214 2023-12-21 10:00:27.000000 pyem_st_artifacts-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-12-21 10:16:29.000000 pyem_st_artifacts-1.0.2/em_st_artifacts/
--rw-rw-rw-   0        0        0        0 2023-08-06 07:52:16.000000 pyem_st_artifacts-1.0.2/em_st_artifacts/__init__.py
--rw-rw-rw-   0        0        0    24008 2023-12-21 09:46:43.000000 pyem_st_artifacts-1.0.2/em_st_artifacts/emotional_math.py
-drwxrwxrwx   0        0        0        0 2023-12-21 10:16:29.000000 pyem_st_artifacts-1.0.2/em_st_artifacts/libs/
-drwxrwxrwx   0        0        0        0 2023-12-21 10:16:29.000000 pyem_st_artifacts-1.0.2/em_st_artifacts/libs/x64/
--rw-rw-rw-   0        0        0   514560 2023-12-11 09:43:00.000000 pyem_st_artifacts-1.0.2/em_st_artifacts/libs/x64/em_st_artifacts-x64.dll
-drwxrwxrwx   0        0        0        0 2023-12-21 10:16:29.000000 pyem_st_artifacts-1.0.2/em_st_artifacts/libs/x86/
--rw-rw-rw-   0        0        0   426496 2023-12-11 09:43:27.000000 pyem_st_artifacts-1.0.2/em_st_artifacts/libs/x86/em_st_artifacts-x86.dll
--rw-rw-rw-   0        0        0     3577 2023-12-21 09:48:57.000000 pyem_st_artifacts-1.0.2/em_st_artifacts/sample.py
-drwxrwxrwx   0        0        0        0 2023-12-21 10:16:29.000000 pyem_st_artifacts-1.0.2/em_st_artifacts/utils/
--rw-rw-rw-   0        0        0      193 2023-08-06 07:52:16.000000 pyem_st_artifacts-1.0.2/em_st_artifacts/utils/EmotionalMathException.py
--rw-rw-rw-   0        0        0        0 2023-08-06 07:52:16.000000 pyem_st_artifacts-1.0.2/em_st_artifacts/utils/__init__.py
--rw-rw-rw-   0        0        0     1000 2023-12-21 09:46:43.000000 pyem_st_artifacts-1.0.2/em_st_artifacts/utils/lib_settings.py
--rw-rw-rw-   0        0        0      655 2023-08-06 07:52:16.000000 pyem_st_artifacts-1.0.2/em_st_artifacts/utils/support_classes.py
-drwxrwxrwx   0        0        0        0 2023-12-21 10:16:29.000000 pyem_st_artifacts-1.0.2/pyem_st_artifacts.egg-info/
--rw-rw-rw-   0        0        0     9762 2023-12-21 10:16:29.000000 pyem_st_artifacts-1.0.2/pyem_st_artifacts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      537 2023-12-21 10:16:29.000000 pyem_st_artifacts-1.0.2/pyem_st_artifacts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-21 10:16:29.000000 pyem_st_artifacts-1.0.2/pyem_st_artifacts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-12-21 10:16:29.000000 pyem_st_artifacts-1.0.2/pyem_st_artifacts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-12-21 10:16:29.000000 pyem_st_artifacts-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1170 2023-12-21 10:15:58.000000 pyem_st_artifacts-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:23:15.549821 pyem_st_artifacts-1.0.3/
+-rw-rw-rw-   0        0        0     1090 2023-08-06 07:52:16.000000 pyem_st_artifacts-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0    11236 2024-05-30 12:23:15.549821 pyem_st_artifacts-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    10640 2024-05-30 12:20:13.000000 pyem_st_artifacts-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 12:23:15.500002 pyem_st_artifacts-1.0.3/em_st_artifacts/
+-rw-rw-rw-   0        0        0        0 2023-08-06 07:52:16.000000 pyem_st_artifacts-1.0.3/em_st_artifacts/__init__.py
+-rw-rw-rw-   0        0        0    24194 2024-05-30 08:48:27.000000 pyem_st_artifacts-1.0.3/em_st_artifacts/emotional_math.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:23:15.480394 pyem_st_artifacts-1.0.3/em_st_artifacts/libs/
+drwxrwxrwx   0        0        0        0 2024-05-30 12:23:15.500002 pyem_st_artifacts-1.0.3/em_st_artifacts/libs/x64/
+-rw-rw-rw-   0        0        0   514560 2023-12-11 09:43:00.000000 pyem_st_artifacts-1.0.3/em_st_artifacts/libs/x64/em_st_artifacts-x64.dll
+drwxrwxrwx   0        0        0        0 2024-05-30 12:23:15.535265 pyem_st_artifacts-1.0.3/em_st_artifacts/libs/x86/
+-rw-rw-rw-   0        0        0   426496 2023-12-11 09:43:27.000000 pyem_st_artifacts-1.0.3/em_st_artifacts/libs/x86/em_st_artifacts-x86.dll
+-rw-rw-rw-   0        0        0     4237 2024-05-30 12:18:40.000000 pyem_st_artifacts-1.0.3/em_st_artifacts/sample.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:23:15.537274 pyem_st_artifacts-1.0.3/em_st_artifacts/utils/
+-rw-rw-rw-   0        0        0      193 2023-08-06 07:52:16.000000 pyem_st_artifacts-1.0.3/em_st_artifacts/utils/EmotionalMathException.py
+-rw-rw-rw-   0        0        0        0 2023-08-06 07:52:16.000000 pyem_st_artifacts-1.0.3/em_st_artifacts/utils/__init__.py
+-rw-rw-rw-   0        0        0     1000 2023-12-21 09:46:43.000000 pyem_st_artifacts-1.0.3/em_st_artifacts/utils/lib_settings.py
+-rw-rw-rw-   0        0        0      655 2023-08-06 07:52:16.000000 pyem_st_artifacts-1.0.3/em_st_artifacts/utils/support_classes.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:23:15.549821 pyem_st_artifacts-1.0.3/pyem_st_artifacts.egg-info/
+-rw-rw-rw-   0        0        0    11236 2024-05-30 12:23:15.000000 pyem_st_artifacts-1.0.3/pyem_st_artifacts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      537 2024-05-30 12:23:15.000000 pyem_st_artifacts-1.0.3/pyem_st_artifacts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 12:23:15.000000 pyem_st_artifacts-1.0.3/pyem_st_artifacts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-30 12:23:15.000000 pyem_st_artifacts-1.0.3/pyem_st_artifacts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 12:23:15.549821 pyem_st_artifacts-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1217 2024-05-30 08:48:27.000000 pyem_st_artifacts-1.0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyem_st_artifacts-1.0.2/LICENSE` & `pyem_st_artifacts-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyem_st_artifacts-1.0.2/PKG-INFO` & `pyem_st_artifacts-1.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,13 @@
-Metadata-Version: 2.1
-Name: pyem_st_artifacts
-Version: 1.0.2
-Summary: Python wrapper for Emotions library
-Home-page: https://gitlab.com/neurosdk2/neurosamples/-/tree/main/python
-Author: Brainbit Inc.
-Author-email: support@brainbit.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Algorithm of emotional states
 ### Description
 The algorithm processes the data by a sliding window of a given length with a given frequency. If artifacts are detected on one of the bipolar channels, the artifacts on the second bipolar channel are checked, and if there are no artifacts, they are switched to that channel; in case of artifacts on both channels, the spectral values and values of mental levels are filled with previous actual values, while the counter of the number of successive artifact windows increases.
 
 ### Artifacts
-When the maximum number of consecutive artifact windows is reached, `MathLibIsArtifactedSequence()` returns true, which allows you to give the user information about the need to check the position of the device. If there is no need to give notification of momentary artifacts, you can use this function as the primary for artifact notifications. Otherwise, use `MathLibIsBothSidesArtifacted()` to check for momentary artifacts, returning true for artifacts on both bipolar channels for the current window.
+When the maximum number of consecutive artifact windows is reached, `math.is_artifacted_sequence()` returns true, which allows you to give the user information about the need to check the position of the device. This flag is usually raised 4 sec after receiving continuous artifacts. If there is no need to give notification of momentary artifacts, you can use this function as the primary for artifact notifications. Otherwise, use `math.is_both_sides_artifacted()` to check for momentary artifacts, returning true for artifacts on both bipolar channels for the current window.
 
 ### Emotional states
 The estimate of emotional states (mental levels - relaxation and concentration) is available in two variants:
 1. immediate assessment through alpha and beta wave intensity (and theta in the case of independent assessment). 
 2. relative to the baseline calibration values of alpha and beta wave intensity
 
 In both cases, the current intensity of the waves is defined as the average for the last N windows.
@@ -44,15 +28,15 @@
 ### Main parameters description
 Structure `MathLibSettings` with fields:
 1. sampling_rate - raw signal sampling frequency, Hz, integer value
 2. process_win_freq - frequency of spectrum analysis and emotional levels, Hz, integer value
 3. fft_window - spectrum calculation window length, integer value
 4. n_first_sec_skipped - skipping the first seconds after connecting to the device, integer value
 5. bipolar_mode - enabled bipolar mode, boolean value
-6. squared_spectrum
+6. squared_spectrum - mode of calculating spectral values of frequencies. If squared = true then values are calculated as the sum of squares of FFT bins of the spectrum of the interval of the corresponding frequency (e.g. alpha), if squared = false then as the sum of FFT bins. Boolean value
 7. channels_number - count channels for multy-channel library mode, integer value
 8. channel_for_analysis - in case of multichannel mode: channel by default for computing spectral values and emotional levels, integer value
 
 `channels_number` and `channel_for_analysis` are not used explicitly for bipolar mode, you can leave the default ones.
 
 Separate parameters:
 1. MentalEstimationMode - type of evaluation of instant mental levels - disabled by default, boolean value
@@ -80,40 +64,49 @@
 2. n_sec_for_averaging - spectrum averaging, integer value
 
 Separate setting is the number of windows after the artifact with the previous actual value - to smooth the switching process after artifacts (`SkipWinsAfterArtifact`).
 
 ## Initialization
 ### Main parameters
 
-##### Python
 ```python
-mls = MathLibSetting(sampling_rate=250,
-                         process_win_freq=25,
-                         fft_window=1000,
-                         n_first_sec_skipped=4,
-                         bipolar_mode=True,
-                         squared_spectrum=True,
-                         channels_number=4,
-                         channel_for_analysis=0)
-
-ads = ArtifactDetectSetting(hanning_win_spectrum=True, num_wins_for_quality_avg=125)
-
-sads = ShortArtifactDetectSetting(ampl_art_extremum_border=25)
+mls = lib_settings.MathLibSetting(sampling_rate=250,
+                                  process_win_freq=25,
+                                  n_first_sec_skipped=4,
+                                  fft_window=1000,
+                                  bipolar_mode=True,
+                                  squared_spectrum=True,
+                                  channels_number=4,
+                                  channel_for_analysis=0)
+
+ads = lib_settings.ArtifactDetectSetting(art_bord=110,
+                                         allowed_percent_artpoints=70,
+                                         raw_betap_limit=800_000,
+                                         global_artwin_sec=4,
+                                         num_wins_for_quality_avg=125,
+                                         hamming_win_spectrum=True,
+                                         hanning_win_spectrum=False,
+                                         total_pow_border=400_000_000,
+                                         spect_art_by_totalp=True)
+
+sads = lib_settings.ShortArtifactDetectSetting(ampl_art_detect_win_size=200,
+                                               ampl_art_zerod_area=200,
+                                               ampl_art_extremum_border=25)
 
-mss = MentalAndSpectralSetting()
+mss = lib_settings.MentalAndSpectralSetting(n_sec_for_averaging=2,
+                                            n_sec_for_instant_estimation=4)
 
-emotions = EmotionalMath(mls, ads, sads, mss)
+math = EmotionalMath(mls, ads, sads, mss)
 ```
 
 ### Optional parameters
 
-##### Python
 ```python
 # setting calibration length
-calibration_length = 8
+calibration_length = 6
 math.set_calibration_length(calibration_length)
 
 # type of evaluation of instant mental levels
 independent_mental_levels = False
 math.set_mental_estimation_mode(independent_mental_levels)
 
 # number of windows after the artifact with the previous actual value
@@ -157,68 +150,68 @@
 1. LEFT
 2. RIGHT
 3. NONE
 
 ## Usage
 1. If you need calibration start calibration right after library init:
 
-##### Python
 ```python
 math.start_calibration()
 ``` 
 
 2. Adding and process data
 In bipolar mode:
 
-##### Python
 ```python
-samples = []
-math.push_data(samples)
-math.process_data_arr()
+def on_brain_bit_signal_data_received(sensor, data):
+    raw_channels = []
+    for sample in data:
+        left_bipolar = sample.T3-sample.O1
+        right_bipolar = sample.T4-sample.O2
+        raw_channels.append(support_classes.RawChannels(left_bipolar, right_bipolar))
+    
+    math.push_data(raw_channels)
+    math.process_data_arr()
+...
+sensor.signalDataReceived = on_brain_bit_signal_data_received
 ``` 
 
 In multy-channel mode:
 
-##### Python
 ```python
 samples = []
 math.push_data_arr(samples)
 math.process_data_arr()
 ``` 
 2. Then check calibration status if you need to calibrate values:
 
-##### Python
 ```python
 calibration_finished = math.calibration_finished()
 # and calibration progress
 calibration_progress = math.get_calibration_percents()
 ``` 
 3. If calibration finished (or you don't need to calibrate) read output values:
 
-##### Python
 ```python
 # Reading mental levels in percent
 mental_data = math.read_mental_data_arr()
 # Reading relative spectral values in percent
 sp_data = math.read_spectral_data_percents_arr()
 ``` 
 4. Check artifacts
 4.1. During calibration
 
-##### Python
 ```python
 if math.is_both_sides_artifacted():
     # signal corruption
 ``` 
 4.2. After (without) calibration
 
-##### Python
 ```python
 if math.is_artifacted_sequence():
     # signal corruption
 ``` 
 ## Finishing work with the library
 
-##### Python
 ```python
 del math
-``` 
+```
```

### Comparing `pyem_st_artifacts-1.0.2/README.md` & `pyem_st_artifacts-1.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,30 @@
+Metadata-Version: 2.1
+Name: pyem_st_artifacts
+Version: 1.0.3
+Summary: Python wrapper for Emotions library
+Home-page: https://gitlab.com/neurosdk2/neurosamples/-/tree/main/python
+Author: Brainbit Inc.
+Author-email: support@brainbit.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Intended Audience :: Developers
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Algorithm of emotional states
 ### Description
 The algorithm processes the data by a sliding window of a given length with a given frequency. If artifacts are detected on one of the bipolar channels, the artifacts on the second bipolar channel are checked, and if there are no artifacts, they are switched to that channel; in case of artifacts on both channels, the spectral values and values of mental levels are filled with previous actual values, while the counter of the number of successive artifact windows increases.
 
 ### Artifacts
-When the maximum number of consecutive artifact windows is reached, `MathLibIsArtifactedSequence()` returns true, which allows you to give the user information about the need to check the position of the device. If there is no need to give notification of momentary artifacts, you can use this function as the primary for artifact notifications. Otherwise, use `MathLibIsBothSidesArtifacted()` to check for momentary artifacts, returning true for artifacts on both bipolar channels for the current window.
+When the maximum number of consecutive artifact windows is reached, `math.is_artifacted_sequence()` returns true, which allows you to give the user information about the need to check the position of the device. This flag is usually raised 4 sec after receiving continuous artifacts. If there is no need to give notification of momentary artifacts, you can use this function as the primary for artifact notifications. Otherwise, use `math.is_both_sides_artifacted()` to check for momentary artifacts, returning true for artifacts on both bipolar channels for the current window.
 
 ### Emotional states
 The estimate of emotional states (mental levels - relaxation and concentration) is available in two variants:
 1. immediate assessment through alpha and beta wave intensity (and theta in the case of independent assessment). 
 2. relative to the baseline calibration values of alpha and beta wave intensity
 
 In both cases, the current intensity of the waves is defined as the average for the last N windows.
@@ -28,15 +45,15 @@
 ### Main parameters description
 Structure `MathLibSettings` with fields:
 1. sampling_rate - raw signal sampling frequency, Hz, integer value
 2. process_win_freq - frequency of spectrum analysis and emotional levels, Hz, integer value
 3. fft_window - spectrum calculation window length, integer value
 4. n_first_sec_skipped - skipping the first seconds after connecting to the device, integer value
 5. bipolar_mode - enabled bipolar mode, boolean value
-6. squared_spectrum
+6. squared_spectrum - mode of calculating spectral values of frequencies. If squared = true then values are calculated as the sum of squares of FFT bins of the spectrum of the interval of the corresponding frequency (e.g. alpha), if squared = false then as the sum of FFT bins. Boolean value
 7. channels_number - count channels for multy-channel library mode, integer value
 8. channel_for_analysis - in case of multichannel mode: channel by default for computing spectral values and emotional levels, integer value
 
 `channels_number` and `channel_for_analysis` are not used explicitly for bipolar mode, you can leave the default ones.
 
 Separate parameters:
 1. MentalEstimationMode - type of evaluation of instant mental levels - disabled by default, boolean value
@@ -64,40 +81,49 @@
 2. n_sec_for_averaging - spectrum averaging, integer value
 
 Separate setting is the number of windows after the artifact with the previous actual value - to smooth the switching process after artifacts (`SkipWinsAfterArtifact`).
 
 ## Initialization
 ### Main parameters
 
-##### Python
 ```python
-mls = MathLibSetting(sampling_rate=250,
-                         process_win_freq=25,
-                         fft_window=1000,
-                         n_first_sec_skipped=4,
-                         bipolar_mode=True,
-                         squared_spectrum=True,
-                         channels_number=4,
-                         channel_for_analysis=0)
-
-ads = ArtifactDetectSetting(hanning_win_spectrum=True, num_wins_for_quality_avg=125)
-
-sads = ShortArtifactDetectSetting(ampl_art_extremum_border=25)
+mls = lib_settings.MathLibSetting(sampling_rate=250,
+                                  process_win_freq=25,
+                                  n_first_sec_skipped=4,
+                                  fft_window=1000,
+                                  bipolar_mode=True,
+                                  squared_spectrum=True,
+                                  channels_number=4,
+                                  channel_for_analysis=0)
+
+ads = lib_settings.ArtifactDetectSetting(art_bord=110,
+                                         allowed_percent_artpoints=70,
+                                         raw_betap_limit=800_000,
+                                         global_artwin_sec=4,
+                                         num_wins_for_quality_avg=125,
+                                         hamming_win_spectrum=True,
+                                         hanning_win_spectrum=False,
+                                         total_pow_border=400_000_000,
+                                         spect_art_by_totalp=True)
+
+sads = lib_settings.ShortArtifactDetectSetting(ampl_art_detect_win_size=200,
+                                               ampl_art_zerod_area=200,
+                                               ampl_art_extremum_border=25)
 
-mss = MentalAndSpectralSetting()
+mss = lib_settings.MentalAndSpectralSetting(n_sec_for_averaging=2,
+                                            n_sec_for_instant_estimation=4)
 
-emotions = EmotionalMath(mls, ads, sads, mss)
+math = EmotionalMath(mls, ads, sads, mss)
 ```
 
 ### Optional parameters
 
-##### Python
 ```python
 # setting calibration length
-calibration_length = 8
+calibration_length = 6
 math.set_calibration_length(calibration_length)
 
 # type of evaluation of instant mental levels
 independent_mental_levels = False
 math.set_mental_estimation_mode(independent_mental_levels)
 
 # number of windows after the artifact with the previous actual value
@@ -141,68 +167,68 @@
 1. LEFT
 2. RIGHT
 3. NONE
 
 ## Usage
 1. If you need calibration start calibration right after library init:
 
-##### Python
 ```python
 math.start_calibration()
 ``` 
 
 2. Adding and process data
 In bipolar mode:
 
-##### Python
 ```python
-samples = []
-math.push_data(samples)
-math.process_data_arr()
+def on_brain_bit_signal_data_received(sensor, data):
+    raw_channels = []
+    for sample in data:
+        left_bipolar = sample.T3-sample.O1
+        right_bipolar = sample.T4-sample.O2
+        raw_channels.append(support_classes.RawChannels(left_bipolar, right_bipolar))
+    
+    math.push_data(raw_channels)
+    math.process_data_arr()
+...
+sensor.signalDataReceived = on_brain_bit_signal_data_received
 ``` 
 
 In multy-channel mode:
 
-##### Python
 ```python
 samples = []
 math.push_data_arr(samples)
 math.process_data_arr()
 ``` 
 2. Then check calibration status if you need to calibrate values:
 
-##### Python
 ```python
 calibration_finished = math.calibration_finished()
 # and calibration progress
 calibration_progress = math.get_calibration_percents()
 ``` 
 3. If calibration finished (or you don't need to calibrate) read output values:
 
-##### Python
 ```python
 # Reading mental levels in percent
 mental_data = math.read_mental_data_arr()
 # Reading relative spectral values in percent
 sp_data = math.read_spectral_data_percents_arr()
 ``` 
 4. Check artifacts
 4.1. During calibration
 
-##### Python
 ```python
 if math.is_both_sides_artifacted():
     # signal corruption
 ``` 
 4.2. After (without) calibration
 
-##### Python
 ```python
 if math.is_artifacted_sequence():
     # signal corruption
 ``` 
 ## Finishing work with the library
 
-##### Python
 ```python
 del math
-``` 
+```
```

### Comparing `pyem_st_artifacts-1.0.2/em_st_artifacts/emotional_math.py` & `pyem_st_artifacts-1.0.3/em_st_artifacts/emotional_math.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,32 +3,33 @@
 import platform
 import sys
 
 from typing import List
 
 from em_st_artifacts.utils.EmotionalMathException import EmotionalMathException
 from em_st_artifacts.utils.lib_settings import (ArtifactDetectSetting, MathLibSetting, MentalAndSpectralSetting,
-                               ShortArtifactDetectSetting, )
-from em_st_artifacts.utils.support_classes import MindData, RawChannels, RawChannelsArray, RawSpectVals, SpectralDataPercents
+                                                ShortArtifactDetectSetting, )
+from em_st_artifacts.utils.support_classes import MindData, RawChannels, RawChannelsArray, RawSpectVals, \
+    SpectralDataPercents
 
 _main_lib_name = None
 if sys.platform == "win32":
     arc = platform.architecture()
     if arc[0].__contains__("64"):
         _main_lib_name = pathlib.Path(__file__).parent.resolve() / "libs" / "x64" / "em_st_artifacts-x64.dll"
     else:
         _main_lib_name = pathlib.Path(__file__).parent.resolve() / "libs" / "x86" / "em_st_artifacts-x86.dll"
 elif sys.platform.startswith("linux"):
-    print('Add linux lib')
+    _main_lib_name = "libem_st_artifacts.so"
 elif sys.platform == "darwin":
     print('Add macos lib')
 else:
     raise FileNotFoundError("This platform (%s) is currently not supported by pyem-st-artifactslib." % sys.platform)
 
-_em_st_artifacts_lib = ctypes.WinDLL(str(_main_lib_name))
+_em_st_artifacts_lib = ctypes.CDLL(str(_main_lib_name))
 
 
 class EmotionalMath:
     class _NativeMathLibSetting(ctypes.Structure):
         _fields_ = [('sampling_rate', ctypes.c_int32), ('process_win_freq', ctypes.c_int32),
                     ('fft_window', ctypes.c_int32), ('n_first_sec_skipped', ctypes.c_int32),
                     ('bipolar_mode', ctypes.c_uint8), ('squared_spectrum', ctypes.c_uint8),
@@ -268,15 +269,17 @@
         self._set_skip_wins_after_artifact(self._native_ptr, nwins, ctypes.byref(op_status))
         self._check_error(op_status)
 
     def push_data(self, samples: List[RawChannels]):
         op_status = self._NativeOpStatus()
         raw_ch_len = len(samples)
         self._push_data(self._native_ptr,
-                        (self._NativeRawChannels * raw_ch_len)(*[self._NativeRawChannels(samples[i].left_bipolar, samples[i].right_bipolar) for i in range(raw_ch_len)]),
+                        (self._NativeRawChannels * raw_ch_len)(
+                            *[self._NativeRawChannels(samples[i].left_bipolar, samples[i].right_bipolar) for i in
+                              range(raw_ch_len)]),
                         raw_ch_len,
                         ctypes.byref(op_status))
         self._check_error(op_status)
 
     def push_data_arr(self, samples: List[RawChannelsArray]):
         native_list = []
 
@@ -366,15 +369,16 @@
 
         if arr_size == 0:
             return []
 
         native_result = (self._NativeMindData * arr_size)()
         native_arr_size = ctypes.c_int(arr_size)
         op_status = self._NativeOpStatus()
-        self._read_mental_data_arr(self._native_ptr, native_result, ctypes.byref(native_arr_size), ctypes.byref(op_status))
+        self._read_mental_data_arr(self._native_ptr, native_result, ctypes.byref(native_arr_size),
+                                   ctypes.byref(op_status))
         self._check_error(op_status)
 
         return [MindData(x.Rel_Attention, x.Rel_Relaxation, x.Inst_Attention, x.Inst_Relaxation) for x in native_result]
 
     def read_average_mental_data(self, n_last_wins_to_average: int) -> MindData:
         native_result = self._NativeMindData()
 
@@ -404,15 +408,16 @@
 
         if arr_size == 0:
             return []
 
         native_result = (self._NativeSpectralDataPercents * arr_size)()
         native_arr_size = ctypes.c_int(arr_size)
         op_status = self._NativeOpStatus()
-        self._read_spectral_data_percents_arr(self._native_ptr, native_result, ctypes.byref(native_arr_size), ctypes.byref(op_status))
+        self._read_spectral_data_percents_arr(self._native_ptr, native_result, ctypes.byref(native_arr_size),
+                                              ctypes.byref(op_status))
         self._check_error(op_status)
 
         return [SpectralDataPercents(x.Delta, x.Theta, x.Alpha, x.Beta, x.Gamma) for x in native_result]
 
     def read_raw_spectral_vals(self) -> RawSpectVals:
         native_result = self._NativeRawSpectVals()
 
@@ -456,15 +461,15 @@
         self._check_error(op_status)
 
         return result.value
 
     @staticmethod
     def _check_error(op_status: _NativeOpStatus):
         if not op_status.Success:
-            error_msg = op_status.ErrorMsg#"".join([op_status.ErrorMsg[x] for x in range(512)])
+            error_msg = op_status.ErrorMsg  #"".join([op_status.ErrorMsg[x] for x in range(512)])
             raise EmotionalMathException(error_msg)
 
     def __del__(self):
         if self._native_ptr is None:
             op_status = self._NativeOpStatus()
 
             self._free_math_lib(self._native_ptr, ctypes.byref(op_status))
```

### Comparing `pyem_st_artifacts-1.0.2/em_st_artifacts/libs/x64/em_st_artifacts-x64.dll` & `pyem_st_artifacts-1.0.3/em_st_artifacts/libs/x64/em_st_artifacts-x64.dll`

 * *Files identical despite different names*

### Comparing `pyem_st_artifacts-1.0.2/em_st_artifacts/libs/x86/em_st_artifacts-x86.dll` & `pyem_st_artifacts-1.0.3/em_st_artifacts/libs/x86/em_st_artifacts-x86.dll`

 * *Files identical despite different names*

### Comparing `pyem_st_artifacts-1.0.2/em_st_artifacts/sample.py` & `pyem_st_artifacts-1.0.3/em_st_artifacts/sample.py`

 * *Files 20% similar despite different names*

```diff
@@ -28,26 +28,37 @@
 
 def main():
     calibration_length = 8
     nwins_skip_after_artifact = 10
 
     mls = MathLibSetting(sampling_rate=250,
                          process_win_freq=25,
-                         fft_window=1000,
                          n_first_sec_skipped=4,
+                         fft_window=1000,
                          bipolar_mode=True,
                          squared_spectrum=True,
                          channels_number=4,
                          channel_for_analysis=0)
 
-    ads = ArtifactDetectSetting(hanning_win_spectrum=True, num_wins_for_quality_avg=125)
-
-    sads = ShortArtifactDetectSetting(ampl_art_extremum_border=25)
+    ads = ArtifactDetectSetting(art_bord=110,
+                                allowed_percent_artpoints=70,
+                                raw_betap_limit=800_000,
+                                global_artwin_sec=4,
+                                num_wins_for_quality_avg=125,
+                                hamming_win_spectrum=True,
+                                hanning_win_spectrum=False,
+                                total_pow_border=400_000_000,
+                                spect_art_by_totalp=True)
+
+    sads = ShortArtifactDetectSetting(ampl_art_detect_win_size=200,
+                                      ampl_art_zerod_area=200,
+                                      ampl_art_extremum_border=25)
 
-    mss = MentalAndSpectralSetting()
+    mss = MentalAndSpectralSetting(n_sec_for_averaging=2,
+                                   n_sec_for_instant_estimation=4)
 
     emotions = EmotionalMath(mls, ads, sads, mss)
     emotions.set_calibration_length(calibration_length)
     emotions.set_mental_estimation_mode(False)
     emotions.set_skip_wins_after_artifact(nwins_skip_after_artifact)
     emotions.set_zero_spect_waves(True, 0, 1, 1, 1, 0)
     emotions.set_spect_normalization_by_bands_width(True)
```

### Comparing `pyem_st_artifacts-1.0.2/em_st_artifacts/utils/lib_settings.py` & `pyem_st_artifacts-1.0.3/em_st_artifacts/utils/lib_settings.py`

 * *Files identical despite different names*

### Comparing `pyem_st_artifacts-1.0.2/em_st_artifacts/utils/support_classes.py` & `pyem_st_artifacts-1.0.3/em_st_artifacts/utils/support_classes.py`

 * *Files identical despite different names*

### Comparing `pyem_st_artifacts-1.0.2/pyem_st_artifacts.egg-info/PKG-INFO` & `pyem_st_artifacts-1.0.3/pyem_st_artifacts.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: pyem-st-artifacts
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python wrapper for Emotions library
 Home-page: https://gitlab.com/neurosdk2/neurosamples/-/tree/main/python
 Author: Brainbit Inc.
 Author-email: support@brainbit.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Algorithm of emotional states
 ### Description
 The algorithm processes the data by a sliding window of a given length with a given frequency. If artifacts are detected on one of the bipolar channels, the artifacts on the second bipolar channel are checked, and if there are no artifacts, they are switched to that channel; in case of artifacts on both channels, the spectral values and values of mental levels are filled with previous actual values, while the counter of the number of successive artifact windows increases.
 
 ### Artifacts
-When the maximum number of consecutive artifact windows is reached, `MathLibIsArtifactedSequence()` returns true, which allows you to give the user information about the need to check the position of the device. If there is no need to give notification of momentary artifacts, you can use this function as the primary for artifact notifications. Otherwise, use `MathLibIsBothSidesArtifacted()` to check for momentary artifacts, returning true for artifacts on both bipolar channels for the current window.
+When the maximum number of consecutive artifact windows is reached, `math.is_artifacted_sequence()` returns true, which allows you to give the user information about the need to check the position of the device. This flag is usually raised 4 sec after receiving continuous artifacts. If there is no need to give notification of momentary artifacts, you can use this function as the primary for artifact notifications. Otherwise, use `math.is_both_sides_artifacted()` to check for momentary artifacts, returning true for artifacts on both bipolar channels for the current window.
 
 ### Emotional states
 The estimate of emotional states (mental levels - relaxation and concentration) is available in two variants:
 1. immediate assessment through alpha and beta wave intensity (and theta in the case of independent assessment). 
 2. relative to the baseline calibration values of alpha and beta wave intensity
 
 In both cases, the current intensity of the waves is defined as the average for the last N windows.
@@ -44,15 +45,15 @@
 ### Main parameters description
 Structure `MathLibSettings` with fields:
 1. sampling_rate - raw signal sampling frequency, Hz, integer value
 2. process_win_freq - frequency of spectrum analysis and emotional levels, Hz, integer value
 3. fft_window - spectrum calculation window length, integer value
 4. n_first_sec_skipped - skipping the first seconds after connecting to the device, integer value
 5. bipolar_mode - enabled bipolar mode, boolean value
-6. squared_spectrum
+6. squared_spectrum - mode of calculating spectral values of frequencies. If squared = true then values are calculated as the sum of squares of FFT bins of the spectrum of the interval of the corresponding frequency (e.g. alpha), if squared = false then as the sum of FFT bins. Boolean value
 7. channels_number - count channels for multy-channel library mode, integer value
 8. channel_for_analysis - in case of multichannel mode: channel by default for computing spectral values and emotional levels, integer value
 
 `channels_number` and `channel_for_analysis` are not used explicitly for bipolar mode, you can leave the default ones.
 
 Separate parameters:
 1. MentalEstimationMode - type of evaluation of instant mental levels - disabled by default, boolean value
@@ -80,40 +81,49 @@
 2. n_sec_for_averaging - spectrum averaging, integer value
 
 Separate setting is the number of windows after the artifact with the previous actual value - to smooth the switching process after artifacts (`SkipWinsAfterArtifact`).
 
 ## Initialization
 ### Main parameters
 
-##### Python
 ```python
-mls = MathLibSetting(sampling_rate=250,
-                         process_win_freq=25,
-                         fft_window=1000,
-                         n_first_sec_skipped=4,
-                         bipolar_mode=True,
-                         squared_spectrum=True,
-                         channels_number=4,
-                         channel_for_analysis=0)
+mls = lib_settings.MathLibSetting(sampling_rate=250,
+                                  process_win_freq=25,
+                                  n_first_sec_skipped=4,
+                                  fft_window=1000,
+                                  bipolar_mode=True,
+                                  squared_spectrum=True,
+                                  channels_number=4,
+                                  channel_for_analysis=0)
+
+ads = lib_settings.ArtifactDetectSetting(art_bord=110,
+                                         allowed_percent_artpoints=70,
+                                         raw_betap_limit=800_000,
+                                         global_artwin_sec=4,
+                                         num_wins_for_quality_avg=125,
+                                         hamming_win_spectrum=True,
+                                         hanning_win_spectrum=False,
+                                         total_pow_border=400_000_000,
+                                         spect_art_by_totalp=True)
+
+sads = lib_settings.ShortArtifactDetectSetting(ampl_art_detect_win_size=200,
+                                               ampl_art_zerod_area=200,
+                                               ampl_art_extremum_border=25)
 
-ads = ArtifactDetectSetting(hanning_win_spectrum=True, num_wins_for_quality_avg=125)
+mss = lib_settings.MentalAndSpectralSetting(n_sec_for_averaging=2,
+                                            n_sec_for_instant_estimation=4)
 
-sads = ShortArtifactDetectSetting(ampl_art_extremum_border=25)
-
-mss = MentalAndSpectralSetting()
-
-emotions = EmotionalMath(mls, ads, sads, mss)
+math = EmotionalMath(mls, ads, sads, mss)
 ```
 
 ### Optional parameters
 
-##### Python
 ```python
 # setting calibration length
-calibration_length = 8
+calibration_length = 6
 math.set_calibration_length(calibration_length)
 
 # type of evaluation of instant mental levels
 independent_mental_levels = False
 math.set_mental_estimation_mode(independent_mental_levels)
 
 # number of windows after the artifact with the previous actual value
@@ -157,68 +167,68 @@
 1. LEFT
 2. RIGHT
 3. NONE
 
 ## Usage
 1. If you need calibration start calibration right after library init:
 
-##### Python
 ```python
 math.start_calibration()
 ``` 
 
 2. Adding and process data
 In bipolar mode:
 
-##### Python
 ```python
-samples = []
-math.push_data(samples)
-math.process_data_arr()
+def on_brain_bit_signal_data_received(sensor, data):
+    raw_channels = []
+    for sample in data:
+        left_bipolar = sample.T3-sample.O1
+        right_bipolar = sample.T4-sample.O2
+        raw_channels.append(support_classes.RawChannels(left_bipolar, right_bipolar))
+    
+    math.push_data(raw_channels)
+    math.process_data_arr()
+...
+sensor.signalDataReceived = on_brain_bit_signal_data_received
 ``` 
 
 In multy-channel mode:
 
-##### Python
 ```python
 samples = []
 math.push_data_arr(samples)
 math.process_data_arr()
 ``` 
 2. Then check calibration status if you need to calibrate values:
 
-##### Python
 ```python
 calibration_finished = math.calibration_finished()
 # and calibration progress
 calibration_progress = math.get_calibration_percents()
 ``` 
 3. If calibration finished (or you don't need to calibrate) read output values:
 
-##### Python
 ```python
 # Reading mental levels in percent
 mental_data = math.read_mental_data_arr()
 # Reading relative spectral values in percent
 sp_data = math.read_spectral_data_percents_arr()
 ``` 
 4. Check artifacts
 4.1. During calibration
 
-##### Python
 ```python
 if math.is_both_sides_artifacted():
     # signal corruption
 ``` 
 4.2. After (without) calibration
 
-##### Python
 ```python
 if math.is_artifacted_sequence():
     # signal corruption
 ``` 
 ## Finishing work with the library
 
-##### Python
 ```python
 del math
 ```
```

### Comparing `pyem_st_artifacts-1.0.2/pyem_st_artifacts.egg-info/SOURCES.txt` & `pyem_st_artifacts-1.0.3/pyem_st_artifacts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyem_st_artifacts-1.0.2/setup.py` & `pyem_st_artifacts-1.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='pyem_st_artifacts',
-    version='1.0.2',
+    version='1.0.3',
     py_modules=[
         'em_st_artifacts.emotional_math',
         'em_st_artifacts.utils.lib_settings',
         'em_st_artifacts.utils.support_classes',
         'em_st_artifacts.utils.EmotionalMathException'],
     packages=['em_st_artifacts'],
     url='https://gitlab.com/neurosdk2/neurosamples/-/tree/main/python',
@@ -22,11 +22,12 @@
     include_package_data=True,
     package_data={"em_st_artifacts": ['libs\\x64\\em_st_artifacts-x64.dll',
                                       'libs\\x86\\em_st_artifacts-x86.dll']},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: Microsoft :: Windows",
+        "Operating System :: POSIX :: Linux",
         "Intended Audience :: Developers",
     ],
     python_requires='>=3.7',
 )
```

