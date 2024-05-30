# Comparing `tmp/pynumint-0.0.1.tar.gz` & `tmp/pynumint-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynumint-0.0.1.tar", last modified: Sun May 26 10:54:59 2024, max compression
+gzip compressed data, was "pynumint-0.0.2.tar", last modified: Thu May 30 06:35:32 2024, max compression
```

## Comparing `pynumint-0.0.1.tar` & `pynumint-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 10:54:59.157812 pynumint-0.0.1/
--rw-rw-rw-   0        0        0     1091 2024-05-26 10:33:54.000000 pynumint-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2569 2024-05-26 10:54:59.156800 pynumint-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2128 2024-05-26 10:52:03.000000 pynumint-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-26 10:54:59.120033 pynumint-0.0.1/pynumint/
-drwxrwxrwx   0        0        0        0 2024-05-26 10:54:59.155076 pynumint-0.0.1/pynumint/src/
-drwxrwxrwx   0        0        0        0 2024-05-26 10:54:59.154064 pynumint-0.0.1/pynumint/src/pynumint.egg-info/
--rw-rw-rw-   0        0        0     2569 2024-05-26 10:54:59.000000 pynumint-0.0.1/pynumint/src/pynumint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2024-05-26 10:54:59.000000 pynumint-0.0.1/pynumint/src/pynumint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 10:54:59.000000 pynumint-0.0.1/pynumint/src/pynumint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-26 10:54:59.000000 pynumint-0.0.1/pynumint/src/pynumint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1814 2024-05-26 10:53:52.000000 pynumint-0.0.1/pynumint/src/pynumint.py
--rw-rw-rw-   0        0        0       42 2024-05-26 10:54:59.157812 pynumint-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1240 2024-05-26 10:36:29.000000 pynumint-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:35:32.981851 pynumint-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2024-05-26 10:33:54.000000 pynumint-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3298 2024-05-30 06:35:32.981851 pynumint-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2848 2024-05-30 06:34:12.000000 pynumint-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 06:35:32.816779 pynumint-0.0.2/pynumint/
+drwxrwxrwx   0        0        0        0 2024-05-30 06:35:32.981851 pynumint-0.0.2/pynumint/src/
+drwxrwxrwx   0        0        0        0 2024-05-30 06:35:32.973475 pynumint-0.0.2/pynumint/src/pynumint.egg-info/
+-rw-rw-rw-   0        0        0     3298 2024-05-30 06:35:31.000000 pynumint-0.0.2/pynumint/src/pynumint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2024-05-30 06:35:31.000000 pynumint-0.0.2/pynumint/src/pynumint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 06:35:31.000000 pynumint-0.0.2/pynumint/src/pynumint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-30 06:35:31.000000 pynumint-0.0.2/pynumint/src/pynumint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2841 2024-05-30 06:28:13.000000 pynumint-0.0.2/pynumint/src/pynumint.py
+-rw-rw-rw-   0        0        0       42 2024-05-30 06:35:32.981851 pynumint-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1240 2024-05-30 06:26:23.000000 pynumint-0.0.2/setup.py
```

### Comparing `pynumint-0.0.1/LICENSE` & `pynumint-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pynumint-0.0.1/PKG-INFO` & `pynumint-0.0.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: pynumint
-Version: 0.0.1
-Summary: pynumint Test Package for Numerical Integration Demo
-Home-page: UNKNOWN
-Author: Arjun Jagdale
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # pynumint: A Numerical Integration Library
 
 pynumint is a Python library for numerical integration methods.
 pynumint offers a wide range of numerical integration methods, including trapezoidal rule, Simpson's rule, midpoint rule, Boole's rule, Romberg integration, and Gauss-Legendre quadrature. Users can choose the most suitable method based on the characteristics of the function and the desired level of accuracy.
 
 ## Installation
 
@@ -25,57 +10,68 @@
 pip install pynumint
 
 ```
 
 ## Usage
 ```bash
 
-from pynumint import trapezoidal_rule, simpsons_rule, midpoint_rule, booles_rule, romberg_integration, gauss_legendre_quadrature
+from pynumint import trapezoidal_rule, simpsons_rule, midpoint_rule, booles_rule, romberg_integration, gauss_legendre_quadrature, gauss_chebyshev_quadrature, gauss_laguerre_quadrature, gauss_hermite_quadrature
 import numpy as np
 
 # Define your functions to be integrated
 def f1(x):
     return x**2
 
 def f2(x):
     return np.sin(x)
 
 def f3(x):
     return np.exp(-x**2)
 
+def f4(x):
+    return np.cos(x)
+
 # Define integration limits and number of intervals
 a = 0
 b = 10
 n = 1000
 
 # Example usage of numerical integration methods
 result_trapezoidal = trapezoidal_rule(f1, a, b, n)
 result_simpsons = simpsons_rule(f2, a, b, n)
 result_midpoint = midpoint_rule(f3, a, b, n)
 result_booles = booles_rule(f1, a, b, n)
 result_romberg = romberg_integration(f2, a, b)
 result_gauss_legendre = gauss_legendre_quadrature(f3, a, b, 5)
+result_gauss_chebyshev = gauss_chebyshev_quadrature(f4, n)
+result_gauss_laguerre = gauss_laguerre_quadrature(f3, n)
+result_gauss_hermite = gauss_hermite_quadrature(f3, n)
 
 print("Results:")
 print(f"Trapezoidal Rule: {result_trapezoidal}")
 print(f"Simpson's Rule: {result_simpsons}")
 print(f"Midpoint Rule: {result_midpoint}")
 print(f"Boole's Rule: {result_booles}")
 print(f"Romberg Integration: {result_romberg}")
 print(f"Gauss-Legendre Quadrature: {result_gauss_legendre}")
+print(f"Gauss-Chebyshev Quadrature: {result_gauss_chebyshev}")
+print(f"Gauss-Laguerre Quadrature: {result_gauss_laguerre}")
+print(f"Gauss-Hermite Quadrature: {result_gauss_hermite}")
 
 ```
 
 ## Output
 ```bash 
 
-Trapezoidal Rule: The integral of f1(x) from 0 to 1 is approximately 0.45969765582371824
-Simpson's Rule: The integral of f2(x) from 0 to 1 is approximately 0.7468241328124364
-Midpoint Rule: The integral of f3(x) from 0 to 1 is approximately 0.7853981842307807
-Boole's Rule: The integral of f1(x) from 0 to 1 is approximately 0.45969769413186057
-Romberg Integration: The integral of f2(x) from 0 to 1 is approximately 0.7468241330950943
-Gauss-Legendre Quadrature: The integral of f3(x) from 0 to 1 is approximately 0.7853981599711883
-
-```
+Trapezoidal Rule: The integral of f1(x) from 0 to 10 is approximately 333.333333
+Simpson's Rule: The integral of f2(x) from 0 to 10 is approximately 1.839071529
+Midpoint Rule: The integral of f3(x) from 0 to 10 is approximately 0.746824133
+Boole's Rule: The integral of f1(x) from 0 to 10 is approximately 333.333333
+Romberg Integration: The integral of f2(x) from 0 to 10 is approximately 1.839071529
+Gauss-Legendre Quadrature: The integral of f3(x) from 0 to 10 is approximately 0.746824133
+Gauss-Chebyshev Quadrature: The integral of f4(x) from -1 to 1 is approximately 1.570796327
+Gauss-Laguerre Quadrature: The integral of f3(x) from 0 to ∞ is approximately 0.886226925
+Gauss-Hermite Quadrature: The integral of f3(x) from -∞ to ∞ is approximately 1.772453851
 
 
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pynumint-0.0.1/pynumint/src/pynumint.egg-info/PKG-INFO` & `pynumint-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynumint
-Version: 0.0.1
+Version: 0.0.2
 Summary: pynumint Test Package for Numerical Integration Demo
 Home-page: UNKNOWN
 Author: Arjun Jagdale
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -25,57 +25,70 @@
 pip install pynumint
 
 ```
 
 ## Usage
 ```bash
 
-from pynumint import trapezoidal_rule, simpsons_rule, midpoint_rule, booles_rule, romberg_integration, gauss_legendre_quadrature
+from pynumint import trapezoidal_rule, simpsons_rule, midpoint_rule, booles_rule, romberg_integration, gauss_legendre_quadrature, gauss_chebyshev_quadrature, gauss_laguerre_quadrature, gauss_hermite_quadrature
 import numpy as np
 
 # Define your functions to be integrated
 def f1(x):
     return x**2
 
 def f2(x):
     return np.sin(x)
 
 def f3(x):
     return np.exp(-x**2)
 
+def f4(x):
+    return np.cos(x)
+
 # Define integration limits and number of intervals
 a = 0
 b = 10
 n = 1000
 
 # Example usage of numerical integration methods
 result_trapezoidal = trapezoidal_rule(f1, a, b, n)
 result_simpsons = simpsons_rule(f2, a, b, n)
 result_midpoint = midpoint_rule(f3, a, b, n)
 result_booles = booles_rule(f1, a, b, n)
 result_romberg = romberg_integration(f2, a, b)
 result_gauss_legendre = gauss_legendre_quadrature(f3, a, b, 5)
+result_gauss_chebyshev = gauss_chebyshev_quadrature(f4, n)
+result_gauss_laguerre = gauss_laguerre_quadrature(f3, n)
+result_gauss_hermite = gauss_hermite_quadrature(f3, n)
 
 print("Results:")
 print(f"Trapezoidal Rule: {result_trapezoidal}")
 print(f"Simpson's Rule: {result_simpsons}")
 print(f"Midpoint Rule: {result_midpoint}")
 print(f"Boole's Rule: {result_booles}")
 print(f"Romberg Integration: {result_romberg}")
 print(f"Gauss-Legendre Quadrature: {result_gauss_legendre}")
+print(f"Gauss-Chebyshev Quadrature: {result_gauss_chebyshev}")
+print(f"Gauss-Laguerre Quadrature: {result_gauss_laguerre}")
+print(f"Gauss-Hermite Quadrature: {result_gauss_hermite}")
 
 ```
 
 ## Output
 ```bash 
 
-Trapezoidal Rule: The integral of f1(x) from 0 to 1 is approximately 0.45969765582371824
-Simpson's Rule: The integral of f2(x) from 0 to 1 is approximately 0.7468241328124364
-Midpoint Rule: The integral of f3(x) from 0 to 1 is approximately 0.7853981842307807
-Boole's Rule: The integral of f1(x) from 0 to 1 is approximately 0.45969769413186057
-Romberg Integration: The integral of f2(x) from 0 to 1 is approximately 0.7468241330950943
-Gauss-Legendre Quadrature: The integral of f3(x) from 0 to 1 is approximately 0.7853981599711883
+Trapezoidal Rule: The integral of f1(x) from 0 to 10 is approximately 333.333333
+Simpson's Rule: The integral of f2(x) from 0 to 10 is approximately 1.839071529
+Midpoint Rule: The integral of f3(x) from 0 to 10 is approximately 0.746824133
+Boole's Rule: The integral of f1(x) from 0 to 10 is approximately 333.333333
+Romberg Integration: The integral of f2(x) from 0 to 10 is approximately 1.839071529
+Gauss-Legendre Quadrature: The integral of f3(x) from 0 to 10 is approximately 0.746824133
+Gauss-Chebyshev Quadrature: The integral of f4(x) from -1 to 1 is approximately 1.570796327
+Gauss-Laguerre Quadrature: The integral of f3(x) from 0 to âˆž is approximately 0.886226925
+Gauss-Hermite Quadrature: The integral of f3(x) from -âˆž to âˆž is approximately 1.772453851
+
 
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pynumint-0.0.1/setup.py` & `pynumint-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pynumint",                     # This is the name of the package
-    version="0.0.1",                        # The initial release version
+    version="0.0.2",                        # The initial release version
     author="Arjun Jagdale",                     # Full name of the author
     description="pynumint Test Package for Numerical Integration Demo",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
```

