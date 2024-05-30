# Comparing `tmp/restmapi-1.0.4.4-py3-none-any.whl.zip` & `tmp/restmapi-1.0.4.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 13895 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      341 b- defN 24-May-24 11:05 restmapi/__init__.py
+Zip file size: 13629 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      341 b- defN 24-May-24 14:35 restmapi/__init__.py
 -rw-rw-rw-  2.0 fat    52579 b- defN 24-May-24 10:58 restmapi/services.py
--rw-rw-rw-  2.0 fat        7 b- defN 24-May-24 11:05 restmapi/version.txt
--rw-rw-rw-  2.0 fat     1091 b- defN 24-May-24 11:05 restmapi-1.0.4.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1915 b- defN 24-May-24 11:05 restmapi-1.0.4.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-24 11:05 restmapi-1.0.4.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 24-May-24 11:05 restmapi-1.0.4.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      628 b- defN 24-May-24 11:05 restmapi-1.0.4.4.dist-info/RECORD
-8 files, 56662 bytes uncompressed, 12797 bytes compressed:  77.4%
+-rw-rw-rw-  2.0 fat        7 b- defN 24-May-24 14:35 restmapi/version.txt
+-rw-rw-rw-  2.0 fat     1091 b- defN 24-May-24 14:36 restmapi-1.0.4.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1255 b- defN 24-May-24 14:36 restmapi-1.0.4.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-24 14:36 restmapi-1.0.4.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 24-May-24 14:36 restmapi-1.0.4.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      628 b- defN 24-May-24 14:36 restmapi-1.0.4.5.dist-info/RECORD
+8 files, 56002 bytes uncompressed, 12531 bytes compressed:  77.6%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: restmapi/services.py
 Comment: 
 
 Filename: restmapi/version.txt
 Comment: 
 
-Filename: restmapi-1.0.4.4.dist-info/LICENSE
+Filename: restmapi-1.0.4.5.dist-info/LICENSE
 Comment: 
 
-Filename: restmapi-1.0.4.4.dist-info/METADATA
+Filename: restmapi-1.0.4.5.dist-info/METADATA
 Comment: 
 
-Filename: restmapi-1.0.4.4.dist-info/WHEEL
+Filename: restmapi-1.0.4.5.dist-info/WHEEL
 Comment: 
 
-Filename: restmapi-1.0.4.4.dist-info/top_level.txt
+Filename: restmapi-1.0.4.5.dist-info/top_level.txt
 Comment: 
 
-Filename: restmapi-1.0.4.4.dist-info/RECORD
+Filename: restmapi-1.0.4.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## restmapi/__init__.py

```diff
@@ -9,8 +9,8 @@
 	print(f"MAPI version: {MAPIServices.instance.get_version()}")
 
 
 __author__  = "Xavier Dourille <dourille@fev.com>"
 # __version__ added below by build pipeline
 
 
-__version__ = '1.0.4.4'
+__version__ = '1.0.4.5'
```

## restmapi/version.txt

```diff
@@ -1 +1 @@
-1.0.4.4
+1.0.4.5
```

## Comparing `restmapi-1.0.4.4.dist-info/LICENSE` & `restmapi-1.0.4.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `restmapi-1.0.4.4.dist-info/RECORD` & `restmapi-1.0.4.5.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-restmapi/__init__.py,sha256=jcgAYDrYRGYAB0OwNNdJbIhihibCoG6XEaxLHiseUZs,341
+restmapi/__init__.py,sha256=t2LUpREa9i_sJ8ddnguUL5TVOY1bTIpa-GSbZ3LqznM,341
 restmapi/services.py,sha256=bR4cJngbx1bu84yQIWuXxL1c-KE8rLs_PlhNGhoUQ20,52579
-restmapi/version.txt,sha256=Vn5rw0p65mKri05Fb6gQhR4EqOt4HYkJKvS0cIhp2zg,7
-restmapi-1.0.4.4.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-restmapi-1.0.4.4.dist-info/METADATA,sha256=XWyULrztV01f65jgSUqLmwh2ZM2seUBwJGc5xmWMovc,1915
-restmapi-1.0.4.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-restmapi-1.0.4.4.dist-info/top_level.txt,sha256=D-cK6tlXm8wsGjwd9PO_LI2M3lvwsgHX4euw7ifbbUM,9
-restmapi-1.0.4.4.dist-info/RECORD,,
+restmapi/version.txt,sha256=bRU0dvk9W-WbgSgLfGDBE4CRZ8lJvDNe4ImGSpltM84,7
+restmapi-1.0.4.5.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+restmapi-1.0.4.5.dist-info/METADATA,sha256=GGyIPlXvphk7fDoAAIrffjDs9QeoMONnZqmdMyJpIfU,1255
+restmapi-1.0.4.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+restmapi-1.0.4.5.dist-info/top_level.txt,sha256=D-cK6tlXm8wsGjwd9PO_LI2M3lvwsgHX4euw7ifbbUM,9
+restmapi-1.0.4.5.dist-info/RECORD,,
```

