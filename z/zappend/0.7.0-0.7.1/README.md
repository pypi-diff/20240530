# Comparing `tmp/zappend-0.7.0.tar.gz` & `tmp/zappend-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zappend-0.7.0.tar", last modified: Tue Mar 19 16:37:00 2024, max compression
+gzip compressed data, was "zappend-0.7.1.tar", last modified: Thu May 30 10:50:26 2024, max compression
```

## Comparing `zappend-0.7.0.tar` & `zappend-0.7.1.tar`

### file list

```diff
@@ -1,62 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:37:00.743400 zappend-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-03-19 16:36:52.000000 zappend-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4998 2024-03-19 16:37:00.743400 zappend-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-03-19 16:36:52.000000 zappend-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-19 16:36:52.000000 zappend-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-19 16:36:52.000000 zappend-0.7.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-19 16:36:52.000000 zappend-0.7.0/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-19 16:36:52.000000 zappend-0.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-03-19 16:37:00.743400 zappend-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:37:00.735400 zappend-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    17683 2024-03-19 16:36:52.000000 zappend-0.7.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-03-19 16:36:52.000000 zappend-0.7.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-03-19 16:36:52.000000 zappend-0.7.0/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-03-19 16:36:52.000000 zappend-0.7.0/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (127)    21520 2024-03-19 16:36:52.000000 zappend-0.7.0/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     9667 2024-03-19 16:36:52.000000 zappend-0.7.0/tests/test_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-03-19 16:36:52.000000 zappend-0.7.0/tests/test_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-03-19 16:36:52.000000 zappend-0.7.0/tests/test_rollbackstore.py
--rw-r--r--   0 runner    (1001) docker     (127)    10317 2024-03-19 16:36:52.000000 zappend-0.7.0/tests/test_tailoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     8324 2024-03-19 16:36:52.000000 zappend-0.7.0/tests/test_xrencoding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:37:00.735400 zappend-0.7.0/zappend/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-19 16:36:52.000000 zappend-0.7.0/zappend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-03-19 16:36:52.000000 zappend-0.7.0/zappend/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-03-19 16:36:52.000000 zappend-0.7.0/zappend/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:37:00.739400 zappend-0.7.0/zappend/config/
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-03-19 16:36:52.000000 zappend-0.7.0/zappend/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-03-19 16:36:52.000000 zappend-0.7.0/zappend/config/attrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7450 2024-03-19 16:36:52.000000 zappend-0.7.0/zappend/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-19 16:36:52.000000 zappend-0.7.0/zappend/config/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-03-19 16:36:52.000000 zappend-0.7.0/zappend/config/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-03-19 16:36:52.000000 zappend-0.7.0/zappend/config/normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)    28739 2024-03-19 16:36:52.000000 zappend-0.7.0/zappend/config/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-03-19 16:36:52.000000 zappend-0.7.0/zappend/config/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-03-19 16:36:52.000000 zappend-0.7.0/zappend/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:37:00.739400 zappend-0.7.0/zappend/fsutil/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-19 16:36:52.000000 zappend-0.7.0/zappend/fsutil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8092 2024-03-19 16:36:52.000000 zappend-0.7.0/zappend/fsutil/fileobj.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-03-19 16:36:52.000000 zappend-0.7.0/zappend/fsutil/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     8540 2024-03-19 16:36:52.000000 zappend-0.7.0/zappend/fsutil/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-03-19 16:36:52.000000 zappend-0.7.0/zappend/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    14800 2024-03-19 16:36:52.000000 zappend-0.7.0/zappend/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-03-19 16:36:52.000000 zappend-0.7.0/zappend/processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-03-19 16:36:52.000000 zappend-0.7.0/zappend/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-03-19 16:36:52.000000 zappend-0.7.0/zappend/rollbackstore.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:37:00.739400 zappend-0.7.0/zappend/slice/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-19 16:36:52.000000 zappend-0.7.0/zappend/slice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-03-19 16:36:52.000000 zappend-0.7.0/zappend/slice/callable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-03-19 16:36:52.000000 zappend-0.7.0/zappend/slice/cm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-03-19 16:36:52.000000 zappend-0.7.0/zappend/slice/source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:37:00.739400 zappend-0.7.0/zappend/slice/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-19 16:36:52.000000 zappend-0.7.0/zappend/slice/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-03-19 16:36:52.000000 zappend-0.7.0/zappend/slice/sources/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-03-19 16:36:52.000000 zappend-0.7.0/zappend/slice/sources/persistent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-03-19 16:36:52.000000 zappend-0.7.0/zappend/slice/sources/temporary.py
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-03-19 16:36:52.000000 zappend-0.7.0/zappend/tailoring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:37:00.739400 zappend-0.7.0/zappend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4998 2024-03-19 16:37:00.000000 zappend-0.7.0/zappend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-03-19 16:37:00.000000 zappend-0.7.0/zappend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 16:37:00.000000 zappend-0.7.0/zappend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-19 16:37:00.000000 zappend-0.7.0/zappend.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-19 16:37:00.000000 zappend-0.7.0/zappend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-19 16:37:00.000000 zappend-0.7.0/zappend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:50:26.623657 zappend-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-30 10:50:22.000000 zappend-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-30 10:50:26.623657 zappend-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-30 10:50:22.000000 zappend-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-30 10:50:22.000000 zappend-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 10:50:26.623657 zappend-0.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:50:26.619657 zappend-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    17984 2024-05-30 10:50:22.000000 zappend-0.7.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-30 10:50:22.000000 zappend-0.7.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-30 10:50:22.000000 zappend-0.7.1/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-05-30 10:50:22.000000 zappend-0.7.1/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21520 2024-05-30 10:50:22.000000 zappend-0.7.1/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9667 2024-05-30 10:50:22.000000 zappend-0.7.1/tests/test_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-05-30 10:50:22.000000 zappend-0.7.1/tests/test_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-05-30 10:50:22.000000 zappend-0.7.1/tests/test_rollbackstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10317 2024-05-30 10:50:22.000000 zappend-0.7.1/tests/test_tailoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-05-30 10:50:22.000000 zappend-0.7.1/tests/test_xrencoding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:50:26.619657 zappend-0.7.1/zappend/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-30 10:50:22.000000 zappend-0.7.1/zappend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-05-30 10:50:22.000000 zappend-0.7.1/zappend/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-05-30 10:50:22.000000 zappend-0.7.1/zappend/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:50:26.619657 zappend-0.7.1/zappend/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-30 10:50:22.000000 zappend-0.7.1/zappend/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-05-30 10:50:22.000000 zappend-0.7.1/zappend/config/attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7450 2024-05-30 10:50:22.000000 zappend-0.7.1/zappend/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-30 10:50:22.000000 zappend-0.7.1/zappend/config/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-30 10:50:22.000000 zappend-0.7.1/zappend/config/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-05-30 10:50:22.000000 zappend-0.7.1/zappend/config/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28739 2024-05-30 10:50:22.000000 zappend-0.7.1/zappend/config/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-30 10:50:22.000000 zappend-0.7.1/zappend/config/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-05-30 10:50:22.000000 zappend-0.7.1/zappend/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:50:26.623657 zappend-0.7.1/zappend/fsutil/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-30 10:50:22.000000 zappend-0.7.1/zappend/fsutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8092 2024-05-30 10:50:22.000000 zappend-0.7.1/zappend/fsutil/fileobj.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-30 10:50:22.000000 zappend-0.7.1/zappend/fsutil/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8540 2024-05-30 10:50:22.000000 zappend-0.7.1/zappend/fsutil/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-30 10:50:22.000000 zappend-0.7.1/zappend/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14800 2024-05-30 10:50:22.000000 zappend-0.7.1/zappend/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10299 2024-05-30 10:50:22.000000 zappend-0.7.1/zappend/processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-30 10:50:22.000000 zappend-0.7.1/zappend/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-30 10:50:22.000000 zappend-0.7.1/zappend/rollbackstore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:50:26.623657 zappend-0.7.1/zappend/slice/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-30 10:50:22.000000 zappend-0.7.1/zappend/slice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-05-30 10:50:22.000000 zappend-0.7.1/zappend/slice/callable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-30 10:50:22.000000 zappend-0.7.1/zappend/slice/cm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-05-30 10:50:22.000000 zappend-0.7.1/zappend/slice/source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:50:26.623657 zappend-0.7.1/zappend/slice/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-30 10:50:22.000000 zappend-0.7.1/zappend/slice/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-30 10:50:22.000000 zappend-0.7.1/zappend/slice/sources/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-30 10:50:22.000000 zappend-0.7.1/zappend/slice/sources/persistent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-30 10:50:22.000000 zappend-0.7.1/zappend/slice/sources/temporary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-30 10:50:22.000000 zappend-0.7.1/zappend/tailoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:50:26.623657 zappend-0.7.1/zappend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-30 10:50:26.000000 zappend-0.7.1/zappend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-30 10:50:26.000000 zappend-0.7.1/zappend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 10:50:26.000000 zappend-0.7.1/zappend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-30 10:50:26.000000 zappend-0.7.1/zappend.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-30 10:50:26.000000 zappend-0.7.1/zappend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 10:50:26.000000 zappend-0.7.1/zappend.egg-info/top_level.txt
```

### Comparing `zappend-0.7.0/LICENSE` & `zappend-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zappend-0.7.0/PKG-INFO` & `zappend-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: zappend
-Version: 0.7.0
+Version: 0.7.1
 Summary: Tool for robustly creating and updating Zarr datacubes from smaller slices
-Home-page: https://github.com/bcdev/zappend
-Author: Norman Fomferra
+Author-email: Norman Fomferra <norman.fomferra@brockmann-consult.de>
 License: MIT
 Project-URL: Documentation, https://bcdev.github.io/zappend/
 Project-URL: Issues, https://github.com/bcdev/zappend/issues
 Project-URL: Changelog, https://github.com/bcdev/zappend/blob/main/CHANGES.md
+Project-URL: Repository, https://github.com/bcdev/zappend
 Keywords: analysis ready data,data science,datacube,xarray,zarr
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: dask
 Requires-Dist: fsspec
```

### Comparing `zappend-0.7.0/README.md` & `zappend-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `zappend-0.7.0/tests/test_api.py` & `zappend-0.7.1/tests/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,15 +173,16 @@
 
         @contextlib.contextmanager
         def drop_tsm(slice_ds: xr.Dataset) -> xr.Dataset:
             yield slice_ds.drop_vars(["tsm"])
 
         target_dir = "memory://target.zarr"
         slices = [make_test_dataset(index=3 * i) for i in range(3)]
-        zappend(slices, target_dir=target_dir, slice_source=drop_tsm)
+        count = zappend(slices, target_dir=target_dir, slice_source=drop_tsm)
+        self.assertEqual(3, count)
         ds = xr.open_zarr(target_dir)
         self.assertEqual({"time": 9, "y": 50, "x": 100}, ds.sizes)
         self.assertEqual({"chl"}, set(ds.data_vars))
         self.assertEqual({"time", "y", "x"}, set(ds.coords))
         self.assertEqual(
             {
                 "Conventions": "CF-1.8",
@@ -192,15 +193,16 @@
 
     def test_some_slices_with_slice_source_func(self):
         def drop_tsm(slice_ds: xr.Dataset) -> xr.Dataset:
             return slice_ds.drop_vars(["tsm"])
 
         target_dir = "memory://target.zarr"
         slices = [make_test_dataset(index=3 * i) for i in range(3)]
-        zappend(slices, target_dir=target_dir, slice_source=drop_tsm)
+        count = zappend(slices, target_dir=target_dir, slice_source=drop_tsm)
+        self.assertEqual(3, count)
         ds = xr.open_zarr(target_dir)
         self.assertEqual({"time": 9, "y": 50, "x": 100}, ds.sizes)
         self.assertEqual({"chl"}, set(ds.data_vars))
         self.assertEqual({"time", "y", "x"}, set(ds.coords))
         self.assertEqual(
             {
                 "Conventions": "CF-1.8",
@@ -214,15 +216,16 @@
         def crop_ds(slice_ds: xr.Dataset) -> xr.Dataset:
             w = slice_ds.x.size
             h = slice_ds.y.size
             return slice_ds.isel(x=slice(5, w - 5), y=slice(5, h - 5))
 
         target_dir = "memory://target.zarr"
         slices = [make_test_dataset(index=3 * i) for i in range(3)]
-        zappend(slices, target_dir=target_dir, slice_source=crop_ds)
+        count = zappend(slices, target_dir=target_dir, slice_source=crop_ds)
+        self.assertEqual(3, count)
         ds = xr.open_zarr(target_dir)
         self.assertEqual({"time": 9, "y": 40, "x": 90}, ds.sizes)
         self.assertEqual({"chl", "tsm"}, set(ds.data_vars))
         self.assertEqual({"time", "y", "x"}, set(ds.coords))
         self.assertEqual((90,), ds.x.encoding.get("chunks"))
         self.assertEqual((40,), ds.y.encoding.get("chunks"))
         self.assertEqual((3,), ds.time.encoding.get("chunks"))
@@ -254,31 +257,33 @@
                     "chunks": [None, 25, 50],
                 }
             },
         }
 
         target_dir = "memory://target.zarr"
         slices = [make_test_dataset(index=3 * i) for i in range(3)]
-        zappend(
+        count = zappend(
             slices, target_dir=target_dir, slice_source=crop_ds, variables=variables
         )
+        self.assertEqual(3, count)
         ds = xr.open_zarr(target_dir)
         self.assertEqual({"time": 9, "y": 40, "x": 90}, ds.sizes)
         self.assertEqual({"chl", "tsm"}, set(ds.data_vars))
         self.assertEqual({"time", "y", "x"}, set(ds.coords))
         self.assertEqual((90,), ds.x.encoding.get("chunks"))
         self.assertEqual((40,), ds.y.encoding.get("chunks"))
         self.assertEqual((3,), ds.time.encoding.get("chunks"))
         self.assertEqual((1, 40, 90), ds.chl.encoding.get("chunks"))
         self.assertEqual((3, 25, 50), ds.tsm.encoding.get("chunks"))
 
     def test_some_slices_with_inc_append_step(self):
         target_dir = "memory://target.zarr"
         slices = [make_test_dataset(index=i, shape=(1, 50, 100)) for i in range(3)]
-        zappend(slices, target_dir=target_dir, append_step="1D")
+        count = zappend(slices, target_dir=target_dir, append_step="1D")
+        self.assertEqual(3, count)
         ds = xr.open_zarr(target_dir)
         np.testing.assert_array_equal(
             ds.time.values,
             np.array(["2024-01-01", "2024-01-02", "2024-01-03"], dtype=np.datetime64),
         )
         self.assertEqual(
             {
@@ -289,15 +294,16 @@
         )
 
     def test_some_slices_with_dec_append_step(self):
         target_dir = "memory://target.zarr"
         slices = [
             make_test_dataset(index=i, shape=(1, 50, 100)) for i in reversed(range(3))
         ]
-        zappend(slices, target_dir=target_dir, append_step="-1D")
+        count = zappend(slices, target_dir=target_dir, append_step="-1D")
+        self.assertEqual(3, count)
         ds = xr.open_zarr(target_dir)
         np.testing.assert_array_equal(
             ds.time.values,
             np.array(["2024-01-03", "2024-01-02", "2024-01-01"], dtype=np.datetime64),
         )
         self.assertEqual(
             {
@@ -412,24 +418,25 @@
             ),
         ):
             zappend(slices, target_dir=target_dir, append_step=append_step)
 
     def test_dynamic_attrs_with_one_slice(self):
         target_dir = "memory://target.zarr"
         slices = [make_test_dataset()]
-        zappend(
+        count = zappend(
             slices,
             target_dir=target_dir,
             permit_eval=True,
             attrs={
                 "title": "HROC Ocean Colour Monthly Composite",
                 "time_coverage_start": "{{ ds.time[0] }}",
                 "time_coverage_end": "{{ ds.time[-1] }}",
             },
         )
+        self.assertEqual(1, count)
         ds = xr.open_zarr(target_dir)
         self.assertEqual(
             {
                 "Conventions": "CF-1.8",
                 "title": "HROC Ocean Colour Monthly Composite",
                 "time_coverage_start": np.datetime_as_string(ds.time[0], unit="s"),
                 "time_coverage_end": np.datetime_as_string(ds.time[-1], unit="s"),
```

### Comparing `zappend-0.7.0/tests/test_cli.py` & `zappend-0.7.1/tests/test_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,15 +62,15 @@
                 "--target",
                 "memory://target.zarr",
                 "memory://slice-1.zarr",
                 "memory://slice-2.zarr",
                 "memory://slice-3.zarr",
             ],
         )
-        self.assertEqual("", result.output)
+        self.assertEqual("3 slice datasets processed.\n", result.output)
         self.assertEqual(0, result.exit_code)
         self.assertTrue(FileObj("memory://target.zarr").exists())
 
     def test_some_slices_and_target_dry_run(self):
         make_test_dataset(uri="memory://slice-1.zarr")
         make_test_dataset(uri="memory://slice-2.zarr")
         make_test_dataset(uri="memory://slice-3.zarr")
@@ -84,15 +84,15 @@
                 "memory://target.zarr",
                 "--dry-run",
                 "memory://slice-1.zarr",
                 "memory://slice-2.zarr",
                 "memory://slice-3.zarr",
             ],
         )
-        self.assertEqual("", result.output)
+        self.assertEqual("3 slice datasets processed.\n", result.output)
         self.assertEqual(0, result.exit_code)
         self.assertFalse(FileObj("memory://target.zarr").exists())
 
     def test_some_slices_and_no_target(self):
         make_test_dataset(uri="memory://slice-1.zarr")
         make_test_dataset(uri="memory://slice-2.zarr")
         make_test_dataset(uri="memory://slice-3.zarr")
```

### Comparing `zappend-0.7.0/tests/test_context.py` & `zappend-0.7.1/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `zappend-0.7.0/tests/test_log.py` & `zappend-0.7.1/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `zappend-0.7.0/tests/test_metadata.py` & `zappend-0.7.1/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `zappend-0.7.0/tests/test_processor.py` & `zappend-0.7.1/tests/test_processor.py`

 * *Files identical despite different names*

### Comparing `zappend-0.7.0/tests/test_profiler.py` & `zappend-0.7.1/tests/test_profiler.py`

 * *Files identical despite different names*

### Comparing `zappend-0.7.0/tests/test_rollbackstore.py` & `zappend-0.7.1/tests/test_rollbackstore.py`

 * *Files identical despite different names*

### Comparing `zappend-0.7.0/tests/test_tailoring.py` & `zappend-0.7.1/tests/test_tailoring.py`

 * *Files identical despite different names*

### Comparing `zappend-0.7.0/tests/test_xrencoding.py` & `zappend-0.7.1/tests/test_xrencoding.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
         )
 
     # noinspection PyMethodMayBeStatic
     def test_overlapping_chunks_in_data_and_encoding_raises(self):
         self.ds["v"] = self.ds.v.chunk(x=10)
         self.ds.v.encoding.update(chunks=(20,))
         with pytest.raises(
-            NotImplementedError,
+            (NotImplementedError, ValueError),
             match="Specified zarr chunks"
             " encoding\\['chunks'\\]=\\(20,\\)"
             " for variable named 'v'",
         ):
             self.ds.to_zarr(TEST_ZARR)
 
     def test_packing_in_v_attrs_has_wrong_effect(self):
```

### Comparing `zappend-0.7.0/zappend/api.py` & `zappend-0.7.1/zappend/api.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 ]
 
 
 def zappend(
     slices: Iterable[Any],
     config: ConfigLike = None,
     **kwargs: Any,
-):
+) -> int:
     """Robustly create or update a Zarr dataset from dataset slices.
 
     The `zappend` function concatenates the dataset slices from given
     `slices` along a given append dimension, e.g., `"time"` (the default)
     for geospatial satellite observations.
     Each append step is atomic, that is, the append operation is a transaction
     that can be rolled back, in case the append operation fails.
@@ -58,15 +58,20 @@
     If a slice source is configured, a slice item represents the argument(s) passed
     to that slice source. Multiple positional arguments can be passed as `list`,
     multiple keyword arguments as `dict`, and both as a `tuple` of `list` and `dict`.
 
     Args:
         slices: An iterable that yields slice items.
         config: Processor configuration.
-            May be a file path or URI, a `dict`, `None`, or a sequence of
+            Can be a file path or URI, a `dict`, `None`, or a sequence of
             the aforementioned. If a sequence is used, subsequent
             configurations are incremental to the previous ones.
         kwargs: Additional configuration parameters.
             Can be used to pass or override configuration values in *config*.
+
+    Returns:
+        The number of slices processed. The value can be useful if \
+        the number of items in `slices` is unknown.
+
     """
     processor = Processor(config, **kwargs)
-    processor.process_slices(slices)
+    return processor.process_slices(slices)
```

### Comparing `zappend-0.7.0/zappend/cli.py` & `zappend-0.7.1/zappend/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,21 +89,22 @@
         click.echo("No slice datasets given.")
         return
 
     from zappend.api import zappend
 
     # noinspection PyBroadException
     try:
-        zappend(
+        count = zappend(
             slices,
             config=config,
             target_dir=target,
             force_new=force_new,
             dry_run=dry_run,
         )
+        click.echo(f"{count} slice dataset{'s' if count != 1 else ''} processed.")
     except BaseException as e:
         if traceback:
             import traceback as tb
 
             tb.print_exc(file=sys.stderr)
         raise click.ClickException(f"{e}") from e
```

### Comparing `zappend-0.7.0/zappend/config/__init__.py` & `zappend-0.7.1/zappend/config/__init__.py`

 * *Files identical despite different names*

### Comparing `zappend-0.7.0/zappend/config/attrs.py` & `zappend-0.7.1/zappend/config/attrs.py`

 * *Files identical despite different names*

### Comparing `zappend-0.7.0/zappend/config/config.py` & `zappend-0.7.1/zappend/config/config.py`

 * *Files identical despite different names*

### Comparing `zappend-0.7.0/zappend/config/markdown.py` & `zappend-0.7.1/zappend/config/markdown.py`

 * *Files identical despite different names*

### Comparing `zappend-0.7.0/zappend/config/normalize.py` & `zappend-0.7.1/zappend/config/normalize.py`

 * *Files identical despite different names*

### Comparing `zappend-0.7.0/zappend/config/schema.py` & `zappend-0.7.1/zappend/config/schema.py`

 * *Files identical despite different names*

### Comparing `zappend-0.7.0/zappend/config/validate.py` & `zappend-0.7.1/zappend/config/validate.py`

 * *Files identical despite different names*

### Comparing `zappend-0.7.0/zappend/context.py` & `zappend-0.7.1/zappend/context.py`

 * *Files identical despite different names*

### Comparing `zappend-0.7.0/zappend/fsutil/fileobj.py` & `zappend-0.7.1/zappend/fsutil/fileobj.py`

 * *Files identical despite different names*

### Comparing `zappend-0.7.0/zappend/fsutil/path.py` & `zappend-0.7.1/zappend/fsutil/path.py`

 * *Files identical despite different names*

### Comparing `zappend-0.7.0/zappend/fsutil/transaction.py` & `zappend-0.7.1/zappend/fsutil/transaction.py`

 * *Files identical despite different names*

### Comparing `zappend-0.7.0/zappend/log.py` & `zappend-0.7.1/zappend/log.py`

 * *Files identical despite different names*

### Comparing `zappend-0.7.0/zappend/metadata.py` & `zappend-0.7.1/zappend/metadata.py`

 * *Files identical despite different names*

### Comparing `zappend-0.7.0/zappend/processor.py` & `zappend-0.7.1/zappend/processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,24 +54,29 @@
                 f"Setting 'force_new' is enabled. This will"
                 f" permanently delete existing targets (no rollback)."
             )
             delete_target_permanently(_config)
         self._config = _config
         self._profiler = Profiler(_config.profiling)
 
-    def process_slices(self, slices: Iterable[SliceItem]):
+    def process_slices(self, slices: Iterable[SliceItem]) -> int:
         """Process the given `slices`.
         Passes each slice in `slices` to the `process_slice()` method.
 
         Args:
             slices: Iterable of slice items.
+        Returns:
+            The number of slices processed.
         """
+        slice_index = 0
         with self._profiler:
-            for slice_index, slice_item in enumerate(slices):
+            for slice_item in slices:
                 self.process_slice(slice_item, slice_index=slice_index)
+                slice_index += 1
+        return slice_index
 
     def process_slice(self, slice_item: SliceItem, slice_index: int = 0):
         """Process a single slice item *slice_item*.
 
         If there is no target yet, just config and slice:
 
         * create target metadata from configuration and slice dataset
```

### Comparing `zappend-0.7.0/zappend/profiler.py` & `zappend-0.7.1/zappend/profiler.py`

 * *Files identical despite different names*

### Comparing `zappend-0.7.0/zappend/rollbackstore.py` & `zappend-0.7.1/zappend/rollbackstore.py`

 * *Files identical despite different names*

### Comparing `zappend-0.7.0/zappend/slice/callable.py` & `zappend-0.7.1/zappend/slice/callable.py`

 * *Files identical despite different names*

### Comparing `zappend-0.7.0/zappend/slice/cm.py` & `zappend-0.7.1/zappend/slice/cm.py`

 * *Files identical despite different names*

### Comparing `zappend-0.7.0/zappend/slice/source.py` & `zappend-0.7.1/zappend/slice/source.py`

 * *Files identical despite different names*

### Comparing `zappend-0.7.0/zappend/slice/sources/memory.py` & `zappend-0.7.1/zappend/slice/sources/memory.py`

 * *Files identical despite different names*

### Comparing `zappend-0.7.0/zappend/slice/sources/persistent.py` & `zappend-0.7.1/zappend/slice/sources/persistent.py`

 * *Files identical despite different names*

### Comparing `zappend-0.7.0/zappend/slice/sources/temporary.py` & `zappend-0.7.1/zappend/slice/sources/temporary.py`

 * *Files identical despite different names*

### Comparing `zappend-0.7.0/zappend/tailoring.py` & `zappend-0.7.1/zappend/tailoring.py`

 * *Files identical despite different names*

### Comparing `zappend-0.7.0/zappend.egg-info/PKG-INFO` & `zappend-0.7.1/zappend.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: zappend
-Version: 0.7.0
+Version: 0.7.1
 Summary: Tool for robustly creating and updating Zarr datacubes from smaller slices
-Home-page: https://github.com/bcdev/zappend
-Author: Norman Fomferra
+Author-email: Norman Fomferra <norman.fomferra@brockmann-consult.de>
 License: MIT
 Project-URL: Documentation, https://bcdev.github.io/zappend/
 Project-URL: Issues, https://github.com/bcdev/zappend/issues
 Project-URL: Changelog, https://github.com/bcdev/zappend/blob/main/CHANGES.md
+Project-URL: Repository, https://github.com/bcdev/zappend
 Keywords: analysis ready data,data science,datacube,xarray,zarr
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: dask
 Requires-Dist: fsspec
```

### Comparing `zappend-0.7.0/zappend.egg-info/SOURCES.txt` & `zappend-0.7.1/zappend.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 LICENSE
 README.md
 pyproject.toml
-requirements-dev.txt
-requirements-doc.txt
-requirements.txt
-setup.cfg
 tests/test_api.py
 tests/test_cli.py
 tests/test_context.py
 tests/test_log.py
 tests/test_metadata.py
 tests/test_processor.py
 tests/test_profiler.py
```

