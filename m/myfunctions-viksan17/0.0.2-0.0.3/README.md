# Comparing `tmp/myfunctions_viksan17-0.0.2.tar.gz` & `tmp/myfunctions_viksan17-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/viksan17/python-class/class5/dist/tmprhwwau8y/myfunctions_viksan17-0.0.2.tar", last modified: Thu May 30 01:12:54 2024, max compression
+gzip compressed data, was "/mnt/viksan17/python-class/class5/dist/tmpu0_go8f1/myfunctions_viksan17-0.0.3.tar", last modified: Thu May 30 01:19:14 2024, max compression
```

## Comparing `myfunctions_viksan17-0.0.2.tar` & `myfunctions_viksan17-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 viksan17  (1704) viksan17  (1705)        0 2024-05-30 01:12:54.000000 myfunctions_viksan17-0.0.2/
--rw-rw-r--   0 viksan17  (1704) viksan17  (1705)      636 2024-05-30 01:12:26.000000 myfunctions_viksan17-0.0.2/setup.py
-drwxrwxr-x   0 viksan17  (1704) viksan17  (1705)        0 2024-05-30 01:12:54.000000 myfunctions_viksan17-0.0.2/myfunctions_viksan17.egg-info/
--rw-rw-r--   0 viksan17  (1704) viksan17  (1705)       21 2024-05-30 01:12:54.000000 myfunctions_viksan17-0.0.2/myfunctions_viksan17.egg-info/top_level.txt
--rw-rw-r--   0 viksan17  (1704) viksan17  (1705)      256 2024-05-30 01:12:54.000000 myfunctions_viksan17-0.0.2/myfunctions_viksan17.egg-info/SOURCES.txt
--rw-rw-r--   0 viksan17  (1704) viksan17  (1705)        1 2024-05-30 01:12:54.000000 myfunctions_viksan17-0.0.2/myfunctions_viksan17.egg-info/dependency_links.txt
--rw-rw-r--   0 viksan17  (1704) viksan17  (1705)      452 2024-05-30 01:12:54.000000 myfunctions_viksan17-0.0.2/myfunctions_viksan17.egg-info/PKG-INFO
-drwxrwxr-x   0 viksan17  (1704) viksan17  (1705)        0 2024-05-30 01:12:54.000000 myfunctions_viksan17-0.0.2/myfunctions_viksan17/
--rw-rw-r--   0 viksan17  (1704) viksan17  (1705)      175 2024-05-30 01:12:12.000000 myfunctions_viksan17-0.0.2/myfunctions_viksan17/math.py
--rw-rw-r--   0 viksan17  (1704) viksan17  (1705)        0 2024-05-30 00:48:44.000000 myfunctions_viksan17-0.0.2/myfunctions_viksan17/__init__.py
--rw-rw-r--   0 viksan17  (1704) viksan17  (1705)        0 2024-05-30 00:48:24.000000 myfunctions_viksan17-0.0.2/README.md
--rw-rw-r--   0 viksan17  (1704) viksan17  (1705)      452 2024-05-30 01:12:54.000000 myfunctions_viksan17-0.0.2/PKG-INFO
--rw-rw-r--   0 viksan17  (1704) viksan17  (1705)       38 2024-05-30 01:12:54.000000 myfunctions_viksan17-0.0.2/setup.cfg
+drwxrwxr-x   0 viksan17  (1704) viksan17  (1705)        0 2024-05-30 01:19:14.000000 myfunctions_viksan17-0.0.3/
+-rw-rw-r--   0 viksan17  (1704) viksan17  (1705)      636 2024-05-30 01:18:52.000000 myfunctions_viksan17-0.0.3/setup.py
+drwxrwxr-x   0 viksan17  (1704) viksan17  (1705)        0 2024-05-30 01:19:14.000000 myfunctions_viksan17-0.0.3/myfunctions_viksan17.egg-info/
+-rw-rw-r--   0 viksan17  (1704) viksan17  (1705)       21 2024-05-30 01:19:14.000000 myfunctions_viksan17-0.0.3/myfunctions_viksan17.egg-info/top_level.txt
+-rw-rw-r--   0 viksan17  (1704) viksan17  (1705)      256 2024-05-30 01:19:14.000000 myfunctions_viksan17-0.0.3/myfunctions_viksan17.egg-info/SOURCES.txt
+-rw-rw-r--   0 viksan17  (1704) viksan17  (1705)        1 2024-05-30 01:19:14.000000 myfunctions_viksan17-0.0.3/myfunctions_viksan17.egg-info/dependency_links.txt
+-rw-rw-r--   0 viksan17  (1704) viksan17  (1705)     2243 2024-05-30 01:19:14.000000 myfunctions_viksan17-0.0.3/myfunctions_viksan17.egg-info/PKG-INFO
+drwxrwxr-x   0 viksan17  (1704) viksan17  (1705)        0 2024-05-30 01:19:14.000000 myfunctions_viksan17-0.0.3/myfunctions_viksan17/
+-rw-rw-r--   0 viksan17  (1704) viksan17  (1705)      175 2024-05-30 01:12:12.000000 myfunctions_viksan17-0.0.3/myfunctions_viksan17/math.py
+-rw-rw-r--   0 viksan17  (1704) viksan17  (1705)        0 2024-05-30 00:48:44.000000 myfunctions_viksan17-0.0.3/myfunctions_viksan17/__init__.py
+-rw-rw-r--   0 viksan17  (1704) viksan17  (1705)     1798 2024-05-30 01:18:46.000000 myfunctions_viksan17-0.0.3/README.md
+-rw-rw-r--   0 viksan17  (1704) viksan17  (1705)     2243 2024-05-30 01:19:14.000000 myfunctions_viksan17-0.0.3/PKG-INFO
+-rw-rw-r--   0 viksan17  (1704) viksan17  (1705)       38 2024-05-30 01:19:14.000000 myfunctions_viksan17-0.0.3/setup.cfg
```

### Comparing `myfunctions_viksan17-0.0.2/setup.py` & `myfunctions_viksan17-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_viksan17',
-    version='0.0.2',
+    version='0.0.3',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/viksan17/',
     license='MIT',
     author='Victor Sanabria',
     author_email='vicsanab92@gmail.com',
     description='A description of your package',
```

