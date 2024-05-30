# Comparing `tmp/myfunctions_andreibelous16-0.0.1.tar.gz` & `tmp/myfunctions_andreibelous16-0.0.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/Andreibelous16/python_class/evolvecyber/class5/dist/tmptcojd_jw/myfunctions_andreibelous16-0.0.1.tar", last modified: Thu May 30 00:58:39 2024, max compression
+gzip compressed data, was "/mnt/Andreibelous16/python_class/evolvecyber/class5/dist/tmpns6rzdkm/myfunctions_andreibelous16-0.0.10.tar", last modified: Thu May 30 01:13:09 2024, max compression
```

## Comparing `myfunctions_andreibelous16-0.0.1.tar` & `myfunctions_andreibelous16-0.0.10.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 Andreibelous16  (1709) Andreibelous16  (1710)        0 2024-05-30 00:58:39.000000 myfunctions_andreibelous16-0.0.1/
--rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)      649 2024-05-30 00:57:42.000000 myfunctions_andreibelous16-0.0.1/setup.py
-drwxrwxr-x   0 Andreibelous16  (1709) Andreibelous16  (1710)        0 2024-05-30 00:58:39.000000 myfunctions_andreibelous16-0.0.1/myfunctions_andreibelous16.egg-info/
--rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)       27 2024-05-30 00:58:39.000000 myfunctions_andreibelous16-0.0.1/myfunctions_andreibelous16.egg-info/top_level.txt
--rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)      292 2024-05-30 00:58:39.000000 myfunctions_andreibelous16-0.0.1/myfunctions_andreibelous16.egg-info/SOURCES.txt
--rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)        1 2024-05-30 00:58:39.000000 myfunctions_andreibelous16-0.0.1/myfunctions_andreibelous16.egg-info/dependency_links.txt
--rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)      465 2024-05-30 00:58:39.000000 myfunctions_andreibelous16-0.0.1/myfunctions_andreibelous16.egg-info/PKG-INFO
-drwxrwxr-x   0 Andreibelous16  (1709) Andreibelous16  (1710)        0 2024-05-30 00:58:39.000000 myfunctions_andreibelous16-0.0.1/myfunctions_andreibelous16/
--rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)      106 2024-05-30 00:54:34.000000 myfunctions_andreibelous16-0.0.1/myfunctions_andreibelous16/math.py
--rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)        0 2024-05-30 00:48:50.000000 myfunctions_andreibelous16-0.0.1/myfunctions_andreibelous16/__init__.py
--rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)        0 2024-05-30 00:48:27.000000 myfunctions_andreibelous16-0.0.1/README.md
--rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)      465 2024-05-30 00:58:39.000000 myfunctions_andreibelous16-0.0.1/PKG-INFO
--rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)       38 2024-05-30 00:58:39.000000 myfunctions_andreibelous16-0.0.1/setup.cfg
+drwxrwxr-x   0 Andreibelous16  (1709) Andreibelous16  (1710)        0 2024-05-30 01:13:09.000000 myfunctions_andreibelous16-0.0.10/
+-rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)      650 2024-05-30 01:12:40.000000 myfunctions_andreibelous16-0.0.10/setup.py
+drwxrwxr-x   0 Andreibelous16  (1709) Andreibelous16  (1710)        0 2024-05-30 01:13:09.000000 myfunctions_andreibelous16-0.0.10/myfunctions_andreibelous16.egg-info/
+-rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)       27 2024-05-30 01:13:09.000000 myfunctions_andreibelous16-0.0.10/myfunctions_andreibelous16.egg-info/top_level.txt
+-rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)      292 2024-05-30 01:13:09.000000 myfunctions_andreibelous16-0.0.10/myfunctions_andreibelous16.egg-info/SOURCES.txt
+-rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)        1 2024-05-30 01:13:09.000000 myfunctions_andreibelous16-0.0.10/myfunctions_andreibelous16.egg-info/dependency_links.txt
+-rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)      466 2024-05-30 01:13:09.000000 myfunctions_andreibelous16-0.0.10/myfunctions_andreibelous16.egg-info/PKG-INFO
+drwxrwxr-x   0 Andreibelous16  (1709) Andreibelous16  (1710)        0 2024-05-30 01:13:09.000000 myfunctions_andreibelous16-0.0.10/myfunctions_andreibelous16/
+-rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)      175 2024-05-30 01:12:57.000000 myfunctions_andreibelous16-0.0.10/myfunctions_andreibelous16/math.py
+-rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)        0 2024-05-30 00:48:50.000000 myfunctions_andreibelous16-0.0.10/myfunctions_andreibelous16/__init__.py
+-rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)        0 2024-05-30 00:48:27.000000 myfunctions_andreibelous16-0.0.10/README.md
+-rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)      466 2024-05-30 01:13:09.000000 myfunctions_andreibelous16-0.0.10/PKG-INFO
+-rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)       38 2024-05-30 01:13:09.000000 myfunctions_andreibelous16-0.0.10/setup.cfg
```

### Comparing `myfunctions_andreibelous16-0.0.1/setup.py` & `myfunctions_andreibelous16-0.0.10/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_andreibelous16',
-    version='0.0.1',
+    version='0.0.10',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/Andreibelous16',
     license='MIT',
     author='Andrei Belous',
     author_email='andrewbelousit@gmail.com',
     description='A description of your package',
```

