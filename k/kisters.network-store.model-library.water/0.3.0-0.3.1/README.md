# Comparing `tmp/kisters.network_store.model_library.water-0.3.0.tar.gz` & `tmp/kisters.network_store.model_library.water-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kisters.network_store.model_library.water-0.3.0.tar", last modified: Thu Mar 21 11:13:59 2024, max compression
+gzip compressed data, was "kisters.network_store.model_library.water-0.3.1.tar", last modified: Wed May 29 21:17:13 2024, max compression
```

## Comparing `kisters.network_store.model_library.water-0.3.0.tar` & `kisters.network_store.model_library.water-0.3.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 11:13:59.989477 kisters.network_store.model_library.water-0.3.0/
--rw-rw-rw-   0 root         (0) root         (0)       99 2024-03-21 11:13:52.000000 kisters.network_store.model_library.water-0.3.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1084 2024-03-21 11:13:52.000000 kisters.network_store.model_library.water-0.3.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)       28 2024-03-21 11:13:52.000000 kisters.network_store.model_library.water-0.3.0/AUTHORS.md
--rw-rw-rw-   0 root         (0) root         (0)    26475 2024-03-21 11:13:52.000000 kisters.network_store.model_library.water-0.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1174 2024-03-21 11:13:59.989477 kisters.network_store.model_library.water-0.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      445 2024-03-21 11:13:52.000000 kisters.network_store.model_library.water-0.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 11:13:59.985477 kisters.network_store.model_library.water-0.3.0/kisters/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 11:13:59.985477 kisters.network_store.model_library.water-0.3.0/kisters/network_store/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 11:13:59.985477 kisters.network_store.model_library.water-0.3.0/kisters/network_store/model_library/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 11:13:59.989477 kisters.network_store.model_library.water-0.3.0/kisters/network_store/model_library/water/
--rw-rw-rw-   0 root         (0) root         (0)       75 2024-03-21 11:13:52.000000 kisters.network_store.model_library.water-0.3.0/kisters/network_store/model_library/water/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      795 2024-03-21 11:13:52.000000 kisters.network_store.model_library.water-0.3.0/kisters/network_store/model_library/water/groups.py
--rw-rw-rw-   0 root         (0) root         (0)    15027 2024-03-21 11:13:52.000000 kisters.network_store.model_library.water-0.3.0/kisters/network_store/model_library/water/links.py
--rw-rw-rw-   0 root         (0) root         (0)     5034 2024-03-21 11:13:52.000000 kisters.network_store.model_library.water-0.3.0/kisters/network_store/model_library/water/nodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 11:13:59.988477 kisters.network_store.model_library.water-0.3.0/kisters.network_store.model_library.water.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1174 2024-03-21 11:13:59.000000 kisters.network_store.model_library.water-0.3.0/kisters.network_store.model_library.water.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      771 2024-03-21 11:13:59.000000 kisters.network_store.model_library.water-0.3.0/kisters.network_store.model_library.water.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-21 11:13:59.000000 kisters.network_store.model_library.water-0.3.0/kisters.network_store.model_library.water.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       94 2024-03-21 11:13:59.000000 kisters.network_store.model_library.water-0.3.0/kisters.network_store.model_library.water.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-21 11:13:59.000000 kisters.network_store.model_library.water-0.3.0/kisters.network_store.model_library.water.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       67 2024-03-21 11:13:59.000000 kisters.network_store.model_library.water-0.3.0/kisters.network_store.model_library.water.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-03-21 11:13:59.000000 kisters.network_store.model_library.water-0.3.0/kisters.network_store.model_library.water.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      408 2024-03-21 11:13:59.990477 kisters.network_store.model_library.water-0.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1381 2024-03-21 11:13:52.000000 kisters.network_store.model_library.water-0.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 11:13:59.989477 kisters.network_store.model_library.water-0.3.0/test/
--rw-rw-rw-   0 root         (0) root         (0)    23054 2024-03-21 11:13:52.000000 kisters.network_store.model_library.water-0.3.0/test/test_water_models.py
--rw-rw-rw-   0 root         (0) root         (0)      469 2024-03-21 11:13:52.000000 kisters.network_store.model_library.water-0.3.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 21:17:13.952200 kisters.network_store.model_library.water-0.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-03-24 18:05:56.000000 kisters.network_store.model_library.water-0.3.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1084 2024-05-29 21:13:06.000000 kisters.network_store.model_library.water-0.3.1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)       28 2022-11-29 20:58:24.000000 kisters.network_store.model_library.water-0.3.1/AUTHORS.md
+-rw-rw-rw-   0 root         (0) root         (0)    26475 2022-11-29 20:58:24.000000 kisters.network_store.model_library.water-0.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1174 2024-05-29 21:17:13.952200 kisters.network_store.model_library.water-0.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      445 2023-03-24 17:53:35.000000 kisters.network_store.model_library.water-0.3.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 21:17:13.948200 kisters.network_store.model_library.water-0.3.1/kisters/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 21:17:13.948200 kisters.network_store.model_library.water-0.3.1/kisters/network_store/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 21:17:13.948200 kisters.network_store.model_library.water-0.3.1/kisters/network_store/model_library/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 21:17:13.951200 kisters.network_store.model_library.water-0.3.1/kisters/network_store/model_library/water/
+-rw-rw-rw-   0 root         (0) root         (0)       75 2022-11-29 20:58:24.000000 kisters.network_store.model_library.water-0.3.1/kisters/network_store/model_library/water/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      795 2024-05-29 21:13:06.000000 kisters.network_store.model_library.water-0.3.1/kisters/network_store/model_library/water/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)    15027 2024-05-29 21:13:06.000000 kisters.network_store.model_library.water-0.3.1/kisters/network_store/model_library/water/links.py
+-rw-rw-rw-   0 root         (0) root         (0)     8866 2024-05-29 21:13:06.000000 kisters.network_store.model_library.water-0.3.1/kisters/network_store/model_library/water/nodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 21:17:13.951200 kisters.network_store.model_library.water-0.3.1/kisters.network_store.model_library.water.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1174 2024-05-29 21:17:13.000000 kisters.network_store.model_library.water-0.3.1/kisters.network_store.model_library.water.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      771 2024-05-29 21:17:13.000000 kisters.network_store.model_library.water-0.3.1/kisters.network_store.model_library.water.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 21:17:13.000000 kisters.network_store.model_library.water-0.3.1/kisters.network_store.model_library.water.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       94 2024-05-29 21:17:13.000000 kisters.network_store.model_library.water-0.3.1/kisters.network_store.model_library.water.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 21:17:13.000000 kisters.network_store.model_library.water-0.3.1/kisters.network_store.model_library.water.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       67 2024-05-29 21:17:13.000000 kisters.network_store.model_library.water-0.3.1/kisters.network_store.model_library.water.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-29 21:17:13.000000 kisters.network_store.model_library.water-0.3.1/kisters.network_store.model_library.water.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      408 2024-05-29 21:17:13.953200 kisters.network_store.model_library.water-0.3.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1381 2024-05-29 21:13:06.000000 kisters.network_store.model_library.water-0.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 21:17:13.952200 kisters.network_store.model_library.water-0.3.1/test/
+-rw-rw-rw-   0 root         (0) root         (0)    23054 2024-05-29 21:13:06.000000 kisters.network_store.model_library.water-0.3.1/test/test_water_models.py
+-rw-rw-rw-   0 root         (0) root         (0)      469 2024-05-29 21:13:06.000000 kisters.network_store.model_library.water-0.3.1/tox.ini
```

### Comparing `kisters.network_store.model_library.water-0.3.0/.gitlab-ci.yml` & `kisters.network_store.model_library.water-0.3.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `kisters.network_store.model_library.water-0.3.0/LICENSE` & `kisters.network_store.model_library.water-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kisters.network_store.model_library.water-0.3.0/PKG-INFO` & `kisters.network_store.model_library.water-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kisters.network_store.model_library.water
-Version: 0.3.0
+Version: 0.3.1
 Summary: Model library for the Kisters Network Store ecosystem
 Home-page: https://gitlab.com/kisters/network-store/model-library-water
 Author: Jesse VanderWees
 Author-email: jesse.vanderwees@kisters-bv.nl
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `kisters.network_store.model_library.water-0.3.0/kisters/network_store/model_library/water/groups.py` & `kisters.network_store.model_library.water-0.3.1/kisters/network_store/model_library/water/groups.py`

 * *Files identical despite different names*

### Comparing `kisters.network_store.model_library.water-0.3.0/kisters/network_store/model_library/water/links.py` & `kisters.network_store.model_library.water-0.3.1/kisters/network_store/model_library/water/links.py`

 * *Files identical despite different names*

### Comparing `kisters.network_store.model_library.water-0.3.0/kisters.network_store.model_library.water.egg-info/PKG-INFO` & `kisters.network_store.model_library.water-0.3.1/kisters.network_store.model_library.water.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kisters.network-store.model-library.water
-Version: 0.3.0
+Version: 0.3.1
 Summary: Model library for the Kisters Network Store ecosystem
 Home-page: https://gitlab.com/kisters/network-store/model-library-water
 Author: Jesse VanderWees
 Author-email: jesse.vanderwees@kisters-bv.nl
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `kisters.network_store.model_library.water-0.3.0/kisters.network_store.model_library.water.egg-info/SOURCES.txt` & `kisters.network_store.model_library.water-0.3.1/kisters.network_store.model_library.water.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kisters.network_store.model_library.water-0.3.0/setup.py` & `kisters.network_store.model_library.water-0.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     author_email="jesse.vanderwees@kisters-bv.nl",
     description="Model library for the Kisters Network Store ecosystem",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/kisters/network-store/model-library-water",
     packages=find_namespace_packages(include=["kisters.*"]),
     zip_safe=False,
-    install_requires=["kisters.network_store.model_library>=0.5.0", "pydantic"],
+    install_requires=["kisters.network_store.model_library~=0.5.0", "pydantic"],
     extras_require={"test": ["pytest"]},
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)",
         "Operating System :: OS Independent",
```

### Comparing `kisters.network_store.model_library.water-0.3.0/test/test_water_models.py` & `kisters.network_store.model_library.water-0.3.1/test/test_water_models.py`

 * *Files identical despite different names*

