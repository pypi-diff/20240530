# Comparing `tmp/ciso-0.2.1.tar.gz` & `tmp/ciso-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ciso-0.2.1.tar", last modified: Thu May 30 19:26:03 2024, max compression
+gzip compressed data, was "ciso-0.2.2.tar", last modified: Thu May 30 19:53:04 2024, max compression
```

## Comparing `ciso-0.2.1.tar` & `ciso-0.2.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-30 19:26:03.763529 ciso-0.2.1/
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-30 19:26:03.755529 ciso-0.2.1/.github/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      310 2023-05-29 12:40:01.000000 ciso-0.2.1/.github/dependabot.yml
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-30 19:26:03.755529 ciso-0.2.1/.github/workflows/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     2273 2024-05-28 17:15:55.000000 ciso-0.2.1/.github/workflows/cibuildwheel.yml
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1331 2024-05-28 17:15:55.000000 ciso-0.2.1/.github/workflows/deploy-docs.yml
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1190 2024-05-30 18:52:49.000000 ciso-0.2.1/.github/workflows/tests.yml
--rw-rw-r--   0 filipe    (1000) filipe    (1000)       63 2022-10-19 12:56:01.000000 ciso-0.2.1/CHANGES.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1292 2022-10-19 21:54:23.000000 ciso-0.2.1/LICENSE.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      234 2022-10-19 17:08:06.000000 ciso-0.2.1/MANIFEST.in
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1090 2024-05-30 19:26:03.763529 ciso-0.2.1/PKG-INFO
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      363 2022-10-19 18:15:07.000000 ciso-0.2.1/README.md
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-30 19:26:03.759529 ciso-0.2.1/ciso/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      192 2022-10-19 21:54:23.000000 ciso-0.2.1/ciso/__init__.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)  1134285 2024-05-30 19:26:02.000000 ciso-0.2.1/ciso/_ciso.c
--rwxrwxr-x   0 filipe    (1000) filipe    (1000)   211048 2024-05-29 19:17:30.000000 ciso-0.2.1/ciso/_ciso.cpython-312-x86_64-linux-gnu.so
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1056 2024-05-30 18:52:49.000000 ciso-0.2.1/ciso/_ciso.pyx
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1502 2024-05-30 18:52:49.000000 ciso-0.2.1/ciso/ciso.py
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-30 19:26:03.763529 ciso-0.2.1/ciso/tests/
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-30 19:26:03.763529 ciso-0.2.1/ciso/tests/data/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    28192 2022-10-19 17:08:06.000000 ciso-0.2.1/ciso/tests/data/fortran.npz
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     2221 2024-05-30 18:52:49.000000 ciso-0.2.1/ciso/tests/test_ciso.py
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-30 19:26:03.763529 ciso-0.2.1/ciso.egg-info/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      380 2024-05-30 19:26:03.000000 ciso-0.2.1/ciso.egg-info/SOURCES.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1547 2024-05-30 18:52:49.000000 ciso-0.2.1/pyproject.toml
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      207 2023-05-29 13:37:06.000000 ciso-0.2.1/requirements-dev.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)       19 2022-10-19 17:08:06.000000 ciso-0.2.1/requirements.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)       38 2024-05-30 19:26:03.763529 ciso-0.2.1/setup.cfg
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      621 2024-05-28 17:59:48.000000 ciso-0.2.1/setup.py
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-30 19:53:04.385362 ciso-0.2.2/
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-30 19:53:04.381362 ciso-0.2.2/.github/
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      310 2023-05-29 12:40:01.000000 ciso-0.2.2/.github/dependabot.yml
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-30 19:53:04.381362 ciso-0.2.2/.github/workflows/
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     2273 2024-05-28 17:15:55.000000 ciso-0.2.2/.github/workflows/cibuildwheel.yml
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     1331 2024-05-28 17:15:55.000000 ciso-0.2.2/.github/workflows/deploy-docs.yml
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     1190 2024-05-30 18:52:49.000000 ciso-0.2.2/.github/workflows/tests.yml
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)       63 2022-10-19 12:56:01.000000 ciso-0.2.2/CHANGES.txt
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     1292 2022-10-19 21:54:23.000000 ciso-0.2.2/LICENSE.txt
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      234 2022-10-19 17:08:06.000000 ciso-0.2.2/MANIFEST.in
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1068 2024-05-30 19:53:04.385362 ciso-0.2.2/PKG-INFO
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      363 2022-10-19 18:15:07.000000 ciso-0.2.2/README.md
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-30 19:53:04.385362 ciso-0.2.2/ciso/
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      192 2022-10-19 21:54:23.000000 ciso-0.2.2/ciso/__init__.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)  1134285 2024-05-30 19:53:02.000000 ciso-0.2.2/ciso/_ciso.c
+-rwxrwxr-x   0 filipe    (1000) filipe    (1000)   211048 2024-05-30 19:34:08.000000 ciso-0.2.2/ciso/_ciso.cpython-312-x86_64-linux-gnu.so
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     1056 2024-05-30 18:52:49.000000 ciso-0.2.2/ciso/_ciso.pyx
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     1502 2024-05-30 18:52:49.000000 ciso-0.2.2/ciso/ciso.py
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-30 19:53:04.385362 ciso-0.2.2/ciso/tests/
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-30 19:53:04.385362 ciso-0.2.2/ciso/tests/data/
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)    28192 2022-10-19 17:08:06.000000 ciso-0.2.2/ciso/tests/data/fortran.npz
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     2221 2024-05-30 18:52:49.000000 ciso-0.2.2/ciso/tests/test_ciso.py
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-30 19:53:04.385362 ciso-0.2.2/ciso.egg-info/
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      380 2024-05-30 19:53:04.000000 ciso-0.2.2/ciso.egg-info/SOURCES.txt
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     1656 2024-05-30 19:52:37.000000 ciso-0.2.2/pyproject.toml
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      207 2023-05-29 13:37:06.000000 ciso-0.2.2/requirements-dev.txt
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)       19 2022-10-19 17:08:06.000000 ciso-0.2.2/requirements.txt
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)       38 2024-05-30 19:53:04.385362 ciso-0.2.2/setup.cfg
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      233 2024-05-30 19:52:37.000000 ciso-0.2.2/setup.py
```

### Comparing `ciso-0.2.1/.github/workflows/cibuildwheel.yml` & `ciso-0.2.2/.github/workflows/cibuildwheel.yml`

 * *Files identical despite different names*

### Comparing `ciso-0.2.1/.github/workflows/deploy-docs.yml` & `ciso-0.2.2/.github/workflows/deploy-docs.yml`

 * *Files identical despite different names*

### Comparing `ciso-0.2.1/.github/workflows/tests.yml` & `ciso-0.2.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `ciso-0.2.1/LICENSE.txt` & `ciso-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ciso-0.2.1/PKG-INFO` & `ciso-0.2.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: ciso
-Version: 0.2.1
+Version: 0.2.2
 Summary: Create isosurfaces from 2D or 3D arrays
 Author: Robert Hetland
 Author-email: hetland@tamu.edu
 License: BSD-2-Clause
 Project-URL: homepage, https://github.com/ioos/ciso
 Project-URL: documentation, https://ioos.github.io/ciso
 Project-URL: repository, https://github.com/ioos/ciso
 Platform: any
 Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: cython>=3
 Requires-Dist: oldest-supported-numpy; python_version < "3.9"
 Requires-Dist: numpy>=2.0.0rc1; python_version >= "3.9"
 Provides-Extra: extras
 Requires-Dist: gridgeo; extra == "extras"
 Requires-Dist: cartopy; extra == "extras"
 Requires-Dist: xarray; extra == "extras"
```

### Comparing `ciso-0.2.1/ciso/_ciso.c` & `ciso-0.2.2/ciso/_ciso.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 /* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/_core/include/numpy/arrayobject.h",
-            "/tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/_core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/_core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/_core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/_core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/_core/include/numpy/arrayobject.h",
+            "/tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/_core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/_core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/_core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/_core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/_core/include"
+            "/tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/_core/include"
         ],
         "name": "ciso._ciso",
         "sources": [
             "ciso/_ciso.pyx"
         ]
     },
     "module_name": "ciso._ciso"
@@ -1668,159 +1668,159 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":770
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":770
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":771
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":772
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":772
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":777
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":777
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":778
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":778
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":780
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":780
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":784
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":784
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":792
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":792
  * ctypedef double complex complex128_t
  * 
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":793
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":793
  * 
  * ctypedef npy_longlong   longlong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":795
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":795
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":796
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":796
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":798
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":798
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":799
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":799
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":800
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":800
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef float complex       cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1865,24 +1865,24 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1096
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1096
  * 
  * # Iterator API added in v1.6
  * ctypedef int (*NpyIter_IterNextFunc)(NpyIter* it) noexcept nogil             # <<<<<<<<<<<<<<
  * ctypedef void (*NpyIter_GetMultiIndexFunc)(NpyIter* it, npy_intp* outcoords) noexcept nogil
  * 
  */
 typedef int (*__pyx_t_5numpy_NpyIter_IterNextFunc)(NpyIter *);
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1097
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1097
  * # Iterator API added in v1.6
  * ctypedef int (*NpyIter_IterNextFunc)(NpyIter* it) noexcept nogil
  * ctypedef void (*NpyIter_GetMultiIndexFunc)(NpyIter* it, npy_intp* outcoords) noexcept nogil             # <<<<<<<<<<<<<<
  * 
  * cdef extern from "numpy/arrayobject.h":
  */
 typedef void (*__pyx_t_5numpy_NpyIter_GetMultiIndexFunc)(NpyIter *, npy_intp *);
@@ -17973,685 +17973,685 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":286
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":286
  * 
  *         @property
  *         cdef inline npy_intp itemsize(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             return PyDataType_ELSIZE(self)
  * 
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_5dtype_8itemsize_itemsize(PyArray_Descr *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":287
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":287
  *         @property
  *         cdef inline npy_intp itemsize(self) noexcept nogil:
  *             return PyDataType_ELSIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyDataType_ELSIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":286
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":286
  * 
  *         @property
  *         cdef inline npy_intp itemsize(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             return PyDataType_ELSIZE(self)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
  * 
  *         @property
  *         cdef inline npy_intp alignment(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             return PyDataType_ALIGNMENT(self)
  * 
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_5dtype_9alignment_alignment(PyArray_Descr *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":291
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":291
  *         @property
  *         cdef inline npy_intp alignment(self) noexcept nogil:
  *             return PyDataType_ALIGNMENT(self)             # <<<<<<<<<<<<<<
  * 
  *         # Use fields/names with care as they may be NULL.  You must check
  */
   __pyx_r = PyDataType_ALIGNMENT(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
  * 
  *         @property
  *         cdef inline npy_intp alignment(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             return PyDataType_ALIGNMENT(self)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":296
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":296
  *         # for this using PyDataType_HASFIELDS.
  *         @property
  *         cdef inline object fields(self):             # <<<<<<<<<<<<<<
  *             return <object>PyDataType_FIELDS(self)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_5dtype_6fields_fields(PyArray_Descr *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1;
   __Pyx_RefNannySetupContext("fields", 1);
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":297
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":297
  *         @property
  *         cdef inline object fields(self):
  *             return <object>PyDataType_FIELDS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyDataType_FIELDS(__pyx_v_self);
   __Pyx_INCREF(((PyObject *)__pyx_t_1));
   __pyx_r = ((PyObject *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":296
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":296
  *         # for this using PyDataType_HASFIELDS.
  *         @property
  *         cdef inline object fields(self):             # <<<<<<<<<<<<<<
  *             return <object>PyDataType_FIELDS(self)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":300
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":300
  * 
  *         @property
  *         cdef inline tuple names(self):             # <<<<<<<<<<<<<<
  *             return <tuple>PyDataType_NAMES(self)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_5dtype_5names_names(PyArray_Descr *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1;
   __Pyx_RefNannySetupContext("names", 1);
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":301
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":301
  *         @property
  *         cdef inline tuple names(self):
  *             return <tuple>PyDataType_NAMES(self)             # <<<<<<<<<<<<<<
  * 
  *         # Use PyDataType_HASSUBARRAY to test whether this field is
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyDataType_NAMES(__pyx_v_self);
   __Pyx_INCREF(((PyObject*)__pyx_t_1));
   __pyx_r = ((PyObject*)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":300
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":300
  * 
  *         @property
  *         cdef inline tuple names(self):             # <<<<<<<<<<<<<<
  *             return <tuple>PyDataType_NAMES(self)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":307
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":307
  *         # this field via the inline helper method PyDataType_SHAPE.
  *         @property
  *         cdef inline PyArray_ArrayDescr* subarray(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             return PyDataType_SUBARRAY(self)
  * 
  */
 
 static CYTHON_INLINE PyArray_ArrayDescr *__pyx_f_5numpy_5dtype_8subarray_subarray(PyArray_Descr *__pyx_v_self) {
   PyArray_ArrayDescr *__pyx_r;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":308
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":308
  *         @property
  *         cdef inline PyArray_ArrayDescr* subarray(self) noexcept nogil:
  *             return PyDataType_SUBARRAY(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyDataType_SUBARRAY(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":307
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":307
  *         # this field via the inline helper method PyDataType_SHAPE.
  *         @property
  *         cdef inline PyArray_ArrayDescr* subarray(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             return PyDataType_SUBARRAY(self)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":311
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":311
  * 
  *         @property
  *         cdef inline npy_uint64 flags(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """The data types flags."""
  *             return PyDataType_FLAGS(self)
  */
 
 static CYTHON_INLINE npy_uint64 __pyx_f_5numpy_5dtype_5flags_flags(PyArray_Descr *__pyx_v_self) {
   npy_uint64 __pyx_r;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":313
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":313
  *         cdef inline npy_uint64 flags(self) noexcept nogil:
  *             """The data types flags."""
  *             return PyDataType_FLAGS(self)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyDataType_FLAGS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":311
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":311
  * 
  *         @property
  *         cdef inline npy_uint64 flags(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """The data types flags."""
  *             return PyDataType_FLAGS(self)
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":323
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":323
  * 
  *         @property
  *         cdef inline int numiter(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """The number of arrays that need to be broadcast to the same shape."""
  *             return PyArray_MultiIter_NUMITER(self)
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_9broadcast_7numiter_numiter(PyArrayMultiIterObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":325
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":325
  *         cdef inline int numiter(self) noexcept nogil:
  *             """The number of arrays that need to be broadcast to the same shape."""
  *             return PyArray_MultiIter_NUMITER(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_MultiIter_NUMITER(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":323
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":323
  * 
  *         @property
  *         cdef inline int numiter(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """The number of arrays that need to be broadcast to the same shape."""
  *             return PyArray_MultiIter_NUMITER(self)
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":328
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":328
  * 
  *         @property
  *         cdef inline npy_intp size(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """The total broadcasted size."""
  *             return PyArray_MultiIter_SIZE(self)
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_9broadcast_4size_size(PyArrayMultiIterObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":330
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":330
  *         cdef inline npy_intp size(self) noexcept nogil:
  *             """The total broadcasted size."""
  *             return PyArray_MultiIter_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_MultiIter_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":328
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":328
  * 
  *         @property
  *         cdef inline npy_intp size(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """The total broadcasted size."""
  *             return PyArray_MultiIter_SIZE(self)
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":333
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":333
  * 
  *         @property
  *         cdef inline npy_intp index(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """The current (1-d) index into the broadcasted result."""
  *             return PyArray_MultiIter_INDEX(self)
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_9broadcast_5index_index(PyArrayMultiIterObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":335
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":335
  *         cdef inline npy_intp index(self) noexcept nogil:
  *             """The current (1-d) index into the broadcasted result."""
  *             return PyArray_MultiIter_INDEX(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_MultiIter_INDEX(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":333
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":333
  * 
  *         @property
  *         cdef inline npy_intp index(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """The current (1-d) index into the broadcasted result."""
  *             return PyArray_MultiIter_INDEX(self)
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":338
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":338
  * 
  *         @property
  *         cdef inline int nd(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """The number of dimensions in the broadcasted result."""
  *             return PyArray_MultiIter_NDIM(self)
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_9broadcast_2nd_nd(PyArrayMultiIterObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":340
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":340
  *         cdef inline int nd(self) noexcept nogil:
  *             """The number of dimensions in the broadcasted result."""
  *             return PyArray_MultiIter_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_MultiIter_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":338
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":338
  * 
  *         @property
  *         cdef inline int nd(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """The number of dimensions in the broadcasted result."""
  *             return PyArray_MultiIter_NDIM(self)
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":343
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":343
  * 
  *         @property
  *         cdef inline npy_intp* dimensions(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """The shape of the broadcasted result."""
  *             return PyArray_MultiIter_DIMS(self)
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_9broadcast_10dimensions_dimensions(PyArrayMultiIterObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":345
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":345
  *         cdef inline npy_intp* dimensions(self) noexcept nogil:
  *             """The shape of the broadcasted result."""
  *             return PyArray_MultiIter_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_MultiIter_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":343
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":343
  * 
  *         @property
  *         cdef inline npy_intp* dimensions(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """The shape of the broadcasted result."""
  *             return PyArray_MultiIter_DIMS(self)
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":348
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":348
  * 
  *         @property
  *         cdef inline void** iters(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """An array of iterator objects that holds the iterators for the arrays to be broadcast together.
  *             On return, the iterators are adjusted for broadcasting."""
  */
 
 static CYTHON_INLINE void **__pyx_f_5numpy_9broadcast_5iters_iters(PyArrayMultiIterObject *__pyx_v_self) {
   void **__pyx_r;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":351
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":351
  *             """An array of iterator objects that holds the iterators for the arrays to be broadcast together.
  *             On return, the iterators are adjusted for broadcasting."""
  *             return PyArray_MultiIter_ITERS(self)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyArray_MultiIter_ITERS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":348
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":348
  * 
  *         @property
  *         cdef inline void** iters(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """An array of iterator objects that holds the iterators for the arrays to be broadcast together.
  *             On return, the iterators are adjusted for broadcasting."""
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":366
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":366
  * 
  *         @property
  *         cdef inline PyObject* base(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":369
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":369
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":366
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":366
  * 
  *         @property
  *         cdef inline PyObject* base(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":372
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":372
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":375
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":375
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":372
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":372
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":378
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":378
  * 
  *         @property
  *         cdef inline int ndim(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":381
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":381
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":378
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":378
  * 
  *         @property
  *         cdef inline int ndim(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":384
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":384
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":389
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":389
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":384
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":384
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":392
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":392
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":396
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":396
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":392
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":392
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":399
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":399
  * 
  *         @property
  *         cdef inline npy_intp size(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":402
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":402
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":399
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":399
  * 
  *         @property
  *         cdef inline npy_intp size(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":405
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":405
  * 
  *         @property
  *         cdef inline char* data(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":411
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":411
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":405
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":405
  * 
  *         @property
  *         cdef inline char* data(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":807
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":807
  * ctypedef long double complex clongdouble_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18660,29 +18660,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":808
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":808
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 808, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":807
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":807
  * ctypedef long double complex clongdouble_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18693,15 +18693,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":810
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":810
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18710,29 +18710,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":811
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":811
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 811, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":810
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":810
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18743,15 +18743,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":813
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":813
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18760,29 +18760,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":814
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":814
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 814, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":813
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":813
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18793,15 +18793,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":816
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":816
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18810,29 +18810,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":817
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":817
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 817, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":816
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":816
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18843,15 +18843,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":819
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":819
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18860,29 +18860,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":820
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":820
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 820, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":819
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":819
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18893,219 +18893,219 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":822
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":822
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":823
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":823
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":824
+    /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":824
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_t_2 = __pyx_f_5numpy_5dtype_8subarray_subarray(__pyx_v_d)->shape;
     __Pyx_INCREF(((PyObject*)__pyx_t_2));
     __pyx_r = ((PyObject*)__pyx_t_2);
     goto __pyx_L0;
 
-    /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":823
+    /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":823
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":826
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":826
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":822
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":822
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1010
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1010
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base) except *:             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1011
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1011
  * 
  * cdef inline void set_array_base(ndarray arr, object base) except *:
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1012
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1012
  * cdef inline void set_array_base(ndarray arr, object base) except *:
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 1012, __pyx_L1_error)
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1010
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1010
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base) except *:             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1015
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1015
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1016
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1016
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1017
+    /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1017
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1016
+    /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1016
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1018
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1018
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1022
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1022
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19121,15 +19121,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1023
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1023
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -19137,68 +19137,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1024
+      /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1024
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy._core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 1024, __pyx_L3_error)
 
-      /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1023
+      /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1023
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1025
+    /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1025
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy._core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 1025, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1026
+      /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1026
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy._core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 1026, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 1026, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1023
+    /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1023
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19206,15 +19206,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1022
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1022
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19229,15 +19229,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1028
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1028
  *         raise ImportError("numpy._core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19253,15 +19253,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19269,68 +19269,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1030
+      /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1030
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy._core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 1030, __pyx_L3_error)
 
-      /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
+      /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1031
+    /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1031
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy._core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 1031, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1032
+      /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1032
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy._core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 1032, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 1032, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
+    /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19338,15 +19338,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1028
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1028
  *         raise ImportError("numpy._core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19361,15 +19361,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1034
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1034
  *         raise ImportError("numpy._core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19385,15 +19385,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1035
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1035
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19401,68 +19401,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1036
+      /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1036
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy._core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 1036, __pyx_L3_error)
 
-      /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1035
+      /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1035
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1037
+    /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1037
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy._core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 1037, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1038
+      /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1038
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy._core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 1038, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 1038, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1035
+    /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1035
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19470,15 +19470,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1034
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1034
  *         raise ImportError("numpy._core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19493,172 +19493,172 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1041
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj) noexcept:             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1053
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1053
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1041
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj) noexcept:             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1056
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1056
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj) noexcept:             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1068
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1068
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1056
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1056
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj) noexcept:             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1071
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1071
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) noexcept nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1078
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1078
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1071
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1071
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) noexcept nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1081
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1081
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) noexcept nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1085
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1085
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1081
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1081
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) noexcept nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1088
+/* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1088
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) noexcept nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1092
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1092
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1088
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1088
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) noexcept nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -21401,26 +21401,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1026
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1026
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy._core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_numpy__core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 1026, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../../../../tmp/build-env-aah_lqaz/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1032
+  /* "../../../../../../../tmp/build-env-q_k65g8m/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1032
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy._core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_numpy__core_umath_failed_to_impo); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 1032, __pyx_L1_error)
```

### Comparing `ciso-0.2.1/ciso/_ciso.cpython-312-x86_64-linux-gnu.so` & `ciso-0.2.2/ciso/_ciso.cpython-312-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `ciso-0.2.1/ciso/_ciso.pyx` & `ciso-0.2.2/ciso/_ciso.pyx`

 * *Files identical despite different names*

### Comparing `ciso-0.2.1/ciso/ciso.py` & `ciso-0.2.2/ciso/ciso.py`

 * *Files identical despite different names*

### Comparing `ciso-0.2.1/ciso/tests/data/fortran.npz` & `ciso-0.2.2/ciso/tests/data/fortran.npz`

 * *Files identical despite different names*

### Comparing `ciso-0.2.1/ciso/tests/test_ciso.py` & `ciso-0.2.2/ciso/tests/test_ciso.py`

 * *Files identical despite different names*

### Comparing `ciso-0.2.1/pyproject.toml` & `ciso-0.2.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [build-system]
 requires = [
   "setuptools>=41.2",
   "setuptools-scm",
-  "cython",
+  "cython>=3",
   "oldest-supported-numpy ; python_version < '3.9'",
   "numpy>=2.0.0rc1 ; python_version >= '3.9'",
   "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ciso"
-dynamic = ["version", "readme"]
+dynamic = ["version"]
 description = "Create isosurfaces from 2D or 3D arrays"
+readme = "README.md"
 authors = [
   {email = "hetland@tamu.edu"},
   {name = "Robert Hetland"}
 ]
 requires-python = ">=3.9"
 license = {text = "BSD-2-Clause"}
 dependencies = [
-    "cython>=3",
     "oldest-supported-numpy ; python_version < '3.9'",
     "numpy>=2.0.0rc1 ; python_version >= '3.9'",
 ]
 
 [project.optional-dependencies]
 extras = [
     "gridgeo",
@@ -39,16 +39,18 @@
 
 [tool.setuptools]
 license-files = ["LICENSE.txt"]
 zip-safe = true
 platforms = ["any"]
 packages = ["ciso"]
 
-[tool.setuptools.dynamic.readme]
-file = ["README.md"]
+[tool.setuptools_scm]
+write_to = "ciso/_version.py"
+write_to_template = "__version__ = '{version}'"
+tag_regex = "^(?P<prefix>v)?(?P<version>[^\\+]+)(?P<suffix>.*)?$"
 
 [tool.pytest.ini_options]
 filterwarnings = [
     "error",
     "ignore::UserWarning",
 ]
 addopts = "-s -rxs -v"
```

