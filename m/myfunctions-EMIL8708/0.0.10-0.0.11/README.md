# Comparing `tmp/myfunctions_EMIL8708-0.0.10.tar.gz` & `tmp/myfunctions_EMIL8708-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/EMIL8708/python-class/class5/dist/tmpg7hqmkx2/myfunctions_EMIL8708-0.0.10.tar", last modified: Thu May 30 01:16:27 2024, max compression
+gzip compressed data, was "/mnt/EMIL8708/python-class/class5/dist/tmpixuszfy4/myfunctions_EMIL8708-0.0.11.tar", last modified: Thu May 30 01:25:14 2024, max compression
```

## Comparing `myfunctions_EMIL8708-0.0.10.tar` & `myfunctions_EMIL8708-0.0.11.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 EMIL8708  (1658) EMIL8708  (1659)        0 2024-05-30 01:16:27.000000 myfunctions_EMIL8708-0.0.10/
--rw-rw-r--   0 EMIL8708  (1658) EMIL8708  (1659)      638 2024-05-30 01:12:31.000000 myfunctions_EMIL8708-0.0.10/setup.py
-drwxrwxr-x   0 EMIL8708  (1658) EMIL8708  (1659)        0 2024-05-30 01:16:27.000000 myfunctions_EMIL8708-0.0.10/myfunctions_EMIL8708/
--rw-rw-r--   0 EMIL8708  (1658) EMIL8708  (1659)      175 2024-05-30 01:15:52.000000 myfunctions_EMIL8708-0.0.10/myfunctions_EMIL8708/math.py
--rw-rw-r--   0 EMIL8708  (1658) EMIL8708  (1659)        0 2024-05-30 00:49:22.000000 myfunctions_EMIL8708-0.0.10/myfunctions_EMIL8708/__init__.py
-drwxrwxr-x   0 EMIL8708  (1658) EMIL8708  (1659)        0 2024-05-30 01:16:27.000000 myfunctions_EMIL8708-0.0.10/myfunctions_EMIL8708.egg-info/
--rw-rw-r--   0 EMIL8708  (1658) EMIL8708  (1659)       21 2024-05-30 01:16:27.000000 myfunctions_EMIL8708-0.0.10/myfunctions_EMIL8708.egg-info/top_level.txt
--rw-rw-r--   0 EMIL8708  (1658) EMIL8708  (1659)      256 2024-05-30 01:16:27.000000 myfunctions_EMIL8708-0.0.10/myfunctions_EMIL8708.egg-info/SOURCES.txt
--rw-rw-r--   0 EMIL8708  (1658) EMIL8708  (1659)        1 2024-05-30 01:16:27.000000 myfunctions_EMIL8708-0.0.10/myfunctions_EMIL8708.egg-info/dependency_links.txt
--rw-rw-r--   0 EMIL8708  (1658) EMIL8708  (1659)      454 2024-05-30 01:16:27.000000 myfunctions_EMIL8708-0.0.10/myfunctions_EMIL8708.egg-info/PKG-INFO
--rw-rw-r--   0 EMIL8708  (1658) EMIL8708  (1659)        0 2024-05-30 00:49:04.000000 myfunctions_EMIL8708-0.0.10/README.md
--rw-rw-r--   0 EMIL8708  (1658) EMIL8708  (1659)      454 2024-05-30 01:16:27.000000 myfunctions_EMIL8708-0.0.10/PKG-INFO
--rw-rw-r--   0 EMIL8708  (1658) EMIL8708  (1659)       38 2024-05-30 01:16:27.000000 myfunctions_EMIL8708-0.0.10/setup.cfg
+drwxrwxr-x   0 EMIL8708  (1658) EMIL8708  (1659)        0 2024-05-30 01:25:14.000000 myfunctions_EMIL8708-0.0.11/
+-rw-rw-r--   0 EMIL8708  (1658) EMIL8708  (1659)      638 2024-05-30 01:22:31.000000 myfunctions_EMIL8708-0.0.11/setup.py
+drwxrwxr-x   0 EMIL8708  (1658) EMIL8708  (1659)        0 2024-05-30 01:25:14.000000 myfunctions_EMIL8708-0.0.11/myfunctions_EMIL8708/
+-rw-rw-r--   0 EMIL8708  (1658) EMIL8708  (1659)      326 2024-05-30 01:24:27.000000 myfunctions_EMIL8708-0.0.11/myfunctions_EMIL8708/math.py
+-rw-rw-r--   0 EMIL8708  (1658) EMIL8708  (1659)        0 2024-05-30 00:49:22.000000 myfunctions_EMIL8708-0.0.11/myfunctions_EMIL8708/__init__.py
+drwxrwxr-x   0 EMIL8708  (1658) EMIL8708  (1659)        0 2024-05-30 01:25:14.000000 myfunctions_EMIL8708-0.0.11/myfunctions_EMIL8708.egg-info/
+-rw-rw-r--   0 EMIL8708  (1658) EMIL8708  (1659)       21 2024-05-30 01:25:14.000000 myfunctions_EMIL8708-0.0.11/myfunctions_EMIL8708.egg-info/top_level.txt
+-rw-rw-r--   0 EMIL8708  (1658) EMIL8708  (1659)      256 2024-05-30 01:25:14.000000 myfunctions_EMIL8708-0.0.11/myfunctions_EMIL8708.egg-info/SOURCES.txt
+-rw-rw-r--   0 EMIL8708  (1658) EMIL8708  (1659)        1 2024-05-30 01:25:14.000000 myfunctions_EMIL8708-0.0.11/myfunctions_EMIL8708.egg-info/dependency_links.txt
+-rw-rw-r--   0 EMIL8708  (1658) EMIL8708  (1659)     2842 2024-05-30 01:25:14.000000 myfunctions_EMIL8708-0.0.11/myfunctions_EMIL8708.egg-info/PKG-INFO
+-rw-rw-r--   0 EMIL8708  (1658) EMIL8708  (1659)     2395 2024-05-30 01:18:44.000000 myfunctions_EMIL8708-0.0.11/README.md
+-rw-rw-r--   0 EMIL8708  (1658) EMIL8708  (1659)     2842 2024-05-30 01:25:14.000000 myfunctions_EMIL8708-0.0.11/PKG-INFO
+-rw-rw-r--   0 EMIL8708  (1658) EMIL8708  (1659)       38 2024-05-30 01:25:14.000000 myfunctions_EMIL8708-0.0.11/setup.cfg
```

### Comparing `myfunctions_EMIL8708-0.0.10/setup.py` & `myfunctions_EMIL8708-0.0.11/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_EMIL8708',
-    version='0.0.10',
+    version='0.0.11',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/EMIL8708',
     license='MIT',
     author='Emil Moldoisaev',
     author_email='moldoisaemil@gmail.com',
     description='A description of your package',
```

