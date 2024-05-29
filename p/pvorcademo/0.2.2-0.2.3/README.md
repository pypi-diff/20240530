# Comparing `tmp/pvorcademo-0.2.2.tar.gz` & `tmp/pvorcademo-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvorcademo-0.2.2.tar", last modified: Fri May 24 21:28:29 2024, max compression
+gzip compressed data, was "pvorcademo-0.2.3.tar", last modified: Wed May 29 23:38:36 2024, max compression
```

## Comparing `pvorcademo-0.2.2.tar` & `pvorcademo-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 srinivasa  (1000) srinivasa  (1000)        0 2024-05-24 21:28:29.786069 pvorcademo-0.2.2/
--rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)      101 2024-05-24 21:28:29.000000 pvorcademo-0.2.2/MANIFEST.in
--rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)     3069 2024-05-24 21:28:29.786069 pvorcademo-0.2.2/PKG-INFO
--rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)     2377 2024-05-13 16:44:36.000000 pvorcademo-0.2.2/README.md
-drwxrwxr-x   0 srinivasa  (1000) srinivasa  (1000)        0 2024-05-24 21:28:29.782070 pvorcademo-0.2.2/pvorcademo/
--rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)    11344 2024-05-24 21:28:29.000000 pvorcademo-0.2.2/pvorcademo/LICENSE
--rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)     2822 2024-05-24 21:28:29.000000 pvorcademo-0.2.2/pvorcademo/orca_demo.py
--rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)    13421 2024-05-24 21:28:29.000000 pvorcademo-0.2.2/pvorcademo/orca_demo_streaming.py
-drwxrwxr-x   0 srinivasa  (1000) srinivasa  (1000)        0 2024-05-24 21:28:29.786069 pvorcademo-0.2.2/pvorcademo.egg-info/
--rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)     3069 2024-05-24 21:28:29.000000 pvorcademo-0.2.2/pvorcademo.egg-info/PKG-INFO
--rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)      313 2024-05-24 21:28:29.000000 pvorcademo-0.2.2/pvorcademo.egg-info/SOURCES.txt
--rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)        1 2024-05-24 21:28:29.000000 pvorcademo-0.2.2/pvorcademo.egg-info/dependency_links.txt
--rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)      115 2024-05-24 21:28:29.000000 pvorcademo-0.2.2/pvorcademo.egg-info/entry_points.txt
--rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)       63 2024-05-24 21:28:29.000000 pvorcademo-0.2.2/pvorcademo.egg-info/requires.txt
--rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)       11 2024-05-24 21:28:29.000000 pvorcademo-0.2.2/pvorcademo.egg-info/top_level.txt
--rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)       38 2024-05-24 21:28:29.786069 pvorcademo-0.2.2/setup.cfg
--rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)     1794 2024-05-24 21:28:24.000000 pvorcademo-0.2.2/setup.py
+drwxrwxr-x   0 srinivasa  (1000) srinivasa  (1000)        0 2024-05-29 23:38:36.050804 pvorcademo-0.2.3/
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)      101 2024-05-29 23:38:36.000000 pvorcademo-0.2.3/MANIFEST.in
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)     3069 2024-05-29 23:38:36.050804 pvorcademo-0.2.3/PKG-INFO
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)     2377 2024-05-13 16:44:36.000000 pvorcademo-0.2.3/README.md
+drwxrwxr-x   0 srinivasa  (1000) srinivasa  (1000)        0 2024-05-29 23:38:36.050804 pvorcademo-0.2.3/pvorcademo/
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)    11344 2024-05-29 23:38:36.000000 pvorcademo-0.2.3/pvorcademo/LICENSE
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)     2822 2024-05-29 23:38:36.000000 pvorcademo-0.2.3/pvorcademo/orca_demo.py
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)    13421 2024-05-29 23:38:36.000000 pvorcademo-0.2.3/pvorcademo/orca_demo_streaming.py
+drwxrwxr-x   0 srinivasa  (1000) srinivasa  (1000)        0 2024-05-29 23:38:36.050804 pvorcademo-0.2.3/pvorcademo.egg-info/
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)     3069 2024-05-29 23:38:36.000000 pvorcademo-0.2.3/pvorcademo.egg-info/PKG-INFO
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)      313 2024-05-29 23:38:36.000000 pvorcademo-0.2.3/pvorcademo.egg-info/SOURCES.txt
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)        1 2024-05-29 23:38:36.000000 pvorcademo-0.2.3/pvorcademo.egg-info/dependency_links.txt
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)      115 2024-05-29 23:38:36.000000 pvorcademo-0.2.3/pvorcademo.egg-info/entry_points.txt
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)       63 2024-05-29 23:38:36.000000 pvorcademo-0.2.3/pvorcademo.egg-info/requires.txt
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)       11 2024-05-29 23:38:36.000000 pvorcademo-0.2.3/pvorcademo.egg-info/top_level.txt
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)       38 2024-05-29 23:38:36.050804 pvorcademo-0.2.3/setup.cfg
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)     1794 2024-05-29 23:38:15.000000 pvorcademo-0.2.3/setup.py
```

### Comparing `pvorcademo-0.2.2/PKG-INFO` & `pvorcademo-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvorcademo
-Version: 0.2.2
+Version: 0.2.3
 Summary: Orca Streaming Text-to-Speech Engine demos
 Home-page: https://github.com/Picovoice/orca
 Author: Picovoice
 Author-email: hello@picovoice.ai
 License: UNKNOWN
 Keywords: Streaming Text-to-Speech,TTS,Speech Synthesis,Voice Generation,Speech Engine
 Platform: UNKNOWN
```

### Comparing `pvorcademo-0.2.2/README.md` & `pvorcademo-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pvorcademo-0.2.2/pvorcademo/LICENSE` & `pvorcademo-0.2.3/pvorcademo/LICENSE`

 * *Files identical despite different names*

### Comparing `pvorcademo-0.2.2/pvorcademo/orca_demo.py` & `pvorcademo-0.2.3/pvorcademo/orca_demo.py`

 * *Files identical despite different names*

### Comparing `pvorcademo-0.2.2/pvorcademo/orca_demo_streaming.py` & `pvorcademo-0.2.3/pvorcademo/orca_demo_streaming.py`

 * *Files identical despite different names*

### Comparing `pvorcademo-0.2.2/pvorcademo.egg-info/PKG-INFO` & `pvorcademo-0.2.3/pvorcademo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvorcademo
-Version: 0.2.2
+Version: 0.2.3
 Summary: Orca Streaming Text-to-Speech Engine demos
 Home-page: https://github.com/Picovoice/orca
 Author: Picovoice
 Author-email: hello@picovoice.ai
 License: UNKNOWN
 Keywords: Streaming Text-to-Speech,TTS,Speech Synthesis,Voice Generation,Speech Engine
 Platform: UNKNOWN
```

### Comparing `pvorcademo-0.2.2/setup.py` & `pvorcademo-0.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,23 +22,23 @@
     f.write(manifest_in)
 
 with open(os.path.join(os.path.dirname(__file__), "README.md"), "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="pvorcademo",
-    version="0.2.2",
+    version="0.2.3",
     author="Picovoice",
     author_email="hello@picovoice.ai",
     description="Orca Streaming Text-to-Speech Engine demos",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Picovoice/orca",
     packages=["pvorcademo"],
-    install_requires=["numpy>=1.24.0", "pvorca==0.2.2", "sounddevice==0.4.6", "tiktoken==0.6.0"],
+    install_requires=["numpy>=1.24.0", "pvorca==0.2.3", "sounddevice==0.4.6", "tiktoken==0.6.0"],
     include_package_data=True,
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
```

