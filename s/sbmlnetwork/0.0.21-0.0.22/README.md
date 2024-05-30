# Comparing `tmp/sbmlnetwork-0.0.21-py3-none-any.whl.zip` & `tmp/sbmlnetwork-0.0.22-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3229 bytes, number of entries: 7
--rw-r--r--  2.0 unx      104 b- defN 24-Apr-06 17:42 sbmlnetwork/__init__.py
--rw-r--r--  2.0 unx      962 b- defN 24-Apr-06 18:43 sbmlnetwork/sbmlnetwork.py
--rw-r--r--  2.0 unx     1084 b- defN 24-Apr-06 20:58 sbmlnetwork-0.0.21.dist-info/LICENSE
--rw-r--r--  2.0 unx     1259 b- defN 24-Apr-06 20:58 sbmlnetwork-0.0.21.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-06 20:58 sbmlnetwork-0.0.21.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 24-Apr-06 20:58 sbmlnetwork-0.0.21.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      572 b- defN 24-Apr-06 20:58 sbmlnetwork-0.0.21.dist-info/RECORD
-7 files, 4085 bytes uncompressed, 2209 bytes compressed:  45.9%
+Zip file size: 3224 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      104 b- defN 24-May-08 01:40 sbmlnetwork/__init__.py
+-rw-r--r--  2.0 unx      962 b- defN 24-May-08 01:40 sbmlnetwork/sbmlnetwork.py
+-rw-r--r--  2.0 unx     1084 b- defN 24-May-08 01:54 sbmlnetwork-0.0.22.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1259 b- defN 24-May-08 01:54 sbmlnetwork-0.0.22.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-08 01:54 sbmlnetwork-0.0.22.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-May-08 01:54 sbmlnetwork-0.0.22.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      572 b- defN 24-May-08 01:54 sbmlnetwork-0.0.22.dist-info/RECORD
+7 files, 4085 bytes uncompressed, 2204 bytes compressed:  46.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: sbmlnetwork/__init__.py
 Comment: 
 
 Filename: sbmlnetwork/sbmlnetwork.py
 Comment: 
 
-Filename: sbmlnetwork-0.0.21.dist-info/LICENSE
+Filename: sbmlnetwork-0.0.22.dist-info/LICENSE
 Comment: 
 
-Filename: sbmlnetwork-0.0.21.dist-info/METADATA
+Filename: sbmlnetwork-0.0.22.dist-info/METADATA
 Comment: 
 
-Filename: sbmlnetwork-0.0.21.dist-info/WHEEL
+Filename: sbmlnetwork-0.0.22.dist-info/WHEEL
 Comment: 
 
-Filename: sbmlnetwork-0.0.21.dist-info/top_level.txt
+Filename: sbmlnetwork-0.0.22.dist-info/top_level.txt
 Comment: 
 
-Filename: sbmlnetwork-0.0.21.dist-info/RECORD
+Filename: sbmlnetwork-0.0.22.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `sbmlnetwork-0.0.21.dist-info/LICENSE` & `sbmlnetwork-0.0.22.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sbmlnetwork-0.0.21.dist-info/METADATA` & `sbmlnetwork-0.0.22.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: sbmlnetwork
-Version: 0.0.21
+Version: 0.0.22
 Summary: A python api to work with libsbmlnetwork library
 Home-page: https://github.com/adelhpour/SBMLNetwork
 Author: Adel Heydarabadipour
 Author-email: adelhp@uw.edu
 Project-URL: Bug Tracker, https://github.com/adelhpour/SBMLNetwork/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: libsbmlnetwork >=0.0.18
-Requires-Dist: networkinfotranslator >=0.0.23
+Requires-Dist: libsbmlnetwork >=0.0.22
+Requires-Dist: networkinfotranslator >=0.0.24
 Requires-Dist: pillow
 
 # SBMLNetwork
 
 SBMLNetwork is a python package designed to visualize and edit SBML model networks. It uses libsbmlnetwork package, which employs an embedded force-directed autolayout algorithm to create aesthetically pleasing networks and utilizes SBML Layout and Render packages to store and retrieve visualization information of models. With its drawing tool and its comprehensive command-line API, users can generate and modify graphical representations of their SBML models, save the visual information of their model to SBML files or strings, and export rendered figures of their model in PDF, PNG, and JPG formats.
```

## Comparing `sbmlnetwork-0.0.21.dist-info/RECORD` & `sbmlnetwork-0.0.22.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 sbmlnetwork/__init__.py,sha256=yaTYN_SWt9c_LAgnNCSqqq5wBGPEZRujumNvj3choPc,104
 sbmlnetwork/sbmlnetwork.py,sha256=5jOca7edLkB6EXtFEb7E0ejMJW9RifIBOpT7eCJOdQ4,962
-sbmlnetwork-0.0.21.dist-info/LICENSE,sha256=gGnkw4gXz_FZnTTWOhvH4kGG_w3jDFAHlIE8ESRa-b4,1084
-sbmlnetwork-0.0.21.dist-info/METADATA,sha256=9843JuSZi7je3ye1Gi9vHXrs7nXjjYLV0lOXChvjwvI,1259
-sbmlnetwork-0.0.21.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-sbmlnetwork-0.0.21.dist-info/top_level.txt,sha256=n2VJnirWoFrbr61pdAjVKFaDBYgHB-2l0brB92WpAm8,12
-sbmlnetwork-0.0.21.dist-info/RECORD,,
+sbmlnetwork-0.0.22.dist-info/LICENSE,sha256=gGnkw4gXz_FZnTTWOhvH4kGG_w3jDFAHlIE8ESRa-b4,1084
+sbmlnetwork-0.0.22.dist-info/METADATA,sha256=ctR6BsXrDGDyBVUD29a5KQsuSTmhFyjENwp5-DCMPC0,1259
+sbmlnetwork-0.0.22.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+sbmlnetwork-0.0.22.dist-info/top_level.txt,sha256=n2VJnirWoFrbr61pdAjVKFaDBYgHB-2l0brB92WpAm8,12
+sbmlnetwork-0.0.22.dist-info/RECORD,,
```

