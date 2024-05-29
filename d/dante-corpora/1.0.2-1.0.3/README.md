# Comparing `tmp/dante_corpora-1.0.2.tar.gz` & `tmp/dante_corpora-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dante_corpora-1.0.2.tar", last modified: Wed May 29 23:16:38 2024, max compression
+gzip compressed data, was "dante_corpora-1.0.3.tar", last modified: Wed May 29 23:19:53 2024, max compression
```

## Comparing `dante_corpora-1.0.2.tar` & `dante_corpora-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 23:16:38.111369 dante_corpora-1.0.2/
--rw-rw-rw-   0        0        0     1091 2024-05-29 22:19:30.000000 dante_corpora-1.0.2/LICENSE
--rw-rw-rw-   0        0        0       69 2024-05-29 23:13:34.000000 dante_corpora-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3044 2024-05-29 23:16:38.110370 dante_corpora-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2718 2024-05-29 22:29:52.000000 dante_corpora-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 23:16:38.097833 dante_corpora-1.0.2/dante/
--rw-rw-rw-   0        0        0       75 2024-05-29 23:01:49.000000 dante_corpora-1.0.2/dante/__init__.py
--rw-rw-rw-   0        0        0      101 2024-05-29 21:34:18.000000 dante_corpora-1.0.2/dante/danteshots.py
--rw-rw-rw-   0        0        0      102 2024-05-29 21:34:22.000000 dante_corpora-1.0.2/dante/dantestocks.py
-drwxrwxrwx   0        0        0        0 2024-05-29 23:16:38.102368 dante_corpora-1.0.2/dante/data/
--rw-rw-rw-   0        0        0  1836029 2024-04-08 13:13:38.000000 dante_corpora-1.0.2/dante/data/danteshots.csv
--rw-rw-rw-   0        0        0   770632 2024-03-11 13:06:38.000000 dante_corpora-1.0.2/dante/data/dantestocks.csv
-drwxrwxrwx   0        0        0        0 2024-05-29 23:16:38.109363 dante_corpora-1.0.2/dante_corpora.egg-info/
--rw-rw-rw-   0        0        0     3044 2024-05-29 23:16:37.000000 dante_corpora-1.0.2/dante_corpora.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      334 2024-05-29 23:16:38.000000 dante_corpora-1.0.2/dante_corpora.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 23:16:37.000000 dante_corpora-1.0.2/dante_corpora.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-29 23:16:37.000000 dante_corpora-1.0.2/dante_corpora.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-29 23:16:37.000000 dante_corpora-1.0.2/dante_corpora.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 23:16:38.111369 dante_corpora-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      620 2024-05-29 23:15:02.000000 dante_corpora-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 23:19:53.706438 dante_corpora-1.0.3/
+-rw-rw-rw-   0        0        0     1091 2024-05-29 22:19:30.000000 dante_corpora-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0       69 2024-05-29 23:13:34.000000 dante_corpora-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3044 2024-05-29 23:19:53.705441 dante_corpora-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2718 2024-05-29 22:29:52.000000 dante_corpora-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 23:19:53.694019 dante_corpora-1.0.3/dante/
+-rw-rw-rw-   0        0        0       75 2024-05-29 23:01:49.000000 dante_corpora-1.0.3/dante/__init__.py
+-rw-rw-rw-   0        0        0       99 2024-05-29 23:19:35.000000 dante_corpora-1.0.3/dante/danteshots.py
+-rw-rw-rw-   0        0        0      100 2024-05-29 23:19:37.000000 dante_corpora-1.0.3/dante/dantestocks.py
+drwxrwxrwx   0        0        0        0 2024-05-29 23:19:53.697013 dante_corpora-1.0.3/dante/data/
+-rw-rw-rw-   0        0        0  1836029 2024-04-08 13:13:38.000000 dante_corpora-1.0.3/dante/data/danteshots.csv
+-rw-rw-rw-   0        0        0   770632 2024-03-11 13:06:38.000000 dante_corpora-1.0.3/dante/data/dantestocks.csv
+drwxrwxrwx   0        0        0        0 2024-05-29 23:19:53.704445 dante_corpora-1.0.3/dante_corpora.egg-info/
+-rw-rw-rw-   0        0        0     3044 2024-05-29 23:19:53.000000 dante_corpora-1.0.3/dante_corpora.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      334 2024-05-29 23:19:53.000000 dante_corpora-1.0.3/dante_corpora.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 23:19:53.000000 dante_corpora-1.0.3/dante_corpora.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-29 23:19:53.000000 dante_corpora-1.0.3/dante_corpora.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-29 23:19:53.000000 dante_corpora-1.0.3/dante_corpora.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 23:19:53.706438 dante_corpora-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      620 2024-05-29 23:19:49.000000 dante_corpora-1.0.3/setup.py
```

### Comparing `dante_corpora-1.0.2/LICENSE` & `dante_corpora-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dante_corpora-1.0.2/PKG-INFO` & `dante_corpora-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dante-corpora
-Version: 1.0.2
+Version: 1.0.3
 Summary: Pacote Python contendo os corpora do projeto DANTE do POeTiSA
 Author: felmateos
 Author-email: felmateos@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas==2.2.2
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dante-corpora Version: 1.0.2 Summary: Pacote Python
+Metadata-Version: 2.1 Name: dante-corpora Version: 1.0.3 Summary: Pacote Python
 contendo os corpora do projeto DANTE do POeTiSA Author: felmateos Author-email:
 felmateos@gmail.com License: MIT Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: pandas==2.2.2
    [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
 shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
       shield]][issues-url] [![MIT License][license-shield]][license-url]
```

### Comparing `dante_corpora-1.0.2/README.md` & `dante_corpora-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dante_corpora-1.0.2/dante/data/danteshots.csv` & `dante_corpora-1.0.3/dante/data/danteshots.csv`

 * *Files identical despite different names*

### Comparing `dante_corpora-1.0.2/dante/data/dantestocks.csv` & `dante_corpora-1.0.3/dante/data/dantestocks.csv`

 * *Files identical despite different names*

### Comparing `dante_corpora-1.0.2/dante_corpora.egg-info/PKG-INFO` & `dante_corpora-1.0.3/dante_corpora.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dante-corpora
-Version: 1.0.2
+Version: 1.0.3
 Summary: Pacote Python contendo os corpora do projeto DANTE do POeTiSA
 Author: felmateos
 Author-email: felmateos@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas==2.2.2
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dante-corpora Version: 1.0.2 Summary: Pacote Python
+Metadata-Version: 2.1 Name: dante-corpora Version: 1.0.3 Summary: Pacote Python
 contendo os corpora do projeto DANTE do POeTiSA Author: felmateos Author-email:
 felmateos@gmail.com License: MIT Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: pandas==2.2.2
    [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
 shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
       shield]][issues-url] [![MIT License][license-shield]][license-url]
```

### Comparing `dante_corpora-1.0.2/setup.py` & `dante_corpora-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='dante-corpora',
-    version='1.0.2',
+    version='1.0.3',
     description='Pacote Python contendo os corpora do projeto DANTE do POeTiSA',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='felmateos',
     author_email='felmateos@gmail.com',
     packages=find_packages(),
     package_data={
```

