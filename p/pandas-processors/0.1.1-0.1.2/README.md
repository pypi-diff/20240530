# Comparing `tmp/pandas_processors-0.1.1.tar.gz` & `tmp/pandas_processors-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas_processors-0.1.1.tar", max compression
+gzip compressed data, was "pandas_processors-0.1.2.tar", max compression
```

## Comparing `pandas_processors-0.1.1.tar` & `pandas_processors-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       95 2024-05-24 00:52:11.697552 pandas_processors-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-05-08 21:02:12.761818 pandas_processors-0.1.1/pandas_processors/__init__.py
--rw-r--r--   0        0        0     2887 2024-05-22 18:28:31.471607 pandas_processors-0.1.1/pandas_processors/_utils.py
--rw-r--r--   0        0        0     7961 2024-05-24 00:52:20.382935 pandas_processors-0.1.1/pandas_processors/create.py
--rw-r--r--   0        0        0     8704 2024-05-24 00:52:20.385238 pandas_processors-0.1.1/pandas_processors/impute.py
--rw-r--r--   0        0        0     3568 2024-05-24 00:52:20.392593 pandas_processors-0.1.1/pandas_processors/normalize.py
--rw-r--r--   0        0        0     1172 2024-05-24 16:42:22.955126 pandas_processors-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      894 1970-01-01 00:00:00.000000 pandas_processors-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       95 2024-05-24 00:52:11.697552 pandas_processors-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-08 21:02:12.761818 pandas_processors-0.1.2/pandas_processors/__init__.py
+-rw-r--r--   0        0        0     2887 2024-05-22 18:28:31.471607 pandas_processors-0.1.2/pandas_processors/_utils.py
+-rw-r--r--   0        0        0     7961 2024-05-24 00:52:20.382935 pandas_processors-0.1.2/pandas_processors/create.py
+-rw-r--r--   0        0        0     7218 2024-05-30 13:38:38.604729 pandas_processors-0.1.2/pandas_processors/impute.py
+-rw-r--r--   0        0        0     3568 2024-05-24 00:52:20.392593 pandas_processors-0.1.2/pandas_processors/normalize.py
+-rw-r--r--   0        0        0     1260 2024-05-30 15:18:13.780856 pandas_processors-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      974 1970-01-01 00:00:00.000000 pandas_processors-0.1.2/PKG-INFO
```

### Comparing `pandas_processors-0.1.1/pandas_processors/_utils.py` & `pandas_processors-0.1.2/pandas_processors/_utils.py`

 * *Files identical despite different names*

### Comparing `pandas_processors-0.1.1/pandas_processors/create.py` & `pandas_processors-0.1.2/pandas_processors/create.py`

 * *Files identical despite different names*

### Comparing `pandas_processors-0.1.1/pandas_processors/impute.py` & `pandas_processors-0.1.2/pandas_processors/impute.py`

 * *Files 13% similar despite different names*

```diff
@@ -243,55 +243,11 @@
             df[columns_] = df[columns_].fillna(df[columns_].mode().iloc[0])
         else:
             raise ValueError('imputation_method must be "missing" or "mode"')
 
         return df
 
 
-def impute_data(df: pd.DataFrame, imputers: list[DataFrameImputer]) -> pd.DataFrame:
-    """
-    Impute missing values in a DataFrame using multiple imputation strategies.
-
-    Parameters
-    ----------
-    df : pandas.DataFrame
-        The DataFrame to impute.
-    imputers : list of DataFrameImputer
-        A list of imputer objects implementing the `impute` method.
-
-    Returns
-    -------
-    pandas.DataFrame
-        The DataFrame with missing values imputed.
-
-    Examples
-    --------
-    >>> import pandas as pd
-    >>> from pandas_processors.impute import MeanMedianImputer, ConstantImputer, CategoryImputer
-    >>> df = pd.DataFrame({
-    ...     'A': [1, 2, None, 4],
-    ...     'B': [5, None, 7, 8],
-    ...     'C': ['a', None, 'c', 'd'],
-    ...     'D': [None, 'e', 'f', None]
-    ... })
-    >>> mean_imputer = MeanMedianImputer(columns=['A', 'B'], imputation_method='mean')
-    >>> constant_imputer = ConstantImputer(columns=['C'], value='Missing')
-    >>> category_imputer = CategoryImputer(columns=['D'], imputation_method='mode', fill_value='Unknown')
-    >>> imputers = [mean_imputer, constant_imputer, category_imputer]
-    >>> imputed_df = impute_data(df, imputers)
-    >>> imputed_df
-              A         B        C  D
-    0  1.000000  5.000000        a  e
-    1  2.000000  6.666667  Missing  e
-    2  2.333333  7.000000        c  f
-    3  4.000000  8.000000        d  e
-    """
-    for imputer in imputers:
-        df = imputer.impute(df)
-
-    return df
-
-
 if __name__ == "__main__":
     import doctest
 
     doctest.testmod()
```

### Comparing `pandas_processors-0.1.1/pandas_processors/normalize.py` & `pandas_processors-0.1.2/pandas_processors/normalize.py`

 * *Files identical despite different names*

### Comparing `pandas_processors-0.1.1/pyproject.toml` & `pandas_processors-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 [tool.poetry]
 name = "pandas-processors"
-version = "0.1.1"
+version = "0.1.2"
 description = "A Python library that provides utilities to process your pandas DataFrame."
 authors = ["khuyentran1401 <khuyentran1476@gmail.com>"]
 repository = "https://github.com/khuyentran1401/pandas-processors.git"
 readme = "README.md"
+documentation = "https://khuyentran1401.github.io/pandas-processors/"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pandas = "^2.2.2"
 scikit-learn = "^1.4.2"
 scipy = "^1.13.0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.7.0"
 mypy = "^1.10.0"
 pandas-stubs = "^2.2.2.240514"
+pdoc3 = "^0.10.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 ignore = ["E501"]
```

### Comparing `pandas_processors-0.1.1/PKG-INFO` & `pandas_processors-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pandas-processors
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python library that provides utilities to process your pandas DataFrame.
 Home-page: https://github.com/khuyentran1401/pandas-processors.git
 Author: khuyentran1401
 Author-email: khuyentran1476@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: scikit-learn (>=1.4.2,<2.0.0)
 Requires-Dist: scipy (>=1.13.0,<2.0.0)
+Project-URL: Documentation, https://khuyentran1401.github.io/pandas-processors/
 Project-URL: Repository, https://github.com/khuyentran1401/pandas-processors.git
 Description-Content-Type: text/markdown
 
 # pandas-processors
 
 A Python library that provides utilities to process your pandas DataFrame.
```

