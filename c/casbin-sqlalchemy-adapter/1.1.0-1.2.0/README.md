# Comparing `tmp/casbin_sqlalchemy_adapter-1.1.0.tar.gz` & `tmp/casbin_sqlalchemy_adapter-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casbin_sqlalchemy_adapter-1.1.0.tar", last modified: Thu Mar 28 17:31:36 2024, max compression
+gzip compressed data, was "casbin_sqlalchemy_adapter-1.2.0.tar", last modified: Thu May 30 02:25:12 2024, max compression
```

## Comparing `casbin_sqlalchemy_adapter-1.1.0.tar` & `casbin_sqlalchemy_adapter-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:31:36.218620 casbin_sqlalchemy_adapter-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-28 17:31:05.000000 casbin_sqlalchemy_adapter-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-03-28 17:31:36.218620 casbin_sqlalchemy_adapter-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-03-28 17:31:05.000000 casbin_sqlalchemy_adapter-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:31:36.218620 casbin_sqlalchemy_adapter-1.1.0/casbin_sqlalchemy_adapter/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-28 17:31:05.000000 casbin_sqlalchemy_adapter-1.1.0/casbin_sqlalchemy_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-03-28 17:31:05.000000 casbin_sqlalchemy_adapter-1.1.0/casbin_sqlalchemy_adapter/adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:31:36.218620 casbin_sqlalchemy_adapter-1.1.0/casbin_sqlalchemy_adapter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-03-28 17:31:36.000000 casbin_sqlalchemy_adapter-1.1.0/casbin_sqlalchemy_adapter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-03-28 17:31:36.000000 casbin_sqlalchemy_adapter-1.1.0/casbin_sqlalchemy_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 17:31:36.000000 casbin_sqlalchemy_adapter-1.1.0/casbin_sqlalchemy_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-28 17:31:36.000000 casbin_sqlalchemy_adapter-1.1.0/casbin_sqlalchemy_adapter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-28 17:31:36.000000 casbin_sqlalchemy_adapter-1.1.0/casbin_sqlalchemy_adapter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-28 17:31:36.222620 casbin_sqlalchemy_adapter-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-03-28 17:31:05.000000 casbin_sqlalchemy_adapter-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:31:36.218620 casbin_sqlalchemy_adapter-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    16896 2024-03-28 17:31:05.000000 casbin_sqlalchemy_adapter-1.1.0/tests/test_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:25:12.490954 casbin_sqlalchemy_adapter-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-30 02:24:37.000000 casbin_sqlalchemy_adapter-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-30 02:25:12.490954 casbin_sqlalchemy_adapter-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-30 02:24:37.000000 casbin_sqlalchemy_adapter-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:25:12.486955 casbin_sqlalchemy_adapter-1.2.0/casbin_sqlalchemy_adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-30 02:24:37.000000 casbin_sqlalchemy_adapter-1.2.0/casbin_sqlalchemy_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9917 2024-05-30 02:24:37.000000 casbin_sqlalchemy_adapter-1.2.0/casbin_sqlalchemy_adapter/adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:25:12.490954 casbin_sqlalchemy_adapter-1.2.0/casbin_sqlalchemy_adapter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-30 02:25:12.000000 casbin_sqlalchemy_adapter-1.2.0/casbin_sqlalchemy_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-30 02:25:12.000000 casbin_sqlalchemy_adapter-1.2.0/casbin_sqlalchemy_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 02:25:12.000000 casbin_sqlalchemy_adapter-1.2.0/casbin_sqlalchemy_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-30 02:25:12.000000 casbin_sqlalchemy_adapter-1.2.0/casbin_sqlalchemy_adapter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-30 02:25:12.000000 casbin_sqlalchemy_adapter-1.2.0/casbin_sqlalchemy_adapter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-30 02:25:12.490954 casbin_sqlalchemy_adapter-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-30 02:24:37.000000 casbin_sqlalchemy_adapter-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:25:12.490954 casbin_sqlalchemy_adapter-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    16896 2024-05-30 02:24:37.000000 casbin_sqlalchemy_adapter-1.2.0/tests/test_adapter.py
```

### Comparing `casbin_sqlalchemy_adapter-1.1.0/LICENSE` & `casbin_sqlalchemy_adapter-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `casbin_sqlalchemy_adapter-1.1.0/PKG-INFO` & `casbin_sqlalchemy_adapter-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casbin_sqlalchemy_adapter
-Version: 1.1.0
+Version: 1.2.0
 Summary: SQLAlchemy Adapter for PyCasbin
 Home-page: https://github.com/pycasbin/sqlalchemy-adapter
 Author: TechLee
 Author-email: techlee@qq.com
 License: Apache 2.0
 Keywords: casbin,SQLAlchemy,casbin-adapter,rbac,access control,abac,acl,permission
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `casbin_sqlalchemy_adapter-1.1.0/README.md` & `casbin_sqlalchemy_adapter-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `casbin_sqlalchemy_adapter-1.1.0/casbin_sqlalchemy_adapter/adapter.py` & `casbin_sqlalchemy_adapter-1.2.0/casbin_sqlalchemy_adapter/adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,32 +123,35 @@
         for attr in ("ptype", "v0", "v1", "v2", "v3", "v4", "v5"):
             if len(getattr(filter, attr)) > 0:
                 querydb = querydb.filter(
                     getattr(self._db_class, attr).in_(getattr(filter, attr))
                 )
         return querydb.order_by(self._db_class.id)
 
-    def _save_policy_line(self, ptype, rule):
-        with self._session_scope() as session:
-            line = self._db_class(ptype=ptype)
-            for i, v in enumerate(rule):
-                setattr(line, "v{}".format(i), v)
+    def _save_policy_line(self, ptype, rule, session=None):
+        line = self._db_class(ptype=ptype)
+        for i, v in enumerate(rule):
+            setattr(line, "v{}".format(i), v)
+        if session:
             session.add(line)
+        else:
+            with self._session_scope() as session:
+                session.add(line)
 
     def save_policy(self, model):
         """saves all policy rules to the storage."""
         with self._session_scope() as session:
             query = session.query(self._db_class)
             query.delete()
             for sec in ["p", "g"]:
                 if sec not in model.model.keys():
                     continue
                 for ptype, ast in model.model[sec].items():
                     for rule in ast.policy:
-                        self._save_policy_line(ptype, rule)
+                        self._save_policy_line(ptype, rule, session=session)
         return True
 
     def add_policy(self, sec, ptype, rule):
         """adds a policy rule to the storage."""
         self._save_policy_line(ptype, rule)
 
     def add_policies(self, sec, ptype, rules):
```

### Comparing `casbin_sqlalchemy_adapter-1.1.0/casbin_sqlalchemy_adapter.egg-info/PKG-INFO` & `casbin_sqlalchemy_adapter-1.2.0/casbin_sqlalchemy_adapter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casbin_sqlalchemy_adapter
-Version: 1.1.0
+Version: 1.2.0
 Summary: SQLAlchemy Adapter for PyCasbin
 Home-page: https://github.com/pycasbin/sqlalchemy-adapter
 Author: TechLee
 Author-email: techlee@qq.com
 License: Apache 2.0
 Keywords: casbin,SQLAlchemy,casbin-adapter,rbac,access control,abac,acl,permission
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `casbin_sqlalchemy_adapter-1.1.0/setup.py` & `casbin_sqlalchemy_adapter-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `casbin_sqlalchemy_adapter-1.1.0/tests/test_adapter.py` & `casbin_sqlalchemy_adapter-1.2.0/tests/test_adapter.py`

 * *Files identical despite different names*

