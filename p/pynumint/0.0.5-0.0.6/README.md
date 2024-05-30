# Comparing `tmp/pynumint-0.0.5.tar.gz` & `tmp/pynumint-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynumint-0.0.5.tar", last modified: Thu May 30 08:24:18 2024, max compression
+gzip compressed data, was "pynumint-0.0.6.tar", last modified: Thu May 30 08:47:40 2024, max compression
```

## Comparing `pynumint-0.0.5.tar` & `pynumint-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 08:24:18.325828 pynumint-0.0.5/
--rw-rw-rw-   0        0        0     1091 2024-05-26 10:33:54.000000 pynumint-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     3978 2024-05-30 08:24:18.324830 pynumint-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3470 2024-05-30 07:34:52.000000 pynumint-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 08:24:18.283712 pynumint-0.0.5/pynumint/
-drwxrwxrwx   0        0        0        0 2024-05-30 08:24:18.323830 pynumint-0.0.5/pynumint/src/
-drwxrwxrwx   0        0        0        0 2024-05-30 08:24:18.322832 pynumint-0.0.5/pynumint/src/pynumint.egg-info/
--rw-rw-rw-   0        0        0     3978 2024-05-30 08:24:18.000000 pynumint-0.0.5/pynumint/src/pynumint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2024-05-30 08:24:18.000000 pynumint-0.0.5/pynumint/src/pynumint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 08:24:18.000000 pynumint-0.0.5/pynumint/src/pynumint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-30 08:24:18.000000 pynumint-0.0.5/pynumint/src/pynumint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4237 2024-05-30 07:33:34.000000 pynumint-0.0.5/pynumint/src/pynumint.py
--rw-rw-rw-   0        0        0       42 2024-05-30 08:24:18.325828 pynumint-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     2957 2024-05-30 08:23:41.000000 pynumint-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 08:47:40.001984 pynumint-0.0.6/
+-rw-rw-rw-   0        0        0     1091 2024-05-26 10:33:54.000000 pynumint-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     3978 2024-05-30 08:47:40.000359 pynumint-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3470 2024-05-30 07:34:52.000000 pynumint-0.0.6/README.md
+-rw-rw-rw-   0        0        0      160 2024-05-30 08:34:23.000000 pynumint-0.0.6/post_install.py
+drwxrwxrwx   0        0        0        0 2024-05-30 08:47:39.795105 pynumint-0.0.6/pynumint/
+drwxrwxrwx   0        0        0        0 2024-05-30 08:47:39.982222 pynumint-0.0.6/pynumint/src/
+drwxrwxrwx   0        0        0        0 2024-05-30 08:47:39.958217 pynumint-0.0.6/pynumint/src/pynumint.egg-info/
+-rw-rw-rw-   0        0        0     3978 2024-05-30 08:47:39.000000 pynumint-0.0.6/pynumint/src/pynumint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2024-05-30 08:47:39.000000 pynumint-0.0.6/pynumint/src/pynumint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 08:47:39.000000 pynumint-0.0.6/pynumint/src/pynumint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-30 08:47:39.000000 pynumint-0.0.6/pynumint/src/pynumint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4237 2024-05-30 07:33:34.000000 pynumint-0.0.6/pynumint/src/pynumint.py
+-rw-rw-rw-   0        0        0       42 2024-05-30 08:47:40.001984 pynumint-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      982 2024-05-30 08:47:05.000000 pynumint-0.0.6/setup.py
```

### Comparing `pynumint-0.0.5/LICENSE` & `pynumint-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pynumint-0.0.5/PKG-INFO` & `pynumint-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynumint
-Version: 0.0.5
+Version: 0.0.6
 Summary: pynumint Test Package for Numerical Integration Demo
 Home-page: https://pypi.org/project/pynumint/
 Author: Arjun Jagdale
 Author-email: arjunjagdale14@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pynumint-0.0.5/README.md` & `pynumint-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pynumint-0.0.5/pynumint/src/pynumint.egg-info/PKG-INFO` & `pynumint-0.0.6/pynumint/src/pynumint.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynumint
-Version: 0.0.5
+Version: 0.0.6
 Summary: pynumint Test Package for Numerical Integration Demo
 Home-page: https://pypi.org/project/pynumint/
 Author: Arjun Jagdale
 Author-email: arjunjagdale14@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pynumint-0.0.5/pynumint/src/pynumint.py` & `pynumint-0.0.6/pynumint/src/pynumint.py`

 * *Files identical despite different names*

