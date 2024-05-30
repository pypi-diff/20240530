# Comparing `tmp/rosbags-0.9.8.tar.gz` & `tmp/rosbags-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosbags-0.9.8.tar", last modified: Thu Nov 25 16:28:16 2021, max compression
+gzip compressed data, was "rosbags-0.9.9.tar", last modified: Wed Jan 12 09:48:09 2022, max compression
```

## Comparing `rosbags-0.9.8.tar` & `rosbags-0.9.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 marko     (1000) marko     (1000)        0 2021-11-25 16:28:16.400735 rosbags-0.9.8/
--rw-r--r--   0 marko     (1000) marko     (1000)    11358 2021-11-25 13:22:46.000000 rosbags-0.9.8/LICENSE.txt
--rw-r--r--   0 marko     (1000) marko     (1000)     4113 2021-11-25 16:28:16.400735 rosbags-0.9.8/PKG-INFO
--rw-r--r--   0 marko     (1000) marko     (1000)     3021 2021-11-25 13:22:46.000000 rosbags-0.9.8/README.rst
--rw-r--r--   0 marko     (1000) marko     (1000)       98 2021-11-25 13:22:46.000000 rosbags-0.9.8/pyproject.toml
--rw-r--r--   0 marko     (1000) marko     (1000)     3555 2021-11-25 16:28:16.400735 rosbags-0.9.8/setup.cfg
--rw-r--r--   0 marko     (1000) marko     (1000)      164 2021-11-25 13:22:46.000000 rosbags-0.9.8/setup.py
-drwxr-xr-x   0 marko     (1000) marko     (1000)        0 2021-11-25 16:28:16.397401 rosbags-0.9.8/src/
-drwxr-xr-x   0 marko     (1000) marko     (1000)        0 2021-11-25 16:28:16.397401 rosbags-0.9.8/src/rosbags/
-drwxr-xr-x   0 marko     (1000) marko     (1000)        0 2021-11-25 16:28:16.400735 rosbags-0.9.8/src/rosbags/convert/
--rw-r--r--   0 marko     (1000) marko     (1000)      424 2021-11-25 13:22:46.000000 rosbags-0.9.8/src/rosbags/convert/__init__.py
--rw-r--r--   0 marko     (1000) marko     (1000)     1437 2021-11-25 16:27:04.000000 rosbags-0.9.8/src/rosbags/convert/__main__.py
--rw-r--r--   0 marko     (1000) marko     (1000)     2904 2021-11-25 13:22:46.000000 rosbags-0.9.8/src/rosbags/convert/converter.py
--rw-r--r--   0 marko     (1000) marko     (1000)        0 2021-11-25 13:22:46.000000 rosbags-0.9.8/src/rosbags/convert/py.typed
-drwxr-xr-x   0 marko     (1000) marko     (1000)        0 2021-11-25 16:28:16.400735 rosbags-0.9.8/src/rosbags/rosbag1/
--rw-r--r--   0 marko     (1000) marko     (1000)      415 2021-11-25 13:22:46.000000 rosbags-0.9.8/src/rosbags/rosbag1/__init__.py
--rw-r--r--   0 marko     (1000) marko     (1000)        0 2021-11-25 13:22:46.000000 rosbags-0.9.8/src/rosbags/rosbag1/py.typed
--rw-r--r--   0 marko     (1000) marko     (1000)    19165 2021-11-25 16:27:04.000000 rosbags-0.9.8/src/rosbags/rosbag1/reader.py
--rw-r--r--   0 marko     (1000) marko     (1000)    12166 2021-11-25 16:27:04.000000 rosbags-0.9.8/src/rosbags/rosbag1/writer.py
-drwxr-xr-x   0 marko     (1000) marko     (1000)        0 2021-11-25 16:28:16.400735 rosbags-0.9.8/src/rosbags/rosbag2/
--rw-r--r--   0 marko     (1000) marko     (1000)      377 2021-11-25 13:22:46.000000 rosbags-0.9.8/src/rosbags/rosbag2/__init__.py
--rw-r--r--   0 marko     (1000) marko     (1000)      434 2021-11-25 13:22:46.000000 rosbags-0.9.8/src/rosbags/rosbag2/connection.py
--rw-r--r--   0 marko     (1000) marko     (1000)        0 2021-11-25 13:22:46.000000 rosbags-0.9.8/src/rosbags/rosbag2/py.typed
--rw-r--r--   0 marko     (1000) marko     (1000)     9336 2021-11-25 16:27:04.000000 rosbags-0.9.8/src/rosbags/rosbag2/reader.py
--rw-r--r--   0 marko     (1000) marko     (1000)     8346 2021-11-25 16:27:04.000000 rosbags-0.9.8/src/rosbags/rosbag2/writer.py
-drwxr-xr-x   0 marko     (1000) marko     (1000)        0 2021-11-25 16:28:16.400735 rosbags-0.9.8/src/rosbags/serde/
--rw-r--r--   0 marko     (1000) marko     (1000)      562 2021-11-25 13:22:46.000000 rosbags-0.9.8/src/rosbags/serde/__init__.py
--rw-r--r--   0 marko     (1000) marko     (1000)    20029 2021-11-25 16:27:04.000000 rosbags-0.9.8/src/rosbags/serde/cdr.py
--rw-r--r--   0 marko     (1000) marko     (1000)     2469 2021-11-25 16:27:04.000000 rosbags-0.9.8/src/rosbags/serde/messages.py
--rw-r--r--   0 marko     (1000) marko     (1000)     2036 2021-11-25 13:22:46.000000 rosbags-0.9.8/src/rosbags/serde/primitives.py
--rw-r--r--   0 marko     (1000) marko     (1000)        0 2021-11-25 13:22:46.000000 rosbags-0.9.8/src/rosbags/serde/py.typed
--rw-r--r--   0 marko     (1000) marko     (1000)    13789 2021-11-25 16:27:04.000000 rosbags-0.9.8/src/rosbags/serde/ros1.py
--rw-r--r--   0 marko     (1000) marko     (1000)     3325 2021-11-25 13:22:46.000000 rosbags-0.9.8/src/rosbags/serde/serdes.py
--rw-r--r--   0 marko     (1000) marko     (1000)     1144 2021-11-25 16:27:04.000000 rosbags-0.9.8/src/rosbags/serde/typing.py
--rw-r--r--   0 marko     (1000) marko     (1000)     2193 2021-11-25 13:22:46.000000 rosbags-0.9.8/src/rosbags/serde/utils.py
-drwxr-xr-x   0 marko     (1000) marko     (1000)        0 2021-11-25 16:28:16.400735 rosbags-0.9.8/src/rosbags/typesys/
--rw-r--r--   0 marko     (1000) marko     (1000)      838 2021-11-25 13:22:46.000000 rosbags-0.9.8/src/rosbags/typesys/__init__.py
--rw-r--r--   0 marko     (1000) marko     (1000)     1480 2021-11-25 13:22:46.000000 rosbags-0.9.8/src/rosbags/typesys/__main__.py
--rw-r--r--   0 marko     (1000) marko     (1000)     1827 2021-11-25 16:27:04.000000 rosbags-0.9.8/src/rosbags/typesys/base.py
--rw-r--r--   0 marko     (1000) marko     (1000)    12454 2021-11-25 16:27:04.000000 rosbags-0.9.8/src/rosbags/typesys/idl.py
--rw-r--r--   0 marko     (1000) marko     (1000)    11432 2021-11-25 16:27:04.000000 rosbags-0.9.8/src/rosbags/typesys/msg.py
--rw-r--r--   0 marko     (1000) marko     (1000)     8042 2021-11-25 16:27:04.000000 rosbags-0.9.8/src/rosbags/typesys/peg.py
--rw-r--r--   0 marko     (1000) marko     (1000)        0 2021-11-25 13:22:46.000000 rosbags-0.9.8/src/rosbags/typesys/py.typed
--rw-r--r--   0 marko     (1000) marko     (1000)     5063 2021-11-25 16:27:04.000000 rosbags-0.9.8/src/rosbags/typesys/register.py
--rw-r--r--   0 marko     (1000) marko     (1000)    90402 2021-11-25 13:22:46.000000 rosbags-0.9.8/src/rosbags/typesys/types.py
-drwxr-xr-x   0 marko     (1000) marko     (1000)        0 2021-11-25 16:28:16.397401 rosbags-0.9.8/src/rosbags.egg-info/
--rw-r--r--   0 marko     (1000) marko     (1000)     4113 2021-11-25 16:28:16.000000 rosbags-0.9.8/src/rosbags.egg-info/PKG-INFO
--rw-r--r--   0 marko     (1000) marko     (1000)     1220 2021-11-25 16:28:16.000000 rosbags-0.9.8/src/rosbags.egg-info/SOURCES.txt
--rw-r--r--   0 marko     (1000) marko     (1000)        1 2021-11-25 16:28:16.000000 rosbags-0.9.8/src/rosbags.egg-info/dependency_links.txt
--rw-r--r--   0 marko     (1000) marko     (1000)       67 2021-11-25 16:28:16.000000 rosbags-0.9.8/src/rosbags.egg-info/entry_points.txt
--rw-r--r--   0 marko     (1000) marko     (1000)        1 2021-11-25 13:31:08.000000 rosbags-0.9.8/src/rosbags.egg-info/not-zip-safe
--rw-r--r--   0 marko     (1000) marko     (1000)      438 2021-11-25 16:28:16.000000 rosbags-0.9.8/src/rosbags.egg-info/requires.txt
--rw-r--r--   0 marko     (1000) marko     (1000)        8 2021-11-25 16:28:16.000000 rosbags-0.9.8/src/rosbags.egg-info/top_level.txt
+drwxr-xr-x   0 marko     (1000) marko     (1000)        0 2022-01-12 09:48:09.444481 rosbags-0.9.9/
+-rw-r--r--   0 marko     (1000) marko     (1000)    11358 2021-11-25 13:22:46.000000 rosbags-0.9.9/LICENSE.txt
+-rw-r--r--   0 marko     (1000) marko     (1000)     4283 2022-01-12 09:48:09.444481 rosbags-0.9.9/PKG-INFO
+-rw-r--r--   0 marko     (1000) marko     (1000)     3191 2022-01-12 09:45:08.000000 rosbags-0.9.9/README.rst
+-rw-r--r--   0 marko     (1000) marko     (1000)       98 2022-01-10 14:50:50.000000 rosbags-0.9.9/pyproject.toml
+-rw-r--r--   0 marko     (1000) marko     (1000)     3555 2022-01-12 09:48:09.444481 rosbags-0.9.9/setup.cfg
+-rw-r--r--   0 marko     (1000) marko     (1000)      164 2021-11-25 13:22:46.000000 rosbags-0.9.9/setup.py
+drwxr-xr-x   0 marko     (1000) marko     (1000)        0 2022-01-12 09:48:09.434481 rosbags-0.9.9/src/
+drwxr-xr-x   0 marko     (1000) marko     (1000)        0 2022-01-12 09:48:09.437814 rosbags-0.9.9/src/rosbags/
+drwxr-xr-x   0 marko     (1000) marko     (1000)        0 2022-01-12 09:48:09.441147 rosbags-0.9.9/src/rosbags/convert/
+-rw-r--r--   0 marko     (1000) marko     (1000)      424 2021-11-25 13:22:46.000000 rosbags-0.9.9/src/rosbags/convert/__init__.py
+-rw-r--r--   0 marko     (1000) marko     (1000)     1663 2022-01-12 09:45:08.000000 rosbags-0.9.9/src/rosbags/convert/__main__.py
+-rw-r--r--   0 marko     (1000) marko     (1000)     5064 2022-01-12 09:45:08.000000 rosbags-0.9.9/src/rosbags/convert/converter.py
+-rw-r--r--   0 marko     (1000) marko     (1000)        0 2021-11-25 13:22:46.000000 rosbags-0.9.9/src/rosbags/convert/py.typed
+drwxr-xr-x   0 marko     (1000) marko     (1000)        0 2022-01-12 09:48:09.444481 rosbags-0.9.9/src/rosbags/rosbag1/
+-rw-r--r--   0 marko     (1000) marko     (1000)      415 2021-11-25 13:22:46.000000 rosbags-0.9.9/src/rosbags/rosbag1/__init__.py
+-rw-r--r--   0 marko     (1000) marko     (1000)        0 2021-11-25 13:22:46.000000 rosbags-0.9.9/src/rosbags/rosbag1/py.typed
+-rw-r--r--   0 marko     (1000) marko     (1000)    19165 2022-01-11 15:56:37.000000 rosbags-0.9.9/src/rosbags/rosbag1/reader.py
+-rw-r--r--   0 marko     (1000) marko     (1000)    12166 2021-11-25 16:31:30.000000 rosbags-0.9.9/src/rosbags/rosbag1/writer.py
+drwxr-xr-x   0 marko     (1000) marko     (1000)        0 2022-01-12 09:48:09.444481 rosbags-0.9.9/src/rosbags/rosbag2/
+-rw-r--r--   0 marko     (1000) marko     (1000)      377 2021-11-25 13:22:46.000000 rosbags-0.9.9/src/rosbags/rosbag2/__init__.py
+-rw-r--r--   0 marko     (1000) marko     (1000)      434 2021-11-25 13:22:46.000000 rosbags-0.9.9/src/rosbags/rosbag2/connection.py
+-rw-r--r--   0 marko     (1000) marko     (1000)        0 2021-11-25 13:22:46.000000 rosbags-0.9.9/src/rosbags/rosbag2/py.typed
+-rw-r--r--   0 marko     (1000) marko     (1000)     9336 2021-11-25 16:31:30.000000 rosbags-0.9.9/src/rosbags/rosbag2/reader.py
+-rw-r--r--   0 marko     (1000) marko     (1000)     8346 2021-11-25 16:31:30.000000 rosbags-0.9.9/src/rosbags/rosbag2/writer.py
+drwxr-xr-x   0 marko     (1000) marko     (1000)        0 2022-01-12 09:48:09.444481 rosbags-0.9.9/src/rosbags/serde/
+-rw-r--r--   0 marko     (1000) marko     (1000)      562 2021-11-25 13:22:46.000000 rosbags-0.9.9/src/rosbags/serde/__init__.py
+-rw-r--r--   0 marko     (1000) marko     (1000)    20209 2022-01-12 09:45:08.000000 rosbags-0.9.9/src/rosbags/serde/cdr.py
+-rw-r--r--   0 marko     (1000) marko     (1000)     2469 2021-11-25 16:31:30.000000 rosbags-0.9.9/src/rosbags/serde/messages.py
+-rw-r--r--   0 marko     (1000) marko     (1000)     2036 2021-11-25 13:22:46.000000 rosbags-0.9.9/src/rosbags/serde/primitives.py
+-rw-r--r--   0 marko     (1000) marko     (1000)        0 2021-11-25 13:22:46.000000 rosbags-0.9.9/src/rosbags/serde/py.typed
+-rw-r--r--   0 marko     (1000) marko     (1000)    13895 2022-01-12 09:45:08.000000 rosbags-0.9.9/src/rosbags/serde/ros1.py
+-rw-r--r--   0 marko     (1000) marko     (1000)     3333 2022-01-12 09:45:08.000000 rosbags-0.9.9/src/rosbags/serde/serdes.py
+-rw-r--r--   0 marko     (1000) marko     (1000)     1144 2021-11-25 16:31:30.000000 rosbags-0.9.9/src/rosbags/serde/typing.py
+-rw-r--r--   0 marko     (1000) marko     (1000)     2193 2021-11-25 13:22:46.000000 rosbags-0.9.9/src/rosbags/serde/utils.py
+drwxr-xr-x   0 marko     (1000) marko     (1000)        0 2022-01-12 09:48:09.444481 rosbags-0.9.9/src/rosbags/typesys/
+-rw-r--r--   0 marko     (1000) marko     (1000)      838 2021-11-25 13:22:46.000000 rosbags-0.9.9/src/rosbags/typesys/__init__.py
+-rw-r--r--   0 marko     (1000) marko     (1000)     1480 2021-11-25 13:22:46.000000 rosbags-0.9.9/src/rosbags/typesys/__main__.py
+-rw-r--r--   0 marko     (1000) marko     (1000)     1827 2021-11-25 16:31:30.000000 rosbags-0.9.9/src/rosbags/typesys/base.py
+-rw-r--r--   0 marko     (1000) marko     (1000)    12454 2021-11-25 16:31:30.000000 rosbags-0.9.9/src/rosbags/typesys/idl.py
+-rw-r--r--   0 marko     (1000) marko     (1000)    11432 2021-11-25 16:31:30.000000 rosbags-0.9.9/src/rosbags/typesys/msg.py
+-rw-r--r--   0 marko     (1000) marko     (1000)     8042 2021-11-25 16:31:30.000000 rosbags-0.9.9/src/rosbags/typesys/peg.py
+-rw-r--r--   0 marko     (1000) marko     (1000)        0 2021-11-25 13:22:46.000000 rosbags-0.9.9/src/rosbags/typesys/py.typed
+-rw-r--r--   0 marko     (1000) marko     (1000)     5063 2021-11-25 16:31:30.000000 rosbags-0.9.9/src/rosbags/typesys/register.py
+-rw-r--r--   0 marko     (1000) marko     (1000)    90402 2021-11-25 16:58:02.000000 rosbags-0.9.9/src/rosbags/typesys/types.py
+drwxr-xr-x   0 marko     (1000) marko     (1000)        0 2022-01-12 09:48:09.441147 rosbags-0.9.9/src/rosbags.egg-info/
+-rw-r--r--   0 marko     (1000) marko     (1000)     4283 2022-01-12 09:48:09.000000 rosbags-0.9.9/src/rosbags.egg-info/PKG-INFO
+-rw-r--r--   0 marko     (1000) marko     (1000)     1220 2022-01-12 09:48:09.000000 rosbags-0.9.9/src/rosbags.egg-info/SOURCES.txt
+-rw-r--r--   0 marko     (1000) marko     (1000)        1 2022-01-12 09:48:09.000000 rosbags-0.9.9/src/rosbags.egg-info/dependency_links.txt
+-rw-r--r--   0 marko     (1000) marko     (1000)       67 2022-01-12 09:48:09.000000 rosbags-0.9.9/src/rosbags.egg-info/entry_points.txt
+-rw-r--r--   0 marko     (1000) marko     (1000)        1 2021-11-25 13:31:08.000000 rosbags-0.9.9/src/rosbags.egg-info/not-zip-safe
+-rw-r--r--   0 marko     (1000) marko     (1000)      438 2022-01-12 09:48:09.000000 rosbags-0.9.9/src/rosbags.egg-info/requires.txt
+-rw-r--r--   0 marko     (1000) marko     (1000)        8 2022-01-12 09:48:09.000000 rosbags-0.9.9/src/rosbags.egg-info/top_level.txt
```

### Comparing `rosbags-0.9.8/LICENSE.txt` & `rosbags-0.9.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rosbags-0.9.8/PKG-INFO` & `rosbags-0.9.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosbags
-Version: 0.9.8
+Version: 0.9.9
 Summary: Pure Python library to read, modify, convert, and write rosbag files.
 Home-page: https://gitlab.com/ternaris/rosbags
 Author: Ternaris
 Author-email: team@ternaris.com
 License: Apache 2.0
 Project-URL: Code, https://gitlab.com/ternaris/rosbags
 Project-URL: Documentation, https://ternaris.gitlab.io/rosbags
@@ -69,22 +69,28 @@
    # create reader instance and open for reading
    with Reader('/home/ros/rosbag_2020_03_24') as reader:
        for connection, timestamp, rawdata in reader.messages(['/imu_raw/Imu']):
             msg = deserialize_cdr(rawdata, connection.msgtype)
             print(msg.header.frame_id)
 
 
-Convert rosbag1 to rosbag2::
+Convert between rosbag versions::
 
    # Convert "foo.bag", result will be "foo/"
    rosbags-convert foo.bag
 
+   # Convert "bar", result will be "bar.bag"
+   rosbags-convert bar
+
    # Convert "foo.bag", save the result as "bar"
    rosbags-convert foo.bag --dst /path/to/bar
 
+   # Convert "bar", save the result as "foo.bag"
+   rosbags-convert bar --dst /path/to/foo.bag
+
 
 Documentation
 =============
 
 Read the `documentation <https://ternaris.gitlab.io/rosbags/>`_ for further information.
 
 .. end documentation
```

### Comparing `rosbags-0.9.8/README.rst` & `rosbags-0.9.9/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -42,22 +42,28 @@
    # create reader instance and open for reading
    with Reader('/home/ros/rosbag_2020_03_24') as reader:
        for connection, timestamp, rawdata in reader.messages(['/imu_raw/Imu']):
             msg = deserialize_cdr(rawdata, connection.msgtype)
             print(msg.header.frame_id)
 
 
-Convert rosbag1 to rosbag2::
+Convert between rosbag versions::
 
    # Convert "foo.bag", result will be "foo/"
    rosbags-convert foo.bag
 
+   # Convert "bar", result will be "bar.bag"
+   rosbags-convert bar
+
    # Convert "foo.bag", save the result as "bar"
    rosbags-convert foo.bag --dst /path/to/bar
 
+   # Convert "bar", save the result as "foo.bag"
+   rosbags-convert bar --dst /path/to/foo.bag
+
 
 Documentation
 =============
 
 Read the `documentation <https://ternaris.gitlab.io/rosbags/>`_ for further information.
 
 .. end documentation
```

### Comparing `rosbags-0.9.8/setup.cfg` & `rosbags-0.9.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rosbags
-version = 0.9.8
+version = 0.9.9
 author = Ternaris
 author_email = team@ternaris.com
 home_page = https://gitlab.com/ternaris/rosbags
 description = Pure Python library to read, modify, convert, and write rosbag files.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 keywords =
```

### Comparing `rosbags-0.9.8/src/rosbags/convert/__main__.py` & `rosbags-0.9.9/src/rosbags/convert/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,26 +35,31 @@
         return path
 
     return topath
 
 
 def main() -> None:
     """Parse cli arguments and run conversion."""
-    parser = argparse.ArgumentParser(description='Convert rosbag1 to rosbag2.')
+    parser = argparse.ArgumentParser(description='Convert between rosbag1 and rosbag2.')
     parser.add_argument(
         'src',
         type=pathtype(),
-        help='source path to read rosbag1 from',
+        help='source path to read rosbag1 or rosbag2 from',
     )
     parser.add_argument(
         '--dst',
         type=pathtype(exists=False),
-        help='destination path for rosbag2',
+        help='destination path for converted rosbag',
     )
+
     args = parser.parse_args()
+    if args.dst is not None and (args.src.suffix == '.bag') == (args.dst.suffix == '.bag'):
+        print('Source and destination rosbag versions must differ.')  # noqa: T001
+        sys.exit(1)
+
     try:
         convert(args.src, args.dst)
     except ConverterError as err:
         print(f'ERROR: {err}')  # noqa: T001
         sys.exit(1)
```

### Comparing `rosbags-0.9.8/src/rosbags/convert/converter.py` & `rosbags-0.9.9/src/rosbags/convert/converter.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,26 +3,32 @@
 """Rosbag1 to Rosbag2 Converter."""
 
 from __future__ import annotations
 
 from dataclasses import asdict
 from typing import TYPE_CHECKING
 
-from rosbags.rosbag1 import Reader, ReaderError
-from rosbags.rosbag2 import Writer, WriterError
-from rosbags.rosbag2.connection import Connection as WConnection
-from rosbags.serde import ros1_to_cdr
+from rosbags.rosbag1 import Reader as Reader1
+from rosbags.rosbag1 import ReaderError as ReaderError1
+from rosbags.rosbag1 import Writer as Writer1
+from rosbags.rosbag1 import WriterError as WriterError1
+from rosbags.rosbag1.reader import Connection as Connection1
+from rosbags.rosbag2 import Reader as Reader2
+from rosbags.rosbag2 import ReaderError as ReaderError2
+from rosbags.rosbag2 import Writer as Writer2
+from rosbags.rosbag2 import WriterError as WriterError2
+from rosbags.rosbag2.connection import Connection as Connection2
+from rosbags.serde import cdr_to_ros1, ros1_to_cdr
 from rosbags.typesys import get_types_from_msg, register_types
+from rosbags.typesys.msg import generate_msgdef
 
 if TYPE_CHECKING:
     from pathlib import Path
     from typing import Any, Optional
 
-    from rosbags.rosbag1.reader import Connection as RConnection
-
 LATCH = """
 - history: 3
   depth: 0
   reliability: 1
   durability: 1
   deadline:
     sec: 2147483647
@@ -38,65 +44,132 @@
 """.strip()
 
 
 class ConverterError(Exception):
     """Converter Error."""
 
 
-def convert_connection(rconn: RConnection) -> WConnection:
+def upgrade_connection(rconn: Connection1) -> Connection2:
     """Convert rosbag1 connection to rosbag2 connection.
 
     Args:
         rconn: Rosbag1 connection.
 
     Returns:
         Rosbag2 connection.
 
     """
-    return WConnection(
+    return Connection2(
         -1,
         0,
         rconn.topic,
         rconn.msgtype,
         'cdr',
         LATCH if rconn.latching else '',
     )
 
 
-def convert(src: Path, dst: Optional[Path]) -> None:
+def downgrade_connection(rconn: Connection2) -> Connection1:
+    """Convert rosbag2 connection to rosbag1 connection.
+
+    Args:
+        rconn: Rosbag2 connection.
+
+    Returns:
+        Rosbag1 connection.
+
+    """
+    msgdef, md5sum = generate_msgdef(rconn.msgtype)
+    return Connection1(
+        -1,
+        rconn.topic,
+        rconn.msgtype,
+        msgdef,
+        md5sum,
+        None,
+        int('durability: 1' in rconn.offered_qos_profiles),
+        [],
+    )
+
+
+def convert_1to2(src: Path, dst: Path) -> None:
     """Convert Rosbag1 to Rosbag2.
 
     Args:
         src: Rosbag1 path.
         dst: Rosbag2 path.
 
+    """
+    with Reader1(src) as reader, Writer2(dst) as writer:
+        typs: dict[str, Any] = {}
+        connmap: dict[int, Connection2] = {}
+
+        for rconn in reader.connections.values():
+            candidate = upgrade_connection(rconn)
+            existing = next((x for x in writer.connections.values() if x == candidate), None)
+            wconn = existing if existing else writer.add_connection(**asdict(candidate))
+            connmap[rconn.cid] = wconn
+            typs.update(get_types_from_msg(rconn.msgdef, rconn.msgtype))
+        register_types(typs)
+
+        for rconn, timestamp, data in reader.messages():
+            data = ros1_to_cdr(data, rconn.msgtype)
+            writer.write(connmap[rconn.cid], timestamp, data)
+
+
+def convert_2to1(src: Path, dst: Path) -> None:
+    """Convert Rosbag2 to Rosbag1.
+
+    Args:
+        src: Rosbag2 path.
+        dst: Rosbag1 path.
+
+    """
+    with Reader2(src) as reader, Writer1(dst) as writer:
+        connmap: dict[int, Connection1] = {}
+        for rconn in reader.connections.values():
+            candidate = downgrade_connection(rconn)
+            # yapf: disable
+            existing = next(
+                (
+                    x
+                    for x in writer.connections.values()
+                    if x.topic == candidate.topic
+                    if x.md5sum == candidate.md5sum
+                    if x.latching == candidate.latching
+                ),
+                None,
+            )
+            # yapf: enable
+            connmap[rconn.id] = existing if existing else writer.add_connection(*candidate[1:-1])
+
+        for rconn, timestamp, data in reader.messages():
+            data = cdr_to_ros1(data, rconn.msgtype)
+            writer.write(connmap[rconn.id], timestamp, data)
+
+
+def convert(src: Path, dst: Optional[Path]) -> None:
+    """Convert between Rosbag1 and Rosbag2.
+
+    Args:
+        src: Source rosbag.
+        dst: Destination rosbag.
+
     Raises:
         ConverterError: An error occured during reading, writing, or
             converting.
 
     """
-    dst = dst if dst else src.with_suffix('')
+    upgrade = src.suffix == '.bag'
+    dst = dst if dst else src.with_suffix('' if upgrade else '.bag')
     if dst.exists():
         raise ConverterError(f'Output path {str(dst)!r} exists already.')
+    func = convert_1to2 if upgrade else convert_2to1
 
     try:
-        with Reader(src) as reader, Writer(dst) as writer:
-            typs: dict[str, Any] = {}
-            connmap: dict[int, WConnection] = {}
-
-            for rconn in reader.connections.values():
-                candidate = convert_connection(rconn)
-                existing = next((x for x in writer.connections.values() if x == candidate), None)
-                wconn = existing if existing else writer.add_connection(**asdict(candidate))
-                connmap[rconn.cid] = wconn
-                typs.update(get_types_from_msg(rconn.msgdef, rconn.msgtype))
-            register_types(typs)
-
-            for rconn, timestamp, data in reader.messages():
-                data = ros1_to_cdr(data, rconn.msgtype)
-                writer.write(connmap[rconn.cid], timestamp, data)
-    except ReaderError as err:
+        func(src, dst)
+    except (ReaderError1, ReaderError2) as err:
         raise ConverterError(f'Reading source bag: {err}') from err
-    except WriterError as err:
+    except (WriterError1, WriterError2) as err:
         raise ConverterError(f'Writing destination bag: {err}') from err
     except Exception as err:  # pylint: disable=broad-except
         raise ConverterError(f'Converting rosbag: {err!r}') from err
```

### Comparing `rosbags-0.9.8/src/rosbags/rosbag1/reader.py` & `rosbags-0.9.9/src/rosbags/rosbag1/reader.py`

 * *Files identical despite different names*

### Comparing `rosbags-0.9.8/src/rosbags/rosbag1/writer.py` & `rosbags-0.9.9/src/rosbags/rosbag1/writer.py`

 * *Files identical despite different names*

### Comparing `rosbags-0.9.8/src/rosbags/rosbag2/reader.py` & `rosbags-0.9.9/src/rosbags/rosbag2/reader.py`

 * *Files identical despite different names*

### Comparing `rosbags-0.9.8/src/rosbags/rosbag2/writer.py` & `rosbags-0.9.9/src/rosbags/rosbag2/writer.py`

 * *Files identical despite different names*

### Comparing `rosbags-0.9.8/src/rosbags/serde/__init__.py` & `rosbags-0.9.9/src/rosbags/serde/__init__.py`

 * *Files identical despite different names*

### Comparing `rosbags-0.9.8/src/rosbags/serde/cdr.py` & `rosbags-0.9.9/src/rosbags/serde/cdr.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,16 @@
                     lines.append(f'  for val in message.{fieldname}:')
                     lines.append('    pos = (pos + 4 - 1) & -4')
                     lines.append('    pos += 4 + len(val.encode()) + 1')
                     aligned = 1
                 else:
                     anext = align(subdesc)
                     if aligned < anext:
-                        lines.append(f'  pos = (pos + {anext} - 1) & -{anext}')
+                        lines.append(f'  if len(message.{fieldname}):')
+                        lines.append(f'    pos = (pos + {anext} - 1) & -{anext}')
                         aligned = anext
                     lines.append(f'  pos += len(message.{fieldname}) * {SIZEMAP[subdesc.args]}')
 
             else:
                 assert subdesc.valtype == Valtype.MESSAGE
                 anext = align(subdesc)
                 anext_after = align_after(subdesc)
@@ -268,15 +269,16 @@
                     lines.append('    pos += length')
                     aligned = 1
                 else:
                     lines.append(f'  size = len(val) * {SIZEMAP[subdesc.args]}')
                     if (endianess == 'le') != (sys.byteorder == 'little'):
                         lines.append('  val = val.byteswap()')
                     if aligned < (anext := align(subdesc)):
-                        lines.append(f'  pos = (pos + {anext} - 1) & -{anext}')
+                        lines.append('  if size:')
+                        lines.append(f'    pos = (pos + {anext} - 1) & -{anext}')
                     lines.append('  rawdata[pos:pos + size] = val.view(numpy.uint8)')
                     lines.append('  pos += size')
                     aligned = anext
 
             if subdesc.valtype == Valtype.MESSAGE:
                 anext = align(subdesc)
                 lines.append(
@@ -413,15 +415,16 @@
                     )
                     lines.append('    pos += 4 + length')
                     lines.append('  values.append(value)')
                     aligned = 1
                 else:
                     lines.append(f'  length = size * {SIZEMAP[subdesc.args]}')
                     if aligned < (anext := align(subdesc)):
-                        lines.append(f'  pos = (pos + {anext} - 1) & -{anext}')
+                        lines.append('  if size:')
+                        lines.append(f'    pos = (pos + {anext} - 1) & -{anext}')
                     lines.append(
                         f'  val = numpy.frombuffer(rawdata, '
                         f'dtype=numpy.{subdesc.args}, count=size, offset=pos)',
                     )
                     if (endianess == 'le') != (sys.byteorder == 'little'):
                         lines.append('  val = val.byteswap()')
                     lines.append('  values.append(val)')
```

### Comparing `rosbags-0.9.8/src/rosbags/serde/messages.py` & `rosbags-0.9.9/src/rosbags/serde/messages.py`

 * *Files identical despite different names*

### Comparing `rosbags-0.9.8/src/rosbags/serde/primitives.py` & `rosbags-0.9.9/src/rosbags/serde/primitives.py`

 * *Files identical despite different names*

### Comparing `rosbags-0.9.8/src/rosbags/serde/ros1.py` & `rosbags-0.9.9/src/rosbags/serde/ros1.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,16 @@
                             '    output[opos:opos + length - 1] = input[ipos:ipos + length - 1]',
                         )
                     lines.append('    ipos += length - 1')
                     lines.append('    opos += length')
                     aligned = 1
                 else:
                     if aligned < (anext := align(subdesc)):
-                        lines.append(f'  opos = (opos + {anext} - 1) & -{anext}')
+                        lines.append('  if size:')
+                        lines.append(f'    opos = (opos + {anext} - 1) & -{anext}')
                     lines.append(f'  length = size * {SIZEMAP[subdesc.args]}')
                     if copy:
                         lines.append('  output[opos:opos + length] = input[ipos:ipos + length]')
                     lines.append('  ipos += length')
                     lines.append('  opos += length')
                     aligned = anext
 
@@ -300,15 +301,16 @@
                     if copy:
                         lines.append('    output[opos:opos + length] = input[ipos:ipos + length]')
                     lines.append('    ipos += length + 1')
                     lines.append('    opos += length')
                     aligned = 1
                 else:
                     if aligned < (anext := align(subdesc)):
-                        lines.append(f'  ipos = (ipos + {anext} - 1) & -{anext}')
+                        lines.append('  if size:')
+                        lines.append(f'    ipos = (ipos + {anext} - 1) & -{anext}')
                     lines.append(f'  length = size * {SIZEMAP[subdesc.args]}')
                     if copy:
                         lines.append('  output[opos:opos + length] = input[ipos:ipos + length]')
                     lines.append('  ipos += length')
                     lines.append('  opos += length')
                     aligned = anext
```

### Comparing `rosbags-0.9.8/src/rosbags/serde/serdes.py` & `rosbags-0.9.9/src/rosbags/serde/serdes.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,22 +122,22 @@
 
     ipos, opos = msgdef.getsize_cdr_to_ros1(
         raw[4:],
         0,
         None,
         0,
     )
-    assert ipos + 4 == len(raw)
+    assert ipos + 4 + 3 >= len(raw)
 
     raw = memoryview(raw)
     size = opos
     rawdata = memoryview(bytearray(size))
 
     ipos, opos = msgdef.cdr_to_ros1(
         raw[4:],
         0,
         rawdata,
         0,
     )
-    assert ipos + 4 == len(raw)
+    assert ipos + 4 + 3 >= len(raw)
     assert opos == size
     return rawdata.toreadonly()
```

### Comparing `rosbags-0.9.8/src/rosbags/serde/typing.py` & `rosbags-0.9.9/src/rosbags/serde/typing.py`

 * *Files identical despite different names*

### Comparing `rosbags-0.9.8/src/rosbags/serde/utils.py` & `rosbags-0.9.9/src/rosbags/serde/utils.py`

 * *Files identical despite different names*

### Comparing `rosbags-0.9.8/src/rosbags/typesys/__init__.py` & `rosbags-0.9.9/src/rosbags/typesys/__init__.py`

 * *Files identical despite different names*

### Comparing `rosbags-0.9.8/src/rosbags/typesys/__main__.py` & `rosbags-0.9.9/src/rosbags/typesys/__main__.py`

 * *Files identical despite different names*

### Comparing `rosbags-0.9.8/src/rosbags/typesys/base.py` & `rosbags-0.9.9/src/rosbags/typesys/base.py`

 * *Files identical despite different names*

### Comparing `rosbags-0.9.8/src/rosbags/typesys/idl.py` & `rosbags-0.9.9/src/rosbags/typesys/idl.py`

 * *Files identical despite different names*

### Comparing `rosbags-0.9.8/src/rosbags/typesys/msg.py` & `rosbags-0.9.9/src/rosbags/typesys/msg.py`

 * *Files identical despite different names*

### Comparing `rosbags-0.9.8/src/rosbags/typesys/peg.py` & `rosbags-0.9.9/src/rosbags/typesys/peg.py`

 * *Files identical despite different names*

### Comparing `rosbags-0.9.8/src/rosbags/typesys/register.py` & `rosbags-0.9.9/src/rosbags/typesys/register.py`

 * *Files identical despite different names*

### Comparing `rosbags-0.9.8/src/rosbags/typesys/types.py` & `rosbags-0.9.9/src/rosbags/typesys/types.py`

 * *Files identical despite different names*

### Comparing `rosbags-0.9.8/src/rosbags.egg-info/PKG-INFO` & `rosbags-0.9.9/src/rosbags.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosbags
-Version: 0.9.8
+Version: 0.9.9
 Summary: Pure Python library to read, modify, convert, and write rosbag files.
 Home-page: https://gitlab.com/ternaris/rosbags
 Author: Ternaris
 Author-email: team@ternaris.com
 License: Apache 2.0
 Project-URL: Code, https://gitlab.com/ternaris/rosbags
 Project-URL: Documentation, https://ternaris.gitlab.io/rosbags
@@ -69,22 +69,28 @@
    # create reader instance and open for reading
    with Reader('/home/ros/rosbag_2020_03_24') as reader:
        for connection, timestamp, rawdata in reader.messages(['/imu_raw/Imu']):
             msg = deserialize_cdr(rawdata, connection.msgtype)
             print(msg.header.frame_id)
 
 
-Convert rosbag1 to rosbag2::
+Convert between rosbag versions::
 
    # Convert "foo.bag", result will be "foo/"
    rosbags-convert foo.bag
 
+   # Convert "bar", result will be "bar.bag"
+   rosbags-convert bar
+
    # Convert "foo.bag", save the result as "bar"
    rosbags-convert foo.bag --dst /path/to/bar
 
+   # Convert "bar", save the result as "foo.bag"
+   rosbags-convert bar --dst /path/to/foo.bag
+
 
 Documentation
 =============
 
 Read the `documentation <https://ternaris.gitlab.io/rosbags/>`_ for further information.
 
 .. end documentation
```

### Comparing `rosbags-0.9.8/src/rosbags.egg-info/SOURCES.txt` & `rosbags-0.9.9/src/rosbags.egg-info/SOURCES.txt`

 * *Files identical despite different names*

