# Comparing `tmp/pyneurosdk2-1.0.8.tar.gz` & `tmp/pyneurosdk2-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyneurosdk2-1.0.8.tar", last modified: Mon May 27 12:25:43 2024, max compression
+gzip compressed data, was "pyneurosdk2-1.0.9.tar", last modified: Thu May 30 10:17:12 2024, max compression
```

## Comparing `pyneurosdk2-1.0.8.tar` & `pyneurosdk2-1.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 12:25:43.364197 pyneurosdk2-1.0.8/
--rw-rw-rw-   0        0        0     1090 2023-04-19 10:44:40.000000 pyneurosdk2-1.0.8/LICENSE
--rw-rw-rw-   0        0        0    14127 2024-05-27 12:25:43.364197 pyneurosdk2-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    13610 2024-05-27 12:15:26.000000 pyneurosdk2-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 12:25:43.263934 pyneurosdk2-1.0.8/neurosdk/
--rw-rw-rw-   0        0        0     7899 2024-05-27 12:09:30.000000 pyneurosdk2-1.0.8/neurosdk/__cmn_types.py
--rw-rw-rw-   0        0        0        0 2022-11-24 14:53:06.000000 pyneurosdk2-1.0.8/neurosdk/__init__.py
--rw-rw-rw-   0        0        0      219 2023-02-28 10:25:36.000000 pyneurosdk2-1.0.8/neurosdk/__utils.py
--rw-rw-rw-   0        0        0     2228 2024-05-27 12:09:30.000000 pyneurosdk2-1.0.8/neurosdk/amp_sensor.py
--rw-rw-rw-   0        0        0     8420 2024-05-27 12:09:30.000000 pyneurosdk2-1.0.8/neurosdk/brainbit_2_sensor.py
--rw-rw-rw-   0        0        0      456 2024-05-27 12:09:30.000000 pyneurosdk2-1.0.8/neurosdk/brainbit_black_sensor.py
--rw-rw-rw-   0        0        0     4380 2024-05-27 12:09:30.000000 pyneurosdk2-1.0.8/neurosdk/brainbit_sensor.py
--rw-rw-rw-   0        0        0    24702 2024-05-27 12:09:30.000000 pyneurosdk2-1.0.8/neurosdk/callibri_sensor.py
--rw-rw-rw-   0        0        0    10162 2024-05-27 12:09:30.000000 pyneurosdk2-1.0.8/neurosdk/cmn_types.py
--rw-rw-rw-   0        0        0     1394 2024-05-27 12:09:30.000000 pyneurosdk2-1.0.8/neurosdk/electrode_sensor.py
--rw-rw-rw-   0        0        0     1499 2024-05-27 12:09:30.000000 pyneurosdk2-1.0.8/neurosdk/envelope_sensor.py
--rw-rw-rw-   0        0        0     4898 2024-05-27 12:09:30.000000 pyneurosdk2-1.0.8/neurosdk/fpg_sensor.py
-drwxrwxrwx   0        0        0        0 2024-05-27 12:25:43.339958 pyneurosdk2-1.0.8/neurosdk/libs/
--rw-rw-rw-   0        0        0   792576 2024-05-27 12:11:19.000000 pyneurosdk2-1.0.8/neurosdk/libs/neurosdk2-x32.dll
--rw-rw-rw-   0        0        0  1110016 2024-05-27 12:05:48.000000 pyneurosdk2-1.0.8/neurosdk/libs/neurosdk2-x64.dll
--rw-rw-rw-   0        0        0     4327 2024-05-27 12:09:30.000000 pyneurosdk2-1.0.8/neurosdk/mems_sensor.py
--rw-rw-rw-   0        0        0     1073 2024-05-27 12:09:30.000000 pyneurosdk2-1.0.8/neurosdk/neuro_smart_sensor.py
--rw-rw-rw-   0        0        0     1767 2024-05-27 12:09:30.000000 pyneurosdk2-1.0.8/neurosdk/resist_sensor.py
--rw-rw-rw-   0        0        0     1581 2024-05-27 12:09:30.000000 pyneurosdk2-1.0.8/neurosdk/respiration_sensor.py
--rw-rw-rw-   0        0        0     6522 2024-05-13 13:38:39.000000 pyneurosdk2-1.0.8/neurosdk/sample.py
--rw-rw-rw-   0        0        0     8924 2024-05-27 12:09:30.000000 pyneurosdk2-1.0.8/neurosdk/scanner.py
--rw-rw-rw-   0        0        0    17478 2024-05-08 11:07:42.000000 pyneurosdk2-1.0.8/neurosdk/sensor.py
--rw-rw-rw-   0        0        0      857 2024-05-27 12:09:30.000000 pyneurosdk2-1.0.8/neurosdk/signal_sensor.py
-drwxrwxrwx   0        0        0        0 2024-05-27 12:25:43.364197 pyneurosdk2-1.0.8/pyneurosdk2.egg-info/
--rw-rw-rw-   0        0        0    14127 2024-05-27 12:25:43.000000 pyneurosdk2-1.0.8/pyneurosdk2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      736 2024-05-27 12:25:43.000000 pyneurosdk2-1.0.8/pyneurosdk2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 12:25:43.000000 pyneurosdk2-1.0.8/pyneurosdk2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-27 12:25:43.000000 pyneurosdk2-1.0.8/pyneurosdk2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 12:25:43.367209 pyneurosdk2-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1502 2024-05-27 12:09:30.000000 pyneurosdk2-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 10:17:12.410090 pyneurosdk2-1.0.9/
+-rw-rw-rw-   0        0        0     1090 2023-04-19 10:44:40.000000 pyneurosdk2-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0    14495 2024-05-30 10:17:12.409090 pyneurosdk2-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    13930 2024-05-30 10:01:48.000000 pyneurosdk2-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 10:17:12.315440 pyneurosdk2-1.0.9/neurosdk/
+-rw-rw-rw-   0        0        0     7899 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9/neurosdk/__cmn_types.py
+-rw-rw-rw-   0        0        0        0 2022-11-24 14:53:06.000000 pyneurosdk2-1.0.9/neurosdk/__init__.py
+-rw-rw-rw-   0        0        0      219 2023-02-28 10:25:36.000000 pyneurosdk2-1.0.9/neurosdk/__utils.py
+-rw-rw-rw-   0        0        0     2228 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9/neurosdk/amp_sensor.py
+-rw-rw-rw-   0        0        0     8420 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9/neurosdk/brainbit_2_sensor.py
+-rw-rw-rw-   0        0        0      456 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9/neurosdk/brainbit_black_sensor.py
+-rw-rw-rw-   0        0        0     4380 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9/neurosdk/brainbit_sensor.py
+-rw-rw-rw-   0        0        0    24702 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9/neurosdk/callibri_sensor.py
+-rw-rw-rw-   0        0        0    10162 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9/neurosdk/cmn_types.py
+-rw-rw-rw-   0        0        0     1394 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9/neurosdk/electrode_sensor.py
+-rw-rw-rw-   0        0        0     1499 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9/neurosdk/envelope_sensor.py
+-rw-rw-rw-   0        0        0     4898 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9/neurosdk/fpg_sensor.py
+drwxrwxrwx   0        0        0        0 2024-05-30 10:17:12.385467 pyneurosdk2-1.0.9/neurosdk/libs/
+-rw-rw-rw-   0        0        0   792576 2024-05-27 12:11:19.000000 pyneurosdk2-1.0.9/neurosdk/libs/neurosdk2-x32.dll
+-rw-rw-rw-   0        0        0  1110016 2024-05-27 12:05:48.000000 pyneurosdk2-1.0.9/neurosdk/libs/neurosdk2-x64.dll
+-rw-rw-rw-   0        0        0     4327 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9/neurosdk/mems_sensor.py
+-rw-rw-rw-   0        0        0     1073 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9/neurosdk/neuro_smart_sensor.py
+-rw-rw-rw-   0        0        0     1767 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9/neurosdk/resist_sensor.py
+-rw-rw-rw-   0        0        0     1581 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9/neurosdk/respiration_sensor.py
+-rw-rw-rw-   0        0        0     6525 2024-05-27 12:36:12.000000 pyneurosdk2-1.0.9/neurosdk/sample.py
+-rw-rw-rw-   0        0        0     8924 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9/neurosdk/scanner.py
+-rw-rw-rw-   0        0        0    17514 2024-05-30 09:20:48.000000 pyneurosdk2-1.0.9/neurosdk/sensor.py
+-rw-rw-rw-   0        0        0      857 2024-05-27 14:09:43.000000 pyneurosdk2-1.0.9/neurosdk/signal_sensor.py
+drwxrwxrwx   0        0        0        0 2024-05-30 10:17:12.407092 pyneurosdk2-1.0.9/pyneurosdk2.egg-info/
+-rw-rw-rw-   0        0        0    14495 2024-05-30 10:17:11.000000 pyneurosdk2-1.0.9/pyneurosdk2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      736 2024-05-30 10:17:11.000000 pyneurosdk2-1.0.9/pyneurosdk2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 10:17:11.000000 pyneurosdk2-1.0.9/pyneurosdk2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-30 10:17:11.000000 pyneurosdk2-1.0.9/pyneurosdk2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 10:17:12.411125 pyneurosdk2-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1549 2024-05-30 09:26:50.000000 pyneurosdk2-1.0.9/setup.py
```

### Comparing `pyneurosdk2-1.0.8/LICENSE` & `pyneurosdk2-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.8/PKG-INFO` & `pyneurosdk2-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: pyneurosdk2
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python wrapper for NeuroSDK2
 Home-page: https://gitlab.com/brainbit-inc/brainbit-sdk
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
 
 # Python NeuroSDK 2
 
@@ -32,14 +33,24 @@
 
 ## Installing
 
 ```
 pip install pyneurosdk2
 ```
 
+### Linux
+
+Currently only Astra Linux is supported. It is necessary to install NeuroSDK2 library before using it:
+
+1. Download NeuroSDK2 `libneurosdk2.deb` package from [GitHub](https://github.com/BrainbitLLC/linux_neurosdk2/tree/main/package)
+2. Install package: 
+```
+sudo apt install ./libneurosdk2.deb
+```
+
 ## Description
 
 The package has the following structure:
  - neurosdk - the main package with the implementation of methods
  - sample - is into the neurosdk package, file `sample.py`
  - libs - also into neurosdk package, contain dll library files
```

### Comparing `pyneurosdk2-1.0.8/README.md` & `pyneurosdk2-1.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,24 @@
 
 ## Installing
 
 ```
 pip install pyneurosdk2
 ```
 
+### Linux
+
+Currently only Astra Linux is supported. It is necessary to install NeuroSDK2 library before using it:
+
+1. Download NeuroSDK2 `libneurosdk2.deb` package from [GitHub](https://github.com/BrainbitLLC/linux_neurosdk2/tree/main/package)
+2. Install package: 
+```
+sudo apt install ./libneurosdk2.deb
+```
+
 ## Description
 
 The package has the following structure:
  - neurosdk - the main package with the implementation of methods
  - sample - is into the neurosdk package, file `sample.py`
  - libs - also into neurosdk package, contain dll library files
```

### Comparing `pyneurosdk2-1.0.8/neurosdk/__cmn_types.py` & `pyneurosdk2-1.0.9/neurosdk/__cmn_types.py`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.8/neurosdk/amp_sensor.py` & `pyneurosdk2-1.0.9/neurosdk/amp_sensor.py`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.8/neurosdk/brainbit_2_sensor.py` & `pyneurosdk2-1.0.9/neurosdk/brainbit_2_sensor.py`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.8/neurosdk/brainbit_sensor.py` & `pyneurosdk2-1.0.9/neurosdk/brainbit_sensor.py`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.8/neurosdk/callibri_sensor.py` & `pyneurosdk2-1.0.9/neurosdk/callibri_sensor.py`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.8/neurosdk/cmn_types.py` & `pyneurosdk2-1.0.9/neurosdk/cmn_types.py`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.8/neurosdk/electrode_sensor.py` & `pyneurosdk2-1.0.9/neurosdk/electrode_sensor.py`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.8/neurosdk/envelope_sensor.py` & `pyneurosdk2-1.0.9/neurosdk/envelope_sensor.py`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.8/neurosdk/fpg_sensor.py` & `pyneurosdk2-1.0.9/neurosdk/fpg_sensor.py`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.8/neurosdk/libs/neurosdk2-x32.dll` & `pyneurosdk2-1.0.9/neurosdk/libs/neurosdk2-x32.dll`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.8/neurosdk/libs/neurosdk2-x64.dll` & `pyneurosdk2-1.0.9/neurosdk/libs/neurosdk2-x64.dll`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.8/neurosdk/mems_sensor.py` & `pyneurosdk2-1.0.9/neurosdk/mems_sensor.py`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.8/neurosdk/neuro_smart_sensor.py` & `pyneurosdk2-1.0.9/neurosdk/neuro_smart_sensor.py`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.8/neurosdk/resist_sensor.py` & `pyneurosdk2-1.0.9/neurosdk/resist_sensor.py`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.8/neurosdk/respiration_sensor.py` & `pyneurosdk2-1.0.9/neurosdk/respiration_sensor.py`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.8/neurosdk/sample.py` & `pyneurosdk2-1.0.9/neurosdk/sample.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from scanner import Scanner
 from cmn_types import *
-from callibri_sensor import CallibriSensor
+from brainbit_2_sensor import BrainBit2Sensor
 
 import concurrent.futures
 from time import sleep
 
 
 def sensor_found(scanner, sensors):
     for index in range(len(sensors)):
```

### Comparing `pyneurosdk2-1.0.8/neurosdk/scanner.py` & `pyneurosdk2-1.0.9/neurosdk/scanner.py`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.8/neurosdk/sensor.py` & `pyneurosdk2-1.0.9/neurosdk/sensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 if sys.platform == "win32":
     arc = platform.architecture()
     if arc[0].__contains__("64"):
         _libname = pathlib.Path(__file__).parent.resolve() / "libs" / "neurosdk2-x64.dll"
     else:
         _libname = pathlib.Path(__file__).parent.resolve() / "libs" / "neurosdk2-x32.dll"
 elif sys.platform.startswith("linux"):
-    print('Add linux lib')
+    # print('Add linux lib')
+    _libname = "libneurosdk2.so"
 elif sys.platform == "darwin":
     print('Add macos lib')
 else:
     raise Exception("This platform (%s) is currently not supported by py_neurosdk." % sys.platform)
 
 _neuro_lib = CDLL(str(_libname))
```

### Comparing `pyneurosdk2-1.0.8/neurosdk/signal_sensor.py` & `pyneurosdk2-1.0.9/neurosdk/signal_sensor.py`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.8/pyneurosdk2.egg-info/PKG-INFO` & `pyneurosdk2-1.0.9/pyneurosdk2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: pyneurosdk2
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python wrapper for NeuroSDK2
 Home-page: https://gitlab.com/brainbit-inc/brainbit-sdk
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
 
 # Python NeuroSDK 2
 
@@ -32,14 +33,24 @@
 
 ## Installing
 
 ```
 pip install pyneurosdk2
 ```
 
+### Linux
+
+Currently only Astra Linux is supported. It is necessary to install NeuroSDK2 library before using it:
+
+1. Download NeuroSDK2 `libneurosdk2.deb` package from [GitHub](https://github.com/BrainbitLLC/linux_neurosdk2/tree/main/package)
+2. Install package: 
+```
+sudo apt install ./libneurosdk2.deb
+```
+
 ## Description
 
 The package has the following structure:
  - neurosdk - the main package with the implementation of methods
  - sample - is into the neurosdk package, file `sample.py`
  - libs - also into neurosdk package, contain dll library files
```

### Comparing `pyneurosdk2-1.0.8/pyneurosdk2.egg-info/SOURCES.txt` & `pyneurosdk2-1.0.9/pyneurosdk2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyneurosdk2-1.0.8/setup.py` & `pyneurosdk2-1.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='pyneurosdk2',
-    version='1.0.8',
+    version='1.0.9',
     py_modules=[
         'neurosdk.scanner',
         'neurosdk.sensor',
         'neurosdk.cmn_types',
         'neurosdk.__cmn_types',
         'neurosdk.__utils',
         'neurosdk.amp_sensor',
@@ -38,11 +38,12 @@
     long_description_content_type='text/markdown',
     include_package_data=True,
     package_data={"neurosdk": ['libs\\neurosdk2-x32.dll', 'libs\\neurosdk2-x64.dll']},
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

