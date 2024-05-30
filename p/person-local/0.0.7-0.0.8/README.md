# Comparing `tmp/person-local-0.0.7.tar.gz` & `tmp/person-local-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "person-local-0.0.7.tar", last modified: Mon Aug 21 06:52:06 2023, max compression
+gzip compressed data, was "person-local-0.0.8.tar", last modified: Mon Aug 21 07:54:00 2023, max compression
```

## Comparing `person-local-0.0.7.tar` & `person-local-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 06:52:06.784512 person-local-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-21 06:52:06.784512 person-local-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-08-21 06:51:49.000000 person-local-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 06:52:06.784512 person-local-0.0.7/person_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-21 06:52:06.000000 person-local-0.0.7/person_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-21 06:52:06.000000 person-local-0.0.7/person_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-21 06:52:06.000000 person-local-0.0.7/person_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-21 06:52:06.000000 person-local-0.0.7/person_local.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 06:52:06.784512 person-local-0.0.7/person_local_python_package/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-21 06:51:49.000000 person-local-0.0.7/person_local_python_package/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 06:52:06.784512 person-local-0.0.7/person_local_python_package/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-21 06:51:49.000000 person-local-0.0.7/person_local_python_package/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-21 06:51:49.000000 person-local-0.0.7/person_local_python_package/src/delete_person_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-08-21 06:51:49.000000 person-local-0.0.7/person_local_python_package/src/insert_person_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-08-21 06:51:49.000000 person-local-0.0.7/person_local_python_package/src/update_person_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-21 06:51:49.000000 person-local-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-21 06:52:06.784512 person-local-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-21 06:51:49.000000 person-local-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 07:54:00.712449 person-local-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-21 07:54:00.712449 person-local-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-08-21 07:53:31.000000 person-local-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 07:54:00.712449 person-local-0.0.8/person_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-21 07:54:00.000000 person-local-0.0.8/person_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-21 07:54:00.000000 person-local-0.0.8/person_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-21 07:54:00.000000 person-local-0.0.8/person_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-21 07:54:00.000000 person-local-0.0.8/person_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 07:54:00.712449 person-local-0.0.8/person_local_python_package/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-21 07:53:31.000000 person-local-0.0.8/person_local_python_package/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 07:54:00.712449 person-local-0.0.8/person_local_python_package/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-21 07:53:31.000000 person-local-0.0.8/person_local_python_package/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-08-21 07:53:31.000000 person-local-0.0.8/person_local_python_package/src/delete_person_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-08-21 07:53:31.000000 person-local-0.0.8/person_local_python_package/src/insert_person_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-08-21 07:53:31.000000 person-local-0.0.8/person_local_python_package/src/update_person_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-21 07:53:31.000000 person-local-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-21 07:54:00.712449 person-local-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-21 07:53:31.000000 person-local-0.0.8/setup.py
```

### Comparing `person-local-0.0.7/README.md` & `person-local-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `person-local-0.0.7/person_local_python_package/src/delete_person_table.py` & `person-local-0.0.8/person_local_python_package/src/delete_person_table.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,13 +15,16 @@
 
 class DeletePerson(generic_crud.GenericCRUD):
     def __init__(self):
         pass
 
     def delete(person_id: int) -> None:
         loger_local.start("Delete person by ID",object={"person_id":person_id})
-        conn = connection.Connection("person").connect()
+        conn = connection.Connection.get_connection("person")
         db_cursor = connection.Connection.cursor(conn)
         query = ("UPDATE person.person_table SET end_timestamp = CURRENT_TIMESTAMP WHERE person_id = {}".format(person_id))
         db_cursor.execute(query)
         conn.commit()
         loger_local.end()
+
+
+DeletePerson.delete('2')
```

### Comparing `person-local-0.0.7/person_local_python_package/src/insert_person_table.py` & `person-local-0.0.8/person_local_python_package/src/insert_person_table.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 }
 loger_local = Logger.create_logger(object=object_init)
 
 
 def insert_person(number: int, gender_id: int, last_coordinate: str, location_id: int) -> int:
     loger_local.start("Insert person",object={"number": number, "gender_id": gender_id, "last_coordinate": last_coordinate , "location_id": location_id})
     try:
-        conn = connection.Connection("person").connect()
+        conn = connection.Connection.get_connection("person")
         db_cursor = connection.Connection.cursor(conn)
         query = ("INSERT INTO person.person_table (number, gender_id, last_coordinate, location_id,start_timestamp) VALUES ({}, {}, {}, {}, CURRENT_TIMESTAMP)".
                  format(number, gender_id, last_coordinate, location_id))
 
         db_cursor.execute(query)
         conn.commit()
         loger_local.info("Person inserted successfully.")
@@ -33,15 +33,15 @@
     loger_local.end("Person added", object={'person_id': last_inserted_id})
     return last_inserted_id    
 
 
 
 def insert_person_ml( person_id: int) -> int:
     loger_local.start("Insert person",object={"id":id})
-    conn = connection.Connection("person").connect()
+    conn = connection.Connection.get_connection("person")
     db_cursor = connection.Connection.cursor(conn)
 
     query = ("INSERT INTO person.person_ml_table (id) VALUES ({})".format(id))
 
     db_cursor.execute(query)
     conn.commit()
     loger_local.end("Person added", object={'person_id': person_id})
```

### Comparing `person-local-0.0.7/person_local_python_package/src/update_person_table.py` & `person-local-0.0.8/person_local_python_package/src/update_person_table.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,74 +9,78 @@
     'component_id': EXTERNAL_USER_COMPONENT_ID,
     'component_name':EXTERNAL_USER_COMPONENT_NAME,
     'component_category':LoggerComponentEnum.ComponentCategory.Code.value,
     "developer_email":"jenya.b@circ.zone"
 }
 loger_local = Logger.create_logger(object=object_init)
 
-def conn_db(db,query: str) -> None:
-    loger_local.start("Sending query to db",object={"db":db,"query":query})
-    conn = connection.Connection("person").connect()
-    db_cursor = connection.Connection.cursor(conn)
-    db_cursor.execute(query)
-    conn.commit()
-    loger_local.end()
+
 
 class UpdatePerson:
+    db_conn = connection.Connection.get_connection("person")
+
     def __init__(self):
         pass
 
+    def conn_db(query: str) -> None:
+        loger_local.start("Sending query to db",object={"query":query})
+        #db_cursor = connection.Connection.cursor(conn)
+        db_cursor = connection.Connection.cursor(UpdatePerson.db_conn)
+        db_cursor.execute(query)
+        UpdatePerson.db_conn.commit()
+        loger_local.end()
+
     def update_person_day(id: int,day: int) -> None:
         loger_local.start("Update day by ID",object={"id":id,"day":day})
         query = ("UPDATE person.person_table SET day = {} WHERE person_id = {}".format(day,id))
-        conn_db("person",query)
+        UpdatePerson.conn_db(query)
         loger_local.end()
 
     def update_person_month(id: int,month: int) -> None:
         loger_local.start("Update month by ID",object={"id":id,"month":month})
         query = ("UPDATE person.person_table SET month = {} WHERE person_id = {}".format(month,id))
-        conn_db("person",query)
+        UpdatePerson.conn_db(query)
         loger_local.end()
 
     def update_person_year(id: int,year: int) -> None:
         loger_local.start("Update year by ID",object={"id":id,"year":year})
         query = ("UPDATE person.person_table SET year = {} WHERE person_id = {}".format(year,id))
-        conn_db("person",query)
+        UpdatePerson.conn_db(query)
         loger_local.end()
 
     def update_person_birthday_date(id: int,birthday_date: datetime.date) -> None:
         loger_local.start("Update birthday date by ID",object={"id":id,"birthday_date":birthday_date})
         query = ("UPDATE person.person_table SET birthday_date = '{}' WHERE person_id = {}".format(birthday_date,id))
-        conn_db("person",query)
+        UpdatePerson.conn_db(query)
         loger_local.end()
 
     def update_person_first_name(id: int,first_name: str) -> None:
         loger_local.start("Update first name by ID",object={"id":id,"first_name":first_name})
         query = ("UPDATE person.person_table SET first_name = '{}' WHERE person_id = {}".format(first_name,id))
-        conn_db("person",query)
+        UpdatePerson.conn_db(query)
         UpdatePerson.update_person_ml_first_name(id,first_name)
         loger_local.end()
 
     def update_person_ml_first_name(id: int,first_name: str) -> None:
         loger_local.start("Update first name in ml table by ID",object={"id":id,"first_name":first_name})
         query = ("UPDATE person.person_ml_table SET first_name = '{}' WHERE person_id = {}".format(first_name,id))
-        conn_db("person",query)
+        UpdatePerson.conn_db(query)
         loger_local.end() 
 
     def update_person_nickname(id: int,nickname: str) -> None:
         loger_local.start("Update nickname by ID",object={"id":id,"nickname":nickname})
         query = ("UPDATE person.person_table SET nickname = '{}' WHERE person_id = {}".format(nickname,id))
-        conn_db("person",query)
+        UpdatePerson.conn_db(query)
         loger_local.end()
 
     def update_person_last_name(id: int,last_name: str) -> None:
         loger_local.start("Update last name by ID",object={"id":id,"last_name":last_name})
         query = ("UPDATE person.person_table SET last_name = '{}' WHERE person_id = {}".format(last_name,id))
-        conn_db("person",query)
+        UpdatePerson.conn_db(query)
         UpdatePerson.update_person_ml_last_name(id,last_name)
         loger_local.end()
 
     def update_person_ml_last_name(id: int,last_name: str) -> None:
         loger_local.start("Update last name in ml table by ID",object={"id":id,"last_name":last_name})
         query = ("UPDATE person.person_ml_table SET last_name = '{}' WHERE person_id = {}".format(last_name,id))
-        conn_db("person",query)
+        UpdatePerson.conn_db(query)
         loger_local.end()
```

### Comparing `person-local-0.0.7/pyproject.toml` & `person-local-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `person-local-0.0.7/setup.py` & `person-local-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 # Each Python project should have pyproject.toml or setup.py
 # used by python -m build
 # ```python -m build``` needs pyproject.toml or setup.py
 # The need for setup.py is changing as of poetry 1.1.0 (including current pre-release) as we have moved away from needing to generate a setup.py file to enable editable installs - We might able to delete this file in the near future
 setuptools.setup(
      name='person-local',  
-     version='0.0.7', # https://pypi.org/project/<project-name>/
+     version='0.0.8', # https://pypi.org/project/<project-name>/
      author="Circles",
      author_email="info@circles.life",
      description="PyPI Package for Circles person Local Python", 
      long_description="This is a package for sharing common XXX function used in different repositories",
      long_description_content_type="text/markdown",
      url="https://github.com/circles-zone/person-local-python-package",
      packages=setuptools.find_packages(),
```

