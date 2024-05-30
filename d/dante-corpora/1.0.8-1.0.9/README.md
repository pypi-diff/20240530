# Comparing `tmp/dante_corpora-1.0.8.tar.gz` & `tmp/dante_corpora-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dante_corpora-1.0.8.tar", last modified: Thu May 30 17:40:25 2024, max compression
+gzip compressed data, was "dante_corpora-1.0.9.tar", last modified: Thu May 30 17:46:46 2024, max compression
```

## Comparing `dante_corpora-1.0.8.tar` & `dante_corpora-1.0.9.tar`

### file list

```diff
@@ -1,16 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 17:40:25.110735 dante_corpora-1.0.8/
--rw-rw-rw-   0        0        0     1091 2024-05-29 22:19:30.000000 dante_corpora-1.0.8/LICENSE
--rw-rw-rw-   0        0        0       20 2024-05-30 17:38:03.000000 dante_corpora-1.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     3045 2024-05-30 17:40:25.110735 dante_corpora-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2747 2024-05-30 17:40:13.000000 dante_corpora-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 17:40:25.105980 dante_corpora-1.0.8/dante/
--rw-rw-rw-   0        0        0       24 2024-05-30 17:37:44.000000 dante_corpora-1.0.8/dante/__init__.py
--rw-rw-rw-   0        0        0     2450 2024-05-30 17:35:37.000000 dante_corpora-1.0.8/dante/corpora.py
-drwxrwxrwx   0        0        0        0 2024-05-30 17:40:25.110033 dante_corpora-1.0.8/dante_corpora.egg-info/
--rw-rw-rw-   0        0        0     3045 2024-05-30 17:40:25.000000 dante_corpora-1.0.8/dante_corpora.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2024-05-30 17:40:25.000000 dante_corpora-1.0.8/dante_corpora.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 17:40:25.000000 dante_corpora-1.0.8/dante_corpora.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-30 17:40:25.000000 dante_corpora-1.0.8/dante_corpora.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-30 17:40:25.000000 dante_corpora-1.0.8/dante_corpora.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 17:40:25.112335 dante_corpora-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      622 2024-05-30 17:40:22.000000 dante_corpora-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 17:46:46.521069 dante_corpora-1.0.9/
+-rw-rw-rw-   0        0        0     1091 2024-05-29 22:19:30.000000 dante_corpora-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0       52 2024-05-30 17:46:15.000000 dante_corpora-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     3045 2024-05-30 17:46:46.520092 dante_corpora-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2747 2024-05-30 17:40:13.000000 dante_corpora-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 17:46:46.423713 dante_corpora-1.0.9/dante/
+-rw-rw-rw-   0        0        0       24 2024-05-30 17:37:44.000000 dante_corpora-1.0.9/dante/__init__.py
+-rw-rw-rw-   0        0        0     2450 2024-05-30 17:35:37.000000 dante_corpora-1.0.9/dante/corpora.py
+drwxrwxrwx   0        0        0        0 2024-05-30 17:46:46.417420 dante_corpora-1.0.9/dante/data/
+drwxrwxrwx   0        0        0        0 2024-05-30 17:46:46.485034 dante_corpora-1.0.9/dante/data/danteshots/
+-rw-rw-rw-   0        0        0 10840347 2024-04-08 13:26:14.000000 dante_corpora-1.0.9/dante/data/danteshots/POS.conllu
+-rw-rw-rw-   0        0        0  1836029 2024-04-08 13:13:38.000000 dante_corpora-1.0.9/dante/data/danteshots/base.csv
+-rw-rw-rw-   0        0        0 12835113 2024-04-29 10:36:02.000000 dante_corpora-1.0.9/dante/data/danteshots/final_table.csv
+-rw-rw-rw-   0        0        0   252772 2024-04-29 10:36:23.000000 dante_corpora-1.0.9/dante/data/danteshots/table_freq.csv
+-rw-rw-rw-   0        0        0    21281 2024-04-29 10:36:30.000000 dante_corpora-1.0.9/dante/data/danteshots/table_freq_indi.csv
+-rw-rw-rw-   0        0        0      162 2024-04-29 10:36:39.000000 dante_corpora-1.0.9/dante/data/danteshots/table_freq_tweet.csv
+drwxrwxrwx   0        0        0        0 2024-05-30 17:46:46.508895 dante_corpora-1.0.9/dante/data/dantestocks/
+-rw-rw-rw-   0        0        0  4349020 2024-04-08 11:17:02.000000 dante_corpora-1.0.9/dante/data/dantestocks/POS.conllu
+-rw-rw-rw-   0        0        0   770632 2024-03-11 13:06:38.000000 dante_corpora-1.0.9/dante/data/dantestocks/base.csv
+-rw-rw-rw-   0        0        0  3488355 2024-04-08 11:17:08.000000 dante_corpora-1.0.9/dante/data/dantestocks/final_table.csv
+-rw-rw-rw-   0        0        0   142000 2024-04-08 11:17:06.000000 dante_corpora-1.0.9/dante/data/dantestocks/table_freq.csv
+-rw-rw-rw-   0        0        0     8598 2024-04-08 11:17:06.000000 dante_corpora-1.0.9/dante/data/dantestocks/table_freq_indi.csv
+-rw-rw-rw-   0        0        0      159 2024-04-08 11:17:08.000000 dante_corpora-1.0.9/dante/data/dantestocks/table_freq_tweet.csv
+drwxrwxrwx   0        0        0        0 2024-05-30 17:46:46.518099 dante_corpora-1.0.9/dante_corpora.egg-info/
+-rw-rw-rw-   0        0        0     3045 2024-05-30 17:46:46.000000 dante_corpora-1.0.9/dante_corpora.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      711 2024-05-30 17:46:46.000000 dante_corpora-1.0.9/dante_corpora.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 17:46:46.000000 dante_corpora-1.0.9/dante_corpora.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-30 17:46:46.000000 dante_corpora-1.0.9/dante_corpora.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-30 17:46:46.000000 dante_corpora-1.0.9/dante_corpora.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 17:46:46.521777 dante_corpora-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      620 2024-05-30 17:46:37.000000 dante_corpora-1.0.9/setup.py
```

### Comparing `dante_corpora-1.0.8/LICENSE` & `dante_corpora-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dante_corpora-1.0.8/PKG-INFO` & `dante_corpora-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dante-corpora
-Version: 1.0.8
+Version: 1.0.9
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
-Metadata-Version: 2.1 Name: dante-corpora Version: 1.0.8 Summary: Pacote Python
+Metadata-Version: 2.1 Name: dante-corpora Version: 1.0.9 Summary: Pacote Python
 contendo os corpora do projeto DANTE do POeTiSA Author: felmateos Author-email:
 felmateos@gmail.com License: MIT Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: pandas==2.2.2
    [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
 shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
       shield]][issues-url] [![MIT License][license-shield]][license-url]
```

### Comparing `dante_corpora-1.0.8/README.md` & `dante_corpora-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dante_corpora-1.0.8/dante/corpora.py` & `dante_corpora-1.0.9/dante/corpora.py`

 * *Files identical despite different names*

### Comparing `dante_corpora-1.0.8/dante_corpora.egg-info/PKG-INFO` & `dante_corpora-1.0.9/dante_corpora.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dante-corpora
-Version: 1.0.8
+Version: 1.0.9
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
-Metadata-Version: 2.1 Name: dante-corpora Version: 1.0.8 Summary: Pacote Python
+Metadata-Version: 2.1 Name: dante-corpora Version: 1.0.9 Summary: Pacote Python
 contendo os corpora do projeto DANTE do POeTiSA Author: felmateos Author-email:
 felmateos@gmail.com License: MIT Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: pandas==2.2.2
    [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
 shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
       shield]][issues-url] [![MIT License][license-shield]][license-url]
```

