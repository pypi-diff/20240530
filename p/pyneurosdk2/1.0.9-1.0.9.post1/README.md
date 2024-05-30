# Comparing `tmp/pyneurosdk2-1.0.9.tar.gz` & `tmp/pyneurosdk2-1.0.9.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyneurosdk2-1.0.9.tar", last modified: Thu May 30 10:17:12 2024, max compression
+gzip compressed data, was "pyneurosdk2-1.0.9.post1.tar", last modified: Thu May 30 12:07:33 2024, max compression
```

## Comparing `pyneurosdk2-1.0.9.tar` & `pyneurosdk2-1.0.9.post1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 10:17:12.410090 pyneurosdk2-1.0.9/
--rw-rw-rw-   0        0        0     1090 2023-04-19 10:44:40.000000 pyneurosdk2-1.0.9/LICENSE
--rw-rw-rw-   0        0        0    14495 2024-05-30 10:17:12.409090 pyneurosdk2-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0    13930 2024-05-30 10:01:48.000000 pyneurosdk2-1.0.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 10:17:12.315440 pyneurosdk2-1.0.9/neurosdk/
--rw-rw-rw-   0        0        0     7899 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9/neurosdk/__cmn_types.py
--rw-rw-rw-   0        0        0        0 2022-11-24 14:53:06.000000 pyneurosdk2-1.0.9/neurosdk/__init__.py
--rw-rw-rw-   0        0        0      219 2023-02-28 10:25:36.000000 pyneurosdk2-1.0.9/neurosdk/__utils.py
--rw-rw-rw-   0        0        0     2228 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9/neurosdk/amp_sensor.py
--rw-rw-rw-   0        0        0     8420 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9/neurosdk/brainbit_2_sensor.py
--rw-rw-rw-   0        0        0      456 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9/neurosdk/brainbit_black_sensor.py
--rw-rw-rw-   0        0        0     4380 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9/neurosdk/brainbit_sensor.py
--rw-rw-rw-   0        0        0    24702 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9/neurosdk/callibri_sensor.py
--rw-rw-rw-   0        0        0    10162 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9/neurosdk/cmn_types.py
--rw-rw-rw-   0        0        0     1394 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9/neurosdk/electrode_sensor.py
--rw-rw-rw-   0        0        0     1499 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9/neurosdk/envelope_sensor.py
--rw-rw-rw-   0        0        0     4898 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9/neurosdk/fpg_sensor.py
-drwxrwxrwx   0        0        0        0 2024-05-30 10:17:12.385467 pyneurosdk2-1.0.9/neurosdk/libs/
--rw-rw-rw-   0        0        0   792576 2024-05-27 12:11:19.000000 pyneurosdk2-1.0.9/neurosdk/libs/neurosdk2-x32.dll
--rw-rw-rw-   0        0        0  1110016 2024-05-27 12:05:48.000000 pyneurosdk2-1.0.9/neurosdk/libs/neurosdk2-x64.dll
--rw-rw-rw-   0        0        0     4327 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9/neurosdk/mems_sensor.py
--rw-rw-rw-   0        0        0     1073 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9/neurosdk/neuro_smart_sensor.py
--rw-rw-rw-   0        0        0     1767 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9/neurosdk/resist_sensor.py
--rw-rw-rw-   0        0        0     1581 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9/neurosdk/respiration_sensor.py
--rw-rw-rw-   0        0        0     6525 2024-05-27 12:36:12.000000 pyneurosdk2-1.0.9/neurosdk/sample.py
--rw-rw-rw-   0        0        0     8924 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9/neurosdk/scanner.py
--rw-rw-rw-   0        0        0    17514 2024-05-30 09:20:48.000000 pyneurosdk2-1.0.9/neurosdk/sensor.py
--rw-rw-rw-   0        0        0      857 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9/neurosdk/signal_sensor.py
-drwxrwxrwx   0        0        0        0 2024-05-30 10:17:12.407092 pyneurosdk2-1.0.9/pyneurosdk2.egg-info/
--rw-rw-rw-   0        0        0    14495 2024-05-30 10:17:11.000000 pyneurosdk2-1.0.9/pyneurosdk2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      736 2024-05-30 10:17:11.000000 pyneurosdk2-1.0.9/pyneurosdk2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 10:17:11.000000 pyneurosdk2-1.0.9/pyneurosdk2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-30 10:17:11.000000 pyneurosdk2-1.0.9/pyneurosdk2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 10:17:12.411125 pyneurosdk2-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1549 2024-05-30 09:26:50.000000 pyneurosdk2-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:07:33.598005 pyneurosdk2-1.0.9.post1/
+-rw-rw-rw-   0        0        0     1090 2023-04-19 10:44:40.000000 pyneurosdk2-1.0.9.post1/LICENSE
+-rw-rw-rw-   0        0        0    14139 2024-05-30 12:07:33.596463 pyneurosdk2-1.0.9.post1/PKG-INFO
+-rw-rw-rw-   0        0        0    13568 2024-05-30 12:07:17.000000 pyneurosdk2-1.0.9.post1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 12:07:33.573221 pyneurosdk2-1.0.9.post1/neurosdk/
+-rw-rw-rw-   0        0        0     7899 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9.post1/neurosdk/__cmn_types.py
+-rw-rw-rw-   0        0        0        0 2022-11-24 14:53:06.000000 pyneurosdk2-1.0.9.post1/neurosdk/__init__.py
+-rw-rw-rw-   0        0        0      219 2023-02-28 10:25:36.000000 pyneurosdk2-1.0.9.post1/neurosdk/__utils.py
+-rw-rw-rw-   0        0        0     2228 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9.post1/neurosdk/amp_sensor.py
+-rw-rw-rw-   0        0        0     8420 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9.post1/neurosdk/brainbit_2_sensor.py
+-rw-rw-rw-   0        0        0      456 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9.post1/neurosdk/brainbit_black_sensor.py
+-rw-rw-rw-   0        0        0     4380 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9.post1/neurosdk/brainbit_sensor.py
+-rw-rw-rw-   0        0        0    24702 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9.post1/neurosdk/callibri_sensor.py
+-rw-rw-rw-   0        0        0    10162 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9.post1/neurosdk/cmn_types.py
+-rw-rw-rw-   0        0        0     1394 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9.post1/neurosdk/electrode_sensor.py
+-rw-rw-rw-   0        0        0     1499 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9.post1/neurosdk/envelope_sensor.py
+-rw-rw-rw-   0        0        0     4898 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9.post1/neurosdk/fpg_sensor.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:07:33.575285 pyneurosdk2-1.0.9.post1/neurosdk/libs/
+-rw-rw-rw-   0        0        0   792576 2024-05-27 12:11:19.000000 pyneurosdk2-1.0.9.post1/neurosdk/libs/neurosdk2-x32.dll
+-rw-rw-rw-   0        0        0  1110016 2024-05-27 12:05:48.000000 pyneurosdk2-1.0.9.post1/neurosdk/libs/neurosdk2-x64.dll
+-rw-rw-rw-   0        0        0     4327 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9.post1/neurosdk/mems_sensor.py
+-rw-rw-rw-   0        0        0     1073 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9.post1/neurosdk/neuro_smart_sensor.py
+-rw-rw-rw-   0        0        0     1767 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9.post1/neurosdk/resist_sensor.py
+-rw-rw-rw-   0        0        0     1581 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9.post1/neurosdk/respiration_sensor.py
+-rw-rw-rw-   0        0        0     6525 2024-05-27 12:36:12.000000 pyneurosdk2-1.0.9.post1/neurosdk/sample.py
+-rw-rw-rw-   0        0        0     8924 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9.post1/neurosdk/scanner.py
+-rw-rw-rw-   0        0        0    17514 2024-05-30 09:20:48.000000 pyneurosdk2-1.0.9.post1/neurosdk/sensor.py
+-rw-rw-rw-   0        0        0      857 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9.post1/neurosdk/signal_sensor.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:07:33.596463 pyneurosdk2-1.0.9.post1/pyneurosdk2.egg-info/
+-rw-rw-rw-   0        0        0    14139 2024-05-30 12:07:33.000000 pyneurosdk2-1.0.9.post1/pyneurosdk2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      736 2024-05-30 12:07:33.000000 pyneurosdk2-1.0.9.post1/pyneurosdk2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 12:07:33.000000 pyneurosdk2-1.0.9.post1/pyneurosdk2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-30 12:07:33.000000 pyneurosdk2-1.0.9.post1/pyneurosdk2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 12:07:33.598005 pyneurosdk2-1.0.9.post1/setup.cfg
+-rw-rw-rw-   0        0        0     1555 2024-05-30 11:53:36.000000 pyneurosdk2-1.0.9.post1/setup.py
```

### Comparing `pyneurosdk2-1.0.9/LICENSE` & `pyneurosdk2-1.0.9.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.9/PKG-INFO` & `pyneurosdk2-1.0.9.post1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneurosdk2
-Version: 1.0.9
+Version: 1.0.9.post1
 Summary: Python wrapper for NeuroSDK2
 Home-page: https://gitlab.com/brainbit-inc/brainbit-sdk
 Author: Brainbit Inc.
 Author-email: support@brainbit.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,26 +13,26 @@
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Python NeuroSDK 2
 
-Welcome to the Python NeuroSDK 2. The Neurosdk library is designed to work with BrainBit, BrainBitBlack, Callibri and Kolibri devices. The library is intended for python version 3.7 and higher, Windows version 10 and higher.
+Welcome to the Python NeuroSDK 2. The Neurosdk library is designed to work with BrainBit, BrainBitBlack, Callibri and Kolibri devices. The library is intended for python version 3.7 and higher, Windows version 10 and higher, Astra Linux.
 
 ## Documentation
 
 - [Installing](#installing)
 - [Description](#description)
 - [Searching device](#searching-device)
 - [Connection](#connection)
 - [Parameters](#paramaters)
-- [Receiving signal](#receiving-signal)
-- [Receiving resistance](#receiving-resistance)
-- [Electrodes connection](#electrodes-connection)
+- [BrainBit sensor](#brainbit-brainbitblack-flex)
+- [Callibri sensor](#callibri-kolibri)
+- [BrainBit 2 sensor](#brainbit-2)
 - [Clean up](#clean_up)
 
 ## Installing
 
 ```
 pip install pyneurosdk2
 ```
@@ -78,15 +78,15 @@
 ```
 
 ## Searching device
 
 The `Scanner` class is used to search for a device. For a correct search, you must specify the list of device types. You can search for one or more device types at the same time. For example, to search for BrainBit and Callibri, you need to create a scanner as follows:
 
 ```python
-scanner = Scanner([SensorFamily.LEBrainBit, SensorFamily.LECallibri])
+scanner = Scanner([SensorFamily.LEBrainBit, SensorFamily.LEBrainBit2, SensorFamily.LECallibri])
 ```
 
 Search start:
 
 ```python
 scanner.start()
 ```
@@ -188,30 +188,24 @@
 
 ```python
 sensor.is_supported_feature(sensor_future)
 sensor.is_supported_command(sensor_command)
 sensor.is_supported_parameter(sensor_parameter)
 ```
 
-## Receiving signal
-
-For any device that supports recieving signal, you can run the following commands for starting:
+## BrainBit, BrainBitBlack, Flex
 
-```python
-sensor.exec_command(SensorCommand.StartSignal)
-```
+### Gain
 
-Stop:
+You can set gain parameter to BrainBit sensor:
 
 ```python
-sensor.exec_command(SensorCommand.StopSignal)
+sensor.gain = SensorGain.Gain3
 ```
 
-## BrainBit, BrainBitBlack, Flex
-
 ### Receiving signal
 
 You can get the signal value using the callback:
 
 ```python
 def on_brain_bit_signal_data_received(sensor, data):
     print(data)
@@ -409,34 +403,28 @@
 - Samples: [float] - array of samples in V. Each sample number into array consistent with `Num` value of `EEGChannelInfo` from `supported_channels` property.
 
 ### Receiving resistance
 
 To get resistance values:
 
 ```python
-def on_brain_bit_resist_data_received(sensor, data):
+def on_brain_bit_2_resist_data_received(sensor, data):
     print(data)
 
 
-sensor.resistDataReceived = on_brain_bit_resist_data_received
+sensor.resistDataReceived = on_brain_bit_2_resist_data_received
 
 sensor.exec_command(SensorCommand.StartResist)
 sensor.exec_command(SensorCommand.StopResist)
 ```
 
-The callback returns one packet of samples, each packet contains the resistance values in volts:
-- O1: float
-- O2: float
-- T3: float
-- T4: float
-
 You get resistance values structure of samples (`ResistRefChannelsData`) for each channel:
- - PackNum - number for each packet
- - Samples - array of values in Ohm. Each sample number into array consistent with `Num` value of `EEGChannelInfo` from `supported_channels` property.
- - Referents - array of values for referents channels. For BrainBit2 sensor is empty now.
+ - PackNum: int - number for each packet
+ - Samples: [float] - array of values in Ohm. Each sample number into array consistent with `Num` value of `EEGChannelInfo` from `supported_channels` property.
+ - Referents: [float] - array of values for referents channels. For BrainBit2 sensor is empty now.
 
 After you have finished working with the resistance, you can unsubscribe from the callback as follows:
 
 ```python
 sensor.resistDataReceived = None
 ```
 
@@ -493,13 +481,7 @@
 
 After you finish working with the device, you need to clean up the resources used. This happens in the destructor of the scanner and sensor, so if they were not called by the system, you must call them manually.
 
 ```python
 del sensor
 del scanner
 ```
-
-## License
-
-Copyright (c) Brainbit Inc. All rights reserved.
-
-Licensed under the [MIT license](LICENSE).
```

### Comparing `pyneurosdk2-1.0.9/README.md` & `pyneurosdk2-1.0.9.post1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # Python NeuroSDK 2
 
-Welcome to the Python NeuroSDK 2. The Neurosdk library is designed to work with BrainBit, BrainBitBlack, Callibri and Kolibri devices. The library is intended for python version 3.7 and higher, Windows version 10 and higher.
+Welcome to the Python NeuroSDK 2. The Neurosdk library is designed to work with BrainBit, BrainBitBlack, Callibri and Kolibri devices. The library is intended for python version 3.7 and higher, Windows version 10 and higher, Astra Linux.
 
 ## Documentation
 
 - [Installing](#installing)
 - [Description](#description)
 - [Searching device](#searching-device)
 - [Connection](#connection)
 - [Parameters](#paramaters)
-- [Receiving signal](#receiving-signal)
-- [Receiving resistance](#receiving-resistance)
-- [Electrodes connection](#electrodes-connection)
+- [BrainBit sensor](#brainbit-brainbitblack-flex)
+- [Callibri sensor](#callibri-kolibri)
+- [BrainBit 2 sensor](#brainbit-2)
 - [Clean up](#clean_up)
 
 ## Installing
 
 ```
 pip install pyneurosdk2
 ```
@@ -61,15 +61,15 @@
 ```
 
 ## Searching device
 
 The `Scanner` class is used to search for a device. For a correct search, you must specify the list of device types. You can search for one or more device types at the same time. For example, to search for BrainBit and Callibri, you need to create a scanner as follows:
 
 ```python
-scanner = Scanner([SensorFamily.LEBrainBit, SensorFamily.LECallibri])
+scanner = Scanner([SensorFamily.LEBrainBit, SensorFamily.LEBrainBit2, SensorFamily.LECallibri])
 ```
 
 Search start:
 
 ```python
 scanner.start()
 ```
@@ -171,30 +171,24 @@
 
 ```python
 sensor.is_supported_feature(sensor_future)
 sensor.is_supported_command(sensor_command)
 sensor.is_supported_parameter(sensor_parameter)
 ```
 
-## Receiving signal
-
-For any device that supports recieving signal, you can run the following commands for starting:
+## BrainBit, BrainBitBlack, Flex
 
-```python
-sensor.exec_command(SensorCommand.StartSignal)
-```
+### Gain
 
-Stop:
+You can set gain parameter to BrainBit sensor:
 
 ```python
-sensor.exec_command(SensorCommand.StopSignal)
+sensor.gain = SensorGain.Gain3
 ```
 
-## BrainBit, BrainBitBlack, Flex
-
 ### Receiving signal
 
 You can get the signal value using the callback:
 
 ```python
 def on_brain_bit_signal_data_received(sensor, data):
     print(data)
@@ -392,34 +386,28 @@
 - Samples: [float] - array of samples in V. Each sample number into array consistent with `Num` value of `EEGChannelInfo` from `supported_channels` property.
 
 ### Receiving resistance
 
 To get resistance values:
 
 ```python
-def on_brain_bit_resist_data_received(sensor, data):
+def on_brain_bit_2_resist_data_received(sensor, data):
     print(data)
 
 
-sensor.resistDataReceived = on_brain_bit_resist_data_received
+sensor.resistDataReceived = on_brain_bit_2_resist_data_received
 
 sensor.exec_command(SensorCommand.StartResist)
 sensor.exec_command(SensorCommand.StopResist)
 ```
 
-The callback returns one packet of samples, each packet contains the resistance values in volts:
-- O1: float
-- O2: float
-- T3: float
-- T4: float
-
 You get resistance values structure of samples (`ResistRefChannelsData`) for each channel:
- - PackNum - number for each packet
- - Samples - array of values in Ohm. Each sample number into array consistent with `Num` value of `EEGChannelInfo` from `supported_channels` property.
- - Referents - array of values for referents channels. For BrainBit2 sensor is empty now.
+ - PackNum: int - number for each packet
+ - Samples: [float] - array of values in Ohm. Each sample number into array consistent with `Num` value of `EEGChannelInfo` from `supported_channels` property.
+ - Referents: [float] - array of values for referents channels. For BrainBit2 sensor is empty now.
 
 After you have finished working with the resistance, you can unsubscribe from the callback as follows:
 
 ```python
 sensor.resistDataReceived = None
 ```
 
@@ -476,13 +464,7 @@
 
 After you finish working with the device, you need to clean up the resources used. This happens in the destructor of the scanner and sensor, so if they were not called by the system, you must call them manually.
 
 ```python
 del sensor
 del scanner
 ```
-
-## License
-
-Copyright (c) Brainbit Inc. All rights reserved.
-
-Licensed under the [MIT license](LICENSE).
```

### Comparing `pyneurosdk2-1.0.9/neurosdk/__cmn_types.py` & `pyneurosdk2-1.0.9.post1/neurosdk/__cmn_types.py`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.9/neurosdk/amp_sensor.py` & `pyneurosdk2-1.0.9.post1/neurosdk/amp_sensor.py`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.9/neurosdk/brainbit_2_sensor.py` & `pyneurosdk2-1.0.9.post1/neurosdk/brainbit_2_sensor.py`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.9/neurosdk/brainbit_sensor.py` & `pyneurosdk2-1.0.9.post1/neurosdk/brainbit_sensor.py`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.9/neurosdk/callibri_sensor.py` & `pyneurosdk2-1.0.9.post1/neurosdk/callibri_sensor.py`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.9/neurosdk/cmn_types.py` & `pyneurosdk2-1.0.9.post1/neurosdk/cmn_types.py`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.9/neurosdk/electrode_sensor.py` & `pyneurosdk2-1.0.9.post1/neurosdk/electrode_sensor.py`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.9/neurosdk/envelope_sensor.py` & `pyneurosdk2-1.0.9.post1/neurosdk/envelope_sensor.py`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.9/neurosdk/fpg_sensor.py` & `pyneurosdk2-1.0.9.post1/neurosdk/fpg_sensor.py`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.9/neurosdk/libs/neurosdk2-x32.dll` & `pyneurosdk2-1.0.9.post1/neurosdk/libs/neurosdk2-x32.dll`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.9/neurosdk/libs/neurosdk2-x64.dll` & `pyneurosdk2-1.0.9.post1/neurosdk/libs/neurosdk2-x64.dll`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.9/neurosdk/mems_sensor.py` & `pyneurosdk2-1.0.9.post1/neurosdk/mems_sensor.py`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.9/neurosdk/neuro_smart_sensor.py` & `pyneurosdk2-1.0.9.post1/neurosdk/neuro_smart_sensor.py`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.9/neurosdk/resist_sensor.py` & `pyneurosdk2-1.0.9.post1/neurosdk/resist_sensor.py`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.9/neurosdk/respiration_sensor.py` & `pyneurosdk2-1.0.9.post1/neurosdk/respiration_sensor.py`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.9/neurosdk/sample.py` & `pyneurosdk2-1.0.9.post1/neurosdk/sample.py`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.9/neurosdk/scanner.py` & `pyneurosdk2-1.0.9.post1/neurosdk/scanner.py`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.9/neurosdk/sensor.py` & `pyneurosdk2-1.0.9.post1/neurosdk/sensor.py`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.9/neurosdk/signal_sensor.py` & `pyneurosdk2-1.0.9.post1/neurosdk/signal_sensor.py`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.9/pyneurosdk2.egg-info/PKG-INFO` & `pyneurosdk2-1.0.9.post1/pyneurosdk2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneurosdk2
-Version: 1.0.9
+Version: 1.0.9.post1
 Summary: Python wrapper for NeuroSDK2
 Home-page: https://gitlab.com/brainbit-inc/brainbit-sdk
 Author: Brainbit Inc.
 Author-email: support@brainbit.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,26 +13,26 @@
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Python NeuroSDK 2
 
-Welcome to the Python NeuroSDK 2. The Neurosdk library is designed to work with BrainBit, BrainBitBlack, Callibri and Kolibri devices. The library is intended for python version 3.7 and higher, Windows version 10 and higher.
+Welcome to the Python NeuroSDK 2. The Neurosdk library is designed to work with BrainBit, BrainBitBlack, Callibri and Kolibri devices. The library is intended for python version 3.7 and higher, Windows version 10 and higher, Astra Linux.
 
 ## Documentation
 
 - [Installing](#installing)
 - [Description](#description)
 - [Searching device](#searching-device)
 - [Connection](#connection)
 - [Parameters](#paramaters)
-- [Receiving signal](#receiving-signal)
-- [Receiving resistance](#receiving-resistance)
-- [Electrodes connection](#electrodes-connection)
+- [BrainBit sensor](#brainbit-brainbitblack-flex)
+- [Callibri sensor](#callibri-kolibri)
+- [BrainBit 2 sensor](#brainbit-2)
 - [Clean up](#clean_up)
 
 ## Installing
 
 ```
 pip install pyneurosdk2
 ```
@@ -78,15 +78,15 @@
 ```
 
 ## Searching device
 
 The `Scanner` class is used to search for a device. For a correct search, you must specify the list of device types. You can search for one or more device types at the same time. For example, to search for BrainBit and Callibri, you need to create a scanner as follows:
 
 ```python
-scanner = Scanner([SensorFamily.LEBrainBit, SensorFamily.LECallibri])
+scanner = Scanner([SensorFamily.LEBrainBit, SensorFamily.LEBrainBit2, SensorFamily.LECallibri])
 ```
 
 Search start:
 
 ```python
 scanner.start()
 ```
@@ -188,30 +188,24 @@
 
 ```python
 sensor.is_supported_feature(sensor_future)
 sensor.is_supported_command(sensor_command)
 sensor.is_supported_parameter(sensor_parameter)
 ```
 
-## Receiving signal
-
-For any device that supports recieving signal, you can run the following commands for starting:
+## BrainBit, BrainBitBlack, Flex
 
-```python
-sensor.exec_command(SensorCommand.StartSignal)
-```
+### Gain
 
-Stop:
+You can set gain parameter to BrainBit sensor:
 
 ```python
-sensor.exec_command(SensorCommand.StopSignal)
+sensor.gain = SensorGain.Gain3
 ```
 
-## BrainBit, BrainBitBlack, Flex
-
 ### Receiving signal
 
 You can get the signal value using the callback:
 
 ```python
 def on_brain_bit_signal_data_received(sensor, data):
     print(data)
@@ -409,34 +403,28 @@
 - Samples: [float] - array of samples in V. Each sample number into array consistent with `Num` value of `EEGChannelInfo` from `supported_channels` property.
 
 ### Receiving resistance
 
 To get resistance values:
 
 ```python
-def on_brain_bit_resist_data_received(sensor, data):
+def on_brain_bit_2_resist_data_received(sensor, data):
     print(data)
 
 
-sensor.resistDataReceived = on_brain_bit_resist_data_received
+sensor.resistDataReceived = on_brain_bit_2_resist_data_received
 
 sensor.exec_command(SensorCommand.StartResist)
 sensor.exec_command(SensorCommand.StopResist)
 ```
 
-The callback returns one packet of samples, each packet contains the resistance values in volts:
-- O1: float
-- O2: float
-- T3: float
-- T4: float
-
 You get resistance values structure of samples (`ResistRefChannelsData`) for each channel:
- - PackNum - number for each packet
- - Samples - array of values in Ohm. Each sample number into array consistent with `Num` value of `EEGChannelInfo` from `supported_channels` property.
- - Referents - array of values for referents channels. For BrainBit2 sensor is empty now.
+ - PackNum: int - number for each packet
+ - Samples: [float] - array of values in Ohm. Each sample number into array consistent with `Num` value of `EEGChannelInfo` from `supported_channels` property.
+ - Referents: [float] - array of values for referents channels. For BrainBit2 sensor is empty now.
 
 After you have finished working with the resistance, you can unsubscribe from the callback as follows:
 
 ```python
 sensor.resistDataReceived = None
 ```
 
@@ -493,13 +481,7 @@
 
 After you finish working with the device, you need to clean up the resources used. This happens in the destructor of the scanner and sensor, so if they were not called by the system, you must call them manually.
 
 ```python
 del sensor
 del scanner
 ```
-
-## License
-
-Copyright (c) Brainbit Inc. All rights reserved.
-
-Licensed under the [MIT license](LICENSE).
```

### Comparing `pyneurosdk2-1.0.9/pyneurosdk2.egg-info/SOURCES.txt` & `pyneurosdk2-1.0.9.post1/pyneurosdk2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.9/setup.py` & `pyneurosdk2-1.0.9.post1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='pyneurosdk2',
-    version='1.0.9',
+    version='1.0.9.post1',
     py_modules=[
         'neurosdk.scanner',
         'neurosdk.sensor',
         'neurosdk.cmn_types',
         'neurosdk.__cmn_types',
         'neurosdk.__utils',
         'neurosdk.amp_sensor',
```

