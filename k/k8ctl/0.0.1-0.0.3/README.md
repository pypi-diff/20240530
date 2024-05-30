# Comparing `tmp/k8ctl-0.0.1-py3-none-any.whl.zip` & `tmp/k8ctl-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,11 @@
-Zip file size: 5886 bytes, number of entries: 6
--rw-r--r--  2.0 unx    11357 b- defN 24-May-29 04:30 k8ctl-0.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1481 b- defN 24-May-29 04:30 k8ctl-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-29 04:30 k8ctl-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       38 b- defN 24-May-29 04:30 k8ctl-0.0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        1 b- defN 24-May-29 04:30 k8ctl-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      469 b- defN 24-May-29 04:30 k8ctl-0.0.1.dist-info/RECORD
-6 files, 13438 bytes uncompressed, 5034 bytes compressed:  62.5%
+Zip file size: 9965 bytes, number of entries: 9
+-rw-r--r--  2.0 unx        0 b- defN 24-May-30 05:37 k8ctl/__init__.py
+-rw-r--r--  2.0 unx     1200 b- defN 24-May-30 05:37 k8ctl/helper.py
+-rw-r--r--  2.0 unx    15374 b- defN 24-May-30 05:37 k8ctl/k8ctl.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-May-30 05:37 k8ctl-0.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1481 b- defN 24-May-30 05:37 k8ctl-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-30 05:37 k8ctl-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       38 b- defN 24-May-30 05:37 k8ctl-0.0.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 24-May-30 05:37 k8ctl-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      684 b- defN 24-May-30 05:37 k8ctl-0.0.3.dist-info/RECORD
+9 files, 30232 bytes uncompressed, 8793 bytes compressed:  70.9%
```

## zipnote {}

```diff
@@ -1,19 +1,28 @@
-Filename: k8ctl-0.0.1.dist-info/LICENSE
+Filename: k8ctl/__init__.py
 Comment: 
 
-Filename: k8ctl-0.0.1.dist-info/METADATA
+Filename: k8ctl/helper.py
 Comment: 
 
-Filename: k8ctl-0.0.1.dist-info/WHEEL
+Filename: k8ctl/k8ctl.py
 Comment: 
 
-Filename: k8ctl-0.0.1.dist-info/entry_points.txt
+Filename: k8ctl-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: k8ctl-0.0.1.dist-info/top_level.txt
+Filename: k8ctl-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: k8ctl-0.0.1.dist-info/RECORD
+Filename: k8ctl-0.0.3.dist-info/WHEEL
+Comment: 
+
+Filename: k8ctl-0.0.3.dist-info/entry_points.txt
+Comment: 
+
+Filename: k8ctl-0.0.3.dist-info/top_level.txt
+Comment: 
+
+Filename: k8ctl-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `k8ctl-0.0.1.dist-info/LICENSE` & `k8ctl-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `k8ctl-0.0.1.dist-info/METADATA` & `k8ctl-0.0.3.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k8ctl
-Version: 0.0.1
+Version: 0.0.3
 Author: Kishorekarthik P
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 
 # k8ctl
```

