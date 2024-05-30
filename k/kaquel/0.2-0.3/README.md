# Comparing `tmp/kaquel-0.2.tar.gz` & `tmp/kaquel-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaquel-0.2.tar", max compression
+gzip compressed data, was "kaquel-0.3.tar", max compression
```

## Comparing `kaquel-0.2.tar` & `kaquel-0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    21863 2024-05-23 19:37:57.637723 kaquel-0.2/LICENSE.txt
--rw-r--r--   0        0        0     1184 2024-05-23 19:37:57.637723 kaquel-0.2/README.rst
--rw-r--r--   0        0        0     1771 2024-05-23 19:37:57.639723 kaquel-0.2/kaquel/__init__.py
--rw-r--r--   0        0        0     2675 2024-05-23 19:37:57.640723 kaquel-0.2/kaquel/errors.py
--rw-r--r--   0        0        0     5806 2024-05-23 19:37:57.640723 kaquel-0.2/kaquel/es_query.py
--rw-r--r--   0        0        0    22254 2024-05-23 19:37:57.640723 kaquel-0.2/kaquel/kql.py
--rw-r--r--   0        0        0     2323 2024-05-23 19:37:57.640723 kaquel-0.2/kaquel/lucene.py
--rw-r--r--   0        0        0        0 2024-05-23 19:37:57.674723 kaquel-0.2/kaquel/py.typed
--rw-r--r--   0        0        0    12480 2024-05-23 19:37:57.640723 kaquel-0.2/kaquel/query.py
--rw-r--r--   0        0        0     2482 2024-05-23 19:37:57.640723 kaquel-0.2/kaquel/utils.py
--rw-r--r--   0        0        0     3115 2024-05-23 19:37:57.641723 kaquel-0.2/pyproject.toml
--rw-r--r--   0        0        0     2350 1970-01-01 00:00:00.000000 kaquel-0.2/PKG-INFO
+-rw-r--r--   0        0        0    21863 2024-05-30 15:24:42.959577 kaquel-0.3/LICENSE.txt
+-rw-r--r--   0        0        0     1184 2024-05-30 15:24:42.959577 kaquel-0.3/README.rst
+-rw-r--r--   0        0        0     1771 2024-05-30 15:24:42.961577 kaquel-0.3/kaquel/__init__.py
+-rw-r--r--   0        0        0     2760 2024-05-30 15:24:42.961577 kaquel-0.3/kaquel/errors.py
+-rw-r--r--   0        0        0     5810 2024-05-30 15:24:42.961577 kaquel-0.3/kaquel/es_query.py
+-rw-r--r--   0        0        0    31933 2024-05-30 15:24:42.962577 kaquel-0.3/kaquel/kql.py
+-rw-r--r--   0        0        0     2323 2024-05-30 15:24:42.962577 kaquel-0.3/kaquel/lucene.py
+-rw-r--r--   0        0        0        0 2024-05-30 15:24:42.994576 kaquel-0.3/kaquel/py.typed
+-rw-r--r--   0        0        0    12479 2024-05-30 15:24:42.962577 kaquel-0.3/kaquel/query.py
+-rw-r--r--   0        0        0     2482 2024-05-30 15:24:42.962577 kaquel-0.3/kaquel/utils.py
+-rw-r--r--   0        0        0     3115 2024-05-30 15:24:42.963577 kaquel-0.3/pyproject.toml
+-rw-r--r--   0        0        0     2350 1970-01-01 00:00:00.000000 kaquel-0.3/PKG-INFO
```

### Comparing `kaquel-0.2/LICENSE.txt` & `kaquel-0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kaquel-0.2/README.rst` & `kaquel-0.3/README.rst`

 * *Files identical despite different names*

### Comparing `kaquel-0.2/kaquel/__init__.py` & `kaquel-0.3/kaquel/__init__.py`

 * *Files identical despite different names*

### Comparing `kaquel-0.2/kaquel/errors.py` & `kaquel-0.3/kaquel/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,7 +66,11 @@
 
 
 class LeadingWildcardsForbidden(Error):
     """A leading wildcard was found, while the feature was disabled."""
 
     def __init__(self, /) -> None:
         super().__init__("Leading wildcards are forbidden.")
+
+
+class RenderError(Error):
+    """An error has occurred while rendering a query."""
```

### Comparing `kaquel-0.2/kaquel/es_query.py` & `kaquel-0.3/kaquel/es_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,23 +96,23 @@
                 if key not in content:
                     continue
 
                 if isinstance(content[key], list):
                     content[key] = [
                         _parse_es_query(
                             element,
-                            context=context + "bool[must{i}].",
+                            context=context + f"bool[{key}{i}].",
                         )
                         for i, element in enumerate(content[key])
                     ]
                 else:
                     content[key] = [
                         _parse_es_query(
                             content[key],
-                            context=context + "bool[must0].",
+                            context=context + f"bool[{key}0].",
                         ),
                     ]
 
             return BooleanQuery(**content)
         elif typ == "exists":
             return ExistsQuery(**content)
         elif typ == "match_all":
```

### Comparing `kaquel-0.2/kaquel/lucene.py` & `kaquel-0.3/kaquel/lucene.py`

 * *Files identical despite different names*

### Comparing `kaquel-0.2/kaquel/query.py` & `kaquel-0.3/kaquel/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
 class ExistsQuery(Query):
     """Exists query.
 
     See `Exists query`_ for more information.
 
     .. _Exists query:
         https://www.elastic.co/guide/en/elasticsearch/reference/current/
-        query-dsl-exists-query.html`
+        query-dsl-exists-query.html
     """
 
     field: Annotated[str, StringConstraints(min_length=1)]
     """Name of the field to check the existence of."""
 
     def render(self, /) -> dict:
         """Render as a Python dictionary.
```

### Comparing `kaquel-0.2/kaquel/utils.py` & `kaquel-0.3/kaquel/utils.py`

 * *Files identical despite different names*

### Comparing `kaquel-0.2/pyproject.toml` & `kaquel-0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "kaquel"
-version = "0.2"
+version = "0.3"
 description = "Tools for handling ElasticSearch queries in various languages"
 readme = "README.rst"
 homepage = "https://kaquel.touhey.pro/"
 repository = "https://gitlab.com/thomas.touhey/kaquel"
 authors = ["Thomas Touhey <thomas@touhey.fr>"]
 keywords = [
     "elasticsearch",
```

### Comparing `kaquel-0.2/PKG-INFO` & `kaquel-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaquel
-Version: 0.2
+Version: 0.3
 Summary: Tools for handling ElasticSearch queries in various languages
 Home-page: https://kaquel.touhey.pro/
 Keywords: elasticsearch,es_query,es-query,kibana,kql,lucene,parsing,query
 Author: Thomas Touhey
 Author-email: thomas@touhey.fr
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

