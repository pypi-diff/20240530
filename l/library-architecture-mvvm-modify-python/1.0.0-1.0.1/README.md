# Comparing `tmp/library_architecture_mvvm_modify_python-1.0.0.tar.gz` & `tmp/library_architecture_mvvm_modify_python-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "library_architecture_mvvm_modify_python-1.0.0.tar", last modified: Thu May 23 12:59:20 2024, max compression
+gzip compressed data, was "library_architecture_mvvm_modify_python-1.0.1.tar", last modified: Thu May 30 12:35:01 2024, max compression
```

## Comparing `library_architecture_mvvm_modify_python-1.0.0.tar` & `library_architecture_mvvm_modify_python-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 12:59:20.657906 library_architecture_mvvm_modify_python-1.0.0/
--rw-rw-rw-   0        0        0     1088 2024-05-17 07:41:38.000000 library_architecture_mvvm_modify_python-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1385 2024-05-23 12:59:20.656090 library_architecture_mvvm_modify_python-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      974 2024-05-17 10:49:14.000000 library_architecture_mvvm_modify_python-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 12:59:20.652848 library_architecture_mvvm_modify_python-1.0.0/library_architecture_mvvm_modify_python.egg-info/
--rw-rw-rw-   0        0        0     1385 2024-05-23 12:59:20.000000 library_architecture_mvvm_modify_python-1.0.0/library_architecture_mvvm_modify_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      465 2024-05-23 12:59:20.000000 library_architecture_mvvm_modify_python-1.0.0/library_architecture_mvvm_modify_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 12:59:20.000000 library_architecture_mvvm_modify_python-1.0.0/library_architecture_mvvm_modify_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2024-05-23 12:59:20.000000 library_architecture_mvvm_modify_python-1.0.0/library_architecture_mvvm_modify_python.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       56 2024-05-23 12:59:20.000000 library_architecture_mvvm_modify_python-1.0.0/library_architecture_mvvm_modify_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    26421 2024-05-23 11:46:14.000000 library_architecture_mvvm_modify_python-1.0.0/library_architecture_mvvm_modify_python.py
-drwxrwxrwx   0        0        0        0 2024-05-23 12:59:20.650854 library_architecture_mvvm_modify_python-1.0.0/named_test_main/
--rw-rw-rw-   0        0        0     4754 2024-05-23 12:22:23.000000 library_architecture_mvvm_modify_python-1.0.0/named_test_main/iterator_test_main.py
--rw-rw-rw-   0        0        0     1916 2024-05-23 11:17:35.000000 library_architecture_mvvm_modify_python-1.0.0/named_test_main/temp_cache_test_main.py
--rw-rw-rw-   0        0        0       42 2024-05-23 12:59:20.657906 library_architecture_mvvm_modify_python-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      878 2024-05-23 12:58:14.000000 library_architecture_mvvm_modify_python-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:35:01.393433 library_architecture_mvvm_modify_python-1.0.1/
+-rw-rw-rw-   0        0        0     1088 2024-05-30 12:04:55.000000 library_architecture_mvvm_modify_python-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1385 2024-05-30 12:35:01.393433 library_architecture_mvvm_modify_python-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      974 2024-05-30 12:04:55.000000 library_architecture_mvvm_modify_python-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 12:35:01.393433 library_architecture_mvvm_modify_python-1.0.1/library_architecture_mvvm_modify_python.egg-info/
+-rw-rw-rw-   0        0        0     1385 2024-05-30 12:35:01.000000 library_architecture_mvvm_modify_python-1.0.1/library_architecture_mvvm_modify_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      465 2024-05-30 12:35:01.000000 library_architecture_mvvm_modify_python-1.0.1/library_architecture_mvvm_modify_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 12:35:01.000000 library_architecture_mvvm_modify_python-1.0.1/library_architecture_mvvm_modify_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2024-05-30 12:35:01.000000 library_architecture_mvvm_modify_python-1.0.1/library_architecture_mvvm_modify_python.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       56 2024-05-30 12:35:01.000000 library_architecture_mvvm_modify_python-1.0.1/library_architecture_mvvm_modify_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    26421 2024-05-30 12:04:56.000000 library_architecture_mvvm_modify_python-1.0.1/library_architecture_mvvm_modify_python.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:35:01.393433 library_architecture_mvvm_modify_python-1.0.1/named_test_main/
+-rw-rw-rw-   0        0        0     4665 2024-05-30 12:21:45.000000 library_architecture_mvvm_modify_python-1.0.1/named_test_main/iterator_test_main.py
+-rw-rw-rw-   0        0        0     1882 2024-05-30 12:25:11.000000 library_architecture_mvvm_modify_python-1.0.1/named_test_main/temp_cache_test_main.py
+-rw-rw-rw-   0        0        0       42 2024-05-30 12:35:01.393433 library_architecture_mvvm_modify_python-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      878 2024-05-30 12:11:22.000000 library_architecture_mvvm_modify_python-1.0.1/setup.py
```

### Comparing `library_architecture_mvvm_modify_python-1.0.0/LICENSE` & `library_architecture_mvvm_modify_python-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `library_architecture_mvvm_modify_python-1.0.0/PKG-INFO` & `library_architecture_mvvm_modify_python-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: library_architecture_mvvm_modify_python
-Version: 1.0.0
+Version: 1.0.1
 Summary: MVVM Modify for Python but you can also port to another language
 Home-page: https://github.com/antonpichka/library_architecture_mvvm_modify_python
 Author: Anton Pichka
 Author-email: antonpichka@gmail.com
 Maintainer: Anton Pichka
 Maintainer-email: antonpichka@gmail.com
 License: MIT
```

### Comparing `library_architecture_mvvm_modify_python-1.0.0/README.md` & `library_architecture_mvvm_modify_python-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `library_architecture_mvvm_modify_python-1.0.0/library_architecture_mvvm_modify_python.egg-info/PKG-INFO` & `library_architecture_mvvm_modify_python-1.0.1/library_architecture_mvvm_modify_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: library_architecture_mvvm_modify_python
-Version: 1.0.0
+Version: 1.0.1
 Summary: MVVM Modify for Python but you can also port to another language
 Home-page: https://github.com/antonpichka/library_architecture_mvvm_modify_python
 Author: Anton Pichka
 Author-email: antonpichka@gmail.com
 Maintainer: Anton Pichka
 Maintainer-email: antonpichka@gmail.com
 License: MIT
```

### Comparing `library_architecture_mvvm_modify_python-1.0.0/library_architecture_mvvm_modify_python.py` & `library_architecture_mvvm_modify_python-1.0.1/library_architecture_mvvm_modify_python.py`

 * *Files identical despite different names*

### Comparing `library_architecture_mvvm_modify_python-1.0.0/named_test_main/iterator_test_main.py` & `library_architecture_mvvm_modify_python-1.0.1/named_test_main/iterator_test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Generic, TypeVar
-from library_architecture_mvvm_modify_python import BaseModel, BaseListModel, BaseModelWNamedWNamedWNamedIterator, CurrentModelWIndex, debug_print
+from library_architecture_mvvm_modify_python import *
 
 class UserBalance(BaseModel):
     def __init__(self, username: str, money: int) -> None:
         super().__init__(username)
         self.USERNAME: str = username
         self.MONEY: int = money
     
@@ -16,15 +16,15 @@
 T = TypeVar("T", bound=UserBalance)
 
 class ListUserBalance(Generic[T],BaseListModel[T]):
     def __init__(self, list_model: list[T]) -> None:
         super().__init__(list_model)
     
     def get_clone(self) -> 'ListUserBalance':
-        new_list_model = list[T]
+        new_list_model: list[T] = []
         for item_model in self.LIST_MODEL:
             new_list_model.append(item_model.get_clone())
         return ListUserBalance(new_list_model)
     
     def to_string(self) -> str:
         str_list_model = "\n"
         for item_model in self.LIST_MODEL:
```

### Comparing `library_architecture_mvvm_modify_python-1.0.0/named_test_main/temp_cache_test_main.py` & `library_architecture_mvvm_modify_python-1.0.1/named_test_main/temp_cache_test_main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import asyncio
-from library_architecture_mvvm_modify_python import TempCacheService, debug_print
+from library_architecture_mvvm_modify_python import *
 
 def __listen_stream_from_key_temp_cache_and_callback_parameter_one(object: str) -> None:
     debug_print("Listen: " + object)
 
 def __listen_stream_from_key_temp_cache_and_callback_parameter_one_first(object: str) -> None:
     debug_print("ListenTwo: " + object)
 
@@ -11,24 +11,24 @@
     debug_print("ListenThree: " + object)
 
 async def main() -> None:
     temp_cache_service = TempCacheService()
     key = "key"
     temp_cache_service.update_where_stream_notification_is_possible_from_key_temp_cache_and_value_parameter_one(key,"One")
     from_key_temp_cache_parameter_temp_cache = temp_cache_service.get_from_key_temp_cache_parameter_temp_cache(key)
-    debug_print("GetFromKeyTempCacheParameterTempCache: " + from_key_temp_cache_parameter_temp_cache)
+    debug_print("FromKeyTempCacheParameterTempCache: " + from_key_temp_cache_parameter_temp_cache)
     temp_cache_service.listen_stream_from_key_temp_cache_and_callback_parameter_one(key,__listen_stream_from_key_temp_cache_and_callback_parameter_one)
     await asyncio.sleep(1)
     temp_cache_service.update_where_stream_notification_is_possible_from_key_temp_cache_and_value_parameter_one(key,"Two")
     temp_cache_service.listen_stream_from_key_temp_cache_and_callback_parameter_one(key,__listen_stream_from_key_temp_cache_and_callback_parameter_one_first)
     await asyncio.sleep(1)
     temp_cache_service.update_where_stream_notification_is_possible_from_key_temp_cache_and_value_parameter_one(key,"Three")
     temp_cache_service.listen_stream_from_key_temp_cache_and_callback_parameter_one(key,__listen_stream_from_key_temp_cache_and_callback_parameter_one_second)
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(main())
 ## EXPECTED OUTPUT:
 ##
-## GetFromKeyTempCacheParameterTempCache: One
+## FromKeyTempCacheParameterTempCache: One
 ## Listen: Two
 ## Listen: Three
 ## ListenTwo: Three
```

### Comparing `library_architecture_mvvm_modify_python-1.0.0/setup.py` & `library_architecture_mvvm_modify_python-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import io
 from setuptools import setup
 
 setup(
     name="library_architecture_mvvm_modify_python",
-    version="1.0.0",
+    version="1.0.1",
     description="MVVM Modify for Python but you can also port to another language",
     long_description=io.open("README.md", "r", encoding="utf-8").read(),
     author="Anton Pichka",
     author_email="antonpichka@gmail.com",
     maintainer="Anton Pichka",
     maintainer_email="antonpichka@gmail.com",
     url="https://github.com/antonpichka/library_architecture_mvvm_modify_python",
```

