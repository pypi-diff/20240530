# Comparing `tmp/sqlink-1.5.4.tar.gz` & `tmp/sqlink-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlink-1.5.4.tar", last modified: Tue Apr 23 08:40:31 2024, max compression
+gzip compressed data, was "sqlink-1.5.5.tar", last modified: Thu May 30 07:48:34 2024, max compression
```

## Comparing `sqlink-1.5.4.tar` & `sqlink-1.5.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 08:40:31.740952 sqlink-1.5.4/
--rw-rw-rw-   0        0        0     1099 2024-03-18 10:38:13.000000 sqlink-1.5.4/LICENSE.txt
--rw-rw-rw-   0        0        0     1044 2024-04-23 08:40:31.739966 sqlink-1.5.4/PKG-INFO
--rw-rw-rw-   0        0        0     4488 2024-03-18 10:41:04.000000 sqlink-1.5.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-23 08:40:31.740952 sqlink-1.5.4/setup.cfg
--rw-rw-rw-   0        0        0      642 2024-04-23 08:39:49.000000 sqlink-1.5.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 08:40:31.700437 sqlink-1.5.4/sqlink/
--rw-rw-rw-   0        0        0      182 2024-03-18 10:38:12.000000 sqlink-1.5.4/sqlink/__init__.py
--rw-rw-rw-   0        0        0    24034 2024-04-23 08:34:25.000000 sqlink-1.5.4/sqlink/dao.py
--rw-rw-rw-   0        0        0     4738 2024-03-18 10:38:12.000000 sqlink-1.5.4/sqlink/database.py
--rw-rw-rw-   0        0        0    13105 2024-04-03 01:03:38.000000 sqlink-1.5.4/sqlink/entity.py
-drwxrwxrwx   0        0        0        0 2024-04-23 08:40:31.716451 sqlink-1.5.4/sqlink.egg-info/
--rw-rw-rw-   0        0        0     1044 2024-04-23 08:40:31.000000 sqlink-1.5.4/sqlink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      715 2024-04-23 08:40:31.000000 sqlink-1.5.4/sqlink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 08:40:31.000000 sqlink-1.5.4/sqlink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-23 08:40:31.000000 sqlink-1.5.4/sqlink.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-23 08:40:31.738961 sqlink-1.5.4/test/
--rw-rw-rw-   0        0        0     3920 2024-03-18 10:38:13.000000 sqlink-1.5.4/test/test_basic_dao.py
--rw-rw-rw-   0        0        0     1116 2024-03-18 10:38:13.000000 sqlink-1.5.4/test/test_comment.py
--rw-rw-rw-   0        0        0     1109 2024-03-18 10:38:13.000000 sqlink-1.5.4/test/test_create_table.py
--rw-rw-rw-   0        0        0     1116 2024-03-18 10:38:13.000000 sqlink-1.5.4/test/test_database.py
--rw-rw-rw-   0        0        0     5258 2024-03-18 10:38:13.000000 sqlink-1.5.4/test/test_entity.py
--rw-rw-rw-   0        0        0      657 2024-04-03 01:09:08.000000 sqlink-1.5.4/test/test_entity_check_ignore_type.py
--rw-rw-rw-   0        0        0     5377 2024-03-18 10:38:13.000000 sqlink-1.5.4/test/test_entity_parse.py
--rw-rw-rw-   0        0        0      889 2024-03-18 10:38:13.000000 sqlink-1.5.4/test/test_env.py
--rw-rw-rw-   0        0        0     3785 2024-03-18 10:38:13.000000 sqlink-1.5.4/test/test_execte_sql_with_daofunc.py
--rw-rw-rw-   0        0        0     4577 2024-03-18 10:38:13.000000 sqlink-1.5.4/test/test_execute_sql_without_dao_func.py
--rw-rw-rw-   0        0        0     3406 2024-03-18 10:38:13.000000 sqlink-1.5.4/test/test_fetch_one.py
--rw-rw-rw-   0        0        0     8258 2024-03-18 10:38:13.000000 sqlink-1.5.4/test/test_fetch_type.py
--rw-rw-rw-   0        0        0     2971 2024-03-18 10:38:13.000000 sqlink-1.5.4/test/test_foreign_key.py
--rw-rw-rw-   0        0        0     1963 2024-03-18 10:38:13.000000 sqlink-1.5.4/test/test_handle_bool.py
--rw-rw-rw-   0        0        0     2450 2024-03-18 10:38:13.000000 sqlink-1.5.4/test/test_ignore.py
--rw-rw-rw-   0        0        0     4368 2024-03-18 10:38:13.000000 sqlink-1.5.4/test/test_insert_conflict.py
--rw-rw-rw-   0        0        0      526 2024-04-23 08:39:29.000000 sqlink-1.5.4/test/test_main.py
--rw-rw-rw-   0        0        0     2386 2024-03-18 10:38:13.000000 sqlink-1.5.4/test/test_select_one_field.py
--rw-rw-rw-   0        0        0     3094 2024-03-18 10:38:13.000000 sqlink-1.5.4/test/test_table_substitute.py
+drwxrwxrwx   0        0        0        0 2024-05-30 07:48:34.095013 sqlink-1.5.5/
+-rw-rw-rw-   0        0        0     1099 2024-03-18 10:38:13.000000 sqlink-1.5.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     1049 2024-05-30 07:48:34.095013 sqlink-1.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4488 2024-03-18 10:41:04.000000 sqlink-1.5.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-30 07:48:34.095013 sqlink-1.5.5/setup.cfg
+-rw-rw-rw-   0        0        0      647 2024-05-30 07:47:17.000000 sqlink-1.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 07:48:34.069451 sqlink-1.5.5/sqlink/
+-rw-rw-rw-   0        0        0      182 2024-03-18 10:38:12.000000 sqlink-1.5.5/sqlink/__init__.py
+-rw-rw-rw-   0        0        0    24029 2024-05-30 07:46:14.000000 sqlink-1.5.5/sqlink/dao.py
+-rw-rw-rw-   0        0        0     4912 2024-05-30 07:46:14.000000 sqlink-1.5.5/sqlink/database.py
+-rw-rw-rw-   0        0        0    13105 2024-04-03 01:03:38.000000 sqlink-1.5.5/sqlink/entity.py
+drwxrwxrwx   0        0        0        0 2024-05-30 07:48:34.074490 sqlink-1.5.5/sqlink.egg-info/
+-rw-rw-rw-   0        0        0     1049 2024-05-30 07:48:34.000000 sqlink-1.5.5/sqlink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      715 2024-05-30 07:48:34.000000 sqlink-1.5.5/sqlink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 07:48:34.000000 sqlink-1.5.5/sqlink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-30 07:48:34.000000 sqlink-1.5.5/sqlink.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 07:48:34.093012 sqlink-1.5.5/test/
+-rw-rw-rw-   0        0        0     3920 2024-03-18 10:38:13.000000 sqlink-1.5.5/test/test_basic_dao.py
+-rw-rw-rw-   0        0        0     1116 2024-03-18 10:38:13.000000 sqlink-1.5.5/test/test_comment.py
+-rw-rw-rw-   0        0        0     1109 2024-03-18 10:38:13.000000 sqlink-1.5.5/test/test_create_table.py
+-rw-rw-rw-   0        0        0     1116 2024-03-18 10:38:13.000000 sqlink-1.5.5/test/test_database.py
+-rw-rw-rw-   0        0        0     5258 2024-03-18 10:38:13.000000 sqlink-1.5.5/test/test_entity.py
+-rw-rw-rw-   0        0        0      657 2024-04-03 01:09:08.000000 sqlink-1.5.5/test/test_entity_check_ignore_type.py
+-rw-rw-rw-   0        0        0     5377 2024-03-18 10:38:13.000000 sqlink-1.5.5/test/test_entity_parse.py
+-rw-rw-rw-   0        0        0      889 2024-03-18 10:38:13.000000 sqlink-1.5.5/test/test_env.py
+-rw-rw-rw-   0        0        0     3785 2024-03-18 10:38:13.000000 sqlink-1.5.5/test/test_execte_sql_with_daofunc.py
+-rw-rw-rw-   0        0        0     4577 2024-03-18 10:38:13.000000 sqlink-1.5.5/test/test_execute_sql_without_dao_func.py
+-rw-rw-rw-   0        0        0     3406 2024-03-18 10:38:13.000000 sqlink-1.5.5/test/test_fetch_one.py
+-rw-rw-rw-   0        0        0     8258 2024-03-18 10:38:13.000000 sqlink-1.5.5/test/test_fetch_type.py
+-rw-rw-rw-   0        0        0     2971 2024-03-18 10:38:13.000000 sqlink-1.5.5/test/test_foreign_key.py
+-rw-rw-rw-   0        0        0     1963 2024-03-18 10:38:13.000000 sqlink-1.5.5/test/test_handle_bool.py
+-rw-rw-rw-   0        0        0     2450 2024-03-18 10:38:13.000000 sqlink-1.5.5/test/test_ignore.py
+-rw-rw-rw-   0        0        0     4368 2024-03-18 10:38:13.000000 sqlink-1.5.5/test/test_insert_conflict.py
+-rw-rw-rw-   0        0        0      526 2024-04-23 08:39:29.000000 sqlink-1.5.5/test/test_main.py
+-rw-rw-rw-   0        0        0     2386 2024-03-18 10:38:13.000000 sqlink-1.5.5/test/test_select_one_field.py
+-rw-rw-rw-   0        0        0     3094 2024-03-18 10:38:13.000000 sqlink-1.5.5/test/test_table_substitute.py
```

### Comparing `sqlink-1.5.4/LICENSE.txt` & `sqlink-1.5.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.4/PKG-INFO` & `sqlink-1.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sqlink
-Version: 1.5.4
+Version: 1.5.5
 Summary: a efficient and concise sql framework.
 Home-page: https://gitee.com/darlingxyz/sqlink
-Author: Nanhai
+Author: NanHaiLoong
 Author-email: nanhai@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `sqlink-1.5.4/README.md` & `sqlink-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.4/setup.py` & `sqlink-1.5.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import setuptools
 
 with open("README_pypi.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sqlink",
-    version="1.5.4",
-    author="Nanhai",
+    version="1.5.5",
+    author="NanHaiLoong",
     author_email="nanhai@163.com",
     description="a efficient and concise sql framework.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/darlingxyz/sqlink",
     packages=['sqlink'],
     classifiers=[
```

### Comparing `sqlink-1.5.4/sqlink/dao.py` & `sqlink-1.5.5/sqlink/dao.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         cls.enable_substitute = enable_substitute
         cls.fetch_type = fetch_type if fetch_type != dataclass else _DATACLASS
         # 新增方法
         cls.execute = execute
         cls.update_cursor = update_cursor
         cls.update_db_type = update_db_type
         cls.create_table = create_table
-        cls._generate_create_table_sql = _generate_create_table_sql
+        cls.get_create_table_sql = get_create_table_sql
         return cls
 
     return decorator
 
 
 def Sql(sql: str, fetch_type=None, fetch_one: bool = False):
     """执行sql语句的装饰器，传入sql语句的同时会自动实现被装饰函数。
@@ -274,15 +274,15 @@
 def update_db_type(self, db_type: str):
     """更新dao对数据库类型的记录"""
     self.db_type = db_type.lower()
 
 
 def create_table(self):
     """依据entity创建表"""
-    sql = self._generate_create_table_sql()
+    sql = self.get_create_table_sql()
     self.cursor.execute(sql)
 
 
 def execute(self, sql: str, args=None, fetch_type=None, fetch_one: bool = False):
     """执行sql语句"""
     sql = __process_main(sql=sql, cls=self)
     if args is None:
@@ -291,16 +291,16 @@
         self.cursor.execute(sql, (args,))
     elif type(args) in (list, tuple):
         self.cursor.execute(sql, __flatten_args(args))
 
     return __fetch_result(self=self, sql=sql, fetch_type=fetch_type, fetch_one=fetch_one)
 
 
-def _generate_create_table_sql(self):
-    """自动生成建表语句"""
+def get_create_table_sql(self) -> str:
+    """返回绑定entity的建表sql语句"""
     table_name = self.entity.__name__.lower()
     # 获取字段名称和类型的字典
     fields = self.entity.__annotations__
 
     field_definitions = []
     foreign_key_constraints = []
```

### Comparing `sqlink-1.5.4/sqlink/database.py` & `sqlink-1.5.5/sqlink/database.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,14 +79,18 @@
 
     def create_tables(self):
         """当表不存在时，才会创建数据表。因此可以反复调用该方法，而不会产生错误。"""
         for dao in self.dao_list:
             dao.create_table()  # noqa
         self.commit()
 
+    def get_create_table_sql(self) -> list[str]:
+        """返回各个entity的建表sql语句"""
+        return [dao.get_create_table_sql() for dao in self.dao_list]
+
     def commit(self):
         """提交事务"""
         self.connection.commit()
 
     def rollback(self):
         """回滚事务"""
         self.connection.rollback()
```

### Comparing `sqlink-1.5.4/sqlink/entity.py` & `sqlink-1.5.5/sqlink/entity.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.4/sqlink.egg-info/PKG-INFO` & `sqlink-1.5.5/sqlink.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sqlink
-Version: 1.5.4
+Version: 1.5.5
 Summary: a efficient and concise sql framework.
 Home-page: https://gitee.com/darlingxyz/sqlink
-Author: Nanhai
+Author: NanHaiLoong
 Author-email: nanhai@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `sqlink-1.5.4/sqlink.egg-info/SOURCES.txt` & `sqlink-1.5.5/sqlink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.4/test/test_basic_dao.py` & `sqlink-1.5.5/test/test_basic_dao.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.4/test/test_comment.py` & `sqlink-1.5.5/test/test_comment.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.4/test/test_create_table.py` & `sqlink-1.5.5/test/test_create_table.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.4/test/test_database.py` & `sqlink-1.5.5/test/test_database.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.4/test/test_entity.py` & `sqlink-1.5.5/test/test_entity.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.4/test/test_entity_check_ignore_type.py` & `sqlink-1.5.5/test/test_entity_check_ignore_type.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.4/test/test_entity_parse.py` & `sqlink-1.5.5/test/test_entity_parse.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.4/test/test_env.py` & `sqlink-1.5.5/test/test_env.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.4/test/test_execte_sql_with_daofunc.py` & `sqlink-1.5.5/test/test_execte_sql_with_daofunc.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.4/test/test_execute_sql_without_dao_func.py` & `sqlink-1.5.5/test/test_execute_sql_without_dao_func.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.4/test/test_fetch_one.py` & `sqlink-1.5.5/test/test_fetch_one.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.4/test/test_fetch_type.py` & `sqlink-1.5.5/test/test_fetch_type.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.4/test/test_foreign_key.py` & `sqlink-1.5.5/test/test_foreign_key.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.4/test/test_handle_bool.py` & `sqlink-1.5.5/test/test_handle_bool.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.4/test/test_ignore.py` & `sqlink-1.5.5/test/test_ignore.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.4/test/test_insert_conflict.py` & `sqlink-1.5.5/test/test_insert_conflict.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.4/test/test_main.py` & `sqlink-1.5.5/test/test_main.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.4/test/test_select_one_field.py` & `sqlink-1.5.5/test/test_select_one_field.py`

 * *Files identical despite different names*

### Comparing `sqlink-1.5.4/test/test_table_substitute.py` & `sqlink-1.5.5/test/test_table_substitute.py`

 * *Files identical despite different names*

