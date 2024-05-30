# Comparing `tmp/mercury-robust-0.0.2.tar.gz` & `tmp/mercury_robust-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercury-robust-0.0.2.tar", last modified: Tue May  9 09:01:08 2023, max compression
+gzip compressed data, was "mercury_robust-0.0.3.tar", last modified: Thu May 30 08:31:56 2024, max compression
```

## Comparing `mercury-robust-0.0.2.tar` & `mercury_robust-0.0.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:01:08.467048 mercury-robust-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-09 09:00:57.000000 mercury-robust-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-05-09 09:01:08.467048 mercury-robust-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-05-09 09:00:57.000000 mercury-robust-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:01:08.463048 mercury-robust-0.0.2/mercury/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:01:08.463048 mercury-robust-0.0.2/mercury/robust/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-09 09:00:57.000000 mercury-robust-0.0.2/mercury/robust/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-05-09 09:00:57.000000 mercury-robust-0.0.2/mercury/robust/_category_struct.py
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-05-09 09:00:57.000000 mercury-robust-0.0.2/mercury/robust/_label_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-05-09 09:00:57.000000 mercury-robust-0.0.2/mercury/robust/_linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-05-09 09:00:57.000000 mercury-robust-0.0.2/mercury/robust/_tree_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-05-09 09:00:57.000000 mercury-robust-0.0.2/mercury/robust/_treeselector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-09 09:00:57.000000 mercury-robust-0.0.2/mercury/robust/basetests.py
--rw-r--r--   0 runner    (1001) docker     (123)    50444 2023-05-09 09:00:57.000000 mercury-robust-0.0.2/mercury/robust/data_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-09 09:00:57.000000 mercury-robust-0.0.2/mercury/robust/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    59316 2023-05-09 09:00:57.000000 mercury-robust-0.0.2/mercury/robust/model_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-09 09:00:57.000000 mercury-robust-0.0.2/mercury/robust/suite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:01:08.467048 mercury-robust-0.0.2/mercury_robust.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-05-09 09:01:08.000000 mercury-robust-0.0.2/mercury_robust.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-09 09:01:08.000000 mercury-robust-0.0.2/mercury_robust.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 09:01:08.000000 mercury-robust-0.0.2/mercury_robust.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-09 09:01:08.000000 mercury-robust-0.0.2/mercury_robust.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 09:01:08.000000 mercury-robust-0.0.2/mercury_robust.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-09 09:00:57.000000 mercury-robust-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 09:01:08.467048 mercury-robust-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:01:08.467048 mercury-robust-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-09 09:00:57.000000 mercury-robust-0.0.2/tests/test_basetests.py
--rw-r--r--   0 runner    (1001) docker     (123)    28586 2023-05-09 09:00:57.000000 mercury-robust-0.0.2/tests/test_data_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    35938 2023-05-09 09:00:57.000000 mercury-robust-0.0.2/tests/test_model_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-09 09:00:57.000000 mercury-robust-0.0.2/tests/test_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:31:56.589188 mercury_robust-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-30 08:31:49.000000 mercury_robust-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-30 08:31:56.589188 mercury_robust-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-30 08:31:49.000000 mercury_robust-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:31:56.581188 mercury_robust-0.0.3/mercury/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:31:56.585188 mercury_robust-0.0.3/mercury/robust/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-30 08:31:49.000000 mercury_robust-0.0.3/mercury/robust/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6754 2024-05-30 08:31:49.000000 mercury_robust-0.0.3/mercury/robust/_category_struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-05-30 08:31:49.000000 mercury_robust-0.0.3/mercury/robust/_label_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-30 08:31:49.000000 mercury_robust-0.0.3/mercury/robust/_linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6016 2024-05-30 08:31:49.000000 mercury_robust-0.0.3/mercury/robust/_tree_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-30 08:31:49.000000 mercury_robust-0.0.3/mercury/robust/_treeselector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-30 08:31:49.000000 mercury_robust-0.0.3/mercury/robust/basetests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50913 2024-05-30 08:31:49.000000 mercury_robust-0.0.3/mercury/robust/data_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-30 08:31:49.000000 mercury_robust-0.0.3/mercury/robust/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59316 2024-05-30 08:31:49.000000 mercury_robust-0.0.3/mercury/robust/model_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-05-30 08:31:49.000000 mercury_robust-0.0.3/mercury/robust/suite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:31:56.585188 mercury_robust-0.0.3/mercury_robust.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-30 08:31:56.000000 mercury_robust-0.0.3/mercury_robust.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-30 08:31:56.000000 mercury_robust-0.0.3/mercury_robust.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 08:31:56.000000 mercury_robust-0.0.3/mercury_robust.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-30 08:31:56.000000 mercury_robust-0.0.3/mercury_robust.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-30 08:31:56.000000 mercury_robust-0.0.3/mercury_robust.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-30 08:31:49.000000 mercury_robust-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 08:31:56.589188 mercury_robust-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:31:56.585188 mercury_robust-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-30 08:31:49.000000 mercury_robust-0.0.3/tests/test_basetests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29184 2024-05-30 08:31:49.000000 mercury_robust-0.0.3/tests/test_data_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35938 2024-05-30 08:31:49.000000 mercury_robust-0.0.3/tests/test_model_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-30 08:31:49.000000 mercury_robust-0.0.3/tests/test_suite.py
```

### Comparing `mercury-robust-0.0.2/LICENSE` & `mercury_robust-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mercury-robust-0.0.2/PKG-INFO` & `mercury_robust-0.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,11 @@
-Metadata-Version: 2.1
-Name: mercury-robust
-Version: 0.0.2
-Summary: Mercury's robust is a library to perform robust testing on models and/or datasets..
-Author-email: Mercury Team <mercury.group@bbva.com>
-Project-URL: Homepage, https://github.com/BBVA/mercury-robust
-Project-URL: Bug Tracker, https://github.com/BBVA/mercury-robust/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: doc
-License-File: LICENSE
-
 # mercury-robust
 
 [![](https://github.com/BBVA/mercury-robust/actions/workflows/test.yml/badge.svg)](https://github.com/BBVA/mercury-robust)
-![](https://img.shields.io/badge/latest-0.0.2-blue)
+![](https://img.shields.io/badge/latest-0.0.3-blue)
 
 ## Mercury project at BBVA
 
 Mercury is a collaborative library that was developed by the Advanced Analytics community at BBVA. Originally, it was created as an [InnerSource](https://en.wikipedia.org/wiki/Inner_source) project but after some time, we decided to release certain parts of the project as Open Source.
 That's the case with the `mercury-robust` package. 
 
 If you're interested in learning more about the Mercury project, we recommend reading this blog [post](https://www.bbvaaifactory.com/mercury-acelerando-la-reutilizacion-en-ciencia-de-datos-dentro-de-bbva/) from www.bbvaaifactory.com
@@ -82,14 +66,14 @@
 
 The easiest way to install `mercury-robust` is using ``pip``:
 
     pip install -U mercury-robust
 
 ## Help and support 
 
-This library is currently maintained by a dedicated team of data scientists and machine learning engineers from BBVA AI Factory. 
+This library is currently maintained by a dedicated team of data scientists and machine learning engineers from BBVA. 
 
 ### Documentation
 website: https://bbva.github.io/mercury-robust/
 
 ### Email 
 mercury.group@bbva.com
```

### Comparing `mercury-robust-0.0.2/mercury/robust/_category_struct.py` & `mercury_robust-0.0.3/mercury/robust/_category_struct.py`

 * *Files identical despite different names*

### Comparing `mercury-robust-0.0.2/mercury/robust/_label_cleaning.py` & `mercury_robust-0.0.3/mercury/robust/_label_cleaning.py`

 * *Files identical despite different names*

### Comparing `mercury-robust-0.0.2/mercury/robust/_linalg.py` & `mercury_robust-0.0.3/mercury/robust/_linalg.py`

 * *Files identical despite different names*

### Comparing `mercury-robust-0.0.2/mercury/robust/_tree_analysis.py` & `mercury_robust-0.0.3/mercury/robust/_tree_analysis.py`

 * *Files identical despite different names*

### Comparing `mercury-robust-0.0.2/mercury/robust/_treeselector.py` & `mercury_robust-0.0.3/mercury/robust/_treeselector.py`

 * *Files identical despite different names*

### Comparing `mercury-robust-0.0.2/mercury/robust/basetests.py` & `mercury_robust-0.0.3/mercury/robust/basetests.py`

 * *Files identical despite different names*

### Comparing `mercury-robust-0.0.2/mercury/robust/data_tests.py` & `mercury_robust-0.0.3/mercury/robust/data_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,22 @@
             cont_cols = self.base_dataset.loc[:, numeric_feats].values
 
             lin_combinations = lin_combs_in_columns(
                 np.matmul(cont_cols.T, cont_cols)  # Compress original matrix
             )
 
         if lin_combinations is not None:
-            raise FailedTestError("Test failed. Linear combinations for continuous features were encountered.")
+            # Create message with the linear combinations found
+            lin_combinations = np.around(lin_combinations, decimals=5)
+            lin_combs_found = []
+            for i in range(lin_combinations.shape[0]):
+                lin_comb_idx = np.where(lin_combinations[i] != 0)[0]
+                lin_comb_cols = self.base_dataset.loc[:, numeric_feats].columns[lin_comb_idx].tolist()
+                lin_combs_found.append(lin_comb_cols)
+            raise FailedTestError(f"Test failed. Linear combinations for continuous features were encountered: {lin_combs_found}.")
 
         individually_redundant = CategoryStruct.individually_redundant(self.base_dataset, current_schema.categorical_feats)
         if len(individually_redundant) > 0:
             raise FailedTestError((
                 f"""Test failed. Any of these categorical variables is redundant: {individually_redundant}. """
                 """Try deleting any of them."""
             ))
```

### Comparing `mercury-robust-0.0.2/mercury/robust/model_tests.py` & `mercury_robust-0.0.3/mercury/robust/model_tests.py`

 * *Files identical despite different names*

### Comparing `mercury-robust-0.0.2/mercury/robust/suite.py` & `mercury_robust-0.0.3/mercury/robust/suite.py`

 * *Files identical despite different names*

### Comparing `mercury-robust-0.0.2/mercury_robust.egg-info/PKG-INFO` & `mercury_robust-0.0.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,46 @@
 Metadata-Version: 2.1
 Name: mercury-robust
-Version: 0.0.2
+Version: 0.0.3
 Summary: Mercury's robust is a library to perform robust testing on models and/or datasets..
 Author-email: Mercury Team <mercury.group@bbva.com>
 Project-URL: Homepage, https://github.com/BBVA/mercury-robust
 Project-URL: Bug Tracker, https://github.com/BBVA/mercury-robust/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: matplotlib>=3.0.2
+Requires-Dist: pandas>=0.24.2
+Requires-Dist: scikit-learn>=0.23.1
+Requires-Dist: seaborn
+Requires-Dist: mercury-dataschema
+Requires-Dist: mercury-monitoring
+Requires-Dist: psutil
+Requires-Dist: cleanlab
 Provides-Extra: dev
+Requires-Dist: tensorflow<2.11; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: xgboost; extra == "dev"
+Requires-Dist: mercury-explainability; extra == "dev"
 Provides-Extra: doc
-License-File: LICENSE
+Requires-Dist: mkdocs; extra == "doc"
+Requires-Dist: mkdocstrings[python]; extra == "doc"
+Requires-Dist: mkdocs-material; extra == "doc"
+Requires-Dist: mkdocs-minify-plugin==0.5.0; extra == "doc"
+Requires-Dist: mkdocs-exclude; extra == "doc"
+Requires-Dist: nbconvert; extra == "doc"
 
 # mercury-robust
 
 [![](https://github.com/BBVA/mercury-robust/actions/workflows/test.yml/badge.svg)](https://github.com/BBVA/mercury-robust)
-![](https://img.shields.io/badge/latest-0.0.2-blue)
+![](https://img.shields.io/badge/latest-0.0.3-blue)
 
 ## Mercury project at BBVA
 
 Mercury is a collaborative library that was developed by the Advanced Analytics community at BBVA. Originally, it was created as an [InnerSource](https://en.wikipedia.org/wiki/Inner_source) project but after some time, we decided to release certain parts of the project as Open Source.
 That's the case with the `mercury-robust` package. 
 
 If you're interested in learning more about the Mercury project, we recommend reading this blog [post](https://www.bbvaaifactory.com/mercury-acelerando-la-reutilizacion-en-ciencia-de-datos-dentro-de-bbva/) from www.bbvaaifactory.com
@@ -82,14 +101,14 @@
 
 The easiest way to install `mercury-robust` is using ``pip``:
 
     pip install -U mercury-robust
 
 ## Help and support 
 
-This library is currently maintained by a dedicated team of data scientists and machine learning engineers from BBVA AI Factory. 
+This library is currently maintained by a dedicated team of data scientists and machine learning engineers from BBVA. 
 
 ### Documentation
 website: https://bbva.github.io/mercury-robust/
 
 ### Email 
 mercury.group@bbva.com
```

### Comparing `mercury-robust-0.0.2/mercury_robust.egg-info/SOURCES.txt` & `mercury_robust-0.0.3/mercury_robust.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mercury-robust-0.0.2/pyproject.toml` & `mercury_robust-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mercury-robust"
 license = {file = "LICENSE.txt"}
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Mercury Team", email="mercury.group@bbva.com" },
 ]
 description = "Mercury's robust is a library to perform robust testing on models and/or datasets.."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `mercury-robust-0.0.2/tests/test_basetests.py` & `mercury_robust-0.0.3/tests/test_basetests.py`

 * *Files identical despite different names*

### Comparing `mercury-robust-0.0.2/tests/test_data_tests.py` & `mercury_robust-0.0.3/tests/test_data_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -853,8 +853,24 @@
         test.run()
 
     # Check it works ignoring some features
     test = NoDuplicatesTest(test_df, ignore_feats=[2])
     with pytest.raises(FailedTestError):
         test.run()
 
+def test_lin_combinations_cont():
 
+    df = pd.DataFrame()
+    df["f1"] = np.random.uniform(size=100)
+    df["f2"] = df["f1"] * 2
+    df["f3"] = np.random.uniform(size=100)
+    df["f4"] = df["f1"] + df["f2"]
+    df["f5"] = np.random.uniform(size=100)
+
+    df["f6"] = np.random.uniform(size=100)
+    df["f7"] = df["f6"] * 3
+    df["f8"] = df["f6"] * 0.1
+
+    schma_reference = DataSchema().generate(df).calculate_statistics()
+    linear_comb_test = LinearCombinationsTest(df, dataset_schema=schma_reference)
+    with pytest.raises(FailedTestError, match="'f1', 'f2'"):
+        linear_comb_test.run()
```

### Comparing `mercury-robust-0.0.2/tests/test_model_tests.py` & `mercury_robust-0.0.3/tests/test_model_tests.py`

 * *Files identical despite different names*

### Comparing `mercury-robust-0.0.2/tests/test_suite.py` & `mercury_robust-0.0.3/tests/test_suite.py`

 * *Files identical despite different names*

