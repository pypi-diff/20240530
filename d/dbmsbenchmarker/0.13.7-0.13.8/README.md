# Comparing `tmp/dbmsbenchmarker-0.13.7.tar.gz` & `tmp/dbmsbenchmarker-0.13.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/DBMS-Benchmarker/DBMS-Benchmarker/dist/.tmp-hip66lo2/dbmsbenchmarker-0.13.7.tar", last modified: Fri May 17 11:49:46 2024, max compression
+gzip compressed data, was "/home/runner/work/DBMS-Benchmarker/DBMS-Benchmarker/dist/.tmp-1yhg4omy/dbmsbenchmarker-0.13.8.tar", last modified: Thu May 30 14:23:43 2024, max compression
```

## Comparing `dbmsbenchmarker-0.13.7.tar` & `dbmsbenchmarker-0.13.8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:49:46.000000 dbmsbenchmarker-0.13.7/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11031 2024-05-17 11:49:46.000000 dbmsbenchmarker-0.13.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10182 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:49:46.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    98237 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/benchmarker.py
--rw-r--r--   0 runner    (1001) docker     (127)    36491 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)    28813 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)    22030 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    28802 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)    18245 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:49:46.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:49:46.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:49:46.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/assets/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/assets/icons/check_box-24px.svg
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/assets/icons/check_box_outline_blank-24px.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/assets/icons/chevron_down.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/assets/icons/chevron_up.svg
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/assets/icons/clear-black-24dp.svg
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/assets/icons/get_app-black-24dp.svg
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/assets/icons/info-24px.svg
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/assets/icons/radio_button_unchecked-24px.svg
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/assets/icons/tune-black-24dp.svg
--rw-r--r--   0 runner    (1001) docker     (127)     8214 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/assets/styles.css
--rw-r--r--   0 runner    (1001) docker     (127)     8751 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)   137186 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/dashboardcli.py
--rw-r--r--   0 runner    (1001) docker     (127)    78029 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:49:46.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11031 2024-05-17 11:49:46.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-17 11:49:46.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 11:49:46.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-17 11:49:46.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-17 11:49:46.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-17 11:49:46.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 11:49:46.000000 dbmsbenchmarker-0.13.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:23:43.000000 dbmsbenchmarker-0.13.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-30 14:23:39.000000 dbmsbenchmarker-0.13.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-30 14:23:39.000000 dbmsbenchmarker-0.13.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11031 2024-05-30 14:23:43.000000 dbmsbenchmarker-0.13.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10182 2024-05-30 14:23:39.000000 dbmsbenchmarker-0.13.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:23:43.000000 dbmsbenchmarker-0.13.8/dbmsbenchmarker/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-30 14:23:39.000000 dbmsbenchmarker-0.13.8/dbmsbenchmarker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98546 2024-05-30 14:23:39.000000 dbmsbenchmarker-0.13.8/dbmsbenchmarker/benchmarker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36491 2024-05-30 14:23:39.000000 dbmsbenchmarker-0.13.8/dbmsbenchmarker/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28837 2024-05-30 14:23:39.000000 dbmsbenchmarker-0.13.8/dbmsbenchmarker/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22030 2024-05-30 14:23:39.000000 dbmsbenchmarker-0.13.8/dbmsbenchmarker/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28802 2024-05-30 14:23:39.000000 dbmsbenchmarker-0.13.8/dbmsbenchmarker/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-05-30 14:23:39.000000 dbmsbenchmarker-0.13.8/dbmsbenchmarker/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18245 2024-05-30 14:23:39.000000 dbmsbenchmarker-0.13.8/dbmsbenchmarker/reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:23:43.000000 dbmsbenchmarker-0.13.8/dbmsbenchmarker/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-30 14:23:39.000000 dbmsbenchmarker-0.13.8/dbmsbenchmarker/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:23:43.000000 dbmsbenchmarker-0.13.8/dbmsbenchmarker/scripts/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:23:43.000000 dbmsbenchmarker-0.13.8/dbmsbenchmarker/scripts/assets/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-30 14:23:39.000000 dbmsbenchmarker-0.13.8/dbmsbenchmarker/scripts/assets/icons/check_box-24px.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-30 14:23:39.000000 dbmsbenchmarker-0.13.8/dbmsbenchmarker/scripts/assets/icons/check_box_outline_blank-24px.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-30 14:23:39.000000 dbmsbenchmarker-0.13.8/dbmsbenchmarker/scripts/assets/icons/chevron_down.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-30 14:23:39.000000 dbmsbenchmarker-0.13.8/dbmsbenchmarker/scripts/assets/icons/chevron_up.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-30 14:23:39.000000 dbmsbenchmarker-0.13.8/dbmsbenchmarker/scripts/assets/icons/clear-black-24dp.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-30 14:23:39.000000 dbmsbenchmarker-0.13.8/dbmsbenchmarker/scripts/assets/icons/get_app-black-24dp.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-30 14:23:39.000000 dbmsbenchmarker-0.13.8/dbmsbenchmarker/scripts/assets/icons/info-24px.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-30 14:23:39.000000 dbmsbenchmarker-0.13.8/dbmsbenchmarker/scripts/assets/icons/radio_button_unchecked-24px.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-30 14:23:39.000000 dbmsbenchmarker-0.13.8/dbmsbenchmarker/scripts/assets/icons/tune-black-24dp.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     8214 2024-05-30 14:23:39.000000 dbmsbenchmarker-0.13.8/dbmsbenchmarker/scripts/assets/styles.css
+-rw-r--r--   0 runner    (1001) docker     (127)    10007 2024-05-30 14:23:39.000000 dbmsbenchmarker-0.13.8/dbmsbenchmarker/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)   137186 2024-05-30 14:23:39.000000 dbmsbenchmarker-0.13.8/dbmsbenchmarker/scripts/dashboardcli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78029 2024-05-30 14:23:39.000000 dbmsbenchmarker-0.13.8/dbmsbenchmarker/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:23:43.000000 dbmsbenchmarker-0.13.8/dbmsbenchmarker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11031 2024-05-30 14:23:43.000000 dbmsbenchmarker-0.13.8/dbmsbenchmarker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-30 14:23:43.000000 dbmsbenchmarker-0.13.8/dbmsbenchmarker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 14:23:43.000000 dbmsbenchmarker-0.13.8/dbmsbenchmarker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-30 14:23:43.000000 dbmsbenchmarker-0.13.8/dbmsbenchmarker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-30 14:23:43.000000 dbmsbenchmarker-0.13.8/dbmsbenchmarker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-30 14:23:43.000000 dbmsbenchmarker-0.13.8/dbmsbenchmarker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 14:23:43.000000 dbmsbenchmarker-0.13.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-30 14:23:39.000000 dbmsbenchmarker-0.13.8/setup.py
```

### Comparing `dbmsbenchmarker-0.13.7/LICENSE` & `dbmsbenchmarker-0.13.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dbmsbenchmarker-0.13.7/PKG-INFO` & `dbmsbenchmarker-0.13.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbmsbenchmarker
-Version: 0.13.7
+Version: 0.13.8
 Summary: DBMS-Benchmarker is a Python-based application-level blackbox benchmark tool for Database Management Systems (DBMS). It connects to a given list of DBMS (via JDBC) and runs a given list of parametrized and randomized (SQL) benchmark queries. Evaluations are available via Python interface, in reports and at an interactive multi-dimensional dashboard.
 Home-page: https://github.com/Beuth-Erdelt/DBMS-Benchmarker
 Author: Patrick Erdelt
 Author-email: perdelt@beuth-hochschule.de
 License: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `dbmsbenchmarker-0.13.7/README.md` & `dbmsbenchmarker-0.13.8/README.md`

 * *Files identical despite different names*

### Comparing `dbmsbenchmarker-0.13.7/dbmsbenchmarker/benchmarker.py` & `dbmsbenchmarker-0.13.8/dbmsbenchmarker/benchmarker.py`

 * *Files 0% similar despite different names*

```diff
@@ -418,14 +418,16 @@
         self.queries = []
         # should benchmarks be overwritten
         self.overwrite = False
         # clear all possibly present benchmarks
         self.clearBenchmarks()
         # should result folder be created
         self.continuing = False
+        # overwrite header of workload file
+        self.workload = {}
         self.path = ""
         if result_path is None:
             if code is None:
                 self.code = str(round(time.time()))
             else:
                 self.code = str(int(code))
             self.path = self.code
@@ -554,15 +556,19 @@
                 copyfile(filename, self.path+'/queries.config')
             else:
                 self.logger.exception('Caught an error: Query file not found')
                 exit(1)
         with open(filename,'r') as inp:
             self.queryconfig = ast.literal_eval(inp.read())
             # global setting in a class variable
-            # overwrites parts of query file
+            # overwrites parts of query file - header
+            if len(self.workload) > 0:
+                for k,v in self.workload.items():
+                    self.queryconfig[k] = v
+            # overwrites parts of query file - queries
             if tools.query.template is not None:
                 for i,q in enumerate(self.queryconfig['queries']):
                     self.queryconfig['queries'][i] = {**q, **tools.query.template}
                     with open(self.path+'/queries.config','w') as outp:
                         pprint.pprint(self.queryconfig, outp)
             self.queries = self.queryconfig["queries"].copy()
             # default for all queries is being 'active'
@@ -1907,15 +1913,16 @@
 
 
 class inspector(benchmarker):
     """
     Class for inspecting done benchmarks
     """
     def __init__(self, result_path, code, anonymize=False, silent=False):
-        benchmarker.__init__(self,result_path=result_path+"/"+str(code), anonymize=anonymize)
+        path = (result_path+"/"+str(code)).replace("//", "/")
+        benchmarker.__init__(self,result_path=path, anonymize=anonymize)
         self.getConfig()
         self.readResultfolder(silent=silent)
         if not silent:
             print("Connections:")
             for c in self.connections:
                 print(c['name'])
             print("Queries:")
```

### Comparing `dbmsbenchmarker-0.13.7/dbmsbenchmarker/evaluator.py` & `dbmsbenchmarker-0.13.8/dbmsbenchmarker/evaluator.py`

 * *Files identical despite different names*

### Comparing `dbmsbenchmarker-0.13.7/dbmsbenchmarker/inspector.py` & `dbmsbenchmarker-0.13.8/dbmsbenchmarker/inspector.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 class inspector():
     """
     Class for inspecting done benchmarks
     """
     def __init__(self, result_path, anonymize=False):
         self.result_path = result_path
         self.anonymize = anonymize
-        self.list_experiments = [f for f in listdir(self.result_path) if isdir(join(self.result_path, f)) and f.isdigit()]
+        self.list_experiments = list(reversed(sorted([f for f in listdir(self.result_path) if isdir(join(self.result_path, f)) and f.isdigit()])))
         self.queries_successful = []
     def get_experiments_preview(self):
         workload_preview = {}
         for code in self.list_experiments:
             filename_query = self.result_path+'/'+code+'/queries.config'
             filename_connections = self.result_path+'/'+code+'/connections.config'
             filename_protocol = self.result_path+'/'+code+'/protocol.json'
```

### Comparing `dbmsbenchmarker-0.13.7/dbmsbenchmarker/layout.py` & `dbmsbenchmarker-0.13.8/dbmsbenchmarker/layout.py`

 * *Files identical despite different names*

### Comparing `dbmsbenchmarker-0.13.7/dbmsbenchmarker/monitor.py` & `dbmsbenchmarker-0.13.8/dbmsbenchmarker/monitor.py`

 * *Files identical despite different names*

### Comparing `dbmsbenchmarker-0.13.7/dbmsbenchmarker/parameter.py` & `dbmsbenchmarker-0.13.8/dbmsbenchmarker/parameter.py`

 * *Files identical despite different names*

### Comparing `dbmsbenchmarker-0.13.7/dbmsbenchmarker/reporter.py` & `dbmsbenchmarker-0.13.8/dbmsbenchmarker/reporter.py`

 * *Files identical despite different names*

### Comparing `dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/assets/icons/chevron_down.svg` & `dbmsbenchmarker-0.13.8/dbmsbenchmarker/scripts/assets/icons/chevron_down.svg`

 * *Files identical despite different names*

### Comparing `dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/assets/icons/chevron_up.svg` & `dbmsbenchmarker-0.13.8/dbmsbenchmarker/scripts/assets/icons/chevron_up.svg`

 * *Files identical despite different names*

### Comparing `dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/assets/styles.css` & `dbmsbenchmarker-0.13.8/dbmsbenchmarker/scripts/assets/styles.css`

 * *Files identical despite different names*

### Comparing `dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/cli.py` & `dbmsbenchmarker-0.13.8/dbmsbenchmarker/scripts/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,146 +22,154 @@
 import random
 from datetime import datetime, timedelta
 
 from dbmsbenchmarker import *
 
 
 def run_benchmarker():
-	# argparse
-	parser = argparse.ArgumentParser(description='A benchmark tool for RDBMS. It connects to a given list of RDBMS via JDBC and runs a given list benchmark queries. Optionally some reports are generated.')
-	parser.add_argument('mode', help='run benchmarks and save results, or just read benchmark results from folder, or continue with missing benchmarks only', choices=['run', 'read', 'continue'])
-	parser.add_argument('-d', '--debug', help='dump debug informations', action='store_true')
-	parser.add_argument('-b', '--batch', help='batch mode (more protocol-like output), automatically on for debug mode', action='store_true')
-	parser.add_argument('-qf', '--query-file', help='name of query config file', default='queries.config')
-	parser.add_argument('-cf', '--connection-file', help='name of connection config file', default='connections.config')
-	parser.add_argument('-q', '--query', help='number of query to benchmark', default=None)
-	parser.add_argument('-c', '--connection', help='name of connection to benchmark', default=None)
-	parser.add_argument('-ca', '--connection-alias', help='alias of connection to benchmark', default='')
-	parser.add_argument('-f', '--config-folder', help='folder containing query and connection config files. If set, the names connections.config and queries.config are assumed automatically.', default=None)
-	parser.add_argument('-r', '--result-folder', help='folder for storing benchmark result files, default is given by timestamp', default=None)
-	parser.add_argument('-e', '--generate-evaluation', help='generate new evaluation file', default='no', choices=['no','yes'])
-	parser.add_argument('-w', '--working', help='working per query or connection', default='query', choices=['query','connection'])
-	#parser.add_argument('-a', '--anonymize', help='anonymize all dbms', action='store_true', default=False)
-	#parser.add_argument('-u', '--unanonymize', help='unanonymize some dbms, only sensible in combination with anonymize', nargs='*', default=[])
-	parser.add_argument('-p', '--numProcesses', help='Number of parallel client processes. Global setting, can be overwritten by connection. Default is 1.', default=None)
-	parser.add_argument('-s', '--seed', help='random seed', default=None)
-	parser.add_argument('-cs', '--copy-subfolder', help='copy subfolder of result folder', action='store_true')
-	parser.add_argument('-ms', '--max-subfolders', help='maximum number of subfolders of result folder', default=None)
-	parser.add_argument('-sl', '--sleep', help='sleep SLEEP seconds before going to work', default=0)
-	parser.add_argument('-st', '--start-time', help='sleep until START-TIME before beginning benchmarking', default=None)
-	parser.add_argument('-sf', '--subfolder', help='stores results in a SUBFOLDER of the result folder', default=None)
-	parser.add_argument('-vq', '--verbose-queries', help='print every query that is sent', action='store_true', default=False)
-	parser.add_argument('-vs', '--verbose-statistics', help='print statistics about query that have been sent', action='store_true', default=False)
-	parser.add_argument('-vr', '--verbose-results', help='print result sets of every query that have been sent', action='store_true', default=False)
-	parser.add_argument('-vp', '--verbose-process', help='print result sets of every query that have been sent', action='store_true', default=False)
-	parser.add_argument('-pn', '--num-run', help='Parameter: Number of executions per query', default=0)
-	parser.add_argument('-m', '--metrics', help='collect hardware metrics per query', action='store_true', default=False)
-	parser.add_argument('-mps', '--metrics-per-stream', help='collect hardware metrics per stream', action='store_true', default=False)
-	#parser.add_argument('-pt', '--timeout', help='Parameter: Timeout in seconds', default=0)
-	logger = logging.getLogger('dbmsbenchmarker')
-	args = parser.parse_args()
-	# evaluate args
-	if args.debug:
-		logging.basicConfig(level=logging.DEBUG)
-		bBatch = True
-	else:
-		logging.basicConfig(level=logging.INFO)
-		bBatch = args.batch
-	# sleep before going to work
-	if int(args.sleep) > 0:
-		logger.debug("Sleeping {} seconds before going to work".format(int(args.sleep)))
-		time.sleep(int(args.sleep))
-	# make a copy of result folder
-	subfolder = args.subfolder
-	rename_connection = ''
-	rename_alias = ''
-	if args.copy_subfolder and len(subfolder) > 0:
-		client = 1
-		while True:
-			if args.max_subfolders is not None and client > int(args.max_subfolders):
-				exit()
-			resultpath = args.result_folder+'/'+subfolder+'-'+str(client)
-			logger.debug("Checking if {} is suitable folder for free job number".format(resultpath))
-			if path.isdir(resultpath):
-				client = client + 1
-				waiting = random.randint(1, 10)
-				logger.debug("Sleeping {} seconds before checking for next free job number".format(waiting))
-				time.sleep(waiting)
-			else:
-				makedirs(resultpath)
-				break
-		subfolder = subfolder+'-'+str(client)
-		rename_connection = args.connection+'-'+str(client)
-		logger.debug("Rename connection {} to {}".format(args.connection, rename_connection))
-		rename_alias = args.connection_alias+'-'+str(client)
-		logger.debug("Rename alias {} to {}".format(args.connection_alias, rename_alias))
-	# sleep before going to work
-	if args.start_time is not None:
-		#logger.debug(args.start_time)
-		now = datetime.utcnow()
-		try:
-			start = datetime.strptime(args.start_time, '%Y-%m-%d %H:%M:%S')
-			if start > now:
-				wait = (start-now).seconds
-				now_string = now.strftime('%Y-%m-%d %H:%M:%S')
-				logger.debug("Sleeping until {} before going to work ({} seconds, it is {} now)".format(args.start_time, wait, now_string))
-				time.sleep(int(wait))
-		except Exception as e:
-			logger.debug("Invalid format: {}".format(args.start_time))
-	# set verbose level
-	if args.verbose_queries:
-		benchmarker.BENCHMARKER_VERBOSE_QUERIES = True
-	if args.verbose_statistics:
-		benchmarker.BENCHMARKER_VERBOSE_STATISTICS = True
-	if args.verbose_results:
-		benchmarker.BENCHMARKER_VERBOSE_RESULTS = True
-	if args.verbose_process:
-		benchmarker.BENCHMARKER_VERBOSE_PROCESS = True
-	if int(args.num_run) > 0:
-		querymanagement = {
- 			'numRun': int(args.num_run),
- 		}
-		tools.query.template = querymanagement
-	# dbmsbenchmarker with reporter
-	experiments = benchmarker.benchmarker(
-		result_path=args.result_folder,
-		working=args.working,
-		batch=bBatch,
-		subfolder=subfolder,#args.subfolder,
-		fixedQuery=args.query,
-		fixedConnection=args.connection,
-		fixedAlias=args.connection_alias,
-		rename_connection=rename_connection,
-		rename_alias=rename_alias,
-		#anonymize=args.anonymize,
-		#unanonymize=args.unanonymize,
-		numProcesses=args.numProcesses,
-		seed=args.seed)
-	experiments.getConfig(args.config_folder, args.connection_file, args.query_file)
-	# switch for args.mode
-	if args.mode == 'read':
-		experiments.readBenchmarks()
-	elif args.mode == 'run':
-		if experiments.continuing:
-			#experiments.generateAllParameters()
-			experiments.continueBenchmarks(overwrite = True)
-		else:
-			#experiments.generateAllParameters()
-			experiments.runBenchmarks()
-		print('Experiment {} has been finished'.format(experiments.code))
-	elif args.mode == 'continue':
-		if experiments.continuing:
-			experiments.continueBenchmarks(overwrite = False)
-		else:
-			print("Continue needs result folder")
-	if args.metrics:
-		# collect hardware metrics
-		experiments.reporter.append(benchmarker.reporter.metricer(experiments))
-		experiments.generateReportsAll()
-	if args.metrics_per_stream:
-		# collect hardware metrics
-		experiments.reporter.append(benchmarker.reporter.metricer(experiments, per_stream=True))
-		experiments.generateReportsAll()
-	if args.generate_evaluation == 'yes':
-		# generate evaluation cube
-		experiments.overwrite = True
-		evaluator.evaluator(experiments, load=False, force=True)
+    # argparse
+    parser = argparse.ArgumentParser(description='A benchmark tool for RDBMS. It connects to a given list of RDBMS via JDBC and runs a given list benchmark queries. Optionally some reports are generated.')
+    parser.add_argument('mode', help='run benchmarks and save results, or just read benchmark results from folder, or continue with missing benchmarks only', choices=['run', 'read', 'continue'])
+    parser.add_argument('-d', '--debug', help='dump debug informations', action='store_true')
+    parser.add_argument('-b', '--batch', help='batch mode (more protocol-like output), automatically on for debug mode', action='store_true')
+    parser.add_argument('-qf', '--query-file', help='name of query config file', default='queries.config')
+    parser.add_argument('-cf', '--connection-file', help='name of connection config file', default='connections.config')
+    parser.add_argument('-q', '--query', help='number of query to benchmark', default=None)
+    parser.add_argument('-c', '--connection', help='name of connection to benchmark', default=None)
+    parser.add_argument('-ca', '--connection-alias', help='alias of connection to benchmark', default='')
+    parser.add_argument('-f', '--config-folder', help='folder containing query and connection config files. If set, the names connections.config and queries.config are assumed automatically.', default=None)
+    parser.add_argument('-r', '--result-folder', help='folder for storing benchmark result files, default is given by timestamp', default=None)
+    parser.add_argument('-e', '--generate-evaluation', help='generate new evaluation file', default='no', choices=['no','yes'])
+    parser.add_argument('-w', '--working', help='working per query or connection', default='query', choices=['query','connection'])
+    #parser.add_argument('-a', '--anonymize', help='anonymize all dbms', action='store_true', default=False)
+    #parser.add_argument('-u', '--unanonymize', help='unanonymize some dbms, only sensible in combination with anonymize', nargs='*', default=[])
+    parser.add_argument('-p', '--numProcesses', help='Number of parallel client processes. Global setting, can be overwritten by connection. Default is 1.', default=None)
+    parser.add_argument('-s', '--seed', help='random seed', default=None)
+    parser.add_argument('-cs', '--copy-subfolder', help='copy subfolder of result folder', action='store_true')
+    parser.add_argument('-ms', '--max-subfolders', help='maximum number of subfolders of result folder', default=None)
+    parser.add_argument('-sl', '--sleep', help='sleep SLEEP seconds before going to work', default=0)
+    parser.add_argument('-st', '--start-time', help='sleep until START-TIME before beginning benchmarking', default=None)
+    parser.add_argument('-sf', '--subfolder', help='stores results in a SUBFOLDER of the result folder', default=None)
+    parser.add_argument('-vq', '--verbose-queries', help='print every query that is sent', action='store_true', default=False)
+    parser.add_argument('-vs', '--verbose-statistics', help='print statistics about query that have been sent', action='store_true', default=False)
+    parser.add_argument('-vr', '--verbose-results', help='print result sets of every query that have been sent', action='store_true', default=False)
+    parser.add_argument('-vp', '--verbose-process', help='print result sets of every query that have been sent', action='store_true', default=False)
+    parser.add_argument('-pn', '--num-run', help='Parameter: Number of executions per query', default=0)
+    parser.add_argument('-m', '--metrics', help='collect hardware metrics per query', action='store_true', default=False)
+    parser.add_argument('-mps', '--metrics-per-stream', help='collect hardware metrics per stream', action='store_true', default=False)
+    parser.add_argument('-wli', '--workload-intro', help='meta data: intro text for workload description', default='')
+    parser.add_argument('-wln', '--workload-name', help='meta data: name of workload', default='')
+    #parser.add_argument('-pt', '--timeout', help='Parameter: Timeout in seconds', default=0)
+    logger = logging.getLogger('dbmsbenchmarker')
+    args = parser.parse_args()
+    # evaluate args
+    if args.debug:
+        logging.basicConfig(level=logging.DEBUG)
+        bBatch = True
+    else:
+        logging.basicConfig(level=logging.INFO)
+        bBatch = args.batch
+    # sleep before going to work
+    if int(args.sleep) > 0:
+        logger.debug("Sleeping {} seconds before going to work".format(int(args.sleep)))
+        time.sleep(int(args.sleep))
+    # make a copy of result folder
+    subfolder = args.subfolder
+    rename_connection = ''
+    rename_alias = ''
+    if args.copy_subfolder and len(subfolder) > 0:
+        client = 1
+        while True:
+            if args.max_subfolders is not None and client > int(args.max_subfolders):
+                exit()
+            resultpath = args.result_folder+'/'+subfolder+'-'+str(client)
+            logger.debug("Checking if {} is suitable folder for free job number".format(resultpath))
+            if path.isdir(resultpath):
+                client = client + 1
+                waiting = random.randint(1, 10)
+                logger.debug("Sleeping {} seconds before checking for next free job number".format(waiting))
+                time.sleep(waiting)
+            else:
+                makedirs(resultpath)
+                break
+        subfolder = subfolder+'-'+str(client)
+        rename_connection = args.connection+'-'+str(client)
+        logger.debug("Rename connection {} to {}".format(args.connection, rename_connection))
+        rename_alias = args.connection_alias+'-'+str(client)
+        logger.debug("Rename alias {} to {}".format(args.connection_alias, rename_alias))
+    # sleep before going to work
+    if args.start_time is not None:
+        #logger.debug(args.start_time)
+        now = datetime.utcnow()
+        try:
+            start = datetime.strptime(args.start_time, '%Y-%m-%d %H:%M:%S')
+            if start > now:
+                wait = (start-now).seconds
+                now_string = now.strftime('%Y-%m-%d %H:%M:%S')
+                logger.debug("Sleeping until {} before going to work ({} seconds, it is {} now)".format(args.start_time, wait, now_string))
+                time.sleep(int(wait))
+        except Exception as e:
+            logger.debug("Invalid format: {}".format(args.start_time))
+    # set verbose level
+    if args.verbose_queries:
+        benchmarker.BENCHMARKER_VERBOSE_QUERIES = True
+    if args.verbose_statistics:
+        benchmarker.BENCHMARKER_VERBOSE_STATISTICS = True
+    if args.verbose_results:
+        benchmarker.BENCHMARKER_VERBOSE_RESULTS = True
+    if args.verbose_process:
+        benchmarker.BENCHMARKER_VERBOSE_PROCESS = True
+    # overwrite parameters of workload queries
+    if int(args.num_run) > 0:
+        querymanagement = {
+             'numRun': int(args.num_run),
+         }
+        tools.query.template = querymanagement
+    # dbmsbenchmarker with reporter
+    experiments = benchmarker.benchmarker(
+        result_path=args.result_folder,
+        working=args.working,
+        batch=bBatch,
+        subfolder=subfolder,#args.subfolder,
+        fixedQuery=args.query,
+        fixedConnection=args.connection,
+        fixedAlias=args.connection_alias,
+        rename_connection=rename_connection,
+        rename_alias=rename_alias,
+        #anonymize=args.anonymize,
+        #unanonymize=args.unanonymize,
+        numProcesses=args.numProcesses,
+        seed=args.seed)
+    # overwrite parameters of workload header
+    if len(args.workload_intro):
+        experiments.workload['intro'] = args.workload_intro
+    if len(args.workload_name):
+        experiments.workload['name'] = args.workload_name
+    experiments.getConfig(args.config_folder, args.connection_file, args.query_file)
+    # switch for args.mode
+    if args.mode == 'read':
+        experiments.readBenchmarks()
+    elif args.mode == 'run':
+        if experiments.continuing:
+            #experiments.generateAllParameters()
+            experiments.continueBenchmarks(overwrite = True)
+        else:
+            #experiments.generateAllParameters()
+            experiments.runBenchmarks()
+        print('Experiment {} has been finished'.format(experiments.code))
+    elif args.mode == 'continue':
+        if experiments.continuing:
+            experiments.continueBenchmarks(overwrite = False)
+        else:
+            print("Continue needs result folder")
+    if args.metrics:
+        # collect hardware metrics
+        experiments.reporter.append(benchmarker.reporter.metricer(experiments))
+        experiments.generateReportsAll()
+    if args.metrics_per_stream:
+        # collect hardware metrics
+        experiments.reporter.append(benchmarker.reporter.metricer(experiments, per_stream=True))
+        experiments.generateReportsAll()
+    if args.generate_evaluation == 'yes':
+        # generate evaluation cube
+        experiments.overwrite = True
+        evaluator.evaluator(experiments, load=False, force=True)
```

### Comparing `dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/dashboardcli.py` & `dbmsbenchmarker-0.13.8/dbmsbenchmarker/scripts/dashboardcli.py`

 * *Files identical despite different names*

### Comparing `dbmsbenchmarker-0.13.7/dbmsbenchmarker/tools.py` & `dbmsbenchmarker-0.13.8/dbmsbenchmarker/tools.py`

 * *Files identical despite different names*

### Comparing `dbmsbenchmarker-0.13.7/dbmsbenchmarker.egg-info/PKG-INFO` & `dbmsbenchmarker-0.13.8/dbmsbenchmarker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbmsbenchmarker
-Version: 0.13.7
+Version: 0.13.8
 Summary: DBMS-Benchmarker is a Python-based application-level blackbox benchmark tool for Database Management Systems (DBMS). It connects to a given list of DBMS (via JDBC) and runs a given list of parametrized and randomized (SQL) benchmark queries. Evaluations are available via Python interface, in reports and at an interactive multi-dimensional dashboard.
 Home-page: https://github.com/Beuth-Erdelt/DBMS-Benchmarker
 Author: Patrick Erdelt
 Author-email: perdelt@beuth-hochschule.de
 License: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `dbmsbenchmarker-0.13.7/dbmsbenchmarker.egg-info/SOURCES.txt` & `dbmsbenchmarker-0.13.8/dbmsbenchmarker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbmsbenchmarker-0.13.7/dbmsbenchmarker.egg-info/requires.txt` & `dbmsbenchmarker-0.13.8/dbmsbenchmarker.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 JayDeBeApi>=1.1.1
 matplotlib>=3.1.1
 numpy>=1.22.2
 pandas>=0.25.1
 tabulate>=0.8.2
 tqdm>=4.28.1
-requests>=2.31.0
+requests>=2.32.0
 JPype1>=1.2.0
 scipy>=1.4.1
 colour>=0.1.5
 Brotli>=1.0.7
 certifi>=2023.7.22
 chardet>=3.0.4
 click>=6.7
```

### Comparing `dbmsbenchmarker-0.13.7/setup.py` & `dbmsbenchmarker-0.13.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="dbmsbenchmarker",
-    version="0.13.7",
+    version="0.13.8",
     author="Patrick Erdelt",
     author_email="perdelt@beuth-hochschule.de",
     description="DBMS-Benchmarker is a Python-based application-level blackbox benchmark tool for Database Management Systems (DBMS). It connects to a given list of DBMS (via JDBC) and runs a given list of parametrized and randomized (SQL) benchmark queries. Evaluations are available via Python interface, in reports and at an interactive multi-dimensional dashboard.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Beuth-Erdelt/DBMS-Benchmarker",
     packages=setuptools.find_packages(),
```

