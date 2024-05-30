# Comparing `tmp/archerysec_cli-3.1.8.tar.gz` & `tmp/archerysec_cli-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archerysec_cli-3.1.8.tar", last modified: Thu Sep 30 13:43:04 2021, max compression
+gzip compressed data, was "archerysec_cli-3.1.9.tar", last modified: Thu Feb 10 06:47:59 2022, max compression
```

## Comparing `archerysec_cli-3.1.8.tar` & `archerysec_cli-3.1.9.tar`

### file list

```diff
@@ -1,25 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 13:43:04.370593 archerysec_cli-3.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-30 13:42:55.000000 archerysec_cli-3.1.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)    12328 2021-09-30 13:43:04.370593 archerysec_cli-3.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11652 2021-09-30 13:42:55.000000 archerysec_cli-3.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 13:43:04.370593 archerysec_cli-3.1.8/archerysec_cli/
--rw-r--r--   0 runner    (1001) docker     (121)     1356 2021-09-30 13:42:55.000000 archerysec_cli-3.1.8/archerysec_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 13:43:04.370593 archerysec_cli-3.1.8/archerysec_cli/cli/
--rw-r--r--   0 runner    (1001) docker     (121)      990 2021-09-30 13:42:55.000000 archerysec_cli-3.1.8/archerysec_cli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16824 2021-09-30 13:42:55.000000 archerysec_cli-3.1.8/archerysec_cli/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 13:43:04.370593 archerysec_cli-3.1.8/archerysec_cli/scanners/
--rw-r--r--   0 runner    (1001) docker     (121)      990 2021-09-30 13:42:55.000000 archerysec_cli-3.1.8/archerysec_cli/scanners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5039 2021-09-30 13:42:55.000000 archerysec_cli-3.1.8/archerysec_cli/scanners/scanners.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 13:43:04.370593 archerysec_cli-3.1.8/archerysec_cli/util/
--rw-r--r--   0 runner    (1001) docker     (121)      990 2021-09-30 13:42:55.000000 archerysec_cli-3.1.8/archerysec_cli/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5958 2021-09-30 13:42:55.000000 archerysec_cli-3.1.8/archerysec_cli/util/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     2926 2021-09-30 13:42:55.000000 archerysec_cli-3.1.8/archerysec_cli/util/check.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-30 13:43:04.370593 archerysec_cli-3.1.8/archerysec_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12328 2021-09-30 13:43:04.000000 archerysec_cli-3.1.8/archerysec_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      505 2021-09-30 13:43:04.000000 archerysec_cli-3.1.8/archerysec_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-30 13:43:04.000000 archerysec_cli-3.1.8/archerysec_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       64 2021-09-30 13:43:04.000000 archerysec_cli-3.1.8/archerysec_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      181 2021-09-30 13:43:04.000000 archerysec_cli-3.1.8/archerysec_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-09-30 13:43:04.000000 archerysec_cli-3.1.8/archerysec_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-30 13:43:04.370593 archerysec_cli-3.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2479 2021-09-30 13:42:55.000000 archerysec_cli-3.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-10 06:47:59.442667 archerysec_cli-3.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-10 06:47:49.000000 archerysec_cli-3.1.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    12328 2022-02-10 06:47:59.442667 archerysec_cli-3.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    11652 2022-02-10 06:47:49.000000 archerysec_cli-3.1.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-10 06:47:59.438667 archerysec_cli-3.1.9/archerysec_cli/
+-rw-r--r--   0 runner    (1001) docker     (121)     1356 2022-02-10 06:47:49.000000 archerysec_cli-3.1.9/archerysec_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-10 06:47:59.442667 archerysec_cli-3.1.9/archerysec_cli/cli/
+-rw-r--r--   0 runner    (1001) docker     (121)      990 2022-02-10 06:47:49.000000 archerysec_cli-3.1.9/archerysec_cli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16906 2022-02-10 06:47:49.000000 archerysec_cli-3.1.9/archerysec_cli/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-10 06:47:59.442667 archerysec_cli-3.1.9/archerysec_cli/formatters/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-10 06:47:49.000000 archerysec_cli-3.1.9/archerysec_cli/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      548 2022-02-10 06:47:49.000000 archerysec_cli-3.1.9/archerysec_cli/formatters/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)      325 2022-02-10 06:47:49.000000 archerysec_cli-3.1.9/archerysec_cli/formatters/json.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-10 06:47:59.442667 archerysec_cli-3.1.9/archerysec_cli/scanners/
+-rw-r--r--   0 runner    (1001) docker     (121)      990 2022-02-10 06:47:49.000000 archerysec_cli-3.1.9/archerysec_cli/scanners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4913 2022-02-10 06:47:49.000000 archerysec_cli-3.1.9/archerysec_cli/scanners/scanners.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-10 06:47:59.442667 archerysec_cli-3.1.9/archerysec_cli/util/
+-rw-r--r--   0 runner    (1001) docker     (121)      990 2022-02-10 06:47:49.000000 archerysec_cli-3.1.9/archerysec_cli/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5958 2022-02-10 06:47:49.000000 archerysec_cli-3.1.9/archerysec_cli/util/api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2926 2022-02-10 06:47:49.000000 archerysec_cli-3.1.9/archerysec_cli/util/check.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-10 06:47:59.442667 archerysec_cli-3.1.9/archerysec_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    12328 2022-02-10 06:47:59.000000 archerysec_cli-3.1.9/archerysec_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      610 2022-02-10 06:47:59.000000 archerysec_cli-3.1.9/archerysec_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-10 06:47:59.000000 archerysec_cli-3.1.9/archerysec_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-10 06:47:59.000000 archerysec_cli-3.1.9/archerysec_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      181 2022-02-10 06:47:59.000000 archerysec_cli-3.1.9/archerysec_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-02-10 06:47:59.000000 archerysec_cli-3.1.9/archerysec_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-10 06:47:59.442667 archerysec_cli-3.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2479 2022-02-10 06:47:49.000000 archerysec_cli-3.1.9/setup.py
```

### Comparing `archerysec_cli-3.1.8/PKG-INFO` & `archerysec_cli-3.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archerysec_cli
-Version: 3.1.8
+Version: 3.1.9
 Summary: A commandline tool that wraps the Archerysec REST API for controlling Archery and executing quick, targeted scans.
 Home-page: https://github.com/archerysec/archerysec-cli.git
 Author: Anand Tiwari
 Author-email:  
 License:  
 Platform: UNKNOWN
 Classifier: Topic :: Security
```

### Comparing `archerysec_cli-3.1.8/README.rst` & `archerysec_cli-3.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `archerysec_cli-3.1.8/archerysec_cli/__init__.py` & `archerysec_cli-3.1.9/archerysec_cli/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 """
 from datetime import datetime
 
 
 __title__ = 'archerysec-cli'
 __authors__ = 'Anand Tiwari'
 __copyright__ = f'Copyright {datetime.now().year} Anand Tiwari, ArcherySec'
-__version__ = '3.1.8'
+__version__ = '3.1.9'
 __version_info__ = tuple(int(i) for i in __version__.split('.'))
 __all__ = [
     '__title__',
     '__authors__',
     '__copyright__',
     '__version__',
     '__version_info__',
```

### Comparing `archerysec_cli-3.1.8/archerysec_cli/cli/__init__.py` & `archerysec_cli-3.1.9/archerysec_cli/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `archerysec_cli-3.1.8/archerysec_cli/cli/cli.py` & `archerysec_cli-3.1.9/archerysec_cli/cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,32 +21,37 @@
 import sys
 
 import click
 import json
 import yaml
 from yaml import safe_load
 
+from archerysec_cli import __version__
 from archerysec_cli.scanners.scanners import ScannersRunner
 from archerysec_cli.util import check
 from archerysec_cli.util.api import API
+from archerysec_cli.formatters import (
+    cli,
+    json
+)
 
 data = """
 
                     _                      _____           
      /\            | |                    / ____|          
     /  \   _ __ ___| |__   ___ _ __ _   _| (___   ___  ___ 
    / /\ \ | '__/ __| '_ \ / _ \ '__| | | |\___ \ / _ \/ __|
   / ____ \| | | (__| | | |  __/ |  | |_| |____) |  __/ (__ 
  /_/    \_\_|  \___|_| |_|\___|_|   \__, |_____/ \___|\___|
                                      __/ |                 
                                     |___/                  
-               
- Copyright (C) 2021 ArcherySec CLI v2.0.1
 """
 print(data)
+print(cli.print_tool_info(__version__))
+
 
 
 @click.command()
 @click.option("--host", "-h", "host", help="Provide ArcherySec End Point Address.")
 @click.option("--token", "-t", "token", help="Provide Auth token from ArcherySec.")
 @click.option('--path', '-p', "path", help='Report File input')
 @click.option('--file-type', "filetype", help='File type')
@@ -91,14 +96,15 @@
 @click.option('--zap-full-scan', "zapfullscan", help="Run ZAP Full Scan", is_flag=True)
 @click.option('--findsecbugs-scan', "findsecbugs", help="Run FindSecBugs Scan", is_flag=True)
 @click.option('--dependency-check', "dependencycheck", help="Run dependency-check Scan", is_flag=True)
 @click.option('--project_name', "projectname", help="Create New Project")
 @click.option('--project_disc', "projectdisc", help="Create New Project")
 @click.option('--code_path', "code_path", help="Path of the source code")
 @click.option('--report_path', "reportpath", help="Path of the Report")
+
 def scan_action(host, token, filetype, target, scanner, projectid, path, upload, projectcreate, projectname,
                 projectdisc, bandit, reportpath, code_path, cicd_id, dependencycheck, threshold,
                 zapbaselinescan, zapfullscan, findsecbugs):
     if upload:
         upload_report(
             host=host,
             token=token,
@@ -166,15 +172,14 @@
             token=token,
             project=projectid,
             findsecbugs='findsecbugs',
             cicd_id=cicd_id,
             reportpath=reportpath
         )
 
-
 def get_cicd_policies(host, token, project, scanner, target, cicd_id):
     archerysec = API(
         host=host, project_id=project, scanner=scanner, target=target, token=token
     )
     cicd_policies = archerysec.get_cicd_policies(cicd_id=cicd_id).data
     return cicd_policies
```

### Comparing `archerysec_cli-3.1.8/archerysec_cli/scanners/__init__.py` & `archerysec_cli-3.1.9/archerysec_cli/scanners/__init__.py`

 * *Files identical despite different names*

### Comparing `archerysec_cli-3.1.8/archerysec_cli/scanners/scanners.py` & `archerysec_cli-3.1.9/archerysec_cli/scanners/scanners.py`

 * *Files 15% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 
     def bandit_scan(self):
         print("Scan Running")
         client = docker.from_env()
         d = client.containers.run(
             "archerysec/bandit:latest",
             volumes={
-                self.pwd: {"bind": "/src", "mode": "rw"},
-                self.report_pwd: {"bind": "/report", "mode": "rw"},
+                self.pwd: {"bind": "/src"},
+                self.report_pwd: {"bind": "/report"},
             },
             detach=True,
         )
         c_id = d.id
         container = client.containers.get(c_id)
         status = container.status
         while status == "running":
@@ -51,17 +51,17 @@
 
     def dependency_check_scan(self, data):
         print("Scan Running")
         client = docker.from_env()
         d = client.containers.run(
             "archerysec/dependency-check:latest",
             volumes={
-                self.pwd: {"bind": "/src", "mode": "rw"},
-                self.report_pwd: {"bind": "/report", "mode": "rw"},
-                data: {"bind": "/usr/share/dependency-check/data", "mode": "rw"},
+                self.pwd: {"bind": "/src"},
+                self.report_pwd: {"bind": "/report"},
+                data: {"bind": "/usr/share/dependency-check/data"},
             },
             command='--scan /src --format "ALL" --project "dependency-check scan: %s" --out /report' % self.pwd,
             detach=True,
         )
         c_id = d.id
         container = client.containers.get(c_id)
         status = container.status
@@ -75,15 +75,15 @@
 
     def owasp_zap_baseline_scan(self, target):
         print("Scan Running")
         client = docker.from_env()
         d = client.containers.run(
             "archerysec/owasp-zap:latest",
             volumes={
-                self.report_pwd: {"bind": "/zap/wrk", "mode": "rw"},
+                self.report_pwd: {"bind": "/zap/wrk"},
             },
             command='zap-baseline.py -t %s -x archerysec-owasp-zap-base-line-report.xml' % target,
             detach=True,
 
         )
         c_id = d.id
         container = client.containers.get(c_id)
@@ -98,15 +98,15 @@
 
     def owasp_zap_full_scan(self, target):
         print("Scan Running")
         client = docker.from_env()
         d = client.containers.run(
             "archerysec/owasp-zap:latest",
             volumes={
-                self.report_pwd: {"bind": "/zap/wrk", "mode": "rw"},
+                self.report_pwd: {"bind": "/zap/wrk"},
             },
             command='zap-full-scan.py -t %s -x archerysec-owasp-zap-full-scan-report.xml' % target,
             detach=True,
         )
         c_id = d.id
         container = client.containers.get(c_id)
         status = container.status
@@ -120,16 +120,16 @@
 
     def findsecbugs_scan(self):
         print("Scan Running")
         client = docker.from_env()
         d = client.containers.run(
             "archerysec/findsecbugs:latest",
             volumes={
-                self.pwd: {"bind": "/src", "mode": "rw"},
-                self.report_pwd: {"bind": "/report", "mode": "rw"},
+                self.pwd: {"bind": "/src"},
+                self.report_pwd: {"bind": "/report"},
             },
             detach=True,
         )
         c_id = d.id
         container = client.containers.get(c_id)
         status = container.status
         while status == "running":
```

### Comparing `archerysec_cli-3.1.8/archerysec_cli/util/__init__.py` & `archerysec_cli-3.1.9/archerysec_cli/util/__init__.py`

 * *Files identical despite different names*

### Comparing `archerysec_cli-3.1.8/archerysec_cli/util/api.py` & `archerysec_cli-3.1.9/archerysec_cli/util/api.py`

 * *Files identical despite different names*

### Comparing `archerysec_cli-3.1.8/archerysec_cli/util/check.py` & `archerysec_cli-3.1.9/archerysec_cli/util/check.py`

 * *Files identical despite different names*

### Comparing `archerysec_cli-3.1.8/archerysec_cli.egg-info/PKG-INFO` & `archerysec_cli-3.1.9/archerysec_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archerysec-cli
-Version: 3.1.8
+Version: 3.1.9
 Summary: A commandline tool that wraps the Archerysec REST API for controlling Archery and executing quick, targeted scans.
 Home-page: https://github.com/archerysec/archerysec-cli.git
 Author: Anand Tiwari
 Author-email:  
 License:  
 Platform: UNKNOWN
 Classifier: Topic :: Security
```

### Comparing `archerysec_cli-3.1.8/setup.py` & `archerysec_cli-3.1.9/setup.py`

 * *Files identical despite different names*

