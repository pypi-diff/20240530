# Comparing `tmp/myfunctions_diana11d-0.0.0.tar.gz` & `tmp/myfunctions_diana11d-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/Diana11d/python-class/evolvecyber/class5/dist/tmplc7qsau4/myfunctions_diana11d-0.0.0.tar", last modified: Thu May 30 00:57:44 2024, max compression
+gzip compressed data, was "/mnt/Diana11d/python-class/evolvecyber/class5/dist/tmp8dfi44wq/myfunctions_diana11d-0.0.1.tar", last modified: Thu May 30 01:18:12 2024, max compression
```

## Comparing `myfunctions_diana11d-0.0.0.tar` & `myfunctions_diana11d-0.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 Diana11d  (1693) Diana11d  (1694)        0 2024-05-30 00:57:44.000000 myfunctions_diana11d-0.0.0/
--rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)      636 2024-05-30 00:57:08.000000 myfunctions_diana11d-0.0.0/setup.py
-drwxrwxr-x   0 Diana11d  (1693) Diana11d  (1694)        0 2024-05-30 00:57:43.000000 myfunctions_diana11d-0.0.0/myfunctions_diana11d/
--rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)      107 2024-05-30 00:54:28.000000 myfunctions_diana11d-0.0.0/myfunctions_diana11d/math.py
--rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)        0 2024-05-30 00:48:46.000000 myfunctions_diana11d-0.0.0/myfunctions_diana11d/__init__.py
--rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)        0 2024-05-30 00:48:23.000000 myfunctions_diana11d-0.0.0/README.md
--rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)      457 2024-05-30 00:57:44.000000 myfunctions_diana11d-0.0.0/PKG-INFO
-drwxrwxr-x   0 Diana11d  (1693) Diana11d  (1694)        0 2024-05-30 00:57:44.000000 myfunctions_diana11d-0.0.0/myfunctions_diana11d.egg-info/
--rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)       21 2024-05-30 00:57:43.000000 myfunctions_diana11d-0.0.0/myfunctions_diana11d.egg-info/top_level.txt
--rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)      256 2024-05-30 00:57:43.000000 myfunctions_diana11d-0.0.0/myfunctions_diana11d.egg-info/SOURCES.txt
--rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)        1 2024-05-30 00:57:43.000000 myfunctions_diana11d-0.0.0/myfunctions_diana11d.egg-info/dependency_links.txt
--rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)      457 2024-05-30 00:57:43.000000 myfunctions_diana11d-0.0.0/myfunctions_diana11d.egg-info/PKG-INFO
--rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)       38 2024-05-30 00:57:44.000000 myfunctions_diana11d-0.0.0/setup.cfg
+drwxrwxr-x   0 Diana11d  (1693) Diana11d  (1694)        0 2024-05-30 01:18:12.000000 myfunctions_diana11d-0.0.1/
+-rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)      641 2024-05-30 01:17:11.000000 myfunctions_diana11d-0.0.1/setup.py
+drwxrwxr-x   0 Diana11d  (1693) Diana11d  (1694)        0 2024-05-30 01:18:12.000000 myfunctions_diana11d-0.0.1/myfunctions_diana11d/
+-rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)      175 2024-05-30 01:15:12.000000 myfunctions_diana11d-0.0.1/myfunctions_diana11d/math.py
+-rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)        0 2024-05-30 00:48:46.000000 myfunctions_diana11d-0.0.1/myfunctions_diana11d/__init__.py
+-rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)        0 2024-05-30 00:48:23.000000 myfunctions_diana11d-0.0.1/README.md
+-rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)      457 2024-05-30 01:18:12.000000 myfunctions_diana11d-0.0.1/PKG-INFO
+drwxrwxr-x   0 Diana11d  (1693) Diana11d  (1694)        0 2024-05-30 01:18:12.000000 myfunctions_diana11d-0.0.1/myfunctions_diana11d.egg-info/
+-rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)       21 2024-05-30 01:18:12.000000 myfunctions_diana11d-0.0.1/myfunctions_diana11d.egg-info/top_level.txt
+-rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)      256 2024-05-30 01:18:12.000000 myfunctions_diana11d-0.0.1/myfunctions_diana11d.egg-info/SOURCES.txt
+-rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)        1 2024-05-30 01:18:12.000000 myfunctions_diana11d-0.0.1/myfunctions_diana11d.egg-info/dependency_links.txt
+-rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)      457 2024-05-30 01:18:12.000000 myfunctions_diana11d-0.0.1/myfunctions_diana11d.egg-info/PKG-INFO
+-rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)       38 2024-05-30 01:18:12.000000 myfunctions_diana11d-0.0.1/setup.cfg
```

### Comparing `myfunctions_diana11d-0.0.0/setup.py` & `myfunctions_diana11d-0.0.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_diana11d',
-    version='',
+    version='0.0.1',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/Diana11d',
     license='MIT',
     author='Diana Dauletkerey',
     author_email='ddauletkerey02@gmail.com',
     description='A description of your package',
```

