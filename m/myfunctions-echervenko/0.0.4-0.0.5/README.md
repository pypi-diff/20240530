# Comparing `tmp/myfunctions_echervenko-0.0.4.tar.gz` & `tmp/myfunctions_echervenko-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/echervenko/python-class/evolvecyber/Class5/dist/tmpj6b1oyjs/myfunctions_echervenko-0.0.4.tar", last modified: Thu May 30 01:31:44 2024, max compression
+gzip compressed data, was "/mnt/echervenko/python-class/evolvecyber/Class5/dist/tmpbx_msesc/myfunctions_echervenko-0.0.5.tar", last modified: Thu May 30 01:33:24 2024, max compression
```

## Comparing `myfunctions_echervenko-0.0.4.tar` & `myfunctions_echervenko-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 echervenko  (1636) echervenko  (1637)        0 2024-05-30 01:31:44.000000 myfunctions_echervenko-0.0.4/
-drwxrwxr-x   0 echervenko  (1636) echervenko  (1637)        0 2024-05-30 01:31:44.000000 myfunctions_echervenko-0.0.4/myfunctions_echervenko/
--rw-rw-r--   0 echervenko  (1636) echervenko  (1637)      363 2024-05-30 01:30:57.000000 myfunctions_echervenko-0.0.4/myfunctions_echervenko/math.py
--rw-rw-r--   0 echervenko  (1636) echervenko  (1637)        0 2024-05-30 00:48:50.000000 myfunctions_echervenko-0.0.4/myfunctions_echervenko/__init__.py
--rw-rw-r--   0 echervenko  (1636) echervenko  (1637)      643 2024-05-30 01:27:13.000000 myfunctions_echervenko-0.0.4/setup.py
-drwxrwxr-x   0 echervenko  (1636) echervenko  (1637)        0 2024-05-30 01:31:44.000000 myfunctions_echervenko-0.0.4/myfunctions_echervenko.egg-info/
--rw-rw-r--   0 echervenko  (1636) echervenko  (1637)       23 2024-05-30 01:31:44.000000 myfunctions_echervenko-0.0.4/myfunctions_echervenko.egg-info/top_level.txt
--rw-rw-r--   0 echervenko  (1636) echervenko  (1637)      268 2024-05-30 01:31:44.000000 myfunctions_echervenko-0.0.4/myfunctions_echervenko.egg-info/SOURCES.txt
--rw-rw-r--   0 echervenko  (1636) echervenko  (1637)        1 2024-05-30 01:31:44.000000 myfunctions_echervenko-0.0.4/myfunctions_echervenko.egg-info/dependency_links.txt
--rw-rw-r--   0 echervenko  (1636) echervenko  (1637)     2847 2024-05-30 01:31:44.000000 myfunctions_echervenko-0.0.4/myfunctions_echervenko.egg-info/PKG-INFO
--rw-rw-r--   0 echervenko  (1636) echervenko  (1637)     2395 2024-05-30 01:18:36.000000 myfunctions_echervenko-0.0.4/README.md
--rw-rw-r--   0 echervenko  (1636) echervenko  (1637)     2847 2024-05-30 01:31:44.000000 myfunctions_echervenko-0.0.4/PKG-INFO
--rw-rw-r--   0 echervenko  (1636) echervenko  (1637)       38 2024-05-30 01:31:44.000000 myfunctions_echervenko-0.0.4/setup.cfg
+drwxrwxr-x   0 echervenko  (1636) echervenko  (1637)        0 2024-05-30 01:33:24.000000 myfunctions_echervenko-0.0.5/
+drwxrwxr-x   0 echervenko  (1636) echervenko  (1637)        0 2024-05-30 01:33:24.000000 myfunctions_echervenko-0.0.5/myfunctions_echervenko/
+-rw-rw-r--   0 echervenko  (1636) echervenko  (1637)      363 2024-05-30 01:30:57.000000 myfunctions_echervenko-0.0.5/myfunctions_echervenko/math.py
+-rw-rw-r--   0 echervenko  (1636) echervenko  (1637)        0 2024-05-30 00:48:50.000000 myfunctions_echervenko-0.0.5/myfunctions_echervenko/__init__.py
+-rw-rw-r--   0 echervenko  (1636) echervenko  (1637)      647 2024-05-30 01:32:35.000000 myfunctions_echervenko-0.0.5/setup.py
+drwxrwxr-x   0 echervenko  (1636) echervenko  (1637)        0 2024-05-30 01:33:24.000000 myfunctions_echervenko-0.0.5/myfunctions_echervenko.egg-info/
+-rw-rw-r--   0 echervenko  (1636) echervenko  (1637)       23 2024-05-30 01:33:24.000000 myfunctions_echervenko-0.0.5/myfunctions_echervenko.egg-info/top_level.txt
+-rw-rw-r--   0 echervenko  (1636) echervenko  (1637)      313 2024-05-30 01:33:24.000000 myfunctions_echervenko-0.0.5/myfunctions_echervenko.egg-info/SOURCES.txt
+-rw-rw-r--   0 echervenko  (1636) echervenko  (1637)        3 2024-05-30 01:33:24.000000 myfunctions_echervenko-0.0.5/myfunctions_echervenko.egg-info/requires.txt
+-rw-rw-r--   0 echervenko  (1636) echervenko  (1637)        1 2024-05-30 01:33:24.000000 myfunctions_echervenko-0.0.5/myfunctions_echervenko.egg-info/dependency_links.txt
+-rw-rw-r--   0 echervenko  (1636) echervenko  (1637)     2847 2024-05-30 01:33:24.000000 myfunctions_echervenko-0.0.5/myfunctions_echervenko.egg-info/PKG-INFO
+-rw-rw-r--   0 echervenko  (1636) echervenko  (1637)     2395 2024-05-30 01:18:36.000000 myfunctions_echervenko-0.0.5/README.md
+-rw-rw-r--   0 echervenko  (1636) echervenko  (1637)     2847 2024-05-30 01:33:24.000000 myfunctions_echervenko-0.0.5/PKG-INFO
+-rw-rw-r--   0 echervenko  (1636) echervenko  (1637)       38 2024-05-30 01:33:24.000000 myfunctions_echervenko-0.0.5/setup.cfg
```

### Comparing `myfunctions_echervenko-0.0.4/setup.py` & `myfunctions_echervenko-0.0.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_echervenko',
-    version='0.0.4',
+    version='0.0.5',
     packages=find_packages(),
-    install_requires=[],
+    install_requires=["os"],
     url='https://github.com/echervenko',
     license='MIT',
     author='Elena Chervenko',
     author_email='chervenkoelena@gmail.com',
     description='A description of your package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

### Comparing `myfunctions_echervenko-0.0.4/myfunctions_echervenko.egg-info/PKG-INFO` & `myfunctions_echervenko-0.0.5/myfunctions_echervenko.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions-echervenko
-Version: 0.0.4
+Version: 0.0.5
 Summary: A description of your package
 Home-page: https://github.com/echervenko
 Author: Elena Chervenko
 Author-email: chervenkoelena@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `myfunctions_echervenko-0.0.4/README.md` & `myfunctions_echervenko-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `myfunctions_echervenko-0.0.4/PKG-INFO` & `myfunctions_echervenko-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions_echervenko
-Version: 0.0.4
+Version: 0.0.5
 Summary: A description of your package
 Home-page: https://github.com/echervenko
 Author: Elena Chervenko
 Author-email: chervenkoelena@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

