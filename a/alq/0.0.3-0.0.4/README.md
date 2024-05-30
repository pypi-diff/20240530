# Comparing `tmp/alq-0.0.3-py3-none-any.whl.zip` & `tmp/alq-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6769 bytes, number of entries: 9
--rwxr-xr-x  2.0 unx      292 b- defN 24-May-22 07:06 alq-0.0.3.data/scripts/alq
+Zip file size: 6771 bytes, number of entries: 9
+-rwxr-xr-x  2.0 unx      292 b- defN 24-May-30 09:00 alq-0.0.4.data/scripts/alq
 -rw-r--r--  2.0 unx        0 b- defN 24-Apr-08 02:29 subfunctions/__init__.py
 -rw-r--r--  2.0 unx     2177 b- defN 24-May-13 08:50 subfunctions/configuration.py
 -rw-r--r--  2.0 unx     3490 b- defN 24-May-22 07:01 subfunctions/fileSystem.py
 -rw-r--r--  2.0 unx     9877 b- defN 24-May-22 07:05 subfunctions/owncloud.py
--rw-r--r--  2.0 unx      217 b- defN 24-May-22 07:06 alq-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-22 07:06 alq-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 24-May-22 07:06 alq-0.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      691 b- defN 24-May-22 07:06 alq-0.0.3.dist-info/RECORD
-9 files, 16849 bytes uncompressed, 5581 bytes compressed:  66.9%
+-rw-r--r--  2.0 unx      219 b- defN 24-May-30 09:00 alq-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-30 09:00 alq-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-May-30 09:00 alq-0.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      691 b- defN 24-May-30 09:00 alq-0.0.4.dist-info/RECORD
+9 files, 16851 bytes uncompressed, 5583 bytes compressed:  66.9%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
-Filename: alq-0.0.3.data/scripts/alq
+Filename: alq-0.0.4.data/scripts/alq
 Comment: 
 
 Filename: subfunctions/__init__.py
 Comment: 
 
 Filename: subfunctions/configuration.py
 Comment: 
 
 Filename: subfunctions/fileSystem.py
 Comment: 
 
 Filename: subfunctions/owncloud.py
 Comment: 
 
-Filename: alq-0.0.3.dist-info/METADATA
+Filename: alq-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: alq-0.0.3.dist-info/WHEEL
+Filename: alq-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: alq-0.0.3.dist-info/top_level.txt
+Filename: alq-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: alq-0.0.3.dist-info/RECORD
+Filename: alq-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `alq-0.0.3.dist-info/RECORD` & `alq-0.0.4.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-alq-0.0.3.data/scripts/alq,sha256=2eSh245C29cfJLTbDW3lcX5SpTeCy4RXM27h2ds-eqQ,292
+alq-0.0.4.data/scripts/alq,sha256=2eSh245C29cfJLTbDW3lcX5SpTeCy4RXM27h2ds-eqQ,292
 subfunctions/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 subfunctions/configuration.py,sha256=up7NE9oPB4OJeLiax878EwF_JwuXJn1mBozu0sW5Hx8,2177
 subfunctions/fileSystem.py,sha256=4n-ditDaah40FTfMFGyGYfmYJwSCqZwbQX6Pbwtjqt8,3490
 subfunctions/owncloud.py,sha256=RgIQMq3lAICIXLJ45mLliXEi0nvziDnhxb7zOjC41Iw,9877
-alq-0.0.3.dist-info/METADATA,sha256=G6bwjeSKt83q5Bkjq1T3PtAbaxg9k3v-ZRsj8_0RYoM,217
-alq-0.0.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-alq-0.0.3.dist-info/top_level.txt,sha256=cj_wvsgatO_VDmqNS0IE7dJSF0CTwS6lwvbgnpfPtiI,13
-alq-0.0.3.dist-info/RECORD,,
+alq-0.0.4.dist-info/METADATA,sha256=z3y-EpJrubhZWqOcRnRaxwYWfpdCFRdn-nOoeNcX5pY,219
+alq-0.0.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+alq-0.0.4.dist-info/top_level.txt,sha256=cj_wvsgatO_VDmqNS0IE7dJSF0CTwS6lwvbgnpfPtiI,13
+alq-0.0.4.dist-info/RECORD,,
```

