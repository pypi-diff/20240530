# Comparing `tmp/myfunctions_andreibelous16-0.0.2.tar.gz` & `tmp/myfunctions_andreibelous16-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/Andreibelous16/python_class/evolvecyber/class5/dist/tmp4sj_3262/myfunctions_andreibelous16-0.0.2.tar", last modified: Thu May 30 01:14:40 2024, max compression
+gzip compressed data, was "/mnt/Andreibelous16/python_class/evolvecyber/class5/dist/tmp7cy6d1h9/myfunctions_andreibelous16-0.0.3.tar", last modified: Thu May 30 01:19:18 2024, max compression
```

## Comparing `myfunctions_andreibelous16-0.0.2.tar` & `myfunctions_andreibelous16-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 Andreibelous16  (1709) Andreibelous16  (1710)        0 2024-05-30 01:14:40.000000 myfunctions_andreibelous16-0.0.2/
--rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)      649 2024-05-30 01:14:17.000000 myfunctions_andreibelous16-0.0.2/setup.py
-drwxrwxr-x   0 Andreibelous16  (1709) Andreibelous16  (1710)        0 2024-05-30 01:14:40.000000 myfunctions_andreibelous16-0.0.2/myfunctions_andreibelous16.egg-info/
--rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)       27 2024-05-30 01:14:40.000000 myfunctions_andreibelous16-0.0.2/myfunctions_andreibelous16.egg-info/top_level.txt
--rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)      292 2024-05-30 01:14:40.000000 myfunctions_andreibelous16-0.0.2/myfunctions_andreibelous16.egg-info/SOURCES.txt
--rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)        1 2024-05-30 01:14:40.000000 myfunctions_andreibelous16-0.0.2/myfunctions_andreibelous16.egg-info/dependency_links.txt
--rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)      465 2024-05-30 01:14:40.000000 myfunctions_andreibelous16-0.0.2/myfunctions_andreibelous16.egg-info/PKG-INFO
-drwxrwxr-x   0 Andreibelous16  (1709) Andreibelous16  (1710)        0 2024-05-30 01:14:40.000000 myfunctions_andreibelous16-0.0.2/myfunctions_andreibelous16/
--rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)      175 2024-05-30 01:12:57.000000 myfunctions_andreibelous16-0.0.2/myfunctions_andreibelous16/math.py
--rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)        0 2024-05-30 00:48:50.000000 myfunctions_andreibelous16-0.0.2/myfunctions_andreibelous16/__init__.py
--rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)        0 2024-05-30 00:48:27.000000 myfunctions_andreibelous16-0.0.2/README.md
--rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)      465 2024-05-30 01:14:40.000000 myfunctions_andreibelous16-0.0.2/PKG-INFO
--rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)       38 2024-05-30 01:14:40.000000 myfunctions_andreibelous16-0.0.2/setup.cfg
+drwxrwxr-x   0 Andreibelous16  (1709) Andreibelous16  (1710)        0 2024-05-30 01:19:18.000000 myfunctions_andreibelous16-0.0.3/
+-rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)      649 2024-05-30 01:18:51.000000 myfunctions_andreibelous16-0.0.3/setup.py
+drwxrwxr-x   0 Andreibelous16  (1709) Andreibelous16  (1710)        0 2024-05-30 01:19:18.000000 myfunctions_andreibelous16-0.0.3/myfunctions_andreibelous16.egg-info/
+-rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)       27 2024-05-30 01:19:18.000000 myfunctions_andreibelous16-0.0.3/myfunctions_andreibelous16.egg-info/top_level.txt
+-rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)      292 2024-05-30 01:19:18.000000 myfunctions_andreibelous16-0.0.3/myfunctions_andreibelous16.egg-info/SOURCES.txt
+-rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)        1 2024-05-30 01:19:18.000000 myfunctions_andreibelous16-0.0.3/myfunctions_andreibelous16.egg-info/dependency_links.txt
+-rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)     2852 2024-05-30 01:19:18.000000 myfunctions_andreibelous16-0.0.3/myfunctions_andreibelous16.egg-info/PKG-INFO
+drwxrwxr-x   0 Andreibelous16  (1709) Andreibelous16  (1710)        0 2024-05-30 01:19:18.000000 myfunctions_andreibelous16-0.0.3/myfunctions_andreibelous16/
+-rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)      175 2024-05-30 01:12:57.000000 myfunctions_andreibelous16-0.0.3/myfunctions_andreibelous16/math.py
+-rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)        0 2024-05-30 00:48:50.000000 myfunctions_andreibelous16-0.0.3/myfunctions_andreibelous16/__init__.py
+-rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)     2394 2024-05-30 01:18:43.000000 myfunctions_andreibelous16-0.0.3/README.md
+-rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)     2852 2024-05-30 01:19:18.000000 myfunctions_andreibelous16-0.0.3/PKG-INFO
+-rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)       38 2024-05-30 01:19:18.000000 myfunctions_andreibelous16-0.0.3/setup.cfg
```

### Comparing `myfunctions_andreibelous16-0.0.2/setup.py` & `myfunctions_andreibelous16-0.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_andreibelous16',
-    version='0.0.2',
+    version='0.0.3',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/Andreibelous16',
     license='MIT',
     author='Andrei Belous',
     author_email='andrewbelousit@gmail.com',
     description='A description of your package',
```

