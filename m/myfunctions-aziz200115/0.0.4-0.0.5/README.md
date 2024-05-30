# Comparing `tmp/myfunctions_aziz200115-0.0.4.tar.gz` & `tmp/myfunctions_aziz200115-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/aziz200115/python-class/evolvecyber/class5/dist/tmpb70xbuxc/myfunctions_aziz200115-0.0.4.tar", last modified: Thu May 30 01:32:14 2024, max compression
+gzip compressed data, was "/mnt/aziz200115/python-class/evolvecyber/class5/dist/tmp3q47ndx1/myfunctions_aziz200115-0.0.5.tar", last modified: Thu May 30 01:32:54 2024, max compression
```

## Comparing `myfunctions_aziz200115-0.0.4.tar` & `myfunctions_aziz200115-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 aziz200115  (1619) aziz200115  (1620)        0 2024-05-30 01:32:14.000000 myfunctions_aziz200115-0.0.4/
--rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)      642 2024-05-30 01:27:58.000000 myfunctions_aziz200115-0.0.4/setup.py
-drwxrwxr-x   0 aziz200115  (1619) aziz200115  (1620)        0 2024-05-30 01:32:14.000000 myfunctions_aziz200115-0.0.4/myfunctions_aziz200115/
--rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)      442 2024-05-30 01:31:10.000000 myfunctions_aziz200115-0.0.4/myfunctions_aziz200115/math.py
--rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)        0 2024-05-30 00:48:59.000000 myfunctions_aziz200115-0.0.4/myfunctions_aziz200115/__init__.py
--rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)      771 2024-05-30 01:19:26.000000 myfunctions_aziz200115-0.0.4/README.md
--rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)     1222 2024-05-30 01:32:14.000000 myfunctions_aziz200115-0.0.4/PKG-INFO
--rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)       38 2024-05-30 01:32:14.000000 myfunctions_aziz200115-0.0.4/setup.cfg
-drwxrwxr-x   0 aziz200115  (1619) aziz200115  (1620)        0 2024-05-30 01:32:14.000000 myfunctions_aziz200115-0.0.4/myfunctions_aziz200115.egg-info/
--rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)       23 2024-05-30 01:32:14.000000 myfunctions_aziz200115-0.0.4/myfunctions_aziz200115.egg-info/top_level.txt
--rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)      268 2024-05-30 01:32:14.000000 myfunctions_aziz200115-0.0.4/myfunctions_aziz200115.egg-info/SOURCES.txt
--rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)        1 2024-05-30 01:32:14.000000 myfunctions_aziz200115-0.0.4/myfunctions_aziz200115.egg-info/dependency_links.txt
--rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)     1222 2024-05-30 01:32:14.000000 myfunctions_aziz200115-0.0.4/myfunctions_aziz200115.egg-info/PKG-INFO
+drwxrwxr-x   0 aziz200115  (1619) aziz200115  (1620)        0 2024-05-30 01:32:54.000000 myfunctions_aziz200115-0.0.5/
+-rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)      646 2024-05-30 01:32:39.000000 myfunctions_aziz200115-0.0.5/setup.py
+drwxrwxr-x   0 aziz200115  (1619) aziz200115  (1620)        0 2024-05-30 01:32:53.000000 myfunctions_aziz200115-0.0.5/myfunctions_aziz200115/
+-rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)      442 2024-05-30 01:31:10.000000 myfunctions_aziz200115-0.0.5/myfunctions_aziz200115/math.py
+-rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)        0 2024-05-30 00:48:59.000000 myfunctions_aziz200115-0.0.5/myfunctions_aziz200115/__init__.py
+-rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)      771 2024-05-30 01:19:26.000000 myfunctions_aziz200115-0.0.5/README.md
+-rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)     1222 2024-05-30 01:32:54.000000 myfunctions_aziz200115-0.0.5/PKG-INFO
+-rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)       38 2024-05-30 01:32:54.000000 myfunctions_aziz200115-0.0.5/setup.cfg
+drwxrwxr-x   0 aziz200115  (1619) aziz200115  (1620)        0 2024-05-30 01:32:54.000000 myfunctions_aziz200115-0.0.5/myfunctions_aziz200115.egg-info/
+-rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)       23 2024-05-30 01:32:53.000000 myfunctions_aziz200115-0.0.5/myfunctions_aziz200115.egg-info/top_level.txt
+-rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)      313 2024-05-30 01:32:53.000000 myfunctions_aziz200115-0.0.5/myfunctions_aziz200115.egg-info/SOURCES.txt
+-rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)        3 2024-05-30 01:32:53.000000 myfunctions_aziz200115-0.0.5/myfunctions_aziz200115.egg-info/requires.txt
+-rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)        1 2024-05-30 01:32:53.000000 myfunctions_aziz200115-0.0.5/myfunctions_aziz200115.egg-info/dependency_links.txt
+-rw-rw-r--   0 aziz200115  (1619) aziz200115  (1620)     1222 2024-05-30 01:32:53.000000 myfunctions_aziz200115-0.0.5/myfunctions_aziz200115.egg-info/PKG-INFO
```

### Comparing `myfunctions_aziz200115-0.0.4/setup.py` & `myfunctions_aziz200115-0.0.5/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_aziz200115',
-    version='0.0.4',
+    version='0.0.5',
     packages=find_packages(),
-    install_requires=[],
+    install_requires=["os"],
     url='https://github.com/aziz200115/',
     license='MIT',
     author='Aziz Shekerbekov',
     author_email='awekerbekov@gmail.com',
     description='A description of your package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

### Comparing `myfunctions_aziz200115-0.0.4/README.md` & `myfunctions_aziz200115-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `myfunctions_aziz200115-0.0.4/PKG-INFO` & `myfunctions_aziz200115-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions_aziz200115
-Version: 0.0.4
+Version: 0.0.5
 Summary: A description of your package
 Home-page: https://github.com/aziz200115/
 Author: Aziz Shekerbekov
 Author-email: awekerbekov@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `myfunctions_aziz200115-0.0.4/myfunctions_aziz200115.egg-info/PKG-INFO` & `myfunctions_aziz200115-0.0.5/myfunctions_aziz200115.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions-aziz200115
-Version: 0.0.4
+Version: 0.0.5
 Summary: A description of your package
 Home-page: https://github.com/aziz200115/
 Author: Aziz Shekerbekov
 Author-email: awekerbekov@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

