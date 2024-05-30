# Comparing `tmp/deeplcmd-0.1.2.tar.gz` & `tmp/deeplcmd-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeplcmd-0.1.2.tar", last modified: Thu May 30 10:16:01 2024, max compression
+gzip compressed data, was "deeplcmd-0.1.4.tar", last modified: Thu May 30 17:59:56 2024, max compression
```

## Comparing `deeplcmd-0.1.2.tar` & `deeplcmd-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:16:01.821941 deeplcmd-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-30 10:15:58.000000 deeplcmd-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-30 10:16:01.821941 deeplcmd-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-30 10:15:58.000000 deeplcmd-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:16:01.821941 deeplcmd-0.1.2/deeplcmd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-30 10:16:01.000000 deeplcmd-0.1.2/deeplcmd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-30 10:16:01.000000 deeplcmd-0.1.2/deeplcmd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 10:16:01.000000 deeplcmd-0.1.2/deeplcmd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-30 10:16:01.000000 deeplcmd-0.1.2/deeplcmd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 10:16:01.000000 deeplcmd-0.1.2/deeplcmd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-30 10:16:01.000000 deeplcmd-0.1.2/deeplcmd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8783 2024-05-30 10:15:58.000000 deeplcmd-0.1.2/deeplcmd.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 10:16:01.821941 deeplcmd-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-30 10:15:58.000000 deeplcmd-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:59:56.733719 deeplcmd-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-30 17:59:53.000000 deeplcmd-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-30 17:59:56.733719 deeplcmd-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-30 17:59:53.000000 deeplcmd-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:59:56.729719 deeplcmd-0.1.4/deeplcmd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 17:59:53.000000 deeplcmd-0.1.4/deeplcmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8783 2024-05-30 17:59:53.000000 deeplcmd-0.1.4/deeplcmd/deeplcmd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:59:56.733719 deeplcmd-0.1.4/deeplcmd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-30 17:59:56.000000 deeplcmd-0.1.4/deeplcmd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-30 17:59:56.000000 deeplcmd-0.1.4/deeplcmd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 17:59:56.000000 deeplcmd-0.1.4/deeplcmd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-30 17:59:56.000000 deeplcmd-0.1.4/deeplcmd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 17:59:56.000000 deeplcmd-0.1.4/deeplcmd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-30 17:59:56.000000 deeplcmd-0.1.4/deeplcmd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 17:59:56.733719 deeplcmd-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-30 17:59:53.000000 deeplcmd-0.1.4/setup.py
```

### Comparing `deeplcmd-0.1.2/LICENSE` & `deeplcmd-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `deeplcmd-0.1.2/PKG-INFO` & `deeplcmd-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 Metadata-Version: 2.1
 Name: deeplcmd
-Version: 0.1.2
+Version: 0.1.4
 Summary: DeepLCMD is a simple command line app for text and document translation with Deepl Translator API 
 Home-page: https://github.com/ilya-smut/deeplcmd
 Author: Ilya Smut
 Author-email: ilya.smut.off.g@gmail.com
-License: GPL-3.0 license 
+License: GPL-3.0 license
 Project-URL: Source Code, https://github.com/ilya-smut/deeplcmd
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Click
 Requires-Dist: Deepl
 
-
 # DeepLCMD
 
 DeepLCMD is a Python-based command line tool that utilizes the DeepL API to translate text and documents into a variety of languages.
 
 ## Features
 
 - Translate text directly from the command line
 - Translate documents from a given file path
 - Supports a variety of target languages
 
 ## Installation
 ```bash
-git clone https://github.com/ilya-smut/deeplcmd
-cd deeplcmd
-pip install -e .
+pip install deeplcmd
 ```
 Please, note. You may want to create a virtual environment for the installation of the script
 ```bash
 python -m venv .venv
 .venv/bin/activate
 ```
 read more about virtual environments here https://docs.python.org/3/library/venv.html
@@ -48,14 +45,21 @@
 OR
 
 ```bash
 deeplcmd login -kf PATH_TO_YOUR_KEYFILE
 
 ```
 
+OR
+
+Open an interactive login. Will prompt you for either a filepath or a key
+```bash
+deeplcmd login
+```
+
 You can translate text using the `text` command:
 
 ```bash
 deeplcmd text -tl TARGET_LANGUAGE "Your text here"
 
 ```
```

### Comparing `deeplcmd-0.1.2/README.md` & `deeplcmd-0.1.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 
 - Translate text directly from the command line
 - Translate documents from a given file path
 - Supports a variety of target languages
 
 ## Installation
 ```bash
-git clone https://github.com/ilya-smut/deeplcmd
-cd deeplcmd
-pip install -e .
+pip install deeplcmd
 ```
 Please, note. You may want to create a virtual environment for the installation of the script
 ```bash
 python -m venv .venv
 .venv/bin/activate
 ```
 read more about virtual environments here https://docs.python.org/3/library/venv.html
@@ -33,14 +31,21 @@
 OR
 
 ```bash
 deeplcmd login -kf PATH_TO_YOUR_KEYFILE
 
 ```
 
+OR
+
+Open an interactive login. Will prompt you for either a filepath or a key
+```bash
+deeplcmd login
+```
+
 You can translate text using the `text` command:
 
 ```bash
 deeplcmd text -tl TARGET_LANGUAGE "Your text here"
 
 ```
 
@@ -49,8 +54,8 @@
 ```bash
 deeplcmd file -tl TARGET_LANGUAGE INPUT_FILE OUTPUT_FILE
 
 ```
 
 In both cases, replace `TARGET_LANGUAGE` with the language you want to translate to. 
 
-Please note that the use of the DeepL API you will need to obtain API key from https://www.deepl.com/pro-api?cta=header-pro-api
+Please note that the use of the DeepL API you will need to obtain API key from https://www.deepl.com/pro-api?cta=header-pro-api
```

### Comparing `deeplcmd-0.1.2/deeplcmd.egg-info/PKG-INFO` & `deeplcmd-0.1.4/deeplcmd.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 Metadata-Version: 2.1
 Name: deeplcmd
-Version: 0.1.2
+Version: 0.1.4
 Summary: DeepLCMD is a simple command line app for text and document translation with Deepl Translator API 
 Home-page: https://github.com/ilya-smut/deeplcmd
 Author: Ilya Smut
 Author-email: ilya.smut.off.g@gmail.com
-License: GPL-3.0 license 
+License: GPL-3.0 license
 Project-URL: Source Code, https://github.com/ilya-smut/deeplcmd
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Click
 Requires-Dist: Deepl
 
-
 # DeepLCMD
 
 DeepLCMD is a Python-based command line tool that utilizes the DeepL API to translate text and documents into a variety of languages.
 
 ## Features
 
 - Translate text directly from the command line
 - Translate documents from a given file path
 - Supports a variety of target languages
 
 ## Installation
 ```bash
-git clone https://github.com/ilya-smut/deeplcmd
-cd deeplcmd
-pip install -e .
+pip install deeplcmd
 ```
 Please, note. You may want to create a virtual environment for the installation of the script
 ```bash
 python -m venv .venv
 .venv/bin/activate
 ```
 read more about virtual environments here https://docs.python.org/3/library/venv.html
@@ -48,14 +45,21 @@
 OR
 
 ```bash
 deeplcmd login -kf PATH_TO_YOUR_KEYFILE
 
 ```
 
+OR
+
+Open an interactive login. Will prompt you for either a filepath or a key
+```bash
+deeplcmd login
+```
+
 You can translate text using the `text` command:
 
 ```bash
 deeplcmd text -tl TARGET_LANGUAGE "Your text here"
 
 ```
```

### Comparing `deeplcmd-0.1.2/deeplcmd.py` & `deeplcmd-0.1.4/deeplcmd/deeplcmd.py`

 * *Files identical despite different names*

