# Comparing `tmp/virtool_core-8.0.2.tar.gz` & `tmp/virtool_core-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virtool_core-8.0.2.tar", max compression
+gzip compressed data, was "virtool_core-9.0.0.tar", max compression
```

## Comparing `virtool_core-8.0.2.tar` & `virtool_core-9.0.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1077 2023-11-23 17:24:28.428120 virtool_core-8.0.2/LICENSE
--rw-r--r--   0        0        0     2087 2023-11-23 17:24:28.432121 virtool_core-8.0.2/README.md
--rw-r--r--   0        0        0     1092 2023-11-23 17:24:37.252110 virtool_core-8.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-11-23 17:24:28.620120 virtool_core-8.0.2/virtool_core/__init__.py
--rw-r--r--   0        0        0     7038 2023-11-23 17:24:28.620120 virtool_core-8.0.2/virtool_core/bio.py
--rw-r--r--   0        0        0       79 2023-11-23 17:24:28.620120 virtool_core-8.0.2/virtool_core/errors.py
--rw-r--r--   0        0        0      940 2023-11-23 17:24:28.620120 virtool_core-8.0.2/virtool_core/logging.py
--rw-r--r--   0        0        0      384 2023-11-23 17:24:28.620120 virtool_core-8.0.2/virtool_core/models/__init__.py
--rw-r--r--   0        0        0     1216 2023-11-23 17:24:28.620120 virtool_core-8.0.2/virtool_core/models/account.py
--rw-r--r--   0        0        0      438 2023-11-23 17:24:28.620120 virtool_core-8.0.2/virtool_core/models/administrator.py
--rw-r--r--   0        0        0     1474 2023-11-23 17:24:28.620120 virtool_core-8.0.2/virtool_core/models/analysis.py
--rw-r--r--   0        0        0      176 2023-11-23 17:24:28.620120 virtool_core-8.0.2/virtool_core/models/auth.py
--rw-r--r--   0        0        0      264 2023-11-23 17:24:28.620120 virtool_core-8.0.2/virtool_core/models/basemodel.py
--rw-r--r--   0        0        0      371 2023-11-23 17:24:28.620120 virtool_core-8.0.2/virtool_core/models/blast.py
--rw-r--r--   0        0        0     1452 2023-11-23 17:24:28.620120 virtool_core-8.0.2/virtool_core/models/enums.py
--rw-r--r--   0        0        0      593 2023-11-23 17:24:28.620120 virtool_core-8.0.2/virtool_core/models/genbank.py
--rw-r--r--   0        0        0      715 2023-11-23 17:24:28.620120 virtool_core-8.0.2/virtool_core/models/group.py
--rw-r--r--   0        0        0     1607 2023-11-23 17:24:28.620120 virtool_core-8.0.2/virtool_core/models/history.py
--rw-r--r--   0        0        0     1613 2023-11-23 17:24:28.620120 virtool_core-8.0.2/virtool_core/models/hmm.py
--rw-r--r--   0        0        0     1163 2023-11-23 17:24:28.620120 virtool_core-8.0.2/virtool_core/models/index.py
--rw-r--r--   0        0        0      359 2023-11-23 17:24:28.620120 virtool_core-8.0.2/virtool_core/models/instancemessage.py
--rw-r--r--   0        0        0     1329 2023-11-23 17:24:28.620120 virtool_core-8.0.2/virtool_core/models/job.py
--rw-r--r--   0        0        0      389 2023-11-23 17:24:28.620120 virtool_core-8.0.2/virtool_core/models/label.py
--rw-r--r--   0        0        0     1810 2023-11-23 17:24:28.620120 virtool_core-8.0.2/virtool_core/models/ml.py
--rw-r--r--   0        0        0     1909 2023-11-23 17:24:28.620120 virtool_core-8.0.2/virtool_core/models/otu.py
--rw-r--r--   0        0        0     1105 2023-11-23 17:24:28.620120 virtool_core-8.0.2/virtool_core/models/project.py
--rw-r--r--   0        0        0     2566 2023-11-23 17:24:28.620120 virtool_core-8.0.2/virtool_core/models/reference.py
--rw-r--r--   0        0        0     4304 2023-11-23 17:24:28.620120 virtool_core-8.0.2/virtool_core/models/roles.py
--rw-r--r--   0        0        0     2109 2023-11-23 17:24:28.620120 virtool_core-8.0.2/virtool_core/models/samples.py
--rw-r--r--   0        0        0      179 2023-11-23 17:24:28.620120 virtool_core-8.0.2/virtool_core/models/searchresult.py
--rw-r--r--   0        0        0      418 2023-11-23 17:24:28.620120 virtool_core-8.0.2/virtool_core/models/session.py
--rw-r--r--   0        0        0      494 2023-11-23 17:24:28.620120 virtool_core-8.0.2/virtool_core/models/settings.py
--rw-r--r--   0        0        0     1007 2023-11-23 17:24:28.620120 virtool_core-8.0.2/virtool_core/models/spaces.py
--rw-r--r--   0        0        0     1412 2023-11-23 17:24:28.620120 virtool_core-8.0.2/virtool_core/models/subtraction.py
--rw-r--r--   0        0        0      446 2023-11-23 17:24:28.620120 virtool_core-8.0.2/virtool_core/models/task.py
--rw-r--r--   0        0        0      656 2023-11-23 17:24:28.620120 virtool_core-8.0.2/virtool_core/models/upload.py
--rw-r--r--   0        0        0      957 2023-11-23 17:24:28.620120 virtool_core-8.0.2/virtool_core/models/user.py
--rw-r--r--   0        0        0      881 2023-11-23 17:24:28.620120 virtool_core-8.0.2/virtool_core/models/validators.py
--rw-r--r--   0        0        0     1901 2023-11-23 17:24:28.620120 virtool_core-8.0.2/virtool_core/mongo.py
--rw-r--r--   0        0        0     3296 2023-11-23 17:24:28.620120 virtool_core-8.0.2/virtool_core/redis.py
--rw-r--r--   0        0        0    10517 2023-11-23 17:24:28.620120 virtool_core-8.0.2/virtool_core/utils.py
--rw-r--r--   0        0        0     3311 1970-01-01 00:00:00.000000 virtool_core-8.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-12-27 23:13:53.055313 virtool_core-9.0.0/LICENSE
+-rw-r--r--   0        0        0     2087 2023-12-27 23:13:53.055313 virtool_core-9.0.0/README.md
+-rw-r--r--   0        0        0     1092 2023-12-27 23:14:02.239380 virtool_core-9.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-27 23:13:53.247315 virtool_core-9.0.0/virtool_core/__init__.py
+-rw-r--r--   0        0        0     7038 2023-12-27 23:13:53.247315 virtool_core-9.0.0/virtool_core/bio.py
+-rw-r--r--   0        0        0       79 2023-12-27 23:13:53.247315 virtool_core-9.0.0/virtool_core/errors.py
+-rw-r--r--   0        0        0      940 2023-12-27 23:13:53.247315 virtool_core-9.0.0/virtool_core/logging.py
+-rw-r--r--   0        0        0      384 2023-12-27 23:13:53.247315 virtool_core-9.0.0/virtool_core/models/__init__.py
+-rw-r--r--   0        0        0     1216 2023-12-27 23:13:53.247315 virtool_core-9.0.0/virtool_core/models/account.py
+-rw-r--r--   0        0        0      438 2023-12-27 23:13:53.251315 virtool_core-9.0.0/virtool_core/models/administrator.py
+-rw-r--r--   0        0        0     1474 2023-12-27 23:13:53.251315 virtool_core-9.0.0/virtool_core/models/analysis.py
+-rw-r--r--   0        0        0      176 2023-12-27 23:13:53.251315 virtool_core-9.0.0/virtool_core/models/auth.py
+-rw-r--r--   0        0        0      264 2023-12-27 23:13:53.251315 virtool_core-9.0.0/virtool_core/models/basemodel.py
+-rw-r--r--   0        0        0      371 2023-12-27 23:13:53.251315 virtool_core-9.0.0/virtool_core/models/blast.py
+-rw-r--r--   0        0        0     1452 2023-12-27 23:13:53.251315 virtool_core-9.0.0/virtool_core/models/enums.py
+-rw-r--r--   0        0        0      593 2023-12-27 23:13:53.251315 virtool_core-9.0.0/virtool_core/models/genbank.py
+-rw-r--r--   0        0        0      715 2023-12-27 23:13:53.251315 virtool_core-9.0.0/virtool_core/models/group.py
+-rw-r--r--   0        0        0     1607 2023-12-27 23:13:53.251315 virtool_core-9.0.0/virtool_core/models/history.py
+-rw-r--r--   0        0        0     1613 2023-12-27 23:13:53.251315 virtool_core-9.0.0/virtool_core/models/hmm.py
+-rw-r--r--   0        0        0     1163 2023-12-27 23:13:53.251315 virtool_core-9.0.0/virtool_core/models/index.py
+-rw-r--r--   0        0        0      359 2023-12-27 23:13:53.251315 virtool_core-9.0.0/virtool_core/models/instancemessage.py
+-rw-r--r--   0        0        0     1329 2023-12-27 23:13:53.251315 virtool_core-9.0.0/virtool_core/models/job.py
+-rw-r--r--   0        0        0      389 2023-12-27 23:13:53.251315 virtool_core-9.0.0/virtool_core/models/label.py
+-rw-r--r--   0        0        0     1810 2023-12-27 23:13:53.251315 virtool_core-9.0.0/virtool_core/models/ml.py
+-rw-r--r--   0        0        0     1909 2023-12-27 23:13:53.251315 virtool_core-9.0.0/virtool_core/models/otu.py
+-rw-r--r--   0        0        0     1105 2023-12-27 23:13:53.251315 virtool_core-9.0.0/virtool_core/models/project.py
+-rw-r--r--   0        0        0     2566 2023-12-27 23:13:53.251315 virtool_core-9.0.0/virtool_core/models/reference.py
+-rw-r--r--   0        0        0     4304 2023-12-27 23:13:53.251315 virtool_core-9.0.0/virtool_core/models/roles.py
+-rw-r--r--   0        0        0     2109 2023-12-27 23:13:53.251315 virtool_core-9.0.0/virtool_core/models/samples.py
+-rw-r--r--   0        0        0      179 2023-12-27 23:13:53.251315 virtool_core-9.0.0/virtool_core/models/searchresult.py
+-rw-r--r--   0        0        0      418 2023-12-27 23:13:53.251315 virtool_core-9.0.0/virtool_core/models/session.py
+-rw-r--r--   0        0        0      494 2023-12-27 23:13:53.251315 virtool_core-9.0.0/virtool_core/models/settings.py
+-rw-r--r--   0        0        0     1007 2023-12-27 23:13:53.251315 virtool_core-9.0.0/virtool_core/models/spaces.py
+-rw-r--r--   0        0        0     1412 2023-12-27 23:13:53.251315 virtool_core-9.0.0/virtool_core/models/subtraction.py
+-rw-r--r--   0        0        0      446 2023-12-27 23:13:53.251315 virtool_core-9.0.0/virtool_core/models/task.py
+-rw-r--r--   0        0        0      656 2023-12-27 23:13:53.251315 virtool_core-9.0.0/virtool_core/models/upload.py
+-rw-r--r--   0        0        0      933 2023-12-27 23:13:53.251315 virtool_core-9.0.0/virtool_core/models/user.py
+-rw-r--r--   0        0        0      881 2023-12-27 23:13:53.251315 virtool_core-9.0.0/virtool_core/models/validators.py
+-rw-r--r--   0        0        0     1901 2023-12-27 23:13:53.251315 virtool_core-9.0.0/virtool_core/mongo.py
+-rw-r--r--   0        0        0     3296 2023-12-27 23:13:53.251315 virtool_core-9.0.0/virtool_core/redis.py
+-rw-r--r--   0        0        0    10517 2023-12-27 23:13:53.251315 virtool_core-9.0.0/virtool_core/utils.py
+-rw-r--r--   0        0        0     3311 1970-01-01 00:00:00.000000 virtool_core-9.0.0/PKG-INFO
```

### Comparing `virtool_core-8.0.2/LICENSE` & `virtool_core-9.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `virtool_core-8.0.2/README.md` & `virtool_core-9.0.0/README.md`

 * *Files identical despite different names*

### Comparing `virtool_core-8.0.2/pyproject.toml` & `virtool_core-9.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "virtool-core"
-version = "8.0.2"
+version = "9.0.0"
 description = "Core utilities for Virtool."
 authors = ["Ian Boyes", "Blake Smith"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/virtool/virtool-core"
 classifiers = [
     "Topic :: Software Development :: Libraries",
```

### Comparing `virtool_core-8.0.2/virtool_core/bio.py` & `virtool_core-9.0.0/virtool_core/bio.py`

 * *Files identical despite different names*

### Comparing `virtool_core-8.0.2/virtool_core/logging.py` & `virtool_core-9.0.0/virtool_core/logging.py`

 * *Files identical despite different names*

### Comparing `virtool_core-8.0.2/virtool_core/models/account.py` & `virtool_core-9.0.0/virtool_core/models/account.py`

 * *Files identical despite different names*

### Comparing `virtool_core-8.0.2/virtool_core/models/analysis.py` & `virtool_core-9.0.0/virtool_core/models/analysis.py`

 * *Files identical despite different names*

### Comparing `virtool_core-8.0.2/virtool_core/models/enums.py` & `virtool_core-9.0.0/virtool_core/models/enums.py`

 * *Files identical despite different names*

### Comparing `virtool_core-8.0.2/virtool_core/models/genbank.py` & `virtool_core-9.0.0/virtool_core/models/genbank.py`

 * *Files identical despite different names*

### Comparing `virtool_core-8.0.2/virtool_core/models/group.py` & `virtool_core-9.0.0/virtool_core/models/group.py`

 * *Files identical despite different names*

### Comparing `virtool_core-8.0.2/virtool_core/models/history.py` & `virtool_core-9.0.0/virtool_core/models/history.py`

 * *Files identical despite different names*

### Comparing `virtool_core-8.0.2/virtool_core/models/hmm.py` & `virtool_core-9.0.0/virtool_core/models/hmm.py`

 * *Files identical despite different names*

### Comparing `virtool_core-8.0.2/virtool_core/models/index.py` & `virtool_core-9.0.0/virtool_core/models/index.py`

 * *Files identical despite different names*

### Comparing `virtool_core-8.0.2/virtool_core/models/job.py` & `virtool_core-9.0.0/virtool_core/models/job.py`

 * *Files identical despite different names*

### Comparing `virtool_core-8.0.2/virtool_core/models/ml.py` & `virtool_core-9.0.0/virtool_core/models/ml.py`

 * *Files identical despite different names*

### Comparing `virtool_core-8.0.2/virtool_core/models/otu.py` & `virtool_core-9.0.0/virtool_core/models/otu.py`

 * *Files identical despite different names*

### Comparing `virtool_core-8.0.2/virtool_core/models/project.py` & `virtool_core-9.0.0/virtool_core/models/project.py`

 * *Files identical despite different names*

### Comparing `virtool_core-8.0.2/virtool_core/models/reference.py` & `virtool_core-9.0.0/virtool_core/models/reference.py`

 * *Files identical despite different names*

### Comparing `virtool_core-8.0.2/virtool_core/models/roles.py` & `virtool_core-9.0.0/virtool_core/models/roles.py`

 * *Files identical despite different names*

### Comparing `virtool_core-8.0.2/virtool_core/models/samples.py` & `virtool_core-9.0.0/virtool_core/models/samples.py`

 * *Files identical despite different names*

### Comparing `virtool_core-8.0.2/virtool_core/models/spaces.py` & `virtool_core-9.0.0/virtool_core/models/spaces.py`

 * *Files identical despite different names*

### Comparing `virtool_core-8.0.2/virtool_core/models/subtraction.py` & `virtool_core-9.0.0/virtool_core/models/subtraction.py`

 * *Files identical despite different names*

### Comparing `virtool_core-8.0.2/virtool_core/models/upload.py` & `virtool_core-9.0.0/virtool_core/models/upload.py`

 * *Files identical despite different names*

### Comparing `virtool_core-8.0.2/virtool_core/models/user.py` & `virtool_core-9.0.0/virtool_core/models/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,31 +11,30 @@
     family_name: str | None
     given_name: str | None
     oid: str
 
 
 class UserNested(BaseModel):
     id: str
-    administrator: bool
     handle: str
 
 
 class UserMinimal(UserNested):
     active: bool
     b2c: UserB2C | None
     b2c_display_name: str | None
     b2c_family_name: str | None
     b2c_given_name: str | None
     b2c_oid: str | None
 
 
 class User(UserMinimal):
+    administrator_role: AdministratorRole | None
     force_reset: bool
     groups: list[GroupMinimal]
     last_password_change: datetime
     permissions: Permissions
     primary_group: GroupMinimal | None
-    administrator_role: AdministratorRole | None
 
 
 class UserSearchResult(SearchResult):
     items: list[User]
```

### Comparing `virtool_core-8.0.2/virtool_core/models/validators.py` & `virtool_core-9.0.0/virtool_core/models/validators.py`

 * *Files identical despite different names*

### Comparing `virtool_core-8.0.2/virtool_core/mongo.py` & `virtool_core-9.0.0/virtool_core/mongo.py`

 * *Files identical despite different names*

### Comparing `virtool_core-8.0.2/virtool_core/redis.py` & `virtool_core-9.0.0/virtool_core/redis.py`

 * *Files identical despite different names*

### Comparing `virtool_core-8.0.2/virtool_core/utils.py` & `virtool_core-9.0.0/virtool_core/utils.py`

 * *Files identical despite different names*

### Comparing `virtool_core-8.0.2/PKG-INFO` & `virtool_core-9.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virtool-core
-Version: 8.0.2
+Version: 9.0.0
 Summary: Core utilities for Virtool.
 Home-page: https://github.com/virtool/virtool-core
 License: MIT
 Author: Ian Boyes
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

