# Comparing `tmp/tuyul_sdk-0.0.1rc2.tar.gz` & `tmp/tuyul_sdk-0.0.1rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuyul_sdk-0.0.1rc2.tar", max compression
+gzip compressed data, was "tuyul_sdk-0.0.1rc3.tar", max compression
```

## Comparing `tuyul_sdk-0.0.1rc2.tar` & `tuyul_sdk-0.0.1rc3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      608 2024-05-30 03:42:23.751006 tuyul_sdk-0.0.1rc2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-30 00:34:07.019714 tuyul_sdk-0.0.1rc2/README.md
--rw-r--r--   0        0        0      735 2024-05-30 03:42:18.398424 tuyul_sdk-0.0.1rc2/tuyul_sdk/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 20:21:44.103798 tuyul_sdk-0.0.1rc2/tuyul_sdk/_certificate/__init__.py
--rw-r--r--   0        0        0   286252 2024-03-18 20:21:44.105798 tuyul_sdk-0.0.1rc2/tuyul_sdk/_certificate/cacert.pem
--rw-r--r--   0        0        0     8658 2024-05-30 02:19:24.831329 tuyul_sdk-0.0.1rc2/tuyul_sdk/_Cipher.py
--rw-r--r--   0        0        0      454 2024-03-30 18:29:45.577779 tuyul_sdk-0.0.1rc2/tuyul_sdk/_Color.py
--rw-r--r--   0        0        0     6587 2024-05-30 02:39:05.441826 tuyul_sdk-0.0.1rc2/tuyul_sdk/_Connection.py
--rw-r--r--   0        0        0     2574 2024-05-30 03:44:10.366863 tuyul_sdk-0.0.1rc2/tuyul_sdk/_Database.py
--rw-r--r--   0        0        0      509 2024-03-18 20:21:43.622544 tuyul_sdk-0.0.1rc2/tuyul_sdk/_input.py
--rw-r--r--   0        0        0      719 2024-03-18 20:21:43.623543 tuyul_sdk-0.0.1rc2/tuyul_sdk/_Line.py
--rw-r--r--   0        0        0      826 2024-05-26 07:36:03.091067 tuyul_sdk-0.0.1rc2/tuyul_sdk/_Log.py
--rw-r--r--   0        0        0     2373 2024-05-26 07:35:32.143357 tuyul_sdk-0.0.1rc2/tuyul_sdk/_Progress.py
--rw-r--r--   0        0        0      229 2024-05-26 07:33:25.053372 tuyul_sdk-0.0.1rc2/tuyul_sdk/_Reset.py
--rw-r--r--   0        0        0     3000 2024-05-26 07:32:31.114228 tuyul_sdk-0.0.1rc2/tuyul_sdk/_UserAgent.py
--rw-r--r--   0        0        0       93 2024-05-30 02:34:28.449126 tuyul_sdk-0.0.1rc2/tuyul_sdk/sql.py
--rw-r--r--   0        0        0      909 1970-01-01 00:00:00.000000 tuyul_sdk-0.0.1rc2/setup.py
--rw-r--r--   0        0        0      881 1970-01-01 00:00:00.000000 tuyul_sdk-0.0.1rc2/PKG-INFO
+-rw-r--r--   0        0        0      608 2024-05-30 03:57:51.069736 tuyul_sdk-0.0.1rc3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-30 00:34:07.019714 tuyul_sdk-0.0.1rc3/README.md
+-rw-r--r--   0        0        0      735 2024-05-30 03:42:18.398424 tuyul_sdk-0.0.1rc3/tuyul_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-18 20:21:44.103798 tuyul_sdk-0.0.1rc3/tuyul_sdk/_certificate/__init__.py
+-rw-r--r--   0        0        0   286252 2024-03-18 20:21:44.105798 tuyul_sdk-0.0.1rc3/tuyul_sdk/_certificate/cacert.pem
+-rw-r--r--   0        0        0     8658 2024-05-30 02:19:24.831329 tuyul_sdk-0.0.1rc3/tuyul_sdk/_Cipher.py
+-rw-r--r--   0        0        0      454 2024-03-30 18:29:45.577779 tuyul_sdk-0.0.1rc3/tuyul_sdk/_Color.py
+-rw-r--r--   0        0        0     6587 2024-05-30 02:39:05.441826 tuyul_sdk-0.0.1rc3/tuyul_sdk/_Connection.py
+-rw-r--r--   0        0        0     2654 2024-05-30 03:57:45.352001 tuyul_sdk-0.0.1rc3/tuyul_sdk/_Database.py
+-rw-r--r--   0        0        0      509 2024-03-18 20:21:43.622544 tuyul_sdk-0.0.1rc3/tuyul_sdk/_input.py
+-rw-r--r--   0        0        0      719 2024-03-18 20:21:43.623543 tuyul_sdk-0.0.1rc3/tuyul_sdk/_Line.py
+-rw-r--r--   0        0        0      826 2024-05-26 07:36:03.091067 tuyul_sdk-0.0.1rc3/tuyul_sdk/_Log.py
+-rw-r--r--   0        0        0     2373 2024-05-26 07:35:32.143357 tuyul_sdk-0.0.1rc3/tuyul_sdk/_Progress.py
+-rw-r--r--   0        0        0      229 2024-05-26 07:33:25.053372 tuyul_sdk-0.0.1rc3/tuyul_sdk/_Reset.py
+-rw-r--r--   0        0        0     3000 2024-05-26 07:32:31.114228 tuyul_sdk-0.0.1rc3/tuyul_sdk/_UserAgent.py
+-rw-r--r--   0        0        0       93 2024-05-30 02:34:28.449126 tuyul_sdk-0.0.1rc3/tuyul_sdk/sql.py
+-rw-r--r--   0        0        0      909 1970-01-01 00:00:00.000000 tuyul_sdk-0.0.1rc3/setup.py
+-rw-r--r--   0        0        0      881 1970-01-01 00:00:00.000000 tuyul_sdk-0.0.1rc3/PKG-INFO
```

### Comparing `tuyul_sdk-0.0.1rc2/pyproject.toml` & `tuyul_sdk-0.0.1rc3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tuyul-sdk"
-version = "0.0.1rc2"
+version = "0.0.1rc3"
 description = ""
 authors = ["Antoni Oktha Fernandes <37358597+DesKaOne@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "tuyul_sdk"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `tuyul_sdk-0.0.1rc2/tuyul_sdk/__init__.py` & `tuyul_sdk-0.0.1rc3/tuyul_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.0.1rc2/tuyul_sdk/_certificate/cacert.pem` & `tuyul_sdk-0.0.1rc3/tuyul_sdk/_certificate/cacert.pem`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.0.1rc2/tuyul_sdk/_Cipher.py` & `tuyul_sdk-0.0.1rc3/tuyul_sdk/_Cipher.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.0.1rc2/tuyul_sdk/_Connection.py` & `tuyul_sdk-0.0.1rc3/tuyul_sdk/_Connection.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.0.1rc2/tuyul_sdk/_Database.py` & `tuyul_sdk-0.0.1rc3/tuyul_sdk/_Database.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,28 +18,28 @@
     @property
     def declarative(self) -> DeclarativeMeta:
         return declarative_base()
 
     class Connection:
 
         FileName: Union[str, None] = None
+        PathName: Union[str, None] = None
         Type: Union[TypeConnection, None] = None
 
         @classmethod
         def BaseMetaData(cls, declarative: DeclarativeMeta) -> MetaData:
             return declarative.metadata
         
         def __init__(self) -> None:
             if self.Type == TypeConnection.ONLINE:
                 DATABASE_URI = str(os.getenv('DATABASE_URI'))
             if self.FileName is not None:
                 if self.Type == TypeConnection.HIDDEN:
-                    Path = '{}/Database'.format(os.path.dirname(__file__))
-                    if os.path.exists(Path) is False: os.mkdir(Path)
-                    DATABASE_URI = 'sqlite:///{}/{}.sqlite'.format(Path, self.FileName)
+                    if os.path.exists(self.PathName) is False: os.mkdir(self.PathName)
+                    DATABASE_URI = 'sqlite:///{}/{}.sqlite'.format(self.PathName, self.FileName)
                 else:
                     if os.path.exists('Database') is False: os.mkdir('Database')
                     DATABASE_URI = 'sqlite:///Database/{}.sqlite'.format(self.FileName)
             else:
                 raise Exception('No filename provided for the Engine.\nPlease set command Engine.build({filename})')
             self.Engine = create_engine(DATABASE_URI, echo=False, pool_pre_ping=True)
 
@@ -47,15 +47,16 @@
             return self.Engine.connect()
 
         def Session(self) -> Session:
             Session = sessionmaker(bind=self.Engine)
             return Session()
 
         @staticmethod
-        def build(declarative: DeclarativeMeta, Type: TypeConnection = None, FileName: str = None):
+        def build(declarative: DeclarativeMeta, Type: TypeConnection = None, PathName: str = None, FileName: str = None):
+            setattr(Database.Connection, 'PathName', PathName)
             if FileName is not None:
                 setattr(Database.Connection, 'FileName', FileName)
             if not Type:
                 setattr(Database.Connection, 'Type', TypeConnection.OFFLINE)
             else:
                 setattr(Database.Connection, 'Type', Type)
             Conn = Database.Connection()
```

### Comparing `tuyul_sdk-0.0.1rc2/tuyul_sdk/_Line.py` & `tuyul_sdk-0.0.1rc3/tuyul_sdk/_Line.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.0.1rc2/tuyul_sdk/_Log.py` & `tuyul_sdk-0.0.1rc3/tuyul_sdk/_Log.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.0.1rc2/tuyul_sdk/_Progress.py` & `tuyul_sdk-0.0.1rc3/tuyul_sdk/_Progress.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.0.1rc2/tuyul_sdk/_UserAgent.py` & `tuyul_sdk-0.0.1rc3/tuyul_sdk/_UserAgent.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.0.1rc2/setup.py` & `tuyul_sdk-0.0.1rc3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'random-user-agent>=1.0.1,<2.0.0',
  'requests>=2.32.3,<3.0.0',
  'sqlalchemy-utils>=0.41.2,<0.42.0',
  'sqlalchemy>=2.0.30,<3.0.0']
 
 setup_kwargs = {
     'name': 'tuyul-sdk',
-    'version': '0.0.1rc2',
+    'version': '0.0.1rc3',
     'description': '',
     'long_description': '',
     'author': 'Antoni Oktha Fernandes',
     'author_email': '37358597+DesKaOne@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `tuyul_sdk-0.0.1rc2/PKG-INFO` & `tuyul_sdk-0.0.1rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuyul-sdk
-Version: 0.0.1rc2
+Version: 0.0.1rc3
 Summary: 
 Author: Antoni Oktha Fernandes
 Author-email: 37358597+DesKaOne@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

