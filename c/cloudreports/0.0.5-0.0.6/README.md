# Comparing `tmp/cloudreports-0.0.5.tar.gz` & `tmp/cloudreports-0.0.6.tar.gz`

## Comparing `cloudreports-0.0.5.tar` & `cloudreports-0.0.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 cloudreports-0.0.5/.gitattributes
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudreports-0.0.5/src/cloudreports/__init__.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 cloudreports-0.0.5/src/cloudreports/client.py
--rw-r--r--   0        0        0    17194 2020-02-02 00:00:00.000000 cloudreports-0.0.5/src/cloudreports/database.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudreports-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 cloudreports-0.0.5/tests/test.py
--rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 cloudreports-0.0.5/.gitignore
--rw-r--r--   0        0        0    35802 2020-02-02 00:00:00.000000 cloudreports-0.0.5/LICENSE
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 cloudreports-0.0.5/README.md
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 cloudreports-0.0.5/pyproject.toml
--rw-r--r--   0        0        0    42904 2020-02-02 00:00:00.000000 cloudreports-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 cloudreports-0.0.6/.gitattributes
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudreports-0.0.6/src/cloudreports/__init__.py
+-rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 cloudreports-0.0.6/src/cloudreports/client.py
+-rw-r--r--   0        0        0    17194 2020-02-02 00:00:00.000000 cloudreports-0.0.6/src/cloudreports/database.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudreports-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 cloudreports-0.0.6/tests/test.py
+-rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 cloudreports-0.0.6/.gitignore
+-rw-r--r--   0        0        0    35802 2020-02-02 00:00:00.000000 cloudreports-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 cloudreports-0.0.6/README.md
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 cloudreports-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0    42904 2020-02-02 00:00:00.000000 cloudreports-0.0.6/PKG-INFO
```

### Comparing `cloudreports-0.0.5/src/cloudreports/client.py` & `cloudreports-0.0.6/src/cloudreports/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         headers = {
                 'Authorization': f'cr_api_token {self.cr_api_token}'
             }
         r = requests.get(f'{self.cr_api_url}/{self.cr_integration_id}', headers=headers)
         return json.loads(r.content)
 
 
-    def set_integration(self, load_date=None, load_rows=None, load_percent=None, tables_qty=None):
+    def set_integration(self, load_date=None, load_rows=None, load_percent=None, tables_qty=None, status=None, status_stop=None):
         """Set intrgration data to CloudReports platform"""
 
         if self.cr_api_url is None:
             return {'result': 'error', 'info': 'cr_api_url is None'}
         if self.cr_api_token is None:
             return {'result': 'error', 'info': 'cr_api_token is None'}
         if self.cr_integration_id is None:
@@ -73,15 +73,19 @@
         if load_date is not None and isinstance(load_date, datetime):
             data['load_date'] = str(load_date)
         if load_rows is not None and type(load_rows) is int:
             data['load_rows'] = load_rows
         if load_percent is not None and type(load_percent) is int:
             data['load_percent'] = load_percent 
         if tables_qty is not None and type(tables_qty) is int:
-            data['tables_qty'] = tables_qty      
+            data['tables_qty'] = tables_qty 
+        if status is not None and type(status) is int and status in [0,1]:
+            data['status'] = status
+        if status_stop is not None and type(status_stop) is int and status_stop in [0,1]:
+            data['status_stop'] = status_stop                 
 
         headers = {
                 'Authorization': f'cr_api_token {self.cr_api_token}'
             }
         r = requests.put(f'{self.cr_api_url}/{self.cr_integration_id}', headers=headers, 
             json=data)
         return r
```

### Comparing `cloudreports-0.0.5/src/cloudreports/database.py` & `cloudreports-0.0.6/src/cloudreports/database.py`

 * *Files identical despite different names*

### Comparing `cloudreports-0.0.5/tests/test.py` & `cloudreports-0.0.6/tests/test.py`

 * *Files identical despite different names*

### Comparing `cloudreports-0.0.5/.gitignore` & `cloudreports-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `cloudreports-0.0.5/LICENSE` & `cloudreports-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudreports-0.0.5/README.md` & `cloudreports-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `cloudreports-0.0.5/pyproject.toml` & `cloudreports-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cloudreports"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="BR Systems", email="help@cloudreports.ru" },
 ]
 description = "Official Library Cloudreports.ru"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `cloudreports-0.0.5/PKG-INFO` & `cloudreports-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cloudreports
-Version: 0.0.5
+Version: 0.0.6
 Summary: Official Library Cloudreports.ru
 Project-URL: Homepage, https://github.com/brmoscow/cloudreports-python
 Project-URL: Bug Tracker, https://github.com/brmoscow/cloudreports-python/issues
 Author-email: BR Systems <help@cloudreports.ru>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

