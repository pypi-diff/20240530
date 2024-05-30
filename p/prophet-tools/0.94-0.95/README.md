# Comparing `tmp/prophet_tools-0.94.tar.gz` & `tmp/prophet_tools-0.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prophet_tools-0.94.tar", last modified: Sun May 26 18:51:55 2024, max compression
+gzip compressed data, was "prophet_tools-0.95.tar", last modified: Thu May 30 18:29:34 2024, max compression
```

## Comparing `prophet_tools-0.94.tar` & `prophet_tools-0.95.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 18:51:55.429113 prophet_tools-0.94/
--rw-rw-rw-   0        0        0      138 2024-05-26 18:51:55.429113 prophet_tools-0.94/PKG-INFO
--rw-rw-rw-   0        0        0      179 2023-12-24 23:12:27.000000 prophet_tools-0.94/README.md
-drwxrwxrwx   0        0        0        0 2024-05-26 18:51:55.424698 prophet_tools-0.94/prophet_tools/
--rw-rw-rw-   0        0        0        0 2024-02-12 01:43:39.000000 prophet_tools-0.94/prophet_tools/__init__.py
--rw-rw-rw-   0        0        0      149 2023-12-24 23:12:27.000000 prophet_tools-0.94/prophet_tools/auto_import.py
--rw-rw-rw-   0        0        0     1811 2024-03-16 17:13:15.000000 prophet_tools-0.94/prophet_tools/file_convertors.py
--rw-rw-rw-   0        0        0      268 2024-02-12 01:41:06.000000 prophet_tools-0.94/prophet_tools/how_to_import.py
--rw-rw-rw-   0        0        0     7558 2024-05-26 18:50:56.000000 prophet_tools-0.94/prophet_tools/my_functions.py
--rw-rw-rw-   0        0        0      463 2024-02-12 01:56:50.000000 prophet_tools-0.94/prophet_tools/parsing.py
--rw-rw-rw-   0        0        0     1287 2024-05-26 18:50:17.000000 prophet_tools-0.94/prophet_tools/terminal.py
--rw-rw-rw-   0        0        0     4164 2023-12-29 20:12:13.000000 prophet_tools-0.94/prophet_tools/всё_подряд.py
-drwxrwxrwx   0        0        0        0 2024-05-26 18:51:55.428112 prophet_tools-0.94/prophet_tools.egg-info/
--rw-rw-rw-   0        0        0      138 2024-05-26 18:51:55.000000 prophet_tools-0.94/prophet_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      449 2024-05-26 18:51:55.000000 prophet_tools-0.94/prophet_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 18:51:55.000000 prophet_tools-0.94/prophet_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-02-12 01:48:06.000000 prophet_tools-0.94/prophet_tools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       14 2024-05-26 18:51:55.000000 prophet_tools-0.94/prophet_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-26 18:51:55.430112 prophet_tools-0.94/setup.cfg
--rw-rw-rw-   0        0        0      241 2024-05-26 18:51:49.000000 prophet_tools-0.94/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 18:29:34.168405 prophet_tools-0.95/
+-rw-rw-rw-   0        0        0      138 2024-05-30 18:29:34.168405 prophet_tools-0.95/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2023-12-24 23:12:27.000000 prophet_tools-0.95/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 18:29:34.163400 prophet_tools-0.95/prophet_tools/
+-rw-rw-rw-   0        0        0        0 2024-02-12 01:43:39.000000 prophet_tools-0.95/prophet_tools/__init__.py
+-rw-rw-rw-   0        0        0      149 2023-12-24 23:12:27.000000 prophet_tools-0.95/prophet_tools/auto_import.py
+-rw-rw-rw-   0        0        0     2025 2024-05-30 18:29:02.000000 prophet_tools-0.95/prophet_tools/file_convertors.py
+-rw-rw-rw-   0        0        0      268 2024-02-12 01:41:06.000000 prophet_tools-0.95/prophet_tools/how_to_import.py
+-rw-rw-rw-   0        0        0     7558 2024-05-26 18:50:56.000000 prophet_tools-0.95/prophet_tools/my_functions.py
+-rw-rw-rw-   0        0        0      463 2024-02-12 01:56:50.000000 prophet_tools-0.95/prophet_tools/parsing.py
+-rw-rw-rw-   0        0        0     1287 2024-05-26 18:50:17.000000 prophet_tools-0.95/prophet_tools/terminal.py
+-rw-rw-rw-   0        0        0     4164 2023-12-29 20:12:13.000000 prophet_tools-0.95/prophet_tools/всё_подряд.py
+drwxrwxrwx   0        0        0        0 2024-05-30 18:29:34.167402 prophet_tools-0.95/prophet_tools.egg-info/
+-rw-rw-rw-   0        0        0      138 2024-05-30 18:29:34.000000 prophet_tools-0.95/prophet_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      449 2024-05-30 18:29:34.000000 prophet_tools-0.95/prophet_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 18:29:34.000000 prophet_tools-0.95/prophet_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-02-12 01:48:06.000000 prophet_tools-0.95/prophet_tools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       14 2024-05-30 18:29:34.000000 prophet_tools-0.95/prophet_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 18:29:34.169403 prophet_tools-0.95/setup.cfg
+-rw-rw-rw-   0        0        0      241 2024-05-30 18:29:25.000000 prophet_tools-0.95/setup.py
```

### Comparing `prophet_tools-0.94/prophet_tools/file_convertors.py` & `prophet_tools-0.95/prophet_tools/file_convertors.py`

 * *Files 13% similar despite different names*

```diff
@@ -39,14 +39,19 @@
 def convert_CR2_to_JPG(path_from, path_to):
     from PIL import Image
 
     image = Image.open(path_from)
     rgb_image = image.convert('RGB')
     rgb_image.save(path_to)
 
+def image_resizer(path):
+    ffiles = mf.list_of_files(path,True)
+    files_to_resize = list(filter(lambda f: (f[-3:] == "jpg" or f[-4:] == "jpeg"), ffiles))
+    batch_image_resizer(files_to_resize,lim=size)
+
 if __name__ == '__main__':
     ppath = None
 
     while True:
         try:
             size = input("MAX SIZE OR FOLDER: ")
             if size[1:2] == ":":
```

### Comparing `prophet_tools-0.94/prophet_tools/my_functions.py` & `prophet_tools-0.95/prophet_tools/my_functions.py`

 * *Files identical despite different names*

### Comparing `prophet_tools-0.94/prophet_tools/terminal.py` & `prophet_tools-0.95/prophet_tools/terminal.py`

 * *Files identical despite different names*

### Comparing `prophet_tools-0.94/prophet_tools/всё_подряд.py` & `prophet_tools-0.95/prophet_tools/всё_подряд.py`

 * *Files identical despite different names*

