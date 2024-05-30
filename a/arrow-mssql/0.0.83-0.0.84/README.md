# Comparing `tmp/arrow_mssql-0.0.83.tar.gz` & `tmp/arrow_mssql-0.0.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arrow_mssql-0.0.83.tar", max compression
+gzip compressed data, was "arrow_mssql-0.0.84.tar", max compression
```

## Comparing `arrow_mssql-0.0.83.tar` & `arrow_mssql-0.0.84.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      188 2024-05-27 17:56:55.897440 arrow_mssql-0.0.83/arrow_mssql/__init__.py
--rw-r--r--   0        0        0     1425 2024-05-27 17:31:29.732859 arrow_mssql-0.0.83/arrow_mssql/connector.py
--rw-r--r--   0        0        0     3649 2024-05-27 17:56:59.114932 arrow_mssql-0.0.83/arrow_mssql/export.py
--rw-r--r--   0        0        0        0 2024-04-02 17:17:13.445964 arrow_mssql-0.0.83/arrow_mssql/input/__init__.py
--rw-r--r--   0        0        0     3600 2024-05-27 17:30:02.243740 arrow_mssql-0.0.83/arrow_mssql/input/datatypes.py
--rw-r--r--   0        0        0     1568 2024-05-27 16:34:31.830782 arrow_mssql-0.0.83/arrow_mssql/input/schema.py
--rw-r--r--   0        0        0     2240 2024-05-27 17:55:00.270584 arrow_mssql-0.0.83/arrow_mssql/iport.py
--rw-r--r--   0        0        0        0 2024-04-02 17:15:34.399775 arrow_mssql-0.0.83/arrow_mssql/output/__init__.py
--rw-r--r--   0        0        0     2553 2024-04-02 19:07:18.402978 arrow_mssql-0.0.83/arrow_mssql/output/datatypes.py
--rw-r--r--   0        0        0     3435 2024-04-02 17:14:32.689965 arrow_mssql-0.0.83/arrow_mssql/output/schemas.py
--rw-r--r--   0        0        0      718 2024-03-18 12:53:20.396252 arrow_mssql-0.0.83/arrow_mssql/utils.py
--rw-r--r--   0        0        0      755 2024-05-27 15:40:06.339505 arrow_mssql-0.0.83/pyproject.toml
--rw-r--r--   0        0        0     1942 2024-05-27 17:56:52.708336 arrow_mssql-0.0.83/README.md
--rw-r--r--   0        0        0     2666 1970-01-01 00:00:00.000000 arrow_mssql-0.0.83/PKG-INFO
+-rw-r--r--   0        0        0      230 2024-05-30 14:07:07.356706 arrow_mssql-0.0.84/arrow_mssql/__init__.py
+-rw-r--r--   0        0        0     1495 2024-05-30 06:49:03.295448 arrow_mssql-0.0.84/arrow_mssql/connector.py
+-rw-r--r--   0        0        0     3649 2024-05-30 06:47:17.899533 arrow_mssql-0.0.84/arrow_mssql/export.py
+-rw-r--r--   0        0        0        0 2024-04-02 17:17:13.445964 arrow_mssql-0.0.84/arrow_mssql/input/__init__.py
+-rw-r--r--   0        0        0     3619 2024-05-30 05:25:47.723508 arrow_mssql-0.0.84/arrow_mssql/input/datatypes.py
+-rw-r--r--   0        0        0     1568 2024-05-30 04:43:07.457746 arrow_mssql-0.0.84/arrow_mssql/input/schema.py
+-rw-r--r--   0        0        0     4180 2024-05-30 14:05:44.941743 arrow_mssql-0.0.84/arrow_mssql/iport.py
+-rw-r--r--   0        0        0        0 2024-04-02 17:15:34.399775 arrow_mssql-0.0.84/arrow_mssql/output/__init__.py
+-rw-r--r--   0        0        0     2553 2024-05-30 04:42:54.595401 arrow_mssql-0.0.84/arrow_mssql/output/datatypes.py
+-rw-r--r--   0        0        0     3435 2024-04-02 17:14:32.689965 arrow_mssql-0.0.84/arrow_mssql/output/schemas.py
+-rw-r--r--   0        0        0      718 2024-05-30 06:33:35.765808 arrow_mssql-0.0.84/arrow_mssql/utils.py
+-rw-r--r--   0        0        0      763 2024-05-30 13:59:14.199460 arrow_mssql-0.0.84/pyproject.toml
+-rw-r--r--   0        0        0     2079 2024-05-30 14:08:27.989597 arrow_mssql-0.0.84/README.md
+-rw-r--r--   0        0        0     2806 1970-01-01 00:00:00.000000 arrow_mssql-0.0.84/PKG-INFO
```

### Comparing `arrow_mssql-0.0.83/arrow_mssql/connector.py` & `arrow_mssql-0.0.84/arrow_mssql/connector.py`

 * *Files 26% similar despite different names*

```diff
@@ -42,19 +42,20 @@
     )
 
     con.add_output_converter(
         -155, 
         datetimeoffset_to_datetime
     )
     
-    con.execute(
-        'set transaction '
-        'isolation level '
-        'read uncommitted;'
+    con.autocommit = True
+    con.set_attr(
+        odbc.SQL_ATTR_TXN_ISOLATION,
+        odbc.SQL_TXN_READ_UNCOMMITTED
     )
+    con.autocommit = False # habilita transacoes
 
     with closing(con.cursor()) as cur:
         cur.execute("SET DATEFIRST 1")
 
     return con
```

### Comparing `arrow_mssql-0.0.83/arrow_mssql/export.py` & `arrow_mssql-0.0.84/arrow_mssql/export.py`

 * *Files identical despite different names*

### Comparing `arrow_mssql-0.0.83/arrow_mssql/input/datatypes.py` & `arrow_mssql-0.0.84/arrow_mssql/input/datatypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
     pa.float16(): 'real',
     pa.float32(): 'real',
     pa.float64(): 'float',
     pa.date32(): 'date',
     pa.date64(): 'date',
     pa.string(): 'varchar(max)',
     pa.utf8(): 'varchar(max)',
-    pa.binary(): 'binary',
+    pa.binary(): 'varbinary(max)',
 }
 
 map_typs_pyodbc = {
     pa.int8(): pyodbc.SQL_TINYINT,
     pa.int16(): pyodbc.SQL_SMALLINT,
     pa.int32(): pyodbc.SQL_INTEGER,
     pa.int64(): pyodbc.SQL_BIGINT,
@@ -132,9 +132,9 @@
     pa.float16(): pyodbc.SQL_REAL,
     pa.float32(): pyodbc.SQL_REAL,
     pa.float64(): pyodbc.SQL_FLOAT,
     pa.date32(): pyodbc.SQL_TYPE_DATE,
     pa.date64(): pyodbc.SQL_TYPE_DATE,
     pa.string(): (pyodbc.SQL_VARCHAR, 0, 0),
     pa.utf8(): (pyodbc.SQL_VARCHAR, 0, 0),
-    pa.binary(): pyodbc.SQL_BINARY,
+    pa.binary(): (pyodbc.SQL_VARBINARY, 0, 0),
 }
```

### Comparing `arrow_mssql-0.0.83/arrow_mssql/input/schema.py` & `arrow_mssql-0.0.84/arrow_mssql/input/schema.py`

 * *Files identical despite different names*

### Comparing `arrow_mssql-0.0.83/arrow_mssql/output/datatypes.py` & `arrow_mssql-0.0.84/arrow_mssql/output/datatypes.py`

 * *Files identical despite different names*

### Comparing `arrow_mssql-0.0.83/arrow_mssql/output/schemas.py` & `arrow_mssql-0.0.84/arrow_mssql/output/schemas.py`

 * *Files identical despite different names*

### Comparing `arrow_mssql-0.0.83/arrow_mssql/utils.py` & `arrow_mssql-0.0.84/arrow_mssql/utils.py`

 * *Files identical despite different names*

### Comparing `arrow_mssql-0.0.83/pyproject.toml` & `arrow_mssql-0.0.84/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "arrow-mssql"
-version = "0.0.83"
-description = "Arrow-mssql exporta tabela ou consulta para .parquet ou .csv, e também faz a leitura de .parquet para tabela do sql server"
+version = "0.0.84"
+description = "Arrow-mssql exporta tabela ou consulta para .parquet ou .csv, e também faz a leitura de .parquet ou .csv para tabela do sql server"
 authors = ["Marcus Holanda <mvsh777@hotmail.com>"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 1 - Planning",
     "Natural Language :: Portuguese (Brazilian)",
     "Programming Language :: PL/SQL",
     "Programming Language :: Python :: 3.11"
```

### Comparing `arrow_mssql-0.0.83/README.md` & `arrow_mssql-0.0.84/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Arrow-mssql
 [![PyPI](https://img.shields.io/pypi/v/arrow-mssql.svg)](https://pypi.org/project/arrow-mssql/)
 
 ## O que é o Arrow-mssql ?
 
-é um projeto que recebe uma tabela ou consulta do `SQL SERVER`
+É um projeto que recebe uma tabela ou consulta do `SQL SERVER`
 e faz a exportação para um arquivo *.parquet* ou *.csv*,
 utilizando a solução [arrow](https://arrow.apache.org/docs/index.html) que é uma tecnologia com
 foco em análise e desempenho na memória.
 
-Agora é possível importar um arquivo *.parquet* para uma tabela do sql server.
+Também é possível importar um arquivo *.parquet* para uma tabela do sql server ou arquivo *.csv*.
 
 ## Instalação
 
 ```bash
 pip install arrow-mssql
 ```
 
@@ -54,15 +54,20 @@
 to_parquet(
     DRIVER, 
     'SELECT N1, N2 FROM NOME_TABELA WHERE N1 = 0', 
     schema='dbo',
     database='seu_banco', 
     path='destino.parquet'
 )
+```
+
+É possivel importar arquivos csv ou parquet, definir um limite de linhas
+e colunas no processo.
 
+```python
 # IMPORTAR .parquet para tabela temporaria do ssms
 # o retornor é um cursor referente a conexao com o banco de dados
 with write_parquet(
     DRIVER, 
     '##teste', 
     path='origem.parquet'
 ) as C:
```

### Comparing `arrow_mssql-0.0.83/PKG-INFO` & `arrow_mssql-0.0.84/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: arrow-mssql
-Version: 0.0.83
-Summary: Arrow-mssql exporta tabela ou consulta para .parquet ou .csv, e também faz a leitura de .parquet para tabela do sql server
+Version: 0.0.84
+Summary: Arrow-mssql exporta tabela ou consulta para .parquet ou .csv, e também faz a leitura de .parquet ou .csv para tabela do sql server
 Author: Marcus Holanda
 Author-email: mvsh777@hotmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 1 - Planning
 Classifier: Natural Language :: Portuguese (Brazilian)
 Classifier: Programming Language :: PL/SQL
 Classifier: Programming Language :: Python :: 3
@@ -18,20 +18,20 @@
 Description-Content-Type: text/markdown
 
 # Arrow-mssql
 [![PyPI](https://img.shields.io/pypi/v/arrow-mssql.svg)](https://pypi.org/project/arrow-mssql/)
 
 ## O que é o Arrow-mssql ?
 
-é um projeto que recebe uma tabela ou consulta do `SQL SERVER`
+É um projeto que recebe uma tabela ou consulta do `SQL SERVER`
 e faz a exportação para um arquivo *.parquet* ou *.csv*,
 utilizando a solução [arrow](https://arrow.apache.org/docs/index.html) que é uma tecnologia com
 foco em análise e desempenho na memória.
 
-Agora é possível importar um arquivo *.parquet* para uma tabela do sql server.
+Também é possível importar um arquivo *.parquet* para uma tabela do sql server ou arquivo *.csv*.
 
 ## Instalação
 
 ```bash
 pip install arrow-mssql
 ```
 
@@ -73,15 +73,20 @@
 to_parquet(
     DRIVER, 
     'SELECT N1, N2 FROM NOME_TABELA WHERE N1 = 0', 
     schema='dbo',
     database='seu_banco', 
     path='destino.parquet'
 )
+```
+
+É possivel importar arquivos csv ou parquet, definir um limite de linhas
+e colunas no processo.
 
+```python
 # IMPORTAR .parquet para tabela temporaria do ssms
 # o retornor é um cursor referente a conexao com o banco de dados
 with write_parquet(
     DRIVER, 
     '##teste', 
     path='origem.parquet'
 ) as C:
```

