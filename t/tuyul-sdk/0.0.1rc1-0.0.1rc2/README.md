# Comparing `tmp/tuyul_sdk-0.0.1rc1.tar.gz` & `tmp/tuyul_sdk-0.0.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuyul_sdk-0.0.1rc1.tar", max compression
+gzip compressed data, was "tuyul_sdk-0.0.1rc2.tar", max compression
```

## Comparing `tuyul_sdk-0.0.1rc1.tar` & `tuyul_sdk-0.0.1rc2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      608 2024-05-30 02:36:02.333454 tuyul_sdk-0.0.1rc1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-30 00:34:07.019714 tuyul_sdk-0.0.1rc1/README.md
--rw-r--r--   0        0        0      696 2024-05-30 02:34:35.462134 tuyul_sdk-0.0.1rc1/tuyul_sdk/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 20:21:44.103798 tuyul_sdk-0.0.1rc1/tuyul_sdk/_certificate/__init__.py
--rw-r--r--   0        0        0   286252 2024-03-18 20:21:44.105798 tuyul_sdk-0.0.1rc1/tuyul_sdk/_certificate/cacert.pem
--rw-r--r--   0        0        0     8658 2024-05-30 02:19:24.831329 tuyul_sdk-0.0.1rc1/tuyul_sdk/_Cipher.py
--rw-r--r--   0        0        0      454 2024-03-30 18:29:45.577779 tuyul_sdk-0.0.1rc1/tuyul_sdk/_Color.py
--rw-r--r--   0        0        0     6587 2024-05-30 02:39:05.441826 tuyul_sdk-0.0.1rc1/tuyul_sdk/_Connection.py
--rw-r--r--   0        0        0     2190 2024-05-30 00:51:02.899443 tuyul_sdk-0.0.1rc1/tuyul_sdk/_Database.py
--rw-r--r--   0        0        0      509 2024-03-18 20:21:43.622544 tuyul_sdk-0.0.1rc1/tuyul_sdk/_input.py
--rw-r--r--   0        0        0      719 2024-03-18 20:21:43.623543 tuyul_sdk-0.0.1rc1/tuyul_sdk/_Line.py
--rw-r--r--   0        0        0      826 2024-05-26 07:36:03.091067 tuyul_sdk-0.0.1rc1/tuyul_sdk/_Log.py
--rw-r--r--   0        0        0     2373 2024-05-26 07:35:32.143357 tuyul_sdk-0.0.1rc1/tuyul_sdk/_Progress.py
--rw-r--r--   0        0        0      229 2024-05-26 07:33:25.053372 tuyul_sdk-0.0.1rc1/tuyul_sdk/_Reset.py
--rw-r--r--   0        0        0     3000 2024-05-26 07:32:31.114228 tuyul_sdk-0.0.1rc1/tuyul_sdk/_UserAgent.py
--rw-r--r--   0        0        0       93 2024-05-30 02:34:28.449126 tuyul_sdk-0.0.1rc1/tuyul_sdk/sql.py
--rw-r--r--   0        0        0      909 1970-01-01 00:00:00.000000 tuyul_sdk-0.0.1rc1/setup.py
--rw-r--r--   0        0        0      881 1970-01-01 00:00:00.000000 tuyul_sdk-0.0.1rc1/PKG-INFO
+-rw-r--r--   0        0        0      608 2024-05-30 03:42:23.751006 tuyul_sdk-0.0.1rc2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-30 00:34:07.019714 tuyul_sdk-0.0.1rc2/README.md
+-rw-r--r--   0        0        0      735 2024-05-30 03:42:18.398424 tuyul_sdk-0.0.1rc2/tuyul_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-18 20:21:44.103798 tuyul_sdk-0.0.1rc2/tuyul_sdk/_certificate/__init__.py
+-rw-r--r--   0        0        0   286252 2024-03-18 20:21:44.105798 tuyul_sdk-0.0.1rc2/tuyul_sdk/_certificate/cacert.pem
+-rw-r--r--   0        0        0     8658 2024-05-30 02:19:24.831329 tuyul_sdk-0.0.1rc2/tuyul_sdk/_Cipher.py
+-rw-r--r--   0        0        0      454 2024-03-30 18:29:45.577779 tuyul_sdk-0.0.1rc2/tuyul_sdk/_Color.py
+-rw-r--r--   0        0        0     6587 2024-05-30 02:39:05.441826 tuyul_sdk-0.0.1rc2/tuyul_sdk/_Connection.py
+-rw-r--r--   0        0        0     2574 2024-05-30 03:44:10.366863 tuyul_sdk-0.0.1rc2/tuyul_sdk/_Database.py
+-rw-r--r--   0        0        0      509 2024-03-18 20:21:43.622544 tuyul_sdk-0.0.1rc2/tuyul_sdk/_input.py
+-rw-r--r--   0        0        0      719 2024-03-18 20:21:43.623543 tuyul_sdk-0.0.1rc2/tuyul_sdk/_Line.py
+-rw-r--r--   0        0        0      826 2024-05-26 07:36:03.091067 tuyul_sdk-0.0.1rc2/tuyul_sdk/_Log.py
+-rw-r--r--   0        0        0     2373 2024-05-26 07:35:32.143357 tuyul_sdk-0.0.1rc2/tuyul_sdk/_Progress.py
+-rw-r--r--   0        0        0      229 2024-05-26 07:33:25.053372 tuyul_sdk-0.0.1rc2/tuyul_sdk/_Reset.py
+-rw-r--r--   0        0        0     3000 2024-05-26 07:32:31.114228 tuyul_sdk-0.0.1rc2/tuyul_sdk/_UserAgent.py
+-rw-r--r--   0        0        0       93 2024-05-30 02:34:28.449126 tuyul_sdk-0.0.1rc2/tuyul_sdk/sql.py
+-rw-r--r--   0        0        0      909 1970-01-01 00:00:00.000000 tuyul_sdk-0.0.1rc2/setup.py
+-rw-r--r--   0        0        0      881 1970-01-01 00:00:00.000000 tuyul_sdk-0.0.1rc2/PKG-INFO
```

### Comparing `tuyul_sdk-0.0.1rc1/pyproject.toml` & `tuyul_sdk-0.0.1rc2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tuyul-sdk"
-version = "0.0.1rc1"
+version = "0.0.1rc2"
 description = ""
 authors = ["Antoni Oktha Fernandes <37358597+DesKaOne@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "tuyul_sdk"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `tuyul_sdk-0.0.1rc1/tuyul_sdk/__init__.py` & `tuyul_sdk-0.0.1rc2/tuyul_sdk/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from ._Color import Color
 from ._input import Input
 from ._Line import Line
 from ._Log import Log
 from ._Progress import ProgressBar, ProgressWait
 from ._Reset import Reset
 from ._UserAgent import UserAgent
-from ._Database import Database
+from ._Database import Database, TypeConnection
 Reset()
 import importlib.metadata
 version = importlib.metadata.version('tuyul_sdk')
 from ._Cipher import AES, Password, Salt
 from ._Connection import Connections, ProxyParams, ProxyType, TypeInjector
 
 __all__ = [
@@ -22,9 +22,10 @@
     'UserAgent',
     'AES',
     'Password',
     'Salt',
     'Connections',
     'ProxyParams',
     'ProxyType',
-    'Database'
+    'Database',
+    'TypeConnection'
 ]
```

### Comparing `tuyul_sdk-0.0.1rc1/tuyul_sdk/_certificate/cacert.pem` & `tuyul_sdk-0.0.1rc2/tuyul_sdk/_certificate/cacert.pem`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.0.1rc1/tuyul_sdk/_Cipher.py` & `tuyul_sdk-0.0.1rc2/tuyul_sdk/_Cipher.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.0.1rc1/tuyul_sdk/_Connection.py` & `tuyul_sdk-0.0.1rc2/tuyul_sdk/_Connection.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.0.1rc1/tuyul_sdk/_Database.py` & `tuyul_sdk-0.0.1rc2/tuyul_sdk/_Database.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,42 @@
+from enum import Enum, auto
 import os
 from typing import Union
 from sqlalchemy.orm import declarative_base
 from sqlalchemy.orm import sessionmaker, Session
 from sqlalchemy.orm.decl_api import DeclarativeMeta
 from sqlalchemy import create_engine, MetaData
 from sqlalchemy_utils import database_exists, create_database
 
+class TypeConnection(Enum):
+    
+    ONLINE  = auto()
+    OFFLINE = auto()
+    HIDDEN  = auto()
+
 class Database:
 
     @property
     def declarative(self) -> DeclarativeMeta:
         return declarative_base()
 
     class Connection:
 
         FileName: Union[str, None] = None
+        Type: Union[TypeConnection, None] = None
 
         @classmethod
         def BaseMetaData(cls, declarative: DeclarativeMeta) -> MetaData:
             return declarative.metadata
         
         def __init__(self) -> None:
-            if os.getenv('METHOD').upper() == 'ONLINE':
+            if self.Type == TypeConnection.ONLINE:
                 DATABASE_URI = str(os.getenv('DATABASE_URI'))
             if self.FileName is not None:
-                if os.getenv('METHOD').upper() == 'HIDDEN':
+                if self.Type == TypeConnection.HIDDEN:
                     Path = '{}/Database'.format(os.path.dirname(__file__))
                     if os.path.exists(Path) is False: os.mkdir(Path)
                     DATABASE_URI = 'sqlite:///{}/{}.sqlite'.format(Path, self.FileName)
                 else:
                     if os.path.exists('Database') is False: os.mkdir('Database')
                     DATABASE_URI = 'sqlite:///Database/{}.sqlite'.format(self.FileName)
             else:
@@ -39,15 +47,19 @@
             return self.Engine.connect()
 
         def Session(self) -> Session:
             Session = sessionmaker(bind=self.Engine)
             return Session()
 
         @staticmethod
-        def build(declarative: DeclarativeMeta, FileName: str = None):
+        def build(declarative: DeclarativeMeta, Type: TypeConnection = None, FileName: str = None):
             if FileName is not None:
                 setattr(Database.Connection, 'FileName', FileName)
+            if not Type:
+                setattr(Database.Connection, 'Type', TypeConnection.OFFLINE)
+            else:
+                setattr(Database.Connection, 'Type', Type)
             Conn = Database.Connection()
             if not database_exists(Conn.Engine.url):
                 create_database(Conn.Engine.url)
                 Conn.BaseMetaData(declarative).create_all(Conn.Engine)
             return Conn
```

### Comparing `tuyul_sdk-0.0.1rc1/tuyul_sdk/_Line.py` & `tuyul_sdk-0.0.1rc2/tuyul_sdk/_Line.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.0.1rc1/tuyul_sdk/_Log.py` & `tuyul_sdk-0.0.1rc2/tuyul_sdk/_Log.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.0.1rc1/tuyul_sdk/_Progress.py` & `tuyul_sdk-0.0.1rc2/tuyul_sdk/_Progress.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.0.1rc1/tuyul_sdk/_UserAgent.py` & `tuyul_sdk-0.0.1rc2/tuyul_sdk/_UserAgent.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.0.1rc1/setup.py` & `tuyul_sdk-0.0.1rc2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'random-user-agent>=1.0.1,<2.0.0',
  'requests>=2.32.3,<3.0.0',
  'sqlalchemy-utils>=0.41.2,<0.42.0',
  'sqlalchemy>=2.0.30,<3.0.0']
 
 setup_kwargs = {
     'name': 'tuyul-sdk',
-    'version': '0.0.1rc1',
+    'version': '0.0.1rc2',
     'description': '',
     'long_description': '',
     'author': 'Antoni Oktha Fernandes',
     'author_email': '37358597+DesKaOne@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `tuyul_sdk-0.0.1rc1/PKG-INFO` & `tuyul_sdk-0.0.1rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuyul-sdk
-Version: 0.0.1rc1
+Version: 0.0.1rc2
 Summary: 
 Author: Antoni Oktha Fernandes
 Author-email: 37358597+DesKaOne@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

