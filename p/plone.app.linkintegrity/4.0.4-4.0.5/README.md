# Comparing `tmp/plone_app_linkintegrity-4.0.4.tar.gz` & `tmp/plone_app_linkintegrity-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone_app_linkintegrity-4.0.4.tar", last modified: Mon May  6 12:50:20 2024, max compression
+gzip compressed data, was "plone_app_linkintegrity-4.0.5.tar", last modified: Thu May 30 18:33:16 2024, max compression
```

## Comparing `plone_app_linkintegrity-4.0.4.tar` & `plone_app_linkintegrity-4.0.5.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:50:20.053295 plone_app_linkintegrity-4.0.4/
--rw-r--r--   0 maurits    (501) staff       (20)    19202 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      150 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    25020 2024-05-06 12:50:20.052895 plone_app_linkintegrity-4.0.4/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     4032 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:50:20.038930 plone_app_linkintegrity-4.0.4/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      685 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:50:20.039252 plone_app_linkintegrity-4.0.4/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:50:20.042878 plone_app_linkintegrity-4.0.4/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:50:20.045896 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:50:20.048072 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      498 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     4158 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/browser/delete_confirmation_info.pt
--rw-r--r--   0 maurits    (501) staff       (20)     6854 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/browser/info.py
--rw-r--r--   0 maurits    (501) staff       (20)     1581 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/browser/update.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2521 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/browser/update.py
--rw-r--r--   0 maurits    (501) staff       (20)     1593 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      599 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/exceptions.py
--rw-r--r--   0 maurits    (501) staff       (20)     6243 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/handlers.py
--rw-r--r--   0 maurits    (501) staff       (20)      174 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     1887 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/parser.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:50:20.034179 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:50:20.048617 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      253 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/profiles/default/ploneapplinkintegrity_default.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1534 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/retriever.py
--rw-r--r--   0 maurits    (501) staff       (20)     2965 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:50:20.051535 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/tests/
--rw-r--r--   0 maurits    (501) staff       (20)      201 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     4324 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/tests/test_circular.py
--rw-r--r--   0 maurits    (501) staff       (20)    17114 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/tests/test_functional.py
--rw-r--r--   0 maurits    (501) staff       (20)     2352 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/tests/test_handlers.py
--rw-r--r--   0 maurits    (501) staff       (20)     2467 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/tests/test_imagescales.py
--rw-r--r--   0 maurits    (501) staff       (20)     1451 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/tests/test_info.py
--rw-r--r--   0 maurits    (501) staff       (20)    11261 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/tests/test_references.py
--rw-r--r--   0 maurits    (501) staff       (20)      167 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/tests/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     2534 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/utils.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-06 12:50:20.052098 plone_app_linkintegrity-4.0.4/plone.app.linkintegrity.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    25020 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone.app.linkintegrity.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1631 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone.app.linkintegrity.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone.app.linkintegrity.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone.app.linkintegrity.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone.app.linkintegrity.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone.app.linkintegrity.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      305 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone.app.linkintegrity.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/plone.app.linkintegrity.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4230 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)       38 2024-05-06 12:50:20.053374 plone_app_linkintegrity-4.0.4/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2222 2024-05-06 12:50:19.000000 plone_app_linkintegrity-4.0.4/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:33:16.284960 plone_app_linkintegrity-4.0.5/
+-rw-r--r--   0 maurits    (501) staff       (20)    19357 2024-05-30 18:33:15.000000 plone_app_linkintegrity-4.0.5/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2024-05-30 18:33:15.000000 plone_app_linkintegrity-4.0.5/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      150 2024-05-30 18:33:15.000000 plone_app_linkintegrity-4.0.5/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    25175 2024-05-30 18:33:16.284236 plone_app_linkintegrity-4.0.5/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     4032 2024-05-30 18:33:15.000000 plone_app_linkintegrity-4.0.5/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:33:16.265287 plone_app_linkintegrity-4.0.5/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2024-05-30 18:33:15.000000 plone_app_linkintegrity-4.0.5/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      685 2024-05-30 18:33:15.000000 plone_app_linkintegrity-4.0.5/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:33:16.265750 plone_app_linkintegrity-4.0.5/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-05-30 18:33:15.000000 plone_app_linkintegrity-4.0.5/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:33:16.270095 plone_app_linkintegrity-4.0.5/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-05-30 18:33:15.000000 plone_app_linkintegrity-4.0.5/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:33:16.274402 plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-30 18:33:15.000000 plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:33:16.277240 plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-30 18:33:15.000000 plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      498 2024-05-30 18:33:15.000000 plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     4158 2024-05-30 18:33:15.000000 plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/browser/delete_confirmation_info.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     6953 2024-05-30 18:33:15.000000 plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/browser/info.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1581 2024-05-30 18:33:15.000000 plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/browser/update.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2521 2024-05-30 18:33:15.000000 plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/browser/update.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1593 2024-05-30 18:33:15.000000 plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      599 2024-05-30 18:33:15.000000 plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/exceptions.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6243 2024-05-30 18:33:15.000000 plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/handlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)      174 2024-05-30 18:33:15.000000 plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1887 2024-05-30 18:33:15.000000 plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/parser.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:33:16.261030 plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:33:16.278216 plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      253 2024-05-30 18:33:15.000000 plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-30 18:33:15.000000 plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/profiles/default/ploneapplinkintegrity_default.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1534 2024-05-30 18:33:15.000000 plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/retriever.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2965 2024-05-30 18:33:15.000000 plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:33:16.282183 plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)      201 2024-05-30 18:33:15.000000 plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4324 2024-05-30 18:33:15.000000 plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/tests/test_circular.py
+-rw-r--r--   0 maurits    (501) staff       (20)    17114 2024-05-30 18:33:15.000000 plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/tests/test_functional.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2352 2024-05-30 18:33:15.000000 plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/tests/test_handlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2467 2024-05-30 18:33:15.000000 plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/tests/test_imagescales.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1451 2024-05-30 18:33:15.000000 plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/tests/test_info.py
+-rw-r--r--   0 maurits    (501) staff       (20)    13079 2024-05-30 18:33:15.000000 plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/tests/test_references.py
+-rw-r--r--   0 maurits    (501) staff       (20)      167 2024-05-30 18:33:15.000000 plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/tests/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2534 2024-05-30 18:33:15.000000 plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/utils.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:33:16.282789 plone_app_linkintegrity-4.0.5/plone.app.linkintegrity.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    25175 2024-05-30 18:33:16.000000 plone_app_linkintegrity-4.0.5/plone.app.linkintegrity.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1631 2024-05-30 18:33:16.000000 plone_app_linkintegrity-4.0.5/plone.app.linkintegrity.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-05-30 18:33:16.000000 plone_app_linkintegrity-4.0.5/plone.app.linkintegrity.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2024-05-30 18:33:16.000000 plone_app_linkintegrity-4.0.5/plone.app.linkintegrity.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2024-05-30 18:33:16.000000 plone_app_linkintegrity-4.0.5/plone.app.linkintegrity.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-05-30 18:33:16.000000 plone_app_linkintegrity-4.0.5/plone.app.linkintegrity.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      305 2024-05-30 18:33:16.000000 plone_app_linkintegrity-4.0.5/plone.app.linkintegrity.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-05-30 18:33:16.000000 plone_app_linkintegrity-4.0.5/plone.app.linkintegrity.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4230 2024-05-30 18:33:15.000000 plone_app_linkintegrity-4.0.5/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2024-05-30 18:33:16.285109 plone_app_linkintegrity-4.0.5/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2222 2024-05-30 18:33:15.000000 plone_app_linkintegrity-4.0.5/setup.py
```

### Comparing `plone_app_linkintegrity-4.0.4/CHANGES.rst` & `plone_app_linkintegrity-4.0.5/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.5 (2024-05-30)
+------------------
+
+Bug fixes:
+
+
+- Fix potential issue calculating breaches with objects sharing the same prefix
+  [pgrunewald] (#97)
+
+
 4.0.4 (2024-05-06)
 ------------------
 
 Bug fixes:
 
 
 - Improve performance for calculating breaches.
```

### Comparing `plone_app_linkintegrity-4.0.4/PKG-INFO` & `plone_app_linkintegrity-4.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.linkintegrity
-Version: 4.0.4
+Version: 4.0.5
 Summary: Manage link integrity in Plone.
 Home-page: https://github.com/plone/plone.app.linkintegrity
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: link integrity plone
 Platform: Any
@@ -165,14 +165,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.5 (2024-05-30)
+------------------
+
+Bug fixes:
+
+
+- Fix potential issue calculating breaches with objects sharing the same prefix
+  [pgrunewald] (#97)
+
+
 4.0.4 (2024-05-06)
 ------------------
 
 Bug fixes:
 
 
 - Improve performance for calculating breaches.
```

### Comparing `plone_app_linkintegrity-4.0.4/README.rst` & `plone_app_linkintegrity-4.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `plone_app_linkintegrity-4.0.4/docs/LICENSE.GPL` & `plone_app_linkintegrity-4.0.5/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone_app_linkintegrity-4.0.4/docs/LICENSE.txt` & `plone_app_linkintegrity-4.0.5/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/browser/delete_confirmation_info.pt` & `plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/browser/delete_confirmation_info.pt`

 * *Files identical despite different names*

### Comparing `plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/browser/info.py` & `plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/browser/info.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,28 +60,30 @@
             obj_path = "/".join(obj.getPhysicalPath())
             path2obj[obj_path] = obj
             path2brains[obj_path] = brains_to_delete = catalog(path={"query": obj_path})
             # add the current items uid and all its children's uids to the
             # list of uids that are ignored
             uids_to_ignore.update([i.UID for i in brains_to_delete])
 
+        excluded_paths = set(path2obj.keys())
+
         # determine breaches
         for obj_path, obj in path2obj.items():
             brains_to_delete = path2brains[obj_path]
             for brain_to_delete in brains_to_delete:
                 try:
                     obj_to_delete = brain_to_delete.getObject()  # noqa
                 except (AttributeError, KeyError):
                     logger.exception(
                         "No object found for %s! Skipping", brain_to_delete
                     )
                     continue
                 # look into potential breach
                 breach = self.check_object(
-                    obj=obj_to_delete, excluded_paths=set(path2obj.keys())
+                    obj=obj_to_delete, excluded_paths=excluded_paths
                 )
                 if breach:
                     for source in breach["sources"]:
                         # Only add the breach if one the sources is not in the
                         # list of items that are to be deleted.
                         if source["uid"] not in uids_to_ignore:
                             results.append(breach)
@@ -130,15 +132,16 @@
         for direct_link in direct_links:
             source_path = direct_link.from_path
             if not source_path:
                 # link is broken
                 continue
             if any(
                 [
-                    source_path.startswith(excluded_path)
+                    source_path == excluded_path
+                    or source_path.startswith(excluded_path + "/")
                     for excluded_path in excluded_paths
                 ]
             ):
                 # source is in excluded_path
                 continue
             source = direct_link.from_object
             if not breaches.get("sources"):
```

### Comparing `plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/browser/update.pt` & `plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/browser/update.pt`

 * *Files identical despite different names*

### Comparing `plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/browser/update.py` & `plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/browser/update.py`

 * *Files identical despite different names*

### Comparing `plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/configure.zcml` & `plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/exceptions.py` & `plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/exceptions.py`

 * *Files identical despite different names*

### Comparing `plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/handlers.py` & `plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/handlers.py`

 * *Files identical despite different names*

### Comparing `plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/parser.py` & `plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/parser.py`

 * *Files identical despite different names*

### Comparing `plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/retriever.py` & `plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/retriever.py`

 * *Files identical despite different names*

### Comparing `plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/testing.py` & `plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/testing.py`

 * *Files identical despite different names*

### Comparing `plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/tests/test_circular.py` & `plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/tests/test_circular.py`

 * *Files identical despite different names*

### Comparing `plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/tests/test_functional.py` & `plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/tests/test_handlers.py` & `plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/tests/test_imagescales.py` & `plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/tests/test_imagescales.py`

 * *Files identical despite different names*

### Comparing `plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/tests/test_info.py` & `plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/tests/test_references.py` & `plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/tests/test_references.py`

 * *Files 5% similar despite different names*

```diff
@@ -274,7 +274,44 @@
 
         doc5_breaches = {r.to_object for r in getOutgoingLinks(doc5)}
         # the order of breaches is non-deterministic
         self.assertEqual({doc1, doc2}, doc5_breaches)
         view = self.portal.restrictedTraverse("@@delete_confirmation_info")
         # deleting the two referenced document results in two reported breaches
         self.assertEqual(len(view.get_breaches([doc1, doc2])), 2)
+
+    def test_if_breaches_under_excluded_paths_are_ignored(self):
+        """Test, if breaches are ignored under certain conditions."""
+        folder_containing_doc4 = self.portal.folder1
+        doc4 = self.portal.folder1.doc4
+        doc1 = self.portal.doc1
+        set_text(doc4, '<a href="doc1">d1</a>')
+        # sanity check: deleting doc1 causes one breach
+        doc4_breaches = {r.to_object for r in getOutgoingLinks(doc4)}
+        self.assertEqual({doc1}, doc4_breaches)
+        view = self.portal.restrictedTraverse("@@delete_confirmation_info")
+        self.assertEqual(len(view.get_breaches([doc1])), 1)
+        # now check for other ways, that should do not produce any breach:
+        # a) we delete the document that links to doc1
+        self.assertEqual(len(view.get_breaches([doc1, doc4])), 0)
+        # b) we delete the folder, containing the document that links to doc1
+        self.assertEqual(len(view.get_breaches([doc1, folder_containing_doc4])), 0)
+
+    def test_if_same_prefix_and_breaches_work(self):
+        """Verify that the same prefix does not lead to acciddental ignored
+        links / breaches.
+        """
+        from plone.app.linkintegrity.testing import create
+
+        doc1 = self.portal.doc1
+        my_page = create(self.portal, "Document", id="my-page", title="My page")
+        my_page2 = create(
+            self.portal,
+            "Document",
+            id="my-page-being-linked",
+            title="My Page Being Linked",
+        )
+        # Create a link, that might be overlooked since both page' ids start
+        # with the same string ("my-page").
+        set_text(doc1, '<a href="my-page-being-linked">.</a>')
+        view = self.portal.restrictedTraverse("@@delete_confirmation_info")
+        self.assertEqual(len(view.get_breaches([my_page, my_page2])), 1)
```

### Comparing `plone_app_linkintegrity-4.0.4/plone/app/linkintegrity/utils.py` & `plone_app_linkintegrity-4.0.5/plone/app/linkintegrity/utils.py`

 * *Files identical despite different names*

### Comparing `plone_app_linkintegrity-4.0.4/plone.app.linkintegrity.egg-info/PKG-INFO` & `plone_app_linkintegrity-4.0.5/plone.app.linkintegrity.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.linkintegrity
-Version: 4.0.4
+Version: 4.0.5
 Summary: Manage link integrity in Plone.
 Home-page: https://github.com/plone/plone.app.linkintegrity
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: link integrity plone
 Platform: Any
@@ -165,14 +165,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.5 (2024-05-30)
+------------------
+
+Bug fixes:
+
+
+- Fix potential issue calculating breaches with objects sharing the same prefix
+  [pgrunewald] (#97)
+
+
 4.0.4 (2024-05-06)
 ------------------
 
 Bug fixes:
 
 
 - Improve performance for calculating breaches.
```

### Comparing `plone_app_linkintegrity-4.0.4/plone.app.linkintegrity.egg-info/SOURCES.txt` & `plone_app_linkintegrity-4.0.5/plone.app.linkintegrity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone_app_linkintegrity-4.0.4/pyproject.toml` & `plone_app_linkintegrity-4.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone_app_linkintegrity-4.0.4/setup.py` & `plone_app_linkintegrity-4.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "4.0.4"
+version = "4.0.5"
 
 setup(
     name="plone.app.linkintegrity",
     version=version,
     description="Manage link integrity in Plone.",
     long_description="\n\n".join(
         [
```

