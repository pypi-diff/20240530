# Comparing `tmp/pynumint-0.0.3.tar.gz` & `tmp/pynumint-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynumint-0.0.3.tar", last modified: Thu May 30 07:03:09 2024, max compression
+gzip compressed data, was "pynumint-0.0.4.tar", last modified: Thu May 30 07:11:11 2024, max compression
```

## Comparing `pynumint-0.0.3.tar` & `pynumint-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 07:03:09.579182 pynumint-0.0.3/
--rw-rw-rw-   0        0        0     1091 2024-05-26 10:33:54.000000 pynumint-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     4035 2024-05-30 07:03:09.579182 pynumint-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3594 2024-05-30 07:00:47.000000 pynumint-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 07:03:09.499196 pynumint-0.0.3/pynumint/
-drwxrwxrwx   0        0        0        0 2024-05-30 07:03:09.569185 pynumint-0.0.3/pynumint/src/
-drwxrwxrwx   0        0        0        0 2024-05-30 07:03:09.569185 pynumint-0.0.3/pynumint/src/pynumint.egg-info/
--rw-rw-rw-   0        0        0     4035 2024-05-30 07:03:09.000000 pynumint-0.0.3/pynumint/src/pynumint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2024-05-30 07:03:09.000000 pynumint-0.0.3/pynumint/src/pynumint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 07:03:09.000000 pynumint-0.0.3/pynumint/src/pynumint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-30 07:03:09.000000 pynumint-0.0.3/pynumint/src/pynumint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4237 2024-05-30 07:02:13.000000 pynumint-0.0.3/pynumint/src/pynumint.py
--rw-rw-rw-   0        0        0       42 2024-05-30 07:03:09.579182 pynumint-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1240 2024-05-30 06:47:50.000000 pynumint-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 07:11:11.583019 pynumint-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2024-05-26 10:33:54.000000 pynumint-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     4015 2024-05-30 07:11:11.583019 pynumint-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3507 2024-05-30 07:09:22.000000 pynumint-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 07:11:11.185218 pynumint-0.0.4/pynumint/
+drwxrwxrwx   0        0        0        0 2024-05-30 07:11:11.583019 pynumint-0.0.4/pynumint/src/
+drwxrwxrwx   0        0        0        0 2024-05-30 07:11:11.582214 pynumint-0.0.4/pynumint/src/pynumint.egg-info/
+-rw-rw-rw-   0        0        0     4015 2024-05-30 07:11:11.000000 pynumint-0.0.4/pynumint/src/pynumint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2024-05-30 07:11:11.000000 pynumint-0.0.4/pynumint/src/pynumint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 07:11:11.000000 pynumint-0.0.4/pynumint/src/pynumint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-30 07:11:11.000000 pynumint-0.0.4/pynumint/src/pynumint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4237 2024-05-30 07:02:13.000000 pynumint-0.0.4/pynumint/src/pynumint.py
+-rw-rw-rw-   0        0        0       42 2024-05-30 07:11:11.583019 pynumint-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1354 2024-05-30 07:10:34.000000 pynumint-0.0.4/setup.py
```

### Comparing `pynumint-0.0.3/LICENSE` & `pynumint-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pynumint-0.0.3/PKG-INFO` & `pynumint-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,27 @@
 Metadata-Version: 2.1
 Name: pynumint
-Version: 0.0.3
+Version: 0.0.4
 Summary: pynumint Test Package for Numerical Integration Demo
-Home-page: UNKNOWN
+Home-page: https://pypi.org/project/pynumint/
 Author: Arjun Jagdale
+Author-email: arjunjagdale14@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pynumint: A Numerical Integration Library
 
 pynumint is a Python library for numerical integration methods.
-pynumint offers a wide range of numerical integration methods, including :
-1] trapezoidal rule 
-2] Simpson's rule 
-3] midpoint rule 
-4] Boole's rule 
-5] Romberg integration
-6] Gauss-Legendre quadrature 
-7] Gauss-Chebyshev quadrature
-8] Gauss-Laguerre quadrature
-9] Gauss-Hermite quadrature 
-10] adaptive Simpson's rule 
-11] Monte Carlo integration
-12] double integrals
-13] Simpson's rule with error estimation
-Users can choose the most suitable method based on the characteristics of the function and the desired level of accuracy.
+pynumint offers a wide range of numerical integration methods, including trapezoidal rule, Simpson's rule, midpoint rule, Boole's rule, Romberg integration, Gauss-Legendre quadrature, Gauss-Chebyshev quadrature, Gauss-Laguerre quadrature, Gauss-Hermite quadrature, adaptive Simpson's rule, Monte Carlo integration, and double integrals. Users can choose the most suitable method based on the characteristics of the function and the desired level of accuracy.
 
 ## Installation
 
 ```bash
 pip install pynumint
```

### Comparing `pynumint-0.0.3/README.md` & `pynumint-0.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,11 @@
 # pynumint: A Numerical Integration Library
 
 pynumint is a Python library for numerical integration methods.
-pynumint offers a wide range of numerical integration methods, including :
-1] trapezoidal rule 
-2] Simpson's rule 
-3] midpoint rule 
-4] Boole's rule 
-5] Romberg integration
-6] Gauss-Legendre quadrature 
-7] Gauss-Chebyshev quadrature
-8] Gauss-Laguerre quadrature
-9] Gauss-Hermite quadrature 
-10] adaptive Simpson's rule 
-11] Monte Carlo integration
-12] double integrals
-13] Simpson's rule with error estimation
-Users can choose the most suitable method based on the characteristics of the function and the desired level of accuracy.
+pynumint offers a wide range of numerical integration methods, including trapezoidal rule, Simpson's rule, midpoint rule, Boole's rule, Romberg integration, Gauss-Legendre quadrature, Gauss-Chebyshev quadrature, Gauss-Laguerre quadrature, Gauss-Hermite quadrature, adaptive Simpson's rule, Monte Carlo integration, and double integrals. Users can choose the most suitable method based on the characteristics of the function and the desired level of accuracy.
 
 ## Installation
 
 ```bash
 pip install pynumint
```

### Comparing `pynumint-0.0.3/pynumint/src/pynumint.egg-info/PKG-INFO` & `pynumint-0.0.4/pynumint/src/pynumint.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,27 @@
 Metadata-Version: 2.1
 Name: pynumint
-Version: 0.0.3
+Version: 0.0.4
 Summary: pynumint Test Package for Numerical Integration Demo
-Home-page: UNKNOWN
+Home-page: https://pypi.org/project/pynumint/
 Author: Arjun Jagdale
+Author-email: arjunjagdale14@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pynumint: A Numerical Integration Library
 
 pynumint is a Python library for numerical integration methods.
-pynumint offers a wide range of numerical integration methods, including :
-1] trapezoidal rule 
-2] Simpson's rule 
-3] midpoint rule 
-4] Boole's rule 
-5] Romberg integration
-6] Gauss-Legendre quadrature 
-7] Gauss-Chebyshev quadrature
-8] Gauss-Laguerre quadrature
-9] Gauss-Hermite quadrature 
-10] adaptive Simpson's rule 
-11] Monte Carlo integration
-12] double integrals
-13] Simpson's rule with error estimation
-Users can choose the most suitable method based on the characteristics of the function and the desired level of accuracy.
+pynumint offers a wide range of numerical integration methods, including trapezoidal rule, Simpson's rule, midpoint rule, Boole's rule, Romberg integration, Gauss-Legendre quadrature, Gauss-Chebyshev quadrature, Gauss-Laguerre quadrature, Gauss-Hermite quadrature, adaptive Simpson's rule, Monte Carlo integration, and double integrals. Users can choose the most suitable method based on the characteristics of the function and the desired level of accuracy.
 
 ## Installation
 
 ```bash
 pip install pynumint
```

### Comparing `pynumint-0.0.3/pynumint/src/pynumint.py` & `pynumint-0.0.4/pynumint/src/pynumint.py`

 * *Files identical despite different names*

### Comparing `pynumint-0.0.3/setup.py` & `pynumint-0.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pynumint",                     # This is the name of the package
-    version="0.0.3",                        # The initial release version
-    author="Arjun Jagdale",                     # Full name of the author
+    version="0.0.4",                     # The initial release version
+    author="Arjun Jagdale",              # Full name of the author
+    author_email="arjunjagdale14@gmail.com",  # Author's email address
     description="pynumint Test Package for Numerical Integration Demo",
-    long_description=long_description,      # Long description read from the the readme file
+    long_description=long_description,   # Long description read from the readme file
     long_description_content_type="text/markdown",
-    packages=setuptools.find_packages(),    # List of all python modules to be installed
+    url="https://pypi.org/project/pynumint/",  # URL of the project
+    packages=setuptools.find_packages(), # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
-    ],                                      # Information to filter the project on PyPi website
-    python_requires='>=3.6',                # Minimum version requirement of the package
+    ],                                   # Information to filter the project on PyPi website
+    python_requires='>=3.6',             # Minimum version requirement of the package
     py_modules=["pynumint"],             # Name of the python package
-    package_dir={'':'pynumint/src'},     # Directory of the source code of the package
-    install_requires=[]                     # Install other dependencies if any
-)
+    package_dir={'': 'pynumint/src'},    # Directory of the source code of the package
+    install_requires=[]                  # Install other dependencies if any
+)
```

