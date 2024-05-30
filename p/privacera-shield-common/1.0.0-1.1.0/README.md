# Comparing `tmp/privacera_shield_common-1.0.0-py3-none-any.whl.zip` & `tmp/privacera_shield_common-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,13 @@
-Zip file size: 8083 bytes, number of entries: 9
+Zip file size: 10121 bytes, number of entries: 11
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 privacera_shield_common/__init__.py
 -rw-r--r--  2.0 unx     9149 b- defN 20-Feb-02 00:00 privacera_shield_common/audit_spooler.py
+-rw-r--r--  2.0 unx     2183 b- defN 20-Feb-02 00:00 privacera_shield_common/config_utils.py
 -rw-r--r--  2.0 unx     5931 b- defN 20-Feb-02 00:00 privacera_shield_common/encryption.py
 -rw-r--r--  2.0 unx     2551 b- defN 20-Feb-02 00:00 privacera_shield_common/file_utils.py
 -rw-r--r--  2.0 unx     2738 b- defN 20-Feb-02 00:00 privacera_shield_common/http_transport.py
-?rw-r--r--  2.0 unx      879 b- defN 20-Feb-02 00:00 privacera_shield_common-1.0.0.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 privacera_shield_common-1.0.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx      294 b- defN 20-Feb-02 00:00 privacera_shield_common-1.0.0.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      837 b- defN 20-Feb-02 00:00 privacera_shield_common-1.0.0.dist-info/RECORD
-9 files, 22466 bytes uncompressed, 6607 bytes compressed:  70.6%
+-rw-r--r--  2.0 unx     3763 b- defN 20-Feb-02 00:00 privacera_shield_common/lru_cache.py
+?rw-r--r--  2.0 unx      913 b- defN 20-Feb-02 00:00 privacera_shield_common-1.1.0.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 privacera_shield_common-1.1.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx      294 b- defN 20-Feb-02 00:00 privacera_shield_common-1.1.0.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     1026 b- defN 20-Feb-02 00:00 privacera_shield_common-1.1.0.dist-info/RECORD
+11 files, 28635 bytes uncompressed, 8343 bytes compressed:  70.9%
```

## zipnote {}

```diff
@@ -1,28 +1,34 @@
 Filename: privacera_shield_common/__init__.py
 Comment: 
 
 Filename: privacera_shield_common/audit_spooler.py
 Comment: 
 
+Filename: privacera_shield_common/config_utils.py
+Comment: 
+
 Filename: privacera_shield_common/encryption.py
 Comment: 
 
 Filename: privacera_shield_common/file_utils.py
 Comment: 
 
 Filename: privacera_shield_common/http_transport.py
 Comment: 
 
-Filename: privacera_shield_common-1.0.0.dist-info/METADATA
+Filename: privacera_shield_common/lru_cache.py
+Comment: 
+
+Filename: privacera_shield_common-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: privacera_shield_common-1.0.0.dist-info/WHEEL
+Filename: privacera_shield_common-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: privacera_shield_common-1.0.0.dist-info/licenses/LICENSE
+Filename: privacera_shield_common-1.1.0.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: privacera_shield_common-1.0.0.dist-info/RECORD
+Filename: privacera_shield_common-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `privacera_shield_common-1.0.0.dist-info/METADATA` & `privacera_shield_common-1.1.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.3
 Name: privacera_shield_common
-Version: 1.0.0
+Version: 1.1.0
 Summary: Privacera AI Governance (PAIG) Shield Common Library
 Project-URL: Homepage, https://github.com/pypa/privacera_shield_common
 Project-URL: Bug Tracker, https://github.com/pypa/privacera_shield_common/issues
 Author-email: PAIG Shield <paig@privacera.com>
 License-File: LICENSE
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8.1
 Requires-Dist: cryptography>=41.0.4
+Requires-Dist: jproperties>=2.1.1
 Requires-Dist: urllib3>=2.0.6
 Description-Content-Type: text/markdown
 
 # Common library for Privacera AI Governance Applications
 
 The `privacera_shield_common` provides the common classes/functions used by the privacera AI governance applications.
```

## Comparing `privacera_shield_common-1.0.0.dist-info/RECORD` & `privacera_shield_common-1.1.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 privacera_shield_common/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 privacera_shield_common/audit_spooler.py,sha256=rtdoaVoGnnDziB8Myz_wHrYSQyUGyiTpDBEdQSIbHwQ,9149
+privacera_shield_common/config_utils.py,sha256=Gmz6HeMFrJpR3_YWlPCbndSVhScIDt0m2BqAvL47MvI,2183
 privacera_shield_common/encryption.py,sha256=_mZ5K_fdGS15iv2THpANmFN1t9hjercnYfyJNd0SiEM,5931
 privacera_shield_common/file_utils.py,sha256=qNOmB3d4JI_NBuodtVes1OhEEjvifB9_FOrlLUiv2n4,2551
 privacera_shield_common/http_transport.py,sha256=Aagujmvj_HJ_dvX_gR90-HKavLnjzjnv4ZMag2KWwsU,2738
-privacera_shield_common-1.0.0.dist-info/METADATA,sha256=ShjZVHQpDsqNCo6LM_QayryWOQv2Q7S2JKiTtOwL0Pw,879
-privacera_shield_common-1.0.0.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
-privacera_shield_common-1.0.0.dist-info/licenses/LICENSE,sha256=3q3EMpPio3ubJdZkO1Ihvz_0MuRxedrvWPWKEZH6R8E,294
-privacera_shield_common-1.0.0.dist-info/RECORD,,
+privacera_shield_common/lru_cache.py,sha256=HuVQyw9Ile-KJcCdm70cyXvtyiwPOQsHg8TptNBB2-I,3763
+privacera_shield_common-1.1.0.dist-info/METADATA,sha256=PXT7YFUX2WfQ8mMULOX-tZYEkbFbVf2TsP9441bqIhg,913
+privacera_shield_common-1.1.0.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
+privacera_shield_common-1.1.0.dist-info/licenses/LICENSE,sha256=3q3EMpPio3ubJdZkO1Ihvz_0MuRxedrvWPWKEZH6R8E,294
+privacera_shield_common-1.1.0.dist-info/RECORD,,
```

