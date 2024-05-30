# Comparing `tmp/pyqueen-1.1.1.tar.gz` & `tmp/pyqueen-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqueen-1.1.1.tar", last modified: Sat May 25 16:46:41 2024, max compression
+gzip compressed data, was "pyqueen-1.1.2.tar", last modified: Thu May 30 14:14:30 2024, max compression
```

## Comparing `pyqueen-1.1.1.tar` & `pyqueen-1.1.2.tar`

### file list

```diff
@@ -1,51 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:46:41.356139 pyqueen-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-25 16:46:37.000000 pyqueen-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-25 16:46:41.356139 pyqueen-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-25 16:46:37.000000 pyqueen-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-25 16:46:37.000000 pyqueen-1.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:46:41.352139 pyqueen-1.1.1/pyqueen/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-25 16:46:37.000000 pyqueen-1.1.1/pyqueen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:46:41.352139 pyqueen-1.1.1/pyqueen/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:46:37.000000 pyqueen-1.1.1/pyqueen/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-25 16:46:37.000000 pyqueen-1.1.1/pyqueen/analysis/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:46:41.352139 pyqueen-1.1.1/pyqueen/chart/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:46:37.000000 pyqueen-1.1.1/pyqueen/chart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-25 16:46:37.000000 pyqueen-1.1.1/pyqueen/chart/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:46:41.356139 pyqueen-1.1.1/pyqueen/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:46:37.000000 pyqueen-1.1.1/pyqueen/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7994 2024-05-25 16:46:37.000000 pyqueen-1.1.1/pyqueen/io/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     9573 2024-05-25 16:46:37.000000 pyqueen-1.1.1/pyqueen/io/data_source_bak.py
--rw-r--r--   0 runner    (1001) docker     (127)     7938 2024-05-25 16:46:37.000000 pyqueen-1.1.1/pyqueen/io/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-05-25 16:46:37.000000 pyqueen-1.1.1/pyqueen/io/ds_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-25 16:46:37.000000 pyqueen-1.1.1/pyqueen/io/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-25 16:46:37.000000 pyqueen-1.1.1/pyqueen/io/ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-25 16:46:37.000000 pyqueen-1.1.1/pyqueen/io/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-25 16:46:37.000000 pyqueen-1.1.1/pyqueen/io/kvdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     7954 2024-05-25 16:46:37.000000 pyqueen-1.1.1/pyqueen/io/sqldb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-25 16:46:37.000000 pyqueen-1.1.1/pyqueen/io/web.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:46:41.356139 pyqueen-1.1.1/pyqueen/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:46:37.000000 pyqueen-1.1.1/pyqueen/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-25 16:46:37.000000 pyqueen-1.1.1/pyqueen/remote/linux.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:46:41.356139 pyqueen-1.1.1/pyqueen/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:46:37.000000 pyqueen-1.1.1/pyqueen/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-05-25 16:46:37.000000 pyqueen-1.1.1/pyqueen/service/pydingtalk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-25 16:46:37.000000 pyqueen-1.1.1/pyqueen/service/pyemail.py
--rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-05-25 16:46:37.000000 pyqueen-1.1.1/pyqueen/service/pywechat.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-25 16:46:37.000000 pyqueen-1.1.1/pyqueen/service/showdoc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:46:41.356139 pyqueen-1.1.1/pyqueen/utility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:46:37.000000 pyqueen-1.1.1/pyqueen/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-25 16:46:37.000000 pyqueen-1.1.1/pyqueen/utility/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     9966 2024-05-25 16:46:37.000000 pyqueen-1.1.1/pyqueen/utility/time_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-05-25 16:46:37.000000 pyqueen-1.1.1/pyqueen/utility/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:46:41.356139 pyqueen-1.1.1/pyqueen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-25 16:46:41.000000 pyqueen-1.1.1/pyqueen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-25 16:46:41.000000 pyqueen-1.1.1/pyqueen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 16:46:41.000000 pyqueen-1.1.1/pyqueen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-25 16:46:41.000000 pyqueen-1.1.1/pyqueen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-25 16:46:41.000000 pyqueen-1.1.1/pyqueen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-25 16:46:41.000000 pyqueen-1.1.1/pyqueen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 16:46:41.356139 pyqueen-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-25 16:46:37.000000 pyqueen-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:46:41.356139 pyqueen-1.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:46:37.000000 pyqueen-1.1.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-25 16:46:37.000000 pyqueen-1.1.1/test/test_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:14:30.659702 pyqueen-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-30 14:14:26.000000 pyqueen-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-30 14:14:30.659702 pyqueen-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-30 14:14:26.000000 pyqueen-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:14:30.651701 pyqueen-1.1.2/pyqueen/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:14:30.655701 pyqueen-1.1.2/pyqueen/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/analysis/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:14:30.655701 pyqueen-1.1.2/pyqueen/chart/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/chart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/chart/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:14:30.655701 pyqueen-1.1.2/pyqueen/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7316 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/io/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/io/ds_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/io/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/io/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/io/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/io/kvdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/io/sqldb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/io/web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:14:30.655701 pyqueen-1.1.2/pyqueen/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/remote/linux.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:14:30.655701 pyqueen-1.1.2/pyqueen/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/service/pydingtalk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/service/pyemail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/service/pywechat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/service/showdoc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:14:30.659702 pyqueen-1.1.2/pyqueen/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/utility/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9966 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/utility/time_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/utility/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:14:30.659702 pyqueen-1.1.2/pyqueen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-30 14:14:30.000000 pyqueen-1.1.2/pyqueen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-30 14:14:30.000000 pyqueen-1.1.2/pyqueen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 14:14:30.000000 pyqueen-1.1.2/pyqueen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-30 14:14:30.000000 pyqueen-1.1.2/pyqueen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-30 14:14:30.000000 pyqueen-1.1.2/pyqueen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 14:14:30.000000 pyqueen-1.1.2/pyqueen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 14:14:30.659702 pyqueen-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-30 14:14:26.000000 pyqueen-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:14:30.659702 pyqueen-1.1.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:14:26.000000 pyqueen-1.1.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-30 14:14:26.000000 pyqueen-1.1.2/test/test_main.py
```

### Comparing `pyqueen-1.1.1/LICENSE` & `pyqueen-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqueen-1.1.1/PKG-INFO` & `pyqueen-1.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pyqueen
-Version: 1.1.1
+Version: 1.1.2
 Summary: Rule your Data
 Home-page: https://github.com/ts7ming/pyqueen.git
 Author: ts7ming
 Author-email: qiming.ma@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pandas
-Requires-Dist: SQLAlchemy
+Requires-Dist: pandas>=2.0.0
+Requires-Dist: SQLAlchemy>=2.0.0
 Requires-Dist: xlrd==1.2.0
 Requires-Dist: XlsxWriter
 
 # PyQueen
 
 ![](logo.jpg)
```

### Comparing `pyqueen-1.1.1/README.md` & `pyqueen-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyqueen-1.1.1/pyqueen/analysis/model.py` & `pyqueen-1.1.2/pyqueen/analysis/model.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.1.1/pyqueen/chart/plot.py` & `pyqueen-1.1.2/pyqueen/chart/plot.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.1.1/pyqueen/io/ds_plugin.py` & `pyqueen-1.1.2/pyqueen/io/ds_plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 import datetime
 import os
-
+import numpy as np
 import pandas as pd
-
+from pyqueen.io.excel import Excel
 
 class DsLog:
+    """
+    Logger for DataSource
+    """
+
     def __init__(self):
+        """
+        Logger for DataSource
+        """
         self.__t_start = None
         self.etl_log = {}
         self.__etl_param_sort = [
             'py_path',
             'func_name',
             'start_time',
             'end_time',
@@ -23,68 +30,108 @@
             'db_name',
             'table_name'
         ]
         self.logger = None
 
     @staticmethod
     def __file_log(etl_log):
+        """
+        std logger for "file", save ds log to file
+        :param etl_log: etl log
+        :return:
+        """
         log_path = etl_log['py_path']
         log_path = str(log_path).replace('.py', '.log')
         info = '\n------------------------------------\n'
         for k, v in etl_log.items():
             info += str(k) + ': ' + str(v) + '\n'
         info += '\n------------------------------------\n'
         with open(log_path, 'a+', encoding='utf-8') as f:
             f.write(info)
 
     def set_logger(self, logger):
+        """
+        reset logger for DataSource
+        :param logger: a function
+        :return:
+        """
         if str(logger) == 'file':
             self.logger = self.__file_log
         else:
             self.logger = logger
 
     def trace_start(self):
+        """
+        DataSource log
+        :return:
+        """
         self.__t_start = datetime.datetime.now()
         import inspect
         a = inspect.stack()[2]
         file_name = a.filename
         func = a.function
         self.etl_log['start_time'] = str(self.__t_start.strftime('%Y-%m-%d %H:%M:%S'))
         self.etl_log['py_path'] = file_name
         self.etl_log['func_name'] = func
 
     def trace_end(self):
+        """
+        DataSource log
+        :return:
+        """
         t_end = datetime.datetime.now()
         t_duration = str((t_end - self.__t_start).seconds)
         self.etl_log['end_time'] = str(t_end.strftime('%Y-%m-%d %H:%M:%S'))
         self.etl_log['duration'] = t_duration
         sortd_log = {i: self.etl_log[i] for i in self.__etl_param_sort if i in self.etl_log}
         for k, v in self.etl_log.items():
             if k not in sortd_log:
                 sortd_log[k] = v
         if self.logger is not None:
             self.logger(sortd_log)
         self.etl_log = {}
 
 
 class DsPlugin:
+    """
+    plugin for DataSource
+    """
     def read_sql(self, sql):
+        """
+        tmp
+        """
         return pd.DataFrame()
 
     def row_count(self, table_name):
+        """
+        quickly count rows of a table
+        :param table_name: table name
+        :return: row nums
+        """
         sql = 'select count(1) from ' + table_name
         df = self.read_sql(sql)
         rows = df.values[0][0]
         return int(rows)
 
     def get_value(self, sql):
+        """
+        quickly get first value of a query
+        :param sql: sql text
+        :return: value
+        """
         df = self.read_sql(sql)
         return df.values[0][0]
 
     def get_sql_group(self, sql, params):
+        """
+        quickly get many params query
+        :param sql:
+        :param params:
+        :return:
+        """
         df = None
         for param in params:
             new_sql = sql.format(param)
             df_tmp = self.read_sql(new_sql)
             if df is None:
                 df = df_tmp
             else:
@@ -112,14 +159,17 @@
         pass
 
     def close_conn(self):
         pass
 
 
 class DsExt:
+    """
+    extend function for DataSource
+    """
     @staticmethod
     def pdsql(sql, data):
         import duckdb
         with duckdb.connect() as conn:
             for df_name, df in data.items():
                 conn.register(df_name, df)
             result = conn.execute(sql).df()
```

### Comparing `pyqueen-1.1.1/pyqueen/io/ftp.py` & `pyqueen-1.1.2/pyqueen/io/ftp.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.1.1/pyqueen/io/image.py` & `pyqueen-1.1.2/pyqueen/io/image.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.1.1/pyqueen/io/kvdb.py` & `pyqueen-1.1.2/pyqueen/io/kvdb.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.1.1/pyqueen/io/web.py` & `pyqueen-1.1.2/pyqueen/io/web.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.1.1/pyqueen/remote/linux.py` & `pyqueen-1.1.2/pyqueen/remote/linux.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.1.1/pyqueen/service/pydingtalk.py` & `pyqueen-1.1.2/pyqueen/service/pydingtalk.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.1.1/pyqueen/service/pyemail.py` & `pyqueen-1.1.2/pyqueen/service/pyemail.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.1.1/pyqueen/service/pywechat.py` & `pyqueen-1.1.2/pyqueen/service/pywechat.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.1.1/pyqueen/service/showdoc.py` & `pyqueen-1.1.2/pyqueen/service/showdoc.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.1.1/pyqueen/utility/command.py` & `pyqueen-1.1.2/pyqueen/utility/command.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.1.1/pyqueen/utility/time_kit.py` & `pyqueen-1.1.2/pyqueen/utility/time_kit.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.1.1/pyqueen/utility/utils.py` & `pyqueen-1.1.2/pyqueen/utility/utils.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.1.1/pyqueen.egg-info/PKG-INFO` & `pyqueen-1.1.2/pyqueen.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pyqueen
-Version: 1.1.1
+Version: 1.1.2
 Summary: Rule your Data
 Home-page: https://github.com/ts7ming/pyqueen.git
 Author: ts7ming
 Author-email: qiming.ma@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pandas
-Requires-Dist: SQLAlchemy
+Requires-Dist: pandas>=2.0.0
+Requires-Dist: SQLAlchemy>=2.0.0
 Requires-Dist: xlrd==1.2.0
 Requires-Dist: XlsxWriter
 
 # PyQueen
 
 ![](logo.jpg)
```

### Comparing `pyqueen-1.1.1/pyqueen.egg-info/SOURCES.txt` & `pyqueen-1.1.2/pyqueen.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 pyqueen.egg-info/top_level.txt
 pyqueen/analysis/__init__.py
 pyqueen/analysis/model.py
 pyqueen/chart/__init__.py
 pyqueen/chart/plot.py
 pyqueen/io/__init__.py
 pyqueen/io/data_source.py
-pyqueen/io/data_source_bak.py
-pyqueen/io/db.py
 pyqueen/io/ds_plugin.py
 pyqueen/io/excel.py
 pyqueen/io/ftp.py
 pyqueen/io/image.py
 pyqueen/io/kvdb.py
 pyqueen/io/sqldb.py
 pyqueen/io/web.py
@@ -32,8 +30,8 @@
 pyqueen/service/pywechat.py
 pyqueen/service/showdoc.py
 pyqueen/utility/__init__.py
 pyqueen/utility/command.py
 pyqueen/utility/time_kit.py
 pyqueen/utility/utils.py
 test/__init__.py
-test/test_data_source.py
+test/test_main.py
```

### Comparing `pyqueen-1.1.1/test/test_data_source.py` & `pyqueen-1.1.2/test/test_main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,135 +1,111 @@
+from pyqueen import DataSource, TimeKit
 import pandas as pd
+import os
 
-from pyqueen import DataSource
+tk = TimeKit()
 
+SERVERS = {
+    'mssql_1': {
+        'conn_type': 'mssql',
+        'host': 'localhost',
+        'port': '1433',
+        'username': 'sa',
+        'password': 'mssql123',
+        'db_name': 'master'
+    },
+    'pgsql_1': {
+        'conn_type': 'pgsql',
+        # 'host': 'localhost',
+        'host':'olympus',
+        'port': '5432',
+        'username': 'postgres',
+        'password': ' ',
+        'db_name': 'postgres'
+    },
+    'mysql_1': {
+        'conn_type': 'mysql',
+        'host': '172.23.213.221',
+        'port': '3306',
+        'username': 'root',
+        'password': '',
+        'db_name': 'mysql'
+    },
+}
+
+
+def clean():
+    for x in os.listdir('.'):
+        if '.db' in x or '.xlsx' in x:
+            os.remove(x)
+
+
+def test_data_source(conn_info):
+    ds = DataSource(**conn_info)
+    test_db_name = 'pq_td_' + str(tk.today)
+    test_table_name = 'pq_tb_' + str(tk.today)
+    print('创建数据库')
+    auto_commit = True
+    if conn_info['conn_type'] == 'mssql': ds.set_db('master')
+    if conn_info['conn_type'] == 'pgsql': ds.set_db('postgres')
+    ds.exe_sql(sql='DROP DATABASE IF EXISTS %s' % test_db_name, auto_commit=auto_commit)
+    ds.exe_sql(sql='CREATE DATABASE %s' % test_db_name, auto_commit=auto_commit)
+    ds.set_db(test_db_name)
+
+    auto_commit = False
+    print('创建表')
+    ds.exe_sql('DROP TABLE IF EXISTS ' + test_table_name)
+    ds.exe_sql('CREATE TABLE %s (id INT NOT NULL,name varchar(100) NULL)' % test_table_name)
+    ds.exe_sql("INSERT INTO %s VALUES (9,'hhh')" % test_table_name)
 
-def test_mysql():
-    ds = DataSource(conn_type='mysql', host='172.23.213.221', username='root', password='qiming', port=3306, db_name='demo')
-
-    sql = 'DROP TABLE IF EXISTS t_table'
-    ds.exe_sql(sql)
-
-    sql = '''
-        CREATE TABLE t_table (
-            id INT NOT NULL,
-            name varchar(100) NULL
-        )
-    '''
-    ds.exe_sql(sql)
-    print('mysql exe_sql is ok')
-
-    import pandas as pd
-
-    df = pd.DataFrame({'id': [1, 2, 3, 4], 'name': ['libnl', 'agds', 'gfrt', 'hhg']})
-    ds.to_db(df, tb_name='t_table', fast_load=False)
-    print('mysql to_db is ok')
-
-    v = ds.get_sql('select count(1) as v from t_table')
-    if int(v.values[0][0]) == 4:
-        print('mysql read_sql is ok')
-    else:
-        print('mysql read_sql not match')
-
-def test_mysql2():
-    ds = DataSource(conn_type='mysql', host='olympus', username='root', password='54maqiming', port=3306, db_name='cdc_source')
-
-    sql = 'DROP TABLE IF EXISTS t_table'
-    ds.exe_sql(sql)
-
-    sql = '''
-        CREATE TABLE t_table (
-            id INT NOT NULL,
-            name varchar(100) NULL
-        )
-    '''
-    ds.exe_sql(sql)
-    print('mysql exe_sql is ok')
-
-    import pandas as pd
-
+    # 模拟数据
     df = pd.DataFrame({'id': [1, 2, 3, 4], 'name': ['libnl', 'agds', 'gfrt', 'hhg']})
-    ds.to_db(df, tb_name='t_table', fast_load=False)
-    print('mysql to_db is ok')
-
-    v = ds.get_sql('select count(1) as v from t_table')
-    if int(v.values[0][0]) == 4:
-        print('mysql read_sql is ok')
-    else:
-        print('mysql read_sql not match')
-
-
-def test_postgresql():
-    ds = DataSource(conn_type='pgsql', host='localhost', username='postgres', password='1qaz2wsx!', port=5432, db_name='postgres')
-
-    sql = 'DROP TABLE IF EXISTS t_table_pg'
-    ds.exe_sql(sql)
-
-    sql = '''
-        CREATE TABLE t_table_pg (
-            id INT NOT NULL,
-            name varchar(100) NULL
-        )
-    '''
-    ds.exe_sql(sql)
-    print('pgsql exe_sql is ok')
-
-    import pandas as pd
+    print('写入表')
+    ds.to_db(df, tb_name=test_table_name, fast_load=False)
 
+    print('查询')
+    v = ds.read_sql('select count(1) as v from ' + test_table_name)
+    if int(v.values[0][0]) != 5:
+        print('read_sql not match')
+    print('导出excel')
+    ds.to_excel(file_path='df2excel.xlsx', sheet_list=[[df, 'sht']])
+
+    auto_commit = True
+    print('删除')
+    if conn_info['conn_type'] == 'mssql': ds.set_db('master')
+    if conn_info['conn_type'] == 'pgsql': ds.set_db('postgres')
+    ds.exe_sql(sql='DROP DATABASE IF EXISTS %s' % test_db_name, auto_commit=auto_commit)
+
+
+def test_data_source_e():
+    print('单独使用 read_sql')
+    ds = DataSource()
     df = pd.DataFrame({'id': [1, 2, 3, 4], 'name': ['libnl', 'agds', 'gfrt', 'hhg']})
-    ds.to_db(df, tb_name='t_table_pg')
-    print('pgsql to_db is ok')
-
-    v = ds.get_sql('select count(1) as v from t_table_pg')
-    v2 = ds.row_count(table_name='t_table_pg')
-    v3 = ds.ge
-    if int(v.values[0][0]) == 4 and int(v2) == 4:
-        print('pgsql read_sql is ok')
-    else:
-        print('pgsql read_sql not match')
-
-
-def test_redis():
-    ds = DataSource(conn_type='redis', host='172.23.213.221', port='6379', db_name=0)
-    ds.set_logger(logger=print)
-    ds.set_v('ff', 11)
-    ds.set_v('中文k', '中文v')
-    if int(ds.get_v('ff')) == 11:
-        print('redis get is ok')
-    else:
-        print('redis get  not match')
-    if ds.get_v('中文k') == '中文v':
-        print('redis get中文 is ok')
-    else:
-        print('redis get  not match')
-
-
-def test_sqlite():
-    ds = DataSource(conn_type='sqlite', file_path='tst.db')
-    import pandas as pd
-
-    df = pd.DataFrame({'dd': [1, 2, 3], 'gg': ['daf', 'gfytr', 'eee']})
-    ds.to_db(df, tb_name='hhhhh')
-    print('sqlite: to_db is ok')
-    sql = 'select max(dd) as f from hhhhh'
-    v = int(ds.get_value(sql))
-    if v == 3:
-        print('sqlite: read_sql is ok')
-
-def test_excel():
-    ds = DataSource(conn_type='excel', file_path='./tst.xlsx')
-    import pandas as pd
-
-    df = pd.DataFrame({'dd': [1, 2, 3], 'gg': ['daf', 'gfytr', 'eee']})
-    ds.to_excel(sheet_list=[[df,'ma']])
-    print('excel: to_excel is ok')
-
+    df2 = pd.DataFrame({'id': [11, 22, 33, 44], 'name': ['trtr', 'sd', 'gf', 'hg']})
+    df_r = ds.read_sql(sql='select * from tb1 union all select * from tb2', data={'tb1': df, 'tb2': df2})
+    if df_r.shape[0] != 8:
+        print('not match')
+
+    print('sql on excel')
+    ds2 = DataSource(conn_type='excel', file_path='test_data_source_e')
+    ds2.to_excel(sheet_list=[[df, 'tb1'], [df2, 'tb2']])
+    df_r = ds2.read_sql(sql='select * from tb1 union all select * from tb2')
+    if df_r.shape[0] != 8:
+        print('not match')
+
+
+def main():
+    conn_list = [
+        'mssql_1',
+        'pgsql_1',
+        'mysql_1'
+    ]
+    for conn in conn_list:
+        clean()
+        test_data_source(SERVERS[conn])
+        clean()
 
+    test_data_source_e()
 
 
 if __name__ == '__main__':
-    # test_mysql()
-    test_mysql2()
-    # test_postgresql()
-    # test_redis()
-    test_sqlite()
-    test_excel()
+    main()
```

