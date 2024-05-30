# Comparing `tmp/myfunctions_echervenko-0.0.1.tar.gz` & `tmp/myfunctions_echervenko-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/echervenko/python-class/evolvecyber/Class5/dist/tmpnss4euau/myfunctions_echervenko-0.0.1.tar", last modified: Thu May 30 00:58:39 2024, max compression
+gzip compressed data, was "/mnt/echervenko/python-class/evolvecyber/Class5/dist/tmpyl1jz7q6/myfunctions_echervenko-0.0.2.tar", last modified: Thu May 30 01:13:51 2024, max compression
```

## Comparing `myfunctions_echervenko-0.0.1.tar` & `myfunctions_echervenko-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 echervenko  (1636) echervenko  (1637)        0 2024-05-30 00:58:39.000000 myfunctions_echervenko-0.0.1/
-drwxrwxr-x   0 echervenko  (1636) echervenko  (1637)        0 2024-05-30 00:58:39.000000 myfunctions_echervenko-0.0.1/myfunctions_echervenko/
--rw-rw-r--   0 echervenko  (1636) echervenko  (1637)      103 2024-05-30 00:54:58.000000 myfunctions_echervenko-0.0.1/myfunctions_echervenko/math.py
--rw-rw-r--   0 echervenko  (1636) echervenko  (1637)        0 2024-05-30 00:48:50.000000 myfunctions_echervenko-0.0.1/myfunctions_echervenko/__init__.py
--rw-rw-r--   0 echervenko  (1636) echervenko  (1637)      643 2024-05-30 00:57:25.000000 myfunctions_echervenko-0.0.1/setup.py
-drwxrwxr-x   0 echervenko  (1636) echervenko  (1637)        0 2024-05-30 00:58:39.000000 myfunctions_echervenko-0.0.1/myfunctions_echervenko.egg-info/
--rw-rw-r--   0 echervenko  (1636) echervenko  (1637)       23 2024-05-30 00:58:39.000000 myfunctions_echervenko-0.0.1/myfunctions_echervenko.egg-info/top_level.txt
--rw-rw-r--   0 echervenko  (1636) echervenko  (1637)      268 2024-05-30 00:58:39.000000 myfunctions_echervenko-0.0.1/myfunctions_echervenko.egg-info/SOURCES.txt
--rw-rw-r--   0 echervenko  (1636) echervenko  (1637)        1 2024-05-30 00:58:39.000000 myfunctions_echervenko-0.0.1/myfunctions_echervenko.egg-info/dependency_links.txt
--rw-rw-r--   0 echervenko  (1636) echervenko  (1637)      459 2024-05-30 00:58:39.000000 myfunctions_echervenko-0.0.1/myfunctions_echervenko.egg-info/PKG-INFO
--rw-rw-r--   0 echervenko  (1636) echervenko  (1637)        0 2024-05-30 00:48:28.000000 myfunctions_echervenko-0.0.1/README.md
--rw-rw-r--   0 echervenko  (1636) echervenko  (1637)      459 2024-05-30 00:58:39.000000 myfunctions_echervenko-0.0.1/PKG-INFO
--rw-rw-r--   0 echervenko  (1636) echervenko  (1637)       38 2024-05-30 00:58:39.000000 myfunctions_echervenko-0.0.1/setup.cfg
+drwxrwxr-x   0 echervenko  (1636) echervenko  (1637)        0 2024-05-30 01:13:51.000000 myfunctions_echervenko-0.0.2/
+drwxrwxr-x   0 echervenko  (1636) echervenko  (1637)        0 2024-05-30 01:13:51.000000 myfunctions_echervenko-0.0.2/myfunctions_echervenko/
+-rw-rw-r--   0 echervenko  (1636) echervenko  (1637)      170 2024-05-30 01:12:35.000000 myfunctions_echervenko-0.0.2/myfunctions_echervenko/math.py
+-rw-rw-r--   0 echervenko  (1636) echervenko  (1637)        0 2024-05-30 00:48:50.000000 myfunctions_echervenko-0.0.2/myfunctions_echervenko/__init__.py
+-rw-rw-r--   0 echervenko  (1636) echervenko  (1637)      643 2024-05-30 01:13:01.000000 myfunctions_echervenko-0.0.2/setup.py
+drwxrwxr-x   0 echervenko  (1636) echervenko  (1637)        0 2024-05-30 01:13:51.000000 myfunctions_echervenko-0.0.2/myfunctions_echervenko.egg-info/
+-rw-rw-r--   0 echervenko  (1636) echervenko  (1637)       23 2024-05-30 01:13:51.000000 myfunctions_echervenko-0.0.2/myfunctions_echervenko.egg-info/top_level.txt
+-rw-rw-r--   0 echervenko  (1636) echervenko  (1637)      268 2024-05-30 01:13:51.000000 myfunctions_echervenko-0.0.2/myfunctions_echervenko.egg-info/SOURCES.txt
+-rw-rw-r--   0 echervenko  (1636) echervenko  (1637)        1 2024-05-30 01:13:51.000000 myfunctions_echervenko-0.0.2/myfunctions_echervenko.egg-info/dependency_links.txt
+-rw-rw-r--   0 echervenko  (1636) echervenko  (1637)      459 2024-05-30 01:13:51.000000 myfunctions_echervenko-0.0.2/myfunctions_echervenko.egg-info/PKG-INFO
+-rw-rw-r--   0 echervenko  (1636) echervenko  (1637)        0 2024-05-30 00:48:28.000000 myfunctions_echervenko-0.0.2/README.md
+-rw-rw-r--   0 echervenko  (1636) echervenko  (1637)      459 2024-05-30 01:13:51.000000 myfunctions_echervenko-0.0.2/PKG-INFO
+-rw-rw-r--   0 echervenko  (1636) echervenko  (1637)       38 2024-05-30 01:13:51.000000 myfunctions_echervenko-0.0.2/setup.cfg
```

### Comparing `myfunctions_echervenko-0.0.1/setup.py` & `myfunctions_echervenko-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_echervenko',
-    version='0.0.1',
+    version='0.0.2',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/echervenko',
     license='MIT',
     author='Elena Chervenko',
     author_email='chervenkoelena@gmail.com',
     description='A description of your package',
```

