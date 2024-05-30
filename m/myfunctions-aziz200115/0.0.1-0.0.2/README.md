# Comparing `tmp/myfunctions_aziz200115-0.0.1.tar.gz` & `tmp/myfunctions_aziz200115-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/aziz200115/python-class/evolvecyber/class5/dist/tmpykpxh38a/myfunctions_aziz200115-0.0.1.tar", last modified: Thu May 30 01:04:12 2024, max compression
+gzip compressed data, was "/mnt/aziz200115/python-class/evolvecyber/class5/dist/tmp5hc2nczf/myfunctions_aziz200115-0.0.2.tar", last modified: Thu May 30 01:14:20 2024, max compression
```

## Comparing `myfunctions_aziz200115-0.0.1.tar` & `myfunctions_aziz200115-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 aziz200115  (1619) aziz200115  (1620)        0 2024-05-30 01:04:12.000000 myfunctions_aziz200115-0.0.1/
--rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)      642 2024-05-30 01:02:25.000000 myfunctions_aziz200115-0.0.1/setup.py
-drwxrwxr-x   0 aziz200115  (1619) aziz200115  (1620)        0 2024-05-30 01:04:12.000000 myfunctions_aziz200115-0.0.1/myfunctions_aziz200115/
--rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)      110 2024-05-30 00:54:51.000000 myfunctions_aziz200115-0.0.1/myfunctions_aziz200115/math.py
--rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)        0 2024-05-30 00:48:59.000000 myfunctions_aziz200115-0.0.1/myfunctions_aziz200115/__init__.py
--rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)        0 2024-05-30 00:48:22.000000 myfunctions_aziz200115-0.0.1/README.md
--rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)      458 2024-05-30 01:04:12.000000 myfunctions_aziz200115-0.0.1/PKG-INFO
--rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)       38 2024-05-30 01:04:12.000000 myfunctions_aziz200115-0.0.1/setup.cfg
-drwxrwxr-x   0 aziz200115  (1619) aziz200115  (1620)        0 2024-05-30 01:04:12.000000 myfunctions_aziz200115-0.0.1/myfunctions_aziz200115.egg-info/
--rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)       23 2024-05-30 01:04:12.000000 myfunctions_aziz200115-0.0.1/myfunctions_aziz200115.egg-info/top_level.txt
--rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)      268 2024-05-30 01:04:12.000000 myfunctions_aziz200115-0.0.1/myfunctions_aziz200115.egg-info/SOURCES.txt
--rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)        1 2024-05-30 01:04:12.000000 myfunctions_aziz200115-0.0.1/myfunctions_aziz200115.egg-info/dependency_links.txt
--rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)      458 2024-05-30 01:04:12.000000 myfunctions_aziz200115-0.0.1/myfunctions_aziz200115.egg-info/PKG-INFO
+drwxrwxr-x   0 aziz200115  (1619) aziz200115  (1620)        0 2024-05-30 01:14:20.000000 myfunctions_aziz200115-0.0.2/
+-rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)      642 2024-05-30 01:12:58.000000 myfunctions_aziz200115-0.0.2/setup.py
+drwxrwxr-x   0 aziz200115  (1619) aziz200115  (1620)        0 2024-05-30 01:14:20.000000 myfunctions_aziz200115-0.0.2/myfunctions_aziz200115/
+-rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)      184 2024-05-30 01:12:44.000000 myfunctions_aziz200115-0.0.2/myfunctions_aziz200115/math.py
+-rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)        0 2024-05-30 00:48:59.000000 myfunctions_aziz200115-0.0.2/myfunctions_aziz200115/__init__.py
+-rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)        0 2024-05-30 00:48:22.000000 myfunctions_aziz200115-0.0.2/README.md
+-rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)      458 2024-05-30 01:14:20.000000 myfunctions_aziz200115-0.0.2/PKG-INFO
+-rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)       38 2024-05-30 01:14:20.000000 myfunctions_aziz200115-0.0.2/setup.cfg
+drwxrwxr-x   0 aziz200115  (1619) aziz200115  (1620)        0 2024-05-30 01:14:20.000000 myfunctions_aziz200115-0.0.2/myfunctions_aziz200115.egg-info/
+-rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)       23 2024-05-30 01:14:20.000000 myfunctions_aziz200115-0.0.2/myfunctions_aziz200115.egg-info/top_level.txt
+-rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)      268 2024-05-30 01:14:20.000000 myfunctions_aziz200115-0.0.2/myfunctions_aziz200115.egg-info/SOURCES.txt
+-rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)        1 2024-05-30 01:14:20.000000 myfunctions_aziz200115-0.0.2/myfunctions_aziz200115.egg-info/dependency_links.txt
+-rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)      458 2024-05-30 01:14:20.000000 myfunctions_aziz200115-0.0.2/myfunctions_aziz200115.egg-info/PKG-INFO
```

### Comparing `myfunctions_aziz200115-0.0.1/setup.py` & `myfunctions_aziz200115-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_aziz200115',
-    version='0.0.1',
+    version='0.0.2',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/aziz200115/',
     license='MIT',
     author='Aziz Shekerbekov',
     author_email='awekerbekov@gmail.com',
     description='A description of your package',
```

