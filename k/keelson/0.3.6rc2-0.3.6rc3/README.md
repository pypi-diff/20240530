# Comparing `tmp/keelson-0.3.6rc2-py3-none-any.whl.zip` & `tmp/keelson-0.3.6rc3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5511 bytes, number of entries: 9
--rw-r--r--  2.0 unx     1236 b- defN 24-May-30 12:47 keelson/Envelope_pb2.py
--rw-r--r--  2.0 unx     3669 b- defN 24-May-30 12:47 keelson/__init__.py
--rw-r--r--  2.0 unx     3348 b- defN 24-May-30 12:47 keelson/codec.py
--rw-r--r--  2.0 unx     1659 b- defN 24-May-30 12:47 keelson/subjects.yaml
--rw-r--r--  2.0 unx     1081 b- defN 24-May-30 12:47 keelson-0.3.6rc2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-30 12:47 keelson-0.3.6rc2.dist-info/WHEEL
--rw-r--r--  2.0 unx      413 b- defN 24-May-30 12:47 keelson-0.3.6rc2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 24-May-30 12:47 keelson-0.3.6rc2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      715 b- defN 24-May-30 12:47 keelson-0.3.6rc2.dist-info/RECORD
-9 files, 12221 bytes uncompressed, 4281 bytes compressed:  65.0%
+Zip file size: 5510 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     1236 b- defN 24-May-30 13:02 keelson/Envelope_pb2.py
+-rw-r--r--  2.0 unx     3669 b- defN 24-May-30 13:01 keelson/__init__.py
+-rw-r--r--  2.0 unx     3348 b- defN 24-May-30 13:01 keelson/codec.py
+-rw-r--r--  2.0 unx     1659 b- defN 24-May-30 13:02 keelson/subjects.yaml
+-rw-r--r--  2.0 unx     1081 b- defN 24-May-30 13:02 keelson-0.3.6rc3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-30 13:02 keelson-0.3.6rc3.dist-info/WHEEL
+-rw-r--r--  2.0 unx      413 b- defN 24-May-30 13:02 keelson-0.3.6rc3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 24-May-30 13:02 keelson-0.3.6rc3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      715 b- defN 24-May-30 13:02 keelson-0.3.6rc3.dist-info/RECORD
+9 files, 12221 bytes uncompressed, 4280 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: keelson/codec.py
 Comment: 
 
 Filename: keelson/subjects.yaml
 Comment: 
 
-Filename: keelson-0.3.6rc2.dist-info/METADATA
+Filename: keelson-0.3.6rc3.dist-info/METADATA
 Comment: 
 
-Filename: keelson-0.3.6rc2.dist-info/WHEEL
+Filename: keelson-0.3.6rc3.dist-info/WHEEL
 Comment: 
 
-Filename: keelson-0.3.6rc2.dist-info/entry_points.txt
+Filename: keelson-0.3.6rc3.dist-info/entry_points.txt
 Comment: 
 
-Filename: keelson-0.3.6rc2.dist-info/top_level.txt
+Filename: keelson-0.3.6rc3.dist-info/top_level.txt
 Comment: 
 
-Filename: keelson-0.3.6rc2.dist-info/RECORD
+Filename: keelson-0.3.6rc3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `keelson-0.3.6rc2.dist-info/METADATA` & `keelson-0.3.6rc3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keelson
-Version: 0.3.6rc2
+Version: 0.3.6rc3
 Summary: A python Software Development Kit for keelson
 Home-page: https://github.com/MO-RISE/keelson/sdks/python
 Author: Fredrik Olsson
 Author-email: fredrik.x.olsson@ri.se
 Maintainer: Fredrik Olsson
 Maintainer-email: fredrik.x.olsson@ri.se
 License: Apache License 2.0
```

## Comparing `keelson-0.3.6rc2.dist-info/RECORD` & `keelson-0.3.6rc3.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 keelson/Envelope_pb2.py,sha256=_wvbnhRzFMR8svuPJPaWjBajaMU_gk0ozwXX0HlYgn0,1236
 keelson/__init__.py,sha256=0pWs0DZtNqiXjPRj6DcL71X8o4BrWKDXYeU4Wo6Vd2Y,3669
 keelson/codec.py,sha256=zNOLxe7pfix2elI7L0T3-qckK4WaXg9XSXNdQ9gHqoc,3348
 keelson/subjects.yaml,sha256=BWVyggJ39y5sRlVF-EGbWsc6tQai6V_Hb4al5gf53kk,1659
-keelson-0.3.6rc2.dist-info/METADATA,sha256=LMdMRb7h8jSwiPpDF4tJ0OZErXBPq1zgzGyOFPLbI44,1081
-keelson-0.3.6rc2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-keelson-0.3.6rc2.dist-info/entry_points.txt,sha256=zjUw7zUIUDruhRSSJGkA6jjvja2kMj07DKyARa9qn4I,413
-keelson-0.3.6rc2.dist-info/top_level.txt,sha256=CyBwGPhq3oBgFE9cp0fPTr9udD3jEM2NcHzx4K_0Z88,8
-keelson-0.3.6rc2.dist-info/RECORD,,
+keelson-0.3.6rc3.dist-info/METADATA,sha256=FrjuevSD-KWg10Gfs9knIUCmozkZB7EZbsZdAJlKNS8,1081
+keelson-0.3.6rc3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+keelson-0.3.6rc3.dist-info/entry_points.txt,sha256=zjUw7zUIUDruhRSSJGkA6jjvja2kMj07DKyARa9qn4I,413
+keelson-0.3.6rc3.dist-info/top_level.txt,sha256=CyBwGPhq3oBgFE9cp0fPTr9udD3jEM2NcHzx4K_0Z88,8
+keelson-0.3.6rc3.dist-info/RECORD,,
```

