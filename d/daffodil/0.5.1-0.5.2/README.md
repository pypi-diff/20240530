# Comparing `tmp/daffodil-0.5.1.tar.gz` & `tmp/daffodil-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daffodil-0.5.1.tar", last modified: Sat May 25 15:36:10 2024, max compression
+gzip compressed data, was "daffodil-0.5.2.tar", last modified: Thu May 30 15:06:53 2024, max compression
```

## Comparing `daffodil-0.5.1.tar` & `daffodil-0.5.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 15:36:10.988795 daffodil-0.5.1/
--rw-rw-rw-   0        0        0     1090 2024-02-28 17:20:31.000000 daffodil-0.5.1/LICENSE
--rw-rw-rw-   0        0        0    54140 2024-05-25 15:36:10.983788 daffodil-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0    53485 2024-05-23 19:59:10.000000 daffodil-0.5.1/README.md
--rw-rw-rw-   0        0        0      819 2024-05-25 15:04:51.000000 daffodil-0.5.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-25 15:36:10.988795 daffodil-0.5.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-25 15:36:10.860789 daffodil-0.5.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-25 15:36:10.886788 daffodil-0.5.1/src/daffodil/
--rw-rw-rw-   0        0        0        4 2024-05-02 03:32:58.000000 daffodil-0.5.1/src/daffodil/__init__.py
--rw-rw-rw-   0        0        0   221695 2024-05-25 15:29:13.000000 daffodil-0.5.1/src/daffodil/daf.py
--rw-rw-rw-   0        0        0    10430 2024-05-15 18:08:46.000000 daffodil-0.5.1/src/daffodil/keyedlist.py
-drwxrwxrwx   0        0        0        0 2024-05-25 15:36:10.960787 daffodil-0.5.1/src/daffodil/lib/
--rw-rw-rw-   0        0        0        4 2024-05-02 03:32:58.000000 daffodil-0.5.1/src/daffodil/lib/__init__.py
--rw-rw-rw-   0        0        0    41798 2024-05-25 15:02:12.000000 daffodil-0.5.1/src/daffodil/lib/daf_indexing.py
--rw-rw-rw-   0        0        0    31645 2024-05-02 16:49:22.000000 daffodil-0.5.1/src/daffodil/lib/daf_md.py
--rw-rw-rw-   0        0        0     7708 2024-05-02 16:49:22.000000 daffodil-0.5.1/src/daffodil/lib/daf_pandas.py
--rw-rw-rw-   0        0        0     5174 2024-05-02 03:32:58.000000 daffodil-0.5.1/src/daffodil/lib/daf_types.py
--rw-rw-rw-   0        0        0    51588 2024-05-20 23:41:53.000000 daffodil-0.5.1/src/daffodil/lib/daf_utils.py
--rw-rw-rw-   0        0        0     5796 2024-05-02 03:32:58.000000 daffodil-0.5.1/src/daffodil/lib/md_demo.py
-drwxrwxrwx   0        0        0        0 2024-05-25 15:36:10.980789 daffodil-0.5.1/src/daffodil.egg-info/
--rw-rw-rw-   0        0        0    54140 2024-05-25 15:36:10.000000 daffodil-0.5.1/src/daffodil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      532 2024-05-25 15:36:10.000000 daffodil-0.5.1/src/daffodil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 15:36:10.000000 daffodil-0.5.1/src/daffodil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-05-25 15:36:10.000000 daffodil-0.5.1/src/daffodil.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-25 15:36:10.000000 daffodil-0.5.1/src/daffodil.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-25 15:36:10.971797 daffodil-0.5.1/tests/
--rw-rw-rw-   0        0        0   164590 2024-05-15 19:07:31.000000 daffodil-0.5.1/tests/test_daf.py
--rw-rw-rw-   0        0        0     2202 2024-05-09 16:48:49.000000 daffodil-0.5.1/tests/test_keyedlist.py
+drwxrwxrwx   0        0        0        0 2024-05-30 15:06:53.459042 daffodil-0.5.2/
+-rw-rw-rw-   0        0        0     1090 2024-02-28 17:20:31.000000 daffodil-0.5.2/LICENSE
+-rw-rw-rw-   0        0        0    54140 2024-05-30 15:06:53.453045 daffodil-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0    53485 2024-05-23 19:59:10.000000 daffodil-0.5.2/README.md
+-rw-rw-rw-   0        0        0      819 2024-05-30 15:00:18.000000 daffodil-0.5.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-30 15:06:53.460042 daffodil-0.5.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-30 15:06:53.370531 daffodil-0.5.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-30 15:06:53.392045 daffodil-0.5.2/src/daffodil/
+-rw-rw-rw-   0        0        0        4 2024-05-02 03:32:58.000000 daffodil-0.5.2/src/daffodil/__init__.py
+-rw-rw-rw-   0        0        0   224810 2024-05-30 14:48:52.000000 daffodil-0.5.2/src/daffodil/daf.py
+-rw-rw-rw-   0        0        0    10430 2024-05-15 18:08:46.000000 daffodil-0.5.2/src/daffodil/keyedlist.py
+drwxrwxrwx   0        0        0        0 2024-05-30 15:06:53.437045 daffodil-0.5.2/src/daffodil/lib/
+-rw-rw-rw-   0        0        0        4 2024-05-02 03:32:58.000000 daffodil-0.5.2/src/daffodil/lib/__init__.py
+-rw-rw-rw-   0        0        0    41798 2024-05-25 15:02:12.000000 daffodil-0.5.2/src/daffodil/lib/daf_indexing.py
+-rw-rw-rw-   0        0        0    31645 2024-05-02 16:49:22.000000 daffodil-0.5.2/src/daffodil/lib/daf_md.py
+-rw-rw-rw-   0        0        0     7708 2024-05-02 16:49:22.000000 daffodil-0.5.2/src/daffodil/lib/daf_pandas.py
+-rw-rw-rw-   0        0        0     5174 2024-05-02 03:32:58.000000 daffodil-0.5.2/src/daffodil/lib/daf_types.py
+-rw-rw-rw-   0        0        0    51786 2024-05-29 19:25:28.000000 daffodil-0.5.2/src/daffodil/lib/daf_utils.py
+-rw-rw-rw-   0        0        0     5796 2024-05-02 03:32:58.000000 daffodil-0.5.2/src/daffodil/lib/md_demo.py
+drwxrwxrwx   0        0        0        0 2024-05-30 15:06:53.448043 daffodil-0.5.2/src/daffodil.egg-info/
+-rw-rw-rw-   0        0        0    54140 2024-05-30 15:06:53.000000 daffodil-0.5.2/src/daffodil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2024-05-30 15:06:53.000000 daffodil-0.5.2/src/daffodil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 15:06:53.000000 daffodil-0.5.2/src/daffodil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-05-30 15:06:53.000000 daffodil-0.5.2/src/daffodil.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-30 15:06:53.000000 daffodil-0.5.2/src/daffodil.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 15:06:53.444040 daffodil-0.5.2/tests/
+-rw-rw-rw-   0        0        0   166877 2024-05-29 16:36:30.000000 daffodil-0.5.2/tests/test_daf.py
+-rw-rw-rw-   0        0        0     2202 2024-05-09 16:48:49.000000 daffodil-0.5.2/tests/test_keyedlist.py
```

### Comparing `daffodil-0.5.1/LICENSE` & `daffodil-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `daffodil-0.5.1/PKG-INFO` & `daffodil-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daffodil
-Version: 0.5.1
+Version: 0.5.2
 Summary: Daffodil provides lightweight and fast 2-D dataframes
 Author-email: Ray Lutz <raylutz@cognisys.com>
 License: MIT
 Project-URL: Homepage, https://github.com/raylutz/daffodil
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `daffodil-0.5.1/README.md` & `daffodil-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `daffodil-0.5.1/pyproject.toml` & `daffodil-0.5.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "daffodil"
-version = "0.5.1"
+version = "0.5.2"
 authors = [
     {name = "Ray Lutz", email = "raylutz@cognisys.com"},
 ]
 description = "Daffodil provides lightweight and fast 2-D dataframes"
 readme = "README.md"
 requires-python = ">=3.6"
```

### Comparing `daffodil-0.5.1/src/daffodil/daf.py` & `daffodil-0.5.2/src/daffodil/daf.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,16 +228,25 @@
             Updated documentation to reflect new approach to dtypes and flattening.
              
     v0.5.1  (2024-05-25)
             changed dependencies in pyproject.toml so they would allow newer versions.
             Upgraded to Python 3.11 and upgraded all libraries to the latest.
             Using venv311
     
-    v0.5.2  (pending)
-    
+    v0.5.2  (2024-05-30)
+            Added .iter_dict() and .iter_klist() to force iteration to produce either dicts or KeyedLists.
+                Producing KeyedLists means the list is not copied into a dict but can be mutated and the lol will be mutated.
+            Correct calculation of slice_len to correct column assignment from another column
+                This may still have some ambiguity if a nested list structure is meant to be assigned to an array cell.
+                    collist = my_daf[:, 'colname'].to_list()    # this will return a list, but sometimes of only one value.
+                    my_daf[:, 'colname2'] = collist             # there is ambiguity here as to whether the list with one
+                                                                # item should be placed in the cell or if just the value.
+                
+    v0.5.3  (pending)            
+            
             
             
     TODO
             add use of pickledjson to express contents of individual cells when not jsonable.
             tests: need to add
                 __str__ and __repr__
                 
@@ -377,25 +386,26 @@
                 python test_keyedlist.py
                 python daf_demo.py
                 python daf_benchmarks.py
         2. Increment version number in pyproject.toml
         3. Remove prior release
                 rm -r dist
         3. build the release
+                pip install --upgrade build
                 python -m build
         4. Upload it
                 twine upload dist/*
                 
      
     venv311\Scripts\activate     
 """       
     
     
-#VERSION  = 'v0.5.1'
-#VERSDATE = '2024-05-25'  
+#VERSION  = 'v0.5.2'
+#VERSDATE = '2024-05-30'  
 
 import os
 import sys
 import io
 import csv
 import copy
 import re
@@ -410,15 +420,15 @@
 import daffodil.lib.daf_utils    as utils
 import daffodil.lib.daf_md       as md
 import daffodil.lib.daf_pandas   as daf_pandas
 
 from daffodil.keyedlist import KeyedList
 
 
-from typing import List, Dict, Any, Tuple, Optional, Union, cast, Type, Callable, Iterable #
+from typing import List, Dict, Any, Tuple, Optional, Union, cast, Type, Callable, Iterable, Iterator #
 def fake_function(a: Optional[List[Dict[str, Tuple[int,Union[Any, str]]]]] = None) -> Optional[int]:
     return None or cast(int, 0)       # pragma: no cover
 
 T_Pydf = Type['Daf']
 T_Daf = Type['Daf']
 T_dodaf = Dict[str, T_Daf]
 
@@ -534,33 +544,47 @@
     @itermode.setter
     def itermode(self, new_itermode):
         if new_itermode in [self.ITERMODE_DICT, self.ITERMODE_KEYEDLIST]:
             self._itermode = new_itermode
         else:
             raise ValueError("Invalid itermode")
 
-    def __iter__(self):
-        self._iter_index = 0
-        return self
-
-    def __next__(self) -> Union[Dict[str, int], KeyedList]:
-        if self._iter_index < len(self.lol):
-            if self._itermode == self.ITERMODE_DICT:
-                row_dict = dict(zip(self.hd.keys(), self.lol[self._iter_index]))
-                self._iter_index += 1
-                return row_dict
-            elif self._itermode == self.ITERMODE_KEYEDLIST:
-                row_klist = KeyedList(self.hd, self.lol[self._iter_index])
-                self._iter_index += 1
-                return row_klist
-            else:
-                raise NotImplementedError
+    def __iter__(self) -> Iterator[Union[Dict[str, Any], KeyedList]]:
+        return self._default_iterator()
+        
+    def _default_iterator(self) -> Iterator[Union[Dict[str, Any], KeyedList]]:
+        if self._itermode == self.ITERMODE_DICT:
+            return self.iter_dict()
+        elif self._itermode == self.ITERMODE_KEYEDLIST:
+            return self.iter_klist()
         else:
-            self._iter_index = 0
-            raise StopIteration
+            raise ValueError(f"Invalid iteration mode: {self._itermode}")
+
+    def iter_dict(self) -> Iterator[Dict[str, Any]]:
+        return DafIterator(self, dict)
+
+    def iter_klist(self) -> Iterator[KeyedList]:
+        return DafIterator(self, KeyedList)
+        
+
+    # def __next__(self) -> Union[Dict[str, int], KeyedList]:
+        # if self._iter_index < len(self.lol):
+            # if self._itermode == self.ITERMODE_DICT:
+                # row_dict = dict(zip(self.hd.keys(), self.lol[self._iter_index]))
+                # self._iter_index += 1
+                # return row_dict
+            # elif self._itermode == self.ITERMODE_KEYEDLIST:
+                # row_klist = KeyedList(self.hd, self.lol[self._iter_index])
+                # self._iter_index += 1
+                # return row_klist
+            # else:
+                # raise NotImplementedError
+        # else:
+            # self._iter_index = 0
+            # raise StopIteration
 
     def __bool__(self):
         """ test daf for existance and not empty 
             test exists in test_daf.py 
 
             if self is a single value, test the value.  # not implemented.
             
@@ -2151,17 +2175,20 @@
             
             mutates existing daf
         """
         if icols is None:
             icols = []
         if irows is None:
             irows = []
+            
+        tot_num_cols = self.num_cols()    
+        tot_num_rows = self.num_rows()    
         
-        num_irows = utils.len_rowcol_spec(irows)
-        num_icols = utils.len_rowcol_spec(icols)
+        num_irows = utils.len_rowcol_spec(irows, tot_num_rows)
+        num_icols = utils.len_rowcol_spec(icols, tot_num_cols)
         
         if num_irows == 1 and isinstance(irows, int):
             irows = [irows]
         if num_icols == 1 and isinstance(icols, int):
             icols = [icols]
             
         if isinstance(irows, slice):
@@ -2187,14 +2214,22 @@
         if num_irows == 1 and num_icols == 1:
         
             irow = irows[0]
             icol = icols[0]
             
             if isinstance(value, dict):
                 self.assign_record_irow(irow, record=value)
+            elif isinstance(value, list) and len(value) == 1:    
+                # frequently, we will have a list generated from a selection of a column, and it it has only one value
+                # it needs to be entered in the array location, but not as a list.
+                # place a list with only one item in a cell can't be done this way:
+                
+                # my_daf[0,0] = [4]   # this will insert 4 not [4]
+            
+                self.lol[irow][icol] = value[0]
             else:    
                 self.lol[irow][icol] = value
                 
         elif num_irows > 1 and num_icols == 0:
             
             if isinstance(value, list):
                 for irow in irows:
@@ -2215,18 +2250,19 @@
             icol = icols[0]
         
             if irows is None:
                 irows = range(len(self.lol))
         
             if isinstance(value, list):
                 for source_idx, irow in enumerate(irows):
+                    
                     try:
                         self.lol[irow][icol] = value[source_idx]
                     except Exception:
-                        import pdb; pdb.set_trace() #temp
+                        breakpoint() #temp
                     
             # elif isinstance(value, dict):
                 # # this is the same as cols=0 bc dict updates the corresponding cols.
                 # for irow in irows:
                     # self.assign_record_irow(irow, record=value)
                 
             elif isinstance(value, type(self)):
@@ -2653,14 +2689,16 @@
                 if irow, specified, ignore icol.
                 if irow=None and icol specified, then use icol.
         """
     
         num_rows, num_cols = self.shape()
 
         if irow is None and icol is None:
+            # no explicit irow or icol specified, this is the normal case
+            
             if num_rows == 1 and num_cols >= 1:
                 # single row, return as list.
                 result_la = self.lol[0]
                     
             elif num_rows > 1 and num_cols == 1:
                 # single column result as a list.
                 result_la = self.icol(0)
@@ -5517,7 +5555,30 @@
 Pydf.gen_stats_pydf          = Daf.gen_stats_daf
 Pydf.value_counts_pydf       = Daf.value_counts_daf
 
 Daf.groupsum                 = Daf.groupsum_daf
 
 Pydf.md_pydf_table = Pydf.to_md            
 
+
+class DafIterator:
+    def __init__(self, this_daf: Daf, rtype: Type[Union[Dict[str, Any], KeyedList]]):
+        self.this_daf = this_daf
+        self.rtype = rtype
+        self._index = 0
+
+    def __iter__(self):
+        return self
+
+    def __next__(self) -> Union[Dict[str, Any], KeyedList]:
+        if self._index < len(self.this_daf.lol):
+            row = self.this_daf.lol[self._index]
+            self._index += 1
+            if self.rtype == dict:
+                return dict(zip(self.this_daf.hd.keys(), row))
+            elif self.rtype == KeyedList:
+                return KeyedList(self.this_daf.hd, row)
+            else:
+                raise NotImplementedError(f"Unknown return type: {self.rtype}")
+        else:
+            self._index = 0
+            raise StopIteration
```

### Comparing `daffodil-0.5.1/src/daffodil/keyedlist.py` & `daffodil-0.5.2/src/daffodil/keyedlist.py`

 * *Files identical despite different names*

### Comparing `daffodil-0.5.1/src/daffodil/lib/daf_indexing.py` & `daffodil-0.5.2/src/daffodil/lib/daf_indexing.py`

 * *Files identical despite different names*

### Comparing `daffodil-0.5.1/src/daffodil/lib/daf_md.py` & `daffodil-0.5.2/src/daffodil/lib/daf_md.py`

 * *Files identical despite different names*

### Comparing `daffodil-0.5.1/src/daffodil/lib/daf_pandas.py` & `daffodil-0.5.2/src/daffodil/lib/daf_pandas.py`

 * *Files identical despite different names*

### Comparing `daffodil-0.5.1/src/daffodil/lib/daf_types.py` & `daffodil-0.5.2/src/daffodil/lib/daf_types.py`

 * *Files identical despite different names*

### Comparing `daffodil-0.5.1/src/daffodil/lib/daf_utils.py` & `daffodil-0.5.2/src/daffodil/lib/daf_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1397,35 +1397,43 @@
 
 def is_list_of_type(test_item: Any, of_type: Type) -> bool:
 
     # test if test_item is T_ls and it is not empty.
 
     if test_item and isinstance(test_item, list) and isinstance(test_item[0], of_type):
         return True
+        
 
-def len_slice(slice_obj: slice):
-    # Calculate the length of the slice, including step
+def len_slice(slice_obj: slice, tot_len: int=0):
+    """ Calculate the length of the slice, including step 
+    
+        tot_len should be the total length of the sliced object.    
+    """
     
     if slice_obj == slice(None, None, None):
         return 0
         
-    start, stop, step = slice_obj.start or 0, slice_obj.stop or 0, slice_obj.step or 1
+    start, stop, step = slice_obj.start or 0, slice_obj.stop or tot_len, slice_obj.step or 1
     
     try:
         len_int = (stop - start + step - 1) // step
     except Exception:
-        import pdb; pdb.set_trace() #perm
+        breakpoint() #perm
         
     return len_int
+    
 
-def len_rowcol_spec(ispec: Union[slice, int, T_li, None]) -> int:
-    """ return the length of a slice, int, li. If None, then len = 0 """
+def len_rowcol_spec(ispec: Union[slice, int, T_li, None], tot_len: int) -> int:
+    """ return the length of a slice, int, li. If None, then len = 0 
+    
+        returns -1 if the length is not terminated
+    """
     
     if isinstance(ispec, slice):
-        return len_slice(ispec)
+        return len_slice(ispec, tot_len)
     elif isinstance(ispec, int):
         return 1
     elif isinstance(ispec, list):
         return len(ispec)
     else:
         return 0
```

### Comparing `daffodil-0.5.1/src/daffodil/lib/md_demo.py` & `daffodil-0.5.2/src/daffodil/lib/md_demo.py`

 * *Files identical despite different names*

### Comparing `daffodil-0.5.1/src/daffodil.egg-info/PKG-INFO` & `daffodil-0.5.2/src/daffodil.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daffodil
-Version: 0.5.1
+Version: 0.5.2
 Summary: Daffodil provides lightweight and fast 2-D dataframes
 Author-email: Ray Lutz <raylutz@cognisys.com>
 License: MIT
 Project-URL: Homepage, https://github.com/raylutz/daffodil
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `daffodil-0.5.1/src/daffodil.egg-info/SOURCES.txt` & `daffodil-0.5.2/src/daffodil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `daffodil-0.5.1/tests/test_daf.py` & `daffodil-0.5.2/tests/test_daf.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #from io import BytesIO
 from pathlib import Path
 
 import sys
 sys.path.append(os.path.join(os.path.dirname(sys.path[0]), 'src'))
 
 from daffodil.daf import Daf
+from daffodil.keyedlist import KeyedList
 from daffodil.lib import daf_utils as utils
 
 class TestDaf(unittest.TestCase):
 
     maxDiff = None
     
     # initialization
@@ -3929,10 +3930,75 @@
         # Test the handling of identifier columns
         wide_daf = narrow_daf.narrow_to_wide(id_cols=['ID'], varname_col='varname', value_col='value')
         self.assertEqual(len(wide_daf.columns()), 3)  # ID, A, B
         
         # Add more assertions based on the expected handling of identifier columns
         
 
+class TestDafIteration(unittest.TestCase):
+
+    def setUp(self):
+        self.header = {'name': 0, 'age': 1}
+        self.data = [['Alice', 30], ['Bob', 25]]
+        self.daf = Daf(lol=self.data, hd=self.header)
+
+    def test_iter_dict_returns_correct_dicts(self):
+        expected_results = [
+            {'name': 'Alice', 'age': 30},
+            {'name': 'Bob', 'age': 25}
+        ]
+
+        results = list(self.daf.iter_dict())
+        self.assertEqual(results, expected_results)
+
+    def test_iter_klist_returns_correct_keyedlists(self):
+        results = list(self.daf.iter_klist())
+
+        self.assertEqual(len(results), 2)
+        self.assertIsInstance(results[0], KeyedList)
+        self.assertEqual(results[0]['name'], 'Alice')
+        self.assertEqual(results[0]['age'], 30)
+        self.assertEqual(results[1]['name'], 'Bob')
+        self.assertEqual(results[1]['age'], 25)
+
+    def test_iter_klist_modifies_underlying_data(self):
+        for row in self.daf.iter_klist():
+            row['age'] += 1
+
+        expected_data = [['Alice', 31], ['Bob', 26]]
+        self.assertEqual(self.data, expected_data)
+
+    def test_default_iteration_mode_dict(self):
+        self.daf._itermode = Daf.ITERMODE_DICT
+
+        expected_results = [
+            {'name': 'Alice', 'age': 30},
+            {'name': 'Bob', 'age': 25}
+        ]
+
+        results = list(iter(self.daf))
+        self.assertEqual(results, expected_results)
+
+    def test_default_iteration_mode_keyedlist(self):
+        self.daf._itermode = Daf.ITERMODE_KEYEDLIST
+
+        results = list(iter(self.daf))
+
+        self.assertEqual(len(results), 2)
+        self.assertIsInstance(results[0], KeyedList)
+        self.assertEqual(results[0]['name'], 'Alice')
+        self.assertEqual(results[0]['age'], 30)
+        self.assertEqual(results[1]['name'], 'Bob')
+        self.assertEqual(results[1]['age'], 25)
+
+    def test_iteration_resets_after_stop_iteration(self):
+        # First iteration
+        results_1 = list(iter(self.daf))
+
+        # Second iteration
+        results_2 = list(iter(self.daf))
+
+        # Verify that the results of both iterations are the same
+        self.assertEqual(results_1, results_2)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `daffodil-0.5.1/tests/test_keyedlist.py` & `daffodil-0.5.2/tests/test_keyedlist.py`

 * *Files identical despite different names*

