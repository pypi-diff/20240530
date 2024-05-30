# Comparing `tmp/myfunctions_aizhan010-0.0.2.tar.gz` & `tmp/myfunctions_aizhan010-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/aizhan010/python/evolvecyber/class5/dist/tmpn165pyb2/myfunctions_aizhan010-0.0.2.tar", last modified: Thu May 30 01:14:11 2024, max compression
+gzip compressed data, was "/mnt/aizhan010/python/evolvecyber/class5/dist/tmpqjc459j4/myfunctions_aizhan010-0.0.3.tar", last modified: Thu May 30 01:19:06 2024, max compression
```

## Comparing `myfunctions_aizhan010-0.0.2.tar` & `myfunctions_aizhan010-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 aizhan010  (1710) aizhan010  (1711)        0 2024-05-30 01:14:11.000000 myfunctions_aizhan010-0.0.2/
--rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)      643 2024-05-30 01:12:44.000000 myfunctions_aizhan010-0.0.2/setup.py
-drwxrwxr-x   0 aizhan010  (1710) aizhan010  (1711)        0 2024-05-30 01:14:11.000000 myfunctions_aizhan010-0.0.2/myfunctions_aizhan010.egg-info/
--rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)        1 2024-05-30 01:14:11.000000 myfunctions_aizhan010-0.0.2/myfunctions_aizhan010.egg-info/top_level.txt
--rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)      198 2024-05-30 01:14:11.000000 myfunctions_aizhan010-0.0.2/myfunctions_aizhan010.egg-info/SOURCES.txt
--rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)        1 2024-05-30 01:14:11.000000 myfunctions_aizhan010-0.0.2/myfunctions_aizhan010.egg-info/dependency_links.txt
--rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)      459 2024-05-30 01:14:11.000000 myfunctions_aizhan010-0.0.2/myfunctions_aizhan010.egg-info/PKG-INFO
--rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)        0 2024-05-30 00:48:26.000000 myfunctions_aizhan010-0.0.2/README.md
--rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)      459 2024-05-30 01:14:11.000000 myfunctions_aizhan010-0.0.2/PKG-INFO
--rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)       38 2024-05-30 01:14:11.000000 myfunctions_aizhan010-0.0.2/setup.cfg
+drwxrwxr-x   0 aizhan010  (1710) aizhan010  (1711)        0 2024-05-30 01:19:06.000000 myfunctions_aizhan010-0.0.3/
+-rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)      643 2024-05-30 01:18:43.000000 myfunctions_aizhan010-0.0.3/setup.py
+drwxrwxr-x   0 aizhan010  (1710) aizhan010  (1711)        0 2024-05-30 01:19:06.000000 myfunctions_aizhan010-0.0.3/myfunctions_aizhan010.egg-info/
+-rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)        1 2024-05-30 01:19:06.000000 myfunctions_aizhan010-0.0.3/myfunctions_aizhan010.egg-info/top_level.txt
+-rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)      198 2024-05-30 01:19:06.000000 myfunctions_aizhan010-0.0.3/myfunctions_aizhan010.egg-info/SOURCES.txt
+-rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)        1 2024-05-30 01:19:06.000000 myfunctions_aizhan010-0.0.3/myfunctions_aizhan010.egg-info/dependency_links.txt
+-rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)     2847 2024-05-30 01:19:06.000000 myfunctions_aizhan010-0.0.3/myfunctions_aizhan010.egg-info/PKG-INFO
+-rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)     2395 2024-05-30 01:18:35.000000 myfunctions_aizhan010-0.0.3/README.md
+-rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)     2847 2024-05-30 01:19:06.000000 myfunctions_aizhan010-0.0.3/PKG-INFO
+-rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)       38 2024-05-30 01:19:06.000000 myfunctions_aizhan010-0.0.3/setup.cfg
```

### Comparing `myfunctions_aizhan010-0.0.2/setup.py` & `myfunctions_aizhan010-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_aizhan010',
-    version='0.0.2',
+    version='0.0.3',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/aizhan010/',
     license='MIT',
     author='Aizhan Maratova',
     author_email='aizhanmaratova6@gmail.com',
     description='A description of your package',
```

