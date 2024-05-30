# Comparing `tmp/myfunctions_nadiaconeaev89-0.0.1.tar.gz` & `tmp/myfunctions_nadiaconeaev89-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/nadiaconeaev89/python-class/evolvecyber/Class5/dist/tmpwhytcl8a/myfunctions_nadiaconeaev89-0.0.1.tar", last modified: Thu May 30 00:58:15 2024, max compression
+gzip compressed data, was "/mnt/nadiaconeaev89/python-class/evolvecyber/Class5/dist/tmpmjwz9381/myfunctions_nadiaconeaev89-0.0.2.tar", last modified: Thu May 30 01:14:13 2024, max compression
```

## Comparing `myfunctions_nadiaconeaev89-0.0.1.tar` & `myfunctions_nadiaconeaev89-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 00:58:15.000000 myfunctions_nadiaconeaev89-0.0.1/
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      651 2024-05-30 00:57:49.000000 myfunctions_nadiaconeaev89-0.0.1/setup.py
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 00:48:31.000000 myfunctions_nadiaconeaev89-0.0.1/README.md
-drwxrwxr-x   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 00:58:15.000000 myfunctions_nadiaconeaev89-0.0.1/myfunctions_nadiaconeaev89/
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      109 2024-05-30 00:54:54.000000 myfunctions_nadiaconeaev89-0.0.1/myfunctions_nadiaconeaev89/math.py
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 00:48:55.000000 myfunctions_nadiaconeaev89-0.0.1/myfunctions_nadiaconeaev89/__init__.py
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      467 2024-05-30 00:58:15.000000 myfunctions_nadiaconeaev89-0.0.1/PKG-INFO
-drwxrwxr-x   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 00:58:15.000000 myfunctions_nadiaconeaev89-0.0.1/myfunctions_nadiaconeaev89.egg-info/
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)       27 2024-05-30 00:58:15.000000 myfunctions_nadiaconeaev89-0.0.1/myfunctions_nadiaconeaev89.egg-info/top_level.txt
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      292 2024-05-30 00:58:15.000000 myfunctions_nadiaconeaev89-0.0.1/myfunctions_nadiaconeaev89.egg-info/SOURCES.txt
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        1 2024-05-30 00:58:15.000000 myfunctions_nadiaconeaev89-0.0.1/myfunctions_nadiaconeaev89.egg-info/dependency_links.txt
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      467 2024-05-30 00:58:15.000000 myfunctions_nadiaconeaev89-0.0.1/myfunctions_nadiaconeaev89.egg-info/PKG-INFO
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)       38 2024-05-30 00:58:15.000000 myfunctions_nadiaconeaev89-0.0.1/setup.cfg
+drwxrwxr-x   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 01:14:13.000000 myfunctions_nadiaconeaev89-0.0.2/
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      651 2024-05-30 01:13:56.000000 myfunctions_nadiaconeaev89-0.0.2/setup.py
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 00:48:31.000000 myfunctions_nadiaconeaev89-0.0.2/README.md
+drwxrwxr-x   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 01:14:13.000000 myfunctions_nadiaconeaev89-0.0.2/myfunctions_nadiaconeaev89/
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      177 2024-05-30 01:13:35.000000 myfunctions_nadiaconeaev89-0.0.2/myfunctions_nadiaconeaev89/math.py
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 00:48:55.000000 myfunctions_nadiaconeaev89-0.0.2/myfunctions_nadiaconeaev89/__init__.py
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      467 2024-05-30 01:14:13.000000 myfunctions_nadiaconeaev89-0.0.2/PKG-INFO
+drwxrwxr-x   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 01:14:13.000000 myfunctions_nadiaconeaev89-0.0.2/myfunctions_nadiaconeaev89.egg-info/
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)       27 2024-05-30 01:14:13.000000 myfunctions_nadiaconeaev89-0.0.2/myfunctions_nadiaconeaev89.egg-info/top_level.txt
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      292 2024-05-30 01:14:13.000000 myfunctions_nadiaconeaev89-0.0.2/myfunctions_nadiaconeaev89.egg-info/SOURCES.txt
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        1 2024-05-30 01:14:13.000000 myfunctions_nadiaconeaev89-0.0.2/myfunctions_nadiaconeaev89.egg-info/dependency_links.txt
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      467 2024-05-30 01:14:13.000000 myfunctions_nadiaconeaev89-0.0.2/myfunctions_nadiaconeaev89.egg-info/PKG-INFO
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)       38 2024-05-30 01:14:13.000000 myfunctions_nadiaconeaev89-0.0.2/setup.cfg
```

### Comparing `myfunctions_nadiaconeaev89-0.0.1/setup.py` & `myfunctions_nadiaconeaev89-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_nadiaconeaev89',
-    version='0.0.1',
+    version='0.0.2',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/nadiaconeaev89/',
     license='MIT',
     author='Nadejda Coneaev',
     author_email='nadejda.savin@gmail.com',
     description='A description of your package',
```

