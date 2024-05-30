# Comparing `tmp/myfunctions_aziz200115-0.0.6.tar.gz` & `tmp/myfunctions_aziz200115-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/aziz200115/python-class/evolvecyber/class5/dist/tmp9_zz1bhw/myfunctions_aziz200115-0.0.6.tar", last modified: Thu May 30 01:36:08 2024, max compression
+gzip compressed data, was "/mnt/aziz200115/python-class/evolvecyber/class5/dist/tmp9bcxtuoz/myfunctions_aziz200115-0.0.7.tar", last modified: Thu May 30 17:08:53 2024, max compression
```

## Comparing `myfunctions_aziz200115-0.0.6.tar` & `myfunctions_aziz200115-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 aziz200115  (1619) aziz200115  (1620)        0 2024-05-30 01:36:08.000000 myfunctions_aziz200115-0.0.6/
--rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)      642 2024-05-30 01:35:58.000000 myfunctions_aziz200115-0.0.6/setup.py
-drwxrwxr-x   0 aziz200115  (1619) aziz200115  (1620)        0 2024-05-30 01:36:08.000000 myfunctions_aziz200115-0.0.6/myfunctions_aziz200115/
--rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)      442 2024-05-30 01:31:10.000000 myfunctions_aziz200115-0.0.6/myfunctions_aziz200115/math.py
--rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)        0 2024-05-30 00:48:59.000000 myfunctions_aziz200115-0.0.6/myfunctions_aziz200115/__init__.py
--rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)      771 2024-05-30 01:19:26.000000 myfunctions_aziz200115-0.0.6/README.md
--rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)     1222 2024-05-30 01:36:08.000000 myfunctions_aziz200115-0.0.6/PKG-INFO
--rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)       38 2024-05-30 01:36:08.000000 myfunctions_aziz200115-0.0.6/setup.cfg
-drwxrwxr-x   0 aziz200115  (1619) aziz200115  (1620)        0 2024-05-30 01:36:08.000000 myfunctions_aziz200115-0.0.6/myfunctions_aziz200115.egg-info/
--rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)       23 2024-05-30 01:36:08.000000 myfunctions_aziz200115-0.0.6/myfunctions_aziz200115.egg-info/top_level.txt
--rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)      268 2024-05-30 01:36:08.000000 myfunctions_aziz200115-0.0.6/myfunctions_aziz200115.egg-info/SOURCES.txt
--rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)        1 2024-05-30 01:36:08.000000 myfunctions_aziz200115-0.0.6/myfunctions_aziz200115.egg-info/dependency_links.txt
--rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)     1222 2024-05-30 01:36:08.000000 myfunctions_aziz200115-0.0.6/myfunctions_aziz200115.egg-info/PKG-INFO
+drwxrwxr-x   0 aziz200115  (1619) aziz200115  (1620)        0 2024-05-30 17:08:53.000000 myfunctions_aziz200115-0.0.7/
+-rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)      642 2024-05-30 17:04:07.000000 myfunctions_aziz200115-0.0.7/setup.py
+drwxrwxr-x   0 aziz200115  (1619) aziz200115  (1620)        0 2024-05-30 17:08:53.000000 myfunctions_aziz200115-0.0.7/myfunctions_aziz200115/
+-rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)      584 2024-05-30 17:05:04.000000 myfunctions_aziz200115-0.0.7/myfunctions_aziz200115/math.py
+-rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)        0 2024-05-30 00:48:59.000000 myfunctions_aziz200115-0.0.7/myfunctions_aziz200115/__init__.py
+-rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)      207 2024-05-30 17:07:05.000000 myfunctions_aziz200115-0.0.7/README.md
+-rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)      658 2024-05-30 17:08:53.000000 myfunctions_aziz200115-0.0.7/PKG-INFO
+-rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)       38 2024-05-30 17:08:53.000000 myfunctions_aziz200115-0.0.7/setup.cfg
+drwxrwxr-x   0 aziz200115  (1619) aziz200115  (1620)        0 2024-05-30 17:08:53.000000 myfunctions_aziz200115-0.0.7/myfunctions_aziz200115.egg-info/
+-rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)       23 2024-05-30 17:08:53.000000 myfunctions_aziz200115-0.0.7/myfunctions_aziz200115.egg-info/top_level.txt
+-rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)      268 2024-05-30 17:08:53.000000 myfunctions_aziz200115-0.0.7/myfunctions_aziz200115.egg-info/SOURCES.txt
+-rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)        1 2024-05-30 17:08:52.000000 myfunctions_aziz200115-0.0.7/myfunctions_aziz200115.egg-info/dependency_links.txt
+-rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)      658 2024-05-30 17:08:52.000000 myfunctions_aziz200115-0.0.7/myfunctions_aziz200115.egg-info/PKG-INFO
```

### Comparing `myfunctions_aziz200115-0.0.6/setup.py` & `myfunctions_aziz200115-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_aziz200115',
-    version='0.0.6',
+    version='0.0.7',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/aziz200115/',
     license='MIT',
     author='Aziz Shekerbekov',
     author_email='awekerbekov@gmail.com',
     description='A description of your package',
```

