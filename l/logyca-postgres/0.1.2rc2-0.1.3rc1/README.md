# Comparing `tmp/logyca_postgres-0.1.2rc2.tar.gz` & `tmp/logyca_postgres-0.1.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logyca_postgres-0.1.2rc2.tar", last modified: Thu May 23 17:43:05 2024, max compression
+gzip compressed data, was "logyca_postgres-0.1.3rc1.tar", last modified: Thu May 30 20:18:28 2024, max compression
```

## Comparing `logyca_postgres-0.1.2rc2.tar` & `logyca_postgres-0.1.3rc1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 17:43:05.471806 logyca_postgres-0.1.2rc2/
--rw-rw-rw-   0        0        0     1092 2024-04-23 14:32:08.000000 logyca_postgres-0.1.2rc2/LICENSE.txt
--rw-rw-rw-   0        0        0    15852 2024-05-23 17:43:05.469702 logyca_postgres-0.1.2rc2/PKG-INFO
--rw-rw-rw-   0        0        0    12919 2024-05-23 17:41:42.000000 logyca_postgres-0.1.2rc2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 17:43:05.409554 logyca_postgres-0.1.2rc2/logyca_postgres/
--rw-rw-rw-   0        0        0      813 2024-04-26 23:15:08.000000 logyca_postgres-0.1.2rc2/logyca_postgres/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:43:05.440745 logyca_postgres-0.1.2rc2/logyca_postgres/dependencies/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_postgres-0.1.2rc2/logyca_postgres/dependencies/__init__.py
--rw-rw-rw-   0        0        0     9945 2024-04-26 23:13:21.000000 logyca_postgres-0.1.2rc2/logyca_postgres/dependencies/conn_postgres_async.py
--rw-rw-rw-   0        0        0     9988 2024-05-20 21:52:10.000000 logyca_postgres-0.1.2rc2/logyca_postgres/dependencies/conn_postgres_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:43:05.440745 logyca_postgres-0.1.2rc2/logyca_postgres/utils/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_postgres-0.1.2rc2/logyca_postgres/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:43:05.459690 logyca_postgres-0.1.2rc2/logyca_postgres/utils/helpers/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_postgres-0.1.2rc2/logyca_postgres/utils/helpers/__init__.py
--rw-rw-rw-   0        0        0      228 2024-04-23 14:32:08.000000 logyca_postgres-0.1.2rc2/logyca_postgres/utils/helpers/functions.py
--rw-rw-rw-   0        0        0      331 2024-04-23 14:32:08.000000 logyca_postgres-0.1.2rc2/logyca_postgres/utils/helpers/singleton.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:43:05.462472 logyca_postgres-0.1.2rc2/logyca_postgres.egg-info/
--rw-rw-rw-   0        0        0    15852 2024-05-23 17:43:05.000000 logyca_postgres-0.1.2rc2/logyca_postgres.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      568 2024-05-23 17:43:05.000000 logyca_postgres-0.1.2rc2/logyca_postgres.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 17:43:05.000000 logyca_postgres-0.1.2rc2/logyca_postgres.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      445 2024-05-23 17:43:05.000000 logyca_postgres-0.1.2rc2/logyca_postgres.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-23 17:43:05.000000 logyca_postgres-0.1.2rc2/logyca_postgres.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 17:43:05.473644 logyca_postgres-0.1.2rc2/setup.cfg
--rw-rw-rw-   0        0        0     2616 2024-05-23 17:42:19.000000 logyca_postgres-0.1.2rc2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 20:18:28.155746 logyca_postgres-0.1.3rc1/
+-rw-rw-rw-   0        0        0     1092 2024-04-23 14:32:08.000000 logyca_postgres-0.1.3rc1/LICENSE.txt
+-rw-rw-rw-   0        0        0    15852 2024-05-30 20:18:28.155746 logyca_postgres-0.1.3rc1/PKG-INFO
+-rw-rw-rw-   0        0        0    12919 2024-05-23 17:41:42.000000 logyca_postgres-0.1.3rc1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 20:18:28.101724 logyca_postgres-0.1.3rc1/logyca_postgres/
+-rw-rw-rw-   0        0        0      813 2024-04-26 23:15:08.000000 logyca_postgres-0.1.3rc1/logyca_postgres/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 20:18:28.132089 logyca_postgres-0.1.3rc1/logyca_postgres/dependencies/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_postgres-0.1.3rc1/logyca_postgres/dependencies/__init__.py
+-rw-rw-rw-   0        0        0     9635 2024-05-30 20:18:06.000000 logyca_postgres-0.1.3rc1/logyca_postgres/dependencies/conn_postgres_async.py
+-rw-rw-rw-   0        0        0     9581 2024-05-30 20:17:51.000000 logyca_postgres-0.1.3rc1/logyca_postgres/dependencies/conn_postgres_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-30 20:18:28.135700 logyca_postgres-0.1.3rc1/logyca_postgres/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_postgres-0.1.3rc1/logyca_postgres/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 20:18:28.145681 logyca_postgres-0.1.3rc1/logyca_postgres/utils/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca_postgres-0.1.3rc1/logyca_postgres/utils/helpers/__init__.py
+-rw-rw-rw-   0        0        0      228 2024-04-23 14:32:08.000000 logyca_postgres-0.1.3rc1/logyca_postgres/utils/helpers/functions.py
+-rw-rw-rw-   0        0        0      331 2024-04-23 14:32:08.000000 logyca_postgres-0.1.3rc1/logyca_postgres/utils/helpers/singleton.py
+drwxrwxrwx   0        0        0        0 2024-05-30 20:18:28.153581 logyca_postgres-0.1.3rc1/logyca_postgres.egg-info/
+-rw-rw-rw-   0        0        0    15852 2024-05-30 20:18:28.000000 logyca_postgres-0.1.3rc1/logyca_postgres.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      568 2024-05-30 20:18:28.000000 logyca_postgres-0.1.3rc1/logyca_postgres.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 20:18:28.000000 logyca_postgres-0.1.3rc1/logyca_postgres.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      445 2024-05-30 20:18:28.000000 logyca_postgres-0.1.3rc1/logyca_postgres.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-30 20:18:28.000000 logyca_postgres-0.1.3rc1/logyca_postgres.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 20:18:28.155746 logyca_postgres-0.1.3rc1/setup.cfg
+-rw-rw-rw-   0        0        0     2616 2024-05-30 20:13:07.000000 logyca_postgres-0.1.3rc1/setup.py
```

### Comparing `logyca_postgres-0.1.2rc2/LICENSE.txt` & `logyca_postgres-0.1.3rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `logyca_postgres-0.1.2rc2/PKG-INFO` & `logyca_postgres-0.1.3rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logyca-postgres
-Version: 0.1.2rc2
+Version: 0.1.3rc1
 Summary: An integration package created by the company LOGYCA that connects Postgres and is used to standardize connections and dependency injection in synchronous or asynchronous mode. Tested in fastapi and in console/worker scripts.
 Home-page: https://github.com/logyca/python-libraries/tree/main/logyca-postgres
 Author: Jaime Andres Cardona Carrillo
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: postgres,driver database
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: logyca-postgres Version: 0.1.2rc2 Summary: An
+Metadata-Version: 2.1 Name: logyca-postgres Version: 0.1.3rc1 Summary: An
 integration package created by the company LOGYCA that connects Postgres and is
 used to standardize connections and dependency injection in synchronous or
 asynchronous mode. Tested in fastapi and in console/worker scripts. Home-page:
 https://github.com/logyca/python-libraries/tree/main/logyca-postgres Author:
 Jaime Andres Cardona Carrillo Author-email: jacardona@outlook.com License: MIT
 License Keywords: postgres,driver database Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: Intended
```

### Comparing `logyca_postgres-0.1.2rc2/README.md` & `logyca_postgres-0.1.3rc1/README.md`

 * *Files identical despite different names*

### Comparing `logyca_postgres-0.1.2rc2/logyca_postgres/__init__.py` & `logyca_postgres-0.1.3rc1/logyca_postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `logyca_postgres-0.1.2rc2/logyca_postgres/dependencies/conn_postgres_async.py` & `logyca_postgres-0.1.3rc1/logyca_postgres/dependencies/conn_postgres_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,21 +189,14 @@
            return False, ''
     except Exception as e:
         return False, str
 
 async def commit_rollback_async(async_session: AsyncSession):
     try:
         await async_session.commit()
-    except IntegrityError as integrity_exc:
-        await async_session.rollback()
-        msg_error_already_exists = "The record you are trying to create already exists."
-        raise HTTPException(
-            status_code=HTTP_409_CONFLICT,
-            detail=msg_error_already_exists,
-        )
-    except Exception as exc:
+    except Exception as e:
         await async_session.rollback()
         raise HTTPException(
             status_code=HTTP_409_CONFLICT,
-            detail=f"{exc}",
+            detail=f"{e}",
         )
```

### Comparing `logyca_postgres-0.1.2rc2/logyca_postgres/dependencies/conn_postgres_sync.py` & `logyca_postgres-0.1.3rc1/logyca_postgres/dependencies/conn_postgres_sync.py`

 * *Files 5% similar despite different names*

```diff
@@ -199,22 +199,14 @@
 def commit_rollback_sync(sync_session: Session):
     '''
     In SQLAlchemy, all CRUD methods are transactions to the database that must be completed with commit or rollback.
     When the session manager is reviewed in the postgres engine, transactions without commit are reported as rollback, generating a false failure report.
     '''
     try:
         sync_session.commit()
-    except IntegrityError as integrity_exc:
-        msg_error_already_exists_exception =f"The record you are trying to create already exists: {0}"
+    except Exception as e:
         sync_session.rollback()
-        msg_error_already_exists = "The record you are trying to create already exists."
         raise HTTPException(
             status_code=HTTP_409_CONFLICT,
-            detail=msg_error_already_exists,
-        )
-    except Exception as exc:
-        sync_session.rollback()
-        raise HTTPException(
-            status_code=HTTP_409_CONFLICT,
-            detail=f"{exc}",
+            detail=f"{e}",
         )
```

### Comparing `logyca_postgres-0.1.2rc2/logyca_postgres.egg-info/PKG-INFO` & `logyca_postgres-0.1.3rc1/logyca_postgres.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logyca-postgres
-Version: 0.1.2rc2
+Version: 0.1.3rc1
 Summary: An integration package created by the company LOGYCA that connects Postgres and is used to standardize connections and dependency injection in synchronous or asynchronous mode. Tested in fastapi and in console/worker scripts.
 Home-page: https://github.com/logyca/python-libraries/tree/main/logyca-postgres
 Author: Jaime Andres Cardona Carrillo
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: postgres,driver database
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: logyca-postgres Version: 0.1.2rc2 Summary: An
+Metadata-Version: 2.1 Name: logyca-postgres Version: 0.1.3rc1 Summary: An
 integration package created by the company LOGYCA that connects Postgres and is
 used to standardize connections and dependency injection in synchronous or
 asynchronous mode. Tested in fastapi and in console/worker scripts. Home-page:
 https://github.com/logyca/python-libraries/tree/main/logyca-postgres Author:
 Jaime Andres Cardona Carrillo Author-email: jacardona@outlook.com License: MIT
 License Keywords: postgres,driver database Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: Intended
```

### Comparing `logyca_postgres-0.1.2rc2/logyca_postgres.egg-info/SOURCES.txt` & `logyca_postgres-0.1.3rc1/logyca_postgres.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logyca_postgres-0.1.2rc2/setup.py` & `logyca_postgres-0.1.3rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 COMPANY_NAME="LOGYCA"
 PACKAGE_NAME = "logyca-postgres"
-VERSION = "0.1.2rc2"
+VERSION = "0.1.3rc1"
 
 install_requires = ["SQLAlchemy>=2.0.6","starlette>=0.24.0"]
 install_requires_asyncpg = ["asyncpg >=0.27.0"]
 install_requires_psycopg2 = ["psycopg2 >=2.9.6"]
 install_requires_psycopg2_binary = ["psycopg2-binary >=2.9.6"]
 
 extras_require = {
```

