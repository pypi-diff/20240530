# Comparing `tmp/myfunctions_nadiaconeaev89-0.0.2.tar.gz` & `tmp/myfunctions_nadiaconeaev89-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/nadiaconeaev89/python-class/evolvecyber/Class5/dist/tmpmjwz9381/myfunctions_nadiaconeaev89-0.0.2.tar", last modified: Thu May 30 01:14:13 2024, max compression
+gzip compressed data, was "/mnt/nadiaconeaev89/python-class/evolvecyber/Class5/dist/tmplbw7s7e_/myfunctions_nadiaconeaev89-0.0.3.tar", last modified: Thu May 30 01:19:22 2024, max compression
```

## Comparing `myfunctions_nadiaconeaev89-0.0.2.tar` & `myfunctions_nadiaconeaev89-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 01:14:13.000000 myfunctions_nadiaconeaev89-0.0.2/
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      651 2024-05-30 01:13:56.000000 myfunctions_nadiaconeaev89-0.0.2/setup.py
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 00:48:31.000000 myfunctions_nadiaconeaev89-0.0.2/README.md
-drwxrwxr-x   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 01:14:13.000000 myfunctions_nadiaconeaev89-0.0.2/myfunctions_nadiaconeaev89/
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      177 2024-05-30 01:13:35.000000 myfunctions_nadiaconeaev89-0.0.2/myfunctions_nadiaconeaev89/math.py
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 00:48:55.000000 myfunctions_nadiaconeaev89-0.0.2/myfunctions_nadiaconeaev89/__init__.py
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      467 2024-05-30 01:14:13.000000 myfunctions_nadiaconeaev89-0.0.2/PKG-INFO
-drwxrwxr-x   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 01:14:13.000000 myfunctions_nadiaconeaev89-0.0.2/myfunctions_nadiaconeaev89.egg-info/
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)       27 2024-05-30 01:14:13.000000 myfunctions_nadiaconeaev89-0.0.2/myfunctions_nadiaconeaev89.egg-info/top_level.txt
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      292 2024-05-30 01:14:13.000000 myfunctions_nadiaconeaev89-0.0.2/myfunctions_nadiaconeaev89.egg-info/SOURCES.txt
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        1 2024-05-30 01:14:13.000000 myfunctions_nadiaconeaev89-0.0.2/myfunctions_nadiaconeaev89.egg-info/dependency_links.txt
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      467 2024-05-30 01:14:13.000000 myfunctions_nadiaconeaev89-0.0.2/myfunctions_nadiaconeaev89.egg-info/PKG-INFO
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)       38 2024-05-30 01:14:13.000000 myfunctions_nadiaconeaev89-0.0.2/setup.cfg
+drwxrwxr-x   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 01:19:22.000000 myfunctions_nadiaconeaev89-0.0.3/
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      651 2024-05-30 01:19:03.000000 myfunctions_nadiaconeaev89-0.0.3/setup.py
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)     2398 2024-05-30 01:18:52.000000 myfunctions_nadiaconeaev89-0.0.3/README.md
+drwxrwxr-x   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 01:19:22.000000 myfunctions_nadiaconeaev89-0.0.3/myfunctions_nadiaconeaev89/
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      177 2024-05-30 01:13:35.000000 myfunctions_nadiaconeaev89-0.0.3/myfunctions_nadiaconeaev89/math.py
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 00:48:55.000000 myfunctions_nadiaconeaev89-0.0.3/myfunctions_nadiaconeaev89/__init__.py
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)     2858 2024-05-30 01:19:22.000000 myfunctions_nadiaconeaev89-0.0.3/PKG-INFO
+drwxrwxr-x   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 01:19:22.000000 myfunctions_nadiaconeaev89-0.0.3/myfunctions_nadiaconeaev89.egg-info/
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)       27 2024-05-30 01:19:22.000000 myfunctions_nadiaconeaev89-0.0.3/myfunctions_nadiaconeaev89.egg-info/top_level.txt
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      292 2024-05-30 01:19:22.000000 myfunctions_nadiaconeaev89-0.0.3/myfunctions_nadiaconeaev89.egg-info/SOURCES.txt
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        1 2024-05-30 01:19:22.000000 myfunctions_nadiaconeaev89-0.0.3/myfunctions_nadiaconeaev89.egg-info/dependency_links.txt
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)     2858 2024-05-30 01:19:22.000000 myfunctions_nadiaconeaev89-0.0.3/myfunctions_nadiaconeaev89.egg-info/PKG-INFO
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)       38 2024-05-30 01:19:22.000000 myfunctions_nadiaconeaev89-0.0.3/setup.cfg
```

### Comparing `myfunctions_nadiaconeaev89-0.0.2/setup.py` & `myfunctions_nadiaconeaev89-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_nadiaconeaev89',
-    version='0.0.2',
+    version='0.0.3',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/nadiaconeaev89/',
     license='MIT',
     author='Nadejda Coneaev',
     author_email='nadejda.savin@gmail.com',
     description='A description of your package',
```

