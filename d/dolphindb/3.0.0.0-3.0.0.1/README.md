# Comparing `tmp/dolphindb-3.0.0.0-cp39-cp39-win_amd64.whl.zip` & `tmp/dolphindb-3.0.0.1-cp310-cp310-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 1633014 bytes, number of entries: 16
--rw-rw-rw-  2.0 fat     1944 b- defN 24-Mar-30 02:24 dolphindb/__init__.py
--rw-rw-rw-  2.0 fat  4225536 b- defN 24-Apr-01 06:12 dolphindb/_dolphindbcpp.cp39-win_amd64.pyd
+Zip file size: 1633076 bytes, number of entries: 16
+-rw-rw-rw-  2.0 fat     1944 b- defN 24-May-28 01:21 dolphindb/__init__.py
+-rw-rw-rw-  2.0 fat  4225536 b- defN 24-May-28 08:31 dolphindb/_dolphindbcpp.cp310-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    12109 b- defN 24-Apr-01 04:13 dolphindb/cep.py
 -rw-rw-rw-  2.0 fat     6490 b- defN 23-Oct-12 02:33 dolphindb/database.py
 -rw-rw-rw-  2.0 fat    69400 b- defN 24-Mar-30 03:26 dolphindb/session.py
 -rw-rw-rw-  2.0 fat     4821 b- defN 24-Mar-30 06:37 dolphindb/settings.py
--rw-rw-rw-  2.0 fat    86085 b- defN 24-Jan-29 02:52 dolphindb/table.py
+-rw-rw-rw-  2.0 fat    86085 b- defN 24-May-27 06:35 dolphindb/table.py
 -rw-rw-rw-  2.0 fat     3513 b- defN 24-Mar-30 06:37 dolphindb/typing.py
 -rw-rw-rw-  2.0 fat     1216 b- defN 24-Jan-25 09:38 dolphindb/utils.py
 -rw-rw-rw-  2.0 fat     7146 b- defN 24-Jan-11 01:35 dolphindb/vector.py
 -rw-rw-rw-  2.0 fat      551 b- defN 24-Mar-22 01:18 dolphindb/_core/__init__.py
--rw-rw-rw-  2.0 fat    11596 b- defN 24-Apr-01 06:12 dolphindb-3.0.0.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1840 b- defN 24-Apr-01 06:12 dolphindb-3.0.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-01 06:12 dolphindb-3.0.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 24-Apr-01 06:12 dolphindb-3.0.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1282 b- defN 24-Apr-01 06:12 dolphindb-3.0.0.0.dist-info/RECORD
-16 files, 4433639 bytes uncompressed, 1630934 bytes compressed:  63.2%
+-rw-rw-rw-  2.0 fat    11596 b- defN 24-May-28 08:31 dolphindb-3.0.0.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1840 b- defN 24-May-28 08:31 dolphindb-3.0.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      102 b- defN 24-May-28 08:31 dolphindb-3.0.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 24-May-28 08:31 dolphindb-3.0.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1283 b- defN 24-May-28 08:31 dolphindb-3.0.0.1.dist-info/RECORD
+16 files, 4433642 bytes uncompressed, 1630994 bytes compressed:  63.2%
```

## zipnote {}

```diff
@@ -1,11 +1,11 @@
 Filename: dolphindb/__init__.py
 Comment: 
 
-Filename: dolphindb/_dolphindbcpp.cp39-win_amd64.pyd
+Filename: dolphindb/_dolphindbcpp.cp310-win_amd64.pyd
 Comment: 
 
 Filename: dolphindb/cep.py
 Comment: 
 
 Filename: dolphindb/database.py
 Comment: 
@@ -27,23 +27,23 @@
 
 Filename: dolphindb/vector.py
 Comment: 
 
 Filename: dolphindb/_core/__init__.py
 Comment: 
 
-Filename: dolphindb-3.0.0.0.dist-info/LICENSE
+Filename: dolphindb-3.0.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: dolphindb-3.0.0.0.dist-info/METADATA
+Filename: dolphindb-3.0.0.1.dist-info/METADATA
 Comment: 
 
-Filename: dolphindb-3.0.0.0.dist-info/WHEEL
+Filename: dolphindb-3.0.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: dolphindb-3.0.0.0.dist-info/top_level.txt
+Filename: dolphindb-3.0.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: dolphindb-3.0.0.0.dist-info/RECORD
+Filename: dolphindb-3.0.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dolphindb/__init__.py

```diff
@@ -15,15 +15,15 @@
 from .table import Table, TableUpdate, TableDelete, TableGroupby, TablePivotBy, TableContextby, Counter
 from .table import wavg, wsum, covar, corr, count, max, min, sum, sum2, size, avg, std, prod, var, first, last
 from .table import eachPre, cumsum, cumprod, cummax, cummin
 from .vector import Vector, FilterCond
 from .database import Database
 from .utils import month
 
-__version__ = "3.0.0.0"
+__version__ = "3.0.0.1"
 
 name = "dolphindb"
 
 __all__ = [
     "Session", "session",
     "DBConnectionPool",
     "BlockReader",
```

## Comparing `dolphindb-3.0.0.0.dist-info/LICENSE` & `dolphindb-3.0.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dolphindb-3.0.0.0.dist-info/METADATA` & `dolphindb-3.0.0.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolphindb
-Version: 3.0.0.0
+Version: 3.0.0.1
 Summary: A C++ boosted DolphinDB Python API based on Pybind11
 Home-page: https://www.dolphindb.com
 Author: DolphinDB, Inc.
 Author-email: support@dolphindb.com
 License: DolphinDB
 Platform: Windows
 Platform: MacOS
```

## Comparing `dolphindb-3.0.0.0.dist-info/RECORD` & `dolphindb-3.0.0.1.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-dolphindb/__init__.py,sha256=11U4NRz5CKs4gvwEWEt2lvYN1htXKxzECUrahWJne54,1944
-dolphindb/_dolphindbcpp.cp39-win_amd64.pyd,sha256=wX-Kxareg-7RNieV72giOqsC_PSPl93RDd6EQXDTbMM,4225536
+dolphindb/__init__.py,sha256=ujj683KyIYI74fwxF_zzOGLRqK2O0OngxURQJAqjl6g,1944
+dolphindb/_dolphindbcpp.cp310-win_amd64.pyd,sha256=NWIwLu7tMcG-6wjbLXg75CK3YcjonH-06qRzQT-YDwU,4225536
 dolphindb/cep.py,sha256=UOTq-NcuOnioLF1W0OxV79L_tR92I0tZ0gmts9qkxaQ,12109
 dolphindb/database.py,sha256=CVHEO1Mu3XzeNJIbXjcTBjhSfq-tzJJMaysL6obZGLw,6490
 dolphindb/session.py,sha256=Ep5dPx1mkByLXGYkgrXSe1GddmEpLRYd54I-TcmObdg,69400
 dolphindb/settings.py,sha256=0V_l93BbLtua4btMqBymP4aVL6udCCNPo9bLs_LKP18,4821
 dolphindb/table.py,sha256=8l85vOPPIiepti56u-BIYNhdDUOxtkyCCTD8vgAQ7rk,86085
 dolphindb/typing.py,sha256=JiyjjNzzseIwHvKAqlP04xwTTh2x-Yz7eH_nZi20dCk,3513
 dolphindb/utils.py,sha256=17pxGaEBObuMou26Ag9XYxUyo6yIq4mRKkf-REx66xw,1216
 dolphindb/vector.py,sha256=pBJSz7DvPv0MPB6iXtBqVSYYMlEct9QCji2EVGb1aJA,7146
 dolphindb/_core/__init__.py,sha256=XsmxlCQM8zR7DUFlfK_VW8SkWBe2n5Vk5WTlhBBQIBM,551
-dolphindb-3.0.0.0.dist-info/LICENSE,sha256=3G-4_VJXNLVIIF3fWcAOpS4EBGoZm2Y78XVyaHTnD68,11596
-dolphindb-3.0.0.0.dist-info/METADATA,sha256=adlTehzKbr_Q1XfA6GZ9Y5cV-5dS1RvHgEJUcgNIsvk,1840
-dolphindb-3.0.0.0.dist-info/WHEEL,sha256=Z6c-bE0pUM47a70GvqO_SvH_XXU0lm62gEAKtoNJ08A,100
-dolphindb-3.0.0.0.dist-info/top_level.txt,sha256=ArqNhkrWzBZ8ppUhSY2qAFwLDocCp2QCgXXh5v8hOkc,10
-dolphindb-3.0.0.0.dist-info/RECORD,,
+dolphindb-3.0.0.1.dist-info/LICENSE,sha256=3G-4_VJXNLVIIF3fWcAOpS4EBGoZm2Y78XVyaHTnD68,11596
+dolphindb-3.0.0.1.dist-info/METADATA,sha256=u1hW7quXK72tB74ZOqnmOz9-Ublk75U7H-Gyx9odGTo,1840
+dolphindb-3.0.0.1.dist-info/WHEEL,sha256=lO6CqtLHCAi38X3Es1a4R1lAjZFvN010IMRCFo2S7Mc,102
+dolphindb-3.0.0.1.dist-info/top_level.txt,sha256=ArqNhkrWzBZ8ppUhSY2qAFwLDocCp2QCgXXh5v8hOkc,10
+dolphindb-3.0.0.1.dist-info/RECORD,,
```

