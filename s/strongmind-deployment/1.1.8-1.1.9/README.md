# Comparing `tmp/strongmind_deployment-1.1.8-py3-none-any.whl.zip` & `tmp/strongmind_deployment-1.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 14087 bytes, number of entries: 12
+Zip file size: 14086 bytes, number of entries: 12
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 strongmind_deployment/__init__.py
 -rw-r--r--  2.0 unx    13147 b- defN 20-Feb-02 00:00 strongmind_deployment/container.py
 -rw-r--r--  2.0 unx     4757 b- defN 20-Feb-02 00:00 strongmind_deployment/dynamo.py
 -rw-r--r--  2.0 unx     3232 b- defN 20-Feb-02 00:00 strongmind_deployment/execution.py
--rw-r--r--  2.0 unx    13957 b- defN 20-Feb-02 00:00 strongmind_deployment/rails.py
+-rw-r--r--  2.0 unx    14036 b- defN 20-Feb-02 00:00 strongmind_deployment/rails.py
 -rw-r--r--  2.0 unx     2918 b- defN 20-Feb-02 00:00 strongmind_deployment/redis.py
 -rw-r--r--  2.0 unx     2097 b- defN 20-Feb-02 00:00 strongmind_deployment/secrets.py
 -rw-r--r--  2.0 unx     2093 b- defN 20-Feb-02 00:00 strongmind_deployment/storage.py
-?rw-r--r--  2.0 unx      696 b- defN 20-Feb-02 00:00 strongmind_deployment-1.1.8.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 strongmind_deployment-1.1.8.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1053 b- defN 20-Feb-02 00:00 strongmind_deployment-1.1.8.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     1069 b- defN 20-Feb-02 00:00 strongmind_deployment-1.1.8.dist-info/RECORD
-12 files, 45106 bytes uncompressed, 12267 bytes compressed:  72.8%
+?rw-r--r--  2.0 unx      696 b- defN 20-Feb-02 00:00 strongmind_deployment-1.1.9.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 strongmind_deployment-1.1.9.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1053 b- defN 20-Feb-02 00:00 strongmind_deployment-1.1.9.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     1069 b- defN 20-Feb-02 00:00 strongmind_deployment-1.1.9.dist-info/RECORD
+12 files, 45185 bytes uncompressed, 12266 bytes compressed:  72.9%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: strongmind_deployment/secrets.py
 Comment: 
 
 Filename: strongmind_deployment/storage.py
 Comment: 
 
-Filename: strongmind_deployment-1.1.8.dist-info/METADATA
+Filename: strongmind_deployment-1.1.9.dist-info/METADATA
 Comment: 
 
-Filename: strongmind_deployment-1.1.8.dist-info/WHEEL
+Filename: strongmind_deployment-1.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: strongmind_deployment-1.1.8.dist-info/licenses/LICENSE
+Filename: strongmind_deployment-1.1.9.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: strongmind_deployment-1.1.8.dist-info/RECORD
+Filename: strongmind_deployment-1.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## strongmind_deployment/rails.py

```diff
@@ -147,14 +147,15 @@
             'DB_PASSWORD': self.db_password.result,
             'DATABASE_URL': self.get_database_url(),
             'RAILS_ENV': 'production'
         }
 
         self.env_vars.update(additional_env_vars)
         self.kwargs['env_vars'] = self.env_vars
+        self.kwargs['secrets'] = self.secret.get_secrets()  # pragma: no cover
         self.kwargs['container_image'] = container_image
 
         self.kwargs['entry_point'] = ["sh", "-c",
                                       "bundle exec rails db:migrate && echo 'Migrations complete'"]
         self.migration_container = ContainerComponent("migration",
                                                       need_load_balancer=False,
                                                       desired_count=0,
```

## Comparing `strongmind_deployment-1.1.8.dist-info/METADATA` & `strongmind_deployment-1.1.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strongmind_deployment
-Version: 1.1.8
+Version: 1.1.9
 Summary: Deployment tools for Strongmind
 Project-URL: Homepage, https://github.com/strongmind/public-reusable-workflows/tree/main/deployment
 Author-email: Belding <teambelding@strongmind.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

## Comparing `strongmind_deployment-1.1.8.dist-info/licenses/LICENSE` & `strongmind_deployment-1.1.9.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `strongmind_deployment-1.1.8.dist-info/RECORD` & `strongmind_deployment-1.1.9.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 strongmind_deployment/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 strongmind_deployment/container.py,sha256=OG8IvFeO0Z4Xaa0NzsVjWzgST8zTnXbiXyQxyZ6t710,13147
 strongmind_deployment/dynamo.py,sha256=ppTNvIMdj9tr85thLlciCoszdZAa6ehgeIIm9pwu1Es,4757
 strongmind_deployment/execution.py,sha256=dA9QLcI38KgOXjhf3Hsek-7vvPkklFWPILqjybcumPw,3232
-strongmind_deployment/rails.py,sha256=_3Neljp-vbkra5zolRLo8qM6HvDbt-D4GWcai3P1fFg,13957
+strongmind_deployment/rails.py,sha256=hb_PfxjGZBmkk6V7NpcxG7QO4DvUCc14SBH3ROfc0NI,14036
 strongmind_deployment/redis.py,sha256=Cl7avjc0PNiqJ3E4IgG9_2js8tcG3FeSNpGbpGmCAeE,2918
 strongmind_deployment/secrets.py,sha256=YbsgCd1Uz94ZAu9VrtNjc0f5nc1xNEHEdhb150mOnzU,2097
 strongmind_deployment/storage.py,sha256=-C09-MBKoHyCb9n6lvyETa14ZuFz030HNpai-4zFpC4,2093
-strongmind_deployment-1.1.8.dist-info/METADATA,sha256=5wURLwbCcOjBm51s1hNOBsVAdN3TlGLaeR_NbXSMsSU,696
-strongmind_deployment-1.1.8.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
-strongmind_deployment-1.1.8.dist-info/licenses/LICENSE,sha256=2zBZXFllrbHYl8Zg63B1X0QWHK1ed93SzZQVh9gd77c,1053
-strongmind_deployment-1.1.8.dist-info/RECORD,,
+strongmind_deployment-1.1.9.dist-info/METADATA,sha256=DSFQIp74jv5TTW0p4I1L3XOP9t8cEfe_DIZFWXeq4mY,696
+strongmind_deployment-1.1.9.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
+strongmind_deployment-1.1.9.dist-info/licenses/LICENSE,sha256=2zBZXFllrbHYl8Zg63B1X0QWHK1ed93SzZQVh9gd77c,1053
+strongmind_deployment-1.1.9.dist-info/RECORD,,
```

