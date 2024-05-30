# Comparing `tmp/robotframework_ghareports-0.1.0-py3-none-any.whl.zip` & `tmp/robotframework_ghareports-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 17205 bytes, number of entries: 7
--rw-r--r--  2.0 unx     6378 b- defN 16-Jan-01 00:00 GHAReports.py
--rw-r--r--  2.0 unx        0 b- defN 16-Jan-01 00:00 __init__.py
--rw-r--r--  2.0 unx     3080 b- defN 16-Jan-01 00:00 mdgen.py
--rw-r--r--  2.0 unx     2218 b- defN 16-Jan-01 00:00 robotframework_ghareports-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       90 b- defN 16-Jan-01 00:00 robotframework_ghareports-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx    35149 b- defN 16-Jan-01 00:00 robotframework_ghareports-0.1.0.dist-info/licenses/LICENSE
-?rw-------  2.0 unx      576 b- defN 16-Jan-01 00:00 robotframework_ghareports-0.1.0.dist-info/RECORD
-7 files, 47491 bytes uncompressed, 16181 bytes compressed:  65.9%
+Zip file size: 19038 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     7105 b- defN 16-Jan-01 00:00 GHAReports/GHAReports.py
+-rw-r--r--  2.0 unx       61 b- defN 16-Jan-01 00:00 GHAReports/__init__.py
+-rw-r--r--  2.0 unx     3658 b- defN 16-Jan-01 00:00 GHAReports/foo
+-rw-r--r--  2.0 unx     3156 b- defN 16-Jan-01 00:00 GHAReports/mdgen.py
+-rw-r--r--  2.0 unx     2607 b- defN 16-Jan-01 00:00 robotframework_ghareports-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       90 b- defN 16-Jan-01 00:00 robotframework_ghareports-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx    35149 b- defN 16-Jan-01 00:00 robotframework_ghareports-0.2.0.dist-info/licenses/LICENSE
+?rw-------  2.0 unx      681 b- defN 16-Jan-01 00:00 robotframework_ghareports-0.2.0.dist-info/RECORD
+8 files, 52507 bytes uncompressed, 17844 bytes compressed:  66.0%
```

## zipnote {}

```diff
@@ -1,22 +1,25 @@
-Filename: GHAReports.py
+Filename: GHAReports/GHAReports.py
 Comment: 
 
-Filename: __init__.py
+Filename: GHAReports/__init__.py
 Comment: 
 
-Filename: mdgen.py
+Filename: GHAReports/foo
 Comment: 
 
-Filename: robotframework_ghareports-0.1.0.dist-info/METADATA
+Filename: GHAReports/mdgen.py
 Comment: 
 
-Filename: robotframework_ghareports-0.1.0.dist-info/WHEEL
+Filename: robotframework_ghareports-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: robotframework_ghareports-0.1.0.dist-info/licenses/LICENSE
+Filename: robotframework_ghareports-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: robotframework_ghareports-0.1.0.dist-info/RECORD
+Filename: robotframework_ghareports-0.2.0.dist-info/licenses/LICENSE
+Comment: 
+
+Filename: robotframework_ghareports-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `GHAReports.py` & `GHAReports/GHAReports.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 import os
 import wrapt
 from pathlib import Path
 import sys
-from mdgen import MDGen, MD_STATUSICONS
+from .mdgen import MDGen, MD_STATUSICONS
 from time import time_ns
 
 
 @wrapt.decorator
 def skip_if_not_initialized(wrapped, instance, args, kwargs):
     if not instance.initialized:
         return
@@ -21,32 +21,40 @@
 
 class GHAReports(object):
     ROBOT_LISTENER_API_VERSION = 2
     _suites = {}
     _current_case = None
     _current_suite = None
     _testcases = {}
+    _output = None
+    _report = None
     initialized = False
     summary = None
     start_ts = None
     stop_ts = None
 
     # suite attributes: name test_cases  hostname id package timestamp properties file log url stdout stderr
     # case attributes: name classname elapsed_sec stdout stderr assertions timestamp status category file line log group url
 
-    def __init__(self, cell_width_in_characters=0):
+    def __init__(self, cell_width_in_characters=0, report_file=None):
         self._output = os.environ.get("GITHUB_STEP_SUMMARY", None)
         self.cell_width_in_characters = cell_width_in_characters
 
         if self._output:
             self.initialized = True
             self._output = Path(self._output).resolve()
             print(f"GHAReports detected Github environment. Generating Step Summary: {str(self._output)}", file=sys.stderr)
         else:
             print("GHAReports did not detect Github environment.", file=sys.stderr)
+
+        if report_file:
+            self.initialized = True
+            self._report = Path(report_file).resolve()
+            print(f"GHAReports is generating extra report file @ {self._report}", file=sys.stderr)
+
         self.summary = MDGen()
 
     @skip_if_not_initialized
     def start_suite(self, name, attrs):
         if not self.start_ts:
             self.start_ts = getmsts()
 
@@ -114,16 +122,23 @@
                     case "FAIL":
                         failed.append([testcase["name"], testcase["message"], duration, testcase["suite"]])
                         stats["fail"] += 1
                     case "SKIP":
                         skipped.append([testcase["name"], testcase["message"], duration, testcase["suite"]])
                         stats["skip"] += 1
 
-        stats["passrate"] = round(stats["pass"] / stats["total"] * 100, 2)
-        total_duration = round((self.stop_ts - self.start_ts) / 1000, 1)
+        try:
+            stats["passrate"] = round(stats["pass"] / stats["total"] * 100, 2)
+        except ZeroDivisionError:
+            stats["passrate"] = 0
+
+        if None in [self.stop_ts, self.start_ts]:
+            total_duration = 0
+        else:
+            total_duration = round((self.stop_ts - self.start_ts) / 1000, 1)
         return (
             [[stats["pass"], stats["fail"], stats["skip"], stats["total"], stats["passrate"], total_duration]],
             passed,
             failed,
             skipped,
         )
 
@@ -148,15 +163,18 @@
             alignments=["center", "center", "center", "center", "right", "right"],
             cell_width_in_characters=self.cell_width_in_characters,
         )
 
         self.summary.header(f"{MD_STATUSICONS['PASS']} Passing tests")
         test_headers = ["Testcase", "Duration (sec)", "Suite"]
         self.summary.table(
-            test_headers, passed, alignments=["left", "right", "left"], cell_width_in_characters=self.cell_width_in_characters
+            test_headers,
+            passed,
+            alignments=["left", "right", "left"],
+            cell_width_in_characters=self.cell_width_in_characters,
         )
 
         self.summary.header(f"{MD_STATUSICONS['FAIL']} Failing tests")
         test_headers = ["Testcase", "Message", "Duration (sec)", "Suite"]
         self.summary.table(
             test_headers,
             failed,
@@ -169,9 +187,13 @@
         self.summary.table(
             test_headers,
             skipped,
             alignments=["left", "left", "right", "left"],
             cell_width_in_characters=self.cell_width_in_characters,
         )
 
-        with open(self._output, "w", encoding="utf-8") as f:
-            f.write(self.summary.getvalue())
+        buffer = self.summary.getvalue()
+        for filename in filter(bool, [self._output, self._report]):
+            try:
+                Path(filename).write_text(buffer, encoding="utf-8")
+            except Exception as e:
+                print(f"GHAReports encountered an errow while writing to {filename}:\n{e}", file=sys.stderr)
```

## Comparing `mdgen.py` & `GHAReports/mdgen.py`

 * *Files 10% similar despite different names*

```diff
@@ -60,20 +60,22 @@
         else:
             self.write("| ")
             self.write(" | ".join("-" * len(headers)))
             self.write(f" |{linesep}")
 
         for row in rows:
             self.write("| ")
-            if cell_width_in_characters != 0:
-                self.write(" | ".join("<br/>".join(wrap(str(cell), cell_width_in_characters)) for cell in row))
-            else:
-                self.write(" | ".join(str(cell) for cell in row))
-            self.write(f" |{linesep}")
-
+            for cell in row:
+                cell = str(cell)
+                if "\n" in cell:
+                    cell = "<br/>".join(cell.split("\n"))
+                if cell_width_in_characters != 0:
+                    cell = "<br/>".join(wrap(cell, cell_width_in_characters))
+                self.write(f"{cell} |")
+            self.write(f"{linesep}")
         self.write(linesep)
 
     def link(self, text, url):
         self.write(f"[{text}]({url}){linesep}")
 
 
 def main():
```

## Comparing `robotframework_ghareports-0.1.0.dist-info/METADATA` & `robotframework_ghareports-0.2.0.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: robotframework-ghareports
-Version: 0.1.0
+Version: 0.2.0
 Summary: Simple github action summary report for robotframework
 Author-Email: Jani Mikkonen <jani.mikkonen@gmail.com>
 License: GPLV3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
 Project-URL: Homepage, https://github.com/rasjani/robotframework-ghareports
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Requires-Dist: robotframework>=4.0.0
 Requires-Dist: wrapt
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: python-language-server[all]; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: invoke; extra == "dev"
 Requires-Dist: pdm; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: build; extra == "dev"
 Provides-Extra: dev
 Description-Content-Type: text/markdown
 
 robotframework-ghareports
 =========================
 
 
@@ -40,26 +41,37 @@
 activated when RF is executed, it checks if environment variable GITHUB_STEP_SUMMARY exists and if it does, it exposes test results
 to a PR - example output looks something like [this](https://github.com/rasjani/robotframework-ghareports/blob/main/example_step_summary.md)
 
 ## Usage
 
 Install:
 
-```
+```shell
 python -mpip install robotframework-ghareports
 ```
 
 Usage:
 
-```
+```shell
 robot --listener GHAReports .
 ```
 
 If you want to limit the width of the tables in the summary, you can provide an argument to the listener like this:
 
 
-```
+```shell
 robot --listener GHAReports:35 .
 ```
 
 This will split each test case name at every 35 characters into a new line.
 
+And if you want to generate the summary even  if a) you are not running in Github *or* you want to generate extra summary file independent of
+Github actions, pass report_file argument to the listener like this:
+
+```shell
+robot --listener GHAReports:report_file=extra_summary.md
+```
+or
+
+```shell
+robot --listener GHAReports:34:extra_summary.md
+```
```

## Comparing `robotframework_ghareports-0.1.0.dist-info/licenses/LICENSE` & `robotframework_ghareports-0.2.0.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

