# Comparing `tmp/linien_common-2.0.3.tar.gz` & `tmp/linien_common-2.0.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linien_common-2.0.3.tar", last modified: Wed May 29 12:09:51 2024, max compression
+gzip compressed data, was "linien_common-2.0.3rc1.tar", last modified: Wed May 29 11:52:15 2024, max compression
```

## Comparing `linien_common-2.0.3.tar` & `linien_common-2.0.3rc1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:09:51.370462 linien_common-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-29 12:09:51.370462 linien_common-2.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:09:51.370462 linien_common-2.0.3/linien_common/
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-29 12:09:39.000000 linien_common-2.0.3/linien_common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9767 2024-05-29 12:09:39.000000 linien_common-2.0.3/linien_common/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-29 12:09:39.000000 linien_common-2.0.3/linien_common/communication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-29 12:09:39.000000 linien_common-2.0.3/linien_common/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-05-29 12:09:39.000000 linien_common-2.0.3/linien_common/influxdb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:09:51.370462 linien_common-2.0.3/linien_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-29 12:09:51.000000 linien_common-2.0.3/linien_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-29 12:09:51.000000 linien_common-2.0.3/linien_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 12:09:51.000000 linien_common-2.0.3/linien_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-29 12:09:51.000000 linien_common-2.0.3/linien_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-29 12:09:51.000000 linien_common-2.0.3/linien_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-29 12:09:39.000000 linien_common-2.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 12:09:51.370462 linien_common-2.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:52:15.894358 linien_common-2.0.3rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-29 11:52:15.894358 linien_common-2.0.3rc1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:52:15.894358 linien_common-2.0.3rc1/linien_common/
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-29 11:52:11.000000 linien_common-2.0.3rc1/linien_common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9767 2024-05-29 11:52:11.000000 linien_common-2.0.3rc1/linien_common/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-29 11:52:11.000000 linien_common-2.0.3rc1/linien_common/communication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-29 11:52:11.000000 linien_common-2.0.3rc1/linien_common/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-05-29 11:52:11.000000 linien_common-2.0.3rc1/linien_common/influxdb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:52:15.894358 linien_common-2.0.3rc1/linien_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-29 11:52:15.000000 linien_common-2.0.3rc1/linien_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-29 11:52:15.000000 linien_common-2.0.3rc1/linien_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 11:52:15.000000 linien_common-2.0.3rc1/linien_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-29 11:52:15.000000 linien_common-2.0.3rc1/linien_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-29 11:52:15.000000 linien_common-2.0.3rc1/linien_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-29 11:52:11.000000 linien_common-2.0.3rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 11:52:15.894358 linien_common-2.0.3rc1/setup.cfg
```

### Comparing `linien_common-2.0.3/PKG-INFO` & `linien_common-2.0.3rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linien-common
-Version: 2.0.3
+Version: 2.0.3rc1
 Summary: Shared components of the Linien spectroscopy lock application.
 Author-email: Benjamin Wiegand <benjamin.wiegand@physik.hu-berlin.de>, Bastian Leykauf <leykauf@physik.hu-berlin.de>, Robert Jördens <rj@quartiq.de>, Christian Freier <christian.freier@gmail.com>, Doron Behar <doron.behar@gmail.com>
 Maintainer-email: Bastian Leykauf <leykauf@physik.hu-berlin.de>
 Project-URL: Homepage, https://github.com/linien-org/linien
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `linien_common-2.0.3/linien_common/__init__.py` & `linien_common-2.0.3rc1/linien_common/__init__.py`

 * *Files identical despite different names*

### Comparing `linien_common-2.0.3/linien_common/common.py` & `linien_common-2.0.3rc1/linien_common/common.py`

 * *Files identical despite different names*

### Comparing `linien_common-2.0.3/linien_common/communication.py` & `linien_common-2.0.3rc1/linien_common/communication.py`

 * *Files identical despite different names*

### Comparing `linien_common-2.0.3/linien_common/config.py` & `linien_common-2.0.3rc1/linien_common/config.py`

 * *Files identical despite different names*

### Comparing `linien_common-2.0.3/linien_common/influxdb.py` & `linien_common-2.0.3rc1/linien_common/influxdb.py`

 * *Files identical despite different names*

### Comparing `linien_common-2.0.3/linien_common.egg-info/PKG-INFO` & `linien_common-2.0.3rc1/linien_common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linien-common
-Version: 2.0.3
+Version: 2.0.3rc1
 Summary: Shared components of the Linien spectroscopy lock application.
 Author-email: Benjamin Wiegand <benjamin.wiegand@physik.hu-berlin.de>, Bastian Leykauf <leykauf@physik.hu-berlin.de>, Robert Jördens <rj@quartiq.de>, Christian Freier <christian.freier@gmail.com>, Doron Behar <doron.behar@gmail.com>
 Maintainer-email: Bastian Leykauf <leykauf@physik.hu-berlin.de>
 Project-URL: Homepage, https://github.com/linien-org/linien
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `linien_common-2.0.3/pyproject.toml` & `linien_common-2.0.3rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "linien-common"
-version = "2.0.3"
+version = "2.0.3rc1"
 authors = [
     { name = "Benjamin Wiegand", email = "benjamin.wiegand@physik.hu-berlin.de" },
     { name = "Bastian Leykauf", email = "leykauf@physik.hu-berlin.de" },
     { name = "Robert Jördens", email = "rj@quartiq.de" },
     { name = "Christian Freier", email = "christian.freier@gmail.com" },
     { name = "Doron Behar", email = "doron.behar@gmail.com" },
 ]
```

