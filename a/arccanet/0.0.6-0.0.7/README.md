# Comparing `tmp/arccanet-0.0.6.tar.gz` & `tmp/arccanet-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arccanet-0.0.6.tar", last modified: Wed May 22 19:00:07 2024, max compression
+gzip compressed data, was "arccanet-0.0.7.tar", last modified: Thu May 30 00:09:32 2024, max compression
```

## Comparing `arccanet-0.0.6.tar` & `arccanet-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:00:07.376383 arccanet-0.0.6/
--rw-r--r--   0 root         (0) root         (0)      231 2024-05-22 19:00:07.375383 arccanet-0.0.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      437 2024-05-22 19:00:06.000000 arccanet-0.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:00:07.374383 arccanet-0.0.6/arccanet/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 19:00:06.000000 arccanet-0.0.6/arccanet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1690 2024-05-22 19:00:06.000000 arccanet-0.0.6/arccanet/conditionbuilder.py
--rw-rw-rw-   0 root         (0) root         (0)       54 2024-05-22 19:00:06.000000 arccanet-0.0.6/arccanet/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3476 2024-05-22 19:00:06.000000 arccanet-0.0.6/arccanet/general.py
--rw-rw-rw-   0 root         (0) root         (0)      229 2024-05-22 19:00:06.000000 arccanet-0.0.6/arccanet/jwt.py
--rw-rw-rw-   0 root         (0) root         (0)       63 2024-05-22 19:00:06.000000 arccanet-0.0.6/arccanet/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)       81 2024-05-22 19:00:06.000000 arccanet-0.0.6/arccanet/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)       45 2024-05-22 19:00:06.000000 arccanet-0.0.6/arccanet/response.py
--rw-rw-rw-   0 root         (0) root         (0)     3469 2024-05-22 19:00:06.000000 arccanet-0.0.6/arccanet/responsebuilder.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-22 19:00:06.000000 arccanet-0.0.6/arccanet/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)       63 2024-05-22 19:00:06.000000 arccanet-0.0.6/arccanet/test.py
--rw-rw-rw-   0 root         (0) root         (0)      335 2024-05-22 19:00:06.000000 arccanet-0.0.6/arccanet/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:00:07.375383 arccanet-0.0.6/arccanet.egg-info/
--rw-r--r--   0 root         (0) root         (0)      231 2024-05-22 19:00:07.000000 arccanet-0.0.6/arccanet.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      438 2024-05-22 19:00:07.000000 arccanet-0.0.6/arccanet.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 19:00:07.000000 arccanet-0.0.6/arccanet.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       79 2024-05-22 19:00:07.000000 arccanet-0.0.6/arccanet.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-22 19:00:07.000000 arccanet-0.0.6/arccanet.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-22 19:00:07.376383 arccanet-0.0.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      387 2024-05-22 19:00:06.000000 arccanet-0.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 00:09:32.358294 arccanet-0.0.7/
+-rw-r--r--   0 root         (0) root         (0)      231 2024-05-30 00:09:32.358294 arccanet-0.0.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      437 2024-05-30 00:09:31.000000 arccanet-0.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 00:09:32.357294 arccanet-0.0.7/arccanet/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-30 00:09:31.000000 arccanet-0.0.7/arccanet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1690 2024-05-30 00:09:31.000000 arccanet-0.0.7/arccanet/conditionbuilder.py
+-rw-rw-rw-   0 root         (0) root         (0)       54 2024-05-30 00:09:31.000000 arccanet-0.0.7/arccanet/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3416 2024-05-30 00:09:31.000000 arccanet-0.0.7/arccanet/general.py
+-rw-rw-rw-   0 root         (0) root         (0)      229 2024-05-30 00:09:31.000000 arccanet-0.0.7/arccanet/jwt.py
+-rw-rw-rw-   0 root         (0) root         (0)       63 2024-05-30 00:09:31.000000 arccanet-0.0.7/arccanet/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)       81 2024-05-30 00:09:31.000000 arccanet-0.0.7/arccanet/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)       45 2024-05-30 00:09:31.000000 arccanet-0.0.7/arccanet/response.py
+-rw-rw-rw-   0 root         (0) root         (0)     3469 2024-05-30 00:09:31.000000 arccanet-0.0.7/arccanet/responsebuilder.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-30 00:09:31.000000 arccanet-0.0.7/arccanet/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)       63 2024-05-30 00:09:31.000000 arccanet-0.0.7/arccanet/test.py
+-rw-rw-rw-   0 root         (0) root         (0)      335 2024-05-30 00:09:31.000000 arccanet-0.0.7/arccanet/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 00:09:32.358294 arccanet-0.0.7/arccanet.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      231 2024-05-30 00:09:32.000000 arccanet-0.0.7/arccanet.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      438 2024-05-30 00:09:32.000000 arccanet-0.0.7/arccanet.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 00:09:32.000000 arccanet-0.0.7/arccanet.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2024-05-30 00:09:32.000000 arccanet-0.0.7/arccanet.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-30 00:09:32.000000 arccanet-0.0.7/arccanet.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 00:09:32.358294 arccanet-0.0.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      387 2024-05-30 00:09:31.000000 arccanet-0.0.7/setup.py
```

### Comparing `arccanet-0.0.6/arccanet/conditionbuilder.py` & `arccanet-0.0.7/arccanet/conditionbuilder.py`

 * *Files identical despite different names*

### Comparing `arccanet-0.0.6/arccanet/general.py` & `arccanet-0.0.7/arccanet/general.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import copy
 import datetime
 import json
 import os
+
 from django.http import Http404
+
 from .exceptions import ValidationError
 
 
 def get_infra_env():
-    if os.environ.get("ENVIRON") == 'production':
-        return 'production'
-    return 'staging'
+    return os.environ.get("ENVIRON")
 
 
 def get_base_lambda_name():
     return "arccanet-infra-{}-".format(get_infra_env())
 
 
 def parse_json(data):
```

### Comparing `arccanet-0.0.6/arccanet/responsebuilder.py` & `arccanet-0.0.7/arccanet/responsebuilder.py`

 * *Files identical despite different names*

