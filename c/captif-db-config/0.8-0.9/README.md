# Comparing `tmp/captif-db-config-0.8.tar.gz` & `tmp/captif-db-config-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "captif-db-config-0.8.tar", max compression
+gzip compressed data, was "captif-db-config-0.9.tar", max compression
```

## Comparing `captif-db-config-0.8.tar` & `captif-db-config-0.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1063 2021-06-15 03:04:34.996240 captif-db-config-0.8/LICENSE
--rw-r--r--   0        0        0      275 2021-06-15 03:04:34.996240 captif-db-config-0.8/README.md
--rw-r--r--   0        0        0     3059 2021-06-15 03:04:34.996240 captif-db-config-0.8/captif_db_config/__init__.py
--rw-r--r--   0        0        0      429 2021-06-15 03:04:34.996240 captif-db-config-0.8/pyproject.toml
--rw-r--r--   0        0        0      963 2021-06-15 03:04:45.923202 captif-db-config-0.8/setup.py
--rw-r--r--   0        0        0      886 2021-06-15 03:04:45.923495 captif-db-config-0.8/PKG-INFO
+-rw-r--r--   0        0        0     1063 2021-06-15 03:50:14.681179 captif-db-config-0.9/LICENSE
+-rw-r--r--   0        0        0      275 2021-06-15 03:50:14.681179 captif-db-config-0.9/README.md
+-rw-r--r--   0        0        0     3205 2021-06-15 03:50:14.681179 captif-db-config-0.9/captif_db_config/__init__.py
+-rw-r--r--   0        0        0      429 2021-06-15 03:50:14.681179 captif-db-config-0.9/pyproject.toml
+-rw-r--r--   0        0        0      963 2021-06-15 03:50:23.451352 captif-db-config-0.9/setup.py
+-rw-r--r--   0        0        0      886 2021-06-15 03:50:23.451636 captif-db-config-0.9/PKG-INFO
```

### Comparing `captif-db-config-0.8/LICENSE` & `captif-db-config-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `captif-db-config-0.8/captif_db_config/__init__.py` & `captif-db-config-0.9/captif_db_config/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8"
+__version__ = "0.9"
 
 import os
 from configparser import ConfigParser
 from pathlib import Path
 from sqlalchemy import create_engine
 from sqlalchemy.engine.url import URL
 from sqlalchemy.orm import sessionmaker
@@ -47,17 +47,17 @@
 class Config:
 
     HOST = get_config_param("host")
     PORT = get_config_param("port")
     USERNAME = get_config_param("username")
     PASSWORD = get_config_param("password")
 
-    SSL_CA = get_config_param("ssl_ca")
-    SSL_CERT = get_config_param("ssl_cert")
-    SSL_KEY = get_config_param("ssl_key")
+    SSL_CA = get_config_param("ssl_ca", raise_exception=False)
+    SSL_CERT = get_config_param("ssl_cert", raise_exception=False)
+    SSL_KEY = get_config_param("ssl_key", raise_exception=False)
 
     @classmethod
     def database_connection_str(cls, database):
         return URL.create(
             drivername=DRIVERNAME,
             username=cls.USERNAME,
             password=cls.PASSWORD,
@@ -65,19 +65,20 @@
             port=cls.PORT,
             database=database,
             query=cls.ssl_args(),
         )
 
     @classmethod
     def ssl_args(cls):
-        return {
+        ssl_dict = {
             "ssl_ca": cls.SSL_CA,
             "ssl_cert": cls.SSL_CERT,
             "ssl_key": cls.SSL_KEY,
         }
+        return {kk: vv for kk, vv in ssl_dict.items() if vv is not None}
 
 
 class DbSession:
     database = None  # Database name
     base = None  # SQLAlchemy Base object
     factory = None
     engine = None
```

### Comparing `captif-db-config-0.8/setup.py` & `captif-db-config-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['mysqlclient>=2.0.3,<3.0.0',
  'sqlalchemy-utils>=0.37.2,<0.38.0',
  'sqlalchemy>=1.4.15,<2.0.0']
 
 setup_kwargs = {
     'name': 'captif-db-config',
-    'version': '0.8',
+    'version': '0.9',
     'description': '',
     'long_description': '# captif-db-config\n\nDatabase configuration.\n\n\n## Config file\n\nPlace a `.captif-db.ini` file in the home directory (`~` on linux). The config file should contain the following information:\n\n```\n[GENERAL]\nhost =\nport =\nusername = \npassword = \nssl_ca =\nssl_cert =\nssl_key =\n```\n',
     'author': 'John Bull',
     'author_email': 'john.bull@nzta.govt.nz',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `captif-db-config-0.8/PKG-INFO` & `captif-db-config-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: captif-db-config
-Version: 0.8
+Version: 0.9
 Summary: 
 License: MIT
 Keywords: CAPTIF
 Author: John Bull
 Author-email: john.bull@nzta.govt.nz
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

