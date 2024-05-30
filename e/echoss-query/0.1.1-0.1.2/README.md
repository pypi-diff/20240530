# Comparing `tmp/echoss_query-0.1.1.tar.gz` & `tmp/echoss_query-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echoss_query-0.1.1.tar", last modified: Tue May 28 06:28:08 2024, max compression
+gzip compressed data, was "echoss_query-0.1.2.tar", last modified: Thu May 30 07:01:03 2024, max compression
```

## Comparing `echoss_query-0.1.1.tar` & `echoss_query-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 sin-incheol   (501) staff       (20)        0 2024-05-28 06:28:08.508176 echoss_query-0.1.1/
--rw-r--r--   0 sin-incheol   (501) staff       (20)     2820 2024-05-28 06:28:08.507675 echoss_query-0.1.1/PKG-INFO
--rw-r--r--   0 sin-incheol   (501) staff       (20)     2427 2024-05-28 05:52:53.000000 echoss_query-0.1.1/README.md
-drwxr-xr-x   0 sin-incheol   (501) staff       (20)        0 2024-05-28 06:28:08.502394 echoss_query-0.1.1/echoss_query/
--rw-r--r--   0 sin-incheol   (501) staff       (20)      180 2024-05-28 05:52:53.000000 echoss_query-0.1.1/echoss_query/__init__.py
-drwxr-xr-x   0 sin-incheol   (501) staff       (20)        0 2024-05-28 06:28:08.506761 echoss_query-0.1.1/echoss_query/query/
--rw-r--r--   0 sin-incheol   (501) staff       (20)        0 2024-05-28 05:52:53.000000 echoss_query-0.1.1/echoss_query/query/__init__.py
--rw-r--r--   0 sin-incheol   (501) staff       (20)    26208 2024-05-28 05:53:49.000000 echoss_query-0.1.1/echoss_query/query/echoss_query.py
-drwxr-xr-x   0 sin-incheol   (501) staff       (20)        0 2024-05-28 06:28:08.505738 echoss_query-0.1.1/echoss_query.egg-info/
--rw-r--r--   0 sin-incheol   (501) staff       (20)     2820 2024-05-28 06:28:08.000000 echoss_query-0.1.1/echoss_query.egg-info/PKG-INFO
--rw-r--r--   0 sin-incheol   (501) staff       (20)      288 2024-05-28 06:28:08.000000 echoss_query-0.1.1/echoss_query.egg-info/SOURCES.txt
--rw-r--r--   0 sin-incheol   (501) staff       (20)        1 2024-05-28 06:28:08.000000 echoss_query-0.1.1/echoss_query.egg-info/dependency_links.txt
--rw-r--r--   0 sin-incheol   (501) staff       (20)       77 2024-05-28 06:28:08.000000 echoss_query-0.1.1/echoss_query.egg-info/requires.txt
--rw-r--r--   0 sin-incheol   (501) staff       (20)       13 2024-05-28 06:28:08.000000 echoss_query-0.1.1/echoss_query.egg-info/top_level.txt
--rw-r--r--   0 sin-incheol   (501) staff       (20)       38 2024-05-28 06:28:08.508304 echoss_query-0.1.1/setup.cfg
--rw-r--r--   0 sin-incheol   (501) staff       (20)      689 2024-05-28 06:27:58.000000 echoss_query-0.1.1/setup.py
+drwxr-xr-x   0 sin-incheol   (501) staff       (20)        0 2024-05-30 07:01:03.317550 echoss_query-0.1.2/
+-rw-r--r--   0 sin-incheol   (501) staff       (20)     2820 2024-05-30 07:01:03.317101 echoss_query-0.1.2/PKG-INFO
+-rw-r--r--   0 sin-incheol   (501) staff       (20)     2427 2024-05-30 06:58:57.000000 echoss_query-0.1.2/README.md
+drwxr-xr-x   0 sin-incheol   (501) staff       (20)        0 2024-05-30 07:01:03.312955 echoss_query-0.1.2/echoss_query/
+-rw-r--r--   0 sin-incheol   (501) staff       (20)      180 2024-05-28 05:52:53.000000 echoss_query-0.1.2/echoss_query/__init__.py
+drwxr-xr-x   0 sin-incheol   (501) staff       (20)        0 2024-05-30 07:01:03.316294 echoss_query-0.1.2/echoss_query/query/
+-rw-r--r--   0 sin-incheol   (501) staff       (20)        0 2024-05-28 05:52:53.000000 echoss_query-0.1.2/echoss_query/query/__init__.py
+-rw-r--r--   0 sin-incheol   (501) staff       (20)     3291 2024-05-30 06:45:03.000000 echoss_query-0.1.2/echoss_query/query/echoss_logger.py
+-rw-r--r--   0 sin-incheol   (501) staff       (20)    24330 2024-05-30 06:56:35.000000 echoss_query-0.1.2/echoss_query/query/echoss_query.py
+drwxr-xr-x   0 sin-incheol   (501) staff       (20)        0 2024-05-30 07:01:03.314967 echoss_query-0.1.2/echoss_query.egg-info/
+-rw-r--r--   0 sin-incheol   (501) staff       (20)     2820 2024-05-30 07:01:03.000000 echoss_query-0.1.2/echoss_query.egg-info/PKG-INFO
+-rw-r--r--   0 sin-incheol   (501) staff       (20)      324 2024-05-30 07:01:03.000000 echoss_query-0.1.2/echoss_query.egg-info/SOURCES.txt
+-rw-r--r--   0 sin-incheol   (501) staff       (20)        1 2024-05-30 07:01:03.000000 echoss_query-0.1.2/echoss_query.egg-info/dependency_links.txt
+-rw-r--r--   0 sin-incheol   (501) staff       (20)       77 2024-05-30 07:01:03.000000 echoss_query-0.1.2/echoss_query.egg-info/requires.txt
+-rw-r--r--   0 sin-incheol   (501) staff       (20)       13 2024-05-30 07:01:03.000000 echoss_query-0.1.2/echoss_query.egg-info/top_level.txt
+-rw-r--r--   0 sin-incheol   (501) staff       (20)       38 2024-05-30 07:01:03.317676 echoss_query-0.1.2/setup.cfg
+-rw-r--r--   0 sin-incheol   (501) staff       (20)      689 2024-05-30 06:57:59.000000 echoss_query-0.1.2/setup.py
```

### Comparing `echoss_query-0.1.1/PKG-INFO` & `echoss_query-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echoss_query
-Version: 0.1.1
+Version: 0.1.2
 Summary: echoss AI Bigdata Solution - Query Package
 Home-page: 
 Author: incheolshin
 Author-email: incheolshin@12cm.co.kr
 Requires-Python: >3.7
 Description-Content-Type: text/markdown
 Requires-Dist: pandas>=1.5.3
@@ -27,15 +27,15 @@
     cd ~/echoss_query
     pip install -r requirements.txt
 ```
 
 ### Quick Start
 -------------
 ```
-    from echoss_query.query import MysqlQuery, MongoQuery, ElasticSearch
+    from echoss_query import MysqlQuery, MongoQuery, ElasticSearch
 
     mysql = MysqlQuery('CONFIG_FILE_PATH' or dict)
     mongo = MongoQuery('CONFIG_FILE_PATH' or dict)
     elastic = ElasticSearch('CONFIG_FILE_PATH' or dict)
 
 
     #CREATE
@@ -53,15 +53,15 @@
     mysql.alter('QUERY_STRING')
 
     #SELECT
 
     mysql.select('QUERY_STRING')
     mongo.select('COLLECTION_NAME','QUERY_STRING or DICTIONARY')
     elastic.get(id='ID')
-    elastic.search(field='FIELD_NAME',value='VALUE')
+    elastic.search_field(field='FIELD_NAME',value='VALUE')
 
     elastic.get_source(id='ID') #-> Extract Source
     mysql.faster_select('QUERY_STRING') #-> Use SSCursor
     mysql.select_list('QUERY_STRING') #-> list
 
     #INSERT
```

### Comparing `echoss_query-0.1.1/README.md` & `echoss_query-0.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     cd ~/echoss_query
     pip install -r requirements.txt
 ```
 
 ### Quick Start
 -------------
 ```
-    from echoss_query.query import MysqlQuery, MongoQuery, ElasticSearch
+    from echoss_query import MysqlQuery, MongoQuery, ElasticSearch
 
     mysql = MysqlQuery('CONFIG_FILE_PATH' or dict)
     mongo = MongoQuery('CONFIG_FILE_PATH' or dict)
     elastic = ElasticSearch('CONFIG_FILE_PATH' or dict)
 
 
     #CREATE
@@ -38,15 +38,15 @@
     mysql.alter('QUERY_STRING')
 
     #SELECT
 
     mysql.select('QUERY_STRING')
     mongo.select('COLLECTION_NAME','QUERY_STRING or DICTIONARY')
     elastic.get(id='ID')
-    elastic.search(field='FIELD_NAME',value='VALUE')
+    elastic.search_field(field='FIELD_NAME',value='VALUE')
 
     elastic.get_source(id='ID') #-> Extract Source
     mysql.faster_select('QUERY_STRING') #-> Use SSCursor
     mysql.select_list('QUERY_STRING') #-> list
 
     #INSERT
```

### Comparing `echoss_query-0.1.1/echoss_query.egg-info/PKG-INFO` & `echoss_query-0.1.2/echoss_query.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echoss-query
-Version: 0.1.1
+Version: 0.1.2
 Summary: echoss AI Bigdata Solution - Query Package
 Home-page: 
 Author: incheolshin
 Author-email: incheolshin@12cm.co.kr
 Requires-Python: >3.7
 Description-Content-Type: text/markdown
 Requires-Dist: pandas>=1.5.3
@@ -27,15 +27,15 @@
     cd ~/echoss_query
     pip install -r requirements.txt
 ```
 
 ### Quick Start
 -------------
 ```
-    from echoss_query.query import MysqlQuery, MongoQuery, ElasticSearch
+    from echoss_query import MysqlQuery, MongoQuery, ElasticSearch
 
     mysql = MysqlQuery('CONFIG_FILE_PATH' or dict)
     mongo = MongoQuery('CONFIG_FILE_PATH' or dict)
     elastic = ElasticSearch('CONFIG_FILE_PATH' or dict)
 
 
     #CREATE
@@ -53,15 +53,15 @@
     mysql.alter('QUERY_STRING')
 
     #SELECT
 
     mysql.select('QUERY_STRING')
     mongo.select('COLLECTION_NAME','QUERY_STRING or DICTIONARY')
     elastic.get(id='ID')
-    elastic.search(field='FIELD_NAME',value='VALUE')
+    elastic.search_field(field='FIELD_NAME',value='VALUE')
 
     elastic.get_source(id='ID') #-> Extract Source
     mysql.faster_select('QUERY_STRING') #-> Use SSCursor
     mysql.select_list('QUERY_STRING') #-> list
 
     #INSERT
```

### Comparing `echoss_query-0.1.1/setup.py` & `echoss_query-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 package_name = "echoss_query"
 
 setup(
     name='echoss_query',
-    version='0.1.1',
+    version='0.1.2',
     url='',
     install_requires=[
         'pandas>=1.5.3',
         'pymongo>=4.3.3',
         'PyMySQL>=1.0.2',
         'PyYAML>=6.0',
         'opensearch-py>=2.2.0'
```

