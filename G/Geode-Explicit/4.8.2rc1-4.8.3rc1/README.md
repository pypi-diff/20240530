# Comparing `tmp/Geode_Explicit-4.8.2rc1-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_Explicit-4.8.3rc1-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 3141707 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat      194 b- defN 24-May-28 05:07 geode_explicit/__init__.py
--rw-rw-rw-  2.0 fat      271 b- defN 24-May-28 05:07 geode_explicit/brep.py
--rw-rw-rw-  2.0 fat      249 b- defN 24-May-28 05:07 geode_explicit/section.py
--rw-rw-rw-  2.0 fat  4034560 b- defN 24-May-28 05:07 geode_explicit/bin/Geode-Explicit_brep.dll
--rw-rw-rw-  2.0 fat    33792 b- defN 24-May-28 05:07 geode_explicit/bin/Geode-Explicit_common.dll
--rw-rw-rw-  2.0 fat  3715072 b- defN 24-May-28 05:07 geode_explicit/bin/Geode-Explicit_section.dll
--rw-rw-rw-  2.0 fat   147456 b- defN 24-May-28 05:07 geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   135680 b- defN 24-May-28 05:07 geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2215 b- defN 24-May-28 05:07 Geode_Explicit-4.8.2rc1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-May-28 05:07 Geode_Explicit-4.8.2rc1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 24-May-28 05:07 Geode_Explicit-4.8.2rc1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1130 b- defN 24-May-28 05:07 Geode_Explicit-4.8.2rc1.dist-info/RECORD
-12 files, 8070734 bytes uncompressed, 3139783 bytes compressed:  61.1%
+Zip file size: 372030 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       89 b- defN 24-May-30 08:37 geode_explicit/__init__.py
+-rw-r--r--  2.0 unx      261 b- defN 24-May-30 08:37 geode_explicit/brep.py
+-rw-r--r--  2.0 unx      240 b- defN 24-May-30 08:37 geode_explicit/section.py
+-rwxr-xr-x  2.0 unx   159296 b- defN 24-May-30 08:37 geode_explicit/lib64/geode_explicit_py_brep.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx   138752 b- defN 24-May-30 08:37 geode_explicit/lib64/geode_explicit_py_section.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx   504832 b- defN 24-May-30 08:37 geode_explicit/lib64/libGeode-Explicit_brep.so
+-rwxr-xr-x  2.0 unx    35352 b- defN 24-May-30 08:37 geode_explicit/lib64/libGeode-Explicit_common.so
+-rwxr-xr-x  2.0 unx    77016 b- defN 24-May-30 08:37 geode_explicit/lib64/libGeode-Explicit_section.so
+-rw-r--r--  2.0 unx     2155 b- defN 24-May-30 08:37 Geode_Explicit-4.8.3rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx      103 b- defN 24-May-30 08:37 Geode_Explicit-4.8.3rc1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 24-May-30 08:37 Geode_Explicit-4.8.3rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1166 b- defN 24-May-30 08:37 Geode_Explicit-4.8.3rc1.dist-info/RECORD
+12 files, 919277 bytes uncompressed, 370026 bytes compressed:  59.7%
```

## zipnote {}

```diff
@@ -3,35 +3,35 @@
 
 Filename: geode_explicit/brep.py
 Comment: 
 
 Filename: geode_explicit/section.py
 Comment: 
 
-Filename: geode_explicit/bin/Geode-Explicit_brep.dll
+Filename: geode_explicit/lib64/geode_explicit_py_brep.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: geode_explicit/bin/Geode-Explicit_common.dll
+Filename: geode_explicit/lib64/geode_explicit_py_section.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: geode_explicit/bin/Geode-Explicit_section.dll
+Filename: geode_explicit/lib64/libGeode-Explicit_brep.so
 Comment: 
 
-Filename: geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd
+Filename: geode_explicit/lib64/libGeode-Explicit_common.so
 Comment: 
 
-Filename: geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd
+Filename: geode_explicit/lib64/libGeode-Explicit_section.so
 Comment: 
 
-Filename: Geode_Explicit-4.8.2rc1.dist-info/METADATA
+Filename: Geode_Explicit-4.8.3rc1.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Explicit-4.8.2rc1.dist-info/WHEEL
+Filename: Geode_Explicit-4.8.3rc1.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_Explicit-4.8.2rc1.dist-info/top_level.txt
+Filename: Geode_Explicit-4.8.3rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_Explicit-4.8.2rc1.dist-info/RECORD
+Filename: Geode_Explicit-4.8.3rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_explicit/__init__.py

```diff
@@ -1,7 +1,4 @@
-## Copyright (c) 2019 - 2024 Geode-solutions
-
-import os, pathlib
-os.add_dll_directory(pathlib.Path(__file__).parent.resolve().joinpath('bin'))
-
-from .section import *
-from .brep import *
+## Copyright (c) 2019 - 2024 Geode-solutions
+
+from .section import *
+from .brep import *
```

## geode_explicit/brep.py

```diff
@@ -1,12 +1,12 @@
-#
-# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-import opengeode_inspector
-import geode_common
-import geode_conversion
-import geode_background
-
-from .bin.geode_explicit_py_brep import *
-ExplicitBRepLibrary.initialize()
+#
+# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+import opengeode_inspector
+import geode_common
+import geode_conversion
+import geode_background
+
+from .lib64.geode_explicit_py_brep import *
+ExplicitBRepLibrary.initialize()
```

## geode_explicit/section.py

```diff
@@ -1,11 +1,11 @@
-#
-# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-import geode_common
-import geode_conversion
-import geode_background
-
-from .bin.geode_explicit_py_section import *
-ExplicitSectionLibrary.initialize()
+#
+# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+import geode_common
+import geode_conversion
+import geode_background
+
+from .lib64.geode_explicit_py_section import *
+ExplicitSectionLibrary.initialize()
```

## Comparing `Geode_Explicit-4.8.2rc1.dist-info/METADATA` & `Geode_Explicit-4.8.3rc1.dist-info/METADATA`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,40 @@
-Metadata-Version: 2.1
-Name: Geode-Explicit
-Version: 4.8.2rc1
-Summary: Geode-solutions OpenGeode module for building explicit models
-Home-page: https://github.com/Geode-solutions/Geode-Explicit
-Author: Geode-solutions
-Author-email: contact@geode-solutions.com
-License: Proprietary
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-Requires-Dist: geode-background ==7.*,>=7.10.1
-Requires-Dist: geode-common ==31.*,>=31.1.0
-Requires-Dist: geode-conversion ==5.*,>=5.3.1rc1
-Requires-Dist: opengeode-core ==14.*,>=14.20.1rc1
-Requires-Dist: opengeode-inspector ==5.*,>=5.1.4
-
-<h1 align="center">Geode-Explicit<sup><i>by Geode-solutions</i></sup></h1>
-<h3 align="center">Geode-solutions OpenGeode module for building explicit models</h3>
-
-<p align="center">
-  <img src="https://github.com/Geode-solutions/Geode-Explicit_private/workflows/CI/badge.svg" alt="Build Status">
-  <img src="https://github.com/Geode-solutions/Geode-Explicit_private/workflows/CD/badge.svg" alt="Deploy Status">
-  <img src="https://codecov.io/gh/Geode-solutions/Geode-Explicit_private/branch/master/graph/badge.svg" alt="Coverage Status">
-  <img src="https://img.shields.io/github/release/Geode-solutions/Geode-Explicit_private.svg" alt="Version">
-</p>
-
-<p align="center">
-  <img src="https://img.shields.io/static/v1?label=Windows&logo=windows&logoColor=white&message=support&color=success" alt="Windows support">
-  <img src="https://img.shields.io/static/v1?label=Ubuntu&logo=Ubuntu&logoColor=white&message=support&color=success" alt="Ubuntu support">
-  <img src="https://img.shields.io/static/v1?label=Red%20Hat&logo=Red-Hat&logoColor=white&message=support&color=success" alt="Red Hat support">
-</p>
-
-<p align="center">
-  <img src="https://img.shields.io/badge/C%2B%2B-11-blue.svg" alt="Language">
-  <img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License">
-  <img src="https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg" alt="Semantic-release">
-  <a href="https://geode-solutions.com/#slack">
-    <img src="https://opengeode-slack-invite.herokuapp.com/badge.svg" alt="Slack invite">
-  </a>
-
-Copyright (c) 2019 - 2024, Geode-solutions
-
-
+Metadata-Version: 2.1
+Name: Geode-Explicit
+Version: 4.8.3rc1
+Summary: Geode-solutions OpenGeode module for building explicit models
+Home-page: https://github.com/Geode-solutions/Geode-Explicit
+Author: Geode-solutions
+Author-email: contact@geode-solutions.com
+License: Proprietary
+Description-Content-Type: text/markdown
+Requires-Dist: geode-background ==7.*,>=7.11.0rc1
+Requires-Dist: geode-common ==31.*,>=31.2.0rc1
+Requires-Dist: geode-conversion ==5.*,>=5.4.1rc1
+Requires-Dist: opengeode-core ==14.*,>=14.21.1
+Requires-Dist: opengeode-inspector ==5.*,>=5.1.4
+
+<h1 align="center">Geode-Explicit<sup><i>by Geode-solutions</i></sup></h1>
+<h3 align="center">Geode-solutions OpenGeode module for building explicit models</h3>
+
+<p align="center">
+  <img src="https://github.com/Geode-solutions/Geode-Explicit_private/workflows/CI/badge.svg" alt="Build Status">
+  <img src="https://github.com/Geode-solutions/Geode-Explicit_private/workflows/CD/badge.svg" alt="Deploy Status">
+  <img src="https://codecov.io/gh/Geode-solutions/Geode-Explicit_private/branch/master/graph/badge.svg" alt="Coverage Status">
+  <img src="https://img.shields.io/github/release/Geode-solutions/Geode-Explicit_private.svg" alt="Version">
+</p>
+
+<p align="center">
+  <img src="https://img.shields.io/static/v1?label=Windows&logo=windows&logoColor=white&message=support&color=success" alt="Windows support">
+  <img src="https://img.shields.io/static/v1?label=Ubuntu&logo=Ubuntu&logoColor=white&message=support&color=success" alt="Ubuntu support">
+  <img src="https://img.shields.io/static/v1?label=Red%20Hat&logo=Red-Hat&logoColor=white&message=support&color=success" alt="Red Hat support">
+</p>
+
+<p align="center">
+  <img src="https://img.shields.io/badge/C%2B%2B-11-blue.svg" alt="Language">
+  <img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License">
+  <img src="https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg" alt="Semantic-release">
+  <a href="https://geode-solutions.com/#slack">
+    <img src="https://opengeode-slack-invite.herokuapp.com/badge.svg" alt="Slack invite">
+  </a>
+
+Copyright (c) 2019 - 2024, Geode-solutions
```

### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: Geode-Explicit Version: 4.8.2rc1 Summary: Geode-
+Metadata-Version: 2.1 Name: Geode-Explicit Version: 4.8.3rc1 Summary: Geode-
 solutions OpenGeode module for building explicit models Home-page: https://
 github.com/Geode-solutions/Geode-Explicit Author: Geode-solutions Author-email:
-contact@geode-solutions.com License: Proprietary Platform: UNKNOWN Description-
-Content-Type: text/markdown Requires-Dist: geode-background ==7.*,>=7.10.1
-Requires-Dist: geode-common ==31.*,>=31.1.0 Requires-Dist: geode-conversion
-==5.*,>=5.3.1rc1 Requires-Dist: opengeode-core ==14.*,>=14.20.1rc1 Requires-
-Dist: opengeode-inspector ==5.*,>=5.1.4
+contact@geode-solutions.com License: Proprietary Description-Content-Type:
+text/markdown Requires-Dist: geode-background ==7.*,>=7.11.0rc1 Requires-Dist:
+geode-common ==31.*,>=31.2.0rc1 Requires-Dist: geode-conversion
+==5.*,>=5.4.1rc1 Requires-Dist: opengeode-core ==14.*,>=14.21.1 Requires-Dist:
+opengeode-inspector ==5.*,>=5.1.4
                 ************ GGeeooddee--EExxpplliicciittbbyy GGeeooddee--ssoolluuttiioonnss ************
     ******** GGeeooddee--ssoolluuttiioonnss OOppeennGGeeooddee mmoodduullee ffoorr bbuuiillddiinngg eexxpplliicciitt mmooddeellss ********
             [Build Status][Deploy Status][Coverage Status][Version]
               [Windows support][Ubuntu support][Red Hat support]
  [Language][License][Semantic-release]_[_S_l_a_c_k_ _i_n_v_i_t_e_]Copyright (c) 2019 - 2024,
                                 Geode-solutions
```

