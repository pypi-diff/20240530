# Comparing `tmp/findimports-2.4.0.tar.gz` & `tmp/findimports-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findimports-2.4.0.tar", last modified: Thu Feb  1 11:49:10 2024, max compression
+gzip compressed data, was "findimports-2.5.0.tar", last modified: Thu May 30 13:56:17 2024, max compression
```

## Comparing `findimports-2.4.0.tar` & `findimports-2.5.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2024-02-01 11:49:10.463336 findimports-2.4.0/
--rw-rw-r--   0 mg        (1000) mg        (1000)      104 2022-10-27 08:53:49.000000 findimports-2.4.0/.coveragerc
--rw-r--r--   0 mg        (1000) mg        (1000)       65 2019-06-13 12:22:56.000000 findimports-2.4.0/.gitignore
--rw-rw-r--   0 mg        (1000) mg        (1000)     3841 2024-02-01 11:48:45.000000 findimports-2.4.0/CHANGES.rst
--rw-r--r--   0 mg        (1000) mg        (1000)     1081 2023-11-29 18:09:13.000000 findimports-2.4.0/LICENSE
--rw-r--r--   0 mg        (1000) mg        (1000)      335 2021-05-09 15:55:08.000000 findimports-2.4.0/MANIFEST.in
--rw-rw-r--   0 mg        (1000) mg        (1000)      400 2020-11-30 09:13:58.000000 findimports-2.4.0/Makefile
--rw-rw-r--   0 mg        (1000) mg        (1000)     6140 2024-02-01 11:49:10.463336 findimports-2.4.0/PKG-INFO
--rw-rw-r--   0 mg        (1000) mg        (1000)     1325 2023-11-29 18:05:10.000000 findimports-2.4.0/README.rst
--rw-rw-r--   0 mg        (1000) mg        (1000)      795 2023-10-05 11:44:51.000000 findimports-2.4.0/appveyor.yml
-drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2024-02-01 11:49:10.459336 findimports-2.4.0/findimports.egg-info/
--rw-r--r--   0 mg        (1000) mg        (1000)     6140 2024-02-01 11:49:10.000000 findimports-2.4.0/findimports.egg-info/PKG-INFO
--rw-r--r--   0 mg        (1000) mg        (1000)     1120 2024-02-01 11:49:10.000000 findimports-2.4.0/findimports.egg-info/SOURCES.txt
--rw-r--r--   0 mg        (1000) mg        (1000)        1 2024-02-01 11:49:10.000000 findimports-2.4.0/findimports.egg-info/dependency_links.txt
--rw-r--r--   0 mg        (1000) mg        (1000)       49 2024-02-01 11:49:10.000000 findimports-2.4.0/findimports.egg-info/entry_points.txt
--rw-r--r--   0 mg        (1000) mg        (1000)        1 2019-06-13 13:08:27.000000 findimports-2.4.0/findimports.egg-info/not-zip-safe
--rw-r--r--   0 mg        (1000) mg        (1000)       12 2024-02-01 11:49:10.000000 findimports-2.4.0/findimports.egg-info/top_level.txt
--rwxrwxr-x   0 mg        (1000) mg        (1000)    43195 2024-02-01 11:48:45.000000 findimports-2.4.0/findimports.py
--rw-rw-r--   0 mg        (1000) mg        (1000)     5599 2021-04-19 14:36:29.000000 findimports-2.4.0/release.mk
--rw-r--r--   0 mg        (1000) mg        (1000)      397 2024-02-01 11:49:10.463336 findimports-2.4.0/setup.cfg
--rwxrwxr-x   0 mg        (1000) mg        (1000)     1974 2023-10-05 11:44:51.000000 findimports-2.4.0/setup.py
-drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2024-02-01 11:49:10.463336 findimports-2.4.0/tests/
--rw-rw-r--   0 mg        (1000) mg        (1000)     1111 2024-02-01 11:44:38.000000 findimports-2.4.0/tests/cmdline.txt
--rw-r--r--   0 mg        (1000) mg        (1000)     1153 2019-06-13 12:22:56.000000 findimports-2.4.0/tests/cyclic-imports.txt
--rw-r--r--   0 mg        (1000) mg        (1000)     2757 2019-06-13 12:22:56.000000 findimports-2.4.0/tests/doctests.txt
--rw-r--r--   0 mg        (1000) mg        (1000)      807 2019-06-13 12:22:56.000000 findimports-2.4.0/tests/dotted-names.txt
--rw-r--r--   0 mg        (1000) mg        (1000)      987 2019-06-13 12:22:56.000000 findimports-2.4.0/tests/duplicate-imports.txt
--rw-r--r--   0 mg        (1000) mg        (1000)      315 2019-06-13 12:22:56.000000 findimports-2.4.0/tests/future.txt
--rw-r--r--   0 mg        (1000) mg        (1000)     1268 2019-06-13 12:22:56.000000 findimports-2.4.0/tests/graph-cache.txt
--rw-rw-r--   0 mg        (1000) mg        (1000)      741 2024-02-01 11:44:38.000000 findimports-2.4.0/tests/graphviz.txt
--rw-rw-r--   0 mg        (1000) mg        (1000)      476 2021-12-16 11:42:56.000000 findimports-2.4.0/tests/ignore-stdlib.txt
--rw-r--r--   0 mg        (1000) mg        (1000)     1405 2019-06-13 12:22:56.000000 findimports-2.4.0/tests/import-statements.txt
--rw-rw-r--   0 mg        (1000) mg        (1000)      440 2024-02-01 11:44:38.000000 findimports-2.4.0/tests/imported-names.txt
--rw-rw-r--   0 mg        (1000) mg        (1000)     1434 2024-02-01 11:44:38.000000 findimports-2.4.0/tests/imports.txt
--rw-rw-r--   0 mg        (1000) mg        (1000)      457 2021-05-09 15:52:01.000000 findimports-2.4.0/tests/legacycoding.txt
--rw-r--r--   0 mg        (1000) mg        (1000)      870 2019-06-13 12:22:56.000000 findimports-2.4.0/tests/name-tracking.txt
--rw-r--r--   0 mg        (1000) mg        (1000)      827 2019-06-13 12:22:56.000000 findimports-2.4.0/tests/package-graph.txt
--rw-r--r--   0 mg        (1000) mg        (1000)      593 2019-06-13 12:22:56.000000 findimports-2.4.0/tests/relative-imports.txt
-drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2024-02-01 11:49:10.463336 findimports-2.4.0/tests/sample-tree/
--rw-rw-r--   0 mg        (1000) mg        (1000)      154 2024-02-01 11:44:38.000000 findimports-2.4.0/tests/sample-tree/apple.py
-drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2024-02-01 11:49:10.463336 findimports-2.4.0/tests/sample-tree/box/
--rw-r--r--   0 mg        (1000) mg        (1000)       27 2019-06-13 12:22:56.000000 findimports-2.4.0/tests/sample-tree/box/.#emacsjunk.py
--rw-r--r--   0 mg        (1000) mg        (1000)       17 2019-06-13 12:22:56.000000 findimports-2.4.0/tests/sample-tree/box/__init__.py
--rw-r--r--   0 mg        (1000) mg        (1000)       35 2019-06-13 12:22:56.000000 findimports-2.4.0/tests/sample-tree/box/cat.py
--rw-r--r--   0 mg        (1000) mg        (1000)       21 2019-06-13 12:22:56.000000 findimports-2.4.0/tests/sample-tree/box/yarn.py
--rw-r--r--   0 mg        (1000) mg        (1000)      190 2019-06-13 12:22:56.000000 findimports-2.4.0/tests/sample-tree/orange.py
--rw-r--r--   0 mg        (1000) mg        (1000)       14 2019-06-13 12:22:56.000000 findimports-2.4.0/tests/sample-tree/snake.egg-info
--rw-r--r--   0 mg        (1000) mg        (1000)      171 2019-06-13 12:22:56.000000 findimports-2.4.0/tests/sample-tree/zippedmodules.zip
--rw-r--r--   0 mg        (1000) mg        (1000)     1164 2019-06-13 12:22:56.000000 findimports-2.4.0/tests/scopes.txt
--rw-r--r--   0 mg        (1000) mg        (1000)     1651 2019-10-31 19:53:10.000000 findimports-2.4.0/tests/test-packages.txt
--rw-rw-r--   0 mg        (1000) mg        (1000)      939 2021-12-16 11:42:56.000000 findimports-2.4.0/tests/unknown-modules.txt
--rw-rw-r--   0 mg        (1000) mg        (1000)     1804 2024-02-01 11:44:38.000000 findimports-2.4.0/tests/unused-names.txt
--rw-rw-r--   0 mg        (1000) mg        (1000)      362 2021-05-09 15:52:01.000000 findimports-2.4.0/tests/utf8-bom.txt
--rw-r--r--   0 mg        (1000) mg        (1000)      434 2019-06-13 12:22:56.000000 findimports-2.4.0/tests/zipfiles.txt
--rw-rw-r--   0 mg        (1000) mg        (1000)     3788 2021-05-17 11:25:11.000000 findimports-2.4.0/tests.py
--rwxr-xr-x   0 mg        (1000) mg        (1000)     2943 2020-12-06 17:18:19.000000 findimports-2.4.0/testsuite.py
--rw-rw-r--   0 mg        (1000) mg        (1000)      783 2023-10-05 11:44:51.000000 findimports-2.4.0/tox.ini
+drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2024-05-30 13:56:17.557944 findimports-2.5.0/
+-rw-rw-r--   0 mg        (1000) mg        (1000)      104 2022-10-27 08:53:49.000000 findimports-2.5.0/.coveragerc
+-rw-r--r--   0 mg        (1000) mg        (1000)       65 2019-06-13 12:22:56.000000 findimports-2.5.0/.gitignore
+-rw-rw-r--   0 mg        (1000) mg        (1000)     4223 2024-05-30 13:55:36.000000 findimports-2.5.0/CHANGES.rst
+-rw-r--r--   0 mg        (1000) mg        (1000)     1081 2023-11-29 18:09:13.000000 findimports-2.5.0/LICENSE
+-rw-r--r--   0 mg        (1000) mg        (1000)      335 2021-05-09 15:55:08.000000 findimports-2.5.0/MANIFEST.in
+-rw-rw-r--   0 mg        (1000) mg        (1000)      400 2020-11-30 09:13:58.000000 findimports-2.5.0/Makefile
+-rw-rw-r--   0 mg        (1000) mg        (1000)     6522 2024-05-30 13:56:17.557944 findimports-2.5.0/PKG-INFO
+-rw-rw-r--   0 mg        (1000) mg        (1000)     1325 2023-11-29 18:05:10.000000 findimports-2.5.0/README.rst
+-rw-rw-r--   0 mg        (1000) mg        (1000)      795 2023-10-05 11:44:51.000000 findimports-2.5.0/appveyor.yml
+drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2024-05-30 13:56:17.553944 findimports-2.5.0/findimports.egg-info/
+-rw-r--r--   0 mg        (1000) mg        (1000)     6522 2024-05-30 13:56:17.000000 findimports-2.5.0/findimports.egg-info/PKG-INFO
+-rw-r--r--   0 mg        (1000) mg        (1000)     1120 2024-05-30 13:56:17.000000 findimports-2.5.0/findimports.egg-info/SOURCES.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)        1 2024-05-30 13:56:17.000000 findimports-2.5.0/findimports.egg-info/dependency_links.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)       49 2024-05-30 13:56:17.000000 findimports-2.5.0/findimports.egg-info/entry_points.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)        1 2019-06-13 13:08:27.000000 findimports-2.5.0/findimports.egg-info/not-zip-safe
+-rw-r--r--   0 mg        (1000) mg        (1000)       12 2024-05-30 13:56:17.000000 findimports-2.5.0/findimports.egg-info/top_level.txt
+-rwxrwxr-x   0 mg        (1000) mg        (1000)    43511 2024-05-30 13:55:36.000000 findimports-2.5.0/findimports.py
+-rw-rw-r--   0 mg        (1000) mg        (1000)     5599 2021-04-19 14:36:29.000000 findimports-2.5.0/release.mk
+-rw-r--r--   0 mg        (1000) mg        (1000)      397 2024-05-30 13:56:17.558944 findimports-2.5.0/setup.cfg
+-rwxrwxr-x   0 mg        (1000) mg        (1000)     1974 2023-10-05 11:44:51.000000 findimports-2.5.0/setup.py
+drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2024-05-30 13:56:17.556944 findimports-2.5.0/tests/
+-rw-rw-r--   0 mg        (1000) mg        (1000)     1111 2024-02-01 11:44:38.000000 findimports-2.5.0/tests/cmdline.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)     1153 2019-06-13 12:22:56.000000 findimports-2.5.0/tests/cyclic-imports.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)     2757 2019-06-13 12:22:56.000000 findimports-2.5.0/tests/doctests.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)      807 2019-06-13 12:22:56.000000 findimports-2.5.0/tests/dotted-names.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)      987 2019-06-13 12:22:56.000000 findimports-2.5.0/tests/duplicate-imports.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)      315 2019-06-13 12:22:56.000000 findimports-2.5.0/tests/future.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)     1268 2019-06-13 12:22:56.000000 findimports-2.5.0/tests/graph-cache.txt
+-rw-rw-r--   0 mg        (1000) mg        (1000)      852 2024-05-29 07:07:58.000000 findimports-2.5.0/tests/graphviz.txt
+-rw-rw-r--   0 mg        (1000) mg        (1000)      476 2021-12-16 11:42:56.000000 findimports-2.5.0/tests/ignore-stdlib.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)     1405 2019-06-13 12:22:56.000000 findimports-2.5.0/tests/import-statements.txt
+-rw-rw-r--   0 mg        (1000) mg        (1000)      440 2024-02-01 11:44:38.000000 findimports-2.5.0/tests/imported-names.txt
+-rw-rw-r--   0 mg        (1000) mg        (1000)     1434 2024-02-01 11:44:38.000000 findimports-2.5.0/tests/imports.txt
+-rw-rw-r--   0 mg        (1000) mg        (1000)      457 2021-05-09 15:52:01.000000 findimports-2.5.0/tests/legacycoding.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)      870 2019-06-13 12:22:56.000000 findimports-2.5.0/tests/name-tracking.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)      827 2019-06-13 12:22:56.000000 findimports-2.5.0/tests/package-graph.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)      593 2019-06-13 12:22:56.000000 findimports-2.5.0/tests/relative-imports.txt
+drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2024-05-30 13:56:17.557944 findimports-2.5.0/tests/sample-tree/
+-rw-rw-r--   0 mg        (1000) mg        (1000)      154 2024-02-01 11:44:38.000000 findimports-2.5.0/tests/sample-tree/apple.py
+drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2024-05-30 13:56:17.557944 findimports-2.5.0/tests/sample-tree/box/
+-rw-r--r--   0 mg        (1000) mg        (1000)       27 2019-06-13 12:22:56.000000 findimports-2.5.0/tests/sample-tree/box/.#emacsjunk.py
+-rw-r--r--   0 mg        (1000) mg        (1000)       17 2019-06-13 12:22:56.000000 findimports-2.5.0/tests/sample-tree/box/__init__.py
+-rw-r--r--   0 mg        (1000) mg        (1000)       35 2019-06-13 12:22:56.000000 findimports-2.5.0/tests/sample-tree/box/cat.py
+-rw-r--r--   0 mg        (1000) mg        (1000)       21 2019-06-13 12:22:56.000000 findimports-2.5.0/tests/sample-tree/box/yarn.py
+-rw-r--r--   0 mg        (1000) mg        (1000)      190 2019-06-13 12:22:56.000000 findimports-2.5.0/tests/sample-tree/orange.py
+-rw-r--r--   0 mg        (1000) mg        (1000)       14 2019-06-13 12:22:56.000000 findimports-2.5.0/tests/sample-tree/snake.egg-info
+-rw-r--r--   0 mg        (1000) mg        (1000)      171 2019-06-13 12:22:56.000000 findimports-2.5.0/tests/sample-tree/zippedmodules.zip
+-rw-r--r--   0 mg        (1000) mg        (1000)     1164 2019-06-13 12:22:56.000000 findimports-2.5.0/tests/scopes.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)     1651 2019-10-31 19:53:10.000000 findimports-2.5.0/tests/test-packages.txt
+-rw-rw-r--   0 mg        (1000) mg        (1000)      939 2021-12-16 11:42:56.000000 findimports-2.5.0/tests/unknown-modules.txt
+-rw-rw-r--   0 mg        (1000) mg        (1000)     1804 2024-02-01 11:44:38.000000 findimports-2.5.0/tests/unused-names.txt
+-rw-rw-r--   0 mg        (1000) mg        (1000)      362 2021-05-09 15:52:01.000000 findimports-2.5.0/tests/utf8-bom.txt
+-rw-r--r--   0 mg        (1000) mg        (1000)      434 2019-06-13 12:22:56.000000 findimports-2.5.0/tests/zipfiles.txt
+-rw-rw-r--   0 mg        (1000) mg        (1000)     3788 2021-05-17 11:25:11.000000 findimports-2.5.0/tests.py
+-rwxr-xr-x   0 mg        (1000) mg        (1000)     2943 2020-12-06 17:18:19.000000 findimports-2.5.0/testsuite.py
+-rw-rw-r--   0 mg        (1000) mg        (1000)      783 2023-10-05 11:44:51.000000 findimports-2.5.0/tox.ini
```

### Comparing `findimports-2.4.0/CHANGES.rst` & `findimports-2.5.0/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 Changes
 =======
 
 
+2.5.0 (2024-05-30)
+------------------
+
+- Fixed extension module detection that never worked on Python 3.  See `pull
+  request 29 <https://github.com/mgedmin/findimports/pull/29>`_.
+
+- Add ``--attr``/``-A`` to add arbitrary graphviz `graph attributes
+  <https://graphviz.org/docs/graph/>`_ to the output.  See `pull
+  request 30 <https://github.com/mgedmin/findimports/pull/30>`_.
+
+
 2.4.0 (2024-02-01)
 ------------------
 
 - Add support for Python 3.12.
 
 - Change license from GPL to MIT.  See `issue 27
   <https://github.com/mgedmin/findimports/issues/27>`_.
```

### Comparing `findimports-2.4.0/LICENSE` & `findimports-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `findimports-2.4.0/PKG-INFO` & `findimports-2.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findimports
-Version: 2.4.0
+Version: 2.5.0
 Summary: Python module import analysis tool
 Home-page: https://github.com/mgedmin/findimports
 Author: Marius Gedminas
 Author-email: marius@gedmin.as
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -63,14 +63,25 @@
 .. _coverage: https://coveralls.io/r/mgedmin/findimports
 
 
 Changes
 =======
 
 
+2.5.0 (2024-05-30)
+------------------
+
+- Fixed extension module detection that never worked on Python 3.  See `pull
+  request 29 <https://github.com/mgedmin/findimports/pull/29>`_.
+
+- Add ``--attr``/``-A`` to add arbitrary graphviz `graph attributes
+  <https://graphviz.org/docs/graph/>`_ to the output.  See `pull
+  request 30 <https://github.com/mgedmin/findimports/pull/30>`_.
+
+
 2.4.0 (2024-02-01)
 ------------------
 
 - Add support for Python 3.12.
 
 - Change license from GPL to MIT.  See `issue 27
   <https://github.com/mgedmin/findimports/issues/27>`_.
```

### Comparing `findimports-2.4.0/README.rst` & `findimports-2.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `findimports-2.4.0/appveyor.yml` & `findimports-2.5.0/appveyor.yml`

 * *Files identical despite different names*

### Comparing `findimports-2.4.0/findimports.egg-info/PKG-INFO` & `findimports-2.5.0/findimports.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findimports
-Version: 2.4.0
+Version: 2.5.0
 Summary: Python module import analysis tool
 Home-page: https://github.com/mgedmin/findimports
 Author: Marius Gedminas
 Author-email: marius@gedmin.as
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -63,14 +63,25 @@
 .. _coverage: https://coveralls.io/r/mgedmin/findimports
 
 
 Changes
 =======
 
 
+2.5.0 (2024-05-30)
+------------------
+
+- Fixed extension module detection that never worked on Python 3.  See `pull
+  request 29 <https://github.com/mgedmin/findimports/pull/29>`_.
+
+- Add ``--attr``/``-A`` to add arbitrary graphviz `graph attributes
+  <https://graphviz.org/docs/graph/>`_ to the output.  See `pull
+  request 30 <https://github.com/mgedmin/findimports/pull/30>`_.
+
+
 2.4.0 (2024-02-01)
 ------------------
 
 - Add support for Python 3.12.
 
 - Change license from GPL to MIT.  See `issue 27
   <https://github.com/mgedmin/findimports/issues/27>`_.
```

### Comparing `findimports-2.4.0/findimports.egg-info/SOURCES.txt` & `findimports-2.5.0/findimports.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `findimports-2.4.0/findimports.py` & `findimports-2.5.0/findimports.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,17 @@
                         multiple times. Default: ['venv']
   -R PREFIX [PREFIX ...], --rmprefix PREFIX [PREFIX ...]
                         remove PREFIX from displayed node names. This
                         operation is applied last. Names that collapses to
                         nothing are removed.
   -D MAX_DEPTH, --depth MAX_DEPTH
                         import depth in ast tree. Default: no limit
+  -A ATTRIBUTES, --attr ATTRIBUTES
+                        Add dot graph attributes. E.g.
+                        "rankdir=TB"
 
 FindImports requires Python 3.6 or later.
 
 Notes:
 
     findimports processes doctest blocks inside docstrings.
 
@@ -95,20 +98,21 @@
 import ast
 import doctest
 import linecache
 import os
 import pickle
 import re
 import sys
+import sysconfig
 import tokenize
 import zipfile
 from operator import attrgetter
 
 
-__version__ = '2.4.0'
+__version__ = '2.5.0'
 __author__ = 'Marius Gedminas <marius@gedmin.as>'
 __licence__ = 'MIT'
 __url__ = 'https://github.com/mgedmin/findimports'
 
 
 STDLIB_MODNAMES_SET = getattr(sys, 'stdlib_module_names', frozenset([
     # taken from Python 3.10
@@ -555,21 +559,16 @@
 
     def __init__(self):
         self.modules = {}
         self.path = list(sys.path)
         self._module_cache = {}
         self._warned_about = set()
         self._stderr = sys.stderr
-        self._exts = ('.py', '.so', '.dll')
-        if hasattr(sys, '_multiarch'):  # pragma: nocover
-            # Ubuntu 14.04 LTS renames
-            # /usr/lib/python2.7/lib-dynload/datetime.so to
-            # /usr/lib/python2.7/lib-dynload/datetime.x86_64-linux-gnu.so
-            # (https://github.com/mgedmin/findimports/issues/3)
-            self._exts += f".{sys._multiarch}.so"
+        self._exts = ['.py', '.so', '.dll']
+        self._exts.append(sysconfig.get_config_var('EXT_SUFFIX'))
 
     def warn(self, about, message, *args):
         if about in self._warned_about:
             return
         if args:
             message = message % args
         print(message, file=self._stderr)
@@ -958,18 +957,20 @@
                 if not self.all_unused:
                     line = linecache.getline(module.filename, lineno)
                     if '#' in line:
                         # assume there's a comment explaining why it's not used
                         continue
                 print(f"{module.filename}:{lineno}: {name} not used")
 
-    def constructDot(self):
+    def constructDot(self, attributes=()):
         """Produce a dependency graph in dot format."""
         lines = list()
         lines.append("digraph ModuleDependencies {")
+        if attributes:
+            lines.extend(map("  {}".format, attributes))
         lines.append("  node[shape=box];")
         allNames = set()
         nameDict = {}
         for n, module in enumerate(self.listModules()):
             module._dot_name = f"mod{n}"
             nameDict[module.modname] = module._dot_name
             line = f"  {module._dot_name}[label=\"{quote(module.label)}\"];"
@@ -989,17 +990,17 @@
                     lines.append("  {0} -> {1};".format(
                         nameDict[module.modname],
                         nameDict[other]
                     ))
         lines.append("}")
         return '\n'.join(lines)
 
-    def printDot(self):
+    def printDot(self, attributes=()):
         """Print a dependency graph in dot format."""
-        print(self.constructDot())
+        print(self.constructDot(attributes=attributes))
 
 
 def quote(s):
     """Quote a string for graphviz.
 
     This function is probably incomplete.
     """
@@ -1083,14 +1084,17 @@
     options.add_argument('-R', '--rmprefix', metavar="PREFIX", nargs="+",
                          help="remove PREFIX from displayed node names. "
                               "This operation is applied last. "
                               "Names that collapses to nothing are removed.")
     options.add_argument('-D', '--depth', type=int,
                          dest='max_depth',
                          help='import depth in ast tree. Default: no limit')
+    options.add_argument('-A', '--attr', type=str, dest='attributes',
+                         action='append',
+                         help='Add dot graph attributes. E.g. "rankdir=TB"')
     try:
         args = parser.parse_args(args=argv[1:] if argv else None)
         if args.condense_to_packages and args.condense_to_packages_externals:
             parser.error('only one of -p and -pE can be provided')
     except SystemExit as e:
         return e.code
 
@@ -1115,13 +1119,16 @@
     if args.collapse_tests:
         g = g.collapseTests()
     if args.collapse_cycles:
         g = g.collapseCycles()
     if args.rmprefix is not None:
         g = g.removePrefixes(args.rmprefix)
     g.external_dependencies = not args.noext
-    getattr(g, args.action)()
+    kwds = {}
+    if args.action == 'printDot' and args.attributes is not None:
+        kwds['attributes'] = args.attributes
+    getattr(g, args.action)(**kwds)
     return 0
 
 
 if __name__ == '__main__':  # pragma: nocover
     sys.exit(main())
```

### Comparing `findimports-2.4.0/release.mk` & `findimports-2.5.0/release.mk`

 * *Files identical despite different names*

### Comparing `findimports-2.4.0/setup.py` & `findimports-2.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `findimports-2.4.0/tests/cmdline.txt` & `findimports-2.5.0/tests/cmdline.txt`

 * *Files identical despite different names*

### Comparing `findimports-2.4.0/tests/cyclic-imports.txt` & `findimports-2.5.0/tests/cyclic-imports.txt`

 * *Files identical despite different names*

### Comparing `findimports-2.4.0/tests/doctests.txt` & `findimports-2.5.0/tests/doctests.txt`

 * *Files identical despite different names*

### Comparing `findimports-2.4.0/tests/dotted-names.txt` & `findimports-2.5.0/tests/dotted-names.txt`

 * *Files identical despite different names*

### Comparing `findimports-2.4.0/tests/duplicate-imports.txt` & `findimports-2.5.0/tests/duplicate-imports.txt`

 * *Files identical despite different names*

### Comparing `findimports-2.4.0/tests/graph-cache.txt` & `findimports-2.5.0/tests/graph-cache.txt`

 * *Files identical despite different names*

### Comparing `findimports-2.4.0/tests/graphviz.txt` & `findimports-2.5.0/tests/graphviz.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Producing import graphs with graphviz
 =====================================
 
 findimports can produce graph descriptions in the dot language used by
 graphviz
 
     >>> from findimports import main
-    >>> exitcode = main(['findimports', '-d', sample_tree])
+    >>> attributes = ['-A', 'rankdir=TB', '-A', 'label=Graph']
+    >>> exitcode = main(['findimports', '-d', sample_tree] + attributes)
     digraph ModuleDependencies {
+      rankdir=TB
+      label=Graph
       node[shape=box];
       mod0[label="apple"];
       mod1[label="box.__init__"];
       mod2[label="box.cat"];
       mod3[label="box.yarn"];
       mod4[label="orange"];
       node[style=dotted];
```

### Comparing `findimports-2.4.0/tests/import-statements.txt` & `findimports-2.5.0/tests/import-statements.txt`

 * *Files identical despite different names*

### Comparing `findimports-2.4.0/tests/imports.txt` & `findimports-2.5.0/tests/imports.txt`

 * *Files identical despite different names*

### Comparing `findimports-2.4.0/tests/name-tracking.txt` & `findimports-2.5.0/tests/name-tracking.txt`

 * *Files identical despite different names*

### Comparing `findimports-2.4.0/tests/package-graph.txt` & `findimports-2.5.0/tests/package-graph.txt`

 * *Files identical despite different names*

### Comparing `findimports-2.4.0/tests/relative-imports.txt` & `findimports-2.5.0/tests/relative-imports.txt`

 * *Files identical despite different names*

### Comparing `findimports-2.4.0/tests/scopes.txt` & `findimports-2.5.0/tests/scopes.txt`

 * *Files identical despite different names*

### Comparing `findimports-2.4.0/tests/test-packages.txt` & `findimports-2.5.0/tests/test-packages.txt`

 * *Files identical despite different names*

### Comparing `findimports-2.4.0/tests/unknown-modules.txt` & `findimports-2.5.0/tests/unknown-modules.txt`

 * *Files identical despite different names*

### Comparing `findimports-2.4.0/tests/unused-names.txt` & `findimports-2.5.0/tests/unused-names.txt`

 * *Files identical despite different names*

### Comparing `findimports-2.4.0/tests.py` & `findimports-2.5.0/tests.py`

 * *Files identical despite different names*

### Comparing `findimports-2.4.0/testsuite.py` & `findimports-2.5.0/testsuite.py`

 * *Files identical despite different names*

### Comparing `findimports-2.4.0/tox.ini` & `findimports-2.5.0/tox.ini`

 * *Files identical despite different names*

