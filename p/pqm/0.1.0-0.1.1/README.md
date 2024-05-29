# Comparing `tmp/pqm-0.1.0.tar.gz` & `tmp/pqm-0.1.1.tar.gz`

## Comparing `pqm-0.1.0.tar` & `pqm-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 pqm-0.1.0/requirements.txt
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 pqm-0.1.0/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 pqm-0.1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 pqm-0.1.0/src/.gitignore
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pqm-0.1.0/src/pqm/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pqm-0.1.0/src/pqm/_version.py
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 pqm-0.1.0/src/pqm/pqm.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 pqm-0.1.0/src/pqm/test_gaussian.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 pqm-0.1.0/tests/test_gaussian.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 pqm-0.1.0/LICENSE
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pqm-0.1.0/README.md
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 pqm-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 pqm-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 pqm-0.1.1/requirements.txt
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 pqm-0.1.1/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 pqm-0.1.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 pqm-0.1.1/src/pqm/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pqm-0.1.1/src/pqm/_version.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 pqm-0.1.1/src/pqm/pqm.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 pqm-0.1.1/src/pqm/test_gaussian.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 pqm-0.1.1/tests/test_gaussian.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 pqm-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 pqm-0.1.1/LICENSE
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 pqm-0.1.1/README.md
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 pqm-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 pqm-0.1.1/PKG-INFO
```

### Comparing `pqm-0.1.0/.github/workflows/cd.yml` & `pqm-0.1.1/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `pqm-0.1.0/.github/workflows/ci.yml` & `pqm-0.1.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pqm-0.1.0/src/pqm/pqm.py` & `pqm-0.1.1/src/pqm/pqm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import Optional
 
 import numpy as np
 from scipy.stats import chi2_contingency
 from scipy.spatial import KDTree
 
-__all__ = "get_pqm_pvalue"
+__all__ = "pqm_pvalue"
 
 
-def get_pqm_pvalue(
+def pqm_pvalue(
     x_samples: np.ndarray,
     y_samples: np.ndarray,
     num_refs: int = 100,
     bootstrap: Optional[int] = None,
 ):
     """
     Perform the PQM test of the null hypothesis that `x_samples` and `y_samples` are drawn form the same distribution.
@@ -29,17 +29,15 @@
 
     Returns
     -------
     float
         pvalue. Null hypothesis that both samples are drawn from the same distribution.
     """
     if bootstrap is not None:
-        return list(
-            get_pqm_pvalue(x_samples, y_samples, num_refs=num_refs) for _ in range(bootstrap)
-        )
+        return list(pqm_pvalue(x_samples, y_samples, num_refs=num_refs) for _ in range(bootstrap))
     if len(y_samples) < num_refs:
         raise ValueError(
             "Number of reference samples must be less than the number of true samples."
         )
     elif len(y_samples) < 2 * num_refs:
         print(
             "Warning: Number of y_samples is small (less than twice the number of reference samples). Result may have high variance."
```

### Comparing `pqm-0.1.0/LICENSE` & `pqm-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pqm-0.1.0/pyproject.toml` & `pqm-0.1.1/pyproject.toml`

 * *Files identical despite different names*

