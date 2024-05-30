# Comparing `tmp/pynumint-0.0.4.tar.gz` & `tmp/pynumint-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynumint-0.0.4.tar", last modified: Thu May 30 07:11:11 2024, max compression
+gzip compressed data, was "pynumint-0.0.5.tar", last modified: Thu May 30 08:24:18 2024, max compression
```

## Comparing `pynumint-0.0.4.tar` & `pynumint-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 07:11:11.583019 pynumint-0.0.4/
--rw-rw-rw-   0        0        0     1091 2024-05-26 10:33:54.000000 pynumint-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     4015 2024-05-30 07:11:11.583019 pynumint-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3507 2024-05-30 07:09:22.000000 pynumint-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 07:11:11.185218 pynumint-0.0.4/pynumint/
-drwxrwxrwx   0        0        0        0 2024-05-30 07:11:11.583019 pynumint-0.0.4/pynumint/src/
-drwxrwxrwx   0        0        0        0 2024-05-30 07:11:11.582214 pynumint-0.0.4/pynumint/src/pynumint.egg-info/
--rw-rw-rw-   0        0        0     4015 2024-05-30 07:11:11.000000 pynumint-0.0.4/pynumint/src/pynumint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2024-05-30 07:11:11.000000 pynumint-0.0.4/pynumint/src/pynumint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 07:11:11.000000 pynumint-0.0.4/pynumint/src/pynumint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-30 07:11:11.000000 pynumint-0.0.4/pynumint/src/pynumint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4237 2024-05-30 07:02:13.000000 pynumint-0.0.4/pynumint/src/pynumint.py
--rw-rw-rw-   0        0        0       42 2024-05-30 07:11:11.583019 pynumint-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1354 2024-05-30 07:10:34.000000 pynumint-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 08:24:18.325828 pynumint-0.0.5/
+-rw-rw-rw-   0        0        0     1091 2024-05-26 10:33:54.000000 pynumint-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     3978 2024-05-30 08:24:18.324830 pynumint-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3470 2024-05-30 07:34:52.000000 pynumint-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 08:24:18.283712 pynumint-0.0.5/pynumint/
+drwxrwxrwx   0        0        0        0 2024-05-30 08:24:18.323830 pynumint-0.0.5/pynumint/src/
+drwxrwxrwx   0        0        0        0 2024-05-30 08:24:18.322832 pynumint-0.0.5/pynumint/src/pynumint.egg-info/
+-rw-rw-rw-   0        0        0     3978 2024-05-30 08:24:18.000000 pynumint-0.0.5/pynumint/src/pynumint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2024-05-30 08:24:18.000000 pynumint-0.0.5/pynumint/src/pynumint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 08:24:18.000000 pynumint-0.0.5/pynumint/src/pynumint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-30 08:24:18.000000 pynumint-0.0.5/pynumint/src/pynumint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4237 2024-05-30 07:33:34.000000 pynumint-0.0.5/pynumint/src/pynumint.py
+-rw-rw-rw-   0        0        0       42 2024-05-30 08:24:18.325828 pynumint-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     2957 2024-05-30 08:23:41.000000 pynumint-0.0.5/setup.py
```

### Comparing `pynumint-0.0.4/LICENSE` & `pynumint-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pynumint-0.0.4/PKG-INFO` & `pynumint-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynumint
-Version: 0.0.4
+Version: 0.0.5
 Summary: pynumint Test Package for Numerical Integration Demo
 Home-page: https://pypi.org/project/pynumint/
 Author: Arjun Jagdale
 Author-email: arjunjagdale14@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -39,18 +39,15 @@
 
 def f2(x):
     return np.sin(x)
 
 def f3(x):
     return np.exp(-x**2)
 
-def f4(x):
-    return np.log(x) 
-
-def f5(x, y):
+def f4(x, y):
     return x * y
 
 # Define integration limits and number of intervals
 a = 0
 b = 10
 n = 1000
 
@@ -62,15 +59,15 @@
 result_romberg = romberg_integration(f2, a, b)
 result_gauss_legendre = gauss_legendre_quadrature(f3, a, b, 5)
 result_gauss_chebyshev = gauss_chebyshev_quadrature(f3, 5)
 result_gauss_laguerre = gauss_laguerre_quadrature(f3, 5)
 result_gauss_hermite = gauss_hermite_quadrature(f3, 5)
 result_adaptive_simpsons = adaptive_simpsons_rule(f3, a, b, 1e-6)
 result_monte_carlo = monte_carlo_integration(f3, a, b)
-result_double_integral = double_integral(f5, 0, 1, 0, 1)
+result_double_integral = double_integral(f4, 0, 1, 0, 1)
 result_simpsons_error, error_estimate = simpsons_rule_with_error(f2, a, b, n)
 
 print("Results:")
 print(f"Trapezoidal Rule: {result_trapezoidal}")
 print(f"Simpson's Rule: {result_simpsons}")
 print(f"Midpoint Rule: {result_midpoint}")
 print(f"Boole's Rule: {result_booles}")
```

### Comparing `pynumint-0.0.4/README.md` & `pynumint-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,18 +23,15 @@
 
 def f2(x):
     return np.sin(x)
 
 def f3(x):
     return np.exp(-x**2)
 
-def f4(x):
-    return np.log(x) 
-
-def f5(x, y):
+def f4(x, y):
     return x * y
 
 # Define integration limits and number of intervals
 a = 0
 b = 10
 n = 1000
 
@@ -46,15 +43,15 @@
 result_romberg = romberg_integration(f2, a, b)
 result_gauss_legendre = gauss_legendre_quadrature(f3, a, b, 5)
 result_gauss_chebyshev = gauss_chebyshev_quadrature(f3, 5)
 result_gauss_laguerre = gauss_laguerre_quadrature(f3, 5)
 result_gauss_hermite = gauss_hermite_quadrature(f3, 5)
 result_adaptive_simpsons = adaptive_simpsons_rule(f3, a, b, 1e-6)
 result_monte_carlo = monte_carlo_integration(f3, a, b)
-result_double_integral = double_integral(f5, 0, 1, 0, 1)
+result_double_integral = double_integral(f4, 0, 1, 0, 1)
 result_simpsons_error, error_estimate = simpsons_rule_with_error(f2, a, b, n)
 
 print("Results:")
 print(f"Trapezoidal Rule: {result_trapezoidal}")
 print(f"Simpson's Rule: {result_simpsons}")
 print(f"Midpoint Rule: {result_midpoint}")
 print(f"Boole's Rule: {result_booles}")
```

### Comparing `pynumint-0.0.4/pynumint/src/pynumint.egg-info/PKG-INFO` & `pynumint-0.0.5/pynumint/src/pynumint.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynumint
-Version: 0.0.4
+Version: 0.0.5
 Summary: pynumint Test Package for Numerical Integration Demo
 Home-page: https://pypi.org/project/pynumint/
 Author: Arjun Jagdale
 Author-email: arjunjagdale14@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -39,18 +39,15 @@
 
 def f2(x):
     return np.sin(x)
 
 def f3(x):
     return np.exp(-x**2)
 
-def f4(x):
-    return np.log(x) 
-
-def f5(x, y):
+def f4(x, y):
     return x * y
 
 # Define integration limits and number of intervals
 a = 0
 b = 10
 n = 1000
 
@@ -62,15 +59,15 @@
 result_romberg = romberg_integration(f2, a, b)
 result_gauss_legendre = gauss_legendre_quadrature(f3, a, b, 5)
 result_gauss_chebyshev = gauss_chebyshev_quadrature(f3, 5)
 result_gauss_laguerre = gauss_laguerre_quadrature(f3, 5)
 result_gauss_hermite = gauss_hermite_quadrature(f3, 5)
 result_adaptive_simpsons = adaptive_simpsons_rule(f3, a, b, 1e-6)
 result_monte_carlo = monte_carlo_integration(f3, a, b)
-result_double_integral = double_integral(f5, 0, 1, 0, 1)
+result_double_integral = double_integral(f4, 0, 1, 0, 1)
 result_simpsons_error, error_estimate = simpsons_rule_with_error(f2, a, b, n)
 
 print("Results:")
 print(f"Trapezoidal Rule: {result_trapezoidal}")
 print(f"Simpson's Rule: {result_simpsons}")
 print(f"Midpoint Rule: {result_midpoint}")
 print(f"Boole's Rule: {result_booles}")
```

### Comparing `pynumint-0.0.4/pynumint/src/pynumint.py` & `pynumint-0.0.5/pynumint/src/pynumint.py`

 * *Files identical despite different names*

