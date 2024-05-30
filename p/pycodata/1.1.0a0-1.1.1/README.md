# Comparing `tmp/pycodata-1.1.0a0.tar.gz` & `tmp/pycodata-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycodata-1.1.0a0.tar", last modified: Tue May 28 22:39:39 2024, max compression
+gzip compressed data, was "pycodata-1.1.1.tar", last modified: Thu May 30 05:04:07 2024, max compression
```

## Comparing `pycodata-1.1.0a0.tar` & `pycodata-1.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 milan      (501) staff       (20)        0 2024-05-28 22:39:39.864756 pycodata-1.1.0a0/
--rw-r--r--   0 milan      (501) staff       (20)     1069 2024-05-24 21:02:42.000000 pycodata-1.1.0a0/LICENSE
--rw-r--r--   0 milan      (501) staff       (20)     2001 2024-05-28 22:39:39.863692 pycodata-1.1.0a0/PKG-INFO
--rw-r--r--   0 milan      (501) staff       (20)     1386 2024-05-28 05:10:18.000000 pycodata-1.1.0a0/README.md
--rw-r--r--   0 milan      (501) staff       (20)      948 2024-05-28 22:39:10.000000 pycodata-1.1.0a0/pyproject.toml
--rw-r--r--   0 milan      (501) staff       (20)       38 2024-05-28 22:39:39.864966 pycodata-1.1.0a0/setup.cfg
--rw-r--r--   0 milan      (501) staff       (20)     2475 2024-05-27 01:37:24.000000 pycodata-1.1.0a0/setup.py
-drwxr-xr-x   0 milan      (501) staff       (20)        0 2024-05-28 22:39:39.791669 pycodata-1.1.0a0/src/
-drwxr-xr-x   0 milan      (501) staff       (20)        0 2024-05-28 22:39:39.855569 pycodata-1.1.0a0/src/pycodata/
--rw-r--r--   0 milan      (501) staff       (20)      432 2024-05-21 21:33:36.000000 pycodata-1.1.0a0/src/pycodata/__init__.py
--rw-r--r--   0 milan      (501) staff       (20)      102 2024-05-28 22:26:18.000000 pycodata-1.1.0a0/src/pycodata/ccodata.h
--rw-r--r--   0 milan      (501) staff       (20)      244 2024-05-28 22:26:18.000000 pycodata-1.1.0a0/src/pycodata/ccodata_constants.h
--rw-r--r--   0 milan      (501) staff       (20)    29567 2024-05-28 22:26:18.000000 pycodata-1.1.0a0/src/pycodata/ccodata_constants_2010.h
--rw-r--r--   0 milan      (501) staff       (20)    29567 2024-05-28 22:26:18.000000 pycodata-1.1.0a0/src/pycodata/ccodata_constants_2014.h
--rw-r--r--   0 milan      (501) staff       (20)    31256 2024-05-28 22:26:18.000000 pycodata-1.1.0a0/src/pycodata/ccodata_constants_2018.h
--rw-r--r--   0 milan      (501) staff       (20)    29568 2024-05-28 22:26:18.000000 pycodata-1.1.0a0/src/pycodata/ccodata_constants_2022.h
--rw-r--r--   0 milan      (501) staff       (20)      188 2024-05-28 22:26:18.000000 pycodata-1.1.0a0/src/pycodata/ccodata_constants_type.h
--rw-r--r--   0 milan      (501) staff       (20)      101 2024-05-28 22:26:18.000000 pycodata-1.1.0a0/src/pycodata/ccodata_version.h
--rw-r--r--   0 milan      (501) staff       (20)   128871 2024-05-28 22:27:20.000000 pycodata-1.1.0a0/src/pycodata/cpy_codata_constants_2010.c
--rw-r--r--   0 milan      (501) staff       (20)   128871 2024-05-28 22:27:20.000000 pycodata-1.1.0a0/src/pycodata/cpy_codata_constants_2014.c
--rw-r--r--   0 milan      (501) staff       (20)   136271 2024-05-28 22:27:21.000000 pycodata-1.1.0a0/src/pycodata/cpy_codata_constants_2018.c
--rw-r--r--   0 milan      (501) staff       (20)   127791 2024-05-28 22:27:21.000000 pycodata-1.1.0a0/src/pycodata/cpy_codata_constants_2022.c
--rw-r--r--   0 milan      (501) staff       (20)      593 2024-05-27 01:37:42.000000 pycodata-1.1.0a0/src/pycodata/cpy_codata_version.c
--rwxr-xr-x   0 milan      (501) staff       (20)   946032 2024-05-28 22:26:18.000000 pycodata-1.1.0a0/src/pycodata/libccodata.dylib
--rw-r--r--   0 milan      (501) staff       (20)   235624 2024-05-28 22:26:18.000000 pycodata-1.1.0a0/src/pycodata/libgcc_s.1.1.dylib
--rw-r--r--   0 milan      (501) staff       (20)  3504752 2024-05-28 22:26:18.000000 pycodata-1.1.0a0/src/pycodata/libgfortran.5.dylib
--rw-r--r--   0 milan      (501) staff       (20)   346616 2024-05-28 22:26:18.000000 pycodata-1.1.0a0/src/pycodata/libquadmath.0.dylib
-drwxr-xr-x   0 milan      (501) staff       (20)        0 2024-05-28 22:39:39.862723 pycodata-1.1.0a0/src/pycodata.egg-info/
--rw-r--r--   0 milan      (501) staff       (20)     2001 2024-05-28 22:39:39.000000 pycodata-1.1.0a0/src/pycodata.egg-info/PKG-INFO
--rw-r--r--   0 milan      (501) staff       (20)     1035 2024-05-28 22:39:39.000000 pycodata-1.1.0a0/src/pycodata.egg-info/SOURCES.txt
--rw-r--r--   0 milan      (501) staff       (20)        1 2024-05-28 22:39:39.000000 pycodata-1.1.0a0/src/pycodata.egg-info/dependency_links.txt
--rw-r--r--   0 milan      (501) staff       (20)        9 2024-05-28 22:39:39.000000 pycodata-1.1.0a0/src/pycodata.egg-info/top_level.txt
-drwxr-xr-x   0 milan      (501) staff       (20)        0 2024-05-28 22:39:39.861466 pycodata-1.1.0a0/test/
--rw-r--r--   0 milan      (501) staff       (20)     4611 2024-05-27 01:38:15.000000 pycodata-1.1.0a0/test/tests.py
+drwxr-xr-x   0 milan      (501) staff       (20)        0 2024-05-30 05:04:07.783100 pycodata-1.1.1/
+-rw-r--r--   0 milan      (501) staff       (20)     1069 2024-05-24 21:02:42.000000 pycodata-1.1.1/LICENSE
+-rw-r--r--   0 milan      (501) staff       (20)     1999 2024-05-30 05:04:07.782062 pycodata-1.1.1/PKG-INFO
+-rw-r--r--   0 milan      (501) staff       (20)     1386 2024-05-28 05:10:18.000000 pycodata-1.1.1/README.md
+-rw-r--r--   0 milan      (501) staff       (20)      947 2024-05-30 04:59:26.000000 pycodata-1.1.1/pyproject.toml
+-rw-r--r--   0 milan      (501) staff       (20)       38 2024-05-30 05:04:07.783280 pycodata-1.1.1/setup.cfg
+-rw-r--r--   0 milan      (501) staff       (20)     2475 2024-05-27 01:37:24.000000 pycodata-1.1.1/setup.py
+drwxr-xr-x   0 milan      (501) staff       (20)        0 2024-05-30 05:04:07.699449 pycodata-1.1.1/src/
+drwxr-xr-x   0 milan      (501) staff       (20)        0 2024-05-30 05:04:07.768056 pycodata-1.1.1/src/pycodata/
+-rw-r--r--   0 milan      (501) staff       (20)      432 2024-05-21 21:33:36.000000 pycodata-1.1.1/src/pycodata/__init__.py
+-rw-r--r--   0 milan      (501) staff       (20)      102 2024-05-30 05:03:16.000000 pycodata-1.1.1/src/pycodata/ccodata.h
+-rw-r--r--   0 milan      (501) staff       (20)      244 2024-05-30 05:03:16.000000 pycodata-1.1.1/src/pycodata/ccodata_constants.h
+-rw-r--r--   0 milan      (501) staff       (20)    29567 2024-05-30 05:03:16.000000 pycodata-1.1.1/src/pycodata/ccodata_constants_2010.h
+-rw-r--r--   0 milan      (501) staff       (20)    29567 2024-05-30 05:03:16.000000 pycodata-1.1.1/src/pycodata/ccodata_constants_2014.h
+-rw-r--r--   0 milan      (501) staff       (20)    31256 2024-05-30 05:03:16.000000 pycodata-1.1.1/src/pycodata/ccodata_constants_2018.h
+-rw-r--r--   0 milan      (501) staff       (20)    29568 2024-05-30 05:03:16.000000 pycodata-1.1.1/src/pycodata/ccodata_constants_2022.h
+-rw-r--r--   0 milan      (501) staff       (20)      188 2024-05-30 05:03:16.000000 pycodata-1.1.1/src/pycodata/ccodata_constants_type.h
+-rw-r--r--   0 milan      (501) staff       (20)      101 2024-05-30 05:03:16.000000 pycodata-1.1.1/src/pycodata/ccodata_version.h
+-rw-r--r--   0 milan      (501) staff       (20)   128871 2024-05-30 05:03:07.000000 pycodata-1.1.1/src/pycodata/cpy_codata_constants_2010.c
+-rw-r--r--   0 milan      (501) staff       (20)   128871 2024-05-30 05:03:07.000000 pycodata-1.1.1/src/pycodata/cpy_codata_constants_2014.c
+-rw-r--r--   0 milan      (501) staff       (20)   136271 2024-05-30 05:03:08.000000 pycodata-1.1.1/src/pycodata/cpy_codata_constants_2018.c
+-rw-r--r--   0 milan      (501) staff       (20)   127791 2024-05-30 05:03:08.000000 pycodata-1.1.1/src/pycodata/cpy_codata_constants_2022.c
+-rw-r--r--   0 milan      (501) staff       (20)      593 2024-05-27 01:37:42.000000 pycodata-1.1.1/src/pycodata/cpy_codata_version.c
+-rwxr-xr-x   0 milan      (501) staff       (20)   946032 2024-05-30 05:03:16.000000 pycodata-1.1.1/src/pycodata/libccodata.dylib
+-rw-r--r--   0 milan      (501) staff       (20)   235624 2024-05-30 05:03:16.000000 pycodata-1.1.1/src/pycodata/libgcc_s.1.1.dylib
+-rw-r--r--   0 milan      (501) staff       (20)  3504752 2024-05-30 05:03:16.000000 pycodata-1.1.1/src/pycodata/libgfortran.5.dylib
+-rw-r--r--   0 milan      (501) staff       (20)   346616 2024-05-30 05:03:16.000000 pycodata-1.1.1/src/pycodata/libquadmath.0.dylib
+drwxr-xr-x   0 milan      (501) staff       (20)        0 2024-05-30 05:04:07.780844 pycodata-1.1.1/src/pycodata.egg-info/
+-rw-r--r--   0 milan      (501) staff       (20)     1999 2024-05-30 05:04:07.000000 pycodata-1.1.1/src/pycodata.egg-info/PKG-INFO
+-rw-r--r--   0 milan      (501) staff       (20)     1035 2024-05-30 05:04:07.000000 pycodata-1.1.1/src/pycodata.egg-info/SOURCES.txt
+-rw-r--r--   0 milan      (501) staff       (20)        1 2024-05-30 05:04:07.000000 pycodata-1.1.1/src/pycodata.egg-info/dependency_links.txt
+-rw-r--r--   0 milan      (501) staff       (20)        9 2024-05-30 05:04:07.000000 pycodata-1.1.1/src/pycodata.egg-info/top_level.txt
+drwxr-xr-x   0 milan      (501) staff       (20)        0 2024-05-30 05:04:07.779744 pycodata-1.1.1/test/
+-rw-r--r--   0 milan      (501) staff       (20)     4611 2024-05-27 01:38:15.000000 pycodata-1.1.1/test/tests.py
```

### Comparing `pycodata-1.1.0a0/LICENSE` & `pycodata-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycodata-1.1.0a0/PKG-INFO` & `pycodata-1.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycodata
-Version: 1.1.0a0
+Version: 1.1.1
 Summary: pycodata: CODATA constants for python.
 Author-email: Milan Skocic <milan.skocic@icloud.com>
 License: License :: OSI Approved :: MIT License
 Project-URL: Documentation, https://milanskocic.github.io/codata-docs/index.html
 Project-URL: Source, https://github.com/MilanSkocic/codata-py
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pycodata-1.1.0a0/README.md` & `pycodata-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pycodata-1.1.0a0/pyproject.toml` & `pycodata-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel", "build"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pycodata"
-version = "1.1.0a"
+version = "1.1.1"
 authors = [{name = "Milan Skocic", email = "milan.skocic@icloud.com"}]
 description = "pycodata: CODATA constants for python."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "License :: OSI Approved :: MIT License"}
 classifiers=["Development Status :: 5 - Production/Stable",
              "Intended Audience :: Science/Research",
```

### Comparing `pycodata-1.1.0a0/setup.py` & `pycodata-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `pycodata-1.1.0a0/src/pycodata/ccodata_constants_2010.h` & `pycodata-1.1.1/src/pycodata/ccodata_constants_2010.h`

 * *Files identical despite different names*

### Comparing `pycodata-1.1.0a0/src/pycodata/ccodata_constants_2014.h` & `pycodata-1.1.1/src/pycodata/ccodata_constants_2014.h`

 * *Files identical despite different names*

### Comparing `pycodata-1.1.0a0/src/pycodata/ccodata_constants_2018.h` & `pycodata-1.1.1/src/pycodata/ccodata_constants_2018.h`

 * *Files identical despite different names*

### Comparing `pycodata-1.1.0a0/src/pycodata/ccodata_constants_2022.h` & `pycodata-1.1.1/src/pycodata/ccodata_constants_2022.h`

 * *Files identical despite different names*

### Comparing `pycodata-1.1.0a0/src/pycodata/cpy_codata_constants_2010.c` & `pycodata-1.1.1/src/pycodata/cpy_codata_constants_2010.c`

 * *Files identical despite different names*

### Comparing `pycodata-1.1.0a0/src/pycodata/cpy_codata_constants_2014.c` & `pycodata-1.1.1/src/pycodata/cpy_codata_constants_2014.c`

 * *Files identical despite different names*

### Comparing `pycodata-1.1.0a0/src/pycodata/cpy_codata_constants_2018.c` & `pycodata-1.1.1/src/pycodata/cpy_codata_constants_2018.c`

 * *Files identical despite different names*

### Comparing `pycodata-1.1.0a0/src/pycodata/cpy_codata_constants_2022.c` & `pycodata-1.1.1/src/pycodata/cpy_codata_constants_2022.c`

 * *Files identical despite different names*

### Comparing `pycodata-1.1.0a0/src/pycodata/cpy_codata_version.c` & `pycodata-1.1.1/src/pycodata/cpy_codata_version.c`

 * *Files identical despite different names*

### Comparing `pycodata-1.1.0a0/src/pycodata/libccodata.dylib` & `pycodata-1.1.1/src/pycodata/libccodata.dylib`

 * *Files identical despite different names*

### Comparing `pycodata-1.1.0a0/src/pycodata/libgcc_s.1.1.dylib` & `pycodata-1.1.1/src/pycodata/libgcc_s.1.1.dylib`

 * *Files identical despite different names*

### Comparing `pycodata-1.1.0a0/src/pycodata/libgfortran.5.dylib` & `pycodata-1.1.1/src/pycodata/libgfortran.5.dylib`

 * *Files identical despite different names*

### Comparing `pycodata-1.1.0a0/src/pycodata/libquadmath.0.dylib` & `pycodata-1.1.1/src/pycodata/libquadmath.0.dylib`

 * *Files identical despite different names*

### Comparing `pycodata-1.1.0a0/src/pycodata.egg-info/PKG-INFO` & `pycodata-1.1.1/src/pycodata.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycodata
-Version: 1.1.0a0
+Version: 1.1.1
 Summary: pycodata: CODATA constants for python.
 Author-email: Milan Skocic <milan.skocic@icloud.com>
 License: License :: OSI Approved :: MIT License
 Project-URL: Documentation, https://milanskocic.github.io/codata-docs/index.html
 Project-URL: Source, https://github.com/MilanSkocic/codata-py
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pycodata-1.1.0a0/src/pycodata.egg-info/SOURCES.txt` & `pycodata-1.1.1/src/pycodata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycodata-1.1.0a0/test/tests.py` & `pycodata-1.1.1/test/tests.py`

 * *Files identical despite different names*

