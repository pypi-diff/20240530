# Comparing `tmp/PolyMesher-1.0.0-py3-none-any.whl.zip` & `tmp/PolyMesher-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 31427 bytes, number of entries: 12
--rw-rw-r--  2.0 unx       62 b- defN 23-Dec-29 23:40 pyPolyMesher/__init__.py
+Zip file size: 31394 bytes, number of entries: 12
+-rw-rw-r--  2.0 unx       62 b- defN 24-May-29 20:36 pyPolyMesher/__init__.py
 -rw-rw-r--  2.0 unx    10395 b- defN 24-May-29 18:54 pyPolyMesher/dFunctions.py
 -rw-rw-r--  2.0 unx     1777 b- defN 23-Dec-29 23:22 pyPolyMesher/dxfImporter.py
 -rw-rw-r--  2.0 unx     5838 b- defN 24-Apr-20 20:18 pyPolyMesher/exampleDomains.py
 -rw-rw-r--  2.0 unx     5902 b- defN 23-Nov-06 21:49 pyPolyMesher/pyExampleDomains.py
 -rw-rw-r--  2.0 unx    20647 b- defN 24-May-29 17:28 pyPolyMesher/pyPolyMesher.py
 -rw-rw-r--  2.0 unx     5218 b- defN 23-Oct-30 21:10 pyPolyMesher/pydFunctions.py
--rw-rw-r--  2.0 unx    35149 b- defN 24-May-29 20:14 PolyMesher-1.0.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx     9822 b- defN 24-May-29 20:14 PolyMesher-1.0.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-May-29 20:14 PolyMesher-1.0.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       13 b- defN 24-May-29 20:14 PolyMesher-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      996 b- defN 24-May-29 20:14 PolyMesher-1.0.0.dist-info/RECORD
-12 files, 95911 bytes uncompressed, 29755 bytes compressed:  69.0%
+-rw-rw-r--  2.0 unx    35149 b- defN 24-May-30 17:11 PolyMesher-1.0.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     9750 b- defN 24-May-30 17:11 PolyMesher-1.0.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-30 17:11 PolyMesher-1.0.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       13 b- defN 24-May-30 17:11 PolyMesher-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      996 b- defN 24-May-30 17:11 PolyMesher-1.0.1.dist-info/RECORD
+12 files, 95839 bytes uncompressed, 29722 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: pyPolyMesher/pyPolyMesher.py
 Comment: 
 
 Filename: pyPolyMesher/pydFunctions.py
 Comment: 
 
-Filename: PolyMesher-1.0.0.dist-info/LICENSE
+Filename: PolyMesher-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: PolyMesher-1.0.0.dist-info/METADATA
+Filename: PolyMesher-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: PolyMesher-1.0.0.dist-info/WHEEL
+Filename: PolyMesher-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: PolyMesher-1.0.0.dist-info/top_level.txt
+Filename: PolyMesher-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: PolyMesher-1.0.0.dist-info/RECORD
+Filename: PolyMesher-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `PolyMesher-1.0.0.dist-info/LICENSE` & `PolyMesher-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `PolyMesher-1.0.0.dist-info/METADATA` & `PolyMesher-1.0.1.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PolyMesher
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package for polygonal mesh generation
 Home-page: https://github.com/Sad-Abd/pyPolyMesher
 Author: Sad-Abd
 Author-email: abedisadjad@gmail.com
 License: GPL-3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
@@ -115,25 +115,20 @@
 <!-- GETTING STARTED -->
 ## Getting Started
 
 This part explains how to install and use this package.
 
 ### Installation
 
-Since pyPolyMesher is not published on PyPI [_yet_], you need to clone the repository:
-
+You can install this package using pip:
 ```
-git clone https://github.com/Sad-Abd/pyPolyMesher.git
+pip install PolyMesher
 ```
 
-Then install it using pip:
-
-```
-pip install ./pyPolyMesher
-```
+Please note that `pyPolyMesher` is published as `PolyMesher` on PYPI.
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 <!-- USAGE EXAMPLES -->
 ## Usage
 
 ### Basic Usage:
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PolyMesher Version: 1.0.0 Summary: A Python package
+Metadata-Version: 2.1 Name: PolyMesher Version: 1.0.1 Summary: A Python package
 for polygonal mesh generation Home-page: https://github.com/Sad-Abd/
 pyPolyMesher Author: Sad-Abd Author-email: abedisadjad@gmail.com License: GPL-
 3.0 Classifier: Programming Language :: Python :: 3 Classifier: Intended
 Audience :: Science/Research Classifier: Topic :: Scientific/Engineering ::
 Mathematics Classifier: Topic :: Scientific/Engineering Classifier: License ::
 OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
@@ -54,17 +54,16 @@
 useful for simulations and analysis. The package provides Lloyd's algorithm for
 efficient and robust meshing of arbitrary SDF-based domains. Researchers can
 conveniently translate geometric constructs and concepts into code using the
 SDF formalism. Overall, pyPolyMesher simplifies the entire workflow - from
 domain specification to quality mesh generation to numerical analysis.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Getting Started This part explains how to install and use this package. ###
-Installation Since pyPolyMesher is not published on PyPI [_yet_], you need to
-clone the repository: ``` git clone https://github.com/Sad-Abd/pyPolyMesher.git
-``` Then install it using pip: ``` pip install ./pyPolyMesher ```
+Installation You can install this package using pip: ``` pip install PolyMesher
+``` Please note that `pyPolyMesher` is published as `PolyMesher` on PYPI.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Usage ### Basic Usage: `pyPolyMesher.PolyMesherPolyMesher(Domain, NElem,
 MaxIter, P=None, anim=False)`: Generate polygon mesh on `Domain` with `NElem`
 number of elements. Improve mesh for `MaxIter` iterations. Can be given an
 initial point set `P`. ```python import pyPolyMesher from
 pyPolyMesher.exampleDomains import MichellDomain MichellDomain.Plot() Node,
 Element, Supp, Load, P = pyPolyMesher.PolyMesher(MichellDomain, 50, 100) ```
```

## Comparing `PolyMesher-1.0.0.dist-info/RECORD` & `PolyMesher-1.0.1.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 pyPolyMesher/__init__.py,sha256=ieduVKAciqPToSjBljcnJiFogqptUAIoO3FCc36cpvg,62
 pyPolyMesher/dFunctions.py,sha256=h_YnEcHsxsx9HqyUoM08eowWVdrlyCDg-EX76KjMWvo,10395
 pyPolyMesher/dxfImporter.py,sha256=SNNUzfxwkug6b6DVHUfHeruh6Q7YiAgmW_-vpi0eAVA,1777
 pyPolyMesher/exampleDomains.py,sha256=WtTlGl3TJ7IBaWhZWNdAEUsulpr7hU5i3sHALY382fI,5838
 pyPolyMesher/pyExampleDomains.py,sha256=nRpaV_pJxYVl1eOCDbo_0y8nkk7V8sjCa4OBG2bFNgQ,5902
 pyPolyMesher/pyPolyMesher.py,sha256=yU1rRvr92VvJ71RjEIRBuwNGIyAmZgWBYzRXJ_BsZDI,20647
 pyPolyMesher/pydFunctions.py,sha256=n9ZiD9WHkDYjulquBKphqmlKDc3lxZYuw6q39i9DeFc,5218
-PolyMesher-1.0.0.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-PolyMesher-1.0.0.dist-info/METADATA,sha256=hIeYB00rGs1WO2M13VKtC58WfEMvW0_D-23m1nbhqsQ,9822
-PolyMesher-1.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-PolyMesher-1.0.0.dist-info/top_level.txt,sha256=b3gtaB8eWeKu9GI8JBfpOWCGfYtVxS-oDAKG1hTxcpY,13
-PolyMesher-1.0.0.dist-info/RECORD,,
+PolyMesher-1.0.1.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+PolyMesher-1.0.1.dist-info/METADATA,sha256=1g5s3SLXAb4AFKEiwh6G7AgtDIvA69Xat6SmGZPFotM,9750
+PolyMesher-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+PolyMesher-1.0.1.dist-info/top_level.txt,sha256=b3gtaB8eWeKu9GI8JBfpOWCGfYtVxS-oDAKG1hTxcpY,13
+PolyMesher-1.0.1.dist-info/RECORD,,
```

