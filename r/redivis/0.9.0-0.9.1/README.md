# Comparing `tmp/redivis-0.9.0.tar.gz` & `tmp/redivis-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redivis-0.9.0.tar", last modified: Thu Dec  1 01:11:05 2022, max compression
+gzip compressed data, was "redivis-0.9.1.tar", last modified: Thu Dec  8 01:45:11 2022, max compression
```

## Comparing `redivis-0.9.0.tar` & `redivis-0.9.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2022-12-01 01:11:05.349605 redivis-0.9.0/
--rw-r--r--   0 ian        (501) staff       (20)     1069 2022-01-20 02:39:33.000000 redivis-0.9.0/LICENSE
--rw-r--r--   0 ian        (501) staff       (20)     1661 2022-12-01 01:11:05.349355 redivis-0.9.0/PKG-INFO
--rw-r--r--   0 ian        (501) staff       (20)      875 2022-08-05 01:02:00.000000 redivis-0.9.0/README.md
--rw-r--r--   0 ian        (501) staff       (20)       38 2022-12-01 01:11:05.349706 redivis-0.9.0/setup.cfg
--rw-r--r--   0 ian        (501) staff       (20)     4017 2022-08-23 01:00:31.000000 redivis-0.9.0/setup.py
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2022-12-01 01:11:05.344090 redivis-0.9.0/src/
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2022-12-01 01:11:05.345011 redivis-0.9.0/src/redivis/
--rw-r--r--   0 ian        (501) staff       (20)      303 2022-06-27 23:31:23.000000 redivis-0.9.0/src/redivis/__init__.py
--rw-r--r--   0 ian        (501) staff       (20)       22 2022-12-01 01:10:14.000000 redivis-0.9.0/src/redivis/_version.py
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2022-12-01 01:11:05.348363 redivis-0.9.0/src/redivis/classes/
--rw-r--r--   0 ian        (501) staff       (20)      629 2022-08-04 23:01:50.000000 redivis-0.9.0/src/redivis/classes/Base.py
--rw-r--r--   0 ian        (501) staff       (20)     4365 2022-08-04 22:49:27.000000 redivis-0.9.0/src/redivis/classes/Dataset.py
--rw-r--r--   0 ian        (501) staff       (20)     2860 2022-08-23 02:57:07.000000 redivis-0.9.0/src/redivis/classes/File.py
--rw-r--r--   0 ian        (501) staff       (20)      855 2022-08-04 22:52:36.000000 redivis-0.9.0/src/redivis/classes/Organization.py
--rw-r--r--   0 ian        (501) staff       (20)     1186 2022-08-04 22:52:36.000000 redivis-0.9.0/src/redivis/classes/Project.py
--rw-r--r--   0 ian        (501) staff       (20)     3353 2022-08-23 02:51:26.000000 redivis-0.9.0/src/redivis/classes/Query.py
--rw-r--r--   0 ian        (501) staff       (20)     3613 2022-12-01 01:07:41.000000 redivis-0.9.0/src/redivis/classes/Row.py
--rw-r--r--   0 ian        (501) staff       (20)    10778 2022-11-14 03:02:27.000000 redivis-0.9.0/src/redivis/classes/Table.py
--rw-r--r--   0 ian        (501) staff       (20)    12825 2022-11-28 20:03:46.000000 redivis-0.9.0/src/redivis/classes/Upload.py
--rw-r--r--   0 ian        (501) staff       (20)      999 2022-08-04 22:52:36.000000 redivis-0.9.0/src/redivis/classes/User.py
--rw-r--r--   0 ian        (501) staff       (20)     1824 2022-11-13 21:16:52.000000 redivis-0.9.0/src/redivis/classes/Variable.py
--rw-r--r--   0 ian        (501) staff       (20)        0 2022-01-20 02:39:33.000000 redivis-0.9.0/src/redivis/classes/__init__.py
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2022-12-01 01:11:05.349031 redivis-0.9.0/src/redivis/common/
--rw-r--r--   0 ian        (501) staff       (20)        0 2022-07-13 03:05:08.000000 redivis-0.9.0/src/redivis/common/__init__.py
--rw-r--r--   0 ian        (501) staff       (20)     3019 2022-11-14 00:14:51.000000 redivis-0.9.0/src/redivis/common/api_request.py
--rw-r--r--   0 ian        (501) staff       (20)      236 2022-01-20 02:39:33.000000 redivis-0.9.0/src/redivis/common/auth.py
--rw-r--r--   0 ian        (501) staff       (20)     4651 2022-12-01 00:34:51.000000 redivis-0.9.0/src/redivis/common/list_rows.py
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2022-12-01 01:11:05.345531 redivis-0.9.0/src/redivis.egg-info/
--rw-r--r--   0 ian        (501) staff       (20)     1661 2022-12-01 01:11:05.000000 redivis-0.9.0/src/redivis.egg-info/PKG-INFO
--rw-r--r--   0 ian        (501) staff       (20)      733 2022-12-01 01:11:05.000000 redivis-0.9.0/src/redivis.egg-info/SOURCES.txt
--rw-r--r--   0 ian        (501) staff       (20)        1 2022-12-01 01:11:05.000000 redivis-0.9.0/src/redivis.egg-info/dependency_links.txt
--rw-r--r--   0 ian        (501) staff       (20)       76 2022-12-01 01:11:05.000000 redivis-0.9.0/src/redivis.egg-info/requires.txt
--rw-r--r--   0 ian        (501) staff       (20)        8 2022-12-01 01:11:05.000000 redivis-0.9.0/src/redivis.egg-info/top_level.txt
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2022-12-08 01:45:11.580193 redivis-0.9.1/
+-rw-r--r--   0 ian        (501) staff       (20)     1069 2022-01-20 02:39:33.000000 redivis-0.9.1/LICENSE
+-rw-r--r--   0 ian        (501) staff       (20)     1661 2022-12-08 01:45:11.580037 redivis-0.9.1/PKG-INFO
+-rw-r--r--   0 ian        (501) staff       (20)      875 2022-08-05 01:02:00.000000 redivis-0.9.1/README.md
+-rw-r--r--   0 ian        (501) staff       (20)       38 2022-12-08 01:45:11.580238 redivis-0.9.1/setup.cfg
+-rw-r--r--   0 ian        (501) staff       (20)     4017 2022-08-23 01:00:31.000000 redivis-0.9.1/setup.py
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2022-12-08 01:45:11.573523 redivis-0.9.1/src/
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2022-12-08 01:45:11.574679 redivis-0.9.1/src/redivis/
+-rw-r--r--   0 ian        (501) staff       (20)      303 2022-06-27 23:31:23.000000 redivis-0.9.1/src/redivis/__init__.py
+-rw-r--r--   0 ian        (501) staff       (20)       22 2022-12-08 01:22:32.000000 redivis-0.9.1/src/redivis/_version.py
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2022-12-08 01:45:11.578948 redivis-0.9.1/src/redivis/classes/
+-rw-r--r--   0 ian        (501) staff       (20)      629 2022-08-04 23:01:50.000000 redivis-0.9.1/src/redivis/classes/Base.py
+-rw-r--r--   0 ian        (501) staff       (20)     4596 2022-12-08 01:15:26.000000 redivis-0.9.1/src/redivis/classes/Dataset.py
+-rw-r--r--   0 ian        (501) staff       (20)     2860 2022-08-23 02:57:07.000000 redivis-0.9.1/src/redivis/classes/File.py
+-rw-r--r--   0 ian        (501) staff       (20)      855 2022-08-04 22:52:36.000000 redivis-0.9.1/src/redivis/classes/Organization.py
+-rw-r--r--   0 ian        (501) staff       (20)     1186 2022-08-04 22:52:36.000000 redivis-0.9.1/src/redivis/classes/Project.py
+-rw-r--r--   0 ian        (501) staff       (20)     3353 2022-08-23 02:51:26.000000 redivis-0.9.1/src/redivis/classes/Query.py
+-rw-r--r--   0 ian        (501) staff       (20)     3613 2022-12-01 01:07:41.000000 redivis-0.9.1/src/redivis/classes/Row.py
+-rw-r--r--   0 ian        (501) staff       (20)    10776 2022-12-08 01:17:00.000000 redivis-0.9.1/src/redivis/classes/Table.py
+-rw-r--r--   0 ian        (501) staff       (20)    12812 2022-12-08 01:30:28.000000 redivis-0.9.1/src/redivis/classes/Upload.py
+-rw-r--r--   0 ian        (501) staff       (20)      999 2022-08-04 22:52:36.000000 redivis-0.9.1/src/redivis/classes/User.py
+-rw-r--r--   0 ian        (501) staff       (20)     1824 2022-11-13 21:16:52.000000 redivis-0.9.1/src/redivis/classes/Variable.py
+-rw-r--r--   0 ian        (501) staff       (20)        0 2022-01-20 02:39:33.000000 redivis-0.9.1/src/redivis/classes/__init__.py
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2022-12-08 01:45:11.579649 redivis-0.9.1/src/redivis/common/
+-rw-r--r--   0 ian        (501) staff       (20)        0 2022-07-13 03:05:08.000000 redivis-0.9.1/src/redivis/common/__init__.py
+-rw-r--r--   0 ian        (501) staff       (20)     3019 2022-11-14 00:14:51.000000 redivis-0.9.1/src/redivis/common/api_request.py
+-rw-r--r--   0 ian        (501) staff       (20)      236 2022-01-20 02:39:33.000000 redivis-0.9.1/src/redivis/common/auth.py
+-rw-r--r--   0 ian        (501) staff       (20)     4651 2022-12-01 00:34:51.000000 redivis-0.9.1/src/redivis/common/list_rows.py
+drwxr-xr-x   0 ian        (501) staff       (20)        0 2022-12-08 01:45:11.575187 redivis-0.9.1/src/redivis.egg-info/
+-rw-r--r--   0 ian        (501) staff       (20)     1661 2022-12-08 01:45:11.000000 redivis-0.9.1/src/redivis.egg-info/PKG-INFO
+-rw-r--r--   0 ian        (501) staff       (20)      733 2022-12-08 01:45:11.000000 redivis-0.9.1/src/redivis.egg-info/SOURCES.txt
+-rw-r--r--   0 ian        (501) staff       (20)        1 2022-12-08 01:45:11.000000 redivis-0.9.1/src/redivis.egg-info/dependency_links.txt
+-rw-r--r--   0 ian        (501) staff       (20)       76 2022-12-08 01:45:11.000000 redivis-0.9.1/src/redivis.egg-info/requires.txt
+-rw-r--r--   0 ian        (501) staff       (20)        8 2022-12-08 01:45:11.000000 redivis-0.9.1/src/redivis.egg-info/top_level.txt
```

### Comparing `redivis-0.9.0/LICENSE` & `redivis-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `redivis-0.9.0/PKG-INFO` & `redivis-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redivis
-Version: 0.9.0
+Version: 0.9.1
 Summary: Redivis python client library
 Home-page: https://github.com/redivis/redivis-python
 Author: Redivis Inc.
 Author-email: support@redivis.com
 License: MIT
 Description: 
         ![Redivis Logo](https://github.com/redivis/redivis-python/raw/main/assets/logo_small.png)
```

### Comparing `redivis-0.9.0/README.md` & `redivis-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `redivis-0.9.0/setup.py` & `redivis-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `redivis-0.9.0/src/redivis/classes/Base.py` & `redivis-0.9.1/src/redivis/classes/Base.py`

 * *Files identical despite different names*

### Comparing `redivis-0.9.0/src/redivis/classes/Dataset.py` & `redivis-0.9.1/src/redivis/classes/Dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -106,18 +106,23 @@
             Table(table["name"], dataset=self, properties=table) for table in tables
         ]
 
     def query(self, query):
         return Query(query, default_dataset=self.identifier)
 
     def release(self):
-        make_request(
+        res = make_request(
             method="POST",
             path=f"{self.uri}/versions/next/release",
         )
+        self.version = f'v{res["tag"]}'
+        self.identifier = (
+            f"{(self.organization or self.user).name}.{self.name}:{self.version}"
+        )
+        self.uri = f"/datasets/{quote_uri(self.identifier, '')}"
         return Dataset(
             name=self.name,
             user=self.user,
             organization=self.organization,
             version="current",
         ).get()
```

### Comparing `redivis-0.9.0/src/redivis/classes/File.py` & `redivis-0.9.1/src/redivis/classes/File.py`

 * *Files identical despite different names*

### Comparing `redivis-0.9.0/src/redivis/classes/Organization.py` & `redivis-0.9.1/src/redivis/classes/Organization.py`

 * *Files identical despite different names*

### Comparing `redivis-0.9.0/src/redivis/classes/Project.py` & `redivis-0.9.1/src/redivis/classes/Project.py`

 * *Files identical despite different names*

### Comparing `redivis-0.9.0/src/redivis/classes/Query.py` & `redivis-0.9.1/src/redivis/classes/Query.py`

 * *Files identical despite different names*

### Comparing `redivis-0.9.0/src/redivis/classes/Row.py` & `redivis-0.9.1/src/redivis/classes/Row.py`

 * *Files identical despite different names*

### Comparing `redivis-0.9.0/src/redivis/classes/Table.py` & `redivis-0.9.1/src/redivis/classes/Table.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,15 +260,15 @@
                 DeprecationWarning,
             )
             upload.create(
                 schema=schema,
                 type=type,
                 has_header_row=has_header_row,
                 skip_bad_records=skip_bad_records,
-                allow_quoted_newlines=allow_quoted_newlines,
+                has_quoted_newlines=allow_quoted_newlines,
                 quote_character=quote_character,
                 delimiter=delimiter,
             )
             upload.upload_file(
                 data,
                 wait_for_finish=True,
                 raise_on_fail=True,
```

### Comparing `redivis-0.9.0/src/redivis/classes/Upload.py` & `redivis-0.9.1/src/redivis/classes/Upload.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,31 +55,29 @@
         replace_on_conflict=False,
         allow_jagged_rows=False,
         if_not_exists=False,
         remove_on_fail=False,
         wait_for_finish=True,
         raise_on_fail=True,
     ):
-        data_is_file = False
         resumable_upload_id = None
 
-        if data:
-            data_is_file = hasattr(data, "read")
-
-        if data and data_is_file:
-            if os.stat(data.name).st_size > 1e7:
-                resumable_upload_id = self.upload_file(
-                    data,
-                    remove_on_fail=remove_on_fail,
-                    wait_for_finish=wait_for_finish,
-                    raise_on_fail=raise_on_fail,
-                    use_legacy_endpoint=False
-                )
-                data = None
-        elif data:
+        if data and (
+            (hasattr(data, "read") and os.stat(data.name).st_size > 1e7)
+            or (hasattr(data, "__len__") and len(data) > 1e7)
+        ):
+            resumable_upload_id = self.upload_file(
+                data,
+                remove_on_fail=remove_on_fail,
+                wait_for_finish=wait_for_finish,
+                raise_on_fail=raise_on_fail,
+                use_legacy_endpoint=False
+            )
+            data = None
+        elif data and not hasattr(data, "read"):
             data = io.StringIO(data)
 
         if schema and type != "stream":
             warnings.warn(
                 "The schema option is ignored for uploads that aren't of type `stream`"
             )
```

### Comparing `redivis-0.9.0/src/redivis/classes/User.py` & `redivis-0.9.1/src/redivis/classes/User.py`

 * *Files identical despite different names*

### Comparing `redivis-0.9.0/src/redivis/classes/Variable.py` & `redivis-0.9.1/src/redivis/classes/Variable.py`

 * *Files identical despite different names*

### Comparing `redivis-0.9.0/src/redivis/common/api_request.py` & `redivis-0.9.1/src/redivis/common/api_request.py`

 * *Files identical despite different names*

### Comparing `redivis-0.9.0/src/redivis/common/list_rows.py` & `redivis-0.9.1/src/redivis/common/list_rows.py`

 * *Files identical despite different names*

### Comparing `redivis-0.9.0/src/redivis.egg-info/PKG-INFO` & `redivis-0.9.1/src/redivis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redivis
-Version: 0.9.0
+Version: 0.9.1
 Summary: Redivis python client library
 Home-page: https://github.com/redivis/redivis-python
 Author: Redivis Inc.
 Author-email: support@redivis.com
 License: MIT
 Description: 
         ![Redivis Logo](https://github.com/redivis/redivis-python/raw/main/assets/logo_small.png)
```

### Comparing `redivis-0.9.0/src/redivis.egg-info/SOURCES.txt` & `redivis-0.9.1/src/redivis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

