# Comparing `tmp/maestro_compose-0.1.8.tar.gz` & `tmp/maestro_compose-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maestro_compose-0.1.8.tar", max compression
+gzip compressed data, was "maestro_compose-0.1.9.tar", max compression
```

## Comparing `maestro_compose-0.1.8.tar` & `maestro_compose-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     4189 2024-05-26 03:15:19.000000 maestro_compose-0.1.8/README.md
--rw-r--r--   0        0        0       57 2024-05-26 03:15:19.000000 maestro_compose-0.1.8/maestro_compose/__init__.py
--rw-r--r--   0        0        0     2285 2024-05-29 23:43:49.957896 maestro_compose-0.1.8/maestro_compose/__main__.py
--rw-r--r--   0        0        0     8474 2024-05-30 00:50:52.046229 maestro_compose-0.1.8/maestro_compose/commands.py
--rw-r--r--   0        0        0     1386 2024-05-29 23:49:52.873322 maestro_compose-0.1.8/maestro_compose/models.py
--rw-r--r--   0        0        0      841 2024-05-30 00:51:08.488257 maestro_compose-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     5198 1970-01-01 00:00:00.000000 maestro_compose-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     4189 2024-05-26 03:15:19.000000 maestro_compose-0.1.9/README.md
+-rw-r--r--   0        0        0       57 2024-05-26 03:15:19.000000 maestro_compose-0.1.9/maestro_compose/__init__.py
+-rw-r--r--   0        0        0     2285 2024-05-29 23:43:49.957896 maestro_compose-0.1.9/maestro_compose/__main__.py
+-rw-r--r--   0        0        0     8521 2024-05-30 00:54:31.696586 maestro_compose-0.1.9/maestro_compose/commands.py
+-rw-r--r--   0        0        0     1386 2024-05-29 23:49:52.873322 maestro_compose-0.1.9/maestro_compose/models.py
+-rw-r--r--   0        0        0      841 2024-05-30 00:54:38.004596 maestro_compose-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     5198 1970-01-01 00:00:00.000000 maestro_compose-0.1.9/PKG-INFO
```

### Comparing `maestro_compose-0.1.8/README.md` & `maestro_compose-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `maestro_compose-0.1.8/maestro_compose/__main__.py` & `maestro_compose-0.1.9/maestro_compose/__main__.py`

 * *Files identical despite different names*

### Comparing `maestro_compose-0.1.8/maestro_compose/commands.py` & `maestro_compose-0.1.9/maestro_compose/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
         all_labels.append(
             {
                 "application": formatted_labels["com.docker.compose.project"],
                 "container": container["Names"],
                 "status": format_color(container["State"], STATUS_COLOR_MAP),
             }
         )
-    return pd.DataFrame(all_labels)
+    return pd.DataFrame(all_labels, column=["application", "container", "status"])
 
 
 def filter_dataframe(df, column_name, include, exclude):
     if df.empty:
         return df
 
     def should_include(row):
```

### Comparing `maestro_compose-0.1.8/maestro_compose/models.py` & `maestro_compose-0.1.9/maestro_compose/models.py`

 * *Files identical despite different names*

### Comparing `maestro_compose-0.1.8/pyproject.toml` & `maestro_compose-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "maestro-compose"
-version = "0.1.8"
+version = "0.1.9"
 description = "A simple command line tool for managing Docker Compose stacks using tags and other metadata."
 license = "MIT"
 authors = ["Nick Schenone <nschenone16@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/nschenone/maestro-compose"
 
 [tool.poetry.dependencies]
```

### Comparing `maestro_compose-0.1.8/PKG-INFO` & `maestro_compose-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maestro-compose
-Version: 0.1.8
+Version: 0.1.9
 Summary: A simple command line tool for managing Docker Compose stacks using tags and other metadata.
 Home-page: https://github.com/nschenone/maestro-compose
 License: MIT
 Author: Nick Schenone
 Author-email: nschenone16@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

