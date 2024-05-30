# Comparing `tmp/cheeseapi-1.3.0.tar.gz` & `tmp/cheeseapi-1.3.1.tar.gz`

## Comparing `cheeseapi-1.3.0.tar` & `cheeseapi-1.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/CheeseAPI/__init__.py
--rw-r--r--   0        0        0     7512 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/CheeseAPI/app.py
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/CheeseAPI/cors.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/CheeseAPI/exception.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/CheeseAPI/file.py
--rw-r--r--   0        0        0    33258 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/CheeseAPI/handle.py
--rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/CheeseAPI/protocol.py
--rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/CheeseAPI/request.py
--rw-r--r--   0        0        0    17620 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/CheeseAPI/response.py
--rw-r--r--   0        0        0    13136 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/CheeseAPI/route.py
--rw-r--r--   0        0        0    10363 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/CheeseAPI/schedule.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/CheeseAPI/server.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/CheeseAPI/signal.py
--rw-r--r--   0        0        0     8218 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/CheeseAPI/text.py
--rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/CheeseAPI/validator.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/CheeseAPI/websocket.py
--rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/CheeseAPI/workspace.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/LICENSE
--rw-r--r--   0        0        0     5007 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/README.md
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     5532 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 cheeseapi-1.3.1/CheeseAPI/__init__.py
+-rw-r--r--   0        0        0     7512 2020-02-02 00:00:00.000000 cheeseapi-1.3.1/CheeseAPI/app.py
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 cheeseapi-1.3.1/CheeseAPI/cors.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 cheeseapi-1.3.1/CheeseAPI/exception.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 cheeseapi-1.3.1/CheeseAPI/file.py
+-rw-r--r--   0        0        0    33258 2020-02-02 00:00:00.000000 cheeseapi-1.3.1/CheeseAPI/handle.py
+-rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 cheeseapi-1.3.1/CheeseAPI/protocol.py
+-rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 cheeseapi-1.3.1/CheeseAPI/request.py
+-rw-r--r--   0        0        0    17620 2020-02-02 00:00:00.000000 cheeseapi-1.3.1/CheeseAPI/response.py
+-rw-r--r--   0        0        0    13136 2020-02-02 00:00:00.000000 cheeseapi-1.3.1/CheeseAPI/route.py
+-rw-r--r--   0        0        0    10363 2020-02-02 00:00:00.000000 cheeseapi-1.3.1/CheeseAPI/schedule.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cheeseapi-1.3.1/CheeseAPI/server.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 cheeseapi-1.3.1/CheeseAPI/signal.py
+-rw-r--r--   0        0        0     7371 2020-02-02 00:00:00.000000 cheeseapi-1.3.1/CheeseAPI/text.py
+-rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 cheeseapi-1.3.1/CheeseAPI/validator.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 cheeseapi-1.3.1/CheeseAPI/websocket.py
+-rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 cheeseapi-1.3.1/CheeseAPI/workspace.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 cheeseapi-1.3.1/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cheeseapi-1.3.1/LICENSE
+-rw-r--r--   0        0        0     5007 2020-02-02 00:00:00.000000 cheeseapi-1.3.1/README.md
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 cheeseapi-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5532 2020-02-02 00:00:00.000000 cheeseapi-1.3.1/PKG-INFO
```

### Comparing `cheeseapi-1.3.0/CheeseAPI/app.py` & `cheeseapi-1.3.1/CheeseAPI/app.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.3.0/CheeseAPI/cors.py` & `cheeseapi-1.3.1/CheeseAPI/cors.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.3.0/CheeseAPI/exception.py` & `cheeseapi-1.3.1/CheeseAPI/exception.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.3.0/CheeseAPI/file.py` & `cheeseapi-1.3.1/CheeseAPI/file.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.3.0/CheeseAPI/handle.py` & `cheeseapi-1.3.1/CheeseAPI/handle.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.3.0/CheeseAPI/protocol.py` & `cheeseapi-1.3.1/CheeseAPI/protocol.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.3.0/CheeseAPI/request.py` & `cheeseapi-1.3.1/CheeseAPI/request.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.3.0/CheeseAPI/response.py` & `cheeseapi-1.3.1/CheeseAPI/response.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.3.0/CheeseAPI/route.py` & `cheeseapi-1.3.1/CheeseAPI/route.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.3.0/CheeseAPI/schedule.py` & `cheeseapi-1.3.1/CheeseAPI/schedule.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.3.0/CheeseAPI/server.py` & `cheeseapi-1.3.1/CheeseAPI/server.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.3.0/CheeseAPI/signal.py` & `cheeseapi-1.3.1/CheeseAPI/signal.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.3.0/CheeseAPI/text.py` & `cheeseapi-1.3.1/CheeseAPI/text.py`

 * *Files 11% similar despite different names*

```diff
@@ -142,25 +142,7 @@
             styledMessage += f'<blue>{minutes}</blue> minutes '
         message += '{:.6f} seconds'.format(timer % 60)
         styledMessage += '<blue>{:.6f}</blue> seconds'.format(timer % 60)
 
         return [
             (message, styledMessage)
         ]
-
-    def validator_requiredMessage(self, scope: str, key: str) -> str:
-        return f'The {scope}.{key} is required'
-
-    def validator_typeMessage(self, scope: str, key: str, expected_type: str) -> str:
-        return f'The {scope}.{key} cannot be converted to {expected_type}'
-
-    def validator_patternMessage(self, scope: str, key: str) -> str:
-        return f'The {scope}.{key} regular check error'
-
-    def validator_minMessage(self, scope: str, key: str, min: object) -> str:
-        return f'The {scope}.{key} cannot be less than {min}'
-
-    def validator_maxMessage(self, scope: str, key: str, max: object) -> str:
-        return f'The {scope}.{key} cannot be larger than {max}'
-
-    def validator_enumMessage(self, scope: str, key: str, enum: List[Any]) -> str:
-        return f'The {scope}.{key} cannot be a value other than {enum}'
```

### Comparing `cheeseapi-1.3.0/CheeseAPI/validator.py` & `cheeseapi-1.3.1/CheeseAPI/validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import json
 from typing import TYPE_CHECKING
 from functools import wraps
 
 from pydantic import BaseModel, ValidationError
 
-from CheeseAPI.response import JsonResponse
+from CheeseAPI.response import JsonResponse, Response
 
 if TYPE_CHECKING:
     from CheeseAPI.request import Request
     from CheeseAPI.response import BaseResponse
 
 class ValidateError(Exception):
-    def __init__(self, response: 'BaseResponse'):
+    def __init__(self, response: 'BaseResponse' = Response(status = 400)):
         self.response: 'BaseResponse' = response
 
 def validator(validator: BaseModel):
     '''
     为路由函数添加校验装饰器。
 
     校验参数以类的校验属性为key，从路径变量、args、form、cookie、headers按顺序尝试匹配，若全部匹配失败，则会默认为None。
@@ -64,14 +64,16 @@
             for key in validator.model_fields.keys():
                 _kwargs[key] = None
 
                 for scope in [ 'path', 'args', 'form', 'cookie', 'headers' ]:
                     try:
                         if scope == 'path':
                             _kwargs[key] = kwargs.get(key)
+                        elif scope == 'headers':
+                            _kwargs[key] = getattr(request, scope).get(key.replace('_', '-'))
                         else:
                             _kwargs[key] = getattr(request, scope).get(key)
 
                         if _kwargs.get(key):
                             break
                     except:
                         ...
```

### Comparing `cheeseapi-1.3.0/CheeseAPI/websocket.py` & `cheeseapi-1.3.1/CheeseAPI/websocket.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.3.0/CheeseAPI/workspace.py` & `cheeseapi-1.3.1/CheeseAPI/workspace.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.3.0/LICENSE` & `cheeseapi-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.3.0/README.md` & `cheeseapi-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.3.0/pyproject.toml` & `cheeseapi-1.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "hatchling" ]
 build-backend = "hatchling.build"
 
 [project]
 name = "CheeseAPI"
-version = "1.3.0"
+version = "1.3.1"
 description = "一款web协程框架。"
 readme = "README.md"
 license-files = { paths = [ "LICENSE" ] }
 authors = [
     { name = "Cheese Unknown", email = "cheese@cheese.ren" }
 ]
 keywords = [ 'API', 'BackEnd' ]
```

### Comparing `cheeseapi-1.3.0/PKG-INFO` & `cheeseapi-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: CheeseAPI
-Version: 1.3.0
+Version: 1.3.1
 Summary: 一款web协程框架。
 Project-URL: Source, https://github.com/CheeseUnknown/CheeseAPI
 Author-email: Cheese Unknown <cheese@cheese.ren>
 License-File: LICENSE
 Keywords: API,BackEnd
 Requires-Dist: cheeselog==1.0.*
 Requires-Dist: cheesesignal==1.1.*
```

