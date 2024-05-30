# Comparing `tmp/bintang-0.1.8-py3-none-any.whl.zip` & `tmp/bintang-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 23071 bytes, number of entries: 14
+Zip file size: 23561 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat       25 b- defN 22-Sep-15 02:00 bintang/__init__.py
 -rw-rw-rw-  2.0 fat     6439 b- defN 22-Jul-05 11:25 bintang/besqlite.py
 -rw-rw-rw-  2.0 fat     1526 b- defN 23-Apr-14 06:25 bintang/cell.py
 -rw-rw-rw-  2.0 fat      566 b- defN 23-Mar-29 02:17 bintang/column.py
--rw-rw-rw-  2.0 fat    24155 b- defN 23-Apr-17 08:28 bintang/core.py
+-rw-rw-rw-  2.0 fat    24160 b- defN 23-Aug-06 23:56 bintang/core.py
 -rw-rw-rw-  2.0 fat     5027 b- defN 23-Apr-14 06:27 bintang/iterdict.py
--rw-rw-rw-  2.0 fat      186 b- defN 23-Apr-17 08:59 bintang/log.py
+-rw-rw-rw-  2.0 fat      186 b- defN 23-Sep-02 04:35 bintang/log.py
 -rw-rw-rw-  2.0 fat     1385 b- defN 23-Apr-12 12:29 bintang/row.py
--rw-rw-rw-  2.0 fat    54492 b- defN 23-Apr-18 13:55 bintang/table.py
--rw-rw-rw-  2.0 fat     1092 b- defN 23-Apr-18 13:57 bintang-0.1.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      249 b- defN 23-Apr-18 13:57 bintang-0.1.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-18 13:57 bintang-0.1.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-18 13:57 bintang-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1043 b- defN 23-Apr-18 13:57 bintang-0.1.8.dist-info/RECORD
-14 files, 96285 bytes uncompressed, 21371 bytes compressed:  77.8%
+-rw-rw-rw-  2.0 fat    56462 b- defN 23-Sep-02 04:29 bintang/table.py
+-rw-rw-rw-  2.0 fat     1092 b- defN 23-Sep-02 04:41 bintang-0.1.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      249 b- defN 23-Sep-02 04:41 bintang-0.1.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Sep-02 04:41 bintang-0.1.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Sep-02 04:41 bintang-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1043 b- defN 23-Sep-02 04:41 bintang-0.1.9.dist-info/RECORD
+14 files, 98260 bytes uncompressed, 21861 bytes compressed:  77.8%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: bintang/row.py
 Comment: 
 
 Filename: bintang/table.py
 Comment: 
 
-Filename: bintang-0.1.8.dist-info/LICENSE
+Filename: bintang-0.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: bintang-0.1.8.dist-info/METADATA
+Filename: bintang-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: bintang-0.1.8.dist-info/WHEEL
+Filename: bintang-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: bintang-0.1.8.dist-info/top_level.txt
+Filename: bintang-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: bintang-0.1.8.dist-info/RECORD
+Filename: bintang-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bintang/core.py

```diff
@@ -131,15 +131,15 @@
 
 
     # def get_columnids(self, tablename, columns):
     #     tableid = self.get_tableid(tablename)
     #     return self.__tables[tableid].get_columnids
     
 
-    def add_table(self,table):
+    def add_table(self,table: str):
         tableid = self.get_tableid(table.name)
         if tableid is None:
             tableid = self.__last_assigned_tableid + 1
             self.__tables[tableid] = table
             self.__last_assigned_tableid = self.__last_assigned_tableid + 1 # update it
         elif tableid is not None:
             raise ValueError('Table {} already exists.'.format(table.name))
```

## bintang/log.py

```diff
@@ -1,6 +1,6 @@
 import logging
 
 log = logging.getLogger(__name__)
 FORMAT = "[%(filename)s:%(lineno)s - %(funcName)10s() ] %(message)s"
 logging.basicConfig(format=FORMAT)
-log.setLevel(logging.DEBUG)
+log.setLevel(logging.ERROR)
```

## bintang/table.py

```diff
@@ -1,8 +1,9 @@
 #from bintang.core import Bintang
+from openpyxl import load_workbook
 from bintang.column import Column
 from bintang.cell import Cell
 from bintang.row import Row
 import json
 import sqlite3
 import uuid
 import re
@@ -35,15 +36,16 @@
     def __init__(self,name, bing=None):
         self.bing = bing
         self.name = name
         self.__columns = {}
         self.__rows = {}
         self.__temprows = []
         self.__last_assigned_columnid= -1 #
-        self.__last_assigned_rowid = -1
+        self.__last_assigned_rowid = -1 # for use when row created
+        self.__last_assigned_idx = -1 # for use when add idx
         self.__be = None
         
 
 
     def __getitem__(self, idx): # subscriptable version of self.get_row_asdict()
         #return self.__rows[idx] # bad design. a raw row isn't that useful at client code
         return self.get_row_asdict(idx)
@@ -190,16 +192,16 @@
         cursor = conn.cursor()
         temp_rows = []
         total_rowcount = 0
         for idx, row in self.iterrows(src_cols, row_type='list'):
             for v in row:
                 temp_rows.append(v)
             if len(temp_rows) == (mrpb * numof_col):
-                # log.debug(prep_stmt)
-                # log.debug(temp_rows)
+                log.debug(prep_stmt)
+                log.debug(temp_rows)
                 cursor.execute(prep_stmt, temp_rows)
                 total_rowcount += cursor.rowcount
                 temp_rows.clear()     
         
         if len(temp_rows) > 0: # if any reminder
             param_markers = self.gen_row_param_markers(numof_col, int(len(temp_rows)/numof_col))
             prep_stmt = sql_template.format(schema,table,",".join(['"{}"'.format(x) for x in dest_columns]),param_markers)
@@ -652,20 +654,24 @@
                     self.__be.add_column(self.name, columnid, column)
                 # deprecated moved up columnid = self.get_columnid(column) # reassign the columnid
         if columnid is None:
             raise ValueError("Cannot make cell due to None column name.")    
         return Cell(columnid,value)
 
 
+    def add_row_deprecated(self,row):
+        rows_idx = len(self.__rows) # can cause re-assign a deleted row
+        self.__rows[rows_idx] = row
 
-
-    def add_row(self,row):
-        rows_idx = len(self.__rows)
+    def add_row(self, row):
+        rows_idx = self.__last_assigned_idx + 1
+        self.__last_assigned_idx += 1
         self.__rows[rows_idx] = row
 
+
     def _XXgen_row_asdict(self, row, columns, rowid=False):
         res = {}
         if rowid == True:
             res['_rowid_'] = row.id # add rowid for internal purpose eg. a merged table
         for column in columns:
             columnid = self.get_columnid(column)
             if columnid not in row.cells:
@@ -1238,51 +1244,91 @@
             columns_ = columns + ['count']
             values = list(k) + [v]
             group_tobj.insert(columns_, values)       
         return group_tobj
     
 
     def DEV_groupby_count(self, columns, count_column):
-        group_tobj = Table('test')
+        group_tobj = Table('testq')
         res_dict = {} #key=a tuple of columns, value=count
         for idx, row in self.iterrows(columns, row_type='list'):
             trow = tuple(row)
             if trow not in res_dict.keys():
                 res_dict[trow] = 1
             else:
                 res_dict[trow] += 1
                 
         for k, v in res_dict.items():
             columns_ = columns + [count_column]
             values = list(k) + [v]
-            group_tobj.insert(columns_, values)       
+            group_tobj.insert(values, columns_,)       
         return group_tobj
     
-    
 
-    def to_excel(self, path, index=False):
+    def read_excel(self, path, sheetname):
+        wb = load_workbook(path, read_only=True, data_only=True)
+        ws = wb[sheetname]
+        columns = []
+        Nonecolumn_cnt = 0
+        for rownum, row_cells in enumerate(ws.iter_rows(),start=1):
+            values = [] # hold column value for each row
+            if rownum == 1:
+                for cell in row_cells:
+                    if cell.value is None:
+                        columname = 'noname' + str(Nonecolumn_cnt)
+                        Nonecolumn_cnt += 1
+                        columns.append(columname)
+                    else:
+                        columns.append(cell.value)
+                if Nonecolumn_cnt > 0:
+                    log.warning('Warning! Noname column detected!')          
+            
+            if rownum > 1:
+                for cell in row_cells:
+                    values.append(cell.value)
+                # if rownum == 370:
+                #     log.debug(f'{values} at rownum 370.')
+                #     log.debug(any(values))
+                if any(values):
+                    self.insert(values, columns)
+        if self.__be is not None:
+            self.add_row_into_be()
+
+
+    def reindex(self):
+        # dict is already indexed with python 3.7+
+        # this only means we rebuild row id so any deleted idx can be reused
+        idxs = list(self.__rows)
+        for i, idx in enumerate(idxs):
+            self.__rows[i] = self.__rows[idx] # reassign
+            if i != idx:
+                del self.__rows[idx]
+            
+
+    def to_excel(self, path, index=False, columns=None):
         from openpyxl import Workbook
         wb = Workbook()
         ws = wb.active
         # add header
-        columns = self.get_columns()
+        if columns is None:
+            columns = self.get_columns()
         log.debug('index: {}'.format(index))
         if index:
             if index == True:
                 columns.insert(0,'_idx')
             if index != True:
                 columns.insert(0,str(index))        
         ws.append(columns)
         # add row
         if index:
-            for idx, row in self.iterrows(row_type='list'):
+            for idx, row in self.iterrows(columns, row_type='list'):
                 row.insert(0,idx)
                 ws.append(row)
         if not index:
-            for idx, row in self.iterrows(row_type='list'):
+            for idx, row in self.iterrows(columns, row_type='list'):
                 ws.append(row)          
         wb.save(path)
 
     def to_list(self, column):
         if isinstance(column, str):
             res_list = []
             for idx, row in self.iterrows([column]):
```

## Comparing `bintang-0.1.8.dist-info/LICENSE` & `bintang-0.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `bintang-0.1.8.dist-info/RECORD` & `bintang-0.1.9.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 bintang/__init__.py,sha256=UIuTaljC0GQNjj4BVS-PnG1uX2B54DR-LKlh14xIHR8,25
 bintang/besqlite.py,sha256=4vfwMAheTgqudMuCH3wlwwWyGJY5aVDd_tmTCiStcJg,6439
 bintang/cell.py,sha256=JW-k_CgYu4nHX3Qk1nTcBP6fkjlsSXMgOuGRz5Dwcs4,1526
 bintang/column.py,sha256=zTMxofr4FXGR95Zcru9G2DlR35e8I3IVifEzOissONM,566
-bintang/core.py,sha256=6rupSkjfpEGcJny5SvdFPg-R5JRgF4L7FxnoKp49FU4,24155
+bintang/core.py,sha256=diEQlZRrHwypsd9IgBPZXnz6iPalPbr_MzDM0J_sw4c,24160
 bintang/iterdict.py,sha256=lTxhrivwbCWhSQNN_TrPWaCg2QyeKa9vqf0X5j3vv2M,5027
-bintang/log.py,sha256=N6LImpolwYOJn4zW-nEpX6o63gInJKSzsw2NKM9V1sE,186
+bintang/log.py,sha256=JpOMYVUbQ4UcNSkt3MbjbUhgLH2mE3ZcywuPrJuaAPI,186
 bintang/row.py,sha256=I63-FY9p-lxmaeOOutKQbF9-jOPC3fTW-6frTqmzBOc,1385
-bintang/table.py,sha256=LEw0csB_23VOa7CPuWDlINwC7FiASF3W2cJZtDQSC1k,54492
-bintang-0.1.8.dist-info/LICENSE,sha256=nDP3WePgnPckoI4QkIfBpSx_ZNsectSpMKuVHjBb_68,1092
-bintang-0.1.8.dist-info/METADATA,sha256=PMIaoNjASUMd3I1-YoQ5eLO2De0G5fs3IfWALLXXLNo,249
-bintang-0.1.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-bintang-0.1.8.dist-info/top_level.txt,sha256=I6MnAK-RhSd0NBsMpB51A4oOOs3-EjdS3IldTjtaR3I,8
-bintang-0.1.8.dist-info/RECORD,,
+bintang/table.py,sha256=0H7GbKYhosSd1KhvFHJa0aZD9CD0UwqB1a6SPOhodv8,56462
+bintang-0.1.9.dist-info/LICENSE,sha256=nDP3WePgnPckoI4QkIfBpSx_ZNsectSpMKuVHjBb_68,1092
+bintang-0.1.9.dist-info/METADATA,sha256=WEPUluCfbQUtx-58L-eiQkXdWXfVKQVs1nqW_zkfBNM,249
+bintang-0.1.9.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+bintang-0.1.9.dist-info/top_level.txt,sha256=I6MnAK-RhSd0NBsMpB51A4oOOs3-EjdS3IldTjtaR3I,8
+bintang-0.1.9.dist-info/RECORD,,
```

