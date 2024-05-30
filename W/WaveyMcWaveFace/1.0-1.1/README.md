# Comparing `tmp/WaveyMcWaveFace-1.0.tar.gz` & `tmp/waveymcwaveface-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WaveyMcWaveFace-1.0.tar", last modified: Tue May 28 20:58:36 2024, max compression
+gzip compressed data, was "waveymcwaveface-1.1.tar", last modified: Thu May 30 14:46:29 2024, max compression
```

## Comparing `WaveyMcWaveFace-1.0.tar` & `waveymcwaveface-1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-28 20:58:36.803419 WaveyMcWaveFace-1.0/
--rw-rw-r--   0 user      (1000) user      (1000)     1029 2024-05-28 20:58:36.803419 WaveyMcWaveFace-1.0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      549 2024-05-28 16:47:58.000000 WaveyMcWaveFace-1.0/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-28 20:58:36.802419 WaveyMcWaveFace-1.0/TiDE/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-28 20:58:36.803419 WaveyMcWaveFace-1.0/TiDE/WaveyMcWaveFace.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     1029 2024-05-28 20:58:36.000000 WaveyMcWaveFace-1.0/TiDE/WaveyMcWaveFace.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      302 2024-05-28 20:58:36.000000 WaveyMcWaveFace-1.0/TiDE/WaveyMcWaveFace.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-05-28 20:58:36.000000 WaveyMcWaveFace-1.0/TiDE/WaveyMcWaveFace.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      140 2024-05-28 20:58:36.000000 WaveyMcWaveFace-1.0/TiDE/WaveyMcWaveFace.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       12 2024-05-28 20:58:36.000000 WaveyMcWaveFace-1.0/TiDE/WaveyMcWaveFace.egg-info/top_level.txt
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-28 20:58:36.803419 WaveyMcWaveFace-1.0/TiDE/tests/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-28 16:31:14.000000 WaveyMcWaveFace-1.0/TiDE/tests/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-28 20:58:36.803419 WaveyMcWaveFace-1.0/TiDE/utils/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-28 16:52:21.000000 WaveyMcWaveFace-1.0/TiDE/utils/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    14764 2024-05-28 12:47:02.000000 WaveyMcWaveFace-1.0/TiDE/utils/tide.py
--rw-rw-r--   0 user      (1000) user      (1000)       38 2024-05-28 20:58:36.803419 WaveyMcWaveFace-1.0/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      997 2024-05-28 20:58:34.000000 WaveyMcWaveFace-1.0/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 14:46:29.030052 waveymcwaveface-1.1/
+-rw-r--r--   0 user      (1000) user      (1000)     1251 2024-05-30 14:46:29.029052 waveymcwaveface-1.1/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      549 2024-05-30 14:25:48.000000 waveymcwaveface-1.1/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 14:46:29.026052 waveymcwaveface-1.1/TiDE/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 14:46:29.029052 waveymcwaveface-1.1/TiDE/WaveyMcWaveFace.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     1251 2024-05-30 14:46:28.000000 waveymcwaveface-1.1/TiDE/WaveyMcWaveFace.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      302 2024-05-30 14:46:28.000000 waveymcwaveface-1.1/TiDE/WaveyMcWaveFace.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-05-30 14:46:28.000000 waveymcwaveface-1.1/TiDE/WaveyMcWaveFace.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       97 2024-05-30 14:46:28.000000 waveymcwaveface-1.1/TiDE/WaveyMcWaveFace.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       12 2024-05-30 14:46:28.000000 waveymcwaveface-1.1/TiDE/WaveyMcWaveFace.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 14:46:29.028052 waveymcwaveface-1.1/TiDE/tests/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 14:25:48.000000 waveymcwaveface-1.1/TiDE/tests/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 14:46:29.028052 waveymcwaveface-1.1/TiDE/utils/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 14:25:48.000000 waveymcwaveface-1.1/TiDE/utils/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    14764 2024-05-30 14:25:48.000000 waveymcwaveface-1.1/TiDE/utils/tide.py
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2024-05-30 14:46:29.030052 waveymcwaveface-1.1/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      998 2024-05-30 14:46:18.000000 waveymcwaveface-1.1/setup.py
```

### Comparing `WaveyMcWaveFace-1.0/README.md` & `waveymcwaveface-1.1/README.md`

 * *Files identical despite different names*

### Comparing `WaveyMcWaveFace-1.0/TiDE/utils/tide.py` & `waveymcwaveface-1.1/TiDE/utils/tide.py`

 * *Files identical despite different names*

### Comparing `WaveyMcWaveFace-1.0/setup.py` & `waveymcwaveface-1.1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 from setuptools import find_packages, setup
 
 with open("README.md") as f:
     long_description = f.read()
 
-
-# Function to read the contents of your requirements file
-def read_requirements():
-    with open('requirements.txt') as req:
-        return req.read().splitlines()
-
-
 setup(
     name="WaveyMcWaveFace",
-    version="1.0",
+    version="1.1",
     description="A quick way to run Google's TiDE model",
     package_dir={"": "TiDE"},
     packages=find_packages(where="TiDE"),
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/AmwayCommon/wavey",
     author="Jordan Howell",
     author_email="jordan.howell@amway.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent"
     ],
-    install_requires=read_requirements(),
+    install_requires=['pandas',
+                      'pandas-profiling',
+                      'pandocfilters',
+                      'numpy',
+                      'scikit-learn',
+                      'torch'],
     extras_require={"dev": ["pytest==8.2.1", "twine==5.1.0"]},
     python_requires=">=3.10"
-    )
+)
```

