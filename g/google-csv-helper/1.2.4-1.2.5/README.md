# Comparing `tmp/google_csv_helper-1.2.4.tar.gz` & `tmp/google_csv_helper-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_csv_helper-1.2.4.tar", last modified: Wed May 29 15:19:14 2024, max compression
+gzip compressed data, was "google_csv_helper-1.2.5.tar", last modified: Thu May 30 16:43:27 2024, max compression
```

## Comparing `google_csv_helper-1.2.4.tar` & `google_csv_helper-1.2.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:19:14.601137 google_csv_helper-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-29 15:19:03.000000 google_csv_helper-1.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-05-29 15:19:14.601137 google_csv_helper-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-05-29 15:19:03.000000 google_csv_helper-1.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:19:14.597137 google_csv_helper-1.2.4/google_csv_helper/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-29 15:19:03.000000 google_csv_helper-1.2.4/google_csv_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-05-29 15:19:03.000000 google_csv_helper-1.2.4/google_csv_helper/adsense_csv_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    11673 2024-05-29 15:19:03.000000 google_csv_helper-1.2.4/google_csv_helper/cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-05-29 15:19:03.000000 google_csv_helper-1.2.4/google_csv_helper/csv_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    16332 2024-05-29 15:19:03.000000 google_csv_helper-1.2.4/google_csv_helper/csv_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-05-29 15:19:03.000000 google_csv_helper-1.2.4/google_csv_helper/ga3_csv_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-05-29 15:19:03.000000 google_csv_helper-1.2.4/google_csv_helper/ga4_csv_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    19458 2024-05-29 15:19:03.000000 google_csv_helper-1.2.4/google_csv_helper/google_common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:19:14.601137 google_csv_helper-1.2.4/google_csv_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-05-29 15:19:14.000000 google_csv_helper-1.2.4/google_csv_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 15:19:14.000000 google_csv_helper-1.2.4/google_csv_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 15:19:14.000000 google_csv_helper-1.2.4/google_csv_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-29 15:19:14.000000 google_csv_helper-1.2.4/google_csv_helper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-29 15:19:14.000000 google_csv_helper-1.2.4/google_csv_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-29 15:19:14.000000 google_csv_helper-1.2.4/google_csv_helper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 15:19:14.601137 google_csv_helper-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-29 15:19:03.000000 google_csv_helper-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:43:27.165145 google_csv_helper-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-30 16:43:22.000000 google_csv_helper-1.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-05-30 16:43:27.165145 google_csv_helper-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-05-30 16:43:22.000000 google_csv_helper-1.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:43:27.161145 google_csv_helper-1.2.5/google_csv_helper/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-30 16:43:22.000000 google_csv_helper-1.2.5/google_csv_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12538 2024-05-30 16:43:22.000000 google_csv_helper-1.2.5/google_csv_helper/adsense_csv_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12082 2024-05-30 16:43:22.000000 google_csv_helper-1.2.5/google_csv_helper/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-05-30 16:43:22.000000 google_csv_helper-1.2.5/google_csv_helper/csv_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16332 2024-05-30 16:43:22.000000 google_csv_helper-1.2.5/google_csv_helper/csv_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-05-30 16:43:22.000000 google_csv_helper-1.2.5/google_csv_helper/ga3_csv_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-05-30 16:43:22.000000 google_csv_helper-1.2.5/google_csv_helper/ga4_csv_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19458 2024-05-30 16:43:22.000000 google_csv_helper-1.2.5/google_csv_helper/google_common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:43:27.161145 google_csv_helper-1.2.5/google_csv_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-05-30 16:43:27.000000 google_csv_helper-1.2.5/google_csv_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-30 16:43:27.000000 google_csv_helper-1.2.5/google_csv_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 16:43:27.000000 google_csv_helper-1.2.5/google_csv_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-30 16:43:27.000000 google_csv_helper-1.2.5/google_csv_helper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-30 16:43:27.000000 google_csv_helper-1.2.5/google_csv_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 16:43:27.000000 google_csv_helper-1.2.5/google_csv_helper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 16:43:27.165145 google_csv_helper-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-30 16:43:22.000000 google_csv_helper-1.2.5/setup.py
```

### Comparing `google_csv_helper-1.2.4/LICENSE` & `google_csv_helper-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `google_csv_helper-1.2.4/PKG-INFO` & `google_csv_helper-1.2.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: google-csv-helper
-Version: 1.2.4
-Summary: A simple tool that takes CSV reports from Google Adsense, Google Admob, and Google Analytics and outputs them in JSON / Pandas.DataFrame format.
-Home-page: https://github.com/changyy/google-csv-helper
-Download-URL: https://pypi.org/project/google-csv-helper/
-Author: Yuan-Yi Chang
-Author-email: <changyy.csie@gmail.com>
-Keywords: python,google,csv,adsense,admob,report
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: MacOS :: MacOS X
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: google-api-python-client==2.114.0
-Requires-Dist: google-auth-oauthlib==1.2.0
-Requires-Dist: numpy==1.26.3
-Requires-Dist: pandas==2.1.4
-Requires-Dist: asciichartpy==1.5.25
-
 # google-csv-helper
 
 [![PyPI](https://img.shields.io/pypi/v/google-csv-helper.svg)](https://pypi.org/project/google-csv-helper/)
 
 A simple tool for parsing google csv files.
 
 # Installation
@@ -99,66 +79,116 @@
 | -- | --: | --: | --: | --: | --: 
 | Admob Global | 1,234.56 | 123.45 (-12.34%) | 0.001 (-1.23%) | 234.56 [06/02 Fri] | 456.78 [06/01 Thu] 
 | Adsense Global | 1,234.56 | 123.45 (-12.34%) | 0.1234 (-2.34%) | 123.45 [06/02 Fri] | 345.67 [06/01 Thu] 
 | Adsense China |  1,234.56 | 123.45 (-12.34%) | 0.2345 (2.34%) | 123.45 [06/02 Fri] | 345.67 `[06/01 Thu] 
 | Total | 1,234.56 | 456.78 | | | 
 ```
 
+---
+
+```
+% google-csv-helper --output markdown --output-chart-columns 'Estimated earnings (USD)' csv 
+```
+
+## Current:
+### Date Range: 2023-06-01 ~ 2023-06-04
+#### compare: 2023-05-01 ~ 2023-05-31
+| Item | Cumulative Revenue | Average Daily Revenue | Average CPC | Min Daily Revenue | Max Daily Revenue 
+| -- | --: | --: | --: | --: | --: 
+| Admob Global | 1,234.56 | 123.45 (-12.34%) | 0.001 (-1.23%) | 234.56 [06/02 Fri] | 456.78 [06/01 Thu] 
+| Adsense Global | 1,234.56 | 123.45 (-12.34%) | 0.1234 (-2.34%) | 123.45 [06/02 Fri] | 345.67 [06/01 Thu] 
+| Adsense China |  1,234.56 | 123.45 (-12.34%) | 0.2345 (2.34%) | 123.45 [06/02 Fri] | 345.67 `[06/01 Thu] 
+| Total | 1,234.56 | 456.78 | | | 
+#### ref
+##### Sum of (Admob Global, Adsense Global, Adsense China) - Cumulative Average of 'Estimated earnings (USD)' Chart:
+```
+ 867.61  ┤
+ 846.52  ┤                          ╭──
+ 825.44  ┼╮                        ╭╯
+ 804.36  ┤│                      ╭─╯
+ 783.27  ┤│                     ╭╯
+ 762.19  ┤│                   ╭─╯
+ 741.11  ┤│ ╭╮ ╭╮            ╭╯
+ 720.02  ┤│╭╯╰─╯╰╮           │
+ 698.94  ┤╰╯     ╰─╮         │
+ 677.86  ┤         ╰╮       ╭╯
+ 656.77  ┤          ╰───╮   │
+ 635.69  ┤              ╰───╯
+```
+
+---
+
 ```
-% google-csv-helper --output markdown --output-chart 'Estimated earnings (USD)' csv 
+% google-csv-helper --output-chart-columns 'Estimated earnings (USD)' --output-chart-detailed-columns csv
 ```
 
 ## Current:
 ### Date Range: 2023-06-01 ~ 2023-06-04
 #### compare: 2023-05-01 ~ 2023-05-31
 | Item | Cumulative Revenue | Average Daily Revenue | Average CPC | Min Daily Revenue | Max Daily Revenue 
 | -- | --: | --: | --: | --: | --: 
 | Admob Global | 1,234.56 | 123.45 (-12.34%) | 0.001 (-1.23%) | 234.56 [06/02 Fri] | 456.78 [06/01 Thu] 
 | Adsense Global | 1,234.56 | 123.45 (-12.34%) | 0.1234 (-2.34%) | 123.45 [06/02 Fri] | 345.67 [06/01 Thu] 
 | Adsense China |  1,234.56 | 123.45 (-12.34%) | 0.2345 (2.34%) | 123.45 [06/02 Fri] | 345.67 `[06/01 Thu] 
 | Total | 1,234.56 | 456.78 | | | 
 #### ref
-##### Admob Global - Cumulative Average of 'Estimated earnings (USD)' Chart:
+##### Sum of (Admob Global, Adsense Global, Adsense China) - Cumulative Average of 'Estimated earnings (USD)' Chart:
+```
+ 867.61  ┤
+ 846.52  ┤                          ╭──
+ 825.44  ┼╮                        ╭╯
+ 804.36  ┤│                      ╭─╯
+ 783.27  ┤│                     ╭╯
+ 762.19  ┤│                   ╭─╯
+ 741.11  ┤│ ╭╮ ╭╮            ╭╯
+ 720.02  ┤│╭╯╰─╯╰╮           │
+ 698.94  ┤╰╯     ╰─╮         │
+ 677.86  ┤         ╰╮       ╭╯
+ 656.77  ┤          ╰───╮   │
+ 635.69  ┤              ╰───╯
+```
+###### Admob Global - Cumulative Average of 'Estimated earnings (USD)' Chart:
 ```
   297.11  ┼╮
   294.28  ┤│     ╭╮
   291.46  ┤│    ╭╯╰─╮
   288.64  ┤│    │   ╰╮
   285.81  ┤│    │    ╰╮╭╮
   282.99  ┤│    │     ╰╯╰╮
   280.17  ┤│    │        ╰╮
   277.35  ┤│   ╭╯         ╰╮
   274.52  ┤│   │           ╰╮ ╭─╮
   271.70  ┤╰╮  │            ╰─╯ ╰─╮  ╭──
   268.88  ┤ ╰──╯                  ╰──╯
   266.06  ┤
 ```
-##### Adsense Global - Cumulative Average of 'Estimated earnings (USD)' Chart:
+###### Adsense Global - Cumulative Average of 'Estimated earnings (USD)' Chart:
 ```
   495.71  ┤
   473.65  ┤                          ╭──
   451.59  ┤                         ╭╯
   429.53  ┼╮                       ╭╯
   407.46  ┤│                     ╭─╯
   385.40  ┤│                    ╭╯
   363.34  ┤│╭─╮                ╭╯
   341.28  ┤╰╯ ╰╮              ╭╯
   319.22  ┤    ╰──╮           │
   297.16  ┤       ╰╮         ╭╯
   275.10  ┤        ╰─╮      ╭╯
   253.04  ┤          ╰──────╯
 ```
-##### Adsense China - Cumulative Average of 'Estimated earnings (USD)' Chart:
+###### Adsense China - Cumulative Average of 'Estimated earnings (USD)' Chart:
 ```
   211.76  ┤
   209.91  ┤     ╭──╮
   208.06  ┤     │  ╰╮
   206.20  ┤     │   ╰╮ ╭─╮
   204.35  ┤     │    ╰─╯ ╰╮  ╭──╮
   202.50  ┤    ╭╯         ╰──╯  ╰─╮
   200.65  ┼╮  ╭╯                  ╰────╮
   198.80  ┤│  │                        ╰
   196.95  ┤│  │
   195.10  ┤│ ╭╯
   193.25  ┤│ │
   191.40  ┤╰─╯
 ```
+
```

### Comparing `google_csv_helper-1.2.4/google_csv_helper/adsense_csv_helper.py` & `google_csv_helper-1.2.5/google_csv_helper/adsense_csv_helper.py`

 * *Files 14% similar despite different names*

```diff
@@ -165,36 +165,72 @@
 
         #charts = {
         #    'config': {'height': 10},
         #    'columns': {
         #        'Estimated earnings (USD)': 'Estimated earnings (USD)',
         #        'CPC (USD)': 'CPC (USD)',
         #    }, 'debug': {
-        #        'showColumns': False
+        #        'showCumulativeAverageChartColumnCandidates': False,
+        #        'showEachCumulativeAverageColumnChart': False,
         #    }
         #}
-        if 'config' in charts and 'columns' in charts and len(charts['columns']) > 0:
+        if 'config' in charts and 'columns' in charts:
             output.append("#### ref")
             chartsConfig = charts['config']
             chartsOutput = charts['columns']
+
+            if 'showCumulativeAverageChartColumnCandidates' in charts['debug'] and charts['debug']['showCumulativeAverageChartColumnCandidates']:
+                for k, v in data['output']['raw'].items(): 
+                    if len(v) == 0 or not isinstance(v[0], pandas.DataFrame):
+                        continue
+                    selectedDataFrame = v[0]
+                    print(f"[INFO] {k} CumulativeAverageChart Column Candidates: {selectedDataFrame.columns.to_list()}")
+
             for selectedColumn, outputColumn in chartsOutput.items():
+                sumOfTargetColumn = {}
+                moreDetails = []
                 for k, v in data['output']['raw'].items():
                     if len(v) == 0 or not isinstance(v[0], pandas.DataFrame):
                         continue
                     selectedDataFrame = v[0]
-                    if 'debug' in charts and 'showChartColumnName' in charts['debug'] and charts['debug']['showChartColumnName']:
-                        print(f"[INFO] {k} field name for drawing chart: {selectedDataFrame.columns.to_list()}")
                     for selectedColumn in chartsOutput.keys():
                         if selectedColumn not in selectedDataFrame.columns:
                             continue
                         #targetValues = list(selectedDataFrame[selectedColumn])
                         #avgValues = []
                         #for i in range(len(targetValues)):
                         #    avgValues.append(sum(targetValues[0:i+1])/(i+1) if i > 0 else targetValues[i])
                         avgValues = selectedDataFrame[selectedColumn].expanding().mean().tolist()
+                        sumOfTargetColumn[k] = avgValues
 
-                        output.append(f"##### {k} - Cumulative Average of '{selectedColumn}' Chart:")
+                        if 'showEachCumulativeAverageColumnChart' in charts['debug'] and charts['debug']['showEachCumulativeAverageColumnChart']:
+                            moreDetails.append(f"###### {k} - Cumulative Average of '{selectedColumn}' Chart:")
+                            moreDetails.append("```")
+                            moreDetails.append(asciichartpy.plot(avgValues, cfg=chartsConfig))
+                            moreDetails.append("```")
+                if len(sumOfTargetColumn) > 0:
+                    passDataLengthCheck = True
+                    sumOfTargetColumnValue = []
+                    for avgValues in sumOfTargetColumn.values():
+                        if len(sumOfTargetColumnValue) == 0:
+                            sumOfTargetColumnValue = avgValues
+                        elif len(sumOfTargetColumnValue) != len(avgValues):
+                            passDataLengthCheck = False
+                            break
+                        else:
+                            sumOfTargetColumnValue = [sum(x) for x in zip(sumOfTargetColumnValue, avgValues)] 
+                    output.append(f"##### Sum of ({', '.join(list(sumOfTargetColumn.keys()))}) - Cumulative Average of '{selectedColumn}' Chart:")
+                    if len(sumOfTargetColumnValue) == 0:
+                        passDataLengthCheck = False
+                        output.append()
+                        output.append('No Data')
+                    elif not passDataLengthCheck:
+                        output.append('All targetColumn lists must have the same number of elements.')
+                    else:
                         output.append("```")
-                        output.append(asciichartpy.plot(avgValues, cfg=chartsConfig))
+                        output.append(asciichartpy.plot(sumOfTargetColumnValue, cfg=chartsConfig))
                         output.append("```")
 
+                    if len(moreDetails) > 0:
+                        output = output + moreDetails
+
         return "\n".join(output)
```

### Comparing `google_csv_helper-1.2.4/google_csv_helper/cmd.py` & `google_csv_helper-1.2.5/google_csv_helper/cmd.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,17 +21,18 @@
             except ValueError:
                 raise argparse.ArgumentTypeError(f"not a valid date: {data}")
         return output
     parser = argparse.ArgumentParser()
     parser.add_argument("csv_dir", nargs="*", type=str, help="the directory where the csv file is located")
     parser.add_argument("--output", choices=['json', 'markdown'], default='markdown', help="results format")
     parser.add_argument("--output-type", choices=['adsense', 'ga3', 'ga4'], default="adsense", help="the report")
-    parser.add_argument("--output-chart", type=str, default="", help="draw cumulative average charts for specific columns identified by field names (multiple fields separated by commas)")
-    parser.add_argument("--output-chart-field-candidate", action="store_true", default=False, help="show field name for drawing cumulative average charts")
-    parser.add_argument("--output-chart-config", type=str, default="{}", help="cumulative average chart configuration")
+    parser.add_argument("--output-chart-columns", type=str, default="", help="specify which CSV columns to plot, identified by field names (multiple fields separated by commas)")
+    parser.add_argument("--output-chart-detailed-columns", action="store_true", default=False, help="specify which CSV columns to plot with detailed information (multiple fields separated by commas)")
+    parser.add_argument("--output-chart-list-columns", action="store_true", default=False, help="lst available CSV columns that can be used for plotting")
+    parser.add_argument("--output-chart-plot-config", type=str, default='{"height": 10}', help="configure additional plot settings such as colors, width, height, etc.")
     parser.add_argument("--report", choices=['date', 'week', 'month'], default='date', help="the report type")
     parser.add_argument("--debug", action="store_true", default=False, help="output the debug messages")
     parser.add_argument("--version", action="store_true", default=False, help="show the version")
     parser.add_argument("--enddate", default="today", type=valid_date, help="date for csv key field filter, date format = 'YYYY-mm-dd'")
     parser.add_argument("--adsense-filename-keyword", type=str, default="adsense", help="the keyword on csv filename of adsense")
     parser.add_argument("--admob-filename-keyword", type=str, default="admob", help="the keyword on csv filename of admob")
     parser.add_argument("--ga-filename-keyword", type=str, default="ga", help="the keyword on csv filename of gogle anayltics")
@@ -184,43 +185,44 @@
 
     if args.debug:
         obj.enableDebug()
 
     #obj.setImportCSVDuplicateRules('default', 'last')
     obj.readAllCSVRawFile()
 
-    output_chart = {
+    setup_output_chart = {
         'config' : { 
             'height': 10,
         }, 'columns': {
         }, 'debug': {
-            'showChartColumnName': args.output_chart_field_candidate,
+            'showCumulativeAverageChartColumnCandidates': args.output_chart_list_columns,
+            'showEachCumulativeAverageColumnChart': args.output_chart_detailed_columns,
         }
     }
-    if args.output_chart != '':
-        for fieldName in args.output_chart.split(','):
+    if args.output_chart_columns != '':
+        for fieldName in args.output_chart_columns.split(','):
             fieldName = fieldName.strip()
             if len(fieldName) == 0:
                 continue
-            output_chart['columns'][fieldName] = fieldName
-    if args.output_chart_config != '' and args.output_chart_config != '{}':
+            setup_output_chart['columns'][fieldName] = fieldName
+    if args.output_chart_plot_config != '' and args.output_chart_plot_config != '{}':
        try:
-           test_json_value = json.loads(args.output_chart_config)
-           output_chart['config'] = test_json_value
+           test_json_value = json.loads(args.output_chart_plot_config)
+           setup_output_chart['config'] = test_json_value
        except Exception as e:
            if args.debug:
                print(e)
 
     if args.output == 'markdown':
         if args.report == 'date':
             if args.output_type == 'adsense':
                 print("## Current:")
-                print(obj.getDailyMarkDownReport(args.enddate, csv_filename_pattern, output_chart))
+                print(obj.getDailyMarkDownReport(args.enddate, csv_filename_pattern, setup_output_chart))
                 print("## Previuos:")
-                print(obj.getDailyMarkDownReport(args.enddate.replace(day=1), csv_filename_pattern, output_chart))
+                print(obj.getDailyMarkDownReport(args.enddate.replace(day=1), csv_filename_pattern, setup_output_chart))
             else:
                 print("## Current:")
                 print(obj.getDailyMarkDownReport(args.enddate, csv_filename_pattern))
                 print("## Previuos:")
                 print(obj.getDailyMarkDownReport(args.enddate - datetime.timedelta(days=7), csv_filename_pattern))
     else:
         if args.report == 'date':
```

### Comparing `google_csv_helper-1.2.4/google_csv_helper/csv_common.py` & `google_csv_helper-1.2.5/google_csv_helper/csv_common.py`

 * *Files identical despite different names*

### Comparing `google_csv_helper-1.2.4/google_csv_helper/csv_helper.py` & `google_csv_helper-1.2.5/google_csv_helper/csv_helper.py`

 * *Files identical despite different names*

### Comparing `google_csv_helper-1.2.4/google_csv_helper/ga3_csv_helper.py` & `google_csv_helper-1.2.5/google_csv_helper/ga3_csv_helper.py`

 * *Files identical despite different names*

### Comparing `google_csv_helper-1.2.4/google_csv_helper/ga4_csv_helper.py` & `google_csv_helper-1.2.5/google_csv_helper/ga4_csv_helper.py`

 * *Files identical despite different names*

### Comparing `google_csv_helper-1.2.4/google_csv_helper/google_common.py` & `google_csv_helper-1.2.5/google_csv_helper/google_common.py`

 * *Files identical despite different names*

### Comparing `google_csv_helper-1.2.4/google_csv_helper.egg-info/PKG-INFO` & `google_csv_helper-1.2.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-csv-helper
-Version: 1.2.4
+Version: 1.2.5
 Summary: A simple tool that takes CSV reports from Google Adsense, Google Admob, and Google Analytics and outputs them in JSON / Pandas.DataFrame format.
 Home-page: https://github.com/changyy/google-csv-helper
 Download-URL: https://pypi.org/project/google-csv-helper/
 Author: Yuan-Yi Chang
 Author-email: <changyy.csie@gmail.com>
 Keywords: python,google,csv,adsense,admob,report
 Classifier: Programming Language :: Python :: 3
@@ -99,66 +99,116 @@
 | -- | --: | --: | --: | --: | --: 
 | Admob Global | 1,234.56 | 123.45 (-12.34%) | 0.001 (-1.23%) | 234.56 [06/02 Fri] | 456.78 [06/01 Thu] 
 | Adsense Global | 1,234.56 | 123.45 (-12.34%) | 0.1234 (-2.34%) | 123.45 [06/02 Fri] | 345.67 [06/01 Thu] 
 | Adsense China |  1,234.56 | 123.45 (-12.34%) | 0.2345 (2.34%) | 123.45 [06/02 Fri] | 345.67 `[06/01 Thu] 
 | Total | 1,234.56 | 456.78 | | | 
 ```
 
+---
+
 ```
-% google-csv-helper --output markdown --output-chart 'Estimated earnings (USD)' csv 
+% google-csv-helper --output markdown --output-chart-columns 'Estimated earnings (USD)' csv 
 ```
 
 ## Current:
 ### Date Range: 2023-06-01 ~ 2023-06-04
 #### compare: 2023-05-01 ~ 2023-05-31
 | Item | Cumulative Revenue | Average Daily Revenue | Average CPC | Min Daily Revenue | Max Daily Revenue 
 | -- | --: | --: | --: | --: | --: 
 | Admob Global | 1,234.56 | 123.45 (-12.34%) | 0.001 (-1.23%) | 234.56 [06/02 Fri] | 456.78 [06/01 Thu] 
 | Adsense Global | 1,234.56 | 123.45 (-12.34%) | 0.1234 (-2.34%) | 123.45 [06/02 Fri] | 345.67 [06/01 Thu] 
 | Adsense China |  1,234.56 | 123.45 (-12.34%) | 0.2345 (2.34%) | 123.45 [06/02 Fri] | 345.67 `[06/01 Thu] 
 | Total | 1,234.56 | 456.78 | | | 
 #### ref
-##### Admob Global - Cumulative Average of 'Estimated earnings (USD)' Chart:
+##### Sum of (Admob Global, Adsense Global, Adsense China) - Cumulative Average of 'Estimated earnings (USD)' Chart:
+```
+ 867.61  ┤
+ 846.52  ┤                          ╭──
+ 825.44  ┼╮                        ╭╯
+ 804.36  ┤│                      ╭─╯
+ 783.27  ┤│                     ╭╯
+ 762.19  ┤│                   ╭─╯
+ 741.11  ┤│ ╭╮ ╭╮            ╭╯
+ 720.02  ┤│╭╯╰─╯╰╮           │
+ 698.94  ┤╰╯     ╰─╮         │
+ 677.86  ┤         ╰╮       ╭╯
+ 656.77  ┤          ╰───╮   │
+ 635.69  ┤              ╰───╯
+```
+
+---
+
+```
+% google-csv-helper --output-chart-columns 'Estimated earnings (USD)' --output-chart-detailed-columns csv
+```
+
+## Current:
+### Date Range: 2023-06-01 ~ 2023-06-04
+#### compare: 2023-05-01 ~ 2023-05-31
+| Item | Cumulative Revenue | Average Daily Revenue | Average CPC | Min Daily Revenue | Max Daily Revenue 
+| -- | --: | --: | --: | --: | --: 
+| Admob Global | 1,234.56 | 123.45 (-12.34%) | 0.001 (-1.23%) | 234.56 [06/02 Fri] | 456.78 [06/01 Thu] 
+| Adsense Global | 1,234.56 | 123.45 (-12.34%) | 0.1234 (-2.34%) | 123.45 [06/02 Fri] | 345.67 [06/01 Thu] 
+| Adsense China |  1,234.56 | 123.45 (-12.34%) | 0.2345 (2.34%) | 123.45 [06/02 Fri] | 345.67 `[06/01 Thu] 
+| Total | 1,234.56 | 456.78 | | | 
+#### ref
+##### Sum of (Admob Global, Adsense Global, Adsense China) - Cumulative Average of 'Estimated earnings (USD)' Chart:
+```
+ 867.61  ┤
+ 846.52  ┤                          ╭──
+ 825.44  ┼╮                        ╭╯
+ 804.36  ┤│                      ╭─╯
+ 783.27  ┤│                     ╭╯
+ 762.19  ┤│                   ╭─╯
+ 741.11  ┤│ ╭╮ ╭╮            ╭╯
+ 720.02  ┤│╭╯╰─╯╰╮           │
+ 698.94  ┤╰╯     ╰─╮         │
+ 677.86  ┤         ╰╮       ╭╯
+ 656.77  ┤          ╰───╮   │
+ 635.69  ┤              ╰───╯
+```
+###### Admob Global - Cumulative Average of 'Estimated earnings (USD)' Chart:
 ```
   297.11  ┼╮
   294.28  ┤│     ╭╮
   291.46  ┤│    ╭╯╰─╮
   288.64  ┤│    │   ╰╮
   285.81  ┤│    │    ╰╮╭╮
   282.99  ┤│    │     ╰╯╰╮
   280.17  ┤│    │        ╰╮
   277.35  ┤│   ╭╯         ╰╮
   274.52  ┤│   │           ╰╮ ╭─╮
   271.70  ┤╰╮  │            ╰─╯ ╰─╮  ╭──
   268.88  ┤ ╰──╯                  ╰──╯
   266.06  ┤
 ```
-##### Adsense Global - Cumulative Average of 'Estimated earnings (USD)' Chart:
+###### Adsense Global - Cumulative Average of 'Estimated earnings (USD)' Chart:
 ```
   495.71  ┤
   473.65  ┤                          ╭──
   451.59  ┤                         ╭╯
   429.53  ┼╮                       ╭╯
   407.46  ┤│                     ╭─╯
   385.40  ┤│                    ╭╯
   363.34  ┤│╭─╮                ╭╯
   341.28  ┤╰╯ ╰╮              ╭╯
   319.22  ┤    ╰──╮           │
   297.16  ┤       ╰╮         ╭╯
   275.10  ┤        ╰─╮      ╭╯
   253.04  ┤          ╰──────╯
 ```
-##### Adsense China - Cumulative Average of 'Estimated earnings (USD)' Chart:
+###### Adsense China - Cumulative Average of 'Estimated earnings (USD)' Chart:
 ```
   211.76  ┤
   209.91  ┤     ╭──╮
   208.06  ┤     │  ╰╮
   206.20  ┤     │   ╰╮ ╭─╮
   204.35  ┤     │    ╰─╯ ╰╮  ╭──╮
   202.50  ┤    ╭╯         ╰──╯  ╰─╮
   200.65  ┼╮  ╭╯                  ╰────╮
   198.80  ┤│  │                        ╰
   196.95  ┤│  │
   195.10  ┤│ ╭╯
   193.25  ┤│ │
   191.40  ┤╰─╯
 ```
+
```

### Comparing `google_csv_helper-1.2.4/google_csv_helper.egg-info/SOURCES.txt` & `google_csv_helper-1.2.5/google_csv_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google_csv_helper-1.2.4/setup.py` & `google_csv_helper-1.2.5/setup.py`

 * *Files identical despite different names*

