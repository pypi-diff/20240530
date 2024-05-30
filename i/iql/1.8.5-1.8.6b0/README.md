# Comparing `tmp/iql-1.8.5.tar.gz` & `tmp/iql-1.8.6b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iql-1.8.5.tar", max compression
+gzip compressed data, was "iql-1.8.6b0.tar", max compression
```

## Comparing `iql-1.8.5.tar` & `iql-1.8.6b0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1479 2024-05-29 22:02:15.805896 iql-1.8.5/LICENSE
--rw-r--r--   0        0        0    16466 2024-05-29 22:02:15.805896 iql-1.8.5/README.md
--rw-r--r--   0        0        0      780 2024-05-29 22:02:15.805896 iql-1.8.5/iql/__init__.py
--rw-r--r--   0        0        0      928 2024-05-29 22:02:15.805896 iql-1.8.5/iql/constants.py
--rw-r--r--   0        0        0        0 2024-05-29 22:02:15.805896 iql-1.8.5/iql/datamodel/__init__.py
--rw-r--r--   0        0        0      703 2024-05-29 22:02:15.805896 iql-1.8.5/iql/datamodel/cache.py
--rw-r--r--   0        0        0      731 2024-05-29 22:02:15.805896 iql-1.8.5/iql/datamodel/database.py
--rw-r--r--   0        0        0    19905 2024-05-29 22:02:15.805896 iql-1.8.5/iql/datamodel/extension.py
--rw-r--r--   0        0        0     6464 2024-05-29 22:02:15.805896 iql-1.8.5/iql/datamodel/querycontainer.py
--rw-r--r--   0        0        0      944 2024-05-29 22:02:15.805896 iql-1.8.5/iql/datamodel/result.py
--rw-r--r--   0        0        0     5526 2024-05-29 22:02:15.805896 iql-1.8.5/iql/datamodel/subquery.py
--rw-r--r--   0        0        0        1 2024-05-29 22:02:15.805896 iql-1.8.5/iql/db_connectors/__init__.py
--rw-r--r--   0        0        0     3757 2024-05-29 22:02:15.805896 iql-1.8.5/iql/db_connectors/duckdb_connector.py
--rw-r--r--   0        0        0        1 2024-05-29 22:02:15.805896 iql-1.8.5/iql/extensions/__init__.py
--rw-r--r--   0        0        0      298 2024-05-29 22:02:15.805896 iql-1.8.5/iql/extensions/blpapi_ext/README.txt
--rw-r--r--   0        0        0        1 2024-05-29 22:02:15.805896 iql-1.8.5/iql/extensions/blpapi_ext/__init__.py
--rw-r--r--   0        0        0     7134 2024-05-29 22:02:15.805896 iql-1.8.5/iql/extensions/blpapi_ext/blp_api_lowlevel.py
--rw-r--r--   0        0        0     3140 2024-05-29 22:02:15.805896 iql-1.8.5/iql/extensions/blpapi_ext/blp_extension.py
--rw-r--r--   0        0        0        1 2024-05-29 22:02:15.805896 iql-1.8.5/iql/extensions/bql_ext/__init__.py
--rw-r--r--   0        0        0     3974 2024-05-29 22:02:15.805896 iql-1.8.5/iql/extensions/bql_ext/bql_datamodel.py
--rw-r--r--   0        0        0     7262 2024-05-29 22:02:15.805896 iql-1.8.5/iql/extensions/bql_ext/bql_extension.py
--rw-r--r--   0        0        0     2701 2024-05-29 22:02:15.805896 iql-1.8.5/iql/extensions/bql_ext/bql_service.py
--rw-r--r--   0        0        0    15106 2024-05-29 22:02:15.805896 iql-1.8.5/iql/extensions/bql_ext/bql_wrapper.py
--rw-r--r--   0        0        0     2610 2024-05-29 22:02:15.805896 iql-1.8.5/iql/extensions/cache_extension.py
--rw-r--r--   0        0        0     3560 2024-05-29 22:02:15.805896 iql-1.8.5/iql/extensions/pandas_extension.py
--rw-r--r--   0        0        0        1 2024-05-29 22:02:15.805896 iql-1.8.5/iql/jupyter_magics/__init__.py
--rw-r--r--   0        0        0     4621 2024-05-29 22:02:15.805896 iql-1.8.5/iql/jupyter_magics/iql_magic.py
--rw-r--r--   0        0        0     1212 2024-05-29 22:02:15.805896 iql-1.8.5/iql/options_parser.py
--rw-r--r--   0        0        0     8537 2024-05-29 22:02:15.805896 iql-1.8.5/iql/ql.py
--rw-r--r--   0        0        0     2706 2024-05-29 22:02:15.805896 iql-1.8.5/iql/utils.py
--rw-r--r--   0        0        0       22 2024-05-29 22:02:15.805896 iql-1.8.5/iql/version.py
--rw-r--r--   0        0        0     1798 2024-05-29 22:02:35.078115 iql-1.8.5/pyproject.toml
--rw-r--r--   0        0        0    17374 1970-01-01 00:00:00.000000 iql-1.8.5/PKG-INFO
+-rw-r--r--   0        0        0     1479 2024-05-30 17:32:24.462438 iql-1.8.6b0/LICENSE
+-rw-r--r--   0        0        0    16466 2024-05-30 17:32:24.462438 iql-1.8.6b0/README.md
+-rw-r--r--   0        0        0      780 2024-05-30 17:32:24.462438 iql-1.8.6b0/iql/__init__.py
+-rw-r--r--   0        0        0      928 2024-05-30 17:32:24.462438 iql-1.8.6b0/iql/constants.py
+-rw-r--r--   0        0        0        0 2024-05-30 17:32:24.462438 iql-1.8.6b0/iql/datamodel/__init__.py
+-rw-r--r--   0        0        0      703 2024-05-30 17:32:24.462438 iql-1.8.6b0/iql/datamodel/cache.py
+-rw-r--r--   0        0        0      731 2024-05-30 17:32:24.462438 iql-1.8.6b0/iql/datamodel/database.py
+-rw-r--r--   0        0        0    21138 2024-05-30 17:32:24.462438 iql-1.8.6b0/iql/datamodel/extension.py
+-rw-r--r--   0        0        0     6547 2024-05-30 17:32:24.462438 iql-1.8.6b0/iql/datamodel/querycontainer.py
+-rw-r--r--   0        0        0      944 2024-05-30 17:32:24.462438 iql-1.8.6b0/iql/datamodel/result.py
+-rw-r--r--   0        0        0     5526 2024-05-30 17:32:24.462438 iql-1.8.6b0/iql/datamodel/subquery.py
+-rw-r--r--   0        0        0        1 2024-05-30 17:32:24.462438 iql-1.8.6b0/iql/db_connectors/__init__.py
+-rw-r--r--   0        0        0     3757 2024-05-30 17:32:24.462438 iql-1.8.6b0/iql/db_connectors/duckdb_connector.py
+-rw-r--r--   0        0        0        1 2024-05-30 17:32:24.462438 iql-1.8.6b0/iql/extensions/__init__.py
+-rw-r--r--   0        0        0      298 2024-05-30 17:32:24.462438 iql-1.8.6b0/iql/extensions/blpapi_ext/README.txt
+-rw-r--r--   0        0        0        1 2024-05-30 17:32:24.462438 iql-1.8.6b0/iql/extensions/blpapi_ext/__init__.py
+-rw-r--r--   0        0        0     7134 2024-05-30 17:32:24.462438 iql-1.8.6b0/iql/extensions/blpapi_ext/blp_api_lowlevel.py
+-rw-r--r--   0        0        0     3140 2024-05-30 17:32:24.462438 iql-1.8.6b0/iql/extensions/blpapi_ext/blp_extension.py
+-rw-r--r--   0        0        0        1 2024-05-30 17:32:24.462438 iql-1.8.6b0/iql/extensions/bql_ext/__init__.py
+-rw-r--r--   0        0        0     3974 2024-05-30 17:32:24.462438 iql-1.8.6b0/iql/extensions/bql_ext/bql_datamodel.py
+-rw-r--r--   0        0        0     7262 2024-05-30 17:32:24.462438 iql-1.8.6b0/iql/extensions/bql_ext/bql_extension.py
+-rw-r--r--   0        0        0     2701 2024-05-30 17:32:24.462438 iql-1.8.6b0/iql/extensions/bql_ext/bql_service.py
+-rw-r--r--   0        0        0    15106 2024-05-30 17:32:24.466439 iql-1.8.6b0/iql/extensions/bql_ext/bql_wrapper.py
+-rw-r--r--   0        0        0     2610 2024-05-30 17:32:24.466439 iql-1.8.6b0/iql/extensions/cache_extension.py
+-rw-r--r--   0        0        0     3560 2024-05-30 17:32:24.466439 iql-1.8.6b0/iql/extensions/pandas_extension.py
+-rw-r--r--   0        0        0        1 2024-05-30 17:32:24.466439 iql-1.8.6b0/iql/jupyter_magics/__init__.py
+-rw-r--r--   0        0        0     4621 2024-05-30 17:32:24.466439 iql-1.8.6b0/iql/jupyter_magics/iql_magic.py
+-rw-r--r--   0        0        0     1212 2024-05-30 17:32:24.466439 iql-1.8.6b0/iql/options_parser.py
+-rw-r--r--   0        0        0     8537 2024-05-30 17:32:24.466439 iql-1.8.6b0/iql/ql.py
+-rw-r--r--   0        0        0     2706 2024-05-30 17:32:24.466439 iql-1.8.6b0/iql/utils.py
+-rw-r--r--   0        0        0       22 2024-05-30 17:32:24.466439 iql-1.8.6b0/iql/version.py
+-rw-r--r--   0        0        0     1791 2024-05-30 17:32:39.078470 iql-1.8.6b0/pyproject.toml
+-rw-r--r--   0        0        0    17376 1970-01-01 00:00:00.000000 iql-1.8.6b0/PKG-INFO
```

### Comparing `iql-1.8.5/LICENSE` & `iql-1.8.6b0/LICENSE`

 * *Files identical despite different names*

### Comparing `iql-1.8.5/README.md` & `iql-1.8.6b0/README.md`

 * *Files identical despite different names*

### Comparing `iql-1.8.5/iql/__init__.py` & `iql-1.8.6b0/iql/__init__.py`

 * *Files identical despite different names*

### Comparing `iql-1.8.5/iql/constants.py` & `iql-1.8.6b0/iql/constants.py`

 * *Files identical despite different names*

### Comparing `iql-1.8.5/iql/datamodel/cache.py` & `iql-1.8.6b0/iql/datamodel/cache.py`

 * *Files identical despite different names*

### Comparing `iql-1.8.5/iql/datamodel/database.py` & `iql-1.8.6b0/iql/datamodel/database.py`

 * *Files identical despite different names*

### Comparing `iql-1.8.5/iql/datamodel/extension.py` & `iql-1.8.6b0/iql/datamodel/extension.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import logging
 from abc import abstractmethod
 from dataclasses import dataclass, field
 from typing import Callable, Dict, Iterable, Optional, Tuple, Union
 
 from pandas import DataFrame
 
@@ -15,14 +16,15 @@
 
 
 @dataclass
 class IqlExtension:
     keyword: str
     subword: str = field(default=None, init=True)  # type: ignore
     cacheable: bool = False
+    is_async: bool = False  # Determines whether executeimpl is implemented asynchronously
 
     # Extensions must be parallelizable, or must
     # implement their own execute_batch.
 
     # Determines whether the local cache settings should be used
     # vs  CACHE_PERIOD and
     # USE_FILE_CACHE
@@ -36,15 +38,15 @@
         return tempdir
 
     def allow_cache_read(self, sq: subquery.SubQuery) -> bool:
         """Caching can be dangerous because of downstream affects, use it for
         truly idempotent queries"""
 
         cacheable = bool(sq.options.get("cache", self.cacheable))
-        #logger.debug(f"{sq.options.get('cache', None)=}, {self.cacheable=}, {self}")
+        # logger.debug(f"{sq.options.get('cache', None)=}, {self.cacheable=}, {self}")
         return cacheable
 
     def allow_cache_save(self, sq: subquery.SubQuery) -> bool:
         return self.allow_cache_read(sq)
 
     def use_path_replacement(self) -> bool:
         """Some extensions just return a filestring to use instead of the SubQuery, such as the
@@ -112,41 +114,65 @@
         cache_policy: Optional[Dict[str, object]] = None,
     ) -> Iterable[IqlResultData]:
         """This is a default implementation that executes each of the queries serially.
 
         Extensions may override this for cases that could be executed concurrently, such as BQL.
 
         """
-
-        completed_results = []
-        # context = get_context('spawn')
-
-        subqueries_flat = subquery.get_subqueries_flat(queries)
-
-        # Executes the ungrouped queries
-        for query in subqueries_flat:
+        if self.is_async:
+            # Execute as a batch
+            # If run in Jupyter, needs nest_async to allow nested async.
+            logger.debug("Executing batch of %s queries", len(list(queries)))
             try:
-                self.execute(query)  # type: ignore
-            except Exception as e:
-                logger.exception("Error in %s", query)
-                raise e
-
-        # Merge the results
-        for query in queries:
-            # For single subqueries, this is a noop
-            # For subquery groups, this merges the results of the children
-            query.merge()
-
-            if self.use_path_replacement():
-                continue
+                # To allow jupyter
+                loop = asyncio.get_running_loop()
+            except RuntimeError:
+                loop = asyncio.new_event_loop()
+                asyncio.set_event_loop(loop)
+                g = asyncio.gather(*(self.executeimpl(sq) for sq in queries))
+                results = loop.run_until_complete(g)
             else:
-                ir = IqlResultData(name=query.name, query=query.subquery, _data=query.dataframe)
-                completed_results.append(ir)
+                g = asyncio.gather(*(self.executeimpl(sq) for sq in queries))
+                results = asyncio.run(g)
+
+            completed_results = []
+            for sq, df in zip(queries, results):
+                sq.dataframe = df
+                ird = IqlResultData(name=sq.name, query=sq.subquery, _data=sq.dataframe)
+                completed_results.append(ird)
+
+            return completed_results
+        else:
+            # Execute serially
+            completed_results = []
+            # context = get_context('spawn')
+
+            subqueries_flat = subquery.get_subqueries_flat(queries)
+
+            # Executes the ungrouped queries
+            for query in subqueries_flat:
+                try:
+                    self.execute(query)  # type: ignore
+                except Exception as e:
+                    logger.exception("Error in %s", query)
+                    raise e
+
+            # Merge the results
+            for query in queries:
+                # For single subqueries, this is a noop
+                # For subquery groups, this merges the results of the children
+                query.merge()
+
+                if self.use_path_replacement():
+                    continue
+                else:
+                    ir = IqlResultData(name=query.name, query=query.subquery, _data=query.dataframe)
+                    completed_results.append(ir)
 
-        return completed_results
+            return completed_results
 
     def create_subquery(self, query: str, name: str, iqc: IqlQueryContainer) -> subquery.SubQuery:
         logger.debug("Creating subquery")
         sq = subquery.SubQuery(extension=self, subquery=query, name=name, iqc=iqc)
         return sq
 
     def create_subqueries(
```

### Comparing `iql-1.8.5/iql/datamodel/querycontainer.py` & `iql-1.8.6b0/iql/datamodel/querycontainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,17 @@
             return (df, [])  # type: ignore
 
         for (
             keyword,
             subword,
         ), e in ql._EXTENSIONS.copy().items():  # copy to prevent dictionary changed size during iteration error
             sqs: Iterable[subquery.SubQuery] = self.get_subqueries_by_extension(keyword, subword)  # type: ignore
+            sqs = list(sqs)
+            if len(sqs) == 0:
+                continue
 
             # If the cache policy has a policy for the subtype, use that, otherwise use defaults
             # Don't use the top level cache policy
             sub_policy: Optional[Dict[str, object]] = (  # type: ignore
                 self.cache_policy.get(keyword, None)  # type: ignore
                 if self.cache_policy is not None
                 else None
```

### Comparing `iql-1.8.5/iql/datamodel/result.py` & `iql-1.8.6b0/iql/datamodel/result.py`

 * *Files identical despite different names*

### Comparing `iql-1.8.5/iql/datamodel/subquery.py` & `iql-1.8.6b0/iql/datamodel/subquery.py`

 * *Files identical despite different names*

### Comparing `iql-1.8.5/iql/db_connectors/duckdb_connector.py` & `iql-1.8.6b0/iql/db_connectors/duckdb_connector.py`

 * *Files identical despite different names*

### Comparing `iql-1.8.5/iql/extensions/blpapi_ext/blp_api_lowlevel.py` & `iql-1.8.6b0/iql/extensions/blpapi_ext/blp_api_lowlevel.py`

 * *Files identical despite different names*

### Comparing `iql-1.8.5/iql/extensions/blpapi_ext/blp_extension.py` & `iql-1.8.6b0/iql/extensions/blpapi_ext/blp_extension.py`

 * *Files identical despite different names*

### Comparing `iql-1.8.5/iql/extensions/bql_ext/bql_datamodel.py` & `iql-1.8.6b0/iql/extensions/bql_ext/bql_datamodel.py`

 * *Files identical despite different names*

### Comparing `iql-1.8.5/iql/extensions/bql_ext/bql_extension.py` & `iql-1.8.6b0/iql/extensions/bql_ext/bql_extension.py`

 * *Files identical despite different names*

### Comparing `iql-1.8.5/iql/extensions/bql_ext/bql_service.py` & `iql-1.8.6b0/iql/extensions/bql_ext/bql_service.py`

 * *Files identical despite different names*

### Comparing `iql-1.8.5/iql/extensions/bql_ext/bql_wrapper.py` & `iql-1.8.6b0/iql/extensions/bql_ext/bql_wrapper.py`

 * *Files identical despite different names*

### Comparing `iql-1.8.5/iql/extensions/cache_extension.py` & `iql-1.8.6b0/iql/extensions/cache_extension.py`

 * *Files identical despite different names*

### Comparing `iql-1.8.5/iql/extensions/pandas_extension.py` & `iql-1.8.6b0/iql/extensions/pandas_extension.py`

 * *Files identical despite different names*

### Comparing `iql-1.8.5/iql/jupyter_magics/iql_magic.py` & `iql-1.8.6b0/iql/jupyter_magics/iql_magic.py`

 * *Files identical despite different names*

### Comparing `iql-1.8.5/iql/options_parser.py` & `iql-1.8.6b0/iql/options_parser.py`

 * *Files identical despite different names*

### Comparing `iql-1.8.5/iql/ql.py` & `iql-1.8.6b0/iql/ql.py`

 * *Files identical despite different names*

### Comparing `iql-1.8.5/iql/utils.py` & `iql-1.8.6b0/iql/utils.py`

 * *Files identical despite different names*

### Comparing `iql-1.8.5/pyproject.toml` & `iql-1.8.6b0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning>=1.0.0,<2.0.0"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "iql"
-version = "1.8.5"
+version = "1.8.6-beta"
 description = "I* Query Language"
 authors = ["Paul T <paul@iqmo.com>"]
 maintainers =  ["Paul T <paul@iqmo.com>"]
 packages = [
     { include = "iql", from = "."}
     ]
 readme = "README.md"
@@ -38,14 +38,15 @@
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.2.1"
 pytest-cov = "^5.0.0"
 pytest-xdist = "^3.6.1"
 bql = {path = "tests/simulators/bql_simulator", develop = true}
 ipykernel = "^6.29.4"
 ipython = "^8.24.0"
+pre-commit = "^3.7.1"
 
 [tool.ruff]
 line-length = 120
 exclude = [
     ".git",
     "__pycache__",
     "build",
@@ -58,15 +59,14 @@
     "W291",
     "E501" ]
 extend-include = ["*.ipynb"]
 
 [tool.ruff.lint]
 # pyflakes, pycodestyle, isort
 select = ["F", "E", "W", "I001"]
-ignore-init-module-imports = true
 
 [tool.pyright]
 typeCheckingMode = "basic"
 reportGeneralTypeIssues = false
 reportPrivateImportUsage = false
 reportAttributeAccessIssue = false 
 exclude = ["tests/**"]
```

### Comparing `iql-1.8.5/PKG-INFO` & `iql-1.8.6b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iql
-Version: 1.8.5
+Version: 1.8.6b0
 Summary: I* Query Language
 Home-page: https://github.com/iqmo-org/iql
 Keywords: iql,query language,duckdb,bql,blpapi
 Author: Paul T
 Author-email: paul@iqmo.com
 Maintainer: Paul T
 Maintainer-email: paul@iqmo.com
```

