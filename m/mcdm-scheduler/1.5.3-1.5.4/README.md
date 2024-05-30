# Comparing `tmp/mcdm_scheduler-1.5.3.tar.gz` & `tmp/mcdm_scheduler-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mcdm_scheduler-1.5.3.tar", last modified: Sat May 25 20:38:44 2024, max compression
+gzip compressed data, was "mcdm_scheduler-1.5.4.tar", last modified: Thu May 30 16:30:43 2024, max compression
```

## Comparing `mcdm_scheduler-1.5.3.tar` & `mcdm_scheduler-1.5.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 20:38:44.000000 mcdm_scheduler-1.5.3/
--rw-rw-rw-   0        0        0      668 2024-05-22 01:01:37.000000 mcdm_scheduler-1.5.3/LICENSE
--rw-rw-rw-   0        0        0     1877 2024-05-25 20:38:44.000000 mcdm_scheduler-1.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     1526 2024-05-24 01:19:05.000000 mcdm_scheduler-1.5.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-25 20:38:44.000000 mcdm_scheduler-1.5.3/mcdm_scheduler/
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 mcdm_scheduler-1.5.3/mcdm_scheduler/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 20:38:44.000000 mcdm_scheduler-1.5.3/mcdm_scheduler/algorithm/
--rw-rw-rw-   0        0        0       19 2024-05-23 23:46:34.000000 mcdm_scheduler-1.5.3/mcdm_scheduler/algorithm/__init__.py
--rw-rw-rw-   0        0        0    16760 2024-05-25 20:36:23.000000 mcdm_scheduler-1.5.3/mcdm_scheduler/algorithm/src.py
-drwxrwxrwx   0        0        0        0 2024-05-25 20:38:44.000000 mcdm_scheduler-1.5.3/mcdm_scheduler/util/
--rw-rw-rw-   0        0        0       87 2024-05-23 23:47:52.000000 mcdm_scheduler-1.5.3/mcdm_scheduler/util/__init__.py
--rw-rw-rw-   0        0        0     2924 2024-05-24 00:42:10.000000 mcdm_scheduler-1.5.3/mcdm_scheduler/util/fuzzy_ppf_ahp.py
--rw-rw-rw-   0        0        0     7629 2024-05-24 00:31:01.000000 mcdm_scheduler-1.5.3/mcdm_scheduler/util/ga.py
--rw-rw-rw-   0        0        0     2460 2024-05-21 23:05:20.000000 mcdm_scheduler-1.5.3/mcdm_scheduler/util/ht2fs.py
-drwxrwxrwx   0        0        0        0 2024-05-25 20:38:44.000000 mcdm_scheduler-1.5.3/mcdm_scheduler.egg-info/
--rw-rw-rw-   0        0        0     1877 2024-05-25 20:38:42.000000 mcdm_scheduler-1.5.3/mcdm_scheduler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      435 2024-05-25 20:38:43.000000 mcdm_scheduler-1.5.3/mcdm_scheduler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 20:38:42.000000 mcdm_scheduler-1.5.3/mcdm_scheduler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-25 20:38:42.000000 mcdm_scheduler-1.5.3/mcdm_scheduler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-25 20:38:42.000000 mcdm_scheduler-1.5.3/mcdm_scheduler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-25 20:38:44.000000 mcdm_scheduler-1.5.3/setup.cfg
--rw-rw-rw-   0        0        0      644 2024-05-25 20:37:32.000000 mcdm_scheduler-1.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 16:30:43.242991 mcdm_scheduler-1.5.4/
+-rw-rw-rw-   0        0        0      668 2024-05-22 01:01:37.000000 mcdm_scheduler-1.5.4/LICENSE
+-rw-rw-rw-   0        0        0     1877 2024-05-30 16:30:43.242991 mcdm_scheduler-1.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1526 2024-05-24 01:19:05.000000 mcdm_scheduler-1.5.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 16:30:43.195342 mcdm_scheduler-1.5.4/mcdm_scheduler/
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 mcdm_scheduler-1.5.4/mcdm_scheduler/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 16:30:43.227311 mcdm_scheduler-1.5.4/mcdm_scheduler/algorithm/
+-rw-rw-rw-   0        0        0       19 2024-05-23 23:46:34.000000 mcdm_scheduler-1.5.4/mcdm_scheduler/algorithm/__init__.py
+-rw-rw-rw-   0        0        0    20004 2024-05-30 14:01:50.000000 mcdm_scheduler-1.5.4/mcdm_scheduler/algorithm/src.py
+drwxrwxrwx   0        0        0        0 2024-05-30 16:30:43.242991 mcdm_scheduler-1.5.4/mcdm_scheduler/util/
+-rw-rw-rw-   0        0        0       87 2024-05-23 23:47:52.000000 mcdm_scheduler-1.5.4/mcdm_scheduler/util/__init__.py
+-rw-rw-rw-   0        0        0     2924 2024-05-24 00:42:10.000000 mcdm_scheduler-1.5.4/mcdm_scheduler/util/fuzzy_ppf_ahp.py
+-rw-rw-rw-   0        0        0     7579 2024-05-30 12:14:22.000000 mcdm_scheduler-1.5.4/mcdm_scheduler/util/ga.py
+-rw-rw-rw-   0        0        0     2460 2024-05-21 23:05:20.000000 mcdm_scheduler-1.5.4/mcdm_scheduler/util/ht2fs.py
+drwxrwxrwx   0        0        0        0 2024-05-30 16:30:43.224135 mcdm_scheduler-1.5.4/mcdm_scheduler.egg-info/
+-rw-rw-rw-   0        0        0     1877 2024-05-30 16:30:42.000000 mcdm_scheduler-1.5.4/mcdm_scheduler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      435 2024-05-30 16:30:43.000000 mcdm_scheduler-1.5.4/mcdm_scheduler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 16:30:42.000000 mcdm_scheduler-1.5.4/mcdm_scheduler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-30 16:30:42.000000 mcdm_scheduler-1.5.4/mcdm_scheduler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-30 16:30:42.000000 mcdm_scheduler-1.5.4/mcdm_scheduler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 16:30:43.242991 mcdm_scheduler-1.5.4/setup.cfg
+-rw-rw-rw-   0        0        0      644 2024-05-30 16:20:37.000000 mcdm_scheduler-1.5.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mcdm_scheduler-1.5.3/LICENSE` & `mcdm_scheduler-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mcdm_scheduler-1.5.3/PKG-INFO` & `mcdm_scheduler-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcdm_scheduler
-Version: 1.5.3
+Version: 1.5.4
 Summary: A Library Incorporating a MCDM tools for Scheduling Problems
 Home-page: https://github.com/Valdecy/mcdm_scheduler
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mcdm_scheduler-1.5.3/README.md` & `mcdm_scheduler-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `mcdm_scheduler-1.5.3/mcdm_scheduler/algorithm/src.py` & `mcdm_scheduler-1.5.4/mcdm_scheduler/algorithm/src.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,27 +12,30 @@
 
 # Required Libraries
 import itertools
 import matplotlib.pyplot as plt
 import matplotlib.patches as mpatches
 plt.style.use('ggplot')
 import numpy as np
+import random
 
 from mcdm_scheduler.util.fuzzy_ppf_ahp import ppf_ahp_method
 from mcdm_scheduler.util.ga            import genetic_algorithm
 from mcdm_scheduler.util.ht2fs         import ht2fs_weight_calculation
 
 ############################################################################
 
 # MCDM Scheduler Class
 class load_mcdm_scheduler():
-    def __init__(self, sequences = [], due_dates = [], setup_time_matrix = [], setup_waste_matrix = [], comparison_matrix = [], crisp_inputs = [], uncertainty_ranges = [], criteria_importance = [], population_size = 5, elite = 1, mutation_rate = 0.1, generations = 100, custom_job_weights = [], custom_objective_weights = [], custom_job_sequence = [], brute_force = False, parallel = False): 
+    def __init__(self, sequences = [], due_dates = [], setup_time_matrix = [], setup_waste_matrix = [], comparison_matrix = [], crisp_inputs = [], uncertainty_ranges = [], criteria_importance = [], population_size = 5, elite = 1, mutation_rate = 0.1, generations = 100, custom_job_weights = [], custom_objective_weights = [], custom_sequence = [], z_permutations = 100, brute_force = False, parallel = False): 
+      self.z_std                          = []
+      self.z_permutations                 = z_permutations
       self.job_weights                    = custom_job_weights         # Job Weights: Opitional
       self.objectives_weights             = custom_objective_weights   # Objectives Weights (Makespan, Max WeightedTardiness, Total Waste, Total Setup Time): Opitional
-      self.custom_job_sequence            = custom_job_sequence
+      self.custom_sequence                = custom_sequence
       self.sequences                      = sequences                  # Job Shop Scheduling Input: Mandatory
       self.due_dates                      = due_dates                  # Job Shop Scheduling Input: Only Relevant if Due Date    is a measure
       self.setup_time_matrix              = setup_time_matrix          # Job Shop Scheduling Input: Only Relevant if Setup Time  is a measure
       self.setup_waste_matrix             = setup_waste_matrix         # Job Shop Scheduling Input: Only Relevant if Setup Waste is a measure
       self.comparison_matrix              = comparison_matrix          # PPF-AHP             Input: Only Relevant if custom_objectives_weights = []
       self.crisp_inputs                   = crisp_inputs               # HT2FS               Input: Only Relevant if custom_job_weights        = []
       self.uncertainty_ranges             = uncertainty_ranges         # HT2FS               Input: Only Relevant if custom_job_weights        = []
@@ -44,61 +47,112 @@
       self.brute_force                    = brute_force
       self.parallel                       = parallel
       self.machine_sequences, self.matrix = self.sequence_inputs()
       self.num_jobs                       = len(self.sequences)
       self.num_machines                   = self.matrix.shape[1]
     
     ###############################################################################
+
+    # Schedule
+    def schedule_jobs(self, permutation):
+        total_length      = np.sum(self.matrix)
+        schedule          = [['' for _ in range(0, total_length)] for _ in range(0, self.num_machines)]
+        machine_end_times = [0] * self.num_machines
+        job_end_times     = [0] * self.num_jobs
+        if (self.parallel == False):
+            for job_id in permutation:
+                operations = self.machine_sequences[job_id]
+                for op_index, machine in enumerate(operations):
+                    time_required = self.matrix[job_id, machine]
+                    start_time    = job_end_times[job_id]
+                    while any(schedule[machine][start_time:start_time + time_required]):
+                        start_time = start_time + 1
+                    end_time = start_time + time_required
+                    for t in range(start_time, end_time):
+                        schedule[machine][t] = f"j{job_id}"
+                    job_end_times[job_id]      = end_time
+                    machine_end_times[machine] = end_time
+        else:        
+            for job_id in permutation:
+                earliest_start_time = float('inf')
+                best_machine        = None
+                for machine, time_required in self.sequences[job_id]:
+                    start_time = machine_end_times[machine]
+                    while any(schedule[machine][start_time:start_time + time_required]):
+                        start_time = start_time + 1
+                    if (start_time < earliest_start_time):
+                        earliest_start_time = start_time
+                        best_machine        = machine
+                time_required = self.matrix[job_id, best_machine]
+                end_time      = earliest_start_time + time_required
+                for t in range(earliest_start_time, end_time):
+                    schedule[best_machine][t]   = f"j{job_id}"
+                machine_end_times[best_machine] = end_time
+                job_end_times[job_id]           = end_time
+        max_time = max(len(row) for row in schedule)
+        for col in range(max_time - 1, -1, -1):
+            if (all(row[col] == '' for row in schedule)):
+                for row in schedule:
+                    row.pop()
+            else:
+                break
+        return np.array(schedule)
+   
+    ###############################################################################
     
     # Plot
     def create_gantt_chart(self, schedule_matrix, size_x = 12, size_y = 8):
-        total_length   = schedule_matrix.shape[1]
+        non_empty_rows = [i for i in range(schedule_matrix.shape[0]) if not np.all(schedule_matrix[i] == '')]
+        schedule       = schedule_matrix[non_empty_rows, :]
+        num_machines   = schedule.shape[0]
+        total_length   = schedule.shape[1]
         fig, ax        = plt.subplots(figsize = (size_x, size_y))
         job_color_dict = {}
         idle_patches   = []
-        job_colors     = itertools.cycle([
-                                            '#1f77b4', '#ff7f0e', '#2ca02c', '#d62728', '#9467bd', '#8c564b', '#e377c2', 
-                                            '#7f7f7f', '#bcbd22', '#17becf', '#bf77f6', '#ff9408', '#d1ffbd', '#c85a53', 
-                                            '#3a18b1', '#ff796c', '#04d8b2', '#ffb07c', '#aaa662', '#0485d1', '#fffe7a', 
-                                            '#b0dd16', '#6f7be3', '#12e193', '#82cafc', '#ac9362', '#f8481c', '#c292a1', 
-                                            '#c0fa8b', '#ca7b80', '#f4d054', '#fbdd7e', '#ffff7e', '#cd7584', '#f9bc08', 
-                                            '#c7c10c'
-                                          ])
-        for machine in range(0, self.num_machines):
+        job_colors     = [
+                            '#1f77b4', '#ff7f0e', '#2ca02c', '#d62728', '#9467bd', '#8c564b', '#e377c2', 
+                            '#7f7f7f', '#bcbd22', '#17becf', '#bf77f6', '#ff9408', '#d1ffbd', '#c85a53', 
+                            '#3a18b1', '#ff796c', '#04d8b2', '#ffb07c', '#aaa662', '#0485d1', '#fffe7a', 
+                            '#b0dd16', '#6f7be3', '#12e193', '#82cafc', '#ac9362', '#f8481c', '#c292a1', 
+                            '#c0fa8b', '#ca7b80', '#f4d054', '#fbdd7e', '#ffff7e', '#cd7584', '#f9bc08', 
+                            '#c7c10c'
+                         ]
+        for machine in range(0, num_machines):
             for time in range(0, total_length):
-                job = schedule_matrix[machine][time]
+                job = schedule[machine][time]
                 if (job):
                     if (job not in job_color_dict):
-                        job_color_dict[job] = next(job_colors)
+                        job_index           = int(job[1:])  
+                        job_color_dict[job] = job_colors[job_index % len(job_colors)]
                     color = job_color_dict[job]
-                    ax.add_patch(mpatches.Rectangle((time, self.num_machines - machine - 1), 1, 1, edgecolor = 'black', facecolor = color))
-                    ax.text(time + 0.5, self.num_machines - machine - 0.5, job, ha = 'center', va = 'center', color = 'black', fontsize = 8, weight = 'bold')
+                    ax.add_patch(mpatches.Rectangle((time, num_machines - machine - 1), 1, 1, edgecolor = 'black', facecolor = color))
+                    ax.text(time + 0.5, num_machines - machine - 0.5, job, ha = 'center', va = 'center', color = 'black', fontsize = 8, weight = 'bold')
                 else:
-                    left_hatch  = mpatches.Rectangle((time, self.num_machines - machine - 1), 1, 1, edgecolor = 'grey', facecolor = 'none', hatch = '//')
-                    right_hatch = mpatches.Rectangle((time, self.num_machines - machine - 1), 1, 1, edgecolor = 'grey', facecolor = 'none', hatch = '\\')
+                    left_hatch = mpatches.Rectangle((time, num_machines - machine - 1), 1, 1, edgecolor = 'black', facecolor = 'none', hatch = '//')
+                    right_hatch = mpatches.Rectangle((time, num_machines - machine - 1), 1, 1, edgecolor = 'black', facecolor = 'none', hatch = '\\')
                     ax.add_patch(left_hatch)
                     ax.add_patch(right_hatch)
                     idle_patches.append((time, machine, left_hatch, right_hatch))
-        for machine in range(0, self.num_machines):
+        for machine in range(0, num_machines):
             for time in range(total_length - 1, -1, -1):
-                if (schedule_matrix[machine][time] == ''):
+                if (schedule[machine][time] == ''):
                     for patch in idle_patches:
-                        if patch[0] == time and patch[1] == machine:
+                        if (patch[0] == time and patch[1] == machine):
                             patch[2].remove()
                             patch[3].remove()
                 else:
                     break
         ax.set_xlim(0, total_length)
-        ax.set_ylim(0, self.num_machines)
-        ax.set_xticks(np.arange(0, total_length + 1, 1))  
-        ax.set_xticklabels(np.arange(0, total_length + 1, 1))  
-        ax.set_yticks(np.arange(0, self.num_machines, 1))
+        ax.set_ylim(0, num_machines)
+        ax.set_xticks(np.arange(0, total_length + 1, 1))
+        ax.set_xticklabels(np.arange(0, total_length + 1, 1))
+        ax.set_yticks(np.arange(0, num_machines, 1))
         ax.set_yticklabels([])
-        for i in range(0, self.num_machines):
-            ax.text(-0.5, self.num_machines - i - 0.5, f'Machine {i}', va = 'center', ha = 'right', fontsize = 10)
+        for i in range(0, num_machines):
+            ax.text(-0.5, num_machines - i - 0.5, f'Machine {i}', va = 'center', ha = 'right', fontsize = 10)
         ax.set_xlabel('Time')
         ax.set_title('Gantt Chart')
         ax.grid(True, linestyle = '--', alpha = 0.7)
         plt.show()
     
     ###############################################################################
     
@@ -126,21 +180,37 @@
             tardiness              = max(0, completion_times[f'j{job}'] - self.due_dates[job])
             weighted_tardiness     = self.job_weights[job] * tardiness
             max_weighted_tardiness = max(max_weighted_tardiness, weighted_tardiness)
         return max_weighted_tardiness
     
     def calculate_total_waste(self, permutation):
         total_waste = 0
-        for i in range(len(permutation) - 1):
+        for i in range(0, len(permutation) - 1):
             total_waste = total_waste + self.setup_waste_matrix[permutation[i]][permutation[i+1]]
         return total_waste
     
+    def calculate_idle_times(self, schedule_matrix):
+        total_idle_time = 0
+        for row in schedule_matrix:
+            row_idle_time  = 0
+            last_job_index = None
+            for i in range(len(row) - 1, -1, -1):
+                if (row[i] != ''):
+                    last_job_index = i
+                    break
+            if (last_job_index is not None):
+                for i in range(0, last_job_index):
+                    if (row[i] == ''):
+                        row_idle_time =  row_idle_time  + 1
+            total_idle_time = total_idle_time + row_idle_time
+        return total_idle_time
+    
     def calculate_total_setup_time(self, permutation):
         total_setup_time = 0
-        for i in range(len(permutation) - 1):
+        for i in range(0, len(permutation) - 1):
             total_setup_time = total_setup_time + self.setup_time_matrix[permutation[i]][permutation[i+1]]
         return total_setup_time
     
     ###############################################################################
     
     # Inputs
     def sequence_inputs(self):
@@ -154,100 +224,107 @@
         for job_id, job in enumerate(self.sequences):
             machine_sequence = [machine for machine, _ in job]
             machine_sequences.append(machine_sequence)
         return machine_sequences, matrix
     
     ###############################################################################
     
-    # Schedule
-    def schedule_jobs(self, permutation):
-        total_length      = np.sum(self.matrix)
-        schedule          = [['' for _ in range(0, total_length)] for _ in range(0, self.num_machines)]
-        machine_end_times = [0] * self.num_machines
-        job_end_times     = [0] * self.num_jobs
-        if (self.parallel == False):
-            for job_id in permutation:
-                operations = self.machine_sequences[job_id]
-                for op_index, machine in enumerate(operations):
-                    time_required = self.matrix[job_id, machine]
-                    start_time    = job_end_times[job_id]
-                    while any(schedule[machine][start_time:start_time + time_required]):
-                        start_time = start_time + 1
-                    end_time = start_time + time_required
-                    for t in range(start_time, end_time):
-                        schedule[machine][t] = f"j{job_id}"
-                    job_end_times[job_id]      = end_time
-                    machine_end_times[machine] = end_time
-        else:        
-            for job_id in permutation:
-                earliest_start_time = float('inf')
-                best_machine = None
-                
-                for machine, time_required in self.sequences[job_id]:
-                    start_time = machine_end_times[machine]
-                    while any(schedule[machine][start_time:start_time + time_required]):
-                        start_time = start_time + 1
-                    if (start_time < earliest_start_time):
-                        earliest_start_time = start_time
-                        best_machine = machine
-                time_required = self.matrix[job_id, best_machine]
-                end_time = earliest_start_time + time_required
-                for t in range(earliest_start_time, end_time):
-                    schedule[best_machine][t] = f"j{job_id}"
-                machine_end_times[best_machine] = end_time
-                job_end_times[job_id] = end_time
-        max_time = max(len(row) for row in schedule)
-        for col in range(max_time - 1, -1, -1):
-            if (all(row[col] == '' for row in schedule)):
-                for row in schedule:
-                    row.pop()
-            else:
-                break
-        return np.array(schedule)
-    
+    # Find Solution
     def brute_force_search(self):
-        job_ids                 = list(range(len(self.sequences)))
+        job_ids                 = list(range(0, len(self.sequences)))
         best_sequence           = None
         minimal_objective_value = float('inf')
         for permutation in itertools.permutations(job_ids):
+            objective_value = self.target_function(permutation)
+            if (objective_value < minimal_objective_value):
+                minimal_objective_value = objective_value
+                best_sequence           = permutation
+        self.best_sequence = best_sequence
+        print('Objective Function:', minimal_objective_value)
+        return best_sequence, minimal_objective_value
+
+    def obj_z_search(self):
+        
+        ################################################
+        def unique_permutations(job_ids, num_permutations):
+            seen = set()
+            while (len(seen) < num_permutations):
+                perm = tuple(random.sample(job_ids, len(job_ids)))
+                seen.add(perm)
+            return list(seen)
+        ################################################
+        
+        job_ids              = list(range(0, len(self.sequences)))
+        num_permutations     = min(self.z_permutations, np.math.factorial(len(job_ids)))
+        sampled_permutations = unique_permutations(job_ids, num_permutations)
+        obj_1_lst            = []
+        obj_2_lst            = []
+        obj_3_lst            = []
+        obj_4_lst            = []
+        z_mean               = []
+        z_std                = []
+        for permutation in sampled_permutations:
             schedule_matrix = self.schedule_jobs(permutation)
-            objective_value = 0.0 / 1.0
             if (self.objectives_weights[0] != 0):
-                makespan               = self.calculate_makespan(schedule_matrix)
-                objective_value        = objective_value + self.objectives_weights[0] * makespan
+                makespan = self.calculate_makespan(schedule_matrix)
+                obj_1_lst.append(makespan)
             if (self.objectives_weights[1] != 0):
                 max_weighted_tardiness = self.calculate_max_weighted_tardiness(schedule_matrix)
-                objective_value        = objective_value + self.objectives_weights[1] * max_weighted_tardiness
+                obj_2_lst.append(max_weighted_tardiness)
             if (self.objectives_weights[2] != 0):
-                total_waste            = self.calculate_total_waste(permutation)
-                objective_value        = objective_value + self.objectives_weights[2] * total_waste
+                total_waste = self.calculate_total_waste(permutation)
+                obj_3_lst.append(total_waste)
             if (self.objectives_weights[3] != 0):
-                total_setup_time       = self.calculate_total_setup_time(permutation)
-                objective_value        = objective_value + self.objectives_weights[3] * total_setup_time
-            if (objective_value < minimal_objective_value):
-                minimal_objective_value = objective_value
-                best_sequence           = permutation
-        self.best_sequence = best_sequence
-        return best_sequence, minimal_objective_value
-    
+                total_setup_time = self.calculate_total_setup_time(permutation)
+                obj_4_lst.append(total_setup_time)
+        if (obj_1_lst):
+            z_mean.append(np.mean(obj_1_lst))
+            z_std.append(np.std(obj_1_lst, ddof = 1))
+        else:
+            z_mean.append(None)
+            z_std.append(None)
+        if (obj_2_lst):
+            z_mean.append(np.mean(obj_2_lst))
+            z_std.append(np.std(obj_2_lst, ddof = 1))
+        else:
+            z_mean.append(None)
+            z_std.append(None)
+        if (obj_3_lst):
+            z_mean.append(np.mean(obj_3_lst))
+            z_std.append(np.std(obj_3_lst, ddof = 1))
+        else:
+            z_mean.append(None)
+            z_std.append(None)
+        if (obj_4_lst):
+            z_mean.append(np.mean(obj_4_lst))
+            z_std.append(np.std(obj_4_lst, ddof = 1))
+        else:
+            z_mean.append(None)
+            z_std.append(None)
+        return z_mean, z_std    
+
     def target_function(self, permutation): 
         schedule_matrix = self.schedule_jobs(permutation)
         objective_value = 0.0 / 1.0
         if (self.objectives_weights[0] != 0):
-            makespan               = self.calculate_makespan(schedule_matrix)
-            objective_value        = objective_value + self.objectives_weights[0] * makespan
+            makespan                 = self.calculate_makespan(schedule_matrix)
+            z_makespan               = ( (makespan - self.z_mean[0]) / (self.z_std[0] + 1e-14)) + 9
+            objective_value          = objective_value + self.objectives_weights[0] * z_makespan
         if (self.objectives_weights[1] != 0):
-            max_weighted_tardiness = self.calculate_max_weighted_tardiness(schedule_matrix)
-            objective_value        = objective_value + self.objectives_weights[1] * max_weighted_tardiness
+            max_weighted_tardiness   = self.calculate_max_weighted_tardiness(schedule_matrix)
+            z_max_weighted_tardiness = ( (max_weighted_tardiness - self.z_mean[1]) /  (self.z_std[1] + 1e-14) ) + 9
+            objective_value          = objective_value + self.objectives_weights[1] * z_max_weighted_tardiness
         if (self.objectives_weights[2] != 0):
-            total_waste            = self.calculate_total_waste(permutation)
-            objective_value        = objective_value + self.objectives_weights[2] * total_waste
+            total_waste              = self.calculate_total_waste(permutation)
+            z_total_waste            = ( (total_waste - self.z_mean[2]) /  (self.z_std[2] + 1e-14) ) + 9
+            objective_value          = objective_value + self.objectives_weights[2] * z_total_waste 
         if (self.objectives_weights[3] != 0):
-            total_setup_time       = self.calculate_total_setup_time(permutation)
-            objective_value        = objective_value + self.objectives_weights[3] * total_setup_time
+            total_setup_time         = self.calculate_total_setup_time(permutation)
+            z_total_setup_time       = ( (total_setup_time - self.z_mean[3]) /  (self.z_std[3] + 1e-14) ) + 9
+            objective_value          = objective_value + self.objectives_weights[3] * z_total_setup_time 
         return objective_value
     
     def run_mcdm_scheduler(self):
         if (len(self.objectives_weights) == 0):
             weights = [[] for item in self.comparison_matrix]
             rc      = [[] for item in self.comparison_matrix]
             g_mean  = []
@@ -265,20 +342,24 @@
             for k in range(0, len(self.crisp_inputs)):
                 job_weights = ht2fs_weight_calculation(self.crisp_inputs[k], self.uncertainty_ranges[k], self.criteria_importance[k])
                 if (len(self.job_weights) == 0):
                     self.job_weights = job_weights
                 else:
                     self.job_weights = [self.job_weights[j] + job_weights[j] for j in range(0, len(self.job_weights))]
             self.job_weights = [x / sum(self.job_weights) for x in self.job_weights]
-        if (self.brute_force == False and len(self.custom_job_sequence) == 0):
-            job_sequence, obj_fun = genetic_algorithm(self.num_jobs, self.population_size, self.elite, self.mutation_rate, self.generations, self.target_function, False)
+        if (self.objectives_weights.count(0) == 3):
+          self.z_mean, self.z_std = [0, 0, 0, 0], [1, 1, 1, 1]
+        else:
+          self.z_mean, self.z_std = self.obj_z_search()
+        if (self.brute_force == False and len(self.custom_sequence) == 0):
+            job_sequence, obj_fun = genetic_algorithm(self.num_jobs, self.population_size, self.elite, self.mutation_rate, self.generations, self.target_function, True)
             schedule_matrix       = self.schedule_jobs(job_sequence) 
-        if (self.brute_force == False and len(self.custom_job_sequence) != 0):
-            job_sequence    = self.custom_job_sequence
-            schedule_matrix = self.schedule_jobs(job_sequence) 
-            obj_fun         = self.target_function(self.custom_job_sequence)
         if (self.brute_force == True and len(self.custom_job_sequence) == 0):
             job_sequence, obj_fun = self.brute_force_search()
             schedule_matrix       = self.schedule_jobs(job_sequence)
+        if (len(self.custom_sequence) != 0):
+            job_sequence    = self.custom_job_sequence
+            schedule_matrix = self.schedule_jobs(job_sequence) 
+            obj_fun         = self.target_function(self.custom_sequence)
         return job_sequence, schedule_matrix, obj_fun
     
 ############################################################################
```

### Comparing `mcdm_scheduler-1.5.3/mcdm_scheduler/util/fuzzy_ppf_ahp.py` & `mcdm_scheduler-1.5.4/mcdm_scheduler/util/fuzzy_ppf_ahp.py`

 * *Files identical despite different names*

### Comparing `mcdm_scheduler-1.5.3/mcdm_scheduler/util/ga.py` & `mcdm_scheduler-1.5.4/mcdm_scheduler/util/ga.py`

 * *Files 4% similar despite different names*

```diff
@@ -164,15 +164,15 @@
     cost             = [item[1] for item in population]
     cost, population = (list(t) for t in zip(*sorted(zip(cost, population))))
     elite_ind        = population[0] 
     fitness          = fitness_function(cost, population_size)
     count            = 0
     while (count <= generations): 
         if (verbose == True):
-            print('Generation: ', count, '; Objective Function: ', round(elite_ind[1], 2))
+            print('Generation: ', count)
         offspring        = breeding(population, fitness, elite, target_function)  
         offspring        = mutation(offspring, mutation_rate, elite, target_function)
         cost             = [item[1] for item in offspring]
         cost, population = (list(t) for t in zip(*sorted(zip(cost, offspring ))))
         elite_child      = population[0]
         fitness          = fitness_function(cost, population_size)
         if(elite_ind[1] > elite_child[1]):
```

### Comparing `mcdm_scheduler-1.5.3/mcdm_scheduler/util/ht2fs.py` & `mcdm_scheduler-1.5.4/mcdm_scheduler/util/ht2fs.py`

 * *Files identical despite different names*

### Comparing `mcdm_scheduler-1.5.3/mcdm_scheduler.egg-info/PKG-INFO` & `mcdm_scheduler-1.5.4/mcdm_scheduler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcdm-scheduler
-Version: 1.5.3
+Version: 1.5.4
 Summary: A Library Incorporating a MCDM tools for Scheduling Problems
 Home-page: https://github.com/Valdecy/mcdm_scheduler
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mcdm_scheduler-1.5.3/setup.py` & `mcdm_scheduler-1.5.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='mcdm_scheduler',
-    version='1.5.3',
+    version='1.5.4',
     license='GNU',
     author='Valdecy Pereira',
     author_email='valdecy.pereira@gmail.com',
     url='https://github.com/Valdecy/mcdm_scheduler',
     packages=find_packages(),
     install_requires=[
         'matplotlib',
```

