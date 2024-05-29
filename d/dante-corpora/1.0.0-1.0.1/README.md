# Comparing `tmp/dante_corpora-1.0.0.tar.gz` & `tmp/dante_corpora-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dante_corpora-1.0.0.tar", last modified: Wed May 29 22:34:53 2024, max compression
+gzip compressed data, was "dante_corpora-1.0.1.tar", last modified: Wed May 29 23:02:58 2024, max compression
```

## Comparing `dante_corpora-1.0.0.tar` & `dante_corpora-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 22:34:53.895954 dante_corpora-1.0.0/
--rw-rw-rw-   0        0        0     1091 2024-05-29 22:19:30.000000 dante_corpora-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     3044 2024-05-29 22:34:53.895954 dante_corpora-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2718 2024-05-29 22:29:52.000000 dante_corpora-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 22:34:53.894986 dante_corpora-1.0.0/dante_corpora.egg-info/
--rw-rw-rw-   0        0        0     3044 2024-05-29 22:34:53.000000 dante_corpora-1.0.0/dante_corpora.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2024-05-29 22:34:53.000000 dante_corpora-1.0.0/dante_corpora.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 22:34:53.000000 dante_corpora-1.0.0/dante_corpora.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-29 22:34:53.000000 dante_corpora-1.0.0/dante_corpora.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-05-29 22:34:53.000000 dante_corpora-1.0.0/dante_corpora.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-29 22:34:53.893162 dante_corpora-1.0.0/danteshots/
--rw-rw-rw-   0        0        0        0 2024-05-29 15:04:17.000000 dante_corpora-1.0.0/danteshots/__init__.py
--rw-rw-rw-   0        0        0      101 2024-05-29 21:34:18.000000 dante_corpora-1.0.0/danteshots/danteshots.py
-drwxrwxrwx   0        0        0        0 2024-05-29 22:34:53.894899 dante_corpora-1.0.0/dantestocks/
--rw-rw-rw-   0        0        0        0 2024-05-29 15:05:20.000000 dante_corpora-1.0.0/dantestocks/__init__.py
--rw-rw-rw-   0        0        0      102 2024-05-29 21:34:22.000000 dante_corpora-1.0.0/dantestocks/dantestocks.py
--rw-rw-rw-   0        0        0       42 2024-05-29 22:34:53.895954 dante_corpora-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      526 2024-05-29 21:04:26.000000 dante_corpora-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 23:02:58.960170 dante_corpora-1.0.1/
+-rw-rw-rw-   0        0        0     1091 2024-05-29 22:19:30.000000 dante_corpora-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     3044 2024-05-29 23:02:58.959169 dante_corpora-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2718 2024-05-29 22:29:52.000000 dante_corpora-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 23:02:58.958171 dante_corpora-1.0.1/dante_corpora.egg-info/
+-rw-rw-rw-   0        0        0     3044 2024-05-29 23:02:58.000000 dante_corpora-1.0.1/dante_corpora.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2024-05-29 23:02:58.000000 dante_corpora-1.0.1/dante_corpora.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 23:02:58.000000 dante_corpora-1.0.1/dante_corpora.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-29 23:02:58.000000 dante_corpora-1.0.1/dante_corpora.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-29 23:02:58.000000 dante_corpora-1.0.1/dante_corpora.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 23:02:58.960170 dante_corpora-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      526 2024-05-29 23:02:47.000000 dante_corpora-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 23:02:58.958171 dante_corpora-1.0.1/src/
+-rw-rw-rw-   0        0        0       75 2024-05-29 23:01:49.000000 dante_corpora-1.0.1/src/__init__.py
+-rw-rw-rw-   0        0        0      101 2024-05-29 21:34:18.000000 dante_corpora-1.0.1/src/danteshots.py
+-rw-rw-rw-   0        0        0      102 2024-05-29 21:34:22.000000 dante_corpora-1.0.1/src/dantestocks.py
```

### Comparing `dante_corpora-1.0.0/LICENSE` & `dante_corpora-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dante_corpora-1.0.0/PKG-INFO` & `dante_corpora-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dante-corpora
-Version: 1.0.0
+Version: 1.0.1
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
-Metadata-Version: 2.1 Name: dante-corpora Version: 1.0.0 Summary: Pacote Python
+Metadata-Version: 2.1 Name: dante-corpora Version: 1.0.1 Summary: Pacote Python
 contendo os corpora do projeto DANTE do POeTiSA Author: felmateos Author-email:
 felmateos@gmail.com License: MIT Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: pandas==2.2.2
    [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
 shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
       shield]][issues-url] [![MIT License][license-shield]][license-url]
```

### Comparing `dante_corpora-1.0.0/README.md` & `dante_corpora-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `dante_corpora-1.0.0/dante_corpora.egg-info/PKG-INFO` & `dante_corpora-1.0.1/dante_corpora.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dante-corpora
-Version: 1.0.0
+Version: 1.0.1
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
-Metadata-Version: 2.1 Name: dante-corpora Version: 1.0.0 Summary: Pacote Python
+Metadata-Version: 2.1 Name: dante-corpora Version: 1.0.1 Summary: Pacote Python
 contendo os corpora do projeto DANTE do POeTiSA Author: felmateos Author-email:
 felmateos@gmail.com License: MIT Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: pandas==2.2.2
    [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
 shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
       shield]][issues-url] [![MIT License][license-shield]][license-url]
```

### Comparing `dante_corpora-1.0.0/setup.py` & `dante_corpora-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='dante-corpora',
-    version='1.0.0',
+    version='1.0.1',
     description='Pacote Python contendo os corpora do projeto DANTE do POeTiSA',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='felmateos',
     author_email='felmateos@gmail.com',
     packages=find_packages(),
     install_requires=[
```

