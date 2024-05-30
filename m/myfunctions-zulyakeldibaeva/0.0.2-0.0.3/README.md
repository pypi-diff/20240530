# Comparing `tmp/myfunctions_zulyakeldibaeva-0.0.2.tar.gz` & `tmp/myfunctions_zulyakeldibaeva-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/zulyakeldibaeva/python-class/evolvecyber/class5/dist/tmpqv_wgix_/myfunctions_zulyakeldibaeva-0.0.2.tar", last modified: Thu May 30 01:14:00 2024, max compression
+gzip compressed data, was "/mnt/zulyakeldibaeva/python-class/evolvecyber/class5/dist/tmpm2omrwaa/myfunctions_zulyakeldibaeva-0.0.3.tar", last modified: Thu May 30 01:20:29 2024, max compression
```

## Comparing `myfunctions_zulyakeldibaeva-0.0.2.tar` & `myfunctions_zulyakeldibaeva-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)        0 2024-05-30 01:14:00.000000 myfunctions_zulyakeldibaeva-0.0.2/
--rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)      659 2024-05-30 01:12:30.000000 myfunctions_zulyakeldibaeva-0.0.2/setup.py
-drwxrwxr-x   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)        0 2024-05-30 01:14:00.000000 myfunctions_zulyakeldibaeva-0.0.2/myfunctions_zulyakeldibaeva.egg-info/
--rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)       28 2024-05-30 01:13:59.000000 myfunctions_zulyakeldibaeva-0.0.2/myfunctions_zulyakeldibaeva.egg-info/top_level.txt
--rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)      298 2024-05-30 01:13:59.000000 myfunctions_zulyakeldibaeva-0.0.2/myfunctions_zulyakeldibaeva.egg-info/SOURCES.txt
--rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)        1 2024-05-30 01:13:59.000000 myfunctions_zulyakeldibaeva-0.0.2/myfunctions_zulyakeldibaeva.egg-info/dependency_links.txt
--rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)      475 2024-05-30 01:13:59.000000 myfunctions_zulyakeldibaeva-0.0.2/myfunctions_zulyakeldibaeva.egg-info/PKG-INFO
--rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)        0 2024-05-30 00:48:24.000000 myfunctions_zulyakeldibaeva-0.0.2/README.md
--rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)      475 2024-05-30 01:14:00.000000 myfunctions_zulyakeldibaeva-0.0.2/PKG-INFO
-drwxrwxr-x   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)        0 2024-05-30 01:13:59.000000 myfunctions_zulyakeldibaeva-0.0.2/myfunctions_zulyakeldibaeva/
--rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)      173 2024-05-30 01:13:07.000000 myfunctions_zulyakeldibaeva-0.0.2/myfunctions_zulyakeldibaeva/math.py
--rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)        0 2024-05-30 00:49:22.000000 myfunctions_zulyakeldibaeva-0.0.2/myfunctions_zulyakeldibaeva/__init__.py
--rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)       38 2024-05-30 01:14:00.000000 myfunctions_zulyakeldibaeva-0.0.2/setup.cfg
+drwxrwxr-x   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)        0 2024-05-30 01:20:29.000000 myfunctions_zulyakeldibaeva-0.0.3/
+-rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)      659 2024-05-30 01:20:18.000000 myfunctions_zulyakeldibaeva-0.0.3/setup.py
+drwxrwxr-x   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)        0 2024-05-30 01:20:29.000000 myfunctions_zulyakeldibaeva-0.0.3/myfunctions_zulyakeldibaeva.egg-info/
+-rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)       28 2024-05-30 01:20:29.000000 myfunctions_zulyakeldibaeva-0.0.3/myfunctions_zulyakeldibaeva.egg-info/top_level.txt
+-rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)      298 2024-05-30 01:20:29.000000 myfunctions_zulyakeldibaeva-0.0.3/myfunctions_zulyakeldibaeva.egg-info/SOURCES.txt
+-rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)        1 2024-05-30 01:20:29.000000 myfunctions_zulyakeldibaeva-0.0.3/myfunctions_zulyakeldibaeva.egg-info/dependency_links.txt
+-rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)     2863 2024-05-30 01:20:29.000000 myfunctions_zulyakeldibaeva-0.0.3/myfunctions_zulyakeldibaeva.egg-info/PKG-INFO
+-rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)     2395 2024-05-30 01:19:31.000000 myfunctions_zulyakeldibaeva-0.0.3/README.md
+-rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)     2863 2024-05-30 01:20:29.000000 myfunctions_zulyakeldibaeva-0.0.3/PKG-INFO
+drwxrwxr-x   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)        0 2024-05-30 01:20:29.000000 myfunctions_zulyakeldibaeva-0.0.3/myfunctions_zulyakeldibaeva/
+-rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)      174 2024-05-30 01:15:19.000000 myfunctions_zulyakeldibaeva-0.0.3/myfunctions_zulyakeldibaeva/math.py
+-rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)        0 2024-05-30 00:49:22.000000 myfunctions_zulyakeldibaeva-0.0.3/myfunctions_zulyakeldibaeva/__init__.py
+-rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)       38 2024-05-30 01:20:29.000000 myfunctions_zulyakeldibaeva-0.0.3/setup.cfg
```

### Comparing `myfunctions_zulyakeldibaeva-0.0.2/setup.py` & `myfunctions_zulyakeldibaeva-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_zulyakeldibaeva',
-    version='0.0.2',
+    version='0.0.3',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/zulyakeldibaeva',
     license='MIT',
     author='Zulfiia Keldibaeva',
     author_email='zulfiiakeldibaeva@gmail.com',
     description='A description of your package',
```

