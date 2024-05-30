# Comparing `tmp/cc_report-0.0.3.tar.gz` & `tmp/cc_report-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cc_report-0.0.3.tar", last modified: Wed May  8 13:41:40 2024, max compression
+gzip compressed data, was "cc_report-0.0.4.tar", last modified: Wed May 29 13:01:35 2024, max compression
```

## Comparing `cc_report-0.0.3.tar` & `cc_report-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 cc         (501) staff       (20)        0 2024-05-08 13:41:40.795652 cc_report-0.0.3/
--rw-r--r--   0 cc         (501) staff       (20)      345 2024-05-08 13:41:40.795468 cc_report-0.0.3/PKG-INFO
-drwxr-xr-x   0 cc         (501) staff       (20)        0 2024-05-08 13:41:40.792863 cc_report-0.0.3/cc_report/
--rw-r--r--   0 cc         (501) staff       (20)      114 2024-05-08 11:24:39.000000 cc_report-0.0.3/cc_report/__init__.py
--rw-r--r--   0 cc         (501) staff       (20)     6016 2024-05-08 09:20:09.000000 cc_report-0.0.3/cc_report/pytest_testreport.py
-drwxr-xr-x   0 cc         (501) staff       (20)        0 2024-05-08 13:41:40.795142 cc_report-0.0.3/cc_report/templates/
--rw-r--r--   0 cc         (501) staff       (20)      114 2024-05-08 11:24:39.000000 cc_report-0.0.3/cc_report/templates/__init__.py
--rw-r--r--   0 cc         (501) staff       (20)    17611 2024-05-08 09:17:46.000000 cc_report-0.0.3/cc_report/templates/templates.html
--rw-r--r--   0 cc         (501) staff       (20)    27983 2024-05-08 09:17:46.000000 cc_report-0.0.3/cc_report/templates/templates2.html
-drwxr-xr-x   0 cc         (501) staff       (20)        0 2024-05-08 13:41:40.793996 cc_report-0.0.3/cc_report.egg-info/
--rw-r--r--   0 cc         (501) staff       (20)      345 2024-05-08 13:41:40.000000 cc_report-0.0.3/cc_report.egg-info/PKG-INFO
--rw-r--r--   0 cc         (501) staff       (20)      364 2024-05-08 13:41:40.000000 cc_report-0.0.3/cc_report.egg-info/SOURCES.txt
--rw-r--r--   0 cc         (501) staff       (20)        1 2024-05-08 13:41:40.000000 cc_report-0.0.3/cc_report.egg-info/dependency_links.txt
--rw-r--r--   0 cc         (501) staff       (20)       52 2024-05-08 13:41:40.000000 cc_report-0.0.3/cc_report.egg-info/entry_points.txt
--rw-r--r--   0 cc         (501) staff       (20)        7 2024-05-08 13:41:40.000000 cc_report-0.0.3/cc_report.egg-info/requires.txt
--rw-r--r--   0 cc         (501) staff       (20)       10 2024-05-08 13:41:40.000000 cc_report-0.0.3/cc_report.egg-info/top_level.txt
--rw-r--r--   0 cc         (501) staff       (20)       38 2024-05-08 13:41:40.795717 cc_report-0.0.3/setup.cfg
--rw-r--r--   0 cc         (501) staff       (20)      830 2024-05-08 13:41:22.000000 cc_report-0.0.3/setup.py
+drwxr-xr-x   0 cc.cheng   (502) staff       (20)        0 2024-05-29 13:01:35.442975 cc_report-0.0.4/
+-rw-r--r--   0 cc.cheng   (502) staff       (20)      345 2024-05-29 13:01:35.442783 cc_report-0.0.4/PKG-INFO
+drwxr-xr-x   0 cc.cheng   (502) staff       (20)        0 2024-05-29 13:01:35.440989 cc_report-0.0.4/cc_report/
+-rw-r--r--   0 cc.cheng   (502) staff       (20)      114 2024-05-28 06:35:48.000000 cc_report-0.0.4/cc_report/__init__.py
+-rw-r--r--   0 cc.cheng   (502) staff       (20)     6018 2024-05-29 13:01:31.000000 cc_report-0.0.4/cc_report/pytest_testreport.py
+drwxr-xr-x   0 cc.cheng   (502) staff       (20)        0 2024-05-29 13:01:35.442572 cc_report-0.0.4/cc_report/templates/
+-rw-r--r--   0 cc.cheng   (502) staff       (20)      114 2024-05-28 06:35:50.000000 cc_report-0.0.4/cc_report/templates/__init__.py
+-rw-r--r--   0 cc.cheng   (502) staff       (20)    17611 2024-05-28 06:35:51.000000 cc_report-0.0.4/cc_report/templates/templates.html
+-rw-r--r--   0 cc.cheng   (502) staff       (20)    27983 2024-05-28 06:35:50.000000 cc_report-0.0.4/cc_report/templates/templates2.html
+drwxr-xr-x   0 cc.cheng   (502) staff       (20)        0 2024-05-29 13:01:35.442034 cc_report-0.0.4/cc_report.egg-info/
+-rw-r--r--   0 cc.cheng   (502) staff       (20)      345 2024-05-29 13:01:35.000000 cc_report-0.0.4/cc_report.egg-info/PKG-INFO
+-rw-r--r--   0 cc.cheng   (502) staff       (20)      364 2024-05-29 13:01:35.000000 cc_report-0.0.4/cc_report.egg-info/SOURCES.txt
+-rw-r--r--   0 cc.cheng   (502) staff       (20)        1 2024-05-29 13:01:35.000000 cc_report-0.0.4/cc_report.egg-info/dependency_links.txt
+-rw-r--r--   0 cc.cheng   (502) staff       (20)       52 2024-05-29 13:01:35.000000 cc_report-0.0.4/cc_report.egg-info/entry_points.txt
+-rw-r--r--   0 cc.cheng   (502) staff       (20)        7 2024-05-29 13:01:35.000000 cc_report-0.0.4/cc_report.egg-info/requires.txt
+-rw-r--r--   0 cc.cheng   (502) staff       (20)       10 2024-05-29 13:01:35.000000 cc_report-0.0.4/cc_report.egg-info/top_level.txt
+-rw-r--r--   0 cc.cheng   (502) staff       (20)       38 2024-05-29 13:01:35.443028 cc_report-0.0.4/setup.cfg
+-rw-r--r--   0 cc.cheng   (502) staff       (20)      830 2024-05-29 13:01:31.000000 cc_report-0.0.4/setup.py
```

### Comparing `cc_report-0.0.3/cc_report/pytest_testreport.py` & `cc_report-0.0.4/cc_report/pytest_testreport.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
     # if os.path.isdir('reports'):
     #     pass
     # else:
     #     os.mkdir('reports')
     # ===========
     paths = str(report2).split('/')[-4:]
-    paths[-1] = time.strftime("%Y-%m-%d_%H_%M_%S_") + paths[-1]
+    # paths[-1] = time.strftime("%Y-%m-%d_%H_%M_%S_") + paths[-1]
     # ===========
     file_name = os.path.join(*paths)
     test_result["run_time"] = '{:.6f} s'.format(time.time() - test_result["start_time"])
     test_result['all'] = len(test_result['cases'])
     if test_result['all'] != 0:
         test_result['pass_rate'] = '{:.2f}'.format(test_result['passed'] / test_result['all'] * 100)
     else:
```

### Comparing `cc_report-0.0.3/cc_report/templates/templates.html` & `cc_report-0.0.4/cc_report/templates/templates.html`

 * *Files identical despite different names*

### Comparing `cc_report-0.0.3/cc_report/templates/templates2.html` & `cc_report-0.0.4/cc_report/templates/templates2.html`

 * *Files identical despite different names*

### Comparing `cc_report-0.0.3/setup.py` & `cc_report-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # @Site   :
 # @File   :setup.py
 
 import setuptools
 
 setuptools.setup(
     name='cc_report',
-    version='0.0.3',
+    version='0.0.4',
     packages=setuptools.find_packages(),
     license='MIT',
     author='cc.cheng',
     author_email='chaicc145@gmail.com',
     description='A MODIFIED REPORT',
     install_requires=['pytest'],
     # 静态文件依赖
```

