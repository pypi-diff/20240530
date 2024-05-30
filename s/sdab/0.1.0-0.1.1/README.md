# Comparing `tmp/sdab-0.1.0.tar.gz` & `tmp/sdab-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdab-0.1.0.tar", last modified: Thu May 30 01:25:47 2024, max compression
+gzip compressed data, was "sdab-0.1.1.tar", last modified: Thu May 30 01:40:06 2024, max compression
```

## Comparing `sdab-0.1.0.tar` & `sdab-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:25:47.978073 sdab-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-30 01:25:37.000000 sdab-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-30 01:25:47.978073 sdab-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-30 01:25:37.000000 sdab-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:25:47.978073 sdab-0.1.0/sdab/
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-30 01:25:37.000000 sdab-0.1.0/sdab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:25:47.978073 sdab-0.1.0/sdab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-30 01:25:47.000000 sdab-0.1.0/sdab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-30 01:25:47.000000 sdab-0.1.0/sdab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 01:25:47.000000 sdab-0.1.0/sdab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-30 01:25:47.000000 sdab-0.1.0/sdab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-30 01:25:47.000000 sdab-0.1.0/sdab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 01:25:47.978073 sdab-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-30 01:25:37.000000 sdab-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:40:06.668221 sdab-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-30 01:39:57.000000 sdab-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-05-30 01:40:06.668221 sdab-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-30 01:39:57.000000 sdab-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:40:06.668221 sdab-0.1.1/sdab/
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-30 01:39:57.000000 sdab-0.1.1/sdab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:40:06.668221 sdab-0.1.1/sdab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-05-30 01:40:06.000000 sdab-0.1.1/sdab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-30 01:40:06.000000 sdab-0.1.1/sdab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 01:40:06.000000 sdab-0.1.1/sdab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-30 01:40:06.000000 sdab-0.1.1/sdab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-30 01:40:06.000000 sdab-0.1.1/sdab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 01:40:06.668221 sdab-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-30 01:39:57.000000 sdab-0.1.1/setup.py
```

### Comparing `sdab-0.1.0/LICENSE` & `sdab-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sdab-0.1.0/PKG-INFO` & `sdab-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdab
-Version: 0.1.0
+Version: 0.1.1
 Summary: Khmer Speech To Text Inference API using Wav2Vec2 with Pretrain Model
 Home-page: https://github.com/MetythornPenn/sdab.git
 Author: Metythorn Penn
 Author-email: metythorn@gmail.com
 License: Apache Software License 2.0
 Description: # Sdab
         
@@ -13,31 +13,47 @@
          
         Sdab is a Python package for Automatic Speech Recognition with focus on Khmer language. It have offline khmer automatic speech recognition model from my Pretrain Model and other that using Wav2Vec2 model.
         
         License: [Apache-2.0 License](https://github.com/MetythornPenn/sdab/blob/main/LICENSE)
         
         Pretrain Model: [Huggingface](https://huggingface.co/metythorn/khmer-asr-openslr)
         
-        ## Install From Source
+        ## Installation
+        
+        
+        #### Install from source
+        ```sh
+        pip install sdab
+        ```
+        
+        #### Install from source
         
         ```sh
         
         # clone repo 
         git clone https://github.com/MetythornPenn/sdab.git
         
-        # install lib from source (recommend python 3.8)
+        # install lib from source
         pip install -e .
         ```
         
         ## Usage
         
+        #### Download sample audio
+        
+        ```bash
+        wget -O audio.wav https://github.com/MetythornPenn/sdab/blob/main/sample/audio.wav
+        ```
+        
+        #### Python API
+        
         ```python
         from sdab import Sdab
         
-        file_path = "sample/audio.wav"
+        file_path = "audio.wav"
         model_name = "metythorn/khmer-asr-openslr"  # or local directory path
         
         sdab = Sdab( file_path = file_path, model_name = model_name)
         print(sdab.result)
         
         # result : ស្ពានកំពងចំលងអ្នកលើងនៅព្រីវែញជាស្ពានវេញជាងគេសក្នុងព្រសរាជាអាចកម្ពុជា
         ```
```

### Comparing `sdab-0.1.0/README.md` & `sdab-0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -5,31 +5,47 @@
  
 Sdab is a Python package for Automatic Speech Recognition with focus on Khmer language. It have offline khmer automatic speech recognition model from my Pretrain Model and other that using Wav2Vec2 model.
 
 License: [Apache-2.0 License](https://github.com/MetythornPenn/sdab/blob/main/LICENSE)
 
 Pretrain Model: [Huggingface](https://huggingface.co/metythorn/khmer-asr-openslr)
 
-## Install From Source
+## Installation
+
+
+#### Install from source
+```sh
+pip install sdab
+```
+
+#### Install from source
 
 ```sh
 
 # clone repo 
 git clone https://github.com/MetythornPenn/sdab.git
 
-# install lib from source (recommend python 3.8)
+# install lib from source
 pip install -e .
 ```
 
 ## Usage
 
+#### Download sample audio
+
+```bash
+wget -O audio.wav https://github.com/MetythornPenn/sdab/blob/main/sample/audio.wav
+```
+
+#### Python API
+
 ```python
 from sdab import Sdab
 
-file_path = "sample/audio.wav"
+file_path = "audio.wav"
 model_name = "metythorn/khmer-asr-openslr"  # or local directory path
 
 sdab = Sdab( file_path = file_path, model_name = model_name)
 print(sdab.result)
 
 # result : ស្ពានកំពងចំលងអ្នកលើងនៅព្រីវែញជាស្ពានវេញជាងគេសក្នុងព្រសរាជាអាចកម្ពុជា
 ```
```

### Comparing `sdab-0.1.0/sdab/__init__.py` & `sdab-0.1.1/sdab/__init__.py`

 * *Files identical despite different names*

### Comparing `sdab-0.1.0/sdab.egg-info/PKG-INFO` & `sdab-0.1.1/sdab.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdab
-Version: 0.1.0
+Version: 0.1.1
 Summary: Khmer Speech To Text Inference API using Wav2Vec2 with Pretrain Model
 Home-page: https://github.com/MetythornPenn/sdab.git
 Author: Metythorn Penn
 Author-email: metythorn@gmail.com
 License: Apache Software License 2.0
 Description: # Sdab
         
@@ -13,31 +13,47 @@
          
         Sdab is a Python package for Automatic Speech Recognition with focus on Khmer language. It have offline khmer automatic speech recognition model from my Pretrain Model and other that using Wav2Vec2 model.
         
         License: [Apache-2.0 License](https://github.com/MetythornPenn/sdab/blob/main/LICENSE)
         
         Pretrain Model: [Huggingface](https://huggingface.co/metythorn/khmer-asr-openslr)
         
-        ## Install From Source
+        ## Installation
+        
+        
+        #### Install from source
+        ```sh
+        pip install sdab
+        ```
+        
+        #### Install from source
         
         ```sh
         
         # clone repo 
         git clone https://github.com/MetythornPenn/sdab.git
         
-        # install lib from source (recommend python 3.8)
+        # install lib from source
         pip install -e .
         ```
         
         ## Usage
         
+        #### Download sample audio
+        
+        ```bash
+        wget -O audio.wav https://github.com/MetythornPenn/sdab/blob/main/sample/audio.wav
+        ```
+        
+        #### Python API
+        
         ```python
         from sdab import Sdab
         
-        file_path = "sample/audio.wav"
+        file_path = "audio.wav"
         model_name = "metythorn/khmer-asr-openslr"  # or local directory path
         
         sdab = Sdab( file_path = file_path, model_name = model_name)
         print(sdab.result)
         
         # result : ស្ពានកំពងចំលងអ្នកលើងនៅព្រីវែញជាស្ពានវេញជាងគេសក្នុងព្រសរាជាអាចកម្ពុជា
         ```
```

### Comparing `sdab-0.1.0/setup.py` & `sdab-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     'soundfile',
     'torch',
     'numpy',
 ]
 
 setup(
     name='sdab',
-    version='0.1.0',
+    version='0.1.1',
     packages=['sdab'],
     url='https://github.com/MetythornPenn/sdab.git',
     license='Apache Software License 2.0',
     author = 'Metythorn Penn',
     author_email = 'metythorn@gmail.com',
     keywords='asr',
     description='Khmer Speech To Text Inference API using Wav2Vec2 with Pretrain Model',
```

