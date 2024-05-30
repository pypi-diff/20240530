# Comparing `tmp/alibabacloud_dm20151123-1.1.2.tar.gz` & `tmp/alibabacloud_dm20151123-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dm20151123-1.1.2.tar", last modified: Mon May 20 03:20:16 2024, max compression
+gzip compressed data, was "dist/alibabacloud_dm20151123-1.2.0.tar", last modified: Thu May 30 17:10:30 2024, max compression
```

## Comparing `alibabacloud_dm20151123-1.1.2.tar` & `alibabacloud_dm20151123-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 03:20:16.000000 alibabacloud_dm20151123-1.1.2/
--rw-r--r--   0 root         (0) root         (0)     2260 2024-05-20 03:20:15.000000 alibabacloud_dm20151123-1.1.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-05-20 03:20:15.000000 alibabacloud_dm20151123-1.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-05-20 03:20:15.000000 alibabacloud_dm20151123-1.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2394 2024-05-20 03:20:16.000000 alibabacloud_dm20151123-1.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1091 2024-05-20 03:20:15.000000 alibabacloud_dm20151123-1.1.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1176 2024-05-20 03:20:15.000000 alibabacloud_dm20151123-1.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 03:20:16.000000 alibabacloud_dm20151123-1.1.2/alibabacloud_dm20151123/
--rw-r--r--   0 root         (0) root         (0)       21 2024-05-20 03:20:15.000000 alibabacloud_dm20151123-1.1.2/alibabacloud_dm20151123/__init__.py
--rw-r--r--   0 root         (0) root         (0)   198476 2024-05-20 03:20:15.000000 alibabacloud_dm20151123-1.1.2/alibabacloud_dm20151123/client.py
--rw-r--r--   0 root         (0) root         (0)   247209 2024-05-20 03:20:15.000000 alibabacloud_dm20151123-1.1.2/alibabacloud_dm20151123/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 03:20:16.000000 alibabacloud_dm20151123-1.1.2/alibabacloud_dm20151123.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2394 2024-05-20 03:20:16.000000 alibabacloud_dm20151123-1.1.2/alibabacloud_dm20151123.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      412 2024-05-20 03:20:16.000000 alibabacloud_dm20151123-1.1.2/alibabacloud_dm20151123.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 03:20:16.000000 alibabacloud_dm20151123-1.1.2/alibabacloud_dm20151123.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-05-20 03:20:16.000000 alibabacloud_dm20151123-1.1.2/alibabacloud_dm20151123.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2024-05-20 03:20:16.000000 alibabacloud_dm20151123-1.1.2/alibabacloud_dm20151123.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-05-20 03:20:16.000000 alibabacloud_dm20151123-1.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2606 2024-05-20 03:20:15.000000 alibabacloud_dm20151123-1.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 17:10:30.000000 alibabacloud_dm20151123-1.2.0/
+-rw-r--r--   0 root         (0) root         (0)     2325 2024-05-30 17:10:30.000000 alibabacloud_dm20151123-1.2.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-30 17:10:30.000000 alibabacloud_dm20151123-1.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-30 17:10:30.000000 alibabacloud_dm20151123-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2394 2024-05-30 17:10:30.000000 alibabacloud_dm20151123-1.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1091 2024-05-30 17:10:30.000000 alibabacloud_dm20151123-1.2.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1176 2024-05-30 17:10:30.000000 alibabacloud_dm20151123-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 17:10:30.000000 alibabacloud_dm20151123-1.2.0/alibabacloud_dm20151123/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-30 17:10:30.000000 alibabacloud_dm20151123-1.2.0/alibabacloud_dm20151123/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   204478 2024-05-30 17:10:30.000000 alibabacloud_dm20151123-1.2.0/alibabacloud_dm20151123/client.py
+-rw-r--r--   0 root         (0) root         (0)   253821 2024-05-30 17:10:30.000000 alibabacloud_dm20151123-1.2.0/alibabacloud_dm20151123/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 17:10:30.000000 alibabacloud_dm20151123-1.2.0/alibabacloud_dm20151123.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2394 2024-05-30 17:10:30.000000 alibabacloud_dm20151123-1.2.0/alibabacloud_dm20151123.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      412 2024-05-30 17:10:30.000000 alibabacloud_dm20151123-1.2.0/alibabacloud_dm20151123.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 17:10:30.000000 alibabacloud_dm20151123-1.2.0/alibabacloud_dm20151123.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-30 17:10:30.000000 alibabacloud_dm20151123-1.2.0/alibabacloud_dm20151123.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2024-05-30 17:10:30.000000 alibabacloud_dm20151123-1.2.0/alibabacloud_dm20151123.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-30 17:10:30.000000 alibabacloud_dm20151123-1.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2606 2024-05-30 17:10:30.000000 alibabacloud_dm20151123-1.2.0/setup.py
```

### Comparing `alibabacloud_dm20151123-1.1.2/ChangeLog.md` & `alibabacloud_dm20151123-1.2.0/ChangeLog.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2024-05-20 Version: 1.1.2
+- Generated python 2015-11-23 for Dm.
+
 2024-05-15 Version: 1.1.1
 - Generated python 2015-11-23 for Dm.
 
 2024-04-22 Version: 1.1.0
 - Support API CreateUserSuppression.
 - Support API GetSuppressionListLevel.
 - Support API ListUserSuppression.
```

### Comparing `alibabacloud_dm20151123-1.1.2/LICENSE` & `alibabacloud_dm20151123-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dm20151123-1.1.2/PKG-INFO` & `alibabacloud_dm20151123-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dm20151123
-Version: 1.1.2
+Version: 1.2.0
 Summary: Alibaba Cloud Dm (20151123) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dm20151123-1.1.2/README-CN.md` & `alibabacloud_dm20151123-1.2.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dm20151123-1.1.2/README.md` & `alibabacloud_dm20151123-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dm20151123-1.1.2/alibabacloud_dm20151123/client.py` & `alibabacloud_dm20151123-1.2.0/alibabacloud_dm20151123/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2737,14 +2737,88 @@
         
         @param request: GetTrackListByMailFromAndTagNameRequest
         @return: GetTrackListByMailFromAndTagNameResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.get_track_list_by_mail_from_and_tag_name_with_options_async(request, runtime)
 
+    def get_user_with_options(
+        self,
+        runtime: util_models.RuntimeOptions,
+    ) -> dm_20151123_models.GetUserResponse:
+        """
+        @summary 获取账号详情
+        
+        @param request: GetUserRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetUserResponse
+        """
+        req = open_api_models.OpenApiRequest()
+        params = open_api_models.Params(
+            action='GetUser',
+            version='2015-11-23',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dm_20151123_models.GetUserResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_user_with_options_async(
+        self,
+        runtime: util_models.RuntimeOptions,
+    ) -> dm_20151123_models.GetUserResponse:
+        """
+        @summary 获取账号详情
+        
+        @param request: GetUserRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetUserResponse
+        """
+        req = open_api_models.OpenApiRequest()
+        params = open_api_models.Params(
+            action='GetUser',
+            version='2015-11-23',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dm_20151123_models.GetUserResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_user(self) -> dm_20151123_models.GetUserResponse:
+        """
+        @summary 获取账号详情
+        
+        @return: GetUserResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return self.get_user_with_options(runtime)
+
+    async def get_user_async(self) -> dm_20151123_models.GetUserResponse:
+        """
+        @summary 获取账号详情
+        
+        @return: GetUserResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return await self.get_user_with_options_async(runtime)
+
     def list_user_suppression_with_options(
         self,
         request: dm_20151123_models.ListUserSuppressionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dm_20151123_models.ListUserSuppressionResponse:
         """
         @summary 列出用户无效地址
@@ -5016,7 +5090,111 @@
         @summary 更新IP防护API
         
         @param request: UpdateIpProtectionRequest
         @return: UpdateIpProtectionResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.update_ip_protection_with_options_async(request, runtime)
+
+    def update_user_with_options(
+        self,
+        tmp_req: dm_20151123_models.UpdateUserRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dm_20151123_models.UpdateUserResponse:
+        """
+        @summary 更新帐号信息
+        
+        @param tmp_req: UpdateUserRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateUserResponse
+        """
+        UtilClient.validate_model(tmp_req)
+        request = dm_20151123_models.UpdateUserShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.user):
+            request.user_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user, 'User', 'json')
+        body = {}
+        if not UtilClient.is_unset(request.user_shrink):
+            body['User'] = request.user_shrink
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='UpdateUser',
+            version='2015-11-23',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dm_20151123_models.UpdateUserResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def update_user_with_options_async(
+        self,
+        tmp_req: dm_20151123_models.UpdateUserRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dm_20151123_models.UpdateUserResponse:
+        """
+        @summary 更新帐号信息
+        
+        @param tmp_req: UpdateUserRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateUserResponse
+        """
+        UtilClient.validate_model(tmp_req)
+        request = dm_20151123_models.UpdateUserShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.user):
+            request.user_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user, 'User', 'json')
+        body = {}
+        if not UtilClient.is_unset(request.user_shrink):
+            body['User'] = request.user_shrink
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='UpdateUser',
+            version='2015-11-23',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dm_20151123_models.UpdateUserResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def update_user(
+        self,
+        request: dm_20151123_models.UpdateUserRequest,
+    ) -> dm_20151123_models.UpdateUserResponse:
+        """
+        @summary 更新帐号信息
+        
+        @param request: UpdateUserRequest
+        @return: UpdateUserResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return self.update_user_with_options(request, runtime)
+
+    async def update_user_async(
+        self,
+        request: dm_20151123_models.UpdateUserRequest,
+    ) -> dm_20151123_models.UpdateUserResponse:
+        """
+        @summary 更新帐号信息
+        
+        @param request: UpdateUserRequest
+        @return: UpdateUserResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return await self.update_user_with_options_async(request, runtime)
```

### Comparing `alibabacloud_dm20151123-1.1.2/alibabacloud_dm20151123/models.py` & `alibabacloud_dm20151123-1.2.0/alibabacloud_dm20151123/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3670,14 +3670,117 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetTrackListByMailFromAndTagNameResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetUserResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        enable_eventbridge: bool = None,
+    ):
+        self.enable_eventbridge = enable_eventbridge
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.enable_eventbridge is not None:
+            result['EnableEventbridge'] = self.enable_eventbridge
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('EnableEventbridge') is not None:
+            self.enable_eventbridge = m.get('EnableEventbridge')
+        return self
+
+
+class GetUserResponseBody(TeaModel):
+    def __init__(
+        self,
+        data: GetUserResponseBodyData = None,
+        request_id: str = None,
+    ):
+        self.data = data
+        self.request_id = request_id
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Data') is not None:
+            temp_model = GetUserResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class GetUserResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetUserResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetUserResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ListUserSuppressionRequest(TeaModel):
     def __init__(
         self,
         address: str = None,
         end_bounce_time: int = None,
         end_create_time: int = None,
         owner_id: int = None,
@@ -7540,7 +7643,159 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = UpdateIpProtectionResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class UpdateUserRequestUser(TeaModel):
+    def __init__(
+        self,
+        enable_eventbridge: bool = None,
+    ):
+        self.enable_eventbridge = enable_eventbridge
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.enable_eventbridge is not None:
+            result['EnableEventbridge'] = self.enable_eventbridge
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('EnableEventbridge') is not None:
+            self.enable_eventbridge = m.get('EnableEventbridge')
+        return self
+
+
+class UpdateUserRequest(TeaModel):
+    def __init__(
+        self,
+        user: UpdateUserRequestUser = None,
+    ):
+        self.user = user
+
+    def validate(self):
+        if self.user:
+            self.user.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.user is not None:
+            result['User'] = self.user.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('User') is not None:
+            temp_model = UpdateUserRequestUser()
+            self.user = temp_model.from_map(m['User'])
+        return self
+
+
+class UpdateUserShrinkRequest(TeaModel):
+    def __init__(
+        self,
+        user_shrink: str = None,
+    ):
+        self.user_shrink = user_shrink
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.user_shrink is not None:
+            result['User'] = self.user_shrink
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('User') is not None:
+            self.user_shrink = m.get('User')
+        return self
+
+
+class UpdateUserResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        # Id of the request
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class UpdateUserResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: UpdateUserResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = UpdateUserResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
```

### Comparing `alibabacloud_dm20151123-1.1.2/alibabacloud_dm20151123.egg-info/PKG-INFO` & `alibabacloud_dm20151123-1.2.0/alibabacloud_dm20151123.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dm20151123
-Version: 1.1.2
+Version: 1.2.0
 Summary: Alibaba Cloud Dm (20151123) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dm20151123-1.1.2/setup.py` & `alibabacloud_dm20151123-1.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dm20151123.
 
-Created on 20/05/2024
+Created on 30/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dm20151123"
 NAME = "alibabacloud_dm20151123" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dm (20151123) SDK Library for Python"
```

