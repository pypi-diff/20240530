# Comparing `tmp/npcolony-1.2.1.tar.gz` & `tmp/npcolony-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/npcolony-1.2.1.tar", last modified: Wed May  1 11:21:21 2024, max compression
+gzip compressed data, was "dist/npcolony-1.2.4.tar", last modified: Wed May 29 22:13:45 2024, max compression
```

## Comparing `npcolony-1.2.1.tar` & `npcolony-1.2.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 11:21:21.000000 npcolony-1.2.1/
--rw-r--r--   0 root         (0) root         (0)     5026 2024-05-01 11:21:13.000000 npcolony-1.2.1/setup.py
--rw-r--r--   0 root         (0) root         (0)     3126 2024-05-01 11:21:13.000000 npcolony-1.2.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-01 11:21:21.000000 npcolony-1.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     5077 2024-05-01 11:21:21.000000 npcolony-1.2.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 11:21:21.000000 npcolony-1.2.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 11:21:21.000000 npcolony-1.2.1/src/colony_npapi/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 11:21:21.000000 npcolony-1.2.1/src/colony_npapi/plugin/
--rw-r--r--   0 root         (0) root         (0)    19624 2024-05-01 11:21:13.000000 npcolony-1.2.1/src/colony_npapi/plugin/base.c
--rw-r--r--   0 root         (0) root         (0)    10238 2024-05-01 11:21:13.000000 npcolony-1.2.1/src/colony_npapi/plugin/python.c
--rw-r--r--   0 root         (0) root         (0)     1578 2024-05-01 11:21:13.000000 npcolony-1.2.1/src/colony_npapi/plugin/util.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 11:21:21.000000 npcolony-1.2.1/src/colony_npapi/system/
--rw-r--r--   0 root         (0) root         (0)     1125 2024-05-01 11:21:13.000000 npcolony-1.2.1/src/colony_npapi/system/gui_unix.c
--rw-r--r--   0 root         (0) root         (0)     2099 2024-05-01 11:21:13.000000 npcolony-1.2.1/src/colony_npapi/system/gui_win32.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 11:21:21.000000 npcolony-1.2.1/src/colony_npapi/print/
--rw-r--r--   0 root         (0) root         (0)     6508 2024-05-01 11:21:13.000000 npcolony-1.2.1/src/colony_npapi/print/print_unix.c
--rw-r--r--   0 root         (0) root         (0)    29604 2024-05-01 11:21:13.000000 npcolony-1.2.1/src/colony_npapi/print/print_win32.c
--rw-r--r--   0 root         (0) root         (0)     1261 2024-05-01 11:21:13.000000 npcolony-1.2.1/src/colony_npapi/stdafx.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 11:21:21.000000 npcolony-1.2.1/src/colony_npapi/encoding/
--rw-r--r--   0 root         (0) root         (0)    11403 2024-05-01 11:21:13.000000 npcolony-1.2.1/src/colony_npapi/encoding/base_64.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 11:21:21.000000 npcolony-1.2.1/src/python/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 11:21:21.000000 npcolony-1.2.1/src/python/npcolony_py/
--rw-r--r--   0 root         (0) root         (0)       44 2024-05-01 11:21:13.000000 npcolony-1.2.1/src/python/npcolony_py/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 11:21:21.000000 npcolony-1.2.1/src/python/npcolony_py/test/
--rw-r--r--   0 root         (0) root         (0)       44 2024-05-01 11:21:13.000000 npcolony-1.2.1/src/python/npcolony_py/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)      323 2024-05-01 11:21:13.000000 npcolony-1.2.1/src/python/npcolony_py/test/global.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 11:21:21.000000 npcolony-1.2.1/src/python/npcolony.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-01 11:21:21.000000 npcolony-1.2.1/src/python/npcolony.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      646 2024-05-01 11:21:21.000000 npcolony-1.2.1/src/python/npcolony.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-05-01 11:21:21.000000 npcolony-1.2.1/src/python/npcolony.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5077 2024-05-01 11:21:21.000000 npcolony-1.2.1/src/python/npcolony.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-01 11:21:18.000000 npcolony-1.2.1/src/python/npcolony.egg-info/not-zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 22:13:45.000000 npcolony-1.2.4/
+-rw-r--r--   0 root         (0) root         (0)     3124 2024-05-29 22:13:37.000000 npcolony-1.2.4/README.md
+-rw-r--r--   0 root         (0) root         (0)     5075 2024-05-29 22:13:45.000000 npcolony-1.2.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 22:13:45.000000 npcolony-1.2.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 22:13:45.000000 npcolony-1.2.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 22:13:45.000000 npcolony-1.2.4/src/colony_npapi/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 22:13:45.000000 npcolony-1.2.4/src/colony_npapi/plugin/
+-rw-r--r--   0 root         (0) root         (0)     1578 2024-05-29 22:13:37.000000 npcolony-1.2.4/src/colony_npapi/plugin/util.c
+-rw-r--r--   0 root         (0) root         (0)    19624 2024-05-29 22:13:37.000000 npcolony-1.2.4/src/colony_npapi/plugin/base.c
+-rw-r--r--   0 root         (0) root         (0)    10238 2024-05-29 22:13:37.000000 npcolony-1.2.4/src/colony_npapi/plugin/python.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 22:13:45.000000 npcolony-1.2.4/src/colony_npapi/system/
+-rw-r--r--   0 root         (0) root         (0)     2099 2024-05-29 22:13:37.000000 npcolony-1.2.4/src/colony_npapi/system/gui_win32.c
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-05-29 22:13:37.000000 npcolony-1.2.4/src/colony_npapi/system/gui_unix.c
+-rw-r--r--   0 root         (0) root         (0)     1261 2024-05-29 22:13:37.000000 npcolony-1.2.4/src/colony_npapi/stdafx.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 22:13:45.000000 npcolony-1.2.4/src/colony_npapi/encoding/
+-rw-r--r--   0 root         (0) root         (0)    11403 2024-05-29 22:13:37.000000 npcolony-1.2.4/src/colony_npapi/encoding/base_64.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 22:13:45.000000 npcolony-1.2.4/src/colony_npapi/print/
+-rw-r--r--   0 root         (0) root         (0)    29604 2024-05-29 22:13:37.000000 npcolony-1.2.4/src/colony_npapi/print/print_win32.c
+-rw-r--r--   0 root         (0) root         (0)     6508 2024-05-29 22:13:37.000000 npcolony-1.2.4/src/colony_npapi/print/print_unix.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 22:13:45.000000 npcolony-1.2.4/src/python/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 22:13:45.000000 npcolony-1.2.4/src/python/npcolony_py/
+-rw-r--r--   0 root         (0) root         (0)       44 2024-05-29 22:13:37.000000 npcolony-1.2.4/src/python/npcolony_py/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 22:13:45.000000 npcolony-1.2.4/src/python/npcolony_py/test/
+-rw-r--r--   0 root         (0) root         (0)       44 2024-05-29 22:13:37.000000 npcolony-1.2.4/src/python/npcolony_py/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      325 2024-05-29 22:13:37.000000 npcolony-1.2.4/src/python/npcolony_py/test/global.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 22:13:45.000000 npcolony-1.2.4/src/python/npcolony.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      646 2024-05-29 22:13:45.000000 npcolony-1.2.4/src/python/npcolony.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     5075 2024-05-29 22:13:45.000000 npcolony-1.2.4/src/python/npcolony.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 22:13:41.000000 npcolony-1.2.4/src/python/npcolony.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-29 22:13:45.000000 npcolony-1.2.4/src/python/npcolony.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 22:13:45.000000 npcolony-1.2.4/src/python/npcolony.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     5093 2024-05-29 22:13:37.000000 npcolony-1.2.4/setup.py
```

### Comparing `npcolony-1.2.1/setup.py` & `npcolony-1.2.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,99 +25,91 @@
 __copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import os
+import glob
 import setuptools
 
-def rename_sources(sources, base = ".c", target = ".cpp"):
+
+def rename_sources(sources, base=".c", target=".cpp"):
     renamed = []
     for source in sources:
         source_extension = os.path.splitext(source)[1]
-        if not source_extension == base: continue
+        if not source_extension == base:
+            continue
         source_name = os.path.splitext(source)[0]
         new_source_path = source_name + target
         os.rename(source, new_source_path)
         renamed.append(new_source_path)
     return renamed
 
-def rollback_sources(sources, base = ".cpp", target = ".c"):
-    return rename_sources(sources, base = base, target = target)
+
+def rollback_sources(sources, base=".cpp", target=".c"):
+    return rename_sources(sources, base=base, target=target)
+
 
 module = setuptools.Extension(
     "npcolony",
-    define_macros = [
-        ("MAJOR_VERSION", "1"),
-        ('MINOR_VERSION', '0')
-    ],
-    include_dirs = [
-        ".",
-        "src/colony_npapi/",
-        "/usr/local/include"
-    ],
-    libraries = [
-        "user32",
-        "gdi32",
-        "winspool",
-        "comdlg32"
-    ] if os.name in ("nt",) else ["cups"],
-    library_dirs = ["/usr/local/lib"],
-    extra_compile_args = [
-        "/DHAVE_LIBPYTHON",
-        "/DHAVE_LIBPYTHON_UNDEF"
-    ] if os.name in ("nt",) else [
-        "-std=c99",
-        "-pedantic",
-        "-finline-functions",
-        "-Wall",
-        "-Wno-long-long",
-        "-Wno-variadic-macros",
-        "-Wno-strict-aliasing",
-        "-Wno-strict-prototypes",
-        "-DNO_CONFIG_H",
-        "-DCOLONY_PLATFORM_UNIX"
-    ],
-    sources = [
-        "src/colony_npapi/stdafx.c",
-        "src/colony_npapi/encoding/base_64.c",
-        "src/colony_npapi/plugin/base.c",
-        "src/colony_npapi/plugin/python.c",
-        "src/colony_npapi/plugin/util.c",
-        "src/colony_npapi/print/print_unix.c",
-        "src/colony_npapi/print/print_win32.c",
-        "src/colony_npapi/system/gui_unix.c",
-        "src/colony_npapi/system/gui_win32.c"
-    ]
+    define_macros=[("MAJOR_VERSION", "1"), ("MINOR_VERSION", "0")],
+    include_dirs=[".", "src/colony_npapi/", "/usr/local/include"],
+    libraries=(
+        ["user32", "gdi32", "winspool", "comdlg32"] if os.name in ("nt",) else ["cups"]
+    ),
+    library_dirs=["/usr/local/lib"],
+    extra_compile_args=(
+        ["/DHAVE_LIBPYTHON", "/DHAVE_LIBPYTHON_UNDEF"]
+        if os.name in ("nt",)
+        else [
+            "-std=c99",
+            "-pedantic",
+            "-finline-functions",
+            "-Wall",
+            "-Wno-long-long",
+            "-Wno-variadic-macros",
+            "-Wno-strict-aliasing",
+            "-Wno-strict-prototypes",
+            "-DNO_CONFIG_H",
+            "-DCOLONY_PLATFORM_UNIX",
+        ]
+    ),
+    sources=glob.glob("src/colony_npapi/*.c")
+    + glob.glob("src/colony_npapi/encoding/*.c")
+    + glob.glob("src/colony_npapi/plugin/*.c")
+    + glob.glob("src/colony_npapi/print/*.c")
+    + glob.glob("src/colony_npapi/system/*.c"),
 )
 
 if os.name in ("nt",):
     module.sources = rename_sources(module.sources)
 try:
     setuptools.setup(
-        name = "npcolony",
-        version = "1.2.1",
-        author = "Hive Solutions Lda.",
-        author_email = "development@hive.pt",
-        description = "Colony Framework",
-        license = "Apache License, Version 2.0",
-        keywords = "colony npapi native",
-        url = "http://colony_npapi.hive.pt",
-        packages = [
-            "npcolony_py",
-            "npcolony_py.test"
-        ],
-        test_suite = "npcolony_py.test",
-        package_dir = {
-            "" : os.path.normpath("src/python")
+        name="npcolony",
+        version="1.2.4",
+        author="Hive Solutions Lda.",
+        author_email="development@hive.pt",
+        description="Colony Framework",
+        license="Apache License, Version 2.0",
+        keywords="colony npapi native",
+        url="http://colony_npapi.hive.pt",
+        packages=["npcolony_py", "npcolony_py.test"],
+        test_suite="npcolony_py.test",
+        package_dir={"": os.path.normpath("src/python")},
+        package_data={
+            "npcolony_py": glob.glob("src/colony_npapi/*.h")
+            + glob.glob("src/colony_npapi/encoding/*.h")
+            + glob.glob("src/colony_npapi/plugin/*.h")
+            + glob.glob("src/colony_npapi/print/*.h")
+            + glob.glob("src/colony_npapi/system/*.h"),
         },
-        zip_safe = False,
-        ext_modules = [module],
-        classifiers = [
+        zip_safe=False,
+        ext_modules=[module],
+        classifiers=[
             "Development Status :: 5 - Production/Stable",
             "Topic :: Utilities",
             "License :: OSI Approved :: Apache Software License",
             "Operating System :: OS Independent",
             "Programming Language :: Python",
             "Programming Language :: Python :: 2.6",
             "Programming Language :: Python :: 2.7",
@@ -129,15 +121,19 @@
             "Programming Language :: Python :: 3.5",
             "Programming Language :: Python :: 3.6",
             "Programming Language :: Python :: 3.7",
             "Programming Language :: Python :: 3.8",
             "Programming Language :: Python :: 3.9",
             "Programming Language :: Python :: 3.10",
             "Programming Language :: Python :: 3.11",
-            "Programming Language :: Python :: 3.12"
+            "Programming Language :: Python :: 3.12",
         ],
-        long_description = open(os.path.join(os.path.dirname(__file__), "README.md"), "rb").read().decode("utf-8"),
-        long_description_content_type = "text/markdown"
+        long_description=open(
+            os.path.join(os.path.dirname(__file__), "README.md"), "rb"
+        )
+        .read()
+        .decode("utf-8"),
+        long_description_content_type="text/markdown",
     )
 finally:
     if os.name in ("nt",):
         rollback_sources(module.sources)
```

### Comparing `npcolony-1.2.1/README.md` & `npcolony-1.2.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -72,9 +72,9 @@
 Colony Gateway is currently licensed under the [Apache License, Version 2.0](http://www.apache.org/licenses/).
 
 ## Build Automation
 
 [![Build Status](https://app.travis-ci.com/hivesolutions/colony-npapi.svg?branch=master)](https://travis-ci.com/github/hivesolutions/colony-npapi)
 [![Build Status GitHub](https://github.com/hivesolutions/colony-npapi/workflows/Main%20Workflow/badge.svg)](https://github.com/hivesolutions/colony-npapi/actions)
 [![Coverage Status](https://coveralls.io/repos/hivesolutions/colony-npapi/badge.svg?branch=master)](https://coveralls.io/r/hivesolutions/colony-npapi?branch=master)
-[![PyPi Status](https://img.shields.io/pypi/v/colony-npapi.svg)](https://pypi.python.org/pypi/appier)
+[![PyPi Status](https://img.shields.io/pypi/v/npcolony.svg)](https://pypi.python.org/pypi/npcolony)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://www.apache.org/licenses/)
```

### Comparing `npcolony-1.2.1/PKG-INFO` & `npcolony-1.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npcolony
-Version: 1.2.1
+Version: 1.2.4
 Summary: Colony Framework
 Home-page: http://colony_npapi.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: # [Colony Gateway (NPAPI Plugin)](http://getcolony.com)
         
@@ -80,15 +80,15 @@
         Colony Gateway is currently licensed under the [Apache License, Version 2.0](http://www.apache.org/licenses/).
         
         ## Build Automation
         
         [![Build Status](https://app.travis-ci.com/hivesolutions/colony-npapi.svg?branch=master)](https://travis-ci.com/github/hivesolutions/colony-npapi)
         [![Build Status GitHub](https://github.com/hivesolutions/colony-npapi/workflows/Main%20Workflow/badge.svg)](https://github.com/hivesolutions/colony-npapi/actions)
         [![Coverage Status](https://coveralls.io/repos/hivesolutions/colony-npapi/badge.svg?branch=master)](https://coveralls.io/r/hivesolutions/colony-npapi?branch=master)
-        [![PyPi Status](https://img.shields.io/pypi/v/colony-npapi.svg)](https://pypi.python.org/pypi/appier)
+        [![PyPi Status](https://img.shields.io/pypi/v/npcolony.svg)](https://pypi.python.org/pypi/npcolony)
         [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://www.apache.org/licenses/)
         
 Keywords: colony npapi native
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `npcolony-1.2.1/src/colony_npapi/plugin/base.c` & `npcolony-1.2.4/src/colony_npapi/plugin/base.c`

 * *Files identical despite different names*

### Comparing `npcolony-1.2.1/src/colony_npapi/plugin/python.c` & `npcolony-1.2.4/src/colony_npapi/plugin/python.c`

 * *Files identical despite different names*

### Comparing `npcolony-1.2.1/src/colony_npapi/plugin/util.c` & `npcolony-1.2.4/src/colony_npapi/plugin/util.c`

 * *Files identical despite different names*

### Comparing `npcolony-1.2.1/src/colony_npapi/system/gui_unix.c` & `npcolony-1.2.4/src/colony_npapi/system/gui_unix.c`

 * *Files identical despite different names*

### Comparing `npcolony-1.2.1/src/colony_npapi/system/gui_win32.c` & `npcolony-1.2.4/src/colony_npapi/system/gui_win32.c`

 * *Files identical despite different names*

### Comparing `npcolony-1.2.1/src/colony_npapi/print/print_unix.c` & `npcolony-1.2.4/src/colony_npapi/print/print_unix.c`

 * *Files identical despite different names*

### Comparing `npcolony-1.2.1/src/colony_npapi/print/print_win32.c` & `npcolony-1.2.4/src/colony_npapi/print/print_win32.c`

 * *Files identical despite different names*

### Comparing `npcolony-1.2.1/src/colony_npapi/stdafx.c` & `npcolony-1.2.4/src/colony_npapi/stdafx.c`

 * *Files identical despite different names*

### Comparing `npcolony-1.2.1/src/colony_npapi/encoding/base_64.c` & `npcolony-1.2.4/src/colony_npapi/encoding/base_64.c`

 * *Files identical despite different names*

### Comparing `npcolony-1.2.1/src/python/npcolony.egg-info/SOURCES.txt` & `npcolony-1.2.4/src/python/npcolony.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `npcolony-1.2.1/src/python/npcolony.egg-info/PKG-INFO` & `npcolony-1.2.4/src/python/npcolony.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npcolony
-Version: 1.2.1
+Version: 1.2.4
 Summary: Colony Framework
 Home-page: http://colony_npapi.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: # [Colony Gateway (NPAPI Plugin)](http://getcolony.com)
         
@@ -80,15 +80,15 @@
         Colony Gateway is currently licensed under the [Apache License, Version 2.0](http://www.apache.org/licenses/).
         
         ## Build Automation
         
         [![Build Status](https://app.travis-ci.com/hivesolutions/colony-npapi.svg?branch=master)](https://travis-ci.com/github/hivesolutions/colony-npapi)
         [![Build Status GitHub](https://github.com/hivesolutions/colony-npapi/workflows/Main%20Workflow/badge.svg)](https://github.com/hivesolutions/colony-npapi/actions)
         [![Coverage Status](https://coveralls.io/repos/hivesolutions/colony-npapi/badge.svg?branch=master)](https://coveralls.io/r/hivesolutions/colony-npapi?branch=master)
-        [![PyPi Status](https://img.shields.io/pypi/v/colony-npapi.svg)](https://pypi.python.org/pypi/appier)
+        [![PyPi Status](https://img.shields.io/pypi/v/npcolony.svg)](https://pypi.python.org/pypi/npcolony)
         [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://www.apache.org/licenses/)
         
 Keywords: colony npapi native
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
```

