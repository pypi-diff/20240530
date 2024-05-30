# Comparing `tmp/upm_micro_project_manager-0.4.1-py3-none-any.whl.zip` & `tmp/upm_micro_project_manager-0.4.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 10186 bytes, number of entries: 11
--rw-r--r--  2.0 unx      425 b- defN 24-May-29 04:30 upm/__init__.py
+Zip file size: 10194 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      425 b- defN 24-May-30 19:12 upm/__init__.py
 -rw-r--r--  2.0 unx     3032 b- defN 24-May-19 08:43 upm/cli.py
 -rw-r--r--  2.0 unx     1393 b- defN 23-Jan-04 14:36 upm/config.py
--rw-r--r--  2.0 unx     7930 b- defN 24-May-27 17:57 upm/template.py
+-rw-r--r--  2.0 unx     7929 b- defN 24-May-30 19:07 upm/template.py
 -rw-r--r--  2.0 unx     2677 b- defN 24-May-19 08:48 upm/upm.py
--rw-r--r--  2.0 unx     1491 b- defN 24-May-29 04:30 upm_micro_project_manager-0.4.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     5976 b- defN 24-May-29 04:30 upm_micro_project_manager-0.4.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-29 04:30 upm_micro_project_manager-0.4.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       37 b- defN 24-May-29 04:30 upm_micro_project_manager-0.4.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        4 b- defN 24-May-29 04:30 upm_micro_project_manager-0.4.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      935 b- defN 24-May-29 04:30 upm_micro_project_manager-0.4.1.dist-info/RECORD
-11 files, 23992 bytes uncompressed, 8588 bytes compressed:  64.2%
+-rw-r--r--  2.0 unx     1491 b- defN 24-May-30 19:12 upm_micro_project_manager-0.4.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5976 b- defN 24-May-30 19:12 upm_micro_project_manager-0.4.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-30 19:12 upm_micro_project_manager-0.4.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       37 b- defN 24-May-30 19:12 upm_micro_project_manager-0.4.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        4 b- defN 24-May-30 19:12 upm_micro_project_manager-0.4.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      935 b- defN 24-May-30 19:12 upm_micro_project_manager-0.4.2.dist-info/RECORD
+11 files, 23991 bytes uncompressed, 8596 bytes compressed:  64.2%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: upm/template.py
 Comment: 
 
 Filename: upm/upm.py
 Comment: 
 
-Filename: upm_micro_project_manager-0.4.1.dist-info/LICENSE
+Filename: upm_micro_project_manager-0.4.2.dist-info/LICENSE
 Comment: 
 
-Filename: upm_micro_project_manager-0.4.1.dist-info/METADATA
+Filename: upm_micro_project_manager-0.4.2.dist-info/METADATA
 Comment: 
 
-Filename: upm_micro_project_manager-0.4.1.dist-info/WHEEL
+Filename: upm_micro_project_manager-0.4.2.dist-info/WHEEL
 Comment: 
 
-Filename: upm_micro_project_manager-0.4.1.dist-info/entry_points.txt
+Filename: upm_micro_project_manager-0.4.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: upm_micro_project_manager-0.4.1.dist-info/top_level.txt
+Filename: upm_micro_project_manager-0.4.2.dist-info/top_level.txt
 Comment: 
 
-Filename: upm_micro_project_manager-0.4.1.dist-info/RECORD
+Filename: upm_micro_project_manager-0.4.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## upm/__init__.py

```diff
@@ -4,8 +4,8 @@
 # date         # 2022-12-02
 # ---------------------------------------------------------------------------
 # description  # a Template for files or directories
 #              #
 #              #
 ##############################################################################
 
-__version__ = "0.4.1"
+__version__ = "0.4.2"
```

## upm/template.py

```diff
@@ -34,39 +34,26 @@
         os.path.basename(filename)
         with open(filename) as fp:
             template = Template('')
             template.__values = json.load(fp)
             return template
 
     @staticmethod
-    def __get_parameters(path, template):
-        """ get the parameters of a template directory if neccessary
-        """
-        try:
-            with open(os.path.join(path, ".upmparams")) as fp:
-                logging.debug("reading parameter file")
-                data = json.load(fp)
-                logging.debug(data)
-                template["params"] = data
-        except:
-            pass
-
-    @staticmethod
     def scan(name, path, description='', _cpath='', _tmpl=None):
         """ scan a directory to create a template
         """
         logging.debug(f'scanning path {path}/{_cpath}')
         template = _tmpl if _tmpl is not None else Template(name, description)
 
         if _cpath == '':
             # we are in our first iteration, load parameter file
             logging.debug(
                 "loading template"
                 )
-            Template.__get_parameters(path, template)
+            template.__get_parameters(path)
 
         for file in os.listdir(os.path.join(path, _cpath)):
             # get all files in directory
             relpath = os.path.join(_cpath, file)
             filepath = os.path.join(path, relpath)
             if os.path.isdir(filepath):
                 # scan subdirs
@@ -83,17 +70,30 @@
 
     def __init__(self, name, description=''):
         """ initialize a template
         """
         self.__values = {
             'name': name,
             'description': description,
+            'params': {},
             'files': {}
             }
 
+    def __get_parameters(self, path):
+        """ get the parameters of a template directory if neccessary
+        """
+        try:
+            with open(os.path.join(path, ".upmparams")) as fp:
+                logging.debug("reading parameter file")
+                data = json.load(fp)
+                logging.debug(data)
+                self.__values["params"] = data
+        except:
+            pass
+
     def add_item(self, path, name, content=b''):
         """ create a directory path in files structure
         """
         files = self.files
         if path != '':
             directory = path.split('/')
             # create directory structure if neccessary
```

## Comparing `upm_micro_project_manager-0.4.1.dist-info/LICENSE` & `upm_micro_project_manager-0.4.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `upm_micro_project_manager-0.4.1.dist-info/METADATA` & `upm_micro_project_manager-0.4.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upm---micro-project-manager
-Version: 0.4.1
+Version: 0.4.2
 Summary: A simple project management system
 Home-page: https://gitlab.com/rapp.jens/upm
 Author: TecDroiD
 Author-email: rapp.jens+pypi@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

## Comparing `upm_micro_project_manager-0.4.1.dist-info/RECORD` & `upm_micro_project_manager-0.4.2.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-upm/__init__.py,sha256=_gke3ZaP6FWJGaXMWbqEGonSmpVUcNjVnmB4arW5GrA,425
+upm/__init__.py,sha256=0Qy9Pc6te8HOuoDw24JT5B3VNitK-qhSUKWjeUGL0d8,425
 upm/cli.py,sha256=ful9TwI1Run6mmnuCoFG8T7HFtIHf8laLISOv-UU0u0,3032
 upm/config.py,sha256=XwdUhnT9iULQTC887get4uiYfuGbFTze3FCvpi3LwzI,1393
-upm/template.py,sha256=zDq1uAt8P5f_soXl7TsvLiYrgx_QPn57swoN9zteCbU,7930
+upm/template.py,sha256=saQqEOxomX9p4vaBSq22-xP5Z0CGf6RBQVTewdweUes,7929
 upm/upm.py,sha256=hnvs2sT6LftQH9uVxvdkYhjGwG9biTk9p6JVkRJsbqU,2677
-upm_micro_project_manager-0.4.1.dist-info/LICENSE,sha256=EHAUKKvC1CprBW_Dc8wFf0XexkwlKr0qw6ukPtoGelg,1491
-upm_micro_project_manager-0.4.1.dist-info/METADATA,sha256=3561W_kzCt-mVRNMm-WVsi09qS63WBVd8TuISKLsCxM,5976
-upm_micro_project_manager-0.4.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-upm_micro_project_manager-0.4.1.dist-info/entry_points.txt,sha256=B0W-0-VAU6FgEXW61LdS4GabGY7D06S1dzvrhueD_Xk,37
-upm_micro_project_manager-0.4.1.dist-info/top_level.txt,sha256=11U8AqJeeTpaSBuvOlSpAhpRbpylgrOK_y3OjeW6Xoc,4
-upm_micro_project_manager-0.4.1.dist-info/RECORD,,
+upm_micro_project_manager-0.4.2.dist-info/LICENSE,sha256=EHAUKKvC1CprBW_Dc8wFf0XexkwlKr0qw6ukPtoGelg,1491
+upm_micro_project_manager-0.4.2.dist-info/METADATA,sha256=TwsE9wmnbD0GJsLzN3dx09ZOh-sBTqPlfYmtw6duxBA,5976
+upm_micro_project_manager-0.4.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+upm_micro_project_manager-0.4.2.dist-info/entry_points.txt,sha256=B0W-0-VAU6FgEXW61LdS4GabGY7D06S1dzvrhueD_Xk,37
+upm_micro_project_manager-0.4.2.dist-info/top_level.txt,sha256=11U8AqJeeTpaSBuvOlSpAhpRbpylgrOK_y3OjeW6Xoc,4
+upm_micro_project_manager-0.4.2.dist-info/RECORD,,
```

