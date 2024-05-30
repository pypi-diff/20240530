# Comparing `tmp/myfunctions_SashaKrav-0.0.1.tar.gz` & `tmp/myfunctions_SashaKrav-0.0.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/SashaKrav/Python-class/class5/dist/tmp35biox3j/myfunctions_SashaKrav-0.0.1.tar", last modified: Thu May 30 00:58:43 2024, max compression
+gzip compressed data, was "/mnt/SashaKrav/Python-class/class5/dist/tmpawn51ngz/myfunctions_SashaKrav-0.0.10.tar", last modified: Thu May 30 01:14:14 2024, max compression
```

## Comparing `myfunctions_SashaKrav-0.0.1.tar` & `myfunctions_SashaKrav-0.0.10.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 SashaKrav  (1628) SashaKrav  (1629)        0 2024-05-30 00:58:43.000000 myfunctions_SashaKrav-0.0.1/
--rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)      611 2024-05-30 00:58:02.000000 myfunctions_SashaKrav-0.0.1/setup.py
-drwxrwxr-x   0 SashaKrav  (1628) SashaKrav  (1629)        0 2024-05-30 00:58:43.000000 myfunctions_SashaKrav-0.0.1/myfunctions_SashaKrav.egg-info/
--rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)        1 2024-05-30 00:58:43.000000 myfunctions_SashaKrav-0.0.1/myfunctions_SashaKrav.egg-info/top_level.txt
--rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)      198 2024-05-30 00:58:43.000000 myfunctions_SashaKrav-0.0.1/myfunctions_SashaKrav.egg-info/SOURCES.txt
--rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)        1 2024-05-30 00:58:43.000000 myfunctions_SashaKrav-0.0.1/myfunctions_SashaKrav.egg-info/dependency_links.txt
--rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)      427 2024-05-30 00:58:43.000000 myfunctions_SashaKrav-0.0.1/myfunctions_SashaKrav.egg-info/PKG-INFO
--rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)        0 2024-05-30 00:48:28.000000 myfunctions_SashaKrav-0.0.1/README.md
--rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)      427 2024-05-30 00:58:43.000000 myfunctions_SashaKrav-0.0.1/PKG-INFO
--rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)       38 2024-05-30 00:58:43.000000 myfunctions_SashaKrav-0.0.1/setup.cfg
+drwxrwxr-x   0 SashaKrav  (1628) SashaKrav  (1629)        0 2024-05-30 01:14:14.000000 myfunctions_SashaKrav-0.0.10/
+-rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)      631 2024-05-30 01:13:53.000000 myfunctions_SashaKrav-0.0.10/setup.py
+drwxrwxr-x   0 SashaKrav  (1628) SashaKrav  (1629)        0 2024-05-30 01:14:14.000000 myfunctions_SashaKrav-0.0.10/myfunctions_SashaKrav.egg-info/
+-rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)        1 2024-05-30 01:14:14.000000 myfunctions_SashaKrav-0.0.10/myfunctions_SashaKrav.egg-info/top_level.txt
+-rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)      198 2024-05-30 01:14:14.000000 myfunctions_SashaKrav-0.0.10/myfunctions_SashaKrav.egg-info/SOURCES.txt
+-rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)        1 2024-05-30 01:14:14.000000 myfunctions_SashaKrav-0.0.10/myfunctions_SashaKrav.egg-info/dependency_links.txt
+-rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)      447 2024-05-30 01:14:14.000000 myfunctions_SashaKrav-0.0.10/myfunctions_SashaKrav.egg-info/PKG-INFO
+-rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)        0 2024-05-30 00:48:28.000000 myfunctions_SashaKrav-0.0.10/README.md
+-rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)      447 2024-05-30 01:14:14.000000 myfunctions_SashaKrav-0.0.10/PKG-INFO
+-rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)       38 2024-05-30 01:14:14.000000 myfunctions_SashaKrav-0.0.10/setup.cfg
```

### Comparing `myfunctions_SashaKrav-0.0.1/setup.py` & `myfunctions_SashaKrav-0.0.10/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_SashaKrav',
-    version='0.0.1',
+    version='0.0.10',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/SashaKrav',
     license='MIT',
     author='SashaKrav',
-    author_email='',
+    author_email='kravcov4k@gmail.com',
     description='A description of your package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
```

