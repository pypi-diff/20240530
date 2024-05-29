# Comparing `tmp/MORALS-0.1.1.tar.gz` & `tmp/morals-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MORALS-0.1.1.tar", last modified: Fri Oct 13 20:14:01 2023, max compression
+gzip compressed data, was "morals-0.1.2.tar", last modified: Wed May 29 22:16:15 2024, max compression
```

## Comparing `MORALS-0.1.1.tar` & `morals-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ewerton    (501) staff       (20)        0 2023-10-13 20:14:01.400699 MORALS-0.1.1/
--rw-r--r--   0 ewerton    (501) staff       (20)     1122 2023-09-19 16:48:06.000000 MORALS-0.1.1/LICENSE
-drwxr-xr-x   0 ewerton    (501) staff       (20)        0 2023-10-13 20:14:01.395491 MORALS-0.1.1/MORALS/
--rw-r--r--   0 ewerton    (501) staff       (20)        0 2023-09-16 01:37:29.000000 MORALS-0.1.1/MORALS/__init__.py
--rw-r--r--   0 ewerton    (501) staff       (20)     8952 2023-10-13 19:54:43.000000 MORALS-0.1.1/MORALS/data_utils.py
--rw-r--r--   0 ewerton    (501) staff       (20)     3028 2023-10-13 19:54:33.000000 MORALS-0.1.1/MORALS/dynamics_utils.py
--rw-r--r--   0 ewerton    (501) staff       (20)    12497 2023-10-13 19:53:48.000000 MORALS-0.1.1/MORALS/grid.py
--rw-r--r--   0 ewerton    (501) staff       (20)     4131 2023-10-13 19:54:19.000000 MORALS-0.1.1/MORALS/mg_utils.py
--rw-r--r--   0 ewerton    (501) staff       (20)     3571 2023-10-13 19:54:24.000000 MORALS-0.1.1/MORALS/models.py
--rw-r--r--   0 ewerton    (501) staff       (20)     9446 2023-10-13 19:53:51.000000 MORALS-0.1.1/MORALS/training.py
-drwxr-xr-x   0 ewerton    (501) staff       (20)        0 2023-10-13 20:14:01.398737 MORALS-0.1.1/MORALS.egg-info/
--rw-r--r--   0 ewerton    (501) staff       (20)      571 2023-10-13 20:14:01.000000 MORALS-0.1.1/MORALS.egg-info/PKG-INFO
--rw-r--r--   0 ewerton    (501) staff       (20)      325 2023-10-13 20:14:01.000000 MORALS-0.1.1/MORALS.egg-info/SOURCES.txt
--rw-r--r--   0 ewerton    (501) staff       (20)        1 2023-10-13 20:14:01.000000 MORALS-0.1.1/MORALS.egg-info/dependency_links.txt
--rw-r--r--   0 ewerton    (501) staff       (20)       92 2023-10-13 20:14:01.000000 MORALS-0.1.1/MORALS.egg-info/requires.txt
--rw-r--r--   0 ewerton    (501) staff       (20)        7 2023-10-13 20:14:01.000000 MORALS-0.1.1/MORALS.egg-info/top_level.txt
--rw-r--r--   0 ewerton    (501) staff       (20)      571 2023-10-13 20:14:01.399879 MORALS-0.1.1/PKG-INFO
--rw-r--r--   0 ewerton    (501) staff       (20)        0 2023-10-13 20:13:41.000000 MORALS-0.1.1/README.md
--rw-r--r--   0 ewerton    (501) staff       (20)      123 2023-10-13 19:49:56.000000 MORALS-0.1.1/pyproject.toml
--rw-r--r--   0 ewerton    (501) staff       (20)       38 2023-10-13 20:14:01.400845 MORALS-0.1.1/setup.cfg
--rw-r--r--   0 ewerton    (501) staff       (20)      585 2023-10-13 20:13:08.000000 MORALS-0.1.1/setup.py
+drwxr-xr-x   0 ewerton    (501) staff       (20)        0 2024-05-29 22:16:15.315537 morals-0.1.2/
+-rw-r--r--   0 ewerton    (501) staff       (20)     1122 2023-11-02 20:16:15.000000 morals-0.1.2/LICENSE
+drwxr-xr-x   0 ewerton    (501) staff       (20)        0 2024-05-29 22:16:15.308145 morals-0.1.2/MORALS/
+-rw-r--r--   0 ewerton    (501) staff       (20)        0 2023-09-16 01:37:29.000000 morals-0.1.2/MORALS/__init__.py
+-rw-r--r--   0 ewerton    (501) staff       (20)     8952 2023-10-13 19:54:43.000000 morals-0.1.2/MORALS/data_utils.py
+-rw-r--r--   0 ewerton    (501) staff       (20)     3028 2023-10-13 19:54:33.000000 morals-0.1.2/MORALS/dynamics_utils.py
+-rw-r--r--   0 ewerton    (501) staff       (20)    12497 2023-10-13 19:53:48.000000 morals-0.1.2/MORALS/grid.py
+-rw-r--r--   0 ewerton    (501) staff       (20)     4131 2023-10-13 19:54:19.000000 morals-0.1.2/MORALS/mg_utils.py
+-rw-r--r--   0 ewerton    (501) staff       (20)     3571 2023-10-13 19:54:24.000000 morals-0.1.2/MORALS/models.py
+-rw-r--r--   0 ewerton    (501) staff       (20)     9446 2023-10-13 19:53:51.000000 morals-0.1.2/MORALS/training.py
+drwxr-xr-x   0 ewerton    (501) staff       (20)        0 2024-05-29 22:16:15.313663 morals-0.1.2/MORALS.egg-info/
+-rw-r--r--   0 ewerton    (501) staff       (20)     3093 2024-05-29 22:16:15.000000 morals-0.1.2/MORALS.egg-info/PKG-INFO
+-rw-r--r--   0 ewerton    (501) staff       (20)      325 2024-05-29 22:16:15.000000 morals-0.1.2/MORALS.egg-info/SOURCES.txt
+-rw-r--r--   0 ewerton    (501) staff       (20)        1 2024-05-29 22:16:15.000000 morals-0.1.2/MORALS.egg-info/dependency_links.txt
+-rw-r--r--   0 ewerton    (501) staff       (20)       91 2024-05-29 22:16:15.000000 morals-0.1.2/MORALS.egg-info/requires.txt
+-rw-r--r--   0 ewerton    (501) staff       (20)        7 2024-05-29 22:16:15.000000 morals-0.1.2/MORALS.egg-info/top_level.txt
+-rw-r--r--   0 ewerton    (501) staff       (20)     3093 2024-05-29 22:16:15.314702 morals-0.1.2/PKG-INFO
+-rw-r--r--   0 ewerton    (501) staff       (20)     2483 2023-11-02 20:16:15.000000 morals-0.1.2/README.md
+-rw-r--r--   0 ewerton    (501) staff       (20)      123 2023-10-13 19:49:56.000000 morals-0.1.2/pyproject.toml
+-rw-r--r--   0 ewerton    (501) staff       (20)       38 2024-05-29 22:16:15.315706 morals-0.1.2/setup.cfg
+-rw-r--r--   0 ewerton    (501) staff       (20)      634 2024-05-29 22:16:03.000000 morals-0.1.2/setup.py
```

### Comparing `MORALS-0.1.1/LICENSE` & `morals-0.1.2/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 MIT License
 
-Copyright (c) 2023 Aravind Sivaramakrishnan, Dhruv Metha Ramesh, Ewerton Rocha Vieira
+Copyright (c) 2023 Ewerton Rocha Vieira, Aravind Sivaramakrishnan, Sumanth Tangirala
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `MORALS-0.1.1/MORALS/data_utils.py` & `morals-0.1.2/MORALS/data_utils.py`

 * *Files identical despite different names*

### Comparing `MORALS-0.1.1/MORALS/dynamics_utils.py` & `morals-0.1.2/MORALS/dynamics_utils.py`

 * *Files identical despite different names*

### Comparing `MORALS-0.1.1/MORALS/grid.py` & `morals-0.1.2/MORALS/grid.py`

 * *Files identical despite different names*

### Comparing `MORALS-0.1.1/MORALS/mg_utils.py` & `morals-0.1.2/MORALS/mg_utils.py`

 * *Files identical despite different names*

### Comparing `MORALS-0.1.1/MORALS/models.py` & `morals-0.1.2/MORALS/models.py`

 * *Files identical despite different names*

### Comparing `MORALS-0.1.1/MORALS/training.py` & `morals-0.1.2/MORALS/training.py`

 * *Files identical despite different names*

