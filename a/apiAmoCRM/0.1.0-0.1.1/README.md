# Comparing `tmp/apiamocrm-0.1.0.tar.gz` & `tmp/apiamocrm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apiamocrm-0.1.0.tar", last modified: Thu May 30 10:04:09 2024, max compression
+gzip compressed data, was "apiamocrm-0.1.1.tar", last modified: Thu May 30 10:13:02 2024, max compression
```

## Comparing `apiamocrm-0.1.0.tar` & `apiamocrm-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 10:04:09.460556 apiamocrm-0.1.0/
--rw-rw-rw-   0        0        0      440 2024-05-30 10:04:09.459560 apiamocrm-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-30 09:48:06.000000 apiamocrm-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 10:04:09.458564 apiamocrm-0.1.0/apiAmoCRM.egg-info/
--rw-rw-rw-   0        0        0      440 2024-05-30 10:04:09.000000 apiamocrm-0.1.0/apiAmoCRM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2024-05-30 10:04:09.000000 apiamocrm-0.1.0/apiAmoCRM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 10:04:09.000000 apiamocrm-0.1.0/apiAmoCRM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-30 10:04:09.000000 apiamocrm-0.1.0/apiAmoCRM.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 10:04:09.000000 apiamocrm-0.1.0/apiAmoCRM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 10:04:09.460556 apiamocrm-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      635 2024-05-30 10:03:59.000000 apiamocrm-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 10:13:02.293902 apiamocrm-0.1.1/
+-rw-rw-rw-   0        0        0      438 2024-05-30 10:13:02.292904 apiamocrm-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-30 09:48:06.000000 apiamocrm-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 10:13:02.291907 apiamocrm-0.1.1/apiAmoCRM.egg-info/
+-rw-rw-rw-   0        0        0      438 2024-05-30 10:13:02.000000 apiamocrm-0.1.1/apiAmoCRM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2024-05-30 10:13:02.000000 apiamocrm-0.1.1/apiAmoCRM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 10:13:02.000000 apiamocrm-0.1.1/apiAmoCRM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-30 10:13:02.000000 apiamocrm-0.1.1/apiAmoCRM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 10:13:02.000000 apiamocrm-0.1.1/apiAmoCRM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 10:13:02.293902 apiamocrm-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      633 2024-05-30 10:12:45.000000 apiamocrm-0.1.1/setup.py
```

### Comparing `apiamocrm-0.1.0/setup.py` & `apiamocrm-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='apiAmoCRM',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
     install_requires=[
         "requests",
     ],
     author='wlovem',
     author_email='wlovemrock@gmail.com',
     description='Api for amoCRM',
@@ -14,9 +14,9 @@
     long_description_content_type='text/markdown',
     url='https://github.com/cheboxarov/DialogServicesWidgets.git',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
-    python_requires='>=3.6',
+    python_requires='>=3',
 )
```

