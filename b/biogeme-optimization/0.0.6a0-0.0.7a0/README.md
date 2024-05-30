# Comparing `tmp/biogeme-optimization-0.0.6a0.tar.gz` & `tmp/biogeme_optimization-0.0.7a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biogeme-optimization-0.0.6a0.tar", last modified: Wed Mar 27 13:04:33 2024, max compression
+gzip compressed data, was "biogeme_optimization-0.0.7a0.tar", last modified: Thu May 30 11:48:54 2024, max compression
```

## Comparing `biogeme-optimization-0.0.6a0.tar` & `biogeme_optimization-0.0.7a0.tar`

### file list

```diff
@@ -1,61 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:04:33.974361 biogeme-optimization-0.0.6a0/
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-03-27 13:04:33.974361 biogeme-optimization-0.0.6a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-03-27 13:04:33.974361 biogeme-optimization-0.0.6a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:04:33.962361 biogeme-optimization-0.0.6a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:04:33.966361 biogeme-optimization-0.0.6a0/src/biogeme_optimization/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7910 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/algebra.py
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/bfgs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/biogeme_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    33178 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    14015 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     6865 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/hybrid_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    12183 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/linesearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     8623 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/neighborhood.py
--rw-r--r--   0 runner    (1001) docker     (127)    14417 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/pareto.py
--rw-r--r--   0 runner    (1001) docker     (127)    12142 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/simple_bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)    13907 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/stochastic_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    10063 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/stochastic_simple_bounds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:04:33.970361 biogeme-optimization-0.0.6a0/src/biogeme_optimization/teaching/
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/teaching/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:04:33.970361 biogeme-optimization-0.0.6a0/src/biogeme_optimization/teaching/linear_constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/teaching/linear_constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16859 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/teaching/linear_constraints/constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)    17255 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/teaching/linear_constraints/linear_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     9257 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/teaching/linear_constraints/standard_canonical.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/teaching/linear_constraints/variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/teaching/matrices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/teaching/plot_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/teaching/polyhedron_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/teaching/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)    22515 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/trust_region.py
--rw-r--r--   0 runner    (1001) docker     (127)     8279 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/vns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:04:33.974361 biogeme-optimization-0.0.6a0/src/biogeme_optimization.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-03-27 13:04:33.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-03-27 13:04:33.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 13:04:33.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-27 13:04:33.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-27 13:04:33.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:04:33.974361 biogeme-optimization-0.0.6a0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6377 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/tests/test_algebra.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/tests/test_bfgs.py
--rw-r--r--   0 runner    (1001) docker     (127)    53852 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/tests/test_bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/tests/test_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/tests/test_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/tests/test_hybrid_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/tests/test_linear_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)    10168 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/tests/test_linesearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/tests/test_matrices.py
--rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/tests/test_neighborhood.py
--rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/tests/test_pareto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/tests/test_plot_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    10094 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/tests/test_simple_bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/tests/test_standard_canonical.py
--rw-r--r--   0 runner    (1001) docker     (127)    23343 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/tests/test_trust_region.py
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/tests/test_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/tests/test_vns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:48:54.131864 biogeme_optimization-0.0.7a0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-05-30 11:48:54.131864 biogeme_optimization-0.0.7a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-30 11:48:50.000000 biogeme_optimization-0.0.7a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-30 11:48:54.131864 biogeme_optimization-0.0.7a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-30 11:48:50.000000 biogeme_optimization-0.0.7a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:48:54.123864 biogeme_optimization-0.0.7a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:48:54.127864 biogeme_optimization-0.0.7a0/src/biogeme_optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-30 11:48:50.000000 biogeme_optimization-0.0.7a0/src/biogeme_optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7910 2024-05-30 11:48:50.000000 biogeme_optimization-0.0.7a0/src/biogeme_optimization/algebra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-05-30 11:48:50.000000 biogeme_optimization-0.0.7a0/src/biogeme_optimization/bfgs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-30 11:48:50.000000 biogeme_optimization-0.0.7a0/src/biogeme_optimization/biogeme_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33178 2024-05-30 11:48:50.000000 biogeme_optimization-0.0.7a0/src/biogeme_optimization/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-30 11:48:50.000000 biogeme_optimization-0.0.7a0/src/biogeme_optimization/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-30 11:48:50.000000 biogeme_optimization-0.0.7a0/src/biogeme_optimization/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-30 11:48:50.000000 biogeme_optimization-0.0.7a0/src/biogeme_optimization/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14015 2024-05-30 11:48:50.000000 biogeme_optimization-0.0.7a0/src/biogeme_optimization/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6865 2024-05-30 11:48:50.000000 biogeme_optimization-0.0.7a0/src/biogeme_optimization/hybrid_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12183 2024-05-30 11:48:50.000000 biogeme_optimization-0.0.7a0/src/biogeme_optimization/linesearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8623 2024-05-30 11:48:50.000000 biogeme_optimization-0.0.7a0/src/biogeme_optimization/neighborhood.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14417 2024-05-30 11:48:50.000000 biogeme_optimization-0.0.7a0/src/biogeme_optimization/pareto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12142 2024-05-30 11:48:50.000000 biogeme_optimization-0.0.7a0/src/biogeme_optimization/simple_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13907 2024-05-30 11:48:50.000000 biogeme_optimization-0.0.7a0/src/biogeme_optimization/stochastic_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10063 2024-05-30 11:48:50.000000 biogeme_optimization-0.0.7a0/src/biogeme_optimization/stochastic_simple_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22515 2024-05-30 11:48:50.000000 biogeme_optimization-0.0.7a0/src/biogeme_optimization/trust_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8279 2024-05-30 11:48:50.000000 biogeme_optimization-0.0.7a0/src/biogeme_optimization/vns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:48:54.131864 biogeme_optimization-0.0.7a0/src/biogeme_optimization.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-05-30 11:48:54.000000 biogeme_optimization-0.0.7a0/src/biogeme_optimization.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-30 11:48:54.000000 biogeme_optimization-0.0.7a0/src/biogeme_optimization.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 11:48:54.000000 biogeme_optimization-0.0.7a0/src/biogeme_optimization.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-30 11:48:54.000000 biogeme_optimization-0.0.7a0/src/biogeme_optimization.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 11:48:54.000000 biogeme_optimization-0.0.7a0/src/biogeme_optimization.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:48:54.131864 biogeme_optimization-0.0.7a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6377 2024-05-30 11:48:50.000000 biogeme_optimization-0.0.7a0/tests/test_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-30 11:48:50.000000 biogeme_optimization-0.0.7a0/tests/test_bfgs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53852 2024-05-30 11:48:50.000000 biogeme_optimization-0.0.7a0/tests/test_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-05-30 11:48:50.000000 biogeme_optimization-0.0.7a0/tests/test_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-05-30 11:48:50.000000 biogeme_optimization-0.0.7a0/tests/test_hybrid_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10168 2024-05-30 11:48:50.000000 biogeme_optimization-0.0.7a0/tests/test_linesearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-05-30 11:48:50.000000 biogeme_optimization-0.0.7a0/tests/test_neighborhood.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-05-30 11:48:50.000000 biogeme_optimization-0.0.7a0/tests/test_pareto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10094 2024-05-30 11:48:50.000000 biogeme_optimization-0.0.7a0/tests/test_simple_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23343 2024-05-30 11:48:50.000000 biogeme_optimization-0.0.7a0/tests/test_trust_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-30 11:48:50.000000 biogeme_optimization-0.0.7a0/tests/test_vns.py
```

### Comparing `biogeme-optimization-0.0.6a0/PKG-INFO` & `biogeme_optimization-0.0.7a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biogeme-optimization
-Version: 0.0.6a0
+Version: 0.0.7a0
 Summary: Various optimization algorithms for teaching and research
 Home-page: http://biogeme.epfl.ch
 Author: Michel Bierlaire
 Author-email: michel.bierlaire@epfl.ch
 Project-URL: Code, https://github.com/michelbierlaire/optimization
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Requires-Dist: numpy>=1.24.2
 Requires-Dist: scipy>=1.10.1
 Requires-Dist: matplotlib>=3.8.2
+Requires-Dist: tomlkit>=0.12.5
 Provides-Extra: testing
 Requires-Dist: pytest>=7.2.0; extra == "testing"
 Requires-Dist: pytest-cov>=4.0.0; extra == "testing"
 Requires-Dist: tox>=3.27.1; extra == "testing"
 
 # biogeme-optimization
 [![PyPi](https://img.shields.io/pypi/v/biogeme_optimization.svg)](https://pypi.python.org/pypi/biogeme_optimization)
```

### Comparing `biogeme-optimization-0.0.6a0/README.md` & `biogeme_optimization-0.0.7a0/README.md`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6a0/setup.cfg` & `biogeme_optimization-0.0.7a0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = biogeme-optimization
-version = 0.0.6a0
+version = 0.0.7a0
 description = Various optimization algorithms for teaching and research
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Michel Bierlaire
 author_email = michel.bierlaire@epfl.ch
 url = http://biogeme.epfl.ch
 download_urls = https://pypi.org/project/bierlaire-optimization
@@ -25,14 +25,15 @@
 [options]
 package_dir = =src
 packages = find:
 install_requires = 
 	numpy >= 1.24.2
 	scipy >= 1.10.1
 	matplotlib >= 3.8.2
+	tomlkit >= 0.12.5
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 testing = 
 	pytest >= 7.2.0
```

### Comparing `biogeme-optimization-0.0.6a0/src/biogeme_optimization/algebra.py` & `biogeme_optimization-0.0.7a0/src/biogeme_optimization/algebra.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6a0/src/biogeme_optimization/bfgs.py` & `biogeme_optimization-0.0.7a0/src/biogeme_optimization/bfgs.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6a0/src/biogeme_optimization/biogeme_logging.py` & `biogeme_optimization-0.0.7a0/src/biogeme_optimization/biogeme_logging.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6a0/src/biogeme_optimization/bounds.py` & `biogeme_optimization-0.0.7a0/src/biogeme_optimization/bounds.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6a0/src/biogeme_optimization/diagnostics.py` & `biogeme_optimization-0.0.7a0/src/biogeme_optimization/diagnostics.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6a0/src/biogeme_optimization/format.py` & `biogeme_optimization-0.0.7a0/src/biogeme_optimization/format.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6a0/src/biogeme_optimization/function.py` & `biogeme_optimization-0.0.7a0/src/biogeme_optimization/function.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6a0/src/biogeme_optimization/hybrid_function.py` & `biogeme_optimization-0.0.7a0/src/biogeme_optimization/hybrid_function.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6a0/src/biogeme_optimization/linesearch.py` & `biogeme_optimization-0.0.7a0/src/biogeme_optimization/linesearch.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6a0/src/biogeme_optimization/neighborhood.py` & `biogeme_optimization-0.0.7a0/src/biogeme_optimization/neighborhood.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6a0/src/biogeme_optimization/pareto.py` & `biogeme_optimization-0.0.7a0/src/biogeme_optimization/pareto.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6a0/src/biogeme_optimization/simple_bounds.py` & `biogeme_optimization-0.0.7a0/src/biogeme_optimization/simple_bounds.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6a0/src/biogeme_optimization/stochastic_function.py` & `biogeme_optimization-0.0.7a0/src/biogeme_optimization/stochastic_function.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6a0/src/biogeme_optimization/stochastic_simple_bounds.py` & `biogeme_optimization-0.0.7a0/src/biogeme_optimization/stochastic_simple_bounds.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6a0/src/biogeme_optimization/trust_region.py` & `biogeme_optimization-0.0.7a0/src/biogeme_optimization/trust_region.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6a0/src/biogeme_optimization/vns.py` & `biogeme_optimization-0.0.7a0/src/biogeme_optimization/vns.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6a0/src/biogeme_optimization.egg-info/PKG-INFO` & `biogeme_optimization-0.0.7a0/src/biogeme_optimization.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biogeme-optimization
-Version: 0.0.6a0
+Version: 0.0.7a0
 Summary: Various optimization algorithms for teaching and research
 Home-page: http://biogeme.epfl.ch
 Author: Michel Bierlaire
 Author-email: michel.bierlaire@epfl.ch
 Project-URL: Code, https://github.com/michelbierlaire/optimization
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Requires-Dist: numpy>=1.24.2
 Requires-Dist: scipy>=1.10.1
 Requires-Dist: matplotlib>=3.8.2
+Requires-Dist: tomlkit>=0.12.5
 Provides-Extra: testing
 Requires-Dist: pytest>=7.2.0; extra == "testing"
 Requires-Dist: pytest-cov>=4.0.0; extra == "testing"
 Requires-Dist: tox>=3.27.1; extra == "testing"
 
 # biogeme-optimization
 [![PyPi](https://img.shields.io/pypi/v/biogeme_optimization.svg)](https://pypi.python.org/pypi/biogeme_optimization)
```

### Comparing `biogeme-optimization-0.0.6a0/src/biogeme_optimization.egg-info/SOURCES.txt` & `biogeme_optimization-0.0.7a0/src/biogeme_optimization.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -20,34 +20,18 @@
 src/biogeme_optimization/trust_region.py
 src/biogeme_optimization/vns.py
 src/biogeme_optimization.egg-info/PKG-INFO
 src/biogeme_optimization.egg-info/SOURCES.txt
 src/biogeme_optimization.egg-info/dependency_links.txt
 src/biogeme_optimization.egg-info/requires.txt
 src/biogeme_optimization.egg-info/top_level.txt
-src/biogeme_optimization/teaching/__init__.py
-src/biogeme_optimization/teaching/matrices.py
-src/biogeme_optimization/teaching/plot_function.py
-src/biogeme_optimization/teaching/polyhedron_2d.py
-src/biogeme_optimization/teaching/variables.py
-src/biogeme_optimization/teaching/linear_constraints/__init__.py
-src/biogeme_optimization/teaching/linear_constraints/constraint.py
-src/biogeme_optimization/teaching/linear_constraints/linear_constraints.py
-src/biogeme_optimization/teaching/linear_constraints/standard_canonical.py
-src/biogeme_optimization/teaching/linear_constraints/variable.py
 tests/test_algebra.py
 tests/test_bfgs.py
 tests/test_bounds.py
-tests/test_constraints.py
 tests/test_function.py
 tests/test_hybrid_function.py
-tests/test_linear_constraints.py
 tests/test_linesearch.py
-tests/test_matrices.py
 tests/test_neighborhood.py
 tests/test_pareto.py
-tests/test_plot_function.py
 tests/test_simple_bounds.py
-tests/test_standard_canonical.py
 tests/test_trust_region.py
-tests/test_variables.py
 tests/test_vns.py
```

### Comparing `biogeme-optimization-0.0.6a0/tests/test_algebra.py` & `biogeme_optimization-0.0.7a0/tests/test_algebra.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6a0/tests/test_bfgs.py` & `biogeme_optimization-0.0.7a0/tests/test_bfgs.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6a0/tests/test_bounds.py` & `biogeme_optimization-0.0.7a0/tests/test_bounds.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6a0/tests/test_function.py` & `biogeme_optimization-0.0.7a0/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6a0/tests/test_hybrid_function.py` & `biogeme_optimization-0.0.7a0/tests/test_hybrid_function.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6a0/tests/test_linesearch.py` & `biogeme_optimization-0.0.7a0/tests/test_linesearch.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6a0/tests/test_neighborhood.py` & `biogeme_optimization-0.0.7a0/tests/test_neighborhood.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6a0/tests/test_pareto.py` & `biogeme_optimization-0.0.7a0/tests/test_pareto.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6a0/tests/test_simple_bounds.py` & `biogeme_optimization-0.0.7a0/tests/test_simple_bounds.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6a0/tests/test_trust_region.py` & `biogeme_optimization-0.0.7a0/tests/test_trust_region.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6a0/tests/test_vns.py` & `biogeme_optimization-0.0.7a0/tests/test_vns.py`

 * *Files identical despite different names*

