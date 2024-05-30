# Comparing `tmp/maslib-0.2.0.tar.gz` & `tmp/maslib-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maslib-0.2.0.tar", last modified: Wed May 29 07:34:22 2024, max compression
+gzip compressed data, was "maslib-0.2.1.tar", last modified: Thu May 30 15:12:13 2024, max compression
```

## Comparing `maslib-0.2.0.tar` & `maslib-0.2.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 07:34:22.874000 maslib-0.2.0/
--rw-rw-rw-   0        0        0       19 2024-05-18 17:23:43.000000 maslib-0.2.0/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-29 07:34:22.851265 maslib-0.2.0/MasLib/
--rw-rw-rw-   0        0        0     1971 2024-05-29 07:32:45.000000 maslib-0.2.0/MasLib/__init__.py
--rw-rw-rw-   0        0        0    19758 2024-05-26 09:46:27.000000 maslib-0.2.0/MasLib/classification.py
--rw-rw-rw-   0        0        0    10049 2024-05-26 09:34:23.000000 maslib-0.2.0/MasLib/clustering.py
--rw-rw-rw-   0        0        0     1820 2024-05-26 09:28:23.000000 maslib-0.2.0/MasLib/correlation.py
--rw-rw-rw-   0        0        0     3677 2024-05-26 09:52:52.000000 maslib-0.2.0/MasLib/encoding.py
--rw-rw-rw-   0        0        0      563 2024-05-26 09:24:37.000000 maslib-0.2.0/MasLib/loading.py
--rw-rw-rw-   0        0        0    10025 2024-05-26 09:23:11.000000 maslib-0.2.0/MasLib/regressions.py
--rw-rw-rw-   0        0        0    17434 2024-05-29 07:29:01.000000 maslib-0.2.0/MasLib/sql.py
--rw-rw-rw-   0        0        0    10975 2024-05-26 16:48:13.000000 maslib-0.2.0/MasLib/text_coding.py
-drwxrwxrwx   0        0        0        0 2024-05-29 07:34:22.871999 maslib-0.2.0/Maslib.egg-info/
--rw-rw-rw-   0        0        0     1057 2024-05-29 07:34:22.000000 maslib-0.2.0/Maslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      534 2024-05-29 07:34:22.000000 maslib-0.2.0/Maslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 07:34:22.000000 maslib-0.2.0/Maslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      135 2024-05-29 07:34:22.000000 maslib-0.2.0/Maslib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-29 07:34:22.000000 maslib-0.2.0/Maslib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1057 2024-05-29 07:34:22.872999 maslib-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      313 2024-05-29 07:33:41.000000 maslib-0.2.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-29 07:34:22.874000 maslib-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      908 2024-05-29 07:30:00.000000 maslib-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-29 07:34:22.869996 maslib-0.2.0/tests/
--rw-rw-rw-   0        0        0     1604 2024-05-19 12:47:10.000000 maslib-0.2.0/tests/test_clustering.py
--rw-rw-rw-   0        0        0     1419 2024-05-18 17:23:43.000000 maslib-0.2.0/tests/test_correlation.py
--rw-rw-rw-   0        0        0     1477 2024-05-18 17:23:43.000000 maslib-0.2.0/tests/test_encoding.py
--rw-rw-rw-   0        0        0     2625 2024-05-18 17:23:43.000000 maslib-0.2.0/tests/test_grid_search.py
--rw-rw-rw-   0        0        0      424 2024-05-19 12:45:36.000000 maslib-0.2.0/tests/test_loading.py
--rw-rw-rw-   0        0        0     2323 2024-05-19 11:18:27.000000 maslib-0.2.0/tests/test_regression.py
--rw-rw-rw-   0        0        0     1438 2024-05-19 12:44:54.000000 maslib-0.2.0/tests/test_text_coding.py
+drwxrwxrwx   0        0        0        0 2024-05-30 15:12:13.477172 maslib-0.2.1/
+-rw-rw-rw-   0        0        0       19 2024-05-18 17:23:43.000000 maslib-0.2.1/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-30 15:12:13.459156 maslib-0.2.1/MasLib/
+-rw-rw-rw-   0        0        0     2051 2024-05-30 15:03:58.000000 maslib-0.2.1/MasLib/__init__.py
+-rw-rw-rw-   0        0        0    19758 2024-05-26 09:46:27.000000 maslib-0.2.1/MasLib/classification.py
+-rw-rw-rw-   0        0        0    10049 2024-05-26 09:34:23.000000 maslib-0.2.1/MasLib/clustering.py
+-rw-rw-rw-   0        0        0     1820 2024-05-26 09:28:23.000000 maslib-0.2.1/MasLib/correlation.py
+-rw-rw-rw-   0        0        0     3677 2024-05-26 09:52:52.000000 maslib-0.2.1/MasLib/encoding.py
+-rw-rw-rw-   0        0        0     3759 2024-05-30 15:10:33.000000 maslib-0.2.1/MasLib/loading.py
+-rw-rw-rw-   0        0        0    10025 2024-05-26 09:23:11.000000 maslib-0.2.1/MasLib/regressions.py
+-rw-rw-rw-   0        0        0    17419 2024-05-30 14:09:04.000000 maslib-0.2.1/MasLib/sql.py
+-rw-rw-rw-   0        0        0    10975 2024-05-26 16:48:13.000000 maslib-0.2.1/MasLib/text_coding.py
+drwxrwxrwx   0        0        0        0 2024-05-30 15:12:13.475170 maslib-0.2.1/Maslib.egg-info/
+-rw-rw-rw-   0        0        0     1154 2024-05-30 15:12:12.000000 maslib-0.2.1/Maslib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      534 2024-05-30 15:12:13.000000 maslib-0.2.1/Maslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 15:12:12.000000 maslib-0.2.1/Maslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      168 2024-05-30 15:12:12.000000 maslib-0.2.1/Maslib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-30 15:12:13.000000 maslib-0.2.1/Maslib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1154 2024-05-30 15:12:13.476171 maslib-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2024-05-29 07:33:41.000000 maslib-0.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-30 15:12:13.477172 maslib-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      989 2024-05-30 15:10:26.000000 maslib-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 15:12:13.473169 maslib-0.2.1/tests/
+-rw-rw-rw-   0        0        0     1604 2024-05-19 12:47:10.000000 maslib-0.2.1/tests/test_clustering.py
+-rw-rw-rw-   0        0        0     1419 2024-05-18 17:23:43.000000 maslib-0.2.1/tests/test_correlation.py
+-rw-rw-rw-   0        0        0     1477 2024-05-18 17:23:43.000000 maslib-0.2.1/tests/test_encoding.py
+-rw-rw-rw-   0        0        0     2625 2024-05-18 17:23:43.000000 maslib-0.2.1/tests/test_grid_search.py
+-rw-rw-rw-   0        0        0      424 2024-05-19 12:45:36.000000 maslib-0.2.1/tests/test_loading.py
+-rw-rw-rw-   0        0        0     2323 2024-05-19 11:18:27.000000 maslib-0.2.1/tests/test_regression.py
+-rw-rw-rw-   0        0        0     1438 2024-05-19 12:44:54.000000 maslib-0.2.1/tests/test_text_coding.py
```

### Comparing `maslib-0.2.0/MasLib/__init__.py` & `maslib-0.2.1/MasLib/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 from .classification import print_metrics, classification_with_svc, classification_with_random_forest, classification_with_knn, classification_with_logistic_regression, classification_with_naive_bayes, classification_with_decision_tree, classification_with_gradient_boosting, classification_with_adaboost,  optimize_svc, optimize_random_forest, optimize_knn, optimize_logistic_regression, optimize_naive_bayes, optimize_decision_tree, optimize_gradient_boosting, optimize_adaboost, grid_search_optimization
 from .clustering import scale_data, kmeans_clustering, hierarchical_clustering, dbscan_clustering, birch_clustering, mean_shift_clustering, spectral_clustering, affinity_propagation_clustering, calculate_metrics, plot_clusters, ClusteringModel, optimize_clustering
 from .correlation import compute_phik_matrix, plot_phik_correlation_matrix
 from .encoding import number_encode_features, process_column_and_merge, json_to_dataframe
-from .loading import save_model
+from .loading import save_model, read_file,read_tskv,read_xml,read_yaml,read_avro,read_orc,read_pickle,read_pdf
 from .regressions import gb_regression, rf_regression, lr_regression, catboost_regression, xgb_regression, cross_val_evaluate, optimize_model
 from .text_coding import preprocess_text, vectorize_text, tfidf_vectorize_texts, lda_model, nmf_model, lsa_model, elbow_method_tfidf, sentiment_analysis, lda_topic_modeling
 from .sql import add_postgresql_record,delete_postgresql_record,update_postgresql_record,clean_postgresql_data,fetch_postgresql_to_dataframe,add_mongodb_record,delete_mongodb_record,update_mongodb_record,fetch_mongodb_to_dataframe,add_mysql_record,delete_mysql_record,update_mysql_record,clean_mysql_data,fetch_mysql_to_dataframe,add_sqlite_record,delete_sqlite_record,update_sqlite_record,clean_sqlite_data,fetch_sqlite_to_dataframe,add_mssql_record,delete_mssql_record,update_mssql_record,clean_mssql_data,fetch_mssql_to_dataframe,load_csv_to_dataframe,load_json_to_dataframe,dataframe_to_postgresql,dataframe_to_mongodb,dataframe_to_mysql,dataframe_to_sqlite,dataframe_to_mssql
```

### Comparing `maslib-0.2.0/MasLib/classification.py` & `maslib-0.2.1/MasLib/classification.py`

 * *Files identical despite different names*

### Comparing `maslib-0.2.0/MasLib/clustering.py` & `maslib-0.2.1/MasLib/clustering.py`

 * *Files identical despite different names*

### Comparing `maslib-0.2.0/MasLib/correlation.py` & `maslib-0.2.1/MasLib/correlation.py`

 * *Files identical despite different names*

### Comparing `maslib-0.2.0/MasLib/encoding.py` & `maslib-0.2.1/MasLib/encoding.py`

 * *Files identical despite different names*

### Comparing `maslib-0.2.0/MasLib/regressions.py` & `maslib-0.2.1/MasLib/regressions.py`

 * *Files identical despite different names*

### Comparing `maslib-0.2.0/MasLib/sql.py` & `maslib-0.2.1/MasLib/sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import psycopg2
 from pymongo import MongoClient
 import mysql.connector
 import sqlite3
-import pyodbc
 import pandas as pd
 
 # PostgreSQL functions
 def add_postgresql_record(conn, table, data):
     """
     Eng: Adds a record to the PostgreSQL table.
     Fra: Ajoute un enregistrement à la table PostgreSQL.
```

### Comparing `maslib-0.2.0/MasLib/text_coding.py` & `maslib-0.2.1/MasLib/text_coding.py`

 * *Files identical despite different names*

### Comparing `maslib-0.2.0/Maslib.egg-info/SOURCES.txt` & `maslib-0.2.1/Maslib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `maslib-0.2.0/setup.py` & `maslib-0.2.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Maslib',
-    version='0.2.0',
+    version='0.2.1',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'pandas',
         'phik',
         'matplotlib',
         'scikit-learn',
@@ -14,15 +14,19 @@
         'joblib',
         'wordcloud',
         'xgboost',
         'nltk',
         'pyodbc',
         'mysql-connector-python',
         'pymongo',
-        'psycopg2-binary'
+        'psycopg2-binary',
+        'PyYAML',
+        'fastavro',
+        'pyorc',
+        'pdfplumber'
 
     ],
     author='Alecsandr_C.V.V',
     author_email='dxomko@gmail.com',
     description='This is a library for optimizing code for python',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

### Comparing `maslib-0.2.0/tests/test_clustering.py` & `maslib-0.2.1/tests/test_clustering.py`

 * *Files identical despite different names*

### Comparing `maslib-0.2.0/tests/test_correlation.py` & `maslib-0.2.1/tests/test_correlation.py`

 * *Files identical despite different names*

### Comparing `maslib-0.2.0/tests/test_encoding.py` & `maslib-0.2.1/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `maslib-0.2.0/tests/test_grid_search.py` & `maslib-0.2.1/tests/test_grid_search.py`

 * *Files identical despite different names*

### Comparing `maslib-0.2.0/tests/test_regression.py` & `maslib-0.2.1/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `maslib-0.2.0/tests/test_text_coding.py` & `maslib-0.2.1/tests/test_text_coding.py`

 * *Files identical despite different names*

