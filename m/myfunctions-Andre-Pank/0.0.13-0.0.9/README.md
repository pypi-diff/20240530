# Comparing `tmp/myfunctions_Andre-Pank-0.0.13.tar.gz` & `tmp/myfunctions_Andre-Pank-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/Andre-Pank/Python-class/evolve-cyber/class5/dist/tmpoc6a9ukw/myfunctions_Andre-Pank-0.0.13.tar", last modified: Thu May 30 01:33:19 2024, max compression
+gzip compressed data, was "/mnt/Andre-Pank/Python-class/evolve-cyber/class5/dist/tmpt59u4fa7/myfunctions_Andre-Pank-0.0.9.tar", last modified: Thu May 30 01:05:27 2024, max compression
```

## Comparing `myfunctions_Andre-Pank-0.0.13.tar` & `myfunctions_Andre-Pank-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 Andre-Pank  (1706) Andre-Pank  (1707)        0 2024-05-30 01:33:19.000000 myfunctions_Andre-Pank-0.0.13/
--rw-rw-r--   0 Andre-Pank  (1706) Andre-Pank  (1707)      650 2024-05-30 01:31:45.000000 myfunctions_Andre-Pank-0.0.13/setup.py
--rw-rw-r--   0 Andre-Pank  (1706) Andre-Pank  (1707)        0 2024-05-30 01:05:16.000000 myfunctions_Andre-Pank-0.0.13/README.md
--rw-rw-r--   0 Andre-Pank  (1706) Andre-Pank  (1707)      466 2024-05-30 01:33:19.000000 myfunctions_Andre-Pank-0.0.13/PKG-INFO
-drwxrwxr-x   0 Andre-Pank  (1706) Andre-Pank  (1707)        0 2024-05-30 01:33:19.000000 myfunctions_Andre-Pank-0.0.13/myfunctions_Andre_Pank.egg-info/
--rw-rw-r--   0 Andre-Pank  (1706) Andre-Pank  (1707)       23 2024-05-30 01:33:19.000000 myfunctions_Andre-Pank-0.0.13/myfunctions_Andre_Pank.egg-info/top_level.txt
--rw-rw-r--   0 Andre-Pank  (1706) Andre-Pank  (1707)      268 2024-05-30 01:33:19.000000 myfunctions_Andre-Pank-0.0.13/myfunctions_Andre_Pank.egg-info/SOURCES.txt
--rw-rw-r--   0 Andre-Pank  (1706) Andre-Pank  (1707)        1 2024-05-30 01:33:19.000000 myfunctions_Andre-Pank-0.0.13/myfunctions_Andre_Pank.egg-info/dependency_links.txt
--rw-rw-r--   0 Andre-Pank  (1706) Andre-Pank  (1707)      466 2024-05-30 01:33:19.000000 myfunctions_Andre-Pank-0.0.13/myfunctions_Andre_Pank.egg-info/PKG-INFO
-drwxrwxr-x   0 Andre-Pank  (1706) Andre-Pank  (1707)        0 2024-05-30 01:33:19.000000 myfunctions_Andre-Pank-0.0.13/myfunctions_Andre-Pank/
--rw-rw-r--   0 Andre-Pank  (1706) Andre-Pank  (1707)      440 2024-05-30 01:31:15.000000 myfunctions_Andre-Pank-0.0.13/myfunctions_Andre-Pank/math.py
--rw-rw-r--   0 Andre-Pank  (1706) Andre-Pank  (1707)        0 2024-05-30 00:49:24.000000 myfunctions_Andre-Pank-0.0.13/myfunctions_Andre-Pank/__init__.py
--rw-rw-r--   0 Andre-Pank  (1706) Andre-Pank  (1707)       38 2024-05-30 01:33:19.000000 myfunctions_Andre-Pank-0.0.13/setup.cfg
+drwxrwxr-x   0 Andre-Pank  (1706) Andre-Pank  (1707)        0 2024-05-30 01:05:27.000000 myfunctions_Andre-Pank-0.0.9/
+-rw-rw-r--   0 Andre-Pank  (1706) Andre-Pank  (1707)      649 2024-05-30 01:00:08.000000 myfunctions_Andre-Pank-0.0.9/setup.py
+-rw-rw-r--   0 Andre-Pank  (1706) Andre-Pank  (1707)        0 2024-05-30 01:05:16.000000 myfunctions_Andre-Pank-0.0.9/README.md
+-rw-rw-r--   0 Andre-Pank  (1706) Andre-Pank  (1707)      465 2024-05-30 01:05:27.000000 myfunctions_Andre-Pank-0.0.9/PKG-INFO
+drwxrwxr-x   0 Andre-Pank  (1706) Andre-Pank  (1707)        0 2024-05-30 01:05:27.000000 myfunctions_Andre-Pank-0.0.9/myfunctions_Andre_Pank.egg-info/
+-rw-rw-r--   0 Andre-Pank  (1706) Andre-Pank  (1707)       23 2024-05-30 01:05:27.000000 myfunctions_Andre-Pank-0.0.9/myfunctions_Andre_Pank.egg-info/top_level.txt
+-rw-rw-r--   0 Andre-Pank  (1706) Andre-Pank  (1707)      268 2024-05-30 01:05:27.000000 myfunctions_Andre-Pank-0.0.9/myfunctions_Andre_Pank.egg-info/SOURCES.txt
+-rw-rw-r--   0 Andre-Pank  (1706) Andre-Pank  (1707)        1 2024-05-30 01:05:27.000000 myfunctions_Andre-Pank-0.0.9/myfunctions_Andre_Pank.egg-info/dependency_links.txt
+-rw-rw-r--   0 Andre-Pank  (1706) Andre-Pank  (1707)      465 2024-05-30 01:05:27.000000 myfunctions_Andre-Pank-0.0.9/myfunctions_Andre_Pank.egg-info/PKG-INFO
+drwxrwxr-x   0 Andre-Pank  (1706) Andre-Pank  (1707)        0 2024-05-30 01:05:27.000000 myfunctions_Andre-Pank-0.0.9/myfunctions_Andre-Pank/
+-rw-rw-r--   0 Andre-Pank  (1706) Andre-Pank  (1707)      113 2024-05-30 00:54:50.000000 myfunctions_Andre-Pank-0.0.9/myfunctions_Andre-Pank/math.py
+-rw-rw-r--   0 Andre-Pank  (1706) Andre-Pank  (1707)        0 2024-05-30 00:49:24.000000 myfunctions_Andre-Pank-0.0.9/myfunctions_Andre-Pank/__init__.py
+-rw-rw-r--   0 Andre-Pank  (1706) Andre-Pank  (1707)       38 2024-05-30 01:05:27.000000 myfunctions_Andre-Pank-0.0.9/setup.cfg
```

### Comparing `myfunctions_Andre-Pank-0.0.13/setup.py` & `myfunctions_Andre-Pank-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_Andre-Pank',
-    version='0.0.13',
+    version='0.0.9',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/Andre-Pank',
     license='MIT',
     author='Andrei Pankevitch ',
     author_email='panchevici.andrei@gmail.com',
     description='A description of your package',
```

