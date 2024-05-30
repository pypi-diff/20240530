# Comparing `tmp/phstatsmethods-0.1.8.tar.gz` & `tmp/phstatsmethods-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phstatsmethods-0.1.8.tar", last modified: Wed May 22 10:16:49 2024, max compression
+gzip compressed data, was "phstatsmethods-0.1.9.tar", last modified: Wed May 22 10:24:50 2024, max compression
```

## Comparing `phstatsmethods-0.1.8.tar` & `phstatsmethods-0.1.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:16:49.741615 phstatsmethods-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35170 2024-05-22 10:16:46.000000 phstatsmethods-0.1.8/LICENSE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:16:49.737615 phstatsmethods-0.1.8/PHStatsMethods/
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-22 10:16:46.000000 phstatsmethods-0.1.8/PHStatsMethods/DSR.py
--rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-05-22 10:16:46.000000 phstatsmethods-0.1.8/PHStatsMethods/ISRate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-05-22 10:16:46.000000 phstatsmethods-0.1.8/PHStatsMethods/ISRatio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-22 10:16:46.000000 phstatsmethods-0.1.8/PHStatsMethods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-05-22 10:16:46.000000 phstatsmethods-0.1.8/PHStatsMethods/confidence_intervals.py
--rw-r--r--   0 runner    (1001) docker     (127)    16953 2024-05-22 10:16:46.000000 phstatsmethods-0.1.8/PHStatsMethods/funnels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-22 10:16:46.000000 phstatsmethods-0.1.8/PHStatsMethods/means.py
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-22 10:16:46.000000 phstatsmethods-0.1.8/PHStatsMethods/proportions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-22 10:16:46.000000 phstatsmethods-0.1.8/PHStatsMethods/quantiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-22 10:16:46.000000 phstatsmethods-0.1.8/PHStatsMethods/rates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-22 10:16:46.000000 phstatsmethods-0.1.8/PHStatsMethods/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-05-22 10:16:46.000000 phstatsmethods-0.1.8/PHStatsMethods/utils_funnel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7413 2024-05-22 10:16:46.000000 phstatsmethods-0.1.8/PHStatsMethods/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:16:49.741615 phstatsmethods-0.1.8/PHStatsMethods.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-22 10:16:49.000000 phstatsmethods-0.1.8/PHStatsMethods.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-22 10:16:49.000000 phstatsmethods-0.1.8/PHStatsMethods.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 10:16:49.000000 phstatsmethods-0.1.8/PHStatsMethods.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-22 10:16:49.000000 phstatsmethods-0.1.8/PHStatsMethods.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-22 10:16:49.000000 phstatsmethods-0.1.8/PHStatsMethods.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-22 10:16:49.741615 phstatsmethods-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-22 10:16:46.000000 phstatsmethods-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 10:16:49.741615 phstatsmethods-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-22 10:16:46.000000 phstatsmethods-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:24:50.582054 phstatsmethods-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35170 2024-05-22 10:24:47.000000 phstatsmethods-0.1.9/LICENSE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:24:50.578054 phstatsmethods-0.1.9/PHStatsMethods/
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-22 10:24:47.000000 phstatsmethods-0.1.9/PHStatsMethods/DSR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-05-22 10:24:47.000000 phstatsmethods-0.1.9/PHStatsMethods/ISRate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-05-22 10:24:47.000000 phstatsmethods-0.1.9/PHStatsMethods/ISRatio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-22 10:24:47.000000 phstatsmethods-0.1.9/PHStatsMethods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-05-22 10:24:47.000000 phstatsmethods-0.1.9/PHStatsMethods/confidence_intervals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16953 2024-05-22 10:24:47.000000 phstatsmethods-0.1.9/PHStatsMethods/funnels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-22 10:24:47.000000 phstatsmethods-0.1.9/PHStatsMethods/means.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-22 10:24:47.000000 phstatsmethods-0.1.9/PHStatsMethods/proportions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-22 10:24:47.000000 phstatsmethods-0.1.9/PHStatsMethods/quantiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-22 10:24:47.000000 phstatsmethods-0.1.9/PHStatsMethods/rates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-22 10:24:47.000000 phstatsmethods-0.1.9/PHStatsMethods/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-05-22 10:24:47.000000 phstatsmethods-0.1.9/PHStatsMethods/utils_funnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7413 2024-05-22 10:24:47.000000 phstatsmethods-0.1.9/PHStatsMethods/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:24:50.578054 phstatsmethods-0.1.9/PHStatsMethods.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-22 10:24:50.000000 phstatsmethods-0.1.9/PHStatsMethods.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-22 10:24:50.000000 phstatsmethods-0.1.9/PHStatsMethods.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 10:24:50.000000 phstatsmethods-0.1.9/PHStatsMethods.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-22 10:24:50.000000 phstatsmethods-0.1.9/PHStatsMethods.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-22 10:24:50.000000 phstatsmethods-0.1.9/PHStatsMethods.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-22 10:24:50.582054 phstatsmethods-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-22 10:24:47.000000 phstatsmethods-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 10:24:50.582054 phstatsmethods-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-22 10:24:47.000000 phstatsmethods-0.1.9/setup.py
```

### Comparing `phstatsmethods-0.1.8/LICENSE.md` & `phstatsmethods-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.8/PHStatsMethods/DSR.py` & `phstatsmethods-0.1.9/PHStatsMethods/DSR.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.8/PHStatsMethods/ISRate.py` & `phstatsmethods-0.1.9/PHStatsMethods/ISRate.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.8/PHStatsMethods/ISRatio.py` & `phstatsmethods-0.1.9/PHStatsMethods/ISRatio.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.8/PHStatsMethods/__init__.py` & `phstatsmethods-0.1.9/PHStatsMethods/__init__.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-__all__ = ["wilson_lower", "wilson_upper", "wilson",
-           "exact_upper", "exact_lower", "exact",
-           "byars_lower", "byars_upper", "byars", 
-           "dobson_lower", "dobson_upper", "student_t_dist", 
-           "calculate_funnel_limits", "assign_funnel_significance", "calculate_funnel_points"
-           "ph_dsr", "ph_ISRate", "ph_ISRatio", "ph_mean", "ph_proportion",
-           "ph_quantile", "ph_rate", "euro_standard_pop"]
-
-from .confidence_intervals import *
-from .DSR import ph_dsr
-from .funnels import calculate_funnel_limits, assign_funnel_significance, calculate_funnel_points
-from .ISRate import ph_ISRate
-from .ISRatio import ph_ISRatio
-from .means import ph_mean
-from .proportions import ph_proportion
-from .quantiles import ph_quantile
-from .rates import ph_rate
-from .utils import euro_standard_pop
-
 """
 This is a Python package to support analysts in the execution of statistical
 methods approved for use in the production of Public Health indicators such as
 those presented via `Fingertips <https://fingertips.phe.org.uk/>`__. It
 provides functions for the generation of Proportions, Rates, DSRs, ISRs,
 Funnel plots and Means including confidence intervals for these statistics,
 and a function for assigning data to quantiles.
@@ -33,8 +14,27 @@
 
     help(*phm.function*)
 
 Licence:
     This project is released under the `GPL-3 <https://opensource.org/licenses/GPL-3.0>`__
     licence.
 
-"""
+"""
+
+from .confidence_intervals import *
+from .DSR import ph_dsr
+from .funnels import calculate_funnel_limits, assign_funnel_significance, calculate_funnel_points
+from .ISRate import ph_ISRate
+from .ISRatio import ph_ISRatio
+from .means import ph_mean
+from .proportions import ph_proportion
+from .quantiles import ph_quantile
+from .rates import ph_rate
+from .utils import euro_standard_pop
+
+__all__ = ["wilson_lower", "wilson_upper", "wilson",
+           "exact_upper", "exact_lower", "exact",
+           "byars_lower", "byars_upper", "byars", 
+           "dobson_lower", "dobson_upper", "student_t_dist", 
+           "calculate_funnel_limits", "assign_funnel_significance", "calculate_funnel_points"
+           "ph_dsr", "ph_ISRate", "ph_ISRatio", "ph_mean", "ph_proportion",
+           "ph_quantile", "ph_rate", "euro_standard_pop"]
```

### Comparing `phstatsmethods-0.1.8/PHStatsMethods/confidence_intervals.py` & `phstatsmethods-0.1.9/PHStatsMethods/confidence_intervals.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.8/PHStatsMethods/funnels.py` & `phstatsmethods-0.1.9/PHStatsMethods/funnels.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.8/PHStatsMethods/means.py` & `phstatsmethods-0.1.9/PHStatsMethods/means.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.8/PHStatsMethods/proportions.py` & `phstatsmethods-0.1.9/PHStatsMethods/proportions.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.8/PHStatsMethods/quantiles.py` & `phstatsmethods-0.1.9/PHStatsMethods/quantiles.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.8/PHStatsMethods/rates.py` & `phstatsmethods-0.1.9/PHStatsMethods/rates.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.8/PHStatsMethods/utils.py` & `phstatsmethods-0.1.9/PHStatsMethods/utils.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.8/PHStatsMethods/utils_funnel.py` & `phstatsmethods-0.1.9/PHStatsMethods/utils_funnel.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.8/PHStatsMethods/validation.py` & `phstatsmethods-0.1.9/PHStatsMethods/validation.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.8/PHStatsMethods.egg-info/PKG-INFO` & `phstatsmethods-0.1.9/PHStatsMethods.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PHStatsMethods
-Version: 0.1.8
+Version: 0.1.9
 Summary: This is a python package to calculate statistics in public health, including indicators for Fingertips.
 Home-page: https://github.com/DataS-DHSC/PHStatsMethods
 Author: Department of Health and Social Care
 Author-email: annabel.westermann@dhsc.gov.uk, hadley.nanayakkara@dhsc.gov.uk, cameron.stewart@dhsc.gov.uk, jack.burden@dhsc.gov.uk, thilaksan.vikneswaran@dhsc.gov.uk, paul.fryers@dhsc.gov.uk, karandeep.kaur@dhsc.gov.uk, phds@phe.gov.uk
 License: GPL-3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `phstatsmethods-0.1.8/PHStatsMethods.egg-info/SOURCES.txt` & `phstatsmethods-0.1.9/PHStatsMethods.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.8/PKG-INFO` & `phstatsmethods-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PHStatsMethods
-Version: 0.1.8
+Version: 0.1.9
 Summary: This is a python package to calculate statistics in public health, including indicators for Fingertips.
 Home-page: https://github.com/DataS-DHSC/PHStatsMethods
 Author: Department of Health and Social Care
 Author-email: annabel.westermann@dhsc.gov.uk, hadley.nanayakkara@dhsc.gov.uk, cameron.stewart@dhsc.gov.uk, jack.burden@dhsc.gov.uk, thilaksan.vikneswaran@dhsc.gov.uk, paul.fryers@dhsc.gov.uk, karandeep.kaur@dhsc.gov.uk, phds@phe.gov.uk
 License: GPL-3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `phstatsmethods-0.1.8/README.md` & `phstatsmethods-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.8/setup.py` & `phstatsmethods-0.1.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='PHStatsMethods',
-    version='0.1.8',
+    version='0.1.9',
     packages=['PHStatsMethods'],
     url='https://github.com/DataS-DHSC/PHStatsMethods',
     license='GPL-3.0',
     author='Department of Health and Social Care',
     author_email='annabel.westermann@dhsc.gov.uk, hadley.nanayakkara@dhsc.gov.uk, cameron.stewart@dhsc.gov.uk, jack.burden@dhsc.gov.uk, thilaksan.vikneswaran@dhsc.gov.uk, paul.fryers@dhsc.gov.uk, karandeep.kaur@dhsc.gov.uk, phds@phe.gov.uk',
     description='This is a python package to calculate statistics in public health, including indicators for Fingertips.',
     long_description=long_description,
```

