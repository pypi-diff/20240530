# Comparing `tmp/k8ctl-0.0.4-py3-none-any.whl.zip` & `tmp/k8ctl-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,8 @@
-Zip file size: 10127 bytes, number of entries: 9
--rw-r--r--  2.0 unx        0 b- defN 24-May-30 10:24 k8ctl/__init__.py
--rw-r--r--  2.0 unx     1246 b- defN 24-May-30 10:24 k8ctl/helper.py
--rw-r--r--  2.0 unx    16623 b- defN 24-May-30 10:24 k8ctl/k8ctl.py
--rw-r--r--  2.0 unx    11357 b- defN 24-May-30 10:24 k8ctl-0.0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     1481 b- defN 24-May-30 10:24 k8ctl-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-30 10:24 k8ctl-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       38 b- defN 24-May-30 10:24 k8ctl-0.0.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 24-May-30 10:24 k8ctl-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      684 b- defN 24-May-30 10:24 k8ctl-0.0.4.dist-info/RECORD
-9 files, 31527 bytes uncompressed, 8955 bytes compressed:  71.6%
+Zip file size: 5888 bytes, number of entries: 6
+-rw-r--r--  2.0 unx    11357 b- defN 24-May-30 10:51 k8ctl-0.0.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1481 b- defN 24-May-30 10:51 k8ctl-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-30 10:51 k8ctl-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       38 b- defN 24-May-30 10:51 k8ctl-0.0.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-May-30 10:51 k8ctl-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      469 b- defN 24-May-30 10:51 k8ctl-0.0.5.dist-info/RECORD
+6 files, 13438 bytes uncompressed, 5036 bytes compressed:  62.5%
```

## zipnote {}

```diff
@@ -1,28 +1,19 @@
-Filename: k8ctl/__init__.py
+Filename: k8ctl-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: k8ctl/helper.py
+Filename: k8ctl-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: k8ctl/k8ctl.py
+Filename: k8ctl-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: k8ctl-0.0.4.dist-info/LICENSE
+Filename: k8ctl-0.0.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: k8ctl-0.0.4.dist-info/METADATA
+Filename: k8ctl-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: k8ctl-0.0.4.dist-info/WHEEL
-Comment: 
-
-Filename: k8ctl-0.0.4.dist-info/entry_points.txt
-Comment: 
-
-Filename: k8ctl-0.0.4.dist-info/top_level.txt
-Comment: 
-
-Filename: k8ctl-0.0.4.dist-info/RECORD
+Filename: k8ctl-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `k8ctl-0.0.4.dist-info/LICENSE` & `k8ctl-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `k8ctl-0.0.4.dist-info/METADATA` & `k8ctl-0.0.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k8ctl
-Version: 0.0.4
+Version: 0.0.5
 Author: Kishorekarthik P
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 
 # k8ctl
```

