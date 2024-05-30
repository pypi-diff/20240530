# Comparing `tmp/ecodev_core-0.0.8.tar.gz` & `tmp/ecodev_core-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecodev_core-0.0.8.tar", max compression
+gzip compressed data, was "ecodev_core-0.0.9.tar", max compression
```

## Comparing `ecodev_core-0.0.8.tar` & `ecodev_core-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1074 2024-02-07 12:29:17.080635 ecodev_core-0.0.8/LICENSE.md
--rw-r--r--   0        0        0     1298 2024-02-07 10:05:35.777930 ecodev_core-0.0.8/README.md
--rw-r--r--   0        0        0     4244 2024-02-29 14:14:24.965546 ecodev_core-0.0.8/ecodev_core/__init__.py
--rw-r--r--   0        0        0     3763 2024-01-09 10:06:30.631726 ecodev_core-0.0.8/ecodev_core/app_activity.py
--rw-r--r--   0        0        0      726 2024-01-09 10:06:30.759726 ecodev_core-0.0.8/ecodev_core/app_rights.py
--rw-r--r--   0        0        0     2949 2024-01-09 10:06:30.675726 ecodev_core-0.0.8/ecodev_core/app_user.py
--rw-r--r--   0        0        0      433 2024-01-10 16:50:53.255183 ecodev_core-0.0.8/ecodev_core/auth_configuration.py
--rw-r--r--   0        0        0     7900 2024-02-07 12:29:17.080635 ecodev_core-0.0.8/ecodev_core/authentication.py
--rw-r--r--   0        0        0     3055 2024-02-29 14:34:28.702073 ecodev_core-0.0.8/ecodev_core/backup.py
--rw-r--r--   0        0        0     6917 2024-01-09 10:06:30.723726 ecodev_core-0.0.8/ecodev_core/check_dependencies.py
--rw-r--r--   0        0        0      899 2023-08-01 12:04:56.058648 ecodev_core-0.0.8/ecodev_core/custom_equal.py
--rw-r--r--   0        0        0     1773 2024-02-29 14:14:24.965546 ecodev_core-0.0.8/ecodev_core/db_connection.py
--rw-r--r--   0        0        0     5041 2023-12-22 08:56:01.155015 ecodev_core-0.0.8/ecodev_core/db_filters.py
--rw-r--r--   0        0        0     3646 2024-02-07 12:29:17.080635 ecodev_core-0.0.8/ecodev_core/db_insertion.py
--rw-r--r--   0        0        0     7345 2024-01-10 16:50:53.255183 ecodev_core-0.0.8/ecodev_core/db_retrieval.py
--rw-r--r--   0        0        0      556 2024-01-09 10:06:30.795725 ecodev_core-0.0.8/ecodev_core/enum_utils.py
--rw-r--r--   0        0        0     2364 2023-12-20 15:13:48.833350 ecodev_core-0.0.8/ecodev_core/list_utils.py
--rw-r--r--   0        0        0     3149 2022-08-23 18:46:19.185851 ecodev_core-0.0.8/ecodev_core/logger.py
--rw-r--r--   0        0        0     1079 2023-04-03 18:49:00.819469 ecodev_core-0.0.8/ecodev_core/pandas_utils.py
--rw-r--r--   0        0        0      320 2023-04-07 08:15:48.908839 ecodev_core-0.0.8/ecodev_core/permissions.py
--rw-r--r--   0        0        0      741 2024-01-10 16:50:53.255183 ecodev_core-0.0.8/ecodev_core/pydantic_utils.py
--rw-r--r--   0        0        0      996 2023-07-24 13:06:11.219573 ecodev_core-0.0.8/ecodev_core/read_write.py
--rw-r--r--   0        0        0     5933 2024-01-09 10:06:30.663726 ecodev_core-0.0.8/ecodev_core/safe_utils.py
--rw-r--r--   0        0        0     2011 2024-02-29 14:34:34.694056 ecodev_core-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3257 1970-01-01 00:00:00.000000 ecodev_core-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-02-07 12:29:17.080635 ecodev_core-0.0.9/LICENSE.md
+-rw-r--r--   0        0        0     1298 2024-02-07 10:05:35.777930 ecodev_core-0.0.9/README.md
+-rw-r--r--   0        0        0     4368 2024-03-15 13:40:53.731623 ecodev_core-0.0.9/ecodev_core/__init__.py
+-rw-r--r--   0        0        0     3763 2024-01-09 10:06:30.631726 ecodev_core-0.0.9/ecodev_core/app_activity.py
+-rw-r--r--   0        0        0      726 2024-01-09 10:06:30.759726 ecodev_core-0.0.9/ecodev_core/app_rights.py
+-rw-r--r--   0        0        0     2949 2024-01-09 10:06:30.675726 ecodev_core-0.0.9/ecodev_core/app_user.py
+-rw-r--r--   0        0        0      433 2024-01-10 16:50:53.255183 ecodev_core-0.0.9/ecodev_core/auth_configuration.py
+-rw-r--r--   0        0        0     7900 2024-02-07 12:29:17.080635 ecodev_core-0.0.9/ecodev_core/authentication.py
+-rw-r--r--   0        0        0     3055 2024-03-15 13:33:52.163110 ecodev_core-0.0.9/ecodev_core/backup.py
+-rw-r--r--   0        0        0     6917 2024-01-09 10:06:30.723726 ecodev_core-0.0.9/ecodev_core/check_dependencies.py
+-rw-r--r--   0        0        0      899 2023-08-01 12:04:56.058648 ecodev_core-0.0.9/ecodev_core/custom_equal.py
+-rw-r--r--   0        0        0     1773 2024-03-15 13:33:52.163110 ecodev_core-0.0.9/ecodev_core/db_connection.py
+-rw-r--r--   0        0        0     5041 2023-12-22 08:56:01.155015 ecodev_core-0.0.9/ecodev_core/db_filters.py
+-rw-r--r--   0        0        0     3646 2024-02-07 12:29:17.080635 ecodev_core-0.0.9/ecodev_core/db_insertion.py
+-rw-r--r--   0        0        0     7345 2024-01-10 16:50:53.255183 ecodev_core-0.0.9/ecodev_core/db_retrieval.py
+-rw-r--r--   0        0        0      556 2024-03-05 11:04:03.380643 ecodev_core-0.0.9/ecodev_core/enum_utils.py
+-rw-r--r--   0        0        0     3006 2024-03-15 13:33:52.187111 ecodev_core-0.0.9/ecodev_core/list_utils.py
+-rw-r--r--   0        0        0     3149 2022-08-23 18:46:19.185851 ecodev_core-0.0.9/ecodev_core/logger.py
+-rw-r--r--   0        0        0     1364 2024-03-15 13:33:52.187111 ecodev_core-0.0.9/ecodev_core/pandas_utils.py
+-rw-r--r--   0        0        0      320 2023-04-07 08:15:48.908839 ecodev_core-0.0.9/ecodev_core/permissions.py
+-rw-r--r--   0        0        0      741 2024-01-10 16:50:53.255183 ecodev_core-0.0.9/ecodev_core/pydantic_utils.py
+-rw-r--r--   0        0        0      996 2023-07-24 13:06:11.219573 ecodev_core-0.0.9/ecodev_core/read_write.py
+-rw-r--r--   0        0        0     5933 2024-01-09 10:06:30.663726 ecodev_core-0.0.9/ecodev_core/safe_utils.py
+-rw-r--r--   0        0        0     2027 2024-03-15 13:51:48.913430 ecodev_core-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3290 1970-01-01 00:00:00.000000 ecodev_core-0.0.9/PKG-INFO
```

### Comparing `ecodev_core-0.0.8/LICENSE.md` & `ecodev_core-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ecodev_core-0.0.8/README.md` & `ecodev_core-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ecodev_core-0.0.8/ecodev_core/__init__.py` & `ecodev_core-0.0.9/ecodev_core/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,19 +38,21 @@
 from ecodev_core.db_insertion import get_raw_df
 from ecodev_core.db_retrieval import count_rows
 from ecodev_core.db_retrieval import get_rows
 from ecodev_core.db_retrieval import ServerSideField
 from ecodev_core.enum_utils import enum_converter
 from ecodev_core.list_utils import first_or_default
 from ecodev_core.list_utils import first_transformed_or_default
+from ecodev_core.list_utils import group_by
 from ecodev_core.list_utils import group_by_value
 from ecodev_core.list_utils import lselect
 from ecodev_core.list_utils import lselectfirst
 from ecodev_core.logger import log_critical
 from ecodev_core.logger import logger_get
+from ecodev_core.pandas_utils import get_excelfile
 from ecodev_core.pandas_utils import jsonify_series
 from ecodev_core.pandas_utils import pd_equals
 from ecodev_core.permissions import Permission
 from ecodev_core.pydantic_utils import Basic
 from ecodev_core.pydantic_utils import CustomFrozen
 from ecodev_core.pydantic_utils import Frozen
 from ecodev_core.pydantic_utils import OrmFrozen
@@ -72,8 +74,8 @@
     'first_or_default', 'lselect', 'lselectfirst', 'first_transformed_or_default', 'log_critical',
     'logger_get', 'Permission', 'AppUser', 'AppRight', 'Basic', 'Frozen', 'CustomFrozen', 'JwtAuth',
     'SafeTestCase', 'SimpleReturn', 'safe_clt', 'stringify', 'boolify', 'get_user', 'floatify',
     'delete_table', 'SCHEME', 'DB_URL', 'pd_equals', 'jsonify_series', 'upsert_app_users', 'intify',
     'enum_converter', 'ServerSideFilter', 'get_rows', 'count_rows', 'ServerSideField', 'get_raw_df',
     'generic_insertion', 'custom_equal', 'is_authorized_user', 'get_method', 'AppActivity',
     'fastapi_monitor', 'dash_monitor', 'is_monitoring_user', 'get_recent_activities', 'select_user',
-    'get_access_token', 'safe_get_user', 'backup']
+    'get_access_token', 'safe_get_user', 'backup', 'group_by', 'get_excelfile']
```

### Comparing `ecodev_core-0.0.8/ecodev_core/app_activity.py` & `ecodev_core-0.0.9/ecodev_core/app_activity.py`

 * *Files identical despite different names*

### Comparing `ecodev_core-0.0.8/ecodev_core/app_rights.py` & `ecodev_core-0.0.9/ecodev_core/app_rights.py`

 * *Files identical despite different names*

### Comparing `ecodev_core-0.0.8/ecodev_core/app_user.py` & `ecodev_core-0.0.9/ecodev_core/app_user.py`

 * *Files identical despite different names*

### Comparing `ecodev_core-0.0.8/ecodev_core/authentication.py` & `ecodev_core-0.0.9/ecodev_core/authentication.py`

 * *Files identical despite different names*

### Comparing `ecodev_core-0.0.8/ecodev_core/backup.py` & `ecodev_core-0.0.9/ecodev_core/backup.py`

 * *Files identical despite different names*

### Comparing `ecodev_core-0.0.8/ecodev_core/check_dependencies.py` & `ecodev_core-0.0.9/ecodev_core/check_dependencies.py`

 * *Files identical despite different names*

### Comparing `ecodev_core-0.0.8/ecodev_core/custom_equal.py` & `ecodev_core-0.0.9/ecodev_core/custom_equal.py`

 * *Files identical despite different names*

### Comparing `ecodev_core-0.0.8/ecodev_core/db_connection.py` & `ecodev_core-0.0.9/ecodev_core/db_connection.py`

 * *Files identical despite different names*

### Comparing `ecodev_core-0.0.8/ecodev_core/db_filters.py` & `ecodev_core-0.0.9/ecodev_core/db_filters.py`

 * *Files identical despite different names*

### Comparing `ecodev_core-0.0.8/ecodev_core/db_insertion.py` & `ecodev_core-0.0.9/ecodev_core/db_insertion.py`

 * *Files identical despite different names*

### Comparing `ecodev_core-0.0.8/ecodev_core/db_retrieval.py` & `ecodev_core-0.0.9/ecodev_core/db_retrieval.py`

 * *Files identical despite different names*

### Comparing `ecodev_core-0.0.8/ecodev_core/enum_utils.py` & `ecodev_core-0.0.9/ecodev_core/enum_utils.py`

 * *Files identical despite different names*

### Comparing `ecodev_core-0.0.8/ecodev_core/list_utils.py` & `ecodev_core-0.0.9/ecodev_core/list_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """
 Module implementing helper methods working on lists
 """
 from collections import defaultdict
+from itertools import groupby
 from typing import Any
 from typing import Callable
 from typing import Dict
+from typing import Iterator
 from typing import List
 from typing import Optional
+from typing import Tuple
 from typing import Union
 
 
 def group_by_value(list_to_group: List[Any]) -> Dict[Any, List[int]]:
     """
     Given a list, group together all equal values by storing them in a dictionary.
     The keys are the unique list values (think about overriding the class equals if you pass
@@ -38,14 +41,27 @@
         return default
 
     if condition is None:
         return next(iter(sequence), default)
     return next((elt for elt in sequence if condition(elt)), default)
 
 
+def group_by(sequence: List[Any], key: Union[Callable, None]) -> Iterator[Tuple[Any, List[Any]]]:
+    """
+    Extension of itertools groupby method.
+
+    Reasons of existence:
+        - do the sorting before the grouping to avoid the usual mistake of forgetting the sorting
+        - convert the group Iterator to a list. More convenient that the default groupby behaviour
+           in all cases where you need to iterate more than once on the group
+    """
+    for key, group in groupby(sorted(sequence, key=key), key=key):
+        yield key, list(group)
+
+
 def lselect(sequence: List[Any], condition: Union[Callable, None] = None) -> List[Any]:
     """
     Filter the passed sequence according to the passed condition
     """
     return list(filter(condition, sequence))
```

### Comparing `ecodev_core-0.0.8/ecodev_core/logger.py` & `ecodev_core-0.0.9/ecodev_core/logger.py`

 * *Files identical despite different names*

### Comparing `ecodev_core-0.0.8/ecodev_core/pandas_utils.py` & `ecodev_core-0.0.9/ecodev_core/pandas_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Module implementing some utilitary methods on pandas types
 """
 import tempfile
+from base64 import b64decode
 from pathlib import Path
 from typing import Dict
 
 import numpy as np
 import pandas as pd
 
 
@@ -24,7 +25,16 @@
 
 def jsonify_series(row: pd.Series) -> Dict:
     """
     Convert a serie into a json compliant dictionary (replacing np.nans by Nones)
     """
     return {key: None if isinstance(value, float) and np.isnan(value) else value for key, value in
             row.to_dict().items()}
+
+
+def get_excelfile(contents: str) -> pd.ExcelFile:
+    """
+    Function which converts user xlsx file upload into a pd.ExcelFile
+    """
+    content_type, content_string = contents.split(',')
+    xl = b64decode(content_string)
+    return pd.ExcelFile(xl)
```

### Comparing `ecodev_core-0.0.8/ecodev_core/pydantic_utils.py` & `ecodev_core-0.0.9/ecodev_core/pydantic_utils.py`

 * *Files identical despite different names*

### Comparing `ecodev_core-0.0.8/ecodev_core/read_write.py` & `ecodev_core-0.0.9/ecodev_core/read_write.py`

 * *Files identical despite different names*

### Comparing `ecodev_core-0.0.8/ecodev_core/safe_utils.py` & `ecodev_core-0.0.9/ecodev_core/safe_utils.py`

 * *Files identical despite different names*

### Comparing `ecodev_core-0.0.8/pyproject.toml` & `ecodev_core-0.0.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ecodev-core"
-version = "0.0.8"
+version = "0.0.9"
 description = "Low level sqlmodel/fastapi/pydantic building blocks"
 authors = ["Thomas Epelbaum <tomepel@gmail.com>",
 					 "Olivier Gabriel <olivier.gabriel.geom@gmail.com>",
 					 "Amaury Salles <amaury.salles@gmail.com>",
 					 "Yoann Diep <yoann.diep@hotmail.fr>",
 					 "Dorian Kodelja <dorian.kodelja@gmail.com>",
 
@@ -49,12 +49,13 @@
 pydantic = {version = "~2", extras = ["python-dotenv"]}
 python-jose = {version = "~3", extras = ["cryptography"]}
 passlib = {version = "~1", extras = ["bcyrypt"]}
 sqladmin = "0.15.2"
 httpx = "~0"
 pydantic-settings = "~2"
 psycopg2-binary = "~2"
+openpyxl = "~3"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ecodev_core-0.0.8/PKG-INFO` & `ecodev_core-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecodev-core
-Version: 0.0.8
+Version: 0.0.9
 Summary: Low level sqlmodel/fastapi/pydantic building blocks
 License: MIT
 Author: Thomas Epelbaum
 Author-email: tomepel@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Web Environment
@@ -32,14 +32,15 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: fastapi (>=0,<1)
 Requires-Dist: httpx (>=0,<1)
 Requires-Dist: numpy (>=1,<2)
+Requires-Dist: openpyxl (>=3,<4)
 Requires-Dist: pandas (>=2,<3)
 Requires-Dist: passlib[bcyrypt] (>=1,<2)
 Requires-Dist: psycopg2-binary (>=2,<3)
 Requires-Dist: pydantic-settings (>=2,<3)
 Requires-Dist: pydantic[python-dotenv] (>=2,<3)
 Requires-Dist: python-jose[cryptography] (>=3,<4)
 Requires-Dist: sqladmin (==0.15.2)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ecodev-core Version: 0.0.8 Summary: Low level
+Metadata-Version: 2.1 Name: ecodev-core Version: 0.0.9 Summary: Low level
 sqlmodel/fastapi/pydantic building blocks License: MIT Author: Thomas Epelbaum
 Author-email: tomepel@gmail.com Requires-Python: >=3.11,<4.0 Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Environment :: Web Environment
 Classifier: Framework :: AsyncIO Classifier: Framework :: FastAPI Classifier:
 Framework :: Pydantic Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Information Technology Classifier: Intended Audience ::
 Science/Research Classifier: Intended Audience :: System Administrators
@@ -15,19 +15,20 @@
 Database Engines/Servers Classifier: Topic :: Internet Classifier: Topic ::
 Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development Classifier: Topic :: Software
 Development :: Libraries Classifier: Topic :: Software Development :: Libraries
 :: Application Frameworks Classifier: Topic :: Software Development ::
 Libraries :: Python Modules Classifier: Typing :: Typed Requires-Dist: fastapi
 (>=0,<1) Requires-Dist: httpx (>=0,<1) Requires-Dist: numpy (>=1,<2) Requires-
-Dist: pandas (>=2,<3) Requires-Dist: passlib[bcyrypt] (>=1,<2) Requires-Dist:
-psycopg2-binary (>=2,<3) Requires-Dist: pydantic-settings (>=2,<3) Requires-
-Dist: pydantic[python-dotenv] (>=2,<3) Requires-Dist: python-jose[cryptography]
-(>=3,<4) Requires-Dist: sqladmin (==0.15.2) Requires-Dist: sqlmodel (>=0,<1)
-Description-Content-Type: text/markdown # ecodev-core
+Dist: openpyxl (>=3,<4) Requires-Dist: pandas (>=2,<3) Requires-Dist: passlib
+[bcyrypt] (>=1,<2) Requires-Dist: psycopg2-binary (>=2,<3) Requires-Dist:
+pydantic-settings (>=2,<3) Requires-Dist: pydantic[python-dotenv] (>=2,<3)
+Requires-Dist: python-jose[cryptography] (>=3,<4) Requires-Dist: sqladmin
+(==0.15.2) Requires-Dist: sqlmodel (>=0,<1) Description-Content-Type: text/
+markdown # ecodev-core
                      _[_C_o_v_e_r_a_g_e_]_[_P_u_b_l_i_s_h_]_[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]
 Low level ecoact generic code. Aimed at being published in open source with
 poetry ## Installation of this package You are strongly encouraged to install
 this package via Docker. Starting from a project with a Docker file: * add the
 module ecodev-core in the `requirements.txt` file * make sure the `.env` file
 includes all required fields (see `BaseSettings` and
 `AuthenticationConfiguration`) * build the new version of the Docker container
```

