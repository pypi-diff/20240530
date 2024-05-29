# Comparing `tmp/csvtex-1.0.0.tar.gz` & `tmp/csvtex-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csvtex-1.0.0.tar", max compression
+gzip compressed data, was "csvtex-1.0.1.tar", max compression
```

## Comparing `csvtex-1.0.0.tar` & `csvtex-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1068 2024-05-29 08:02:31.141592 csvtex-1.0.0/LICENSE
--rw-r--r--   0        0        0     2304 2024-05-29 08:43:42.284273 csvtex-1.0.0/README.md
--rw-r--r--   0        0        0      196 2024-05-29 08:32:45.254861 csvtex-1.0.0/csvtex/__init__.py
--rw-r--r--   0        0        0     4161 2024-05-29 08:34:53.123889 csvtex-1.0.0/csvtex/main.py
--rw-r--r--   0        0        0      391 2024-05-29 08:42:56.643889 csvtex-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2787 1970-01-01 00:00:00.000000 csvtex-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-29 08:02:31.141592 csvtex-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2304 2024-05-29 08:43:42.284273 csvtex-1.0.1/README.md
+-rw-r--r--   0        0        0      196 2024-05-29 08:32:45.254861 csvtex-1.0.1/csvtex/__init__.py
+-rw-r--r--   0        0        0     4161 2024-05-29 08:34:53.123889 csvtex-1.0.1/csvtex/main.py
+-rw-r--r--   0        0        0      391 2024-05-29 09:10:31.704151 csvtex-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2887 1970-01-01 00:00:00.000000 csvtex-1.0.1/PKG-INFO
```

### Comparing `csvtex-1.0.0/LICENSE` & `csvtex-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `csvtex-1.0.0/README.md` & `csvtex-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `csvtex-1.0.0/csvtex/main.py` & `csvtex-1.0.1/csvtex/main.py`

 * *Files identical despite different names*

### Comparing `csvtex-1.0.0/PKG-INFO` & `csvtex-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: csvtex
-Version: 1.0.0
+Version: 1.0.1
 Summary: 
 License: MIT
 Author: Scott Suk
 Author-email: scottsuk0306@gmail.com
-Requires-Python: >3.9
+Requires-Python: >3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Description-Content-Type: text/markdown
 
 # 📊 csvtex - Convert CSV Files to LaTeX Tables 📄
```

