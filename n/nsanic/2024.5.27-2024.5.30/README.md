# Comparing `tmp/nsanic-2024.5.27-py3-none-any.whl.zip` & `tmp/nsanic-2024.5.30-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 59391 bytes, number of entries: 42
+Zip file size: 59390 bytes, number of entries: 42
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-19 13:56 nsanic/__init__.py
 -rw-rw-rw-  2.0 fat     3462 b- defN 24-May-16 07:52 nsanic/base_blue.py
 -rw-rw-rw-  2.0 fat     8536 b- defN 24-May-16 07:52 nsanic/base_conf.py
 -rw-rw-rw-  2.0 fat     3241 b- defN 24-May-16 07:52 nsanic/base_server.py
 -rw-rw-rw-  2.0 fat     9666 b- defN 24-May-16 07:52 nsanic/base_ws.py
 -rw-rw-rw-  2.0 fat     2908 b- defN 24-May-16 07:52 nsanic/exception.py
 -rw-rw-rw-  2.0 fat     7704 b- defN 24-May-27 03:10 nsanic/handler_http.py
 -rw-rw-rw-  2.0 fat     2727 b- defN 24-May-16 07:52 nsanic/handler_ws.py
 -rw-rw-rw-  2.0 fat      576 b- defN 24-May-16 07:52 nsanic/middleware.py
 -rw-rw-rw-  2.0 fat    10352 b- defN 24-May-16 07:52 nsanic/mult_creator.py
--rw-rw-rw-  2.0 fat     8531 b- defN 24-May-16 07:52 nsanic/verify.py
+-rw-rw-rw-  2.0 fat     8531 b- defN 24-May-30 03:29 nsanic/verify.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-19 13:56 nsanic/libs/__init__.py
 -rw-rw-rw-  2.0 fat     7656 b- defN 24-May-16 07:52 nsanic/libs/base_timed.py
 -rw-rw-rw-  2.0 fat     1276 b- defN 24-May-16 07:52 nsanic/libs/component.py
 -rw-rw-rw-  2.0 fat     3151 b- defN 24-Apr-28 08:45 nsanic/libs/consts.py
 -rw-rw-rw-  2.0 fat     1578 b- defN 24-Mar-21 14:40 nsanic/libs/crypto.py
 -rw-rw-rw-  2.0 fat     3171 b- defN 24-May-16 07:52 nsanic/libs/decorator.py
 -rw-rw-rw-  2.0 fat     1125 b- defN 24-Mar-21 14:40 nsanic/libs/file_type.py
@@ -31,14 +31,14 @@
 -rw-rw-rw-  2.0 fat    18726 b- defN 24-May-16 07:52 nsanic/orm/db_model.py
 -rw-rw-rw-  2.0 fat    11698 b- defN 24-Apr-03 07:45 nsanic/orm/mssql_generator.py
 -rw-rw-rw-  2.0 fat    11743 b- defN 24-Apr-28 08:44 nsanic/orm/mysql_generator.py
 -rw-rw-rw-  2.0 fat    11720 b- defN 24-Apr-03 07:45 nsanic/orm/pgsql_generator.py
 -rw-rw-rw-  2.0 fat     5037 b- defN 24-May-16 07:52 nsanic/orm/rc_model.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-19 13:56 test/__init__.py
 -rw-rw-rw-  2.0 fat      701 b- defN 24-May-16 07:52 test/test_unit.py
--rw-rw-rw-  2.0 fat     1090 b- defN 24-May-27 03:10 nsanic-2024.5.27.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4803 b- defN 24-May-27 03:10 nsanic-2024.5.27.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-27 03:10 nsanic-2024.5.27.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       52 b- defN 24-May-27 03:10 nsanic-2024.5.27.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       12 b- defN 24-May-27 03:10 nsanic-2024.5.27.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     3332 b- defN 24-May-27 03:10 nsanic-2024.5.27.dist-info/RECORD
-42 files, 183160 bytes uncompressed, 54161 bytes compressed:  70.4%
+-rw-rw-rw-  2.0 fat     1090 b- defN 24-May-30 03:30 nsanic-2024.5.30.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4803 b- defN 24-May-30 03:30 nsanic-2024.5.30.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-30 03:30 nsanic-2024.5.30.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       52 b- defN 24-May-30 03:30 nsanic-2024.5.30.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       12 b- defN 24-May-30 03:30 nsanic-2024.5.30.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     3332 b- defN 24-May-30 03:30 nsanic-2024.5.30.dist-info/RECORD
+42 files, 183160 bytes uncompressed, 54160 bytes compressed:  70.4%
```

## zipnote {}

```diff
@@ -102,26 +102,26 @@
 
 Filename: test/__init__.py
 Comment: 
 
 Filename: test/test_unit.py
 Comment: 
 
-Filename: nsanic-2024.5.27.dist-info/LICENSE
+Filename: nsanic-2024.5.30.dist-info/LICENSE
 Comment: 
 
-Filename: nsanic-2024.5.27.dist-info/METADATA
+Filename: nsanic-2024.5.30.dist-info/METADATA
 Comment: 
 
-Filename: nsanic-2024.5.27.dist-info/WHEEL
+Filename: nsanic-2024.5.30.dist-info/WHEEL
 Comment: 
 
-Filename: nsanic-2024.5.27.dist-info/entry_points.txt
+Filename: nsanic-2024.5.30.dist-info/entry_points.txt
 Comment: 
 
-Filename: nsanic-2024.5.27.dist-info/top_level.txt
+Filename: nsanic-2024.5.30.dist-info/top_level.txt
 Comment: 
 
-Filename: nsanic-2024.5.27.dist-info/RECORD
+Filename: nsanic-2024.5.30.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nsanic/verify.py

```diff
@@ -98,15 +98,15 @@
             return False, f'{p_name}参数值无法解析成整形'
     if inner:
         if (minval is not None) and (val < minval):
             return False, f'{p_name}参数值小于限制的最小值:{minval}'
         if (maxval is not None) and (val > maxval):
             return False, f'{p_name}参数值大于限制的最大值:{maxval}'
     else:
-        if (maxval is not None) and (maxval is not None) and (minval < val < maxval):
+        if (minval is not None) and (maxval is not None) and (minval < val < maxval):
             return False, f'{p_name}参数值不在指定的限制范围'
     return True, val
 
 
 def vstr(val, require=False, default: str = None, turn=0, minlen: int = None, maxlen: int = None, p_name=''):
     """
     字符串参数校验
@@ -177,15 +177,15 @@
         return True, val
     if inner:
         if (maxval is not None) and (val > maxval):
             return False, f'{p_name}参数值大于限制的最大值:{maxval}'
         if (minval is not None) and (val < minval):
             return False, f'{p_name}参数值小于限制的最小值:{minval}'
     else:
-        if (maxval is not None) and (maxval is not None) and (minval < val < maxval):
+        if (minval is not None) and (maxval is not None) and (minval < val < maxval):
             return False, f'{p_name}参数值不在指定的限制范围'
     return True, val
 
 
 def vdatetime(
         val,
         require=False,
```

## Comparing `nsanic-2024.5.27.dist-info/LICENSE` & `nsanic-2024.5.30.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `nsanic-2024.5.27.dist-info/METADATA` & `nsanic-2024.5.30.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsanic
-Version: 2024.5.27
+Version: 2024.5.30
 Summary: A web framework who is use sanic + tortoise-orm + redis to quick create http&websocket server.
 Author: DHDONG
 Author-email: zscych@qq.com
 License: MIT
 Keywords: WebServer,Sanic,WebSite Develop,Web Framework
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

## Comparing `nsanic-2024.5.27.dist-info/RECORD` & `nsanic-2024.5.30.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 nsanic/base_server.py,sha256=gBe2mYNXe9a1jKQKBBmck-89_yoctWHoTOT0sKXz_jg,3241
 nsanic/base_ws.py,sha256=1Q2BeULQRPLd2Fpe4oDGN3ygB31qFSICts0enzZt154,9666
 nsanic/exception.py,sha256=PXrcflYcbyD_AN4gNQEEfiZFOTEcAUV46FTEnVHApGc,2908
 nsanic/handler_http.py,sha256=WorCMGofJVX5TWLba3yTUEh0qs-OBt6zlNXRHAWhJco,7704
 nsanic/handler_ws.py,sha256=6N2OEYgP4ZtNi0mzEYbq1JNf5yPBiK-LRC1E96mfygs,2727
 nsanic/middleware.py,sha256=ic_aSDWJl-Vt1k-w9O_ixd_qf5R-Xoy3DnMtdU79y2Q,576
 nsanic/mult_creator.py,sha256=roZLTg_CaRmTVqVuep5AS-eCZU00-ytB6e3BGwqd7ik,10352
-nsanic/verify.py,sha256=hHwff_FMZyZoihzXzl68FkUyOu6YQ-uqKPm1zTNXwYU,8531
+nsanic/verify.py,sha256=rsrZQ8O0KjyheQ9MWfQMExm6XDp2aDjlhNalka4zLh4,8531
 nsanic/libs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nsanic/libs/base_timed.py,sha256=Qrs0OpRhHROW3-g2gFwMiw0oi8SnGgaY9TrGXLJS_E4,7656
 nsanic/libs/component.py,sha256=gxLOAyL1F4zGqJEYeskzV3E3FgeEIZnN3gzD4EgNGZQ,1276
 nsanic/libs/consts.py,sha256=OHIOgaLY8R8jZRiwDeEDg_3NN7kj-gZ_7HnP6Ccoq4c,3151
 nsanic/libs/crypto.py,sha256=rCuzGGGYSZimdd8OhQCfIdZBUbBnX0FdPNO3sivy1L4,1578
 nsanic/libs/decorator.py,sha256=l5uNOJUM6AXPAfSNer7uy-2ivXJc-yUytbwBxQ-jCSs,3171
 nsanic/libs/file_type.py,sha256=4OBdtXoNedXYpucs_99VdPfQw_Of6d8XFsRtTbGi8k0,1125
@@ -30,13 +30,13 @@
 nsanic/orm/db_model.py,sha256=Mo9UcXZM2u2i7PvT-crmqln7VCSyrll3wmvntGFcBnM,18726
 nsanic/orm/mssql_generator.py,sha256=c9q71hljWqBxoNriG0OefwD48w3gVTb62HnFKjreom4,11698
 nsanic/orm/mysql_generator.py,sha256=6AMVa9twa7GRCuTlEga5g2zHJvkCD9YocUwGGcvLQ4Q,11743
 nsanic/orm/pgsql_generator.py,sha256=BMNDAZ-2X9dPbUOBlhR5UJBfqXWpl23KRgTozleKCCQ,11720
 nsanic/orm/rc_model.py,sha256=Rk687YpLZp6XR42UzspTrOVlotlEAlp53RDRfYnlDG8,5037
 test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 test/test_unit.py,sha256=ru4EliRtBozPFs9UjVTybZ0cMUFtOgjS8FSdNnQFtO4,701
-nsanic-2024.5.27.dist-info/LICENSE,sha256=GSAKapQH5ZIGWlpQTA7v5YrfECyaxaohUb1vJX-qepw,1090
-nsanic-2024.5.27.dist-info/METADATA,sha256=koACjclt9y0jkHPtMRvq4JMQ7_fIwPfuonmoSPhlzMs,4803
-nsanic-2024.5.27.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-nsanic-2024.5.27.dist-info/entry_points.txt,sha256=NJGRx7PJixNk9kbISqsD8AGtQHq1NppCxvEsfEPx43Q,52
-nsanic-2024.5.27.dist-info/top_level.txt,sha256=Y7ottGiwpMZQKgvVy-Jy3SBJdxMFJSJ8ivpRD-c23xI,12
-nsanic-2024.5.27.dist-info/RECORD,,
+nsanic-2024.5.30.dist-info/LICENSE,sha256=GSAKapQH5ZIGWlpQTA7v5YrfECyaxaohUb1vJX-qepw,1090
+nsanic-2024.5.30.dist-info/METADATA,sha256=54Vi-Z1LZpkIjIqly-pu1xignmnptUurwP26bwNGsWU,4803
+nsanic-2024.5.30.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+nsanic-2024.5.30.dist-info/entry_points.txt,sha256=NJGRx7PJixNk9kbISqsD8AGtQHq1NppCxvEsfEPx43Q,52
+nsanic-2024.5.30.dist-info/top_level.txt,sha256=Y7ottGiwpMZQKgvVy-Jy3SBJdxMFJSJ8ivpRD-c23xI,12
+nsanic-2024.5.30.dist-info/RECORD,,
```

