# Comparing `tmp/pynumint-0.0.7.tar.gz` & `tmp/pynumint-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynumint-0.0.7.tar", last modified: Thu May 30 13:48:34 2024, max compression
+gzip compressed data, was "pynumint-0.0.8.tar", last modified: Thu May 30 14:07:58 2024, max compression
```

## Comparing `pynumint-0.0.7.tar` & `pynumint-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 13:48:34.019258 pynumint-0.0.7/
--rw-rw-rw-   0        0        0     1091 2024-05-26 10:33:54.000000 pynumint-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     4942 2024-05-30 13:48:34.019258 pynumint-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     4434 2024-05-30 13:47:32.000000 pynumint-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 13:48:33.517269 pynumint-0.0.7/pynumint/
-drwxrwxrwx   0        0        0        0 2024-05-30 13:48:34.019258 pynumint-0.0.7/pynumint/src/
-drwxrwxrwx   0        0        0        0 2024-05-30 13:48:33.968770 pynumint-0.0.7/pynumint/src/pynumint.egg-info/
--rw-rw-rw-   0        0        0     4942 2024-05-30 13:48:33.000000 pynumint-0.0.7/pynumint/src/pynumint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2024-05-30 13:48:33.000000 pynumint-0.0.7/pynumint/src/pynumint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 13:48:33.000000 pynumint-0.0.7/pynumint/src/pynumint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-05-30 13:48:33.000000 pynumint-0.0.7/pynumint/src/pynumint.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2024-05-30 13:48:33.000000 pynumint-0.0.7/pynumint/src/pynumint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4237 2024-05-30 07:33:34.000000 pynumint-0.0.7/pynumint/src/pynumint.py
--rw-rw-rw-   0        0        0       42 2024-05-30 13:48:34.019258 pynumint-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1095 2024-05-30 13:47:48.000000 pynumint-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:07:58.692528 pynumint-0.0.8/
+-rw-rw-rw-   0        0        0     1091 2024-05-26 10:33:54.000000 pynumint-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     5453 2024-05-30 14:07:58.692528 pynumint-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4434 2024-05-30 13:47:32.000000 pynumint-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 14:07:58.625426 pynumint-0.0.8/pynumint/
+drwxrwxrwx   0        0        0        0 2024-05-30 14:07:58.692528 pynumint-0.0.8/pynumint/src/
+drwxrwxrwx   0        0        0        0 2024-05-30 14:07:58.689813 pynumint-0.0.8/pynumint/src/pynumint.egg-info/
+-rw-rw-rw-   0        0        0     5453 2024-05-30 14:07:58.000000 pynumint-0.0.8/pynumint/src/pynumint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2024-05-30 14:07:58.000000 pynumint-0.0.8/pynumint/src/pynumint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 14:07:58.000000 pynumint-0.0.8/pynumint/src/pynumint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-05-30 14:07:58.000000 pynumint-0.0.8/pynumint/src/pynumint.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       60 2024-05-30 14:07:58.000000 pynumint-0.0.8/pynumint/src/pynumint.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-30 14:07:58.000000 pynumint-0.0.8/pynumint/src/pynumint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4237 2024-05-30 07:33:34.000000 pynumint-0.0.8/pynumint/src/pynumint.py
+-rw-rw-rw-   0        0        0       42 2024-05-30 14:07:58.692528 pynumint-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1836 2024-05-30 14:07:35.000000 pynumint-0.0.8/setup.py
```

### Comparing `pynumint-0.0.7/LICENSE` & `pynumint-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pynumint-0.0.7/PKG-INFO` & `pynumint-0.0.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,31 @@
 Metadata-Version: 2.1
 Name: pynumint
-Version: 0.0.7
+Version: 0.0.8
 Summary: pynumint Test Package for Numerical Integration Demo
-Home-page: https://pypi.org/project/pynumint/
+Home-page: https://github.com/CodeSleuthX/pynumint
 Author: Arjun Jagdale
 Author-email: arjunjagdale14@gmail.com
 License: UNKNOWN
+Project-URL: Bug Reports, https://github.com/CodeSleuthX/pynumint/issues
+Project-URL: Source, https://github.com/CodeSleuthX/pynumint
+Keywords: numerical integration mathematics science
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: test
 License-File: LICENSE
 
 # pynumint: A Numerical Integration Library
 ![ml drop](https://github.com/CodeSleuthX/pynumint/assets/142811259/b7d21ac6-c862-42d9-b64e-23dd2f732d8f)
 
 pynumint is a Python library for numerical integration methods.
 pynumint offers a wide range of numerical integration methods, including trapezoidal rule, Simpson's rule, midpoint rule, Boole's rule, Romberg integration, Gauss-Legendre quadrature, Gauss-Chebyshev quadrature, Gauss-Laguerre quadrature, Gauss-Hermite quadrature, adaptive Simpson's rule, Monte Carlo integration, and double integrals. Users can choose the most suitable method based on the characteristics of the function and the desired level of accuracy.
```

### Comparing `pynumint-0.0.7/README.md` & `pynumint-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pynumint-0.0.7/pynumint/src/pynumint.egg-info/PKG-INFO` & `pynumint-0.0.8/pynumint/src/pynumint.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,31 @@
 Metadata-Version: 2.1
 Name: pynumint
-Version: 0.0.7
+Version: 0.0.8
 Summary: pynumint Test Package for Numerical Integration Demo
-Home-page: https://pypi.org/project/pynumint/
+Home-page: https://github.com/CodeSleuthX/pynumint
 Author: Arjun Jagdale
 Author-email: arjunjagdale14@gmail.com
 License: UNKNOWN
+Project-URL: Bug Reports, https://github.com/CodeSleuthX/pynumint/issues
+Project-URL: Source, https://github.com/CodeSleuthX/pynumint
+Keywords: numerical integration mathematics science
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: test
 License-File: LICENSE
 
 # pynumint: A Numerical Integration Library
 ![ml drop](https://github.com/CodeSleuthX/pynumint/assets/142811259/b7d21ac6-c862-42d9-b64e-23dd2f732d8f)
 
 pynumint is a Python library for numerical integration methods.
 pynumint offers a wide range of numerical integration methods, including trapezoidal rule, Simpson's rule, midpoint rule, Boole's rule, Romberg integration, Gauss-Legendre quadrature, Gauss-Chebyshev quadrature, Gauss-Laguerre quadrature, Gauss-Hermite quadrature, adaptive Simpson's rule, Monte Carlo integration, and double integrals. Users can choose the most suitable method based on the characteristics of the function and the desired level of accuracy.
```

### Comparing `pynumint-0.0.7/pynumint/src/pynumint.py` & `pynumint-0.0.8/pynumint/src/pynumint.py`

 * *Files identical despite different names*

