# Comparing `tmp/txdpy-8.9.1.tar.gz` & `tmp/txdpy-8.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txdpy-8.9.1.tar", last modified: Mon May 27 10:25:14 2024, max compression
+gzip compressed data, was "txdpy-8.9.2.tar", last modified: Thu May 30 02:04:10 2024, max compression
```

## Comparing `txdpy-8.9.1.tar` & `txdpy-8.9.2.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 10:25:14.771398 txdpy-8.9.1/
--rw-rw-rw-   0        0        0      333 2024-05-27 10:25:14.771398 txdpy-8.9.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-27 10:25:14.771398 txdpy-8.9.1/setup.cfg
--rw-rw-rw-   0        0        0      340 2024-05-27 10:23:46.000000 txdpy-8.9.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-27 10:25:14.755778 txdpy-8.9.1/txdpy/
--rw-rw-rw-   0        0        0     3287 2024-05-27 06:54:38.000000 txdpy-8.9.1/txdpy/__init__.py
--rw-rw-rw-   0        0        0    27787 2024-05-27 07:11:53.000000 txdpy-8.9.1/txdpy/bk_179.py
--rw-rw-rw-   0        0        0    28823 2024-05-27 10:22:55.000000 txdpy-8.9.1/txdpy/excel数据或mysql操作.py
--rw-rw-rw-   0        0        0      930 2024-05-25 06:52:11.000000 txdpy-8.9.1/txdpy/列表操作.py
--rw-rw-rw-   0        0        0     2183 2024-05-25 06:52:11.000000 txdpy-8.9.1/txdpy/字符串类型的判断和提取.py
--rw-rw-rw-   0        0        0     6240 2024-05-25 06:53:20.000000 txdpy-8.9.1/txdpy/数据库操作.py
--rw-rw-rw-   0        0        0     5308 2024-05-25 06:52:11.000000 txdpy-8.9.1/txdpy/文本括号及引号不匹配检查.py
--rw-rw-rw-   0        0        0      263 2024-05-27 06:52:44.000000 txdpy-8.9.1/txdpy/文本错别字检查.py
--rw-rw-rw-   0        0        0     5882 2024-05-25 06:52:11.000000 txdpy-8.9.1/txdpy/爬虫辅助功能.py
--rw-rw-rw-   0        0        0     3546 2024-05-27 06:56:43.000000 txdpy-8.9.1/txdpy/百度ai接口使用.py
--rw-rw-rw-   0        0        0     2459 2024-05-25 06:52:11.000000 txdpy-8.9.1/txdpy/省市区名称的提取或判断.py
-drwxrwxrwx   0        0        0        0 2024-05-27 10:25:14.771398 txdpy-8.9.1/txdpy.egg-info/
--rw-rw-rw-   0        0        0      333 2024-05-27 10:25:14.000000 txdpy-8.9.1/txdpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      489 2024-05-27 10:25:14.000000 txdpy-8.9.1/txdpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 10:25:14.000000 txdpy-8.9.1/txdpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2024-05-27 10:25:14.000000 txdpy-8.9.1/txdpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-27 10:25:14.000000 txdpy-8.9.1/txdpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 02:04:10.910848 txdpy-8.9.2/
+-rw-rw-rw-   0        0        0      333 2024-05-30 02:04:10.909848 txdpy-8.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-30 02:04:10.910848 txdpy-8.9.2/setup.cfg
+-rw-rw-rw-   0        0        0      340 2024-05-30 02:04:02.000000 txdpy-8.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 02:04:10.899467 txdpy-8.9.2/txdpy/
+-rw-rw-rw-   0        0        0     3209 2024-05-29 10:04:07.000000 txdpy-8.9.2/txdpy/__init__.py
+-rw-rw-rw-   0        0        0    27787 2024-05-27 09:21:28.000000 txdpy-8.9.2/txdpy/bk_179.py
+-rw-rw-rw-   0        0        0    29024 2024-05-29 08:45:08.000000 txdpy-8.9.2/txdpy/excel数据或mysql操作.py
+-rw-rw-rw-   0        0        0      930 2024-05-27 09:21:28.000000 txdpy-8.9.2/txdpy/列表操作.py
+-rw-rw-rw-   0        0        0     2183 2024-05-27 09:21:28.000000 txdpy-8.9.2/txdpy/字符串类型的判断和提取.py
+-rw-rw-rw-   0        0        0     6238 2024-05-28 08:08:14.000000 txdpy-8.9.2/txdpy/数据库操作.py
+-rw-rw-rw-   0        0        0     5308 2024-05-27 09:21:28.000000 txdpy-8.9.2/txdpy/文本括号及引号不匹配检查.py
+-rw-rw-rw-   0        0        0     5882 2024-05-27 09:21:28.000000 txdpy-8.9.2/txdpy/爬虫辅助功能.py
+-rw-rw-rw-   0        0        0     3556 2024-05-30 02:02:14.000000 txdpy-8.9.2/txdpy/百度ai接口使用.py
+-rw-rw-rw-   0        0        0     2459 2024-05-27 09:21:28.000000 txdpy-8.9.2/txdpy/省市区名称的提取或判断.py
+drwxrwxrwx   0        0        0        0 2024-05-30 02:04:10.908847 txdpy-8.9.2/txdpy.egg-info/
+-rw-rw-rw-   0        0        0      333 2024-05-30 02:04:10.000000 txdpy-8.9.2/txdpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      458 2024-05-30 02:04:10.000000 txdpy-8.9.2/txdpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 02:04:10.000000 txdpy-8.9.2/txdpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2024-05-30 02:04:10.000000 txdpy-8.9.2/txdpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-30 02:04:10.000000 txdpy-8.9.2/txdpy.egg-info/top_level.txt
```

### Comparing `txdpy-8.9.1/txdpy/__init__.py` & `txdpy-8.9.2/txdpy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,11 +53,10 @@
 from .文本括号及引号不匹配检查 import 文本括号及引号不匹配检查
 from .爬虫辅助功能 import req
 from .爬虫辅助功能 import format_string_dict
 from .爬虫辅助功能 import webptablesl
 from .爬虫辅助功能 import dow_file
 from .百度ai接口使用 import TextSimilar
 from .百度ai接口使用 import translate
-from .百度ai接口使用 import 文本错别字检查方法二
+from .百度ai接口使用 import 文本错别字检查
 from .省市区名称的提取或判断 import get_ssq
-from .省市区名称的提取或判断 import is_ssq
-# from .文本错别字检查 import 文本错别字检查方法一
+from .省市区名称的提取或判断 import is_ssq
```

### Comparing `txdpy-8.9.1/txdpy/bk_179.py` & `txdpy-8.9.2/txdpy/bk_179.py`

 * *Files identical despite different names*

### Comparing `txdpy-8.9.1/txdpy/excel数据或mysql操作.py` & `txdpy-8.9.2/txdpy/excel数据或mysql操作.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,14 +87,15 @@
 
 
 def gen_excel(data: list, save_path, header=None, is_optstr=True):
     """生成.xlsx数据文件
     :param data:二维列表数据
     :param save_path:保存为.xlsx文件路径
     :param header:表头以列表形式传入，非必要参数
+    :param is_optstr:文本格式整理默认为 True
     """
     import xlsxwriter
     from tqdm import tqdm
     if header:
         data = list(data)
         data.insert(0, header)
     workbook = xlsxwriter.Workbook(save_path if save_path.endswith('.xlsx') else f'{save_path}.xlsx')
@@ -339,16 +340,15 @@
                 pass
 
 
 class MysqlConn:
     """
     连接Mysql数据库
     """
-
-    def __init__(self, database, config: list = []):
+    def __init__(self, database, config:list= []):
         """
         :param database 数据库名
         :param config 数据库配置[host, port, user, password]
         """
         self.config = config
         self.database = database
         self.cursor = None
@@ -360,34 +360,33 @@
             config = {
                 'host': self.config[0],
                 'port': self.config[1],
                 'user': self.config[2],
                 'password': self.config[3],
                 'db': self.database,
             }
-            self.db = pymysql.connect(**config)  # 连接数据库
+            self.db = pymysql.connect(**config) # 连接数据库
 
-            self.cursor = self.db.cursor()  # 创建游标，用于执行SQL语句
+            self.cursor = self.db.cursor() # 创建游标，用于执行SQL语句
             logger.info("连接数据库成功。")
             return self
         else:
             with open('c:/mysql_config.json', 'r', encoding='utf-8') as f:
-                self.mysql_config = json.load(f)
+                self.mysql_config=json.load(f)
             try:
                 self.server = SSHTunnelForwarder(
                     ssh_address_or_host=eval(self.mysql_config["2"]['ssh_address_or_host']),
                     ssh_username='root',
                     ssh_password=self.mysql_config["2"]['ssh_password'],
                     remote_bind_address=eval(self.mysql_config["2"]['remote_bind_address'])
                 )
                 # 启动隧道服务
                 self.server.start()
-                self.db = pymysql.connect(host='127.0.0.1', port=self.server.local_bind_port,
-                                          user=self.mysql_config["2"]['user'],
-                                          password=self.mysql_config["2"]['passwd'], database=self.database)
+                self.db = pymysql.connect(host='127.0.0.1', port=self.server.local_bind_port, user=self.mysql_config["2"]['user'],
+                                     password=self.mysql_config["2"]['passwd'], database= self.database)
                 self.cursor = self.db.cursor()
                 logger.success("成功连接到MySQL数据库")
             except Error as e:
                 logger.error(f"连接失败: {e}")
             return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
@@ -420,20 +419,21 @@
         if isinstance(params[0], tuple):
             if self.cursor.executemany(sql, params):
                 self.db.commit()
         else:
             if self.cursor.execute(sql, params):
                 self.db.commit()
 
-    def insert(self, table_name, data_pass: Union[dict, List[dict], list, Dict[str, List[Any]]] = None,
-               replace: Union[dict] = None):
+    def insert(self, table_name, data_pass: Union[dict, List[dict], list, Dict[str, List[Any]]]= None, replace:Union[dict]= None, list_increment_id:Union[int]= None, list_insert_field:Union[list]= None):
         """  mysql插入数据/替换数据
         :param table_name 表名
         :param data_pass 接收插入数据，支持以下格式之一： - 单个字典 - 单个列表 - 列表中包含多个列表 - 列表中包含多个字典 - 字典中的值为列表，是所有需要插入的数据 注意：data_pass参数与replace参数互斥，若同时提供，将以replace` 数据为准进行操作。
         :param replace 插入并更新数据，支持以下格式之一：- 单个字典 - 列表中包含多个列表 - 列表中包含多个字典 - 单个列表
+        :param list_increment_id 以列表格式插入所有字段数据时，如果数据中没有自增的值，list_increment_id = 数据库中字段的位置(int)
+        :param list_insert_field 指定列表插入时的字段，例如：["字段1", "字段2"]， 不与list_increment_id参数同时使用
         """
 
         if (not replace and not data_pass) or not self.cursor:
             logger.error(f'数据列表为空或连接未建立')
             return
 
         def detailed_data(keys):
@@ -503,57 +503,52 @@
                         item = detailed_data(keys)
                         sql = f"INSERT INTO {table_name} ({item['columns']}) VALUES ({item['placeholders']})"
                         params = tuple(tuple(item.get(key) for key in keys) for item in data_pass)
                         self.execute_sql(sql, params)
                         logger.success(f"{self.cursor.rowcount} 条数据插入成功")
 
                     # - 多条列表
-                    elif isinstance(data_pass[0], list):  # data_pass 为多条的 list
+                    elif isinstance(data_pass[0], list): # data_pass 为多条的 list
+                        if list_increment_id:
+                            for item in data_pass:
+                                item.insert(list_increment_id-1, 0)
+
                         placeholders = ', '.join(['%s'] * len(data_pass[0]))
                         sql = f"INSERT INTO {table_name} VALUES ({placeholders})"
+
+                        if list_insert_field:
+                            field = ','.join(list_insert_field)
+                            sql = f"INSERT INTO {table_name}({field}) VALUES ({placeholders})"
+
                         params = tuple(tuple(data) for data in data_pass)
 
                         self.execute_sql(sql, params)
                         logger.success(f'{self.cursor.rowcount} 条数据插入成功')
 
                     # - 一个列表
                     else:
+                        if list_increment_id:
+                            data_pass.insert(list_increment_id- 1, 0)
+
                         placeholders = ', '.join(['%s'] * len(data_pass))
                         sql = f"INSERT INTO {table_name} VALUES ({placeholders})"
+                        if list_insert_field:
+                            field = ','.join(list_insert_field)
+                            sql = f"INSERT INTO {table_name}({field}) VALUES ({placeholders})"
+
                         self.execute_sql(sql, tuple(data_pass))
                         logger.success(f'{self.cursor.rowcount} 条数据插入成功')
 
+                # - 单个字典
                 elif isinstance(data_pass, dict):
                     keys = ','.join(data_pass.keys())
                     values = ','.join(['%s'] * len(data_pass))
                     sql = f'INSERT INTO {table_name}({keys}) VALUES({values})'
-
-                    is_list = False
-                    is_len = True
-                    reference_length = len(next(iter(data_pass.values())))
-
-                    for value in data_pass.values():
-                        if len(value) != reference_length:
-                            is_len = False
-
-                    for key, value in data_pass.items():
-                        if isinstance(value, list):
-                            is_list = True
-                        else:
-                            is_list = False
-
-                    if is_list:
-                        if is_len:
-                            if self.cursor.executemany(sql, tuple(zip(*data_pass.values()))):
-                                self.db.commit()
-                        else:
-                            raise ("传入格式错误，列表长度不一致。")
-                    else:
-                        if self.cursor.execute(sql, tuple(data_pass.values())):
-                            self.db.commit()
+                    if self.cursor.execute(sql, tuple(data_pass.values())):
+                        self.db.commit()
 
                     logger.success(f"{self.cursor.rowcount} 条数据插入成功")
 
         except Error as e:
             logger.error(f"插入数据时发生错误: {e}")
 
     def update(self, table_name, match_field, data_pass: Union[dict, List[dict]]):
@@ -599,15 +594,15 @@
 
                 self.execute_sql(sql, params)
                 logger.success(f"{self.cursor.rowcount} 条数据插入成功")
 
         except Error as e:
             logger.error(f"插入数据时发生错误: {e}")
 
-    def select(self, table_name, fields=None, output_format=None):
+    def select(self, table_name, fields=None, output_format= None):
         """  mysql查询数据
         :param table_name 表名
         :param fields 默认查询所有字段, 自定义字段列表传入, fields=['COUNT(*)']查询数据数量
         :param output_format 输出格式，默认输出为list，fields='dict'输出格式为字典
         """
 
         def execute_select(sql):
@@ -637,12 +632,12 @@
 
         # - 查询全部数据
         else:
             columns = self.get_table_columns(table_name)
             results = execute_select(base_query)
             logger.info(f"已查询出所有数据，有{len(results)}条")
 
-            mysql_data = [columns] + [list(row) for row in results]
+            mysql_data = [columns] +[list(row) for row in results]
 
             if output_format == "dict":
                 mysql_data = [{column: value for column, value in zip(mysql_data[0], row)} for row in mysql_data[1:]]
             return mysql_data
```

### Comparing `txdpy-8.9.1/txdpy/列表操作.py` & `txdpy-8.9.2/txdpy/列表操作.py`

 * *Files identical despite different names*

### Comparing `txdpy-8.9.1/txdpy/字符串类型的判断和提取.py` & `txdpy-8.9.2/txdpy/字符串类型的判断和提取.py`

 * *Files identical despite different names*

### Comparing `txdpy-8.9.1/txdpy/数据库操作.py` & `txdpy-8.9.2/txdpy/数据库操作.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -166,8 +166,8 @@
         self.db.close()
         logger.info('数据库连接已断开！')
 
     def except_handl(self, e, sql):
         logger.error(q)
         logger.error(translate(str(e)))
         logger.error(sql)
-        sys.exit()
+        sys.exit()
```

### Comparing `txdpy-8.9.1/txdpy/文本括号及引号不匹配检查.py` & `txdpy-8.9.2/txdpy/文本括号及引号不匹配检查.py`

 * *Files identical despite different names*

### Comparing `txdpy-8.9.1/txdpy/爬虫辅助功能.py` & `txdpy-8.9.2/txdpy/爬虫辅助功能.py`

 * *Files identical despite different names*

### Comparing `txdpy-8.9.1/txdpy/百度ai接口使用.py` & `txdpy-8.9.2/txdpy/百度ai接口使用.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     m = md5()
     m.update((appid + q + salt + secret_key).encode("utf8"))
     s = f'http://api.fanyi.baidu.com/api/trans/vip/translate?q={q}&from=en&to=zh&appid={appid}&salt={salt}&sign={m.hexdigest()}'
     result = get(s).json()
     return result["trans_result"][0]['dst']
 
 
-class 文本错别字检查方法二():
+class 文本错别字检查():
     """
     百度的错别字识别接口
     """
     pass
 
     def __init__(self):
         API_KEY, SECRET_KEY = \
@@ -73,14 +73,15 @@
             post("https://aip.baidubce.com/oauth/2.0/token", params=params).json().get("access_token"))
 
     def __call__(self, 文本):
         """
         :param 文本: 要识别错别字的文本
         :return: [(错误文本,可能正确的文本,错误文本出现的位置),]
         """
+        sleep(.5)
         url = "https://aip.baidubce.com/rpc/2.0/nlp/v1/ecnet?charset=utf-8&access_token=" + self.access_token
         payload = dumps({
             "text": 文本
         })
         headers = {
             'Content-Type': 'application/json',
             'Accept': 'application/json'
```

### Comparing `txdpy-8.9.1/txdpy/省市区名称的提取或判断.py` & `txdpy-8.9.2/txdpy/省市区名称的提取或判断.py`

 * *Files identical despite different names*

