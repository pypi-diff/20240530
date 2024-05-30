# Comparing `tmp/vprikol_api_python-1.8.5.tar.gz` & `tmp/vprikol_api_python-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vprikol_api_python-1.8.5.tar", max compression
+gzip compressed data, was "vprikol_api_python-1.9.0.tar", max compression
```

## Comparing `vprikol_api_python-1.8.5.tar` & `vprikol_api_python-1.9.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       32 2023-11-02 18:40:51.105140 vprikol_api_python-1.8.5/README.md
--rw-r--r--   0        0        0      351 2023-11-02 18:40:51.109140 vprikol_api_python-1.8.5/pyproject.toml
--rw-r--r--   0        0        0       51 2023-11-02 18:40:51.109140 vprikol_api_python-1.8.5/vprikol_api/__init__.py
--rw-r--r--   0        0        0      921 2023-11-02 18:40:51.109140 vprikol_api_python-1.8.5/vprikol_api/api.py
--rw-r--r--   0        0        0     5663 2023-11-02 18:40:51.109140 vprikol_api_python-1.8.5/vprikol_api/main.py
--rw-r--r--   0        0        0     3781 2023-11-02 18:40:51.109140 vprikol_api_python-1.8.5/vprikol_api/model.py
--rw-r--r--   0        0        0      506 1970-01-01 00:00:00.000000 vprikol_api_python-1.8.5/PKG-INFO
+-rw-r--r--   0        0        0       32 2023-11-02 20:33:20.735336 vprikol_api_python-1.9.0/README.md
+-rw-r--r--   0        0        0      351 2023-11-02 20:33:20.735336 vprikol_api_python-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0       51 2023-11-02 20:33:20.735336 vprikol_api_python-1.9.0/vprikol_api/__init__.py
+-rw-r--r--   0        0        0      921 2023-11-02 20:33:20.735336 vprikol_api_python-1.9.0/vprikol_api/api.py
+-rw-r--r--   0        0        0     6280 2023-11-02 20:33:20.735336 vprikol_api_python-1.9.0/vprikol_api/main.py
+-rw-r--r--   0        0        0     3936 2023-11-02 20:33:20.735336 vprikol_api_python-1.9.0/vprikol_api/model.py
+-rw-r--r--   0        0        0      506 1970-01-01 00:00:00.000000 vprikol_api_python-1.9.0/PKG-INFO
```

### Comparing `vprikol_api_python-1.8.5/vprikol_api/api.py` & `vprikol_api_python-1.9.0/vprikol_api/api.py`

 * *Files identical despite different names*

### Comparing `vprikol_api_python-1.8.5/vprikol_api/main.py` & `vprikol_api_python-1.9.0/vprikol_api/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import time
+
 from .model import IpAPIResponse, MembersAPIResponse, PlayerInfoAPIResponse, CreatedFindTaskAPIResponse, \
     ServerStatusAPIResponse, RatingAPIResponse, CheckRPUsernameAPIResponse, GenerateRPUsernameAPIResponse, \
-    PlayerInfoNotFound
+    PlayerInfoNotFound, PlayerOnlineAPIResponse
 
 from .api import get, post
 from typing import Literal
 import asyncio
 from pydantic import parse_obj_as, ValidationError
 
 
@@ -81,14 +83,15 @@
                            params=params)
 
         if not result.success:
             raise Exception(result.error)
 
         if isinstance(result.data, list):
             return parse_obj_as(list[ServerStatusAPIResponse], result.data)
+
         return ServerStatusAPIResponse(**result.data)
 
     async def get_rating(self, server_id: int, rating_type: Literal[1, 2, 3]) -> RatingAPIResponse:
         params = {'type': rating_type, 'server': server_id}
 
         result = await get(url=f'{self.base_url}rating', headers=self.headers,
                            params=params)
@@ -111,7 +114,18 @@
             -> GenerateRPUsernameAPIResponse:
         result = await get(url=f'{self.base_url}rpnick', headers=self.headers,
                            params={'gender': gender, 'nation': nation})
         if not result.success:
             raise Exception(result.error)
 
         return GenerateRPUsernameAPIResponse(**result.data)
+
+    async def get_player_online(self, nickname: str, server_id: int, count: int = 100,
+                                offset: int = 0, date: int = int(time.time())) -> PlayerOnlineAPIResponse:
+        result = await get(url=f'{self.base_url}online', headers=self.headers,
+                           params={'nickname': nickname, 'count': count, 'offset': offset, 'server_id': server_id,
+                                   'filter_by_date': date})
+
+        if not result.success:
+            raise Exception(result.error)
+
+        return PlayerOnlineAPIResponse(**result.data)
```

### Comparing `vprikol_api_python-1.8.5/vprikol_api/model.py` & `vprikol_api_python-1.9.0/vprikol_api/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,7 +136,16 @@
     surname: CheckRPUsernameName
     nickname: str = Field(alias='nick')
 
 
 class GenerateRPUsernameAPIResponse(BaseModel):
     name: str
     surname: str
+
+
+class OnlinePlayerInfo(BaseModel):
+    login_at: int
+    logout_at: int
+
+
+class PlayerOnlineAPIResponse(BaseModel):
+    sessions: list[OnlinePlayerInfo]
```

