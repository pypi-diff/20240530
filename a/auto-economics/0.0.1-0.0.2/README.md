# Comparing `tmp/auto_economics-0.0.1.tar.gz` & `tmp/auto_economics-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_economics-0.0.1.tar", last modified: Wed May 29 15:07:32 2024, max compression
+gzip compressed data, was "auto_economics-0.0.2.tar", last modified: Thu May 30 06:54:05 2024, max compression
```

## Comparing `auto_economics-0.0.1.tar` & `auto_economics-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ulrikhaugland   (501) staff       (20)        0 2024-05-29 15:07:32.081836 auto_economics-0.0.1/
--rw-rw-r--   0 ulrikhaugland   (501) staff       (20)    11337 2023-04-27 10:12:58.000000 auto_economics-0.0.1/LICENSE
--rw-rw-r--   0 ulrikhaugland   (501) staff       (20)      111 2023-04-27 10:12:58.000000 auto_economics-0.0.1/MANIFEST.in
--rw-r--r--   0 ulrikhaugland   (501) staff       (20)      823 2024-05-29 15:07:32.081524 auto_economics-0.0.1/PKG-INFO
--rw-rw-r--   0 ulrikhaugland   (501) staff       (20)       47 2023-04-27 10:12:58.000000 auto_economics-0.0.1/README.md
-drwxr-xr-x   0 ulrikhaugland   (501) staff       (20)        0 2024-05-29 15:07:32.079640 auto_economics-0.0.1/auto_economics/
--rw-r--r--   0 ulrikhaugland   (501) staff       (20)       22 2024-05-29 14:52:35.000000 auto_economics-0.0.1/auto_economics/__init__.py
--rw-r--r--   0 ulrikhaugland   (501) staff       (20)      324 2024-05-29 14:52:35.000000 auto_economics-0.0.1/auto_economics/_modidx.py
--rw-r--r--   0 ulrikhaugland   (501) staff       (20)      796 2024-05-29 14:52:35.000000 auto_economics-0.0.1/auto_economics/core.py
-drwxr-xr-x   0 ulrikhaugland   (501) staff       (20)        0 2024-05-29 15:07:32.081195 auto_economics-0.0.1/auto_economics.egg-info/
--rw-r--r--   0 ulrikhaugland   (501) staff       (20)      823 2024-05-29 15:07:32.000000 auto_economics-0.0.1/auto_economics.egg-info/PKG-INFO
--rw-r--r--   0 ulrikhaugland   (501) staff       (20)      394 2024-05-29 15:07:32.000000 auto_economics-0.0.1/auto_economics.egg-info/SOURCES.txt
--rw-r--r--   0 ulrikhaugland   (501) staff       (20)        1 2024-05-29 15:07:32.000000 auto_economics-0.0.1/auto_economics.egg-info/dependency_links.txt
--rw-r--r--   0 ulrikhaugland   (501) staff       (20)       50 2024-05-29 15:07:32.000000 auto_economics-0.0.1/auto_economics.egg-info/entry_points.txt
--rw-r--r--   0 ulrikhaugland   (501) staff       (20)        1 2024-05-29 13:35:39.000000 auto_economics-0.0.1/auto_economics.egg-info/not-zip-safe
--rw-r--r--   0 ulrikhaugland   (501) staff       (20)        7 2024-05-29 15:07:32.000000 auto_economics-0.0.1/auto_economics.egg-info/requires.txt
--rw-r--r--   0 ulrikhaugland   (501) staff       (20)       15 2024-05-29 15:07:32.000000 auto_economics-0.0.1/auto_economics.egg-info/top_level.txt
--rw-r--r--   0 ulrikhaugland   (501) staff       (20)      957 2024-05-29 14:11:13.000000 auto_economics-0.0.1/settings.ini
--rw-r--r--   0 ulrikhaugland   (501) staff       (20)       38 2024-05-29 15:07:32.081895 auto_economics-0.0.1/setup.cfg
--rw-rw-r--   0 ulrikhaugland   (501) staff       (20)     2596 2023-04-27 10:12:58.000000 auto_economics-0.0.1/setup.py
+drwxr-xr-x   0 ulrikhaugland   (501) staff       (20)        0 2024-05-30 06:54:05.407876 auto_economics-0.0.2/
+-rw-rw-r--   0 ulrikhaugland   (501) staff       (20)    11337 2023-04-27 10:12:58.000000 auto_economics-0.0.2/LICENSE
+-rw-rw-r--   0 ulrikhaugland   (501) staff       (20)      111 2023-04-27 10:12:58.000000 auto_economics-0.0.2/MANIFEST.in
+-rw-r--r--   0 ulrikhaugland   (501) staff       (20)     2185 2024-05-30 06:54:05.407530 auto_economics-0.0.2/PKG-INFO
+-rw-r--r--   0 ulrikhaugland   (501) staff       (20)     1409 2024-05-30 06:52:54.000000 auto_economics-0.0.2/README.md
+drwxr-xr-x   0 ulrikhaugland   (501) staff       (20)        0 2024-05-30 06:54:05.405480 auto_economics-0.0.2/auto_economics/
+-rw-r--r--   0 ulrikhaugland   (501) staff       (20)       22 2024-05-30 06:50:54.000000 auto_economics-0.0.2/auto_economics/__init__.py
+-rw-r--r--   0 ulrikhaugland   (501) staff       (20)     3953 2024-05-30 06:52:24.000000 auto_economics-0.0.2/auto_economics/_modidx.py
+-rw-r--r--   0 ulrikhaugland   (501) staff       (20)    16820 2024-05-30 06:50:54.000000 auto_economics-0.0.2/auto_economics/core.py
+drwxr-xr-x   0 ulrikhaugland   (501) staff       (20)        0 2024-05-30 06:54:05.407177 auto_economics-0.0.2/auto_economics.egg-info/
+-rw-r--r--   0 ulrikhaugland   (501) staff       (20)     2185 2024-05-30 06:54:05.000000 auto_economics-0.0.2/auto_economics.egg-info/PKG-INFO
+-rw-r--r--   0 ulrikhaugland   (501) staff       (20)      394 2024-05-30 06:54:05.000000 auto_economics-0.0.2/auto_economics.egg-info/SOURCES.txt
+-rw-r--r--   0 ulrikhaugland   (501) staff       (20)        1 2024-05-30 06:54:05.000000 auto_economics-0.0.2/auto_economics.egg-info/dependency_links.txt
+-rw-r--r--   0 ulrikhaugland   (501) staff       (20)       50 2024-05-30 06:54:05.000000 auto_economics-0.0.2/auto_economics.egg-info/entry_points.txt
+-rw-r--r--   0 ulrikhaugland   (501) staff       (20)        1 2024-05-29 13:35:39.000000 auto_economics-0.0.2/auto_economics.egg-info/not-zip-safe
+-rw-r--r--   0 ulrikhaugland   (501) staff       (20)        7 2024-05-30 06:54:05.000000 auto_economics-0.0.2/auto_economics.egg-info/requires.txt
+-rw-r--r--   0 ulrikhaugland   (501) staff       (20)       15 2024-05-30 06:54:05.000000 auto_economics-0.0.2/auto_economics.egg-info/top_level.txt
+-rw-r--r--   0 ulrikhaugland   (501) staff       (20)      957 2024-05-30 06:53:26.000000 auto_economics-0.0.2/settings.ini
+-rw-r--r--   0 ulrikhaugland   (501) staff       (20)       38 2024-05-30 06:54:05.407936 auto_economics-0.0.2/setup.cfg
+-rw-rw-r--   0 ulrikhaugland   (501) staff       (20)     2596 2023-04-27 10:12:58.000000 auto_economics-0.0.2/setup.py
```

### Comparing `auto_economics-0.0.1/LICENSE` & `auto_economics-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_economics-0.0.1/settings.ini` & `auto_economics-0.0.2/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = auto_economics
 lib_name = %(repo)s
-version = 0.0.1
+version = 0.0.2
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = auto_economics
```

### Comparing `auto_economics-0.0.1/setup.py` & `auto_economics-0.0.2/setup.py`

 * *Files identical despite different names*

