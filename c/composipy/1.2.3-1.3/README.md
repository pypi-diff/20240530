# Comparing `tmp/composipy-1.2.3.tar.gz` & `tmp/composipy-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composipy-1.2.3.tar", last modified: Sat Jan 27 18:37:55 2024, max compression
+gzip compressed data, was "composipy-1.3.tar", last modified: Thu May 30 17:29:10 2024, max compression
```

## Comparing `composipy-1.2.3.tar` & `composipy-1.3.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 18:37:55.271024 composipy-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-01-27 18:37:35.000000 composipy-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-01-27 18:37:55.271024 composipy-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-01-27 18:37:35.000000 composipy-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 18:37:55.263024 composipy-1.2.3/composipy/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-01-27 18:37:35.000000 composipy-1.2.3/composipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 18:37:55.263024 composipy-1.2.3/composipy/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 18:37:35.000000 composipy-1.2.3/composipy/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8962 2024-01-27 18:37:35.000000 composipy-1.2.3/composipy/core/material.py
--rw-r--r--   0 runner    (1001) docker     (127)     9147 2024-01-27 18:37:35.000000 composipy-1.2.3/composipy/core/property.py
--rw-r--r--   0 runner    (1001) docker     (127)    12849 2024-01-27 18:37:35.000000 composipy-1.2.3/composipy/core/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 18:37:55.263024 composipy-1.2.3/composipy/nastranapi/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-01-27 18:37:35.000000 composipy-1.2.3/composipy/nastranapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6123 2024-01-27 18:37:35.000000 composipy-1.2.3/composipy/nastranapi/pcomp_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 18:37:55.263024 composipy-1.2.3/composipy/optimize/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-01-27 18:37:35.000000 composipy-1.2.3/composipy/optimize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-01-27 18:37:35.000000 composipy-1.2.3/composipy/optimize/_maximize_buckling.py
--rw-r--r--   0 runner    (1001) docker     (127)     6088 2024-01-27 18:37:35.000000 composipy-1.2.3/composipy/optimize/_minimize_panel_weight.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 18:37:55.267024 composipy-1.2.3/composipy/pre_integrated_component/
--rw-r--r--   0 runner    (1001) docker     (127)  2267905 2024-01-27 18:37:35.000000 composipy-1.2.3/composipy/pre_integrated_component/_S.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 18:37:35.000000 composipy-1.2.3/composipy/pre_integrated_component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   113898 2024-01-27 18:37:35.000000 composipy-1.2.3/composipy/pre_integrated_component/_ii_F.py
--rw-r--r--   0 runner    (1001) docker     (127)     6183 2024-01-27 18:37:35.000000 composipy-1.2.3/composipy/pre_integrated_component/build_k.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-01-27 18:37:35.000000 composipy-1.2.3/composipy/pre_integrated_component/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-01-27 18:37:35.000000 composipy-1.2.3/composipy/pre_integrated_component/write_pre_integrated_terms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-01-27 18:37:35.000000 composipy-1.2.3/composipy/pre_integrated_component/write_shape_function.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 18:37:55.267024 composipy-1.2.3/composipy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-27 18:37:35.000000 composipy-1.2.3/composipy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-01-27 18:37:35.000000 composipy-1.2.3/composipy/utils/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-27 18:37:35.000000 composipy-1.2.3/composipy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 18:37:55.271024 composipy-1.2.3/composipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-01-27 18:37:55.000000 composipy-1.2.3/composipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-01-27 18:37:55.000000 composipy-1.2.3/composipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-27 18:37:55.000000 composipy-1.2.3/composipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-27 18:37:55.000000 composipy-1.2.3/composipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-27 18:37:55.000000 composipy-1.2.3/composipy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-01-27 18:37:35.000000 composipy-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-27 18:37:55.271024 composipy-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-01-27 18:37:35.000000 composipy-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 18:37:55.271024 composipy-1.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-01-27 18:37:35.000000 composipy-1.2.3/tests/test_ABD.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-01-27 18:37:35.000000 composipy-1.2.3/tests/test_Material_Q0.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-01-27 18:37:35.000000 composipy-1.2.3/tests/test_lamination_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-01-27 18:37:35.000000 composipy-1.2.3/tests/test_plate_buckling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-01-27 18:37:35.000000 composipy-1.2.3/tests/test_plate_buckling_LP.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:29:10.480925 composipy-1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-30 17:28:53.000000 composipy-1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-05-30 17:29:10.480925 composipy-1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-05-30 17:28:53.000000 composipy-1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:29:10.472926 composipy-1.3/composipy/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-30 17:28:53.000000 composipy-1.3/composipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:29:10.472926 composipy-1.3/composipy/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 17:28:53.000000 composipy-1.3/composipy/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8962 2024-05-30 17:28:53.000000 composipy-1.3/composipy/core/material.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9147 2024-05-30 17:28:53.000000 composipy-1.3/composipy/core/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12849 2024-05-30 17:28:53.000000 composipy-1.3/composipy/core/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:29:10.476925 composipy-1.3/composipy/nastranapi/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-30 17:28:53.000000 composipy-1.3/composipy/nastranapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6123 2024-05-30 17:28:53.000000 composipy-1.3/composipy/nastranapi/pcomp_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:29:10.476925 composipy-1.3/composipy/optimize/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-30 17:28:53.000000 composipy-1.3/composipy/optimize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-05-30 17:28:53.000000 composipy-1.3/composipy/optimize/_maximize_buckling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-05-30 17:28:53.000000 composipy-1.3/composipy/optimize/_minimize_panel_weight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-05-30 17:28:53.000000 composipy-1.3/composipy/optimize/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:29:10.480925 composipy-1.3/composipy/pre_integrated_component/
+-rw-r--r--   0 runner    (1001) docker     (127)  2267905 2024-05-30 17:28:53.000000 composipy-1.3/composipy/pre_integrated_component/_S.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 17:28:53.000000 composipy-1.3/composipy/pre_integrated_component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   113898 2024-05-30 17:28:53.000000 composipy-1.3/composipy/pre_integrated_component/_ii_F.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6183 2024-05-30 17:28:53.000000 composipy-1.3/composipy/pre_integrated_component/build_k.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-30 17:28:53.000000 composipy-1.3/composipy/pre_integrated_component/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-05-30 17:28:53.000000 composipy-1.3/composipy/pre_integrated_component/write_pre_integrated_terms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-30 17:28:53.000000 composipy-1.3/composipy/pre_integrated_component/write_shape_function.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:29:10.480925 composipy-1.3/composipy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-30 17:28:53.000000 composipy-1.3/composipy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-30 17:28:53.000000 composipy-1.3/composipy/utils/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-30 17:28:53.000000 composipy-1.3/composipy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:29:10.480925 composipy-1.3/composipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-05-30 17:29:10.000000 composipy-1.3/composipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-30 17:29:10.000000 composipy-1.3/composipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 17:29:10.000000 composipy-1.3/composipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 17:29:10.000000 composipy-1.3/composipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 17:29:10.000000 composipy-1.3/composipy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-30 17:28:53.000000 composipy-1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 17:29:10.480925 composipy-1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-30 17:28:53.000000 composipy-1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:29:10.480925 composipy-1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-30 17:28:53.000000 composipy-1.3/tests/test_ABD.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-30 17:28:53.000000 composipy-1.3/tests/test_Material_Q0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-30 17:28:53.000000 composipy-1.3/tests/test_lamination_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-30 17:28:53.000000 composipy-1.3/tests/test_plate_buckling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-30 17:28:53.000000 composipy-1.3/tests/test_plate_buckling_LP.py
```

### Comparing `composipy-1.2.3/LICENSE` & `composipy-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `composipy-1.2.3/PKG-INFO` & `composipy-1.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,21 @@
-Metadata-Version: 2.1
-Name: composipy
-Version: 1.2.3
-Summary: This package intends to perform composite material calculations
-Home-page: https://github.com/rafaelpsilva07/composipy
-Author: Rafael Pereira
-Author-email: rafaelpsilva07@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: scipy
-Requires-Dist: matplotlib
-
 [![Downloads](https://static.pepy.tech/badge/composipy)](https://pepy.tech/project/composipy)
-[![Deploy](https://github.com/rafaelpsilva07/composipy/actions/workflows/python-publish.yml\badge.svg)](https://github.com/rafaelpsilva07/composipy/actions/workflows/python-publish.yml)
+[![Deploy](https://github.com/rafaelpsilva07/composipy/actions/workflows/python-publish.yml/badge.svg)](https://github.com/rafaelpsilva07/composipy/actions/workflows/python-publish.yml)
 [![Test](https://github.com/rafaelpsilva07/composipy/actions/workflows/pytest_test.yml/badge.svg)](https://github.com/rafaelpsilva07/composipy/actions/workflows/pytest_test.yml)
 ![PyPI](https://img.shields.io/pypi/v/composipy)
+[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rafael-pereira-da-silva07/)
+[![Youtube](https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=W4foqYR8IL0&t=622s&ab_channel=EngenhariaRefinada)
 [![DOI](https://zenodo.org/badge/332543985.svg)](https://zenodo.org/badge/latestdoi/332543985)
 
 
 # Composipy
 
 ## What it is
 
-**composipy** is a python library to calculate composite plates using the classical laminate theory. This library is designed to be simple, userfriendly and helpfull.
+Composipy is a Python-based library designed to address the challenges of composite plate analysis and optimization in the aerospace industry, where weight reduction is crucial for efficient and profitable aircraft design. The library offers tools for plate buckling analysis and lamination parameter optimization, empowering engineers to streamline the design process and enhance structural performance. Utilizing object-oriented programming and native Python structures, Composipy ensures a seamless workflow and easy integration into existing engineering practices. Through continuous integration and delivery practices, Composipy maintains reliability and efficiency. 
 
 Composipy is able to perform buckling calculation considering different boundary conditions and in-plane load applications. See [Examples](https://rafaelpsilva07.github.io/composipy/notebooks/Examples_BCs.html).
 
 
 <img src="https://github.com/rafaelpsilva07/composipy/blob/main/doc/images/load_bcs_examples.PNG" width="700">
 
 
@@ -45,89 +30,87 @@
 
 ### Built from source
 
 ```shell
 python setup.py install
 ```
 
-
 ## Documentation
 
-- [Composipy documentation](https://rafaelpsilva07.github.io/composipy/#contents)
-
 - [Examples](https://rafaelpsilva07.github.io/composipy/notebooks/index.html)
 
 - [Code References](https://rafaelpsilva07.github.io/composipy/reference/index.html)
 
+- [Optitmization functions](https://rafaelpsilva07.github.io/composipy/reference/optimization_functions.html)
 
 ## Quick start
 
 ### Create the Material Properties.
 
 ```python
->>> from composipy import OrthotropicMaterial
->>> 
->>> E1 = 60800
->>> E2 = 58250
->>> v12 = 0.07
->>> G12 = 4550
->>> t = 0.21
->>>
->>> mat_1 = OrthotropicMaterial(E1, E2, v12, G12, t)
+from composipy import OrthotropicMaterial
+ 
+E1 = 60800
+E2 = 58250
+v12 = 0.07
+G12 = 4550
+t = 0.21
+
+mat_1 = OrthotropicMaterial(E1, E2, v12, G12, t)
 ```
 
 See [OrthotropicMaterial](https://rafaelpsilva07.github.io/composipy/reference/classes.html) for reference.
 
 
 ### Define the Laminate.
 
 ```python
->>> from composipy import LaminateProperty
->>> stacking = [-45, 45, 90, 0, 0, 0, 0, 90, 45, -45]
->>> laminate1 = LaminateProperty(stacking, mat_1)
+from composipy import LaminateProperty
+stacking = [-45, 45, 90, 0, 0, 0, 0, 90, 45, -45]
+laminate1 = LaminateProperty(stacking, mat_1)
 ```
 
 See [LaminateProperty](https://rafaelpsilva07.github.io/composipy/reference/classes.html#laminateproperty) for reference.
 
 ### Calculate Stiffnnes Matrix and Lamination Parameters
 
 ```python
->>> print(laminate1.ABD) # prints the ABD matrix as a np.ndarray
->>> print(laminate1.xiA) # prints lamination parameters of extension as a np.ndarray
->>> print(laminate1.xiD) # prints lamination parameters of bending as a np.ndarray
+print(laminate1.ABD) # prints the ABD matrix as a np.ndarray
+print(laminate1.xiA) # prints lamination parameters of extension as a np.ndarray
+print(laminate1.xiD) # prints lamination parameters of bending as a np.ndarray
 ```
 
 ### Create a Plate Structure.
 
 ```python
->>> from composipy import PlateStructure
->>> 
->>> constraints = {    
----     'x0' : ['TX', 'TY', 'TZ', 'RX', 'RY', 'RZ'],
----     'xa' : ['TX', 'TY', 'TZ', 'RX', 'RY', 'RZ'],
----     'y0' : ['TX', 'TY', 'TZ', 'RX', 'RY', 'RZ'],
----     'yb' : ['TX', 'TY', 'TZ', 'RX', 'RY', 'RZ']
---- }
->>> panel = PlateStructure(laminate1, 360, 360, m=10, n=10, Nxx=-1, constraints=constraints)
+from composipy import PlateStructure
+ 
+constraints = {    
+     'x0' : ['TX', 'TY', 'TZ', 'RX', 'RY', 'RZ'],
+     'xa' : ['TX', 'TY', 'TZ', 'RX', 'RY', 'RZ'],
+     'y0' : ['TX', 'TY', 'TZ', 'RX', 'RY', 'RZ'],
+     'yb' : ['TX', 'TY', 'TZ', 'RX', 'RY', 'RZ']
+}
+panel = PlateStructure(laminate1, 360, 360, m=10, n=10, Nxx=-1, constraints=constraints)
 ```
 
 See [PlateStructure](https://rafaelpsilva07.github.io/composipy/reference/classes.html#platestructure) for reference.
 
 
 ### Calculate Buckling
 ```python
->>> print(panel.buckling_analysis()) # solve the eigenvalue problem.
+print(panel.buckling_analysis()) # solve the eigenvalue problem.
 ```
 
 ### Plot Buckling shape mode
 ```python
->>> print(panel.plot_eigenvalue())
+print(panel.plot_eigenvalue())
 ```
 
 
-
 ## Theoretical References
 
-The implementation of composipy is based on the following references
+The implementation of composipy is based on the following reference:
 
-- [Mechanics Of Composite Materials by Robert M. Jones](https://www.routledge.com/Mechanics-Of-Composite-Materials/Jones/p/book/9781560327127)
-- [Castro S.G.P., Donadon M.V. Assembly of semi-analytical models to address linear buckling and vibration of stiffened composite panels with debonding defect. Compos. Struct., 160 (2017), pp. 232-247,](https://www.sciencedirect.com/science/article/abs/pii/S026382231631008X)
+- SILVA, Rafael Pereira da. Composite Plate optimization combining semi-analytical model, Lamination Parameters and a Gradient-Based Optimizer. 2023. 82f. Dissertation of Master of Science – Instituto Tecnológico de Aeronáutica, São José dos Campos.
+- rafaelpsilva07. (2024). rafaelpsilva07/rafaelmscdissertation: v1.0.0 (1.0.0). Zenodo. https://doi.org/10.5281/zenodo.10546621
+- Application repository: https://github.com/rafaelpsilva07/rafaelmscdissertation
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `composipy-1.2.3/composipy/core/material.py` & `composipy-1.3/composipy/core/material.py`

 * *Files identical despite different names*

### Comparing `composipy-1.2.3/composipy/core/property.py` & `composipy-1.3/composipy/core/property.py`

 * *Files identical despite different names*

### Comparing `composipy-1.2.3/composipy/core/structure.py` & `composipy-1.3/composipy/core/structure.py`

 * *Files identical despite different names*

### Comparing `composipy-1.2.3/composipy/nastranapi/pcomp_generator.py` & `composipy-1.3/composipy/nastranapi/pcomp_generator.py`

 * *Files identical despite different names*

### Comparing `composipy-1.2.3/composipy/pre_integrated_component/_S.py` & `composipy-1.3/composipy/pre_integrated_component/_S.py`

 * *Files identical despite different names*

### Comparing `composipy-1.2.3/composipy/pre_integrated_component/_ii_F.py` & `composipy-1.3/composipy/pre_integrated_component/_ii_F.py`

 * *Files identical despite different names*

### Comparing `composipy-1.2.3/composipy/pre_integrated_component/build_k.py` & `composipy-1.3/composipy/pre_integrated_component/build_k.py`

 * *Files identical despite different names*

### Comparing `composipy-1.2.3/composipy/pre_integrated_component/functions.py` & `composipy-1.3/composipy/pre_integrated_component/functions.py`

 * *Files identical despite different names*

### Comparing `composipy-1.2.3/composipy/pre_integrated_component/write_pre_integrated_terms.py` & `composipy-1.3/composipy/pre_integrated_component/write_pre_integrated_terms.py`

 * *Files identical despite different names*

### Comparing `composipy-1.2.3/composipy/pre_integrated_component/write_shape_function.py` & `composipy-1.3/composipy/pre_integrated_component/write_shape_function.py`

 * *Files identical despite different names*

### Comparing `composipy-1.2.3/composipy/utils/validators.py` & `composipy-1.3/composipy/utils/validators.py`

 * *Files identical despite different names*

### Comparing `composipy-1.2.3/composipy.egg-info/PKG-INFO` & `composipy-1.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composipy
-Version: 1.2.3
+Version: 1.3
 Summary: This package intends to perform composite material calculations
 Home-page: https://github.com/rafaelpsilva07/composipy
 Author: Rafael Pereira
 Author-email: rafaelpsilva07@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,25 +12,27 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: matplotlib
 
 [![Downloads](https://static.pepy.tech/badge/composipy)](https://pepy.tech/project/composipy)
-[![Deploy](https://github.com/rafaelpsilva07/composipy/actions/workflows/python-publish.yml\badge.svg)](https://github.com/rafaelpsilva07/composipy/actions/workflows/python-publish.yml)
+[![Deploy](https://github.com/rafaelpsilva07/composipy/actions/workflows/python-publish.yml/badge.svg)](https://github.com/rafaelpsilva07/composipy/actions/workflows/python-publish.yml)
 [![Test](https://github.com/rafaelpsilva07/composipy/actions/workflows/pytest_test.yml/badge.svg)](https://github.com/rafaelpsilva07/composipy/actions/workflows/pytest_test.yml)
 ![PyPI](https://img.shields.io/pypi/v/composipy)
+[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rafael-pereira-da-silva07/)
+[![Youtube](https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=W4foqYR8IL0&t=622s&ab_channel=EngenhariaRefinada)
 [![DOI](https://zenodo.org/badge/332543985.svg)](https://zenodo.org/badge/latestdoi/332543985)
 
 
 # Composipy
 
 ## What it is
 
-**composipy** is a python library to calculate composite plates using the classical laminate theory. This library is designed to be simple, userfriendly and helpfull.
+Composipy is a Python-based library designed to address the challenges of composite plate analysis and optimization in the aerospace industry, where weight reduction is crucial for efficient and profitable aircraft design. The library offers tools for plate buckling analysis and lamination parameter optimization, empowering engineers to streamline the design process and enhance structural performance. Utilizing object-oriented programming and native Python structures, Composipy ensures a seamless workflow and easy integration into existing engineering practices. Through continuous integration and delivery practices, Composipy maintains reliability and efficiency. 
 
 Composipy is able to perform buckling calculation considering different boundary conditions and in-plane load applications. See [Examples](https://rafaelpsilva07.github.io/composipy/notebooks/Examples_BCs.html).
 
 
 <img src="https://github.com/rafaelpsilva07/composipy/blob/main/doc/images/load_bcs_examples.PNG" width="700">
 
 
@@ -45,89 +47,87 @@
 
 ### Built from source
 
 ```shell
 python setup.py install
 ```
 
-
 ## Documentation
 
-- [Composipy documentation](https://rafaelpsilva07.github.io/composipy/#contents)
-
 - [Examples](https://rafaelpsilva07.github.io/composipy/notebooks/index.html)
 
 - [Code References](https://rafaelpsilva07.github.io/composipy/reference/index.html)
 
+- [Optitmization functions](https://rafaelpsilva07.github.io/composipy/reference/optimization_functions.html)
 
 ## Quick start
 
 ### Create the Material Properties.
 
 ```python
->>> from composipy import OrthotropicMaterial
->>> 
->>> E1 = 60800
->>> E2 = 58250
->>> v12 = 0.07
->>> G12 = 4550
->>> t = 0.21
->>>
->>> mat_1 = OrthotropicMaterial(E1, E2, v12, G12, t)
+from composipy import OrthotropicMaterial
+ 
+E1 = 60800
+E2 = 58250
+v12 = 0.07
+G12 = 4550
+t = 0.21
+
+mat_1 = OrthotropicMaterial(E1, E2, v12, G12, t)
 ```
 
 See [OrthotropicMaterial](https://rafaelpsilva07.github.io/composipy/reference/classes.html) for reference.
 
 
 ### Define the Laminate.
 
 ```python
->>> from composipy import LaminateProperty
->>> stacking = [-45, 45, 90, 0, 0, 0, 0, 90, 45, -45]
->>> laminate1 = LaminateProperty(stacking, mat_1)
+from composipy import LaminateProperty
+stacking = [-45, 45, 90, 0, 0, 0, 0, 90, 45, -45]
+laminate1 = LaminateProperty(stacking, mat_1)
 ```
 
 See [LaminateProperty](https://rafaelpsilva07.github.io/composipy/reference/classes.html#laminateproperty) for reference.
 
 ### Calculate Stiffnnes Matrix and Lamination Parameters
 
 ```python
->>> print(laminate1.ABD) # prints the ABD matrix as a np.ndarray
->>> print(laminate1.xiA) # prints lamination parameters of extension as a np.ndarray
->>> print(laminate1.xiD) # prints lamination parameters of bending as a np.ndarray
+print(laminate1.ABD) # prints the ABD matrix as a np.ndarray
+print(laminate1.xiA) # prints lamination parameters of extension as a np.ndarray
+print(laminate1.xiD) # prints lamination parameters of bending as a np.ndarray
 ```
 
 ### Create a Plate Structure.
 
 ```python
->>> from composipy import PlateStructure
->>> 
->>> constraints = {    
----     'x0' : ['TX', 'TY', 'TZ', 'RX', 'RY', 'RZ'],
----     'xa' : ['TX', 'TY', 'TZ', 'RX', 'RY', 'RZ'],
----     'y0' : ['TX', 'TY', 'TZ', 'RX', 'RY', 'RZ'],
----     'yb' : ['TX', 'TY', 'TZ', 'RX', 'RY', 'RZ']
---- }
->>> panel = PlateStructure(laminate1, 360, 360, m=10, n=10, Nxx=-1, constraints=constraints)
+from composipy import PlateStructure
+ 
+constraints = {    
+     'x0' : ['TX', 'TY', 'TZ', 'RX', 'RY', 'RZ'],
+     'xa' : ['TX', 'TY', 'TZ', 'RX', 'RY', 'RZ'],
+     'y0' : ['TX', 'TY', 'TZ', 'RX', 'RY', 'RZ'],
+     'yb' : ['TX', 'TY', 'TZ', 'RX', 'RY', 'RZ']
+}
+panel = PlateStructure(laminate1, 360, 360, m=10, n=10, Nxx=-1, constraints=constraints)
 ```
 
 See [PlateStructure](https://rafaelpsilva07.github.io/composipy/reference/classes.html#platestructure) for reference.
 
 
 ### Calculate Buckling
 ```python
->>> print(panel.buckling_analysis()) # solve the eigenvalue problem.
+print(panel.buckling_analysis()) # solve the eigenvalue problem.
 ```
 
 ### Plot Buckling shape mode
 ```python
->>> print(panel.plot_eigenvalue())
+print(panel.plot_eigenvalue())
 ```
 
 
-
 ## Theoretical References
 
-The implementation of composipy is based on the following references
+The implementation of composipy is based on the following reference:
 
-- [Mechanics Of Composite Materials by Robert M. Jones](https://www.routledge.com/Mechanics-Of-Composite-Materials/Jones/p/book/9781560327127)
-- [Castro S.G.P., Donadon M.V. Assembly of semi-analytical models to address linear buckling and vibration of stiffened composite panels with debonding defect. Compos. Struct., 160 (2017), pp. 232-247,](https://www.sciencedirect.com/science/article/abs/pii/S026382231631008X)
+- SILVA, Rafael Pereira da. Composite Plate optimization combining semi-analytical model, Lamination Parameters and a Gradient-Based Optimizer. 2023. 82f. Dissertation of Master of Science – Instituto Tecnológico de Aeronáutica, São José dos Campos.
+- rafaelpsilva07. (2024). rafaelpsilva07/rafaelmscdissertation: v1.0.0 (1.0.0). Zenodo. https://doi.org/10.5281/zenodo.10546621
+- Application repository: https://github.com/rafaelpsilva07/rafaelmscdissertation
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `composipy-1.2.3/composipy.egg-info/SOURCES.txt` & `composipy-1.3/composipy.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 composipy/core/property.py
 composipy/core/structure.py
 composipy/nastranapi/__init__.py
 composipy/nastranapi/pcomp_generator.py
 composipy/optimize/__init__.py
 composipy/optimize/_maximize_buckling.py
 composipy/optimize/_minimize_panel_weight.py
+composipy/optimize/utils.py
 composipy/pre_integrated_component/_S.py
 composipy/pre_integrated_component/__init__.py
 composipy/pre_integrated_component/_ii_F.py
 composipy/pre_integrated_component/build_k.py
 composipy/pre_integrated_component/functions.py
 composipy/pre_integrated_component/write_pre_integrated_terms.py
 composipy/pre_integrated_component/write_shape_function.py
```

### Comparing `composipy-1.2.3/setup.py` & `composipy-1.3/setup.py`

 * *Files identical despite different names*

### Comparing `composipy-1.2.3/tests/test_ABD.py` & `composipy-1.3/tests/test_ABD.py`

 * *Files identical despite different names*

### Comparing `composipy-1.2.3/tests/test_Material_Q0.py` & `composipy-1.3/tests/test_Material_Q0.py`

 * *Files identical despite different names*

### Comparing `composipy-1.2.3/tests/test_lamination_parameters.py` & `composipy-1.3/tests/test_lamination_parameters.py`

 * *Files identical despite different names*

### Comparing `composipy-1.2.3/tests/test_plate_buckling.py` & `composipy-1.3/tests/test_plate_buckling.py`

 * *Files identical despite different names*

### Comparing `composipy-1.2.3/tests/test_plate_buckling_LP.py` & `composipy-1.3/tests/test_plate_buckling_LP.py`

 * *Files identical despite different names*

