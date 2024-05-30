# Comparing `tmp/predictions_sepsis-0.0.3.tar.gz` & `tmp/predictions_sepsis-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/predictions_sepsis-0.0.3.tar", last modified: Thu May 30 15:49:33 2024, max compression
+gzip compressed data, was "dist/predictions_sepsis-0.0.5.tar", last modified: Thu May 30 16:05:39 2024, max compression
```

## Comparing `predictions_sepsis-0.0.3.tar` & `predictions_sepsis-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 artemij    (501) staff       (20)        0 2024-05-30 15:49:33.000000 predictions_sepsis-0.0.3/
--rw-r--r--   0 artemij    (501) staff       (20)      518 2024-05-30 15:49:33.000000 predictions_sepsis-0.0.3/PKG-INFO
-drwxr-xr-x   0 artemij    (501) staff       (20)        0 2024-05-30 15:49:33.000000 predictions_sepsis-0.0.3/sepsis_predictions/
--rw-r--r--   0 artemij    (501) staff       (20)       55 2024-05-30 15:45:26.000000 predictions_sepsis-0.0.3/sepsis_predictions/__init__.py
-drwxr-xr-x   0 artemij    (501) staff       (20)        0 2024-05-30 15:49:33.000000 predictions_sepsis-0.0.3/predictions_sepsis.egg-info/
--rw-r--r--   0 artemij    (501) staff       (20)      518 2024-05-30 15:49:33.000000 predictions_sepsis-0.0.3/predictions_sepsis.egg-info/PKG-INFO
--rw-r--r--   0 artemij    (501) staff       (20)      268 2024-05-30 15:49:33.000000 predictions_sepsis-0.0.3/predictions_sepsis.egg-info/SOURCES.txt
--rw-r--r--   0 artemij    (501) staff       (20)       17 2024-05-30 15:49:33.000000 predictions_sepsis-0.0.3/predictions_sepsis.egg-info/requires.txt
--rw-r--r--   0 artemij    (501) staff       (20)       19 2024-05-30 15:49:33.000000 predictions_sepsis-0.0.3/predictions_sepsis.egg-info/top_level.txt
--rw-r--r--   0 artemij    (501) staff       (20)        1 2024-05-30 15:49:33.000000 predictions_sepsis-0.0.3/predictions_sepsis.egg-info/dependency_links.txt
--rw-r--r--   0 artemij    (501) staff       (20)        0 2024-05-30 15:10:11.000000 predictions_sepsis-0.0.3/README.md
--rw-r--r--   0 artemij    (501) staff       (20)      751 2024-05-30 15:46:50.000000 predictions_sepsis-0.0.3/setup.py
--rw-r--r--   0 artemij    (501) staff       (20)       38 2024-05-30 15:49:33.000000 predictions_sepsis-0.0.3/setup.cfg
+drwxr-xr-x   0 artemij    (501) staff       (20)        0 2024-05-30 16:05:39.000000 predictions_sepsis-0.0.5/
+-rw-r--r--   0 artemij    (501) staff       (20)      518 2024-05-30 16:05:39.000000 predictions_sepsis-0.0.5/PKG-INFO
+drwxr-xr-x   0 artemij    (501) staff       (20)        0 2024-05-30 16:05:39.000000 predictions_sepsis-0.0.5/predictions_sepsis.egg-info/
+-rw-r--r--   0 artemij    (501) staff       (20)      518 2024-05-30 16:05:39.000000 predictions_sepsis-0.0.5/predictions_sepsis.egg-info/PKG-INFO
+-rw-r--r--   0 artemij    (501) staff       (20)      268 2024-05-30 16:05:39.000000 predictions_sepsis-0.0.5/predictions_sepsis.egg-info/SOURCES.txt
+-rw-r--r--   0 artemij    (501) staff       (20)       17 2024-05-30 16:05:39.000000 predictions_sepsis-0.0.5/predictions_sepsis.egg-info/requires.txt
+-rw-r--r--   0 artemij    (501) staff       (20)       19 2024-05-30 16:05:39.000000 predictions_sepsis-0.0.5/predictions_sepsis.egg-info/top_level.txt
+-rw-r--r--   0 artemij    (501) staff       (20)        1 2024-05-30 16:05:39.000000 predictions_sepsis-0.0.5/predictions_sepsis.egg-info/dependency_links.txt
+-rw-r--r--   0 artemij    (501) staff       (20)        0 2024-05-30 15:10:11.000000 predictions_sepsis-0.0.5/README.md
+-rw-r--r--   0 artemij    (501) staff       (20)      751 2024-05-30 16:05:39.000000 predictions_sepsis-0.0.5/setup.py
+-rw-r--r--   0 artemij    (501) staff       (20)       38 2024-05-30 16:05:39.000000 predictions_sepsis-0.0.5/setup.cfg
+drwxr-xr-x   0 artemij    (501) staff       (20)        0 2024-05-30 16:05:39.000000 predictions_sepsis-0.0.5/predictions_sepsis/
+-rw-r--r--   0 artemij    (501) staff       (20)       56 2024-05-30 16:02:02.000000 predictions_sepsis-0.0.5/predictions_sepsis/__init__.py
```

### Comparing `predictions_sepsis-0.0.3/PKG-INFO` & `predictions_sepsis-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: predictions_sepsis
-Version: 0.0.3
+Version: 0.0.5
 Summary: Module for sepsis predictions
 Home-page: https://github.com/sslavian812/sepsis-predictions.git
 Author: @Margo78, @akp1n
 Author-email: timtimk30@yandex.ru
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: example python
```

### Comparing `predictions_sepsis-0.0.3/predictions_sepsis.egg-info/PKG-INFO` & `predictions_sepsis-0.0.5/predictions_sepsis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: predictions-sepsis
-Version: 0.0.3
+Version: 0.0.5
 Summary: Module for sepsis predictions
 Home-page: https://github.com/sslavian812/sepsis-predictions.git
 Author: @Margo78, @akp1n
 Author-email: timtimk30@yandex.ru
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: example python
```

### Comparing `predictions_sepsis-0.0.3/setup.py` & `predictions_sepsis-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 setup(
     name='predictions_sepsis',
-    version='0.0.3',
+    version='0.0.5',
     author='@Margo78, @akp1n',
     author_email='timtimk30@yandex.ru',
     description='Module for sepsis predictions',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/sslavian812/sepsis-predictions.git',
     packages=find_packages(),
```

