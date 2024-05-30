# Comparing `tmp/mcdm_scheduler-1.5.4.tar.gz` & `tmp/mcdm_scheduler-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcdm_scheduler-1.5.4.tar", last modified: Thu May 30 16:30:43 2024, max compression
+gzip compressed data, was "mcdm_scheduler-1.5.5.tar", last modified: Thu May 30 17:15:49 2024, max compression
```

## Comparing `mcdm_scheduler-1.5.4.tar` & `mcdm_scheduler-1.5.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 16:30:43.242991 mcdm_scheduler-1.5.4/
--rw-rw-rw-   0        0        0      668 2024-05-22 01:01:37.000000 mcdm_scheduler-1.5.4/LICENSE
--rw-rw-rw-   0        0        0     1877 2024-05-30 16:30:43.242991 mcdm_scheduler-1.5.4/PKG-INFO
--rw-rw-rw-   0        0        0     1526 2024-05-24 01:19:05.000000 mcdm_scheduler-1.5.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 16:30:43.195342 mcdm_scheduler-1.5.4/mcdm_scheduler/
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 mcdm_scheduler-1.5.4/mcdm_scheduler/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 16:30:43.227311 mcdm_scheduler-1.5.4/mcdm_scheduler/algorithm/
--rw-rw-rw-   0        0        0       19 2024-05-23 23:46:34.000000 mcdm_scheduler-1.5.4/mcdm_scheduler/algorithm/__init__.py
--rw-rw-rw-   0        0        0    20004 2024-05-30 14:01:50.000000 mcdm_scheduler-1.5.4/mcdm_scheduler/algorithm/src.py
-drwxrwxrwx   0        0        0        0 2024-05-30 16:30:43.242991 mcdm_scheduler-1.5.4/mcdm_scheduler/util/
--rw-rw-rw-   0        0        0       87 2024-05-23 23:47:52.000000 mcdm_scheduler-1.5.4/mcdm_scheduler/util/__init__.py
--rw-rw-rw-   0        0        0     2924 2024-05-24 00:42:10.000000 mcdm_scheduler-1.5.4/mcdm_scheduler/util/fuzzy_ppf_ahp.py
--rw-rw-rw-   0        0        0     7579 2024-05-30 12:14:22.000000 mcdm_scheduler-1.5.4/mcdm_scheduler/util/ga.py
--rw-rw-rw-   0        0        0     2460 2024-05-21 23:05:20.000000 mcdm_scheduler-1.5.4/mcdm_scheduler/util/ht2fs.py
-drwxrwxrwx   0        0        0        0 2024-05-30 16:30:43.224135 mcdm_scheduler-1.5.4/mcdm_scheduler.egg-info/
--rw-rw-rw-   0        0        0     1877 2024-05-30 16:30:42.000000 mcdm_scheduler-1.5.4/mcdm_scheduler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      435 2024-05-30 16:30:43.000000 mcdm_scheduler-1.5.4/mcdm_scheduler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 16:30:42.000000 mcdm_scheduler-1.5.4/mcdm_scheduler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-30 16:30:42.000000 mcdm_scheduler-1.5.4/mcdm_scheduler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-30 16:30:42.000000 mcdm_scheduler-1.5.4/mcdm_scheduler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 16:30:43.242991 mcdm_scheduler-1.5.4/setup.cfg
--rw-rw-rw-   0        0        0      644 2024-05-30 16:20:37.000000 mcdm_scheduler-1.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 17:15:49.079937 mcdm_scheduler-1.5.5/
+-rw-rw-rw-   0        0        0      668 2024-05-22 01:01:37.000000 mcdm_scheduler-1.5.5/LICENSE
+-rw-rw-rw-   0        0        0     1877 2024-05-30 17:15:49.079937 mcdm_scheduler-1.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1526 2024-05-24 01:19:05.000000 mcdm_scheduler-1.5.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 17:15:49.064315 mcdm_scheduler-1.5.5/mcdm_scheduler/
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 mcdm_scheduler-1.5.5/mcdm_scheduler/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 17:15:49.064315 mcdm_scheduler-1.5.5/mcdm_scheduler/algorithm/
+-rw-rw-rw-   0        0        0       19 2024-05-23 23:46:34.000000 mcdm_scheduler-1.5.5/mcdm_scheduler/algorithm/__init__.py
+-rw-rw-rw-   0        0        0    19800 2024-05-30 17:07:17.000000 mcdm_scheduler-1.5.5/mcdm_scheduler/algorithm/src.py
+drwxrwxrwx   0        0        0        0 2024-05-30 17:15:49.079937 mcdm_scheduler-1.5.5/mcdm_scheduler/util/
+-rw-rw-rw-   0        0        0       87 2024-05-23 23:47:52.000000 mcdm_scheduler-1.5.5/mcdm_scheduler/util/__init__.py
+-rw-rw-rw-   0        0        0     2924 2024-05-24 00:42:10.000000 mcdm_scheduler-1.5.5/mcdm_scheduler/util/fuzzy_ppf_ahp.py
+-rw-rw-rw-   0        0        0     7579 2024-05-30 12:14:22.000000 mcdm_scheduler-1.5.5/mcdm_scheduler/util/ga.py
+-rw-rw-rw-   0        0        0     2418 2024-05-30 17:06:23.000000 mcdm_scheduler-1.5.5/mcdm_scheduler/util/ht2fs.py
+drwxrwxrwx   0        0        0        0 2024-05-30 17:15:49.064315 mcdm_scheduler-1.5.5/mcdm_scheduler.egg-info/
+-rw-rw-rw-   0        0        0     1877 2024-05-30 17:15:48.000000 mcdm_scheduler-1.5.5/mcdm_scheduler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      435 2024-05-30 17:15:48.000000 mcdm_scheduler-1.5.5/mcdm_scheduler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 17:15:48.000000 mcdm_scheduler-1.5.5/mcdm_scheduler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-30 17:15:48.000000 mcdm_scheduler-1.5.5/mcdm_scheduler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-30 17:15:48.000000 mcdm_scheduler-1.5.5/mcdm_scheduler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 17:15:49.079937 mcdm_scheduler-1.5.5/setup.cfg
+-rw-rw-rw-   0        0        0      644 2024-05-30 17:11:39.000000 mcdm_scheduler-1.5.5/setup.py
```

### Comparing `mcdm_scheduler-1.5.4/LICENSE` & `mcdm_scheduler-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mcdm_scheduler-1.5.4/PKG-INFO` & `mcdm_scheduler-1.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcdm_scheduler
-Version: 1.5.4
+Version: 1.5.5
 Summary: A Library Incorporating a MCDM tools for Scheduling Problems
 Home-page: https://github.com/Valdecy/mcdm_scheduler
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mcdm_scheduler-1.5.4/README.md` & `mcdm_scheduler-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `mcdm_scheduler-1.5.4/mcdm_scheduler/algorithm/src.py` & `mcdm_scheduler-1.5.5/mcdm_scheduler/algorithm/src.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,28 +22,27 @@
 from mcdm_scheduler.util.ga            import genetic_algorithm
 from mcdm_scheduler.util.ht2fs         import ht2fs_weight_calculation
 
 ############################################################################
 
 # MCDM Scheduler Class
 class load_mcdm_scheduler():
-    def __init__(self, sequences = [], due_dates = [], setup_time_matrix = [], setup_waste_matrix = [], comparison_matrix = [], crisp_inputs = [], uncertainty_ranges = [], criteria_importance = [], population_size = 5, elite = 1, mutation_rate = 0.1, generations = 100, custom_job_weights = [], custom_objective_weights = [], custom_sequence = [], z_permutations = 100, brute_force = False, parallel = False): 
+    def __init__(self, sequences = [], due_dates = [], setup_time_matrix = [], setup_waste_matrix = [], comparison_matrix = [], crisp_inputs = [], uncertainty_ranges = [], population_size = 5, elite = 1, mutation_rate = 0.1, generations = 100, custom_job_weights = [], custom_objective_weights = [], custom_sequence = [], z_permutations = 100, brute_force = False, parallel = False): 
       self.z_std                          = []
       self.z_permutations                 = z_permutations
       self.job_weights                    = custom_job_weights         # Job Weights: Opitional
       self.objectives_weights             = custom_objective_weights   # Objectives Weights (Makespan, Max WeightedTardiness, Total Waste, Total Setup Time): Opitional
       self.custom_sequence                = custom_sequence
       self.sequences                      = sequences                  # Job Shop Scheduling Input: Mandatory
       self.due_dates                      = due_dates                  # Job Shop Scheduling Input: Only Relevant if Due Date    is a measure
       self.setup_time_matrix              = setup_time_matrix          # Job Shop Scheduling Input: Only Relevant if Setup Time  is a measure
       self.setup_waste_matrix             = setup_waste_matrix         # Job Shop Scheduling Input: Only Relevant if Setup Waste is a measure
       self.comparison_matrix              = comparison_matrix          # PPF-AHP             Input: Only Relevant if custom_objectives_weights = []
       self.crisp_inputs                   = crisp_inputs               # HT2FS               Input: Only Relevant if custom_job_weights        = []
       self.uncertainty_ranges             = uncertainty_ranges         # HT2FS               Input: Only Relevant if custom_job_weights        = []
-      self.criteria_importance            = criteria_importance        # HT2FS               Input: Only Relevant if custom_job_weights        = []
       self.population_size                = population_size            # GA
       self.elite                          = int(elite)                 # GA
       self.mutation_rate                  = mutation_rate              # GA
       self.generations                    = generations                # GA
       self.brute_force                    = brute_force
       self.parallel                       = parallel
       self.machine_sequences, self.matrix = self.sequence_inputs()
@@ -336,15 +335,15 @@
                 else:
                     g_mean = [g_mean[j]*weights[i][j] for j in range(0, len(weights[i]))]
                 i = i + 1
             g_mean = [g_mean[j]**(1/len(weights)) for j in range(0, len(g_mean))]   
             self.objectives_weights = g_mean
         if (len(self.job_weights) == 0):
             for k in range(0, len(self.crisp_inputs)):
-                job_weights = ht2fs_weight_calculation(self.crisp_inputs[k], self.uncertainty_ranges[k], self.criteria_importance[k])
+                job_weights = ht2fs_weight_calculation(self.crisp_inputs[k], self.uncertainty_ranges[k])
                 if (len(self.job_weights) == 0):
                     self.job_weights = job_weights
                 else:
                     self.job_weights = [self.job_weights[j] + job_weights[j] for j in range(0, len(self.job_weights))]
             self.job_weights = [x / sum(self.job_weights) for x in self.job_weights]
         if (self.objectives_weights.count(0) == 3):
           self.z_mean, self.z_std = [0, 0, 0, 0], [1, 1, 1, 1]
```

### Comparing `mcdm_scheduler-1.5.4/mcdm_scheduler/util/fuzzy_ppf_ahp.py` & `mcdm_scheduler-1.5.5/mcdm_scheduler/util/fuzzy_ppf_ahp.py`

 * *Files identical despite different names*

### Comparing `mcdm_scheduler-1.5.4/mcdm_scheduler/util/ga.py` & `mcdm_scheduler-1.5.5/mcdm_scheduler/util/ga.py`

 * *Files identical despite different names*

### Comparing `mcdm_scheduler-1.5.4/mcdm_scheduler/util/ht2fs.py` & `mcdm_scheduler-1.5.5/mcdm_scheduler/util/ht2fs.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 # Required Libraries
 import numpy as np
 
 ###############################################################################
 
 # Function: HT2FS
-def ht2fs_weight_calculation(crisp_inputs, uncertainty_ranges, criteria_importance):
+def ht2fs_weight_calculation(crisp_inputs, uncertainty_ranges):
     
     ################################################
     def fuzzify_input(crisp_value, uncertainty_range):
         a = crisp_value - 2 * uncertainty_range
         b = crisp_value - uncertainty_range
         c = crisp_value
         d = crisp_value
         e = crisp_value + uncertainty_range
         f = crisp_value + 2 * uncertainty_range
         return (a, b, c, d, e, f)
 
-    def construct_fuzzy_decision_matrix(fuzzy_inputs, criteria_importance):
-        n            = len(criteria_importance)
+    def construct_fuzzy_decision_matrix(fuzzy_inputs, crisp_inputs):
+        n            = len(crisp_inputs)
         fuzzy_matrix = np.zeros((n, n), dtype = object)
         for i in range(n):
             for j in range(n):
                 if (i == j):
                     fuzzy_matrix[i][j] = fuzzify_input(1.0, 0.0)
                 else:
                     fuzzy_matrix[i][j] = fuzzy_inputs[j]
@@ -46,13 +46,13 @@
     def defuzzify_value(fuzzy_value):
         a, b, c, d, e, f = fuzzy_value
         numerator        = (a + 2*b + 3*c + 3*d + 2*e + f) / 12
         return numerator
     ################################################
     
     fuzzy_inputs          = [fuzzify_input(crisp, uncertainty) for crisp, uncertainty in zip(crisp_inputs, uncertainty_ranges)]
-    fuzzy_decision_matrix = construct_fuzzy_decision_matrix(fuzzy_inputs, criteria_importance)
+    fuzzy_decision_matrix = construct_fuzzy_decision_matrix(fuzzy_inputs, crisp_inputs)
     composite_weights     = apply_fuzzy_arithmetic(fuzzy_decision_matrix)
     crisp_weights         = [defuzzify_value(fuzzy) for fuzzy in composite_weights]
     return crisp_weights
 
 ###############################################################################
```

### Comparing `mcdm_scheduler-1.5.4/mcdm_scheduler.egg-info/PKG-INFO` & `mcdm_scheduler-1.5.5/mcdm_scheduler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcdm-scheduler
-Version: 1.5.4
+Version: 1.5.5
 Summary: A Library Incorporating a MCDM tools for Scheduling Problems
 Home-page: https://github.com/Valdecy/mcdm_scheduler
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mcdm_scheduler-1.5.4/setup.py` & `mcdm_scheduler-1.5.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='mcdm_scheduler',
-    version='1.5.4',
+    version='1.5.5',
     license='GNU',
     author='Valdecy Pereira',
     author_email='valdecy.pereira@gmail.com',
     url='https://github.com/Valdecy/mcdm_scheduler',
     packages=find_packages(),
     install_requires=[
         'matplotlib',
```

