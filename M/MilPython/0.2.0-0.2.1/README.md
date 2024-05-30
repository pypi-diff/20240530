# Comparing `tmp/MilPython-0.2.0.tar.gz` & `tmp/MilPython-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MilPython-0.2.0.tar", last modified: Mon Feb 26 15:00:35 2024, max compression
+gzip compressed data, was "MilPython-0.2.1.tar", last modified: Thu May 30 09:55:03 2024, max compression
```

## Comparing `MilPython-0.2.0.tar` & `MilPython-0.2.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-02-26 15:00:35.002499 MilPython-0.2.0/
--rw-rw-rw-   0        0        0     1091 2024-02-15 06:28:24.000000 MilPython-0.2.0/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2024-02-26 15:00:34.933041 MilPython-0.2.0/MilPython.egg-info/
--rw-rw-rw-   0        0        0      856 2024-02-15 10:42:06.000000 MilPython-0.2.0/MilPython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      590 2024-02-15 10:42:06.000000 MilPython-0.2.0/MilPython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-15 10:42:06.000000 MilPython-0.2.0/MilPython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-02-15 10:42:06.000000 MilPython-0.2.0/MilPython.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-02-15 10:42:06.000000 MilPython-0.2.0/MilPython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1157 2024-02-26 15:00:35.001503 MilPython-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      514 2024-02-20 15:19:09.000000 MilPython-0.2.0/README.md
--rw-rw-rw-   0        0        0      317 2024-02-26 15:00:10.000000 MilPython-0.2.0/UpdateVersion_Info.md
-drwxrwxrwx   0        0        0        0 2024-02-26 15:00:34.986659 MilPython-0.2.0/dist/
--rw-rw-rw-   0        0        0     7891 2024-02-26 15:00:10.000000 MilPython-0.2.0/dist/MilPython-0.0.1-py3-none-any.whl
--rw-rw-rw-   0        0        0     6481 2024-02-26 15:00:10.000000 MilPython-0.2.0/dist/MilPython-0.0.1.tar.gz
--rw-rw-rw-   0        0        0    20949 2024-02-26 15:00:10.000000 MilPython-0.2.0/dist/MilPython-0.0.2.tar.gz
--rw-rw-rw-   0        0        0    21090 2024-02-26 15:00:10.000000 MilPython-0.2.0/dist/MilPython-0.0.3.tar.gz
--rw-rw-rw-   0        0        0    21248 2024-02-26 15:00:10.000000 MilPython-0.2.0/dist/MilPython-0.0.4.tar.gz
--rw-rw-rw-   0        0        0    21093 2024-02-26 15:00:10.000000 MilPython-0.2.0/dist/MilPython-0.0.5.tar.gz
--rw-rw-rw-   0        0        0    21110 2024-02-26 15:00:10.000000 MilPython-0.2.0/dist/MilPython-0.0.6.tar.gz
--rw-rw-rw-   0        0        0   120653 2024-02-26 15:00:10.000000 MilPython-0.2.0/dist/MilPython-0.0.7.tar.gz
--rw-rw-rw-   0        0        0   121010 2024-02-26 15:00:10.000000 MilPython-0.2.0/dist/MilPython-0.0.8.tar.gz
--rw-rw-rw-   0        0        0   241651 2024-02-26 15:00:10.000000 MilPython-0.2.0/dist/MilPython-0.0.9.tar.gz
--rw-rw-rw-   0        0        0  1212444 2024-02-26 15:00:10.000000 MilPython-0.2.0/dist/MilPython-0.1.0.tar.gz
--rw-rw-rw-   0        0        0  1819185 2024-02-26 15:00:10.000000 MilPython-0.2.0/dist/MilPython-0.1.1.tar.gz
--rw-rw-rw-   0        0        0       42 2024-02-26 15:00:35.002499 MilPython-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      873 2024-02-26 10:53:52.000000 MilPython-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-26 15:00:34.922122 MilPython-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2024-02-26 15:00:34.994531 MilPython-0.2.0/src/MilPython/
--rw-rw-rw-   0        0        0      295 2024-02-21 15:24:19.000000 MilPython-0.2.0/src/MilPython/__init__.py
--rw-rw-rw-   0        0        0      619 2024-02-15 19:14:53.000000 MilPython-0.2.0/src/MilPython/equation.py
--rw-rw-rw-   0        0        0      953 2024-02-16 08:26:55.000000 MilPython-0.2.0/src/MilPython/lpInputdata.py
--rw-rw-rw-   0        0        0    12976 2024-02-21 15:24:19.000000 MilPython-0.2.0/src/MilPython/lpMain.py
--rw-rw-rw-   0        0        0     4302 2024-02-20 14:03:53.000000 MilPython-0.2.0/src/MilPython/lpObject.py
--rw-rw-rw-   0        0        0     3721 2024-02-20 14:03:53.000000 MilPython-0.2.0/src/MilPython/lpStateVar.py
--rw-rw-rw-   0        0        0      622 2024-02-21 15:24:19.000000 MilPython-0.2.0/src/MilPython/tools.py
-drwxrwxrwx   0        0        0        0 2024-02-26 15:00:35.000506 MilPython-0.2.0/src/MilPython.egg-info/
--rw-rw-rw-   0        0        0     1157 2024-02-26 15:00:34.000000 MilPython-0.2.0/src/MilPython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      958 2024-02-26 15:00:34.000000 MilPython-0.2.0/src/MilPython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-26 15:00:34.000000 MilPython-0.2.0/src/MilPython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-02-26 15:00:34.000000 MilPython-0.2.0/src/MilPython.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-02-26 15:00:34.000000 MilPython-0.2.0/src/MilPython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        7 2024-02-26 15:00:26.000000 MilPython-0.2.0/version.txt
--rwxrwxrwx   0        0        0     1731 2024-02-26 15:00:11.000000 MilPython-0.2.0/versionUpdate.bat
+drwxrwxrwx   0        0        0        0 2024-05-30 09:55:03.323595 MilPython-0.2.1/
+-rw-rw-rw-   0        0        0     1091 2024-02-15 06:28:24.000000 MilPython-0.2.1/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 09:55:03.293136 MilPython-0.2.1/MilPython.egg-info/
+-rw-rw-rw-   0        0        0      856 2024-02-15 10:42:06.000000 MilPython-0.2.1/MilPython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      590 2024-02-15 10:42:06.000000 MilPython-0.2.1/MilPython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-15 10:42:06.000000 MilPython-0.2.1/MilPython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-02-15 10:42:06.000000 MilPython-0.2.1/MilPython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-02-15 10:42:06.000000 MilPython-0.2.1/MilPython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1157 2024-05-30 09:55:03.323595 MilPython-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      514 2024-02-20 15:19:09.000000 MilPython-0.2.1/README.md
+-rw-rw-rw-   0        0        0      317 2024-02-26 15:04:52.000000 MilPython-0.2.1/UpdateVersion_Info.md
+drwxrwxrwx   0        0        0        0 2024-05-30 09:55:03.305595 MilPython-0.2.1/dist/
+-rw-rw-rw-   0        0        0     7891 2024-02-26 15:04:52.000000 MilPython-0.2.1/dist/MilPython-0.0.1-py3-none-any.whl
+-rw-rw-rw-   0        0        0     6481 2024-02-26 15:04:52.000000 MilPython-0.2.1/dist/MilPython-0.0.1.tar.gz
+-rw-rw-rw-   0        0        0    20949 2024-02-26 15:04:52.000000 MilPython-0.2.1/dist/MilPython-0.0.2.tar.gz
+-rw-rw-rw-   0        0        0    21090 2024-02-26 15:04:52.000000 MilPython-0.2.1/dist/MilPython-0.0.3.tar.gz
+-rw-rw-rw-   0        0        0    21248 2024-02-26 15:04:52.000000 MilPython-0.2.1/dist/MilPython-0.0.4.tar.gz
+-rw-rw-rw-   0        0        0    21093 2024-02-26 15:04:52.000000 MilPython-0.2.1/dist/MilPython-0.0.5.tar.gz
+-rw-rw-rw-   0        0        0    21110 2024-02-26 15:04:52.000000 MilPython-0.2.1/dist/MilPython-0.0.6.tar.gz
+-rw-rw-rw-   0        0        0   120653 2024-02-26 15:04:52.000000 MilPython-0.2.1/dist/MilPython-0.0.7.tar.gz
+-rw-rw-rw-   0        0        0   121010 2024-02-26 15:04:52.000000 MilPython-0.2.1/dist/MilPython-0.0.8.tar.gz
+-rw-rw-rw-   0        0        0   241651 2024-02-26 15:04:52.000000 MilPython-0.2.1/dist/MilPython-0.0.9.tar.gz
+-rw-rw-rw-   0        0        0  1212444 2024-02-26 15:04:52.000000 MilPython-0.2.1/dist/MilPython-0.1.0.tar.gz
+-rw-rw-rw-   0        0        0  1819185 2024-02-26 15:04:52.000000 MilPython-0.2.1/dist/MilPython-0.1.1.tar.gz
+-rw-rw-rw-   0        0        0       42 2024-05-30 09:55:03.324593 MilPython-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      873 2024-05-30 09:54:22.000000 MilPython-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 09:55:03.281830 MilPython-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-30 09:55:03.314596 MilPython-0.2.1/src/MilPython/
+-rw-rw-rw-   0        0        0      295 2024-02-21 15:24:19.000000 MilPython-0.2.1/src/MilPython/__init__.py
+-rw-rw-rw-   0        0        0      619 2024-02-15 19:14:53.000000 MilPython-0.2.1/src/MilPython/equation.py
+-rw-rw-rw-   0        0        0     1046 2024-05-30 09:36:46.000000 MilPython-0.2.1/src/MilPython/lpInputdata.py
+-rw-rw-rw-   0        0        0    13245 2024-05-30 09:45:38.000000 MilPython-0.2.1/src/MilPython/lpMain.py
+-rw-rw-rw-   0        0        0     4302 2024-02-20 14:03:53.000000 MilPython-0.2.1/src/MilPython/lpObject.py
+-rw-rw-rw-   0        0        0     3721 2024-02-20 14:03:53.000000 MilPython-0.2.1/src/MilPython/lpStateVar.py
+-rw-rw-rw-   0        0        0      622 2024-02-21 15:24:19.000000 MilPython-0.2.1/src/MilPython/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-30 09:55:03.322595 MilPython-0.2.1/src/MilPython.egg-info/
+-rw-rw-rw-   0        0        0     1157 2024-05-30 09:55:03.000000 MilPython-0.2.1/src/MilPython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      958 2024-05-30 09:55:03.000000 MilPython-0.2.1/src/MilPython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 09:55:03.000000 MilPython-0.2.1/src/MilPython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-30 09:55:03.000000 MilPython-0.2.1/src/MilPython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-30 09:55:03.000000 MilPython-0.2.1/src/MilPython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        7 2024-05-30 09:54:33.000000 MilPython-0.2.1/version.txt
+-rwxrwxrwx   0        0        0     1731 2024-02-26 15:04:52.000000 MilPython-0.2.1/versionUpdate.bat
```

### Comparing `MilPython-0.2.0/LICENSE.txt` & `MilPython-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MilPython-0.2.0/MilPython.egg-info/PKG-INFO` & `MilPython-0.2.1/MilPython.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `MilPython-0.2.0/MilPython.egg-info/SOURCES.txt` & `MilPython-0.2.1/MilPython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MilPython-0.2.0/PKG-INFO` & `MilPython-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MilPython
-Version: 0.2.0
+Version: 0.2.1
 Summary: Framework for building MILP optimizations for time series with gurobipy
 Home-page: https://github.com/hanneshanse/MilPython
 Author: Hannes Hanse
 Author-email: hannes.hanse@tu-clausthal.de
 License: MIT
 Keywords: milp,time series,optimization,gurobi,gurobipy
 Classifier: Programming Language :: Python :: 3
```

### Comparing `MilPython-0.2.0/README.md` & `MilPython-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `MilPython-0.2.0/dist/MilPython-0.0.1-py3-none-any.whl` & `MilPython-0.2.1/dist/MilPython-0.0.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `MilPython-0.2.0/dist/MilPython-0.0.1.tar.gz` & `MilPython-0.2.1/dist/MilPython-0.0.1.tar.gz`

 * *Files identical despite different names*

### Comparing `MilPython-0.2.0/dist/MilPython-0.0.2.tar.gz` & `MilPython-0.2.1/dist/MilPython-0.0.2.tar.gz`

 * *Files identical despite different names*

### Comparing `MilPython-0.2.0/dist/MilPython-0.0.3.tar.gz` & `MilPython-0.2.1/dist/MilPython-0.0.3.tar.gz`

 * *Files identical despite different names*

### Comparing `MilPython-0.2.0/dist/MilPython-0.0.4.tar.gz` & `MilPython-0.2.1/dist/MilPython-0.0.4.tar.gz`

 * *Files identical despite different names*

### Comparing `MilPython-0.2.0/dist/MilPython-0.0.5.tar.gz` & `MilPython-0.2.1/dist/MilPython-0.0.5.tar.gz`

 * *Files identical despite different names*

### Comparing `MilPython-0.2.0/dist/MilPython-0.0.6.tar.gz` & `MilPython-0.2.1/dist/MilPython-0.0.6.tar.gz`

 * *Files identical despite different names*

### Comparing `MilPython-0.2.0/dist/MilPython-0.0.7.tar.gz` & `MilPython-0.2.1/dist/MilPython-0.0.7.tar.gz`

 * *Files identical despite different names*

### Comparing `MilPython-0.2.0/dist/MilPython-0.0.8.tar.gz` & `MilPython-0.2.1/dist/MilPython-0.0.8.tar.gz`

 * *Files identical despite different names*

### Comparing `MilPython-0.2.0/dist/MilPython-0.0.9.tar.gz` & `MilPython-0.2.1/dist/MilPython-0.0.9.tar.gz`

 * *Files identical despite different names*

### Comparing `MilPython-0.2.0/dist/MilPython-0.1.0.tar.gz` & `MilPython-0.2.1/dist/MilPython-0.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `MilPython-0.2.0/dist/MilPython-0.1.1.tar.gz` & `MilPython-0.2.1/dist/MilPython-0.1.1.tar.gz`

 * *Files identical despite different names*

### Comparing `MilPython-0.2.0/setup.py` & `MilPython-0.2.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "Readme.md").read_text()
 
 setup(
     name='MilPython',
-    version='0.2.0',
+    version='0.2.1',
     description='Framework for building MILP optimizations for time series with gurobipy',
     license='MIT',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Hannes Hanse',
     author_email='hannes.hanse@tu-clausthal.de',
     keywords=['milp','time series','optimization','gurobi','gurobipy'],
```

### Comparing `MilPython-0.2.0/src/MilPython/equation.py` & `MilPython-0.2.1/src/MilPython/equation.py`

 * *Files identical despite different names*

### Comparing `MilPython-0.2.0/src/MilPython/lpInputdata.py` & `MilPython-0.2.1/src/MilPython/lpInputdata.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 class LPInputdata:
     '''
     Class, that contains all input data for the optimization.
     Contains time series as dict
     In der Initialisierung des LPMain-Objekts wird dieser Klasse außerdem die Gesamtanzahl an Variablen zugewiesen
     '''
-    def __init__(self,data:dict,dt_h:float):
+    def __init__(self,data:dict,dt_h:float,verbose=True):
         """
         Args:
             data (dict): dictionary of all important input data
             dt_h (float): stepsize in hours
         """        
         self.data = data                            # dict containing time series input data
         self.steps=len(next(iter(data.items()))[1]) # number of steps                           #! leads to error if first item in data is no time series
         self.dt_h = dt_h                            # stepsize in hours
         self.num_vars=None                          # total number of stateVariables
-        self.num_vars_timedep=None                  # number of time dependent stateVars
+        self.num_vars_timedep=None                  # number of time dependent stateVars
+        self.verbose=verbose                        #verbosity of optimization
```

### Comparing `MilPython-0.2.0/src/MilPython/lpMain.py` & `MilPython-0.2.1/src/MilPython/lpMain.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,14 +160,17 @@
         Aeq, beq, senses: Matrix or vector of equations with the comparison operator of each equation
         ctype, lb, ub: Type and upper and lower limits of the variables
         f: target function
         '''
         # Transfer the optimization problem to the Gurobi API.
         # Create an empty problem
         problem = gp.Model()
+        if self.inputdata.verbose == False:
+            problem.setParam('LogToConsole',0)
+            problem.setParam('Warning',1)
         # add variables
         x = problem.addMVar(shape=self.inputdata.num_vars,lb=self.lb,ub=self.ub,vtype=self.vtypes)
         # x = problem.addMVar(shape=self.inputdata.num_vars,lb=self.lb,ub=self.ub,vtype=['C' for _ in range(self.inputdata.num_vars)])
         # Pass target function
         
         if objective == Obj.MINIMIZE:
             problem.setObjective(self.f @ x, gp.GRB.MINIMIZE)    
@@ -239,14 +242,17 @@
         ctype, lb, ub: Type and upper and lower limits of the variables
         f: target function
         '''
         import cplex
         # nbew empty problem
         problem = cplex.Cplex()
 
+        if self.inputdata.verbose == False:
+            problem.set_log_stream(None)
+            problem.set_results_stream(None)
         # Adding variables
         problem.variables.add(names=['x' + str(i) for i in range(self.inputdata.num_vars)])
 
         # formatting the variable-type-list to fit cplex
         types = [(i, problem.variables.type.continuous) if vtype_i == 'C' 
                     else (i, problem.variables.type.binary) if vtype_i == 'B'
                     else (i, problem.variables.type.semi_continuous) if vtype_i == 'S'
```

### Comparing `MilPython-0.2.0/src/MilPython/lpObject.py` & `MilPython-0.2.1/src/MilPython/lpObject.py`

 * *Files identical despite different names*

### Comparing `MilPython-0.2.0/src/MilPython/lpStateVar.py` & `MilPython-0.2.1/src/MilPython/lpStateVar.py`

 * *Files identical despite different names*

### Comparing `MilPython-0.2.0/src/MilPython/tools.py` & `MilPython-0.2.1/src/MilPython/tools.py`

 * *Files identical despite different names*

### Comparing `MilPython-0.2.0/src/MilPython.egg-info/PKG-INFO` & `MilPython-0.2.1/src/MilPython.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MilPython
-Version: 0.2.0
+Version: 0.2.1
 Summary: Framework for building MILP optimizations for time series with gurobipy
 Home-page: https://github.com/hanneshanse/MilPython
 Author: Hannes Hanse
 Author-email: hannes.hanse@tu-clausthal.de
 License: MIT
 Keywords: milp,time series,optimization,gurobi,gurobipy
 Classifier: Programming Language :: Python :: 3
```

### Comparing `MilPython-0.2.0/src/MilPython.egg-info/SOURCES.txt` & `MilPython-0.2.1/src/MilPython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MilPython-0.2.0/versionUpdate.bat` & `MilPython-0.2.1/versionUpdate.bat`

 * *Files identical despite different names*

