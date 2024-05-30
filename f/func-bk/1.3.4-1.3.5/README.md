# Comparing `tmp/func_bk-1.3.4.tar.gz` & `tmp/func_bk-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "func_bk-1.3.4.tar", last modified: Thu May 30 12:49:35 2024, max compression
+gzip compressed data, was "func_bk-1.3.5.tar", last modified: Thu May 30 12:55:00 2024, max compression
```

## Comparing `func_bk-1.3.4.tar` & `func_bk-1.3.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 12:49:35.020662 func_bk-1.3.4/
--rw-rw-rw-   0        0        0     2994 2024-05-30 12:49:35.020662 func_bk-1.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     2777 2024-05-30 12:32:20.000000 func_bk-1.3.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 12:49:35.013661 func_bk-1.3.4/func_bk/
--rw-rw-rw-   0        0        0     2491 2024-05-30 10:23:47.000000 func_bk-1.3.4/func_bk/__init__.py
--rw-rw-rw-   0        0        0     1719 2024-05-30 12:33:24.000000 func_bk-1.3.4/func_bk/django.py
--rw-rw-rw-   0        0        0     4604 2024-05-30 12:43:39.000000 func_bk-1.3.4/func_bk/fast_api.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:49:35.019659 func_bk-1.3.4/func_bk.egg-info/
--rw-rw-rw-   0        0        0     2994 2024-05-30 12:49:34.000000 func_bk-1.3.4/func_bk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2024-05-30 12:49:34.000000 func_bk-1.3.4/func_bk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 12:49:34.000000 func_bk-1.3.4/func_bk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-30 12:49:34.000000 func_bk-1.3.4/func_bk.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2024-05-30 12:49:34.000000 func_bk-1.3.4/func_bk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       44 2024-05-30 12:49:35.021659 func_bk-1.3.4/setup.cfg
--rw-rw-rw-   0        0        0      492 2024-05-30 12:34:31.000000 func_bk-1.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:55:00.360558 func_bk-1.3.5/
+-rw-rw-rw-   0        0        0     2994 2024-05-30 12:55:00.359556 func_bk-1.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2777 2024-05-30 12:32:20.000000 func_bk-1.3.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 12:55:00.353556 func_bk-1.3.5/func_bk/
+-rw-rw-rw-   0        0        0     2491 2024-05-30 10:23:47.000000 func_bk-1.3.5/func_bk/__init__.py
+-rw-rw-rw-   0        0        0     1719 2024-05-30 12:33:24.000000 func_bk-1.3.5/func_bk/django.py
+-rw-rw-rw-   0        0        0     7004 2024-05-30 12:54:41.000000 func_bk-1.3.5/func_bk/fast_api.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:55:00.359556 func_bk-1.3.5/func_bk.egg-info/
+-rw-rw-rw-   0        0        0     2994 2024-05-30 12:55:00.000000 func_bk-1.3.5/func_bk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2024-05-30 12:55:00.000000 func_bk-1.3.5/func_bk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 12:55:00.000000 func_bk-1.3.5/func_bk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-30 12:55:00.000000 func_bk-1.3.5/func_bk.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2024-05-30 12:55:00.000000 func_bk-1.3.5/func_bk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       44 2024-05-30 12:55:00.361557 func_bk-1.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      492 2024-05-30 12:34:31.000000 func_bk-1.3.5/setup.py
```

### Comparing `func_bk-1.3.4/PKG-INFO` & `func_bk-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func_bk
-Version: 1.3.4
+Version: 1.3.5
 Summary: add function for normal python and add class(for inheritance) for django
 Author-email: lilo.pio147@mail.ru
 Description-Content-Type: text/markdown
 
 add function 
 
 sejango - 3 arguments form(django),key(in form cleaned data),var(return if key is not find)
```

### Comparing `func_bk-1.3.4/README.md` & `func_bk-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `func_bk-1.3.4/func_bk/__init__.py` & `func_bk-1.3.5/func_bk/__init__.py`

 * *Files identical despite different names*

### Comparing `func_bk-1.3.4/func_bk/django.py` & `func_bk-1.3.5/func_bk/django.py`

 * *Files identical despite different names*

### Comparing `func_bk-1.3.4/func_bk.egg-info/PKG-INFO` & `func_bk-1.3.5/func_bk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func_bk
-Version: 1.3.4
+Version: 1.3.5
 Summary: add function for normal python and add class(for inheritance) for django
 Author-email: lilo.pio147@mail.ru
 Description-Content-Type: text/markdown
 
 add function 
 
 sejango - 3 arguments form(django),key(in form cleaned data),var(return if key is not find)
```

