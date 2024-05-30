# Comparing `tmp/Geode_Conversion-5.4.0rc1-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_Conversion-5.4.1rc1-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 1660052 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      171 b- defN 24-May-29 12:38 geode_conversion/__init__.py
--rw-rw-rw-  2.0 fat      178 b- defN 24-May-29 12:38 geode_conversion/model.py
--rw-rw-rw-  2.0 fat  4110336 b- defN 24-May-29 12:39 geode_conversion/bin/Geode-Conversion_model.dll
--rw-rw-rw-  2.0 fat   148480 b- defN 24-May-29 12:39 geode_conversion/bin/geode_conversion_py_model.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1993 b- defN 24-May-29 12:39 Geode_Conversion-5.4.0rc1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-May-29 12:39 Geode_Conversion-5.4.0rc1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 24-May-29 12:39 Geode_Conversion-5.4.0rc1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      743 b- defN 24-May-29 12:39 Geode_Conversion-5.4.0rc1.dist-info/RECORD
-8 files, 4262018 bytes uncompressed, 1658740 bytes compressed:  61.1%
+Zip file size: 1640031 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       67 b- defN 24-May-30 08:27 geode_conversion/__init__.py
+-rw-r--r--  2.0 unx      172 b- defN 24-May-30 08:27 geode_conversion/model.py
+-rwxr-xr-x  2.0 unx   167512 b- defN 24-May-30 08:27 geode_conversion/lib64/geode_conversion_py_model.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx  3631216 b- defN 24-May-30 08:27 geode_conversion/lib64/libGeode-Conversion_model.so
+-rw-r--r--  2.0 unx     1934 b- defN 24-May-30 08:27 Geode_Conversion-5.4.1rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx      103 b- defN 24-May-30 08:27 Geode_Conversion-5.4.1rc1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 24-May-30 08:27 Geode_Conversion-5.4.1rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      760 b- defN 24-May-30 08:27 Geode_Conversion-5.4.1rc1.dist-info/RECORD
+8 files, 3801781 bytes uncompressed, 1638683 bytes compressed:  56.9%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: geode_conversion/__init__.py
 Comment: 
 
 Filename: geode_conversion/model.py
 Comment: 
 
-Filename: geode_conversion/bin/Geode-Conversion_model.dll
+Filename: geode_conversion/lib64/geode_conversion_py_model.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: geode_conversion/bin/geode_conversion_py_model.cp39-win_amd64.pyd
+Filename: geode_conversion/lib64/libGeode-Conversion_model.so
 Comment: 
 
-Filename: Geode_Conversion-5.4.0rc1.dist-info/METADATA
+Filename: Geode_Conversion-5.4.1rc1.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Conversion-5.4.0rc1.dist-info/WHEEL
+Filename: Geode_Conversion-5.4.1rc1.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_Conversion-5.4.0rc1.dist-info/top_level.txt
+Filename: Geode_Conversion-5.4.1rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_Conversion-5.4.0rc1.dist-info/RECORD
+Filename: Geode_Conversion-5.4.1rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_conversion/__init__.py

```diff
@@ -1,6 +1,3 @@
-## Copyright (c) 2019 - 2024 Geode-solutions
-
-import os, pathlib
-os.add_dll_directory(pathlib.Path(__file__).parent.resolve().joinpath('bin'))
-
-from .model import *
+## Copyright (c) 2019 - 2024 Geode-solutions
+
+from .model import *
```

## geode_conversion/model.py

```diff
@@ -1,8 +1,8 @@
-#
-# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-
-from .bin.geode_conversion_py_model import *
-ConversionModelLibrary.initialize()
+#
+# Copyright (c) 2019 - 2024 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+
+from .lib64.geode_conversion_py_model import *
+ConversionModelLibrary.initialize()
```

## Comparing `Geode_Conversion-5.4.0rc1.dist-info/METADATA` & `Geode_Conversion-5.4.1rc1.dist-info/METADATA`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-Metadata-Version: 2.1
-Name: Geode-Conversion
-Version: 5.4.0rc1
-Summary: Conversion module for Geode-solutions OpenGeode modules
-Home-page: https://github.com/Geode-solutions/Geode-Conversion
-Author: Geode-solutions
-Author-email: contact@geode-solutions.com
-License: Proprietary
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-Requires-Dist: opengeode-core ==14.*,>=14.21.0
-
-<h1 align="center">Geode-Conversion<sup><i>by Geode-solutions</i></sup></h1>
-<h3 align="center">Conversion OpenGeode module</h3>
-
-<p align="center">
-  <img src="https://github.com/Geode-solutions/Geode-Conversion_private/workflows/CI/badge.svg" alt="Build Status">
-  <img src="https://github.com/Geode-solutions/Geode-Conversion_private/workflows/CD/badge.svg" alt="Deploy Status">
-  <img src="https://codecov.io/gh/Geode-solutions/Geode-Conversion_private/branch/master/graph/badge.svg" alt="Coverage Status">
-  <img src="https://img.shields.io/github/release/Geode-solutions/Geode-Conversion_private.svg" alt="Version">
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
+Name: Geode-Conversion
+Version: 5.4.1rc1
+Summary: Conversion module for Geode-solutions OpenGeode modules
+Home-page: https://github.com/Geode-solutions/Geode-Conversion
+Author: Geode-solutions
+Author-email: contact@geode-solutions.com
+License: Proprietary
+Description-Content-Type: text/markdown
+Requires-Dist: opengeode-core ==14.*,>=14.21.1
+
+<h1 align="center">Geode-Conversion<sup><i>by Geode-solutions</i></sup></h1>
+<h3 align="center">Conversion OpenGeode module</h3>
+
+<p align="center">
+  <img src="https://github.com/Geode-solutions/Geode-Conversion_private/workflows/CI/badge.svg" alt="Build Status">
+  <img src="https://github.com/Geode-solutions/Geode-Conversion_private/workflows/CD/badge.svg" alt="Deploy Status">
+  <img src="https://codecov.io/gh/Geode-solutions/Geode-Conversion_private/branch/master/graph/badge.svg" alt="Coverage Status">
+  <img src="https://img.shields.io/github/release/Geode-solutions/Geode-Conversion_private.svg" alt="Version">
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
@@ -1,12 +1,11 @@
-Metadata-Version: 2.1 Name: Geode-Conversion Version: 5.4.0rc1 Summary:
+Metadata-Version: 2.1 Name: Geode-Conversion Version: 5.4.1rc1 Summary:
 Conversion module for Geode-solutions OpenGeode modules Home-page: https://
 github.com/Geode-solutions/Geode-Conversion Author: Geode-solutions Author-
-email: contact@geode-solutions.com License: Proprietary Platform: UNKNOWN
-Description-Content-Type: text/markdown Requires-Dist: opengeode-core
-==14.*,>=14.21.0
+email: contact@geode-solutions.com License: Proprietary Description-Content-
+Type: text/markdown Requires-Dist: opengeode-core ==14.*,>=14.21.1
                ************ GGeeooddee--CCoonnvveerrssiioonnbbyy GGeeooddee--ssoolluuttiioonnss ************
                      ******** CCoonnvveerrssiioonn OOppeennGGeeooddee mmoodduullee ********
             [Build Status][Deploy Status][Coverage Status][Version]
               [Windows support][Ubuntu support][Red Hat support]
  [Language][License][Semantic-release]_[_S_l_a_c_k_ _i_n_v_i_t_e_]Copyright (c) 2019 - 2024,
                                 Geode-solutions
```

## Comparing `Geode_Conversion-5.4.0rc1.dist-info/RECORD` & `Geode_Conversion-5.4.1rc1.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-geode_conversion/__init__.py,sha256=K2g9LCrqwB6gfE3Ca5Ia_5Q8csgvLJwn6uiVylAsCsA,171
-geode_conversion/model.py,sha256=kPyg0FrL-HSROjMRnY025-loYYW-S1CTSoEcOZXw4mE,178
-geode_conversion/bin/Geode-Conversion_model.dll,sha256=fWRLnaXCeobPGaYBMYtrbHoib5wbi90DsuuWAtHfBUE,4110336
-geode_conversion/bin/geode_conversion_py_model.cp39-win_amd64.pyd,sha256=plPduj86doRTDhTE0fiOnEILluw10OfPPi-2CuIBxR4,148480
-Geode_Conversion-5.4.0rc1.dist-info/METADATA,sha256=mUsW7fYvs4syHfDxFwbjXTUSp9zpPNKGvqFaP_N5cqk,1993
-Geode_Conversion-5.4.0rc1.dist-info/WHEEL,sha256=Z6c-bE0pUM47a70GvqO_SvH_XXU0lm62gEAKtoNJ08A,100
-Geode_Conversion-5.4.0rc1.dist-info/top_level.txt,sha256=PnM_M6Sy8psC1M_rMpCs6FAGjv7uyDWsRvR46jFUpXU,17
-Geode_Conversion-5.4.0rc1.dist-info/RECORD,,
+geode_conversion/__init__.py,sha256=RsV8awSP62XSZuP8SaKhurf1Ki8I8CcqjKJ7adwFlAk,67
+geode_conversion/model.py,sha256=dhs7dRZ8whMnYqmgnwh6CFb8VJY4z156djRZ8DVEftI,172
+geode_conversion/lib64/geode_conversion_py_model.cpython-39-x86_64-linux-gnu.so,sha256=dVQHIC3eXOaeTcfAWFdAWNOViwflh1wSidRpwXnk2jY,167512
+geode_conversion/lib64/libGeode-Conversion_model.so,sha256=_BJd0d51_I1SURuip_YZhaztw3s6G9B52uysLh8-X_0,3631216
+Geode_Conversion-5.4.1rc1.dist-info/METADATA,sha256=8OTEE0Ng7V48Jxo1Tt1o1VSwGTd1-YrKqhKmZLrMQEs,1934
+Geode_Conversion-5.4.1rc1.dist-info/WHEEL,sha256=cPiEulY4lHJMdGCxx29HxfDkwhV9C6172sJgZUA9dSs,103
+Geode_Conversion-5.4.1rc1.dist-info/top_level.txt,sha256=PnM_M6Sy8psC1M_rMpCs6FAGjv7uyDWsRvR46jFUpXU,17
+Geode_Conversion-5.4.1rc1.dist-info/RECORD,,
```

