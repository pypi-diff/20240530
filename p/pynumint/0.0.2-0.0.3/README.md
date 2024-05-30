# Comparing `tmp/pynumint-0.0.2.tar.gz` & `tmp/pynumint-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynumint-0.0.2.tar", last modified: Thu May 30 06:35:32 2024, max compression
+gzip compressed data, was "pynumint-0.0.3.tar", last modified: Thu May 30 07:03:09 2024, max compression
```

## Comparing `pynumint-0.0.2.tar` & `pynumint-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 06:35:32.981851 pynumint-0.0.2/
--rw-rw-rw-   0        0        0     1091 2024-05-26 10:33:54.000000 pynumint-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     3298 2024-05-30 06:35:32.981851 pynumint-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2848 2024-05-30 06:34:12.000000 pynumint-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 06:35:32.816779 pynumint-0.0.2/pynumint/
-drwxrwxrwx   0        0        0        0 2024-05-30 06:35:32.981851 pynumint-0.0.2/pynumint/src/
-drwxrwxrwx   0        0        0        0 2024-05-30 06:35:32.973475 pynumint-0.0.2/pynumint/src/pynumint.egg-info/
--rw-rw-rw-   0        0        0     3298 2024-05-30 06:35:31.000000 pynumint-0.0.2/pynumint/src/pynumint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2024-05-30 06:35:31.000000 pynumint-0.0.2/pynumint/src/pynumint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 06:35:31.000000 pynumint-0.0.2/pynumint/src/pynumint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-30 06:35:31.000000 pynumint-0.0.2/pynumint/src/pynumint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2841 2024-05-30 06:28:13.000000 pynumint-0.0.2/pynumint/src/pynumint.py
--rw-rw-rw-   0        0        0       42 2024-05-30 06:35:32.981851 pynumint-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1240 2024-05-30 06:26:23.000000 pynumint-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 07:03:09.579182 pynumint-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2024-05-26 10:33:54.000000 pynumint-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     4035 2024-05-30 07:03:09.579182 pynumint-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3594 2024-05-30 07:00:47.000000 pynumint-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 07:03:09.499196 pynumint-0.0.3/pynumint/
+drwxrwxrwx   0        0        0        0 2024-05-30 07:03:09.569185 pynumint-0.0.3/pynumint/src/
+drwxrwxrwx   0        0        0        0 2024-05-30 07:03:09.569185 pynumint-0.0.3/pynumint/src/pynumint.egg-info/
+-rw-rw-rw-   0        0        0     4035 2024-05-30 07:03:09.000000 pynumint-0.0.3/pynumint/src/pynumint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2024-05-30 07:03:09.000000 pynumint-0.0.3/pynumint/src/pynumint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 07:03:09.000000 pynumint-0.0.3/pynumint/src/pynumint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-30 07:03:09.000000 pynumint-0.0.3/pynumint/src/pynumint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4237 2024-05-30 07:02:13.000000 pynumint-0.0.3/pynumint/src/pynumint.py
+-rw-rw-rw-   0        0        0       42 2024-05-30 07:03:09.579182 pynumint-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1240 2024-05-30 06:47:50.000000 pynumint-0.0.3/setup.py
```

### Comparing `pynumint-0.0.2/LICENSE` & `pynumint-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pynumint-0.0.2/PKG-INFO` & `pynumint-0.0.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,94 +1,108 @@
-Metadata-Version: 2.1
-Name: pynumint
-Version: 0.0.2
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
-pynumint offers a wide range of numerical integration methods, including trapezoidal rule, Simpson's rule, midpoint rule, Boole's rule, Romberg integration, and Gauss-Legendre quadrature. Users can choose the most suitable method based on the characteristics of the function and the desired level of accuracy.
+pynumint offers a wide range of numerical integration methods, including :
+1] trapezoidal rule 
+2] Simpson's rule 
+3] midpoint rule 
+4] Boole's rule 
+5] Romberg integration
+6] Gauss-Legendre quadrature 
+7] Gauss-Chebyshev quadrature
+8] Gauss-Laguerre quadrature
+9] Gauss-Hermite quadrature 
+10] adaptive Simpson's rule 
+11] Monte Carlo integration
+12] double integrals
+13] Simpson's rule with error estimation
+Users can choose the most suitable method based on the characteristics of the function and the desired level of accuracy.
 
 ## Installation
 
 ```bash
-
 pip install pynumint
 
+
 ```
 
 ## Usage
 ```bash
 
-from pynumint import trapezoidal_rule, simpsons_rule, midpoint_rule, booles_rule, romberg_integration, gauss_legendre_quadrature, gauss_chebyshev_quadrature, gauss_laguerre_quadrature, gauss_hermite_quadrature
+from pynumint import trapezoidal_rule, simpsons_rule, midpoint_rule, booles_rule, romberg_integration, gauss_legendre_quadrature, gauss_chebyshev_quadrature, gauss_laguerre_quadrature, gauss_hermite_quadrature, adaptive_simpsons_rule, monte_carlo_integration, double_integral, simpsons_rule_with_error
 import numpy as np
 
 # Define your functions to be integrated
 def f1(x):
     return x**2
 
 def f2(x):
     return np.sin(x)
 
 def f3(x):
     return np.exp(-x**2)
 
 def f4(x):
-    return np.cos(x)
+    return np.log(x) 
+
+def f5(x, y):
+    return x * y
 
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
-result_gauss_chebyshev = gauss_chebyshev_quadrature(f4, n)
-result_gauss_laguerre = gauss_laguerre_quadrature(f3, n)
-result_gauss_hermite = gauss_hermite_quadrature(f3, n)
+result_gauss_chebyshev = gauss_chebyshev_quadrature(f3, 5)
+result_gauss_laguerre = gauss_laguerre_quadrature(f3, 5)
+result_gauss_hermite = gauss_hermite_quadrature(f3, 5)
+result_adaptive_simpsons = adaptive_simpsons_rule(f3, a, b, 1e-6)
+result_monte_carlo = monte_carlo_integration(f3, a, b)
+result_double_integral = double_integral(f5, 0, 1, 0, 1)
+result_simpsons_error, error_estimate = simpsons_rule_with_error(f2, a, b, n)
 
 print("Results:")
 print(f"Trapezoidal Rule: {result_trapezoidal}")
 print(f"Simpson's Rule: {result_simpsons}")
 print(f"Midpoint Rule: {result_midpoint}")
 print(f"Boole's Rule: {result_booles}")
 print(f"Romberg Integration: {result_romberg}")
 print(f"Gauss-Legendre Quadrature: {result_gauss_legendre}")
 print(f"Gauss-Chebyshev Quadrature: {result_gauss_chebyshev}")
 print(f"Gauss-Laguerre Quadrature: {result_gauss_laguerre}")
 print(f"Gauss-Hermite Quadrature: {result_gauss_hermite}")
+print(f"Adaptive Simpson's Rule: {result_adaptive_simpsons}")
+print(f"Monte Carlo Integration: {result_monte_carlo}")
+print(f"Double Integral: {result_double_integral}")
+print(f"Simpson's Rule with Error Estimation: {result_simpsons_error} with an error estimate of {error_estimate}")
+
+
 
 ```
 
 ## Output
 ```bash 
 
-Trapezoidal Rule: The integral of f1(x) from 0 to 10 is approximately 333.333333
-Simpson's Rule: The integral of f2(x) from 0 to 10 is approximately 1.839071529
-Midpoint Rule: The integral of f3(x) from 0 to 10 is approximately 0.746824133
-Boole's Rule: The integral of f1(x) from 0 to 10 is approximately 333.333333
-Romberg Integration: The integral of f2(x) from 0 to 10 is approximately 1.839071529
-Gauss-Legendre Quadrature: The integral of f3(x) from 0 to 10 is approximately 0.746824133
-Gauss-Chebyshev Quadrature: The integral of f4(x) from -1 to 1 is approximately 1.570796327
-Gauss-Laguerre Quadrature: The integral of f3(x) from 0 to âˆž is approximately 0.886226925
-Gauss-Hermite Quadrature: The integral of f3(x) from -âˆž to âˆž is approximately 1.772453851
-
+Results:
+Trapezoidal Rule: 333.33350000000013
+Simpson's Rule: 1.8390715291786217
+Midpoint Rule: 0.8862269254527569
+Boole's Rule: 333.3333333333334
+Romberg Integration: 1.839071529076259
+Gauss-Legendre Quadrature: 0.9622861833849173
+Gauss-Chebyshev Quadrature: 2.026469405000093
+Gauss-Laguerre Quadrature: 0.5408201719540809
+Gauss-Hermite Quadrature: 1.260069748687603
+Adaptive Simpson's Rule: 0.443113467730597
+Monte Carlo Integration: 0.7746479690195586
+Double Integral: 0.25507601265177027
+Simpson's Rule with Error Estimation: 1.8390715291786217 with an error estimate of 5.555553794065748e-06
 
 ```
 
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pynumint-0.0.2/setup.py` & `pynumint-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pynumint",                     # This is the name of the package
-    version="0.0.2",                        # The initial release version
+    version="0.0.3",                        # The initial release version
     author="Arjun Jagdale",                     # Full name of the author
     description="pynumint Test Package for Numerical Integration Demo",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
```

