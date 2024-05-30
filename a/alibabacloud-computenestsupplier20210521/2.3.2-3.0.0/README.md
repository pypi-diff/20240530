# Comparing `tmp/alibabacloud_computenestsupplier20210521-2.3.2.tar.gz` & `tmp/alibabacloud_computenestsupplier20210521-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_computenestsupplier20210521-2.3.2.tar", last modified: Fri Sep  8 17:13:49 2023, max compression
+gzip compressed data, was "dist/alibabacloud_computenestsupplier20210521-3.0.0.tar", last modified: Thu May 30 15:38:11 2024, max compression
```

## Comparing `alibabacloud_computenestsupplier20210521-2.3.2.tar` & `alibabacloud_computenestsupplier20210521-3.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-08 17:13:49.000000 alibabacloud_computenestsupplier20210521-2.3.2/
--rw-r--r--   0 root         (0) root         (0)      973 2023-09-08 17:13:48.000000 alibabacloud_computenestsupplier20210521-2.3.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-09-08 17:13:48.000000 alibabacloud_computenestsupplier20210521-2.3.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-09-08 17:13:48.000000 alibabacloud_computenestsupplier20210521-2.3.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2424 2023-09-08 17:13:49.000000 alibabacloud_computenestsupplier20210521-2.3.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1070 2023-09-08 17:13:48.000000 alibabacloud_computenestsupplier20210521-2.3.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1155 2023-09-08 17:13:48.000000 alibabacloud_computenestsupplier20210521-2.3.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-08 17:13:49.000000 alibabacloud_computenestsupplier20210521-2.3.2/alibabacloud_computenestsupplier20210521/
--rw-r--r--   0 root         (0) root         (0)       21 2023-09-08 17:13:48.000000 alibabacloud_computenestsupplier20210521-2.3.2/alibabacloud_computenestsupplier20210521/__init__.py
--rw-r--r--   0 root         (0) root         (0)   107437 2023-09-08 17:13:48.000000 alibabacloud_computenestsupplier20210521-2.3.2/alibabacloud_computenestsupplier20210521/client.py
--rw-r--r--   0 root         (0) root         (0)   262084 2023-09-08 17:13:48.000000 alibabacloud_computenestsupplier20210521-2.3.2/alibabacloud_computenestsupplier20210521/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-08 17:13:49.000000 alibabacloud_computenestsupplier20210521-2.3.2/alibabacloud_computenestsupplier20210521.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2424 2023-09-08 17:13:49.000000 alibabacloud_computenestsupplier20210521-2.3.2/alibabacloud_computenestsupplier20210521.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      548 2023-09-08 17:13:49.000000 alibabacloud_computenestsupplier20210521-2.3.2/alibabacloud_computenestsupplier20210521.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-08 17:13:49.000000 alibabacloud_computenestsupplier20210521-2.3.2/alibabacloud_computenestsupplier20210521.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2023-09-08 17:13:49.000000 alibabacloud_computenestsupplier20210521-2.3.2/alibabacloud_computenestsupplier20210521.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       41 2023-09-08 17:13:49.000000 alibabacloud_computenestsupplier20210521-2.3.2/alibabacloud_computenestsupplier20210521.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-09-08 17:13:49.000000 alibabacloud_computenestsupplier20210521-2.3.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2691 2023-09-08 17:13:48.000000 alibabacloud_computenestsupplier20210521-2.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 15:38:11.000000 alibabacloud_computenestsupplier20210521-3.0.0/
+-rw-r--r--   0 root         (0) root         (0)     1055 2024-05-30 15:38:11.000000 alibabacloud_computenestsupplier20210521-3.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-30 15:38:11.000000 alibabacloud_computenestsupplier20210521-3.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-30 15:38:11.000000 alibabacloud_computenestsupplier20210521-3.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2513 2024-05-30 15:38:11.000000 alibabacloud_computenestsupplier20210521-3.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1159 2024-05-30 15:38:11.000000 alibabacloud_computenestsupplier20210521-3.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1244 2024-05-30 15:38:11.000000 alibabacloud_computenestsupplier20210521-3.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 15:38:11.000000 alibabacloud_computenestsupplier20210521-3.0.0/alibabacloud_computenestsupplier20210521/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-30 15:38:11.000000 alibabacloud_computenestsupplier20210521-3.0.0/alibabacloud_computenestsupplier20210521/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   155971 2024-05-30 15:38:11.000000 alibabacloud_computenestsupplier20210521-3.0.0/alibabacloud_computenestsupplier20210521/client.py
+-rw-r--r--   0 root         (0) root         (0)   332983 2024-05-30 15:38:11.000000 alibabacloud_computenestsupplier20210521-3.0.0/alibabacloud_computenestsupplier20210521/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 15:38:11.000000 alibabacloud_computenestsupplier20210521-3.0.0/alibabacloud_computenestsupplier20210521.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2513 2024-05-30 15:38:11.000000 alibabacloud_computenestsupplier20210521-3.0.0/alibabacloud_computenestsupplier20210521.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      548 2024-05-30 15:38:11.000000 alibabacloud_computenestsupplier20210521-3.0.0/alibabacloud_computenestsupplier20210521.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 15:38:11.000000 alibabacloud_computenestsupplier20210521-3.0.0/alibabacloud_computenestsupplier20210521.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-30 15:38:11.000000 alibabacloud_computenestsupplier20210521-3.0.0/alibabacloud_computenestsupplier20210521.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2024-05-30 15:38:11.000000 alibabacloud_computenestsupplier20210521-3.0.0/alibabacloud_computenestsupplier20210521.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-30 15:38:11.000000 alibabacloud_computenestsupplier20210521-3.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2691 2024-05-30 15:38:11.000000 alibabacloud_computenestsupplier20210521-3.0.0/setup.py
```

### Comparing `alibabacloud_computenestsupplier20210521-2.3.2/ChangeLog.md` & `alibabacloud_computenestsupplier20210521-3.0.0/ChangeLog.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-09-08 Version: 2.3.2
+- Generated python 2021-05-21 for ComputeNestSupplier.
+
 2023-08-31 Version: 2.3.1
 - Generated python 2021-05-21 for ComputeNestSupplier.
 
 2023-08-31 Version: 2.3.0
 - Generated python 2021-05-21 for ComputeNestSupplier.
 
 2023-08-18 Version: 2.2.0
```

### Comparing `alibabacloud_computenestsupplier20210521-2.3.2/LICENSE` & `alibabacloud_computenestsupplier20210521-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_computenestsupplier20210521-2.3.2/PKG-INFO` & `alibabacloud_computenestsupplier20210521-3.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_computenestsupplier20210521
-Version: 2.3.2
+Version: 3.0.0
 Summary: Alibaba Cloud ComputeNestSupplier (20210521) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/computenestsupplier-20210521/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_computenestsupplier20210521-2.3.2/README-CN.md` & `alibabacloud_computenestsupplier20210521-3.0.0/README-CN.md`

 * *Files 12% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 ## 使用说明
 
 [快速使用](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-CN.md#%E5%BF%AB%E9%80%9F%E4%BD%BF%E7%94%A8)
 
 ## 发行说明
 
-每个版本的详细更改记录在[发行说明](./ChangeLog.md)中。
+每个版本的详细更改记录在[发行说明](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/computenestsupplier-20210521/ChangeLog.md)中。
 
 ## 相关
 
 - [最新源码](https://github.com/aliyun/alibabacloud-python-sdk/)
 
 ## 许可证
```

### Comparing `alibabacloud_computenestsupplier20210521-2.3.2/README.md` & `alibabacloud_computenestsupplier20210521-3.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 ## Usage
 
 [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
 
 ## Changelog
 
-Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/computenestsupplier-20210521/ChangeLog.md).
 
 ## References
 
 - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
 
 ## License
```

### Comparing `alibabacloud_computenestsupplier20210521-2.3.2/alibabacloud_computenestsupplier20210521/client.py` & `alibabacloud_computenestsupplier20210521-3.0.0/alibabacloud_computenestsupplier20210521/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -37,19 +37,128 @@
     ) -> str:
         if not UtilClient.empty(endpoint):
             return endpoint
         if not UtilClient.is_unset(endpoint_map) and not UtilClient.empty(endpoint_map.get(region_id)):
             return endpoint_map.get(region_id)
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
+    def add_service_shared_accounts_with_options(
+        self,
+        request: compute_nest_supplier_20210521_models.AddServiceSharedAccountsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> compute_nest_supplier_20210521_models.AddServiceSharedAccountsResponse:
+        """
+        @param request: AddServiceSharedAccountsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: AddServiceSharedAccountsResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.client_token):
+            query['ClientToken'] = request.client_token
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.service_id):
+            query['ServiceId'] = request.service_id
+        if not UtilClient.is_unset(request.shared_accounts):
+            query['SharedAccounts'] = request.shared_accounts
+        if not UtilClient.is_unset(request.type):
+            query['Type'] = request.type
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='AddServiceSharedAccounts',
+            version='2021-05-21',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            compute_nest_supplier_20210521_models.AddServiceSharedAccountsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def add_service_shared_accounts_with_options_async(
+        self,
+        request: compute_nest_supplier_20210521_models.AddServiceSharedAccountsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> compute_nest_supplier_20210521_models.AddServiceSharedAccountsResponse:
+        """
+        @param request: AddServiceSharedAccountsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: AddServiceSharedAccountsResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.client_token):
+            query['ClientToken'] = request.client_token
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.service_id):
+            query['ServiceId'] = request.service_id
+        if not UtilClient.is_unset(request.shared_accounts):
+            query['SharedAccounts'] = request.shared_accounts
+        if not UtilClient.is_unset(request.type):
+            query['Type'] = request.type
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='AddServiceSharedAccounts',
+            version='2021-05-21',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            compute_nest_supplier_20210521_models.AddServiceSharedAccountsResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def add_service_shared_accounts(
+        self,
+        request: compute_nest_supplier_20210521_models.AddServiceSharedAccountsRequest,
+    ) -> compute_nest_supplier_20210521_models.AddServiceSharedAccountsResponse:
+        """
+        @param request: AddServiceSharedAccountsRequest
+        @return: AddServiceSharedAccountsResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return self.add_service_shared_accounts_with_options(request, runtime)
+
+    async def add_service_shared_accounts_async(
+        self,
+        request: compute_nest_supplier_20210521_models.AddServiceSharedAccountsRequest,
+    ) -> compute_nest_supplier_20210521_models.AddServiceSharedAccountsResponse:
+        """
+        @param request: AddServiceSharedAccountsRequest
+        @return: AddServiceSharedAccountsResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return await self.add_service_shared_accounts_with_options_async(request, runtime)
+
     def continue_deploy_service_instance_with_options(
         self,
         request: compute_nest_supplier_20210521_models.ContinueDeployServiceInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.ContinueDeployServiceInstanceResponse:
+        """
+        @param request: ContinueDeployServiceInstanceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ContinueDeployServiceInstanceResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dry_run):
             query['DryRun'] = request.dry_run
         if not UtilClient.is_unset(request.parameters):
@@ -78,14 +187,19 @@
         )
 
     async def continue_deploy_service_instance_with_options_async(
         self,
         request: compute_nest_supplier_20210521_models.ContinueDeployServiceInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.ContinueDeployServiceInstanceResponse:
+        """
+        @param request: ContinueDeployServiceInstanceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ContinueDeployServiceInstanceResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dry_run):
             query['DryRun'] = request.dry_run
         if not UtilClient.is_unset(request.parameters):
@@ -113,29 +227,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def continue_deploy_service_instance(
         self,
         request: compute_nest_supplier_20210521_models.ContinueDeployServiceInstanceRequest,
     ) -> compute_nest_supplier_20210521_models.ContinueDeployServiceInstanceResponse:
+        """
+        @param request: ContinueDeployServiceInstanceRequest
+        @return: ContinueDeployServiceInstanceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.continue_deploy_service_instance_with_options(request, runtime)
 
     async def continue_deploy_service_instance_async(
         self,
         request: compute_nest_supplier_20210521_models.ContinueDeployServiceInstanceRequest,
     ) -> compute_nest_supplier_20210521_models.ContinueDeployServiceInstanceResponse:
+        """
+        @param request: ContinueDeployServiceInstanceRequest
+        @return: ContinueDeployServiceInstanceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.continue_deploy_service_instance_with_options_async(request, runtime)
 
     def create_artifact_with_options(
         self,
         tmp_req: compute_nest_supplier_20210521_models.CreateArtifactRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.CreateArtifactResponse:
+        """
+        @summary 创建部署物
+        
+        @param tmp_req: CreateArtifactRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateArtifactResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = compute_nest_supplier_20210521_models.CreateArtifactShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.artifact_property):
             request.artifact_property_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.artifact_property, 'ArtifactProperty', 'json')
         query = {}
         if not UtilClient.is_unset(request.artifact_id):
@@ -176,14 +305,21 @@
         )
 
     async def create_artifact_with_options_async(
         self,
         tmp_req: compute_nest_supplier_20210521_models.CreateArtifactRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.CreateArtifactResponse:
+        """
+        @summary 创建部署物
+        
+        @param tmp_req: CreateArtifactRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateArtifactResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = compute_nest_supplier_20210521_models.CreateArtifactShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.artifact_property):
             request.artifact_property_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.artifact_property, 'ArtifactProperty', 'json')
         query = {}
         if not UtilClient.is_unset(request.artifact_id):
@@ -223,35 +359,56 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_artifact(
         self,
         request: compute_nest_supplier_20210521_models.CreateArtifactRequest,
     ) -> compute_nest_supplier_20210521_models.CreateArtifactResponse:
+        """
+        @summary 创建部署物
+        
+        @param request: CreateArtifactRequest
+        @return: CreateArtifactResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_artifact_with_options(request, runtime)
 
     async def create_artifact_async(
         self,
         request: compute_nest_supplier_20210521_models.CreateArtifactRequest,
     ) -> compute_nest_supplier_20210521_models.CreateArtifactResponse:
+        """
+        @summary 创建部署物
+        
+        @param request: CreateArtifactRequest
+        @return: CreateArtifactResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_artifact_with_options_async(request, runtime)
 
     def create_service_with_options(
         self,
         request: compute_nest_supplier_20210521_models.CreateServiceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.CreateServiceResponse:
+        """
+        @summary 创建新服务版本
+        
+        @param request: CreateServiceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateServiceResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.alarm_metadata):
             query['AlarmMetadata'] = request.alarm_metadata
         if not UtilClient.is_unset(request.approval_type):
             query['ApprovalType'] = request.approval_type
+        if not UtilClient.is_unset(request.build_parameters):
+            query['BuildParameters'] = request.build_parameters
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.deploy_metadata):
             query['DeployMetadata'] = request.deploy_metadata
         if not UtilClient.is_unset(request.deploy_type):
             query['DeployType'] = request.deploy_type
         if not UtilClient.is_unset(request.duration):
@@ -264,14 +421,16 @@
             query['LogMetadata'] = request.log_metadata
         if not UtilClient.is_unset(request.operation_metadata):
             query['OperationMetadata'] = request.operation_metadata
         if not UtilClient.is_unset(request.policy_names):
             query['PolicyNames'] = request.policy_names
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resellable):
+            query['Resellable'] = request.resellable
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         if not UtilClient.is_unset(request.service_id):
             query['ServiceId'] = request.service_id
         if not UtilClient.is_unset(request.service_info):
             query['ServiceInfo'] = request.service_info
         if not UtilClient.is_unset(request.service_type):
@@ -312,20 +471,29 @@
         )
 
     async def create_service_with_options_async(
         self,
         request: compute_nest_supplier_20210521_models.CreateServiceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.CreateServiceResponse:
+        """
+        @summary 创建新服务版本
+        
+        @param request: CreateServiceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateServiceResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.alarm_metadata):
             query['AlarmMetadata'] = request.alarm_metadata
         if not UtilClient.is_unset(request.approval_type):
             query['ApprovalType'] = request.approval_type
+        if not UtilClient.is_unset(request.build_parameters):
+            query['BuildParameters'] = request.build_parameters
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.deploy_metadata):
             query['DeployMetadata'] = request.deploy_metadata
         if not UtilClient.is_unset(request.deploy_type):
             query['DeployType'] = request.deploy_type
         if not UtilClient.is_unset(request.duration):
@@ -338,14 +506,16 @@
             query['LogMetadata'] = request.log_metadata
         if not UtilClient.is_unset(request.operation_metadata):
             query['OperationMetadata'] = request.operation_metadata
         if not UtilClient.is_unset(request.policy_names):
             query['PolicyNames'] = request.policy_names
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resellable):
+            query['Resellable'] = request.resellable
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         if not UtilClient.is_unset(request.service_id):
             query['ServiceId'] = request.service_id
         if not UtilClient.is_unset(request.service_info):
             query['ServiceInfo'] = request.service_info
         if not UtilClient.is_unset(request.service_type):
@@ -385,39 +555,60 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_service(
         self,
         request: compute_nest_supplier_20210521_models.CreateServiceRequest,
     ) -> compute_nest_supplier_20210521_models.CreateServiceResponse:
+        """
+        @summary 创建新服务版本
+        
+        @param request: CreateServiceRequest
+        @return: CreateServiceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_service_with_options(request, runtime)
 
     async def create_service_async(
         self,
         request: compute_nest_supplier_20210521_models.CreateServiceRequest,
     ) -> compute_nest_supplier_20210521_models.CreateServiceResponse:
+        """
+        @summary 创建新服务版本
+        
+        @param request: CreateServiceRequest
+        @return: CreateServiceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_service_with_options_async(request, runtime)
 
     def create_service_instance_with_options(
         self,
         tmp_req: compute_nest_supplier_20210521_models.CreateServiceInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.CreateServiceInstanceResponse:
+        """
+        @summary 商家侧创建服务实例
+        
+        @param tmp_req: CreateServiceInstanceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateServiceInstanceResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = compute_nest_supplier_20210521_models.CreateServiceInstanceShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.parameters):
             request.parameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.parameters, 'Parameters', 'json')
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dry_run):
             query['DryRun'] = request.dry_run
+        if not UtilClient.is_unset(request.end_time):
+            query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.name):
             query['Name'] = request.name
         if not UtilClient.is_unset(request.parameters_shrink):
             query['Parameters'] = request.parameters_shrink
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_group_id):
@@ -454,24 +645,33 @@
         )
 
     async def create_service_instance_with_options_async(
         self,
         tmp_req: compute_nest_supplier_20210521_models.CreateServiceInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.CreateServiceInstanceResponse:
+        """
+        @summary 商家侧创建服务实例
+        
+        @param tmp_req: CreateServiceInstanceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateServiceInstanceResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = compute_nest_supplier_20210521_models.CreateServiceInstanceShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.parameters):
             request.parameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.parameters, 'Parameters', 'json')
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dry_run):
             query['DryRun'] = request.dry_run
+        if not UtilClient.is_unset(request.end_time):
+            query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.name):
             query['Name'] = request.name
         if not UtilClient.is_unset(request.parameters_shrink):
             query['Parameters'] = request.parameters_shrink
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_group_id):
@@ -507,29 +707,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_service_instance(
         self,
         request: compute_nest_supplier_20210521_models.CreateServiceInstanceRequest,
     ) -> compute_nest_supplier_20210521_models.CreateServiceInstanceResponse:
+        """
+        @summary 商家侧创建服务实例
+        
+        @param request: CreateServiceInstanceRequest
+        @return: CreateServiceInstanceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_service_instance_with_options(request, runtime)
 
     async def create_service_instance_async(
         self,
         request: compute_nest_supplier_20210521_models.CreateServiceInstanceRequest,
     ) -> compute_nest_supplier_20210521_models.CreateServiceInstanceResponse:
+        """
+        @summary 商家侧创建服务实例
+        
+        @param request: CreateServiceInstanceRequest
+        @return: CreateServiceInstanceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_service_instance_with_options_async(request, runtime)
 
     def delete_artifact_with_options(
         self,
         request: compute_nest_supplier_20210521_models.DeleteArtifactRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.DeleteArtifactResponse:
+        """
+        @summary 删除部署物
+        
+        @param request: DeleteArtifactRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteArtifactResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.artifact_id):
             query['ArtifactId'] = request.artifact_id
         if not UtilClient.is_unset(request.artifact_version):
             query['ArtifactVersion'] = request.artifact_version
         req = open_api_models.OpenApiRequest(
@@ -552,14 +771,21 @@
         )
 
     async def delete_artifact_with_options_async(
         self,
         request: compute_nest_supplier_20210521_models.DeleteArtifactRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.DeleteArtifactResponse:
+        """
+        @summary 删除部署物
+        
+        @param request: DeleteArtifactRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteArtifactResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.artifact_id):
             query['ArtifactId'] = request.artifact_id
         if not UtilClient.is_unset(request.artifact_version):
             query['ArtifactVersion'] = request.artifact_version
         req = open_api_models.OpenApiRequest(
@@ -581,29 +807,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_artifact(
         self,
         request: compute_nest_supplier_20210521_models.DeleteArtifactRequest,
     ) -> compute_nest_supplier_20210521_models.DeleteArtifactResponse:
+        """
+        @summary 删除部署物
+        
+        @param request: DeleteArtifactRequest
+        @return: DeleteArtifactResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_artifact_with_options(request, runtime)
 
     async def delete_artifact_async(
         self,
         request: compute_nest_supplier_20210521_models.DeleteArtifactRequest,
     ) -> compute_nest_supplier_20210521_models.DeleteArtifactResponse:
+        """
+        @summary 删除部署物
+        
+        @param request: DeleteArtifactRequest
+        @return: DeleteArtifactResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_artifact_with_options_async(request, runtime)
 
     def delete_service_with_options(
         self,
         request: compute_nest_supplier_20210521_models.DeleteServiceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.DeleteServiceResponse:
+        """
+        @param request: DeleteServiceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteServiceResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.service_id):
@@ -630,14 +873,19 @@
         )
 
     async def delete_service_with_options_async(
         self,
         request: compute_nest_supplier_20210521_models.DeleteServiceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.DeleteServiceResponse:
+        """
+        @param request: DeleteServiceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteServiceResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.service_id):
@@ -663,29 +911,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_service(
         self,
         request: compute_nest_supplier_20210521_models.DeleteServiceRequest,
     ) -> compute_nest_supplier_20210521_models.DeleteServiceResponse:
+        """
+        @param request: DeleteServiceRequest
+        @return: DeleteServiceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_service_with_options(request, runtime)
 
     async def delete_service_async(
         self,
         request: compute_nest_supplier_20210521_models.DeleteServiceRequest,
     ) -> compute_nest_supplier_20210521_models.DeleteServiceResponse:
+        """
+        @param request: DeleteServiceRequest
+        @return: DeleteServiceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_service_with_options_async(request, runtime)
 
     def delete_service_instances_with_options(
         self,
         request: compute_nest_supplier_20210521_models.DeleteServiceInstancesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.DeleteServiceInstancesResponse:
+        """
+        @param request: DeleteServiceInstancesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteServiceInstancesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.service_instance_id):
@@ -710,14 +971,19 @@
         )
 
     async def delete_service_instances_with_options_async(
         self,
         request: compute_nest_supplier_20210521_models.DeleteServiceInstancesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.DeleteServiceInstancesResponse:
+        """
+        @param request: DeleteServiceInstancesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteServiceInstancesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.service_instance_id):
@@ -741,29 +1007,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_service_instances(
         self,
         request: compute_nest_supplier_20210521_models.DeleteServiceInstancesRequest,
     ) -> compute_nest_supplier_20210521_models.DeleteServiceInstancesResponse:
+        """
+        @param request: DeleteServiceInstancesRequest
+        @return: DeleteServiceInstancesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_service_instances_with_options(request, runtime)
 
     async def delete_service_instances_async(
         self,
         request: compute_nest_supplier_20210521_models.DeleteServiceInstancesRequest,
     ) -> compute_nest_supplier_20210521_models.DeleteServiceInstancesResponse:
+        """
+        @param request: DeleteServiceInstancesRequest
+        @return: DeleteServiceInstancesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_service_instances_with_options_async(request, runtime)
 
     def deploy_service_instance_with_options(
         self,
         request: compute_nest_supplier_20210521_models.DeployServiceInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.DeployServiceInstanceResponse:
+        """
+        @param request: DeployServiceInstanceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeployServiceInstanceResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.service_instance_id):
@@ -788,14 +1067,19 @@
         )
 
     async def deploy_service_instance_with_options_async(
         self,
         request: compute_nest_supplier_20210521_models.DeployServiceInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.DeployServiceInstanceResponse:
+        """
+        @param request: DeployServiceInstanceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeployServiceInstanceResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.service_instance_id):
@@ -819,29 +1103,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def deploy_service_instance(
         self,
         request: compute_nest_supplier_20210521_models.DeployServiceInstanceRequest,
     ) -> compute_nest_supplier_20210521_models.DeployServiceInstanceResponse:
+        """
+        @param request: DeployServiceInstanceRequest
+        @return: DeployServiceInstanceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.deploy_service_instance_with_options(request, runtime)
 
     async def deploy_service_instance_async(
         self,
         request: compute_nest_supplier_20210521_models.DeployServiceInstanceRequest,
     ) -> compute_nest_supplier_20210521_models.DeployServiceInstanceResponse:
+        """
+        @param request: DeployServiceInstanceRequest
+        @return: DeployServiceInstanceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.deploy_service_instance_with_options_async(request, runtime)
 
     def get_artifact_with_options(
         self,
         request: compute_nest_supplier_20210521_models.GetArtifactRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.GetArtifactResponse:
+        """
+        @summary 获取部署物信息
+        
+        @param request: GetArtifactRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetArtifactResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.artifact_id):
             query['ArtifactId'] = request.artifact_id
         if not UtilClient.is_unset(request.artifact_name):
             query['ArtifactName'] = request.artifact_name
         if not UtilClient.is_unset(request.artifact_version):
@@ -866,14 +1165,21 @@
         )
 
     async def get_artifact_with_options_async(
         self,
         request: compute_nest_supplier_20210521_models.GetArtifactRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.GetArtifactResponse:
+        """
+        @summary 获取部署物信息
+        
+        @param request: GetArtifactRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetArtifactResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.artifact_id):
             query['ArtifactId'] = request.artifact_id
         if not UtilClient.is_unset(request.artifact_name):
             query['ArtifactName'] = request.artifact_name
         if not UtilClient.is_unset(request.artifact_version):
@@ -897,29 +1203,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_artifact(
         self,
         request: compute_nest_supplier_20210521_models.GetArtifactRequest,
     ) -> compute_nest_supplier_20210521_models.GetArtifactResponse:
+        """
+        @summary 获取部署物信息
+        
+        @param request: GetArtifactRequest
+        @return: GetArtifactResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_artifact_with_options(request, runtime)
 
     async def get_artifact_async(
         self,
         request: compute_nest_supplier_20210521_models.GetArtifactRequest,
     ) -> compute_nest_supplier_20210521_models.GetArtifactResponse:
+        """
+        @summary 获取部署物信息
+        
+        @param request: GetArtifactRequest
+        @return: GetArtifactResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_artifact_with_options_async(request, runtime)
 
     def get_artifact_repository_credentials_with_options(
         self,
         request: compute_nest_supplier_20210521_models.GetArtifactRepositoryCredentialsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.GetArtifactRepositoryCredentialsResponse:
+        """
+        @summary 获取部署物仓库访问凭证
+        
+        @param request: GetArtifactRepositoryCredentialsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetArtifactRepositoryCredentialsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.artifact_type):
             query['ArtifactType'] = request.artifact_type
         if not UtilClient.is_unset(request.deploy_region_id):
             query['DeployRegionId'] = request.deploy_region_id
         req = open_api_models.OpenApiRequest(
@@ -942,14 +1267,21 @@
         )
 
     async def get_artifact_repository_credentials_with_options_async(
         self,
         request: compute_nest_supplier_20210521_models.GetArtifactRepositoryCredentialsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.GetArtifactRepositoryCredentialsResponse:
+        """
+        @summary 获取部署物仓库访问凭证
+        
+        @param request: GetArtifactRepositoryCredentialsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetArtifactRepositoryCredentialsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.artifact_type):
             query['ArtifactType'] = request.artifact_type
         if not UtilClient.is_unset(request.deploy_region_id):
             query['DeployRegionId'] = request.deploy_region_id
         req = open_api_models.OpenApiRequest(
@@ -971,29 +1303,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_artifact_repository_credentials(
         self,
         request: compute_nest_supplier_20210521_models.GetArtifactRepositoryCredentialsRequest,
     ) -> compute_nest_supplier_20210521_models.GetArtifactRepositoryCredentialsResponse:
+        """
+        @summary 获取部署物仓库访问凭证
+        
+        @param request: GetArtifactRepositoryCredentialsRequest
+        @return: GetArtifactRepositoryCredentialsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_artifact_repository_credentials_with_options(request, runtime)
 
     async def get_artifact_repository_credentials_async(
         self,
         request: compute_nest_supplier_20210521_models.GetArtifactRepositoryCredentialsRequest,
     ) -> compute_nest_supplier_20210521_models.GetArtifactRepositoryCredentialsResponse:
+        """
+        @summary 获取部署物仓库访问凭证
+        
+        @param request: GetArtifactRepositoryCredentialsRequest
+        @return: GetArtifactRepositoryCredentialsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_artifact_repository_credentials_with_options_async(request, runtime)
 
     def get_service_with_options(
         self,
         request: compute_nest_supplier_20210521_models.GetServiceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.GetServiceResponse:
+        """
+        @summary 查询服务详情
+        
+        @param request: GetServiceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetServiceResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.filter_ali_uid):
             query['FilterAliUid'] = request.filter_ali_uid
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.service_id):
@@ -1024,14 +1375,21 @@
         )
 
     async def get_service_with_options_async(
         self,
         request: compute_nest_supplier_20210521_models.GetServiceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.GetServiceResponse:
+        """
+        @summary 查询服务详情
+        
+        @param request: GetServiceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetServiceResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.filter_ali_uid):
             query['FilterAliUid'] = request.filter_ali_uid
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.service_id):
@@ -1061,37 +1419,60 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_service(
         self,
         request: compute_nest_supplier_20210521_models.GetServiceRequest,
     ) -> compute_nest_supplier_20210521_models.GetServiceResponse:
+        """
+        @summary 查询服务详情
+        
+        @param request: GetServiceRequest
+        @return: GetServiceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_service_with_options(request, runtime)
 
     async def get_service_async(
         self,
         request: compute_nest_supplier_20210521_models.GetServiceRequest,
     ) -> compute_nest_supplier_20210521_models.GetServiceResponse:
+        """
+        @summary 查询服务详情
+        
+        @param request: GetServiceRequest
+        @return: GetServiceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_service_with_options_async(request, runtime)
 
     def get_service_estimate_cost_with_options(
         self,
         tmp_req: compute_nest_supplier_20210521_models.GetServiceEstimateCostRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.GetServiceEstimateCostResponse:
+        """
+        @summary 计算巢服务部署询价
+        
+        @param tmp_req: GetServiceEstimateCostRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetServiceEstimateCostResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = compute_nest_supplier_20210521_models.GetServiceEstimateCostShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.commodity):
+            request.commodity_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.commodity, 'Commodity', 'json')
         if not UtilClient.is_unset(tmp_req.parameters):
             request.parameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.parameters, 'Parameters', 'json')
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
+        if not UtilClient.is_unset(request.commodity_shrink):
+            query['Commodity'] = request.commodity_shrink
         if not UtilClient.is_unset(request.parameters_shrink):
             query['Parameters'] = request.parameters_shrink
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.service_id):
             query['ServiceId'] = request.service_id
         if not UtilClient.is_unset(request.service_instance_id):
@@ -1122,22 +1503,33 @@
         )
 
     async def get_service_estimate_cost_with_options_async(
         self,
         tmp_req: compute_nest_supplier_20210521_models.GetServiceEstimateCostRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.GetServiceEstimateCostResponse:
+        """
+        @summary 计算巢服务部署询价
+        
+        @param tmp_req: GetServiceEstimateCostRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetServiceEstimateCostResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = compute_nest_supplier_20210521_models.GetServiceEstimateCostShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.commodity):
+            request.commodity_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.commodity, 'Commodity', 'json')
         if not UtilClient.is_unset(tmp_req.parameters):
             request.parameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.parameters, 'Parameters', 'json')
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
+        if not UtilClient.is_unset(request.commodity_shrink):
+            query['Commodity'] = request.commodity_shrink
         if not UtilClient.is_unset(request.parameters_shrink):
             query['Parameters'] = request.parameters_shrink
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.service_id):
             query['ServiceId'] = request.service_id
         if not UtilClient.is_unset(request.service_instance_id):
@@ -1167,29 +1559,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_service_estimate_cost(
         self,
         request: compute_nest_supplier_20210521_models.GetServiceEstimateCostRequest,
     ) -> compute_nest_supplier_20210521_models.GetServiceEstimateCostResponse:
+        """
+        @summary 计算巢服务部署询价
+        
+        @param request: GetServiceEstimateCostRequest
+        @return: GetServiceEstimateCostResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_service_estimate_cost_with_options(request, runtime)
 
     async def get_service_estimate_cost_async(
         self,
         request: compute_nest_supplier_20210521_models.GetServiceEstimateCostRequest,
     ) -> compute_nest_supplier_20210521_models.GetServiceEstimateCostResponse:
+        """
+        @summary 计算巢服务部署询价
+        
+        @param request: GetServiceEstimateCostRequest
+        @return: GetServiceEstimateCostResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_service_estimate_cost_with_options_async(request, runtime)
 
     def get_service_instance_with_options(
         self,
         request: compute_nest_supplier_20210521_models.GetServiceInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.GetServiceInstanceResponse:
+        """
+        @param request: GetServiceInstanceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetServiceInstanceResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.service_instance_id):
             query['ServiceInstanceId'] = request.service_instance_id
         req = open_api_models.OpenApiRequest(
@@ -1212,14 +1621,19 @@
         )
 
     async def get_service_instance_with_options_async(
         self,
         request: compute_nest_supplier_20210521_models.GetServiceInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.GetServiceInstanceResponse:
+        """
+        @param request: GetServiceInstanceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetServiceInstanceResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.service_instance_id):
             query['ServiceInstanceId'] = request.service_instance_id
         req = open_api_models.OpenApiRequest(
@@ -1241,29 +1655,170 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_service_instance(
         self,
         request: compute_nest_supplier_20210521_models.GetServiceInstanceRequest,
     ) -> compute_nest_supplier_20210521_models.GetServiceInstanceResponse:
+        """
+        @param request: GetServiceInstanceRequest
+        @return: GetServiceInstanceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_service_instance_with_options(request, runtime)
 
     async def get_service_instance_async(
         self,
         request: compute_nest_supplier_20210521_models.GetServiceInstanceRequest,
     ) -> compute_nest_supplier_20210521_models.GetServiceInstanceResponse:
+        """
+        @param request: GetServiceInstanceRequest
+        @return: GetServiceInstanceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_service_instance_with_options_async(request, runtime)
 
+    def get_service_template_parameter_constraints_with_options(
+        self,
+        request: compute_nest_supplier_20210521_models.GetServiceTemplateParameterConstraintsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> compute_nest_supplier_20210521_models.GetServiceTemplateParameterConstraintsResponse:
+        """
+        @summary 获取ROS模板参数限制
+        
+        @param request: GetServiceTemplateParameterConstraintsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetServiceTemplateParameterConstraintsResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.client_token):
+            query['ClientToken'] = request.client_token
+        if not UtilClient.is_unset(request.deploy_region_id):
+            query['DeployRegionId'] = request.deploy_region_id
+        if not UtilClient.is_unset(request.enable_private_vpc_connection):
+            query['EnablePrivateVpcConnection'] = request.enable_private_vpc_connection
+        if not UtilClient.is_unset(request.parameters):
+            query['Parameters'] = request.parameters
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.service_id):
+            query['ServiceId'] = request.service_id
+        if not UtilClient.is_unset(request.service_instance_id):
+            query['ServiceInstanceId'] = request.service_instance_id
+        if not UtilClient.is_unset(request.service_version):
+            query['ServiceVersion'] = request.service_version
+        if not UtilClient.is_unset(request.template_name):
+            query['TemplateName'] = request.template_name
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetServiceTemplateParameterConstraints',
+            version='2021-05-21',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            compute_nest_supplier_20210521_models.GetServiceTemplateParameterConstraintsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_service_template_parameter_constraints_with_options_async(
+        self,
+        request: compute_nest_supplier_20210521_models.GetServiceTemplateParameterConstraintsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> compute_nest_supplier_20210521_models.GetServiceTemplateParameterConstraintsResponse:
+        """
+        @summary 获取ROS模板参数限制
+        
+        @param request: GetServiceTemplateParameterConstraintsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetServiceTemplateParameterConstraintsResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.client_token):
+            query['ClientToken'] = request.client_token
+        if not UtilClient.is_unset(request.deploy_region_id):
+            query['DeployRegionId'] = request.deploy_region_id
+        if not UtilClient.is_unset(request.enable_private_vpc_connection):
+            query['EnablePrivateVpcConnection'] = request.enable_private_vpc_connection
+        if not UtilClient.is_unset(request.parameters):
+            query['Parameters'] = request.parameters
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.service_id):
+            query['ServiceId'] = request.service_id
+        if not UtilClient.is_unset(request.service_instance_id):
+            query['ServiceInstanceId'] = request.service_instance_id
+        if not UtilClient.is_unset(request.service_version):
+            query['ServiceVersion'] = request.service_version
+        if not UtilClient.is_unset(request.template_name):
+            query['TemplateName'] = request.template_name
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetServiceTemplateParameterConstraints',
+            version='2021-05-21',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            compute_nest_supplier_20210521_models.GetServiceTemplateParameterConstraintsResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_service_template_parameter_constraints(
+        self,
+        request: compute_nest_supplier_20210521_models.GetServiceTemplateParameterConstraintsRequest,
+    ) -> compute_nest_supplier_20210521_models.GetServiceTemplateParameterConstraintsResponse:
+        """
+        @summary 获取ROS模板参数限制
+        
+        @param request: GetServiceTemplateParameterConstraintsRequest
+        @return: GetServiceTemplateParameterConstraintsResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return self.get_service_template_parameter_constraints_with_options(request, runtime)
+
+    async def get_service_template_parameter_constraints_async(
+        self,
+        request: compute_nest_supplier_20210521_models.GetServiceTemplateParameterConstraintsRequest,
+    ) -> compute_nest_supplier_20210521_models.GetServiceTemplateParameterConstraintsResponse:
+        """
+        @summary 获取ROS模板参数限制
+        
+        @param request: GetServiceTemplateParameterConstraintsRequest
+        @return: GetServiceTemplateParameterConstraintsResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return await self.get_service_template_parameter_constraints_with_options_async(request, runtime)
+
     def get_upload_credentials_with_options(
         self,
         request: compute_nest_supplier_20210521_models.GetUploadCredentialsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.GetUploadCredentialsResponse:
+        """
+        @param request: GetUploadCredentialsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetUploadCredentialsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.file_name):
             query['FileName'] = request.file_name
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -1284,14 +1839,19 @@
         )
 
     async def get_upload_credentials_with_options_async(
         self,
         request: compute_nest_supplier_20210521_models.GetUploadCredentialsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.GetUploadCredentialsResponse:
+        """
+        @param request: GetUploadCredentialsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetUploadCredentialsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.file_name):
             query['FileName'] = request.file_name
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -1311,29 +1871,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_upload_credentials(
         self,
         request: compute_nest_supplier_20210521_models.GetUploadCredentialsRequest,
     ) -> compute_nest_supplier_20210521_models.GetUploadCredentialsResponse:
+        """
+        @param request: GetUploadCredentialsRequest
+        @return: GetUploadCredentialsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_upload_credentials_with_options(request, runtime)
 
     async def get_upload_credentials_async(
         self,
         request: compute_nest_supplier_20210521_models.GetUploadCredentialsRequest,
     ) -> compute_nest_supplier_20210521_models.GetUploadCredentialsResponse:
+        """
+        @param request: GetUploadCredentialsRequest
+        @return: GetUploadCredentialsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_upload_credentials_with_options_async(request, runtime)
 
     def list_acr_image_repositories_with_options(
         self,
         request: compute_nest_supplier_20210521_models.ListAcrImageRepositoriesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.ListAcrImageRepositoriesResponse:
+        """
+        @summary 展示部署物
+        
+        @param request: ListAcrImageRepositoriesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListAcrImageRepositoriesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.artifact_type):
             query['ArtifactType'] = request.artifact_type
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
@@ -1360,14 +1935,21 @@
         )
 
     async def list_acr_image_repositories_with_options_async(
         self,
         request: compute_nest_supplier_20210521_models.ListAcrImageRepositoriesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.ListAcrImageRepositoriesResponse:
+        """
+        @summary 展示部署物
+        
+        @param request: ListAcrImageRepositoriesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListAcrImageRepositoriesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.artifact_type):
             query['ArtifactType'] = request.artifact_type
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
@@ -1393,29 +1975,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_acr_image_repositories(
         self,
         request: compute_nest_supplier_20210521_models.ListAcrImageRepositoriesRequest,
     ) -> compute_nest_supplier_20210521_models.ListAcrImageRepositoriesResponse:
+        """
+        @summary 展示部署物
+        
+        @param request: ListAcrImageRepositoriesRequest
+        @return: ListAcrImageRepositoriesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_acr_image_repositories_with_options(request, runtime)
 
     async def list_acr_image_repositories_async(
         self,
         request: compute_nest_supplier_20210521_models.ListAcrImageRepositoriesRequest,
     ) -> compute_nest_supplier_20210521_models.ListAcrImageRepositoriesResponse:
+        """
+        @summary 展示部署物
+        
+        @param request: ListAcrImageRepositoriesRequest
+        @return: ListAcrImageRepositoriesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_acr_image_repositories_with_options_async(request, runtime)
 
     def list_acr_image_tags_with_options(
         self,
         request: compute_nest_supplier_20210521_models.ListAcrImageTagsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.ListAcrImageTagsResponse:
+        """
+        @summary 展示部署物
+        
+        @param request: ListAcrImageTagsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListAcrImageTagsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.artifact_type):
             query['ArtifactType'] = request.artifact_type
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
@@ -1442,14 +2043,21 @@
         )
 
     async def list_acr_image_tags_with_options_async(
         self,
         request: compute_nest_supplier_20210521_models.ListAcrImageTagsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.ListAcrImageTagsResponse:
+        """
+        @summary 展示部署物
+        
+        @param request: ListAcrImageTagsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListAcrImageTagsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.artifact_type):
             query['ArtifactType'] = request.artifact_type
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
@@ -1475,35 +2083,54 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_acr_image_tags(
         self,
         request: compute_nest_supplier_20210521_models.ListAcrImageTagsRequest,
     ) -> compute_nest_supplier_20210521_models.ListAcrImageTagsResponse:
+        """
+        @summary 展示部署物
+        
+        @param request: ListAcrImageTagsRequest
+        @return: ListAcrImageTagsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_acr_image_tags_with_options(request, runtime)
 
     async def list_acr_image_tags_async(
         self,
         request: compute_nest_supplier_20210521_models.ListAcrImageTagsRequest,
     ) -> compute_nest_supplier_20210521_models.ListAcrImageTagsResponse:
+        """
+        @summary 展示部署物
+        
+        @param request: ListAcrImageTagsRequest
+        @return: ListAcrImageTagsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_acr_image_tags_with_options_async(request, runtime)
 
     def list_artifact_versions_with_options(
         self,
         request: compute_nest_supplier_20210521_models.ListArtifactVersionsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.ListArtifactVersionsResponse:
+        """
+        @summary 展示部署物版本
+        
+        @param request: ListArtifactVersionsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListArtifactVersionsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.artifact_id):
             query['ArtifactId'] = request.artifact_id
-        if not UtilClient.is_unset(request.max_result):
-            query['MaxResult'] = request.max_result
+        if not UtilClient.is_unset(request.max_results):
+            query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListArtifactVersions',
@@ -1522,20 +2149,27 @@
         )
 
     async def list_artifact_versions_with_options_async(
         self,
         request: compute_nest_supplier_20210521_models.ListArtifactVersionsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.ListArtifactVersionsResponse:
+        """
+        @summary 展示部署物版本
+        
+        @param request: ListArtifactVersionsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListArtifactVersionsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.artifact_id):
             query['ArtifactId'] = request.artifact_id
-        if not UtilClient.is_unset(request.max_result):
-            query['MaxResult'] = request.max_result
+        if not UtilClient.is_unset(request.max_results):
+            query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListArtifactVersions',
@@ -1553,29 +2187,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_artifact_versions(
         self,
         request: compute_nest_supplier_20210521_models.ListArtifactVersionsRequest,
     ) -> compute_nest_supplier_20210521_models.ListArtifactVersionsResponse:
+        """
+        @summary 展示部署物版本
+        
+        @param request: ListArtifactVersionsRequest
+        @return: ListArtifactVersionsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_artifact_versions_with_options(request, runtime)
 
     async def list_artifact_versions_async(
         self,
         request: compute_nest_supplier_20210521_models.ListArtifactVersionsRequest,
     ) -> compute_nest_supplier_20210521_models.ListArtifactVersionsResponse:
+        """
+        @summary 展示部署物版本
+        
+        @param request: ListArtifactVersionsRequest
+        @return: ListArtifactVersionsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_artifact_versions_with_options_async(request, runtime)
 
     def list_artifacts_with_options(
         self,
         request: compute_nest_supplier_20210521_models.ListArtifactsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.ListArtifactsResponse:
+        """
+        @summary 展示部署物
+        
+        @param request: ListArtifactsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListArtifactsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.filter):
             query['Filter'] = request.filter
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
@@ -1604,14 +2257,21 @@
         )
 
     async def list_artifacts_with_options_async(
         self,
         request: compute_nest_supplier_20210521_models.ListArtifactsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.ListArtifactsResponse:
+        """
+        @summary 展示部署物
+        
+        @param request: ListArtifactsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListArtifactsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.filter):
             query['Filter'] = request.filter
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
@@ -1639,29 +2299,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_artifacts(
         self,
         request: compute_nest_supplier_20210521_models.ListArtifactsRequest,
     ) -> compute_nest_supplier_20210521_models.ListArtifactsResponse:
+        """
+        @summary 展示部署物
+        
+        @param request: ListArtifactsRequest
+        @return: ListArtifactsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_artifacts_with_options(request, runtime)
 
     async def list_artifacts_async(
         self,
         request: compute_nest_supplier_20210521_models.ListArtifactsRequest,
     ) -> compute_nest_supplier_20210521_models.ListArtifactsResponse:
+        """
+        @summary 展示部署物
+        
+        @param request: ListArtifactsRequest
+        @return: ListArtifactsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_artifacts_with_options_async(request, runtime)
 
     def list_service_instances_with_options(
         self,
         request: compute_nest_supplier_20210521_models.ListServiceInstancesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.ListServiceInstancesResponse:
+        """
+        @param request: ListServiceInstancesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListServiceInstancesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.filter):
             query['Filter'] = request.filter
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
@@ -1694,14 +2371,19 @@
         )
 
     async def list_service_instances_with_options_async(
         self,
         request: compute_nest_supplier_20210521_models.ListServiceInstancesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.ListServiceInstancesResponse:
+        """
+        @param request: ListServiceInstancesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListServiceInstancesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.filter):
             query['Filter'] = request.filter
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
@@ -1733,37 +2415,54 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_service_instances(
         self,
         request: compute_nest_supplier_20210521_models.ListServiceInstancesRequest,
     ) -> compute_nest_supplier_20210521_models.ListServiceInstancesResponse:
+        """
+        @param request: ListServiceInstancesRequest
+        @return: ListServiceInstancesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_service_instances_with_options(request, runtime)
 
     async def list_service_instances_async(
         self,
         request: compute_nest_supplier_20210521_models.ListServiceInstancesRequest,
     ) -> compute_nest_supplier_20210521_models.ListServiceInstancesResponse:
+        """
+        @param request: ListServiceInstancesRequest
+        @return: ListServiceInstancesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_service_instances_with_options_async(request, runtime)
 
     def list_service_usages_with_options(
         self,
         request: compute_nest_supplier_20210521_models.ListServiceUsagesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.ListServiceUsagesResponse:
+        """
+        @summary 商家获取服务使用申请接口
+        
+        @param request: ListServiceUsagesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListServiceUsagesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.filter):
             query['Filter'] = request.filter
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
+        if not UtilClient.is_unset(request.supplier_role):
+            query['SupplierRole'] = request.supplier_role
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListServiceUsages',
             version='2021-05-21',
             protocol='HTTPS',
@@ -1780,22 +2479,31 @@
         )
 
     async def list_service_usages_with_options_async(
         self,
         request: compute_nest_supplier_20210521_models.ListServiceUsagesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.ListServiceUsagesResponse:
+        """
+        @summary 商家获取服务使用申请接口
+        
+        @param request: ListServiceUsagesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListServiceUsagesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.filter):
             query['Filter'] = request.filter
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
+        if not UtilClient.is_unset(request.supplier_role):
+            query['SupplierRole'] = request.supplier_role
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListServiceUsages',
             version='2021-05-21',
             protocol='HTTPS',
@@ -1811,29 +2519,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_service_usages(
         self,
         request: compute_nest_supplier_20210521_models.ListServiceUsagesRequest,
     ) -> compute_nest_supplier_20210521_models.ListServiceUsagesResponse:
+        """
+        @summary 商家获取服务使用申请接口
+        
+        @param request: ListServiceUsagesRequest
+        @return: ListServiceUsagesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_service_usages_with_options(request, runtime)
 
     async def list_service_usages_async(
         self,
         request: compute_nest_supplier_20210521_models.ListServiceUsagesRequest,
     ) -> compute_nest_supplier_20210521_models.ListServiceUsagesResponse:
+        """
+        @summary 商家获取服务使用申请接口
+        
+        @param request: ListServiceUsagesRequest
+        @return: ListServiceUsagesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_service_usages_with_options_async(request, runtime)
 
     def list_services_with_options(
         self,
         request: compute_nest_supplier_20210521_models.ListServicesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.ListServicesResponse:
+        """
+        @summary 查询服务
+        
+        @param request: ListServicesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListServicesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.all_versions):
             query['AllVersions'] = request.all_versions
         if not UtilClient.is_unset(request.filter):
             query['Filter'] = request.filter
         if not UtilClient.is_unset(request.max_results):
@@ -1866,14 +2593,21 @@
         )
 
     async def list_services_with_options_async(
         self,
         request: compute_nest_supplier_20210521_models.ListServicesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.ListServicesResponse:
+        """
+        @summary 查询服务
+        
+        @param request: ListServicesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListServicesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.all_versions):
             query['AllVersions'] = request.all_versions
         if not UtilClient.is_unset(request.filter):
             query['Filter'] = request.filter
         if not UtilClient.is_unset(request.max_results):
@@ -1905,29 +2639,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_services(
         self,
         request: compute_nest_supplier_20210521_models.ListServicesRequest,
     ) -> compute_nest_supplier_20210521_models.ListServicesResponse:
+        """
+        @summary 查询服务
+        
+        @param request: ListServicesRequest
+        @return: ListServicesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_services_with_options(request, runtime)
 
     async def list_services_async(
         self,
         request: compute_nest_supplier_20210521_models.ListServicesRequest,
     ) -> compute_nest_supplier_20210521_models.ListServicesResponse:
+        """
+        @summary 查询服务
+        
+        @param request: ListServicesRequest
+        @return: ListServicesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_services_with_options_async(request, runtime)
 
     def modify_service_instance_resources_with_options(
         self,
         request: compute_nest_supplier_20210521_models.ModifyServiceInstanceResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.ModifyServiceInstanceResourcesResponse:
+        """
+        @summary 修改服务实例资源
+        
+        @param request: ModifyServiceInstanceResourcesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyServiceInstanceResourcesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.resources):
             query['Resources'] = request.resources
         if not UtilClient.is_unset(request.service_instance_id):
             query['ServiceInstanceId'] = request.service_instance_id
         if not UtilClient.is_unset(request.service_instance_resources_action):
@@ -1952,14 +2705,21 @@
         )
 
     async def modify_service_instance_resources_with_options_async(
         self,
         request: compute_nest_supplier_20210521_models.ModifyServiceInstanceResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.ModifyServiceInstanceResourcesResponse:
+        """
+        @summary 修改服务实例资源
+        
+        @param request: ModifyServiceInstanceResourcesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyServiceInstanceResourcesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.resources):
             query['Resources'] = request.resources
         if not UtilClient.is_unset(request.service_instance_id):
             query['ServiceInstanceId'] = request.service_instance_id
         if not UtilClient.is_unset(request.service_instance_resources_action):
@@ -1983,29 +2743,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_service_instance_resources(
         self,
         request: compute_nest_supplier_20210521_models.ModifyServiceInstanceResourcesRequest,
     ) -> compute_nest_supplier_20210521_models.ModifyServiceInstanceResourcesResponse:
+        """
+        @summary 修改服务实例资源
+        
+        @param request: ModifyServiceInstanceResourcesRequest
+        @return: ModifyServiceInstanceResourcesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_service_instance_resources_with_options(request, runtime)
 
     async def modify_service_instance_resources_async(
         self,
         request: compute_nest_supplier_20210521_models.ModifyServiceInstanceResourcesRequest,
     ) -> compute_nest_supplier_20210521_models.ModifyServiceInstanceResourcesResponse:
+        """
+        @summary 修改服务实例资源
+        
+        @param request: ModifyServiceInstanceResourcesRequest
+        @return: ModifyServiceInstanceResourcesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_service_instance_resources_with_options_async(request, runtime)
 
     def push_metering_data_with_options(
         self,
         request: compute_nest_supplier_20210521_models.PushMeteringDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.PushMeteringDataResponse:
+        """
+        @param request: PushMeteringDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: PushMeteringDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.metering):
             query['Metering'] = request.metering
         if not UtilClient.is_unset(request.service_instance_id):
             query['ServiceInstanceId'] = request.service_instance_id
         req = open_api_models.OpenApiRequest(
@@ -2028,14 +2805,19 @@
         )
 
     async def push_metering_data_with_options_async(
         self,
         request: compute_nest_supplier_20210521_models.PushMeteringDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.PushMeteringDataResponse:
+        """
+        @param request: PushMeteringDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: PushMeteringDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.metering):
             query['Metering'] = request.metering
         if not UtilClient.is_unset(request.service_instance_id):
             query['ServiceInstanceId'] = request.service_instance_id
         req = open_api_models.OpenApiRequest(
@@ -2057,29 +2839,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def push_metering_data(
         self,
         request: compute_nest_supplier_20210521_models.PushMeteringDataRequest,
     ) -> compute_nest_supplier_20210521_models.PushMeteringDataResponse:
+        """
+        @param request: PushMeteringDataRequest
+        @return: PushMeteringDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.push_metering_data_with_options(request, runtime)
 
     async def push_metering_data_async(
         self,
         request: compute_nest_supplier_20210521_models.PushMeteringDataRequest,
     ) -> compute_nest_supplier_20210521_models.PushMeteringDataResponse:
+        """
+        @param request: PushMeteringDataRequest
+        @return: PushMeteringDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.push_metering_data_with_options_async(request, runtime)
 
     def register_service_with_options(
         self,
         request: compute_nest_supplier_20210521_models.RegisterServiceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.RegisterServiceResponse:
+        """
+        @param request: RegisterServiceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RegisterServiceResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.service_id):
@@ -2104,14 +2899,19 @@
         )
 
     async def register_service_with_options_async(
         self,
         request: compute_nest_supplier_20210521_models.RegisterServiceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.RegisterServiceResponse:
+        """
+        @param request: RegisterServiceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RegisterServiceResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.service_id):
@@ -2135,29 +2935,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def register_service(
         self,
         request: compute_nest_supplier_20210521_models.RegisterServiceRequest,
     ) -> compute_nest_supplier_20210521_models.RegisterServiceResponse:
+        """
+        @param request: RegisterServiceRequest
+        @return: RegisterServiceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.register_service_with_options(request, runtime)
 
     async def register_service_async(
         self,
         request: compute_nest_supplier_20210521_models.RegisterServiceRequest,
     ) -> compute_nest_supplier_20210521_models.RegisterServiceResponse:
+        """
+        @param request: RegisterServiceRequest
+        @return: RegisterServiceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.register_service_with_options_async(request, runtime)
 
     def release_artifact_with_options(
         self,
         request: compute_nest_supplier_20210521_models.ReleaseArtifactRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.ReleaseArtifactResponse:
+        """
+        @summary 发布部署物
+        
+        @param request: ReleaseArtifactRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ReleaseArtifactResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.artifact_id):
             query['ArtifactId'] = request.artifact_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -2178,14 +2993,21 @@
         )
 
     async def release_artifact_with_options_async(
         self,
         request: compute_nest_supplier_20210521_models.ReleaseArtifactRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.ReleaseArtifactResponse:
+        """
+        @summary 发布部署物
+        
+        @param request: ReleaseArtifactRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ReleaseArtifactResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.artifact_id):
             query['ArtifactId'] = request.artifact_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -2205,29 +3027,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def release_artifact(
         self,
         request: compute_nest_supplier_20210521_models.ReleaseArtifactRequest,
     ) -> compute_nest_supplier_20210521_models.ReleaseArtifactResponse:
+        """
+        @summary 发布部署物
+        
+        @param request: ReleaseArtifactRequest
+        @return: ReleaseArtifactResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.release_artifact_with_options(request, runtime)
 
     async def release_artifact_async(
         self,
         request: compute_nest_supplier_20210521_models.ReleaseArtifactRequest,
     ) -> compute_nest_supplier_20210521_models.ReleaseArtifactResponse:
+        """
+        @summary 发布部署物
+        
+        @param request: ReleaseArtifactRequest
+        @return: ReleaseArtifactResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.release_artifact_with_options_async(request, runtime)
 
     def update_artifact_with_options(
         self,
         tmp_req: compute_nest_supplier_20210521_models.UpdateArtifactRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.UpdateArtifactResponse:
+        """
+        @summary 更新部署物
+        
+        @param tmp_req: UpdateArtifactRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateArtifactResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = compute_nest_supplier_20210521_models.UpdateArtifactShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.artifact_property):
             request.artifact_property_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.artifact_property, 'ArtifactProperty', 'json')
         query = {}
         if not UtilClient.is_unset(request.artifact_id):
@@ -2260,14 +3101,21 @@
         )
 
     async def update_artifact_with_options_async(
         self,
         tmp_req: compute_nest_supplier_20210521_models.UpdateArtifactRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.UpdateArtifactResponse:
+        """
+        @summary 更新部署物
+        
+        @param tmp_req: UpdateArtifactRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateArtifactResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = compute_nest_supplier_20210521_models.UpdateArtifactShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.artifact_property):
             request.artifact_property_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.artifact_property, 'ArtifactProperty', 'json')
         query = {}
         if not UtilClient.is_unset(request.artifact_id):
@@ -2299,30 +3147,51 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_artifact(
         self,
         request: compute_nest_supplier_20210521_models.UpdateArtifactRequest,
     ) -> compute_nest_supplier_20210521_models.UpdateArtifactResponse:
+        """
+        @summary 更新部署物
+        
+        @param request: UpdateArtifactRequest
+        @return: UpdateArtifactResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.update_artifact_with_options(request, runtime)
 
     async def update_artifact_async(
         self,
         request: compute_nest_supplier_20210521_models.UpdateArtifactRequest,
     ) -> compute_nest_supplier_20210521_models.UpdateArtifactResponse:
+        """
+        @summary 更新部署物
+        
+        @param request: UpdateArtifactRequest
+        @return: UpdateArtifactResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.update_artifact_with_options_async(request, runtime)
 
     def update_service_with_options(
         self,
-        request: compute_nest_supplier_20210521_models.UpdateServiceRequest,
+        tmp_req: compute_nest_supplier_20210521_models.UpdateServiceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.UpdateServiceResponse:
-        UtilClient.validate_model(request)
+        """
+        @param tmp_req: UpdateServiceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateServiceResponse
+        """
+        UtilClient.validate_model(tmp_req)
+        request = compute_nest_supplier_20210521_models.UpdateServiceShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.update_option):
+            request.update_option_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.update_option, 'UpdateOption', 'json')
         query = {}
         if not UtilClient.is_unset(request.alarm_metadata):
             query['AlarmMetadata'] = request.alarm_metadata
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.deploy_metadata):
             query['DeployMetadata'] = request.deploy_metadata
@@ -2338,26 +3207,30 @@
             query['LogMetadata'] = request.log_metadata
         if not UtilClient.is_unset(request.operation_metadata):
             query['OperationMetadata'] = request.operation_metadata
         if not UtilClient.is_unset(request.policy_names):
             query['PolicyNames'] = request.policy_names
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resellable):
+            query['Resellable'] = request.resellable
         if not UtilClient.is_unset(request.service_id):
             query['ServiceId'] = request.service_id
         if not UtilClient.is_unset(request.service_info):
             query['ServiceInfo'] = request.service_info
         if not UtilClient.is_unset(request.service_type):
             query['ServiceType'] = request.service_type
         if not UtilClient.is_unset(request.service_version):
             query['ServiceVersion'] = request.service_version
         if not UtilClient.is_unset(request.tenant_type):
             query['TenantType'] = request.tenant_type
         if not UtilClient.is_unset(request.trial_duration):
             query['TrialDuration'] = request.trial_duration
+        if not UtilClient.is_unset(request.update_option_shrink):
+            query['UpdateOption'] = request.update_option_shrink
         if not UtilClient.is_unset(request.upgrade_metadata):
             query['UpgradeMetadata'] = request.upgrade_metadata
         if not UtilClient.is_unset(request.version_name):
             query['VersionName'] = request.version_name
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -2375,18 +3248,27 @@
         return TeaCore.from_map(
             compute_nest_supplier_20210521_models.UpdateServiceResponse(),
             self.call_api(params, req, runtime)
         )
 
     async def update_service_with_options_async(
         self,
-        request: compute_nest_supplier_20210521_models.UpdateServiceRequest,
+        tmp_req: compute_nest_supplier_20210521_models.UpdateServiceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.UpdateServiceResponse:
-        UtilClient.validate_model(request)
+        """
+        @param tmp_req: UpdateServiceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateServiceResponse
+        """
+        UtilClient.validate_model(tmp_req)
+        request = compute_nest_supplier_20210521_models.UpdateServiceShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.update_option):
+            request.update_option_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.update_option, 'UpdateOption', 'json')
         query = {}
         if not UtilClient.is_unset(request.alarm_metadata):
             query['AlarmMetadata'] = request.alarm_metadata
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.deploy_metadata):
             query['DeployMetadata'] = request.deploy_metadata
@@ -2402,26 +3284,30 @@
             query['LogMetadata'] = request.log_metadata
         if not UtilClient.is_unset(request.operation_metadata):
             query['OperationMetadata'] = request.operation_metadata
         if not UtilClient.is_unset(request.policy_names):
             query['PolicyNames'] = request.policy_names
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resellable):
+            query['Resellable'] = request.resellable
         if not UtilClient.is_unset(request.service_id):
             query['ServiceId'] = request.service_id
         if not UtilClient.is_unset(request.service_info):
             query['ServiceInfo'] = request.service_info
         if not UtilClient.is_unset(request.service_type):
             query['ServiceType'] = request.service_type
         if not UtilClient.is_unset(request.service_version):
             query['ServiceVersion'] = request.service_version
         if not UtilClient.is_unset(request.tenant_type):
             query['TenantType'] = request.tenant_type
         if not UtilClient.is_unset(request.trial_duration):
             query['TrialDuration'] = request.trial_duration
+        if not UtilClient.is_unset(request.update_option_shrink):
+            query['UpdateOption'] = request.update_option_shrink
         if not UtilClient.is_unset(request.upgrade_metadata):
             query['UpgradeMetadata'] = request.upgrade_metadata
         if not UtilClient.is_unset(request.version_name):
             query['VersionName'] = request.version_name
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -2441,16 +3327,368 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_service(
         self,
         request: compute_nest_supplier_20210521_models.UpdateServiceRequest,
     ) -> compute_nest_supplier_20210521_models.UpdateServiceResponse:
+        """
+        @param request: UpdateServiceRequest
+        @return: UpdateServiceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.update_service_with_options(request, runtime)
 
     async def update_service_async(
         self,
         request: compute_nest_supplier_20210521_models.UpdateServiceRequest,
     ) -> compute_nest_supplier_20210521_models.UpdateServiceResponse:
+        """
+        @param request: UpdateServiceRequest
+        @return: UpdateServiceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.update_service_with_options_async(request, runtime)
+
+    def update_service_instance_attribute_with_options(
+        self,
+        request: compute_nest_supplier_20210521_models.UpdateServiceInstanceAttributeRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> compute_nest_supplier_20210521_models.UpdateServiceInstanceAttributeResponse:
+        """
+        @summary 更新服务实例属性
+        
+        @param request: UpdateServiceInstanceAttributeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateServiceInstanceAttributeResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.end_time):
+            query['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.service_instance_id):
+            query['ServiceInstanceId'] = request.service_instance_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='UpdateServiceInstanceAttribute',
+            version='2021-05-21',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            compute_nest_supplier_20210521_models.UpdateServiceInstanceAttributeResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def update_service_instance_attribute_with_options_async(
+        self,
+        request: compute_nest_supplier_20210521_models.UpdateServiceInstanceAttributeRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> compute_nest_supplier_20210521_models.UpdateServiceInstanceAttributeResponse:
+        """
+        @summary 更新服务实例属性
+        
+        @param request: UpdateServiceInstanceAttributeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateServiceInstanceAttributeResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.end_time):
+            query['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.service_instance_id):
+            query['ServiceInstanceId'] = request.service_instance_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='UpdateServiceInstanceAttribute',
+            version='2021-05-21',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            compute_nest_supplier_20210521_models.UpdateServiceInstanceAttributeResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def update_service_instance_attribute(
+        self,
+        request: compute_nest_supplier_20210521_models.UpdateServiceInstanceAttributeRequest,
+    ) -> compute_nest_supplier_20210521_models.UpdateServiceInstanceAttributeResponse:
+        """
+        @summary 更新服务实例属性
+        
+        @param request: UpdateServiceInstanceAttributeRequest
+        @return: UpdateServiceInstanceAttributeResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return self.update_service_instance_attribute_with_options(request, runtime)
+
+    async def update_service_instance_attribute_async(
+        self,
+        request: compute_nest_supplier_20210521_models.UpdateServiceInstanceAttributeRequest,
+    ) -> compute_nest_supplier_20210521_models.UpdateServiceInstanceAttributeResponse:
+        """
+        @summary 更新服务实例属性
+        
+        @param request: UpdateServiceInstanceAttributeRequest
+        @return: UpdateServiceInstanceAttributeResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return await self.update_service_instance_attribute_with_options_async(request, runtime)
+
+    def update_service_instance_spec_with_options(
+        self,
+        tmp_req: compute_nest_supplier_20210521_models.UpdateServiceInstanceSpecRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> compute_nest_supplier_20210521_models.UpdateServiceInstanceSpecResponse:
+        """
+        @summary 变配服务实例
+        
+        @param tmp_req: UpdateServiceInstanceSpecRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateServiceInstanceSpecResponse
+        """
+        UtilClient.validate_model(tmp_req)
+        request = compute_nest_supplier_20210521_models.UpdateServiceInstanceSpecShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.parameters):
+            request.parameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.parameters, 'Parameters', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.client_token):
+            query['ClientToken'] = request.client_token
+        if not UtilClient.is_unset(request.enable_user_prometheus):
+            query['EnableUserPrometheus'] = request.enable_user_prometheus
+        if not UtilClient.is_unset(request.operation_name):
+            query['OperationName'] = request.operation_name
+        if not UtilClient.is_unset(request.parameters_shrink):
+            query['Parameters'] = request.parameters_shrink
+        if not UtilClient.is_unset(request.predefined_parameters_name):
+            query['PredefinedParametersName'] = request.predefined_parameters_name
+        if not UtilClient.is_unset(request.service_instance_id):
+            query['ServiceInstanceId'] = request.service_instance_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='UpdateServiceInstanceSpec',
+            version='2021-05-21',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            compute_nest_supplier_20210521_models.UpdateServiceInstanceSpecResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def update_service_instance_spec_with_options_async(
+        self,
+        tmp_req: compute_nest_supplier_20210521_models.UpdateServiceInstanceSpecRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> compute_nest_supplier_20210521_models.UpdateServiceInstanceSpecResponse:
+        """
+        @summary 变配服务实例
+        
+        @param tmp_req: UpdateServiceInstanceSpecRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateServiceInstanceSpecResponse
+        """
+        UtilClient.validate_model(tmp_req)
+        request = compute_nest_supplier_20210521_models.UpdateServiceInstanceSpecShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.parameters):
+            request.parameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.parameters, 'Parameters', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.client_token):
+            query['ClientToken'] = request.client_token
+        if not UtilClient.is_unset(request.enable_user_prometheus):
+            query['EnableUserPrometheus'] = request.enable_user_prometheus
+        if not UtilClient.is_unset(request.operation_name):
+            query['OperationName'] = request.operation_name
+        if not UtilClient.is_unset(request.parameters_shrink):
+            query['Parameters'] = request.parameters_shrink
+        if not UtilClient.is_unset(request.predefined_parameters_name):
+            query['PredefinedParametersName'] = request.predefined_parameters_name
+        if not UtilClient.is_unset(request.service_instance_id):
+            query['ServiceInstanceId'] = request.service_instance_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='UpdateServiceInstanceSpec',
+            version='2021-05-21',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            compute_nest_supplier_20210521_models.UpdateServiceInstanceSpecResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def update_service_instance_spec(
+        self,
+        request: compute_nest_supplier_20210521_models.UpdateServiceInstanceSpecRequest,
+    ) -> compute_nest_supplier_20210521_models.UpdateServiceInstanceSpecResponse:
+        """
+        @summary 变配服务实例
+        
+        @param request: UpdateServiceInstanceSpecRequest
+        @return: UpdateServiceInstanceSpecResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return self.update_service_instance_spec_with_options(request, runtime)
+
+    async def update_service_instance_spec_async(
+        self,
+        request: compute_nest_supplier_20210521_models.UpdateServiceInstanceSpecRequest,
+    ) -> compute_nest_supplier_20210521_models.UpdateServiceInstanceSpecResponse:
+        """
+        @summary 变配服务实例
+        
+        @param request: UpdateServiceInstanceSpecRequest
+        @return: UpdateServiceInstanceSpecResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return await self.update_service_instance_spec_with_options_async(request, runtime)
+
+    def upgrade_service_instance_with_options(
+        self,
+        tmp_req: compute_nest_supplier_20210521_models.UpgradeServiceInstanceRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> compute_nest_supplier_20210521_models.UpgradeServiceInstanceResponse:
+        """
+        @param tmp_req: UpgradeServiceInstanceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpgradeServiceInstanceResponse
+        """
+        UtilClient.validate_model(tmp_req)
+        request = compute_nest_supplier_20210521_models.UpgradeServiceInstanceShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.parameters):
+            request.parameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.parameters, 'Parameters', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.client_token):
+            query['ClientToken'] = request.client_token
+        if not UtilClient.is_unset(request.dry_run):
+            query['DryRun'] = request.dry_run
+        if not UtilClient.is_unset(request.parameters_shrink):
+            query['Parameters'] = request.parameters_shrink
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.service_instance_id):
+            query['ServiceInstanceId'] = request.service_instance_id
+        if not UtilClient.is_unset(request.service_version):
+            query['ServiceVersion'] = request.service_version
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='UpgradeServiceInstance',
+            version='2021-05-21',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            compute_nest_supplier_20210521_models.UpgradeServiceInstanceResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def upgrade_service_instance_with_options_async(
+        self,
+        tmp_req: compute_nest_supplier_20210521_models.UpgradeServiceInstanceRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> compute_nest_supplier_20210521_models.UpgradeServiceInstanceResponse:
+        """
+        @param tmp_req: UpgradeServiceInstanceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpgradeServiceInstanceResponse
+        """
+        UtilClient.validate_model(tmp_req)
+        request = compute_nest_supplier_20210521_models.UpgradeServiceInstanceShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.parameters):
+            request.parameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.parameters, 'Parameters', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.client_token):
+            query['ClientToken'] = request.client_token
+        if not UtilClient.is_unset(request.dry_run):
+            query['DryRun'] = request.dry_run
+        if not UtilClient.is_unset(request.parameters_shrink):
+            query['Parameters'] = request.parameters_shrink
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.service_instance_id):
+            query['ServiceInstanceId'] = request.service_instance_id
+        if not UtilClient.is_unset(request.service_version):
+            query['ServiceVersion'] = request.service_version
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='UpgradeServiceInstance',
+            version='2021-05-21',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            compute_nest_supplier_20210521_models.UpgradeServiceInstanceResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def upgrade_service_instance(
+        self,
+        request: compute_nest_supplier_20210521_models.UpgradeServiceInstanceRequest,
+    ) -> compute_nest_supplier_20210521_models.UpgradeServiceInstanceResponse:
+        """
+        @param request: UpgradeServiceInstanceRequest
+        @return: UpgradeServiceInstanceResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return self.upgrade_service_instance_with_options(request, runtime)
+
+    async def upgrade_service_instance_async(
+        self,
+        request: compute_nest_supplier_20210521_models.UpgradeServiceInstanceRequest,
+    ) -> compute_nest_supplier_20210521_models.UpgradeServiceInstanceResponse:
+        """
+        @param request: UpgradeServiceInstanceRequest
+        @return: UpgradeServiceInstanceResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return await self.upgrade_service_instance_with_options_async(request, runtime)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alibabacloud_computenestsupplier20210521-2.3.2/alibabacloud_computenestsupplier20210521/models.py` & `alibabacloud_computenestsupplier20210521-3.0.0/alibabacloud_computenestsupplier20210521/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,193 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
 from typing import List, Dict, Any
 
 
+class AddServiceSharedAccountsRequestSharedAccounts(TeaModel):
+    def __init__(
+        self,
+        permission: str = None,
+        user_ali_uid: str = None,
+    ):
+        # This parameter is required.
+        self.permission = permission
+        # This parameter is required.
+        self.user_ali_uid = user_ali_uid
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
+        if self.permission is not None:
+            result['Permission'] = self.permission
+        if self.user_ali_uid is not None:
+            result['UserAliUid'] = self.user_ali_uid
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Permission') is not None:
+            self.permission = m.get('Permission')
+        if m.get('UserAliUid') is not None:
+            self.user_ali_uid = m.get('UserAliUid')
+        return self
+
+
+class AddServiceSharedAccountsRequest(TeaModel):
+    def __init__(
+        self,
+        client_token: str = None,
+        region_id: str = None,
+        service_id: str = None,
+        shared_accounts: List[AddServiceSharedAccountsRequestSharedAccounts] = None,
+        type: str = None,
+    ):
+        self.client_token = client_token
+        # This parameter is required.
+        self.region_id = region_id
+        # This parameter is required.
+        self.service_id = service_id
+        # This parameter is required.
+        self.shared_accounts = shared_accounts
+        self.type = type
+
+    def validate(self):
+        if self.shared_accounts:
+            for k in self.shared_accounts:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.client_token is not None:
+            result['ClientToken'] = self.client_token
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.service_id is not None:
+            result['ServiceId'] = self.service_id
+        result['SharedAccounts'] = []
+        if self.shared_accounts is not None:
+            for k in self.shared_accounts:
+                result['SharedAccounts'].append(k.to_map() if k else None)
+        if self.type is not None:
+            result['Type'] = self.type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ClientToken') is not None:
+            self.client_token = m.get('ClientToken')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ServiceId') is not None:
+            self.service_id = m.get('ServiceId')
+        self.shared_accounts = []
+        if m.get('SharedAccounts') is not None:
+            for k in m.get('SharedAccounts'):
+                temp_model = AddServiceSharedAccountsRequestSharedAccounts()
+                self.shared_accounts.append(temp_model.from_map(k))
+        if m.get('Type') is not None:
+            self.type = m.get('Type')
+        return self
+
+
+class AddServiceSharedAccountsResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
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
+class AddServiceSharedAccountsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: AddServiceSharedAccountsResponseBody = None,
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
+            temp_model = AddServiceSharedAccountsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ContinueDeployServiceInstanceRequest(TeaModel):
     def __init__(
         self,
         client_token: str = None,
         dry_run: bool = None,
         parameters: str = None,
         region_id: str = None,
         service_instance_id: str = None,
     ):
         self.client_token = client_token
         self.dry_run = dry_run
         self.parameters = parameters
+        # This parameter is required.
         self.region_id = region_id
+        # This parameter is required.
         self.service_instance_id = service_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -143,17 +310,14 @@
         body: ContinueDeployServiceInstanceResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -304,20 +468,23 @@
         resource_group_id: str = None,
         support_region_ids: List[str] = None,
         tag: List[CreateArtifactRequestTag] = None,
         version_name: str = None,
     ):
         self.artifact_id = artifact_id
         self.artifact_property = artifact_property
+        # This parameter is required.
         self.artifact_type = artifact_type
         self.description = description
+        # This parameter is required.
         self.name = name
         self.resource_group_id = resource_group_id
         self.support_region_ids = support_region_ids
         self.tag = tag
+        # This parameter is required.
         self.version_name = version_name
 
     def validate(self):
         if self.artifact_property:
             self.artifact_property.validate()
         if self.tag:
             for k in self.tag:
@@ -423,20 +590,23 @@
         resource_group_id: str = None,
         support_region_ids: List[str] = None,
         tag: List[CreateArtifactShrinkRequestTag] = None,
         version_name: str = None,
     ):
         self.artifact_id = artifact_id
         self.artifact_property_shrink = artifact_property_shrink
+        # This parameter is required.
         self.artifact_type = artifact_type
         self.description = description
+        # This parameter is required.
         self.name = name
         self.resource_group_id = resource_group_id
         self.support_region_ids = support_region_ids
         self.tag = tag
+        # This parameter is required.
         self.version_name = version_name
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
@@ -596,17 +766,14 @@
         body: CreateArtifactResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -628,52 +795,101 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateArtifactResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateServiceRequestServiceInfoAgreements(TeaModel):
+    def __init__(
+        self,
+        name: str = None,
+        url: str = None,
+    ):
+        self.name = name
+        self.url = url
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
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.url is not None:
+            result['Url'] = self.url
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('Url') is not None:
+            self.url = m.get('Url')
+        return self
+
+
 class CreateServiceRequestServiceInfo(TeaModel):
     def __init__(
         self,
+        agreements: List[CreateServiceRequestServiceInfoAgreements] = None,
         image: str = None,
         locale: str = None,
         long_description_url: str = None,
         name: str = None,
         short_description: str = None,
     ):
+        self.agreements = agreements
         self.image = image
+        # This parameter is required.
         self.locale = locale
         self.long_description_url = long_description_url
+        # This parameter is required.
         self.name = name
         self.short_description = short_description
 
     def validate(self):
-        pass
+        if self.agreements:
+            for k in self.agreements:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        result['Agreements'] = []
+        if self.agreements is not None:
+            for k in self.agreements:
+                result['Agreements'].append(k.to_map() if k else None)
         if self.image is not None:
             result['Image'] = self.image
         if self.locale is not None:
             result['Locale'] = self.locale
         if self.long_description_url is not None:
             result['LongDescriptionUrl'] = self.long_description_url
         if self.name is not None:
             result['Name'] = self.name
         if self.short_description is not None:
             result['ShortDescription'] = self.short_description
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        self.agreements = []
+        if m.get('Agreements') is not None:
+            for k in m.get('Agreements'):
+                temp_model = CreateServiceRequestServiceInfoAgreements()
+                self.agreements.append(temp_model.from_map(k))
         if m.get('Image') is not None:
             self.image = m.get('Image')
         if m.get('Locale') is not None:
             self.locale = m.get('Locale')
         if m.get('LongDescriptionUrl') is not None:
             self.long_description_url = m.get('LongDescriptionUrl')
         if m.get('Name') is not None:
@@ -717,24 +933,26 @@
 
 
 class CreateServiceRequest(TeaModel):
     def __init__(
         self,
         alarm_metadata: str = None,
         approval_type: str = None,
+        build_parameters: str = None,
         client_token: str = None,
         deploy_metadata: str = None,
         deploy_type: str = None,
         duration: int = None,
         is_support_operated: bool = None,
         license_metadata: str = None,
         log_metadata: str = None,
         operation_metadata: str = None,
         policy_names: str = None,
         region_id: str = None,
+        resellable: bool = None,
         resource_group_id: str = None,
         service_id: str = None,
         service_info: List[CreateServiceRequestServiceInfo] = None,
         service_type: str = None,
         share_type: str = None,
         source_service_id: str = None,
         source_service_version: str = None,
@@ -742,24 +960,28 @@
         tenant_type: str = None,
         trial_duration: int = None,
         upgrade_metadata: str = None,
         version_name: str = None,
     ):
         self.alarm_metadata = alarm_metadata
         self.approval_type = approval_type
+        self.build_parameters = build_parameters
         self.client_token = client_token
         self.deploy_metadata = deploy_metadata
+        # This parameter is required.
         self.deploy_type = deploy_type
         self.duration = duration
         self.is_support_operated = is_support_operated
         self.license_metadata = license_metadata
         self.log_metadata = log_metadata
         self.operation_metadata = operation_metadata
         self.policy_names = policy_names
+        # This parameter is required.
         self.region_id = region_id
+        self.resellable = resellable
         self.resource_group_id = resource_group_id
         self.service_id = service_id
         self.service_info = service_info
         self.service_type = service_type
         self.share_type = share_type
         self.source_service_id = source_service_id
         self.source_service_version = source_service_version
@@ -785,14 +1007,16 @@
             return _map
 
         result = dict()
         if self.alarm_metadata is not None:
             result['AlarmMetadata'] = self.alarm_metadata
         if self.approval_type is not None:
             result['ApprovalType'] = self.approval_type
+        if self.build_parameters is not None:
+            result['BuildParameters'] = self.build_parameters
         if self.client_token is not None:
             result['ClientToken'] = self.client_token
         if self.deploy_metadata is not None:
             result['DeployMetadata'] = self.deploy_metadata
         if self.deploy_type is not None:
             result['DeployType'] = self.deploy_type
         if self.duration is not None:
@@ -805,14 +1029,16 @@
             result['LogMetadata'] = self.log_metadata
         if self.operation_metadata is not None:
             result['OperationMetadata'] = self.operation_metadata
         if self.policy_names is not None:
             result['PolicyNames'] = self.policy_names
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.resellable is not None:
+            result['Resellable'] = self.resellable
         if self.resource_group_id is not None:
             result['ResourceGroupId'] = self.resource_group_id
         if self.service_id is not None:
             result['ServiceId'] = self.service_id
         result['ServiceInfo'] = []
         if self.service_info is not None:
             for k in self.service_info:
@@ -841,14 +1067,16 @@
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AlarmMetadata') is not None:
             self.alarm_metadata = m.get('AlarmMetadata')
         if m.get('ApprovalType') is not None:
             self.approval_type = m.get('ApprovalType')
+        if m.get('BuildParameters') is not None:
+            self.build_parameters = m.get('BuildParameters')
         if m.get('ClientToken') is not None:
             self.client_token = m.get('ClientToken')
         if m.get('DeployMetadata') is not None:
             self.deploy_metadata = m.get('DeployMetadata')
         if m.get('DeployType') is not None:
             self.deploy_type = m.get('DeployType')
         if m.get('Duration') is not None:
@@ -861,14 +1089,16 @@
             self.log_metadata = m.get('LogMetadata')
         if m.get('OperationMetadata') is not None:
             self.operation_metadata = m.get('OperationMetadata')
         if m.get('PolicyNames') is not None:
             self.policy_names = m.get('PolicyNames')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('Resellable') is not None:
+            self.resellable = m.get('Resellable')
         if m.get('ResourceGroupId') is not None:
             self.resource_group_id = m.get('ResourceGroupId')
         if m.get('ServiceId') is not None:
             self.service_id = m.get('ServiceId')
         self.service_info = []
         if m.get('ServiceInfo') is not None:
             for k in m.get('ServiceInfo'):
@@ -951,17 +1181,14 @@
         body: CreateServiceResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1021,31 +1248,36 @@
 
 
 class CreateServiceInstanceRequest(TeaModel):
     def __init__(
         self,
         client_token: str = None,
         dry_run: bool = None,
+        end_time: str = None,
         name: str = None,
         parameters: Dict[str, Any] = None,
         region_id: str = None,
         resource_group_id: str = None,
         service_id: str = None,
         service_version: str = None,
         specification_name: str = None,
         tag: List[CreateServiceInstanceRequestTag] = None,
         template_name: str = None,
         user_id: str = None,
     ):
         self.client_token = client_token
         self.dry_run = dry_run
+        # Use the UTC time format: yyyy-MM-ddTHH:mmZ
+        self.end_time = end_time
         self.name = name
         self.parameters = parameters
+        # This parameter is required.
         self.region_id = region_id
         self.resource_group_id = resource_group_id
+        # This parameter is required.
         self.service_id = service_id
         self.service_version = service_version
         self.specification_name = specification_name
         self.tag = tag
         self.template_name = template_name
         self.user_id = user_id
 
@@ -1061,14 +1293,16 @@
             return _map
 
         result = dict()
         if self.client_token is not None:
             result['ClientToken'] = self.client_token
         if self.dry_run is not None:
             result['DryRun'] = self.dry_run
+        if self.end_time is not None:
+            result['EndTime'] = self.end_time
         if self.name is not None:
             result['Name'] = self.name
         if self.parameters is not None:
             result['Parameters'] = self.parameters
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.resource_group_id is not None:
@@ -1091,14 +1325,16 @@
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('ClientToken') is not None:
             self.client_token = m.get('ClientToken')
         if m.get('DryRun') is not None:
             self.dry_run = m.get('DryRun')
+        if m.get('EndTime') is not None:
+            self.end_time = m.get('EndTime')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('Parameters') is not None:
             self.parameters = m.get('Parameters')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('ResourceGroupId') is not None:
@@ -1155,31 +1391,36 @@
 
 
 class CreateServiceInstanceShrinkRequest(TeaModel):
     def __init__(
         self,
         client_token: str = None,
         dry_run: bool = None,
+        end_time: str = None,
         name: str = None,
         parameters_shrink: str = None,
         region_id: str = None,
         resource_group_id: str = None,
         service_id: str = None,
         service_version: str = None,
         specification_name: str = None,
         tag: List[CreateServiceInstanceShrinkRequestTag] = None,
         template_name: str = None,
         user_id: str = None,
     ):
         self.client_token = client_token
         self.dry_run = dry_run
+        # Use the UTC time format: yyyy-MM-ddTHH:mmZ
+        self.end_time = end_time
         self.name = name
         self.parameters_shrink = parameters_shrink
+        # This parameter is required.
         self.region_id = region_id
         self.resource_group_id = resource_group_id
+        # This parameter is required.
         self.service_id = service_id
         self.service_version = service_version
         self.specification_name = specification_name
         self.tag = tag
         self.template_name = template_name
         self.user_id = user_id
 
@@ -1195,14 +1436,16 @@
             return _map
 
         result = dict()
         if self.client_token is not None:
             result['ClientToken'] = self.client_token
         if self.dry_run is not None:
             result['DryRun'] = self.dry_run
+        if self.end_time is not None:
+            result['EndTime'] = self.end_time
         if self.name is not None:
             result['Name'] = self.name
         if self.parameters_shrink is not None:
             result['Parameters'] = self.parameters_shrink
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.resource_group_id is not None:
@@ -1225,14 +1468,16 @@
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('ClientToken') is not None:
             self.client_token = m.get('ClientToken')
         if m.get('DryRun') is not None:
             self.dry_run = m.get('DryRun')
+        if m.get('EndTime') is not None:
+            self.end_time = m.get('EndTime')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('Parameters') is not None:
             self.parameters_shrink = m.get('Parameters')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('ResourceGroupId') is not None:
@@ -1302,17 +1547,14 @@
         body: CreateServiceInstanceResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1340,14 +1582,15 @@
 
 class DeleteArtifactRequest(TeaModel):
     def __init__(
         self,
         artifact_id: str = None,
         artifact_version: str = None,
     ):
+        # This parameter is required.
         self.artifact_id = artifact_id
         self.artifact_version = artifact_version
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -1406,17 +1649,14 @@
         body: DeleteArtifactResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1447,16 +1687,19 @@
         self,
         client_token: str = None,
         region_id: str = None,
         service_id: str = None,
         service_version: str = None,
     ):
         self.client_token = client_token
+        # This parameter is required.
         self.region_id = region_id
+        # This parameter is required.
         self.service_id = service_id
+        # This parameter is required.
         self.service_version = service_version
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1522,17 +1765,14 @@
         body: DeleteServiceResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1562,15 +1802,17 @@
     def __init__(
         self,
         client_token: str = None,
         region_id: str = None,
         service_instance_id: List[str] = None,
     ):
         self.client_token = client_token
+        # This parameter is required.
         self.region_id = region_id
+        # This parameter is required.
         self.service_instance_id = service_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1632,17 +1874,14 @@
         body: DeleteServiceInstancesResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1672,15 +1911,17 @@
     def __init__(
         self,
         client_token: str = None,
         region_id: str = None,
         service_instance_id: str = None,
     ):
         self.client_token = client_token
+        # This parameter is required.
         self.region_id = region_id
+        # This parameter is required.
         self.service_instance_id = service_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1742,17 +1983,14 @@
         body: DeployServiceInstanceResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1977,17 +2215,14 @@
         body: GetArtifactResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2015,14 +2250,15 @@
 
 class GetArtifactRepositoryCredentialsRequest(TeaModel):
     def __init__(
         self,
         artifact_type: str = None,
         deploy_region_id: str = None,
     ):
+        # This parameter is required.
         self.artifact_type = artifact_type
         self.deploy_region_id = deploy_region_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -2200,17 +2436,14 @@
         body: GetArtifactRepositoryCredentialsResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2244,14 +2477,15 @@
         service_id: str = None,
         service_version: str = None,
         shared_account_type: str = None,
         show_detail: List[str] = None,
     ):
         self.filter_ali_uid = filter_ali_uid
         self.region_id = region_id
+        # This parameter is required.
         self.service_id = service_id
         self.service_version = service_version
         self.shared_account_type = shared_account_type
         self.show_detail = show_detail
 
     def validate(self):
         pass
@@ -2289,130 +2523,645 @@
         if m.get('SharedAccountType') is not None:
             self.shared_account_type = m.get('SharedAccountType')
         if m.get('ShowDetail') is not None:
             self.show_detail = m.get('ShowDetail')
         return self
 
 
-class GetServiceResponseBodyCommodityEntities(TeaModel):
+class GetServiceResponseBodyCommodityCssMetadataComponentsMappings(TeaModel):
     def __init__(
         self,
-        entity_ids: List[str] = None,
-        predefined_parameter_name: str = None,
+        mappings: Dict[str, str] = None,
+        template_name: str = None,
+    ):
+        self.mappings = mappings
+        self.template_name = template_name
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
+        if self.mappings is not None:
+            result['Mappings'] = self.mappings
+        if self.template_name is not None:
+            result['TemplateName'] = self.template_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Mappings') is not None:
+            self.mappings = m.get('Mappings')
+        if m.get('TemplateName') is not None:
+            self.template_name = m.get('TemplateName')
+        return self
+
+
+class GetServiceResponseBodyCommodityCssMetadataMeteringEntityExtraInfos(TeaModel):
+    def __init__(
+        self,
+        entity_id: str = None,
+        metric_name: str = None,
+        promql: str = None,
+        type: str = None,
+    ):
+        self.entity_id = entity_id
+        self.metric_name = metric_name
+        self.promql = promql
+        self.type = type
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
+        if self.entity_id is not None:
+            result['EntityId'] = self.entity_id
+        if self.metric_name is not None:
+            result['MetricName'] = self.metric_name
+        if self.promql is not None:
+            result['Promql'] = self.promql
+        if self.type is not None:
+            result['Type'] = self.type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('EntityId') is not None:
+            self.entity_id = m.get('EntityId')
+        if m.get('MetricName') is not None:
+            self.metric_name = m.get('MetricName')
+        if m.get('Promql') is not None:
+            self.promql = m.get('Promql')
+        if m.get('Type') is not None:
+            self.type = m.get('Type')
+        return self
+
+
+class GetServiceResponseBodyCommodityCssMetadataMeteringEntityMappings(TeaModel):
+    def __init__(
+        self,
+        entity_ids: str = None,
+        specification_name: str = None,
         template_name: str = None,
     ):
         self.entity_ids = entity_ids
-        self.predefined_parameter_name = predefined_parameter_name
+        self.specification_name = specification_name
         self.template_name = template_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.entity_ids is not None:
             result['EntityIds'] = self.entity_ids
-        if self.predefined_parameter_name is not None:
-            result['PredefinedParameterName'] = self.predefined_parameter_name
+        if self.specification_name is not None:
+            result['SpecificationName'] = self.specification_name
         if self.template_name is not None:
             result['TemplateName'] = self.template_name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('EntityIds') is not None:
             self.entity_ids = m.get('EntityIds')
-        if m.get('PredefinedParameterName') is not None:
-            self.predefined_parameter_name = m.get('PredefinedParameterName')
+        if m.get('SpecificationName') is not None:
+            self.specification_name = m.get('SpecificationName')
         if m.get('TemplateName') is not None:
             self.template_name = m.get('TemplateName')
         return self
 
 
-class GetServiceResponseBodyCommoditySpecifications(TeaModel):
+class GetServiceResponseBodyCommodityCssMetadata(TeaModel):
+    def __init__(
+        self,
+        components_mappings: List[GetServiceResponseBodyCommodityCssMetadataComponentsMappings] = None,
+        metering_entity_extra_infos: List[GetServiceResponseBodyCommodityCssMetadataMeteringEntityExtraInfos] = None,
+        metering_entity_mappings: List[GetServiceResponseBodyCommodityCssMetadataMeteringEntityMappings] = None,
+    ):
+        self.components_mappings = components_mappings
+        self.metering_entity_extra_infos = metering_entity_extra_infos
+        self.metering_entity_mappings = metering_entity_mappings
+
+    def validate(self):
+        if self.components_mappings:
+            for k in self.components_mappings:
+                if k:
+                    k.validate()
+        if self.metering_entity_extra_infos:
+            for k in self.metering_entity_extra_infos:
+                if k:
+                    k.validate()
+        if self.metering_entity_mappings:
+            for k in self.metering_entity_mappings:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['ComponentsMappings'] = []
+        if self.components_mappings is not None:
+            for k in self.components_mappings:
+                result['ComponentsMappings'].append(k.to_map() if k else None)
+        result['MeteringEntityExtraInfos'] = []
+        if self.metering_entity_extra_infos is not None:
+            for k in self.metering_entity_extra_infos:
+                result['MeteringEntityExtraInfos'].append(k.to_map() if k else None)
+        result['MeteringEntityMappings'] = []
+        if self.metering_entity_mappings is not None:
+            for k in self.metering_entity_mappings:
+                result['MeteringEntityMappings'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.components_mappings = []
+        if m.get('ComponentsMappings') is not None:
+            for k in m.get('ComponentsMappings'):
+                temp_model = GetServiceResponseBodyCommodityCssMetadataComponentsMappings()
+                self.components_mappings.append(temp_model.from_map(k))
+        self.metering_entity_extra_infos = []
+        if m.get('MeteringEntityExtraInfos') is not None:
+            for k in m.get('MeteringEntityExtraInfos'):
+                temp_model = GetServiceResponseBodyCommodityCssMetadataMeteringEntityExtraInfos()
+                self.metering_entity_extra_infos.append(temp_model.from_map(k))
+        self.metering_entity_mappings = []
+        if m.get('MeteringEntityMappings') is not None:
+            for k in m.get('MeteringEntityMappings'):
+                temp_model = GetServiceResponseBodyCommodityCssMetadataMeteringEntityMappings()
+                self.metering_entity_mappings.append(temp_model.from_map(k))
+        return self
+
+
+class GetServiceResponseBodyCommodityMarketplaceMetadataMeteringEntityExtraInfos(TeaModel):
+    def __init__(
+        self,
+        entity_id: str = None,
+        metric_name: str = None,
+        promql: str = None,
+        type: str = None,
+    ):
+        self.entity_id = entity_id
+        self.metric_name = metric_name
+        self.promql = promql
+        self.type = type
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
+        if self.entity_id is not None:
+            result['EntityId'] = self.entity_id
+        if self.metric_name is not None:
+            result['MetricName'] = self.metric_name
+        if self.promql is not None:
+            result['Promql'] = self.promql
+        if self.type is not None:
+            result['Type'] = self.type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('EntityId') is not None:
+            self.entity_id = m.get('EntityId')
+        if m.get('MetricName') is not None:
+            self.metric_name = m.get('MetricName')
+        if m.get('Promql') is not None:
+            self.promql = m.get('Promql')
+        if m.get('Type') is not None:
+            self.type = m.get('Type')
+        return self
+
+
+class GetServiceResponseBodyCommodityMarketplaceMetadataMeteringEntityMappings(TeaModel):
+    def __init__(
+        self,
+        entity_ids: str = None,
+        specification_name: str = None,
+        template_name: str = None,
+    ):
+        self.entity_ids = entity_ids
+        self.specification_name = specification_name
+        self.template_name = template_name
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
+        if self.entity_ids is not None:
+            result['EntityIds'] = self.entity_ids
+        if self.specification_name is not None:
+            result['SpecificationName'] = self.specification_name
+        if self.template_name is not None:
+            result['TemplateName'] = self.template_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('EntityIds') is not None:
+            self.entity_ids = m.get('EntityIds')
+        if m.get('SpecificationName') is not None:
+            self.specification_name = m.get('SpecificationName')
+        if m.get('TemplateName') is not None:
+            self.template_name = m.get('TemplateName')
+        return self
+
+
+class GetServiceResponseBodyCommodityMarketplaceMetadataSpecificationMappings(TeaModel):
     def __init__(
         self,
-        predefined_parameter_name: str = None,
         specification_code: str = None,
+        specification_name: str = None,
         template_name: str = None,
+        trial_type: str = None,
     ):
-        self.predefined_parameter_name = predefined_parameter_name
         self.specification_code = specification_code
+        self.specification_name = specification_name
         self.template_name = template_name
+        self.trial_type = trial_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.predefined_parameter_name is not None:
-            result['PredefinedParameterName'] = self.predefined_parameter_name
         if self.specification_code is not None:
             result['SpecificationCode'] = self.specification_code
+        if self.specification_name is not None:
+            result['SpecificationName'] = self.specification_name
         if self.template_name is not None:
             result['TemplateName'] = self.template_name
+        if self.trial_type is not None:
+            result['TrialType'] = self.trial_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('PredefinedParameterName') is not None:
-            self.predefined_parameter_name = m.get('PredefinedParameterName')
         if m.get('SpecificationCode') is not None:
             self.specification_code = m.get('SpecificationCode')
+        if m.get('SpecificationName') is not None:
+            self.specification_name = m.get('SpecificationName')
         if m.get('TemplateName') is not None:
             self.template_name = m.get('TemplateName')
+        if m.get('TrialType') is not None:
+            self.trial_type = m.get('TrialType')
+        return self
+
+
+class GetServiceResponseBodyCommodityMarketplaceMetadata(TeaModel):
+    def __init__(
+        self,
+        metering_entity_extra_infos: List[GetServiceResponseBodyCommodityMarketplaceMetadataMeteringEntityExtraInfos] = None,
+        metering_entity_mappings: List[GetServiceResponseBodyCommodityMarketplaceMetadataMeteringEntityMappings] = None,
+        specification_mappings: List[GetServiceResponseBodyCommodityMarketplaceMetadataSpecificationMappings] = None,
+    ):
+        self.metering_entity_extra_infos = metering_entity_extra_infos
+        self.metering_entity_mappings = metering_entity_mappings
+        self.specification_mappings = specification_mappings
+
+    def validate(self):
+        if self.metering_entity_extra_infos:
+            for k in self.metering_entity_extra_infos:
+                if k:
+                    k.validate()
+        if self.metering_entity_mappings:
+            for k in self.metering_entity_mappings:
+                if k:
+                    k.validate()
+        if self.specification_mappings:
+            for k in self.specification_mappings:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['MeteringEntityExtraInfos'] = []
+        if self.metering_entity_extra_infos is not None:
+            for k in self.metering_entity_extra_infos:
+                result['MeteringEntityExtraInfos'].append(k.to_map() if k else None)
+        result['MeteringEntityMappings'] = []
+        if self.metering_entity_mappings is not None:
+            for k in self.metering_entity_mappings:
+                result['MeteringEntityMappings'].append(k.to_map() if k else None)
+        result['SpecificationMappings'] = []
+        if self.specification_mappings is not None:
+            for k in self.specification_mappings:
+                result['SpecificationMappings'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.metering_entity_extra_infos = []
+        if m.get('MeteringEntityExtraInfos') is not None:
+            for k in m.get('MeteringEntityExtraInfos'):
+                temp_model = GetServiceResponseBodyCommodityMarketplaceMetadataMeteringEntityExtraInfos()
+                self.metering_entity_extra_infos.append(temp_model.from_map(k))
+        self.metering_entity_mappings = []
+        if m.get('MeteringEntityMappings') is not None:
+            for k in m.get('MeteringEntityMappings'):
+                temp_model = GetServiceResponseBodyCommodityMarketplaceMetadataMeteringEntityMappings()
+                self.metering_entity_mappings.append(temp_model.from_map(k))
+        self.specification_mappings = []
+        if m.get('SpecificationMappings') is not None:
+            for k in m.get('SpecificationMappings'):
+                temp_model = GetServiceResponseBodyCommodityMarketplaceMetadataSpecificationMappings()
+                self.specification_mappings.append(temp_model.from_map(k))
+        return self
+
+
+class GetServiceResponseBodyCommodityMeteringEntities(TeaModel):
+    def __init__(
+        self,
+        entity_id: str = None,
+        name: str = None,
+    ):
+        self.entity_id = entity_id
+        self.name = name
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
+        if self.entity_id is not None:
+            result['EntityId'] = self.entity_id
+        if self.name is not None:
+            result['Name'] = self.name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('EntityId') is not None:
+            self.entity_id = m.get('EntityId')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        return self
+
+
+class GetServiceResponseBodyCommoditySpecifications(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        name: str = None,
+        times: List[str] = None,
+    ):
+        self.code = code
+        self.name = name
+        self.times = times
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
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.times is not None:
+            result['Times'] = self.times
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('Times') is not None:
+            self.times = m.get('Times')
+        return self
+
+
+class GetServiceResponseBodyCommodity(TeaModel):
+    def __init__(
+        self,
+        charge_type: str = None,
+        commodity_code: str = None,
+        components: List[str] = None,
+        css_metadata: GetServiceResponseBodyCommodityCssMetadata = None,
+        marketplace_metadata: GetServiceResponseBodyCommodityMarketplaceMetadata = None,
+        metering_entities: List[GetServiceResponseBodyCommodityMeteringEntities] = None,
+        saas_boost_metadata: str = None,
+        specifications: List[GetServiceResponseBodyCommoditySpecifications] = None,
+        type: str = None,
+    ):
+        self.charge_type = charge_type
+        self.commodity_code = commodity_code
+        self.components = components
+        self.css_metadata = css_metadata
+        self.marketplace_metadata = marketplace_metadata
+        self.metering_entities = metering_entities
+        self.saas_boost_metadata = saas_boost_metadata
+        self.specifications = specifications
+        self.type = type
+
+    def validate(self):
+        if self.css_metadata:
+            self.css_metadata.validate()
+        if self.marketplace_metadata:
+            self.marketplace_metadata.validate()
+        if self.metering_entities:
+            for k in self.metering_entities:
+                if k:
+                    k.validate()
+        if self.specifications:
+            for k in self.specifications:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.charge_type is not None:
+            result['ChargeType'] = self.charge_type
+        if self.commodity_code is not None:
+            result['CommodityCode'] = self.commodity_code
+        if self.components is not None:
+            result['Components'] = self.components
+        if self.css_metadata is not None:
+            result['CssMetadata'] = self.css_metadata.to_map()
+        if self.marketplace_metadata is not None:
+            result['MarketplaceMetadata'] = self.marketplace_metadata.to_map()
+        result['MeteringEntities'] = []
+        if self.metering_entities is not None:
+            for k in self.metering_entities:
+                result['MeteringEntities'].append(k.to_map() if k else None)
+        if self.saas_boost_metadata is not None:
+            result['SaasBoostMetadata'] = self.saas_boost_metadata
+        result['Specifications'] = []
+        if self.specifications is not None:
+            for k in self.specifications:
+                result['Specifications'].append(k.to_map() if k else None)
+        if self.type is not None:
+            result['Type'] = self.type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ChargeType') is not None:
+            self.charge_type = m.get('ChargeType')
+        if m.get('CommodityCode') is not None:
+            self.commodity_code = m.get('CommodityCode')
+        if m.get('Components') is not None:
+            self.components = m.get('Components')
+        if m.get('CssMetadata') is not None:
+            temp_model = GetServiceResponseBodyCommodityCssMetadata()
+            self.css_metadata = temp_model.from_map(m['CssMetadata'])
+        if m.get('MarketplaceMetadata') is not None:
+            temp_model = GetServiceResponseBodyCommodityMarketplaceMetadata()
+            self.marketplace_metadata = temp_model.from_map(m['MarketplaceMetadata'])
+        self.metering_entities = []
+        if m.get('MeteringEntities') is not None:
+            for k in m.get('MeteringEntities'):
+                temp_model = GetServiceResponseBodyCommodityMeteringEntities()
+                self.metering_entities.append(temp_model.from_map(k))
+        if m.get('SaasBoostMetadata') is not None:
+            self.saas_boost_metadata = m.get('SaasBoostMetadata')
+        self.specifications = []
+        if m.get('Specifications') is not None:
+            for k in m.get('Specifications'):
+                temp_model = GetServiceResponseBodyCommoditySpecifications()
+                self.specifications.append(temp_model.from_map(k))
+        if m.get('Type') is not None:
+            self.type = m.get('Type')
+        return self
+
+
+class GetServiceResponseBodyServiceInfosAgreements(TeaModel):
+    def __init__(
+        self,
+        name: str = None,
+        url: str = None,
+    ):
+        self.name = name
+        self.url = url
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
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.url is not None:
+            result['Url'] = self.url
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('Url') is not None:
+            self.url = m.get('Url')
         return self
 
 
 class GetServiceResponseBodyServiceInfos(TeaModel):
     def __init__(
         self,
+        agreements: List[GetServiceResponseBodyServiceInfosAgreements] = None,
         image: str = None,
         locale: str = None,
         long_description_url: str = None,
         name: str = None,
         short_description: str = None,
     ):
+        self.agreements = agreements
         self.image = image
         self.locale = locale
         self.long_description_url = long_description_url
         self.name = name
         self.short_description = short_description
 
     def validate(self):
-        pass
+        if self.agreements:
+            for k in self.agreements:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        result['Agreements'] = []
+        if self.agreements is not None:
+            for k in self.agreements:
+                result['Agreements'].append(k.to_map() if k else None)
         if self.image is not None:
             result['Image'] = self.image
         if self.locale is not None:
             result['Locale'] = self.locale
         if self.long_description_url is not None:
             result['LongDescriptionUrl'] = self.long_description_url
         if self.name is not None:
             result['Name'] = self.name
         if self.short_description is not None:
             result['ShortDescription'] = self.short_description
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        self.agreements = []
+        if m.get('Agreements') is not None:
+            for k in m.get('Agreements'):
+                temp_model = GetServiceResponseBodyServiceInfosAgreements()
+                self.agreements.append(temp_model.from_map(k))
         if m.get('Image') is not None:
             self.image = m.get('Image')
         if m.get('Locale') is not None:
             self.locale = m.get('Locale')
         if m.get('LongDescriptionUrl') is not None:
             self.long_description_url = m.get('LongDescriptionUrl')
         if m.get('Name') is not None:
@@ -2531,41 +3280,48 @@
 
 
 class GetServiceResponseBody(TeaModel):
     def __init__(
         self,
         alarm_metadata: str = None,
         approval_type: str = None,
+        build_info: str = None,
+        categories: str = None,
+        commodity: GetServiceResponseBodyCommodity = None,
         commodity_code: str = None,
-        commodity_entities: List[GetServiceResponseBodyCommodityEntities] = None,
-        commodity_specifications: List[GetServiceResponseBodyCommoditySpecifications] = None,
         create_time: str = None,
+        cross_region_connection_status: str = None,
         default_license_days: int = None,
         deploy_metadata: str = None,
         deploy_type: str = None,
         duration: int = None,
+        entity_source: Dict[str, str] = None,
         is_support_operated: bool = None,
         license_metadata: str = None,
         log_metadata: str = None,
         operation_metadata: str = None,
         pay_from_type: str = None,
         pay_type: str = None,
         permission: str = None,
         policy_names: str = None,
         progress: int = None,
         publish_time: str = None,
         registration_id: str = None,
         request_id: str = None,
+        resellable: bool = None,
         resource_group_id: str = None,
+        service_audit_document_url: str = None,
+        service_discoverable: str = None,
         service_doc_url: str = None,
         service_id: str = None,
         service_infos: List[GetServiceResponseBodyServiceInfos] = None,
         service_product_url: str = None,
         service_type: str = None,
         share_type: str = None,
+        share_type_status: str = None,
         source_service_id: str = None,
         source_service_version: str = None,
         source_supplier_name: str = None,
         statistic: GetServiceResponseBodyStatistic = None,
         status: str = None,
         status_detail: str = None,
         supplier_name: str = None,
@@ -2575,44 +3331,53 @@
         test_status: str = None,
         trial_duration: int = None,
         trial_type: str = None,
         update_time: str = None,
         upgrade_metadata: str = None,
         version: str = None,
         version_name: str = None,
+        virtual_internet_service: str = None,
+        virtual_internet_service_id: str = None,
     ):
         self.alarm_metadata = alarm_metadata
         self.approval_type = approval_type
+        self.build_info = build_info
+        self.categories = categories
+        self.commodity = commodity
         self.commodity_code = commodity_code
-        self.commodity_entities = commodity_entities
-        self.commodity_specifications = commodity_specifications
         self.create_time = create_time
+        self.cross_region_connection_status = cross_region_connection_status
         self.default_license_days = default_license_days
         self.deploy_metadata = deploy_metadata
         self.deploy_type = deploy_type
         self.duration = duration
+        self.entity_source = entity_source
         self.is_support_operated = is_support_operated
         self.license_metadata = license_metadata
         self.log_metadata = log_metadata
         self.operation_metadata = operation_metadata
         self.pay_from_type = pay_from_type
         self.pay_type = pay_type
         self.permission = permission
         self.policy_names = policy_names
         self.progress = progress
         self.publish_time = publish_time
         self.registration_id = registration_id
         self.request_id = request_id
+        self.resellable = resellable
         self.resource_group_id = resource_group_id
+        self.service_audit_document_url = service_audit_document_url
+        self.service_discoverable = service_discoverable
         self.service_doc_url = service_doc_url
         self.service_id = service_id
         self.service_infos = service_infos
         self.service_product_url = service_product_url
         self.service_type = service_type
         self.share_type = share_type
+        self.share_type_status = share_type_status
         self.source_service_id = source_service_id
         self.source_service_version = source_service_version
         self.source_supplier_name = source_supplier_name
         self.statistic = statistic
         self.status = status
         self.status_detail = status_detail
         self.supplier_name = supplier_name
@@ -2622,24 +3387,20 @@
         self.test_status = test_status
         self.trial_duration = trial_duration
         self.trial_type = trial_type
         self.update_time = update_time
         self.upgrade_metadata = upgrade_metadata
         self.version = version
         self.version_name = version_name
+        self.virtual_internet_service = virtual_internet_service
+        self.virtual_internet_service_id = virtual_internet_service_id
 
     def validate(self):
-        if self.commodity_entities:
-            for k in self.commodity_entities:
-                if k:
-                    k.validate()
-        if self.commodity_specifications:
-            for k in self.commodity_specifications:
-                if k:
-                    k.validate()
+        if self.commodity:
+            self.commodity.validate()
         if self.service_infos:
             for k in self.service_infos:
                 if k:
                     k.validate()
         if self.statistic:
             self.statistic.validate()
         if self.tags:
@@ -2653,34 +3414,36 @@
             return _map
 
         result = dict()
         if self.alarm_metadata is not None:
             result['AlarmMetadata'] = self.alarm_metadata
         if self.approval_type is not None:
             result['ApprovalType'] = self.approval_type
+        if self.build_info is not None:
+            result['BuildInfo'] = self.build_info
+        if self.categories is not None:
+            result['Categories'] = self.categories
+        if self.commodity is not None:
+            result['Commodity'] = self.commodity.to_map()
         if self.commodity_code is not None:
             result['CommodityCode'] = self.commodity_code
-        result['CommodityEntities'] = []
-        if self.commodity_entities is not None:
-            for k in self.commodity_entities:
-                result['CommodityEntities'].append(k.to_map() if k else None)
-        result['CommoditySpecifications'] = []
-        if self.commodity_specifications is not None:
-            for k in self.commodity_specifications:
-                result['CommoditySpecifications'].append(k.to_map() if k else None)
         if self.create_time is not None:
             result['CreateTime'] = self.create_time
+        if self.cross_region_connection_status is not None:
+            result['CrossRegionConnectionStatus'] = self.cross_region_connection_status
         if self.default_license_days is not None:
             result['DefaultLicenseDays'] = self.default_license_days
         if self.deploy_metadata is not None:
             result['DeployMetadata'] = self.deploy_metadata
         if self.deploy_type is not None:
             result['DeployType'] = self.deploy_type
         if self.duration is not None:
             result['Duration'] = self.duration
+        if self.entity_source is not None:
+            result['EntitySource'] = self.entity_source
         if self.is_support_operated is not None:
             result['IsSupportOperated'] = self.is_support_operated
         if self.license_metadata is not None:
             result['LicenseMetadata'] = self.license_metadata
         if self.log_metadata is not None:
             result['LogMetadata'] = self.log_metadata
         if self.operation_metadata is not None:
@@ -2697,30 +3460,38 @@
             result['Progress'] = self.progress
         if self.publish_time is not None:
             result['PublishTime'] = self.publish_time
         if self.registration_id is not None:
             result['RegistrationId'] = self.registration_id
         if self.request_id is not None:
             result['RequestId'] = self.request_id
+        if self.resellable is not None:
+            result['Resellable'] = self.resellable
         if self.resource_group_id is not None:
             result['ResourceGroupId'] = self.resource_group_id
+        if self.service_audit_document_url is not None:
+            result['ServiceAuditDocumentUrl'] = self.service_audit_document_url
+        if self.service_discoverable is not None:
+            result['ServiceDiscoverable'] = self.service_discoverable
         if self.service_doc_url is not None:
             result['ServiceDocUrl'] = self.service_doc_url
         if self.service_id is not None:
             result['ServiceId'] = self.service_id
         result['ServiceInfos'] = []
         if self.service_infos is not None:
             for k in self.service_infos:
                 result['ServiceInfos'].append(k.to_map() if k else None)
         if self.service_product_url is not None:
             result['ServiceProductUrl'] = self.service_product_url
         if self.service_type is not None:
             result['ServiceType'] = self.service_type
         if self.share_type is not None:
             result['ShareType'] = self.share_type
+        if self.share_type_status is not None:
+            result['ShareTypeStatus'] = self.share_type_status
         if self.source_service_id is not None:
             result['SourceServiceId'] = self.source_service_id
         if self.source_service_version is not None:
             result['SourceServiceVersion'] = self.source_service_version
         if self.source_supplier_name is not None:
             result['SourceSupplierName'] = self.source_supplier_name
         if self.statistic is not None:
@@ -2749,44 +3520,49 @@
             result['UpdateTime'] = self.update_time
         if self.upgrade_metadata is not None:
             result['UpgradeMetadata'] = self.upgrade_metadata
         if self.version is not None:
             result['Version'] = self.version
         if self.version_name is not None:
             result['VersionName'] = self.version_name
+        if self.virtual_internet_service is not None:
+            result['VirtualInternetService'] = self.virtual_internet_service
+        if self.virtual_internet_service_id is not None:
+            result['VirtualInternetServiceId'] = self.virtual_internet_service_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AlarmMetadata') is not None:
             self.alarm_metadata = m.get('AlarmMetadata')
         if m.get('ApprovalType') is not None:
             self.approval_type = m.get('ApprovalType')
+        if m.get('BuildInfo') is not None:
+            self.build_info = m.get('BuildInfo')
+        if m.get('Categories') is not None:
+            self.categories = m.get('Categories')
+        if m.get('Commodity') is not None:
+            temp_model = GetServiceResponseBodyCommodity()
+            self.commodity = temp_model.from_map(m['Commodity'])
         if m.get('CommodityCode') is not None:
             self.commodity_code = m.get('CommodityCode')
-        self.commodity_entities = []
-        if m.get('CommodityEntities') is not None:
-            for k in m.get('CommodityEntities'):
-                temp_model = GetServiceResponseBodyCommodityEntities()
-                self.commodity_entities.append(temp_model.from_map(k))
-        self.commodity_specifications = []
-        if m.get('CommoditySpecifications') is not None:
-            for k in m.get('CommoditySpecifications'):
-                temp_model = GetServiceResponseBodyCommoditySpecifications()
-                self.commodity_specifications.append(temp_model.from_map(k))
         if m.get('CreateTime') is not None:
             self.create_time = m.get('CreateTime')
+        if m.get('CrossRegionConnectionStatus') is not None:
+            self.cross_region_connection_status = m.get('CrossRegionConnectionStatus')
         if m.get('DefaultLicenseDays') is not None:
             self.default_license_days = m.get('DefaultLicenseDays')
         if m.get('DeployMetadata') is not None:
             self.deploy_metadata = m.get('DeployMetadata')
         if m.get('DeployType') is not None:
             self.deploy_type = m.get('DeployType')
         if m.get('Duration') is not None:
             self.duration = m.get('Duration')
+        if m.get('EntitySource') is not None:
+            self.entity_source = m.get('EntitySource')
         if m.get('IsSupportOperated') is not None:
             self.is_support_operated = m.get('IsSupportOperated')
         if m.get('LicenseMetadata') is not None:
             self.license_metadata = m.get('LicenseMetadata')
         if m.get('LogMetadata') is not None:
             self.log_metadata = m.get('LogMetadata')
         if m.get('OperationMetadata') is not None:
@@ -2803,16 +3579,22 @@
             self.progress = m.get('Progress')
         if m.get('PublishTime') is not None:
             self.publish_time = m.get('PublishTime')
         if m.get('RegistrationId') is not None:
             self.registration_id = m.get('RegistrationId')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
+        if m.get('Resellable') is not None:
+            self.resellable = m.get('Resellable')
         if m.get('ResourceGroupId') is not None:
             self.resource_group_id = m.get('ResourceGroupId')
+        if m.get('ServiceAuditDocumentUrl') is not None:
+            self.service_audit_document_url = m.get('ServiceAuditDocumentUrl')
+        if m.get('ServiceDiscoverable') is not None:
+            self.service_discoverable = m.get('ServiceDiscoverable')
         if m.get('ServiceDocUrl') is not None:
             self.service_doc_url = m.get('ServiceDocUrl')
         if m.get('ServiceId') is not None:
             self.service_id = m.get('ServiceId')
         self.service_infos = []
         if m.get('ServiceInfos') is not None:
             for k in m.get('ServiceInfos'):
@@ -2820,14 +3602,16 @@
                 self.service_infos.append(temp_model.from_map(k))
         if m.get('ServiceProductUrl') is not None:
             self.service_product_url = m.get('ServiceProductUrl')
         if m.get('ServiceType') is not None:
             self.service_type = m.get('ServiceType')
         if m.get('ShareType') is not None:
             self.share_type = m.get('ShareType')
+        if m.get('ShareTypeStatus') is not None:
+            self.share_type_status = m.get('ShareTypeStatus')
         if m.get('SourceServiceId') is not None:
             self.source_service_id = m.get('SourceServiceId')
         if m.get('SourceServiceVersion') is not None:
             self.source_service_version = m.get('SourceServiceVersion')
         if m.get('SourceSupplierName') is not None:
             self.source_supplier_name = m.get('SourceSupplierName')
         if m.get('Statistic') is not None:
@@ -2858,14 +3642,18 @@
             self.update_time = m.get('UpdateTime')
         if m.get('UpgradeMetadata') is not None:
             self.upgrade_metadata = m.get('UpgradeMetadata')
         if m.get('Version') is not None:
             self.version = m.get('Version')
         if m.get('VersionName') is not None:
             self.version_name = m.get('VersionName')
+        if m.get('VirtualInternetService') is not None:
+            self.virtual_internet_service = m.get('VirtualInternetService')
+        if m.get('VirtualInternetServiceId') is not None:
+            self.virtual_internet_service_id = m.get('VirtualInternetServiceId')
         return self
 
 
 class GetServiceResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -2873,17 +3661,14 @@
         body: GetServiceResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2905,46 +3690,85 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetServiceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetServiceEstimateCostRequestCommodity(TeaModel):
+    def __init__(
+        self,
+        pay_period: int = None,
+        pay_period_unit: str = None,
+    ):
+        self.pay_period = pay_period
+        self.pay_period_unit = pay_period_unit
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
+        if self.pay_period is not None:
+            result['PayPeriod'] = self.pay_period
+        if self.pay_period_unit is not None:
+            result['PayPeriodUnit'] = self.pay_period_unit
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('PayPeriod') is not None:
+            self.pay_period = m.get('PayPeriod')
+        if m.get('PayPeriodUnit') is not None:
+            self.pay_period_unit = m.get('PayPeriodUnit')
+        return self
+
+
 class GetServiceEstimateCostRequest(TeaModel):
     def __init__(
         self,
         client_token: str = None,
+        commodity: GetServiceEstimateCostRequestCommodity = None,
         parameters: Dict[str, Any] = None,
         region_id: str = None,
         service_id: str = None,
         service_instance_id: str = None,
         service_version: str = None,
         specification_name: str = None,
         template_name: str = None,
     ):
         self.client_token = client_token
+        self.commodity = commodity
         self.parameters = parameters
         self.region_id = region_id
+        # This parameter is required.
         self.service_id = service_id
         self.service_instance_id = service_instance_id
         self.service_version = service_version
         self.specification_name = specification_name
         self.template_name = template_name
 
     def validate(self):
-        pass
+        if self.commodity:
+            self.commodity.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.client_token is not None:
             result['ClientToken'] = self.client_token
+        if self.commodity is not None:
+            result['Commodity'] = self.commodity.to_map()
         if self.parameters is not None:
             result['Parameters'] = self.parameters
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.service_id is not None:
             result['ServiceId'] = self.service_id
         if self.service_instance_id is not None:
@@ -2957,14 +3781,17 @@
             result['TemplateName'] = self.template_name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('ClientToken') is not None:
             self.client_token = m.get('ClientToken')
+        if m.get('Commodity') is not None:
+            temp_model = GetServiceEstimateCostRequestCommodity()
+            self.commodity = temp_model.from_map(m['Commodity'])
         if m.get('Parameters') is not None:
             self.parameters = m.get('Parameters')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('ServiceId') is not None:
             self.service_id = m.get('ServiceId')
         if m.get('ServiceInstanceId') is not None:
@@ -2978,25 +3805,28 @@
         return self
 
 
 class GetServiceEstimateCostShrinkRequest(TeaModel):
     def __init__(
         self,
         client_token: str = None,
+        commodity_shrink: str = None,
         parameters_shrink: str = None,
         region_id: str = None,
         service_id: str = None,
         service_instance_id: str = None,
         service_version: str = None,
         specification_name: str = None,
         template_name: str = None,
     ):
         self.client_token = client_token
+        self.commodity_shrink = commodity_shrink
         self.parameters_shrink = parameters_shrink
         self.region_id = region_id
+        # This parameter is required.
         self.service_id = service_id
         self.service_instance_id = service_instance_id
         self.service_version = service_version
         self.specification_name = specification_name
         self.template_name = template_name
 
     def validate(self):
@@ -3006,14 +3836,16 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.client_token is not None:
             result['ClientToken'] = self.client_token
+        if self.commodity_shrink is not None:
+            result['Commodity'] = self.commodity_shrink
         if self.parameters_shrink is not None:
             result['Parameters'] = self.parameters_shrink
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.service_id is not None:
             result['ServiceId'] = self.service_id
         if self.service_instance_id is not None:
@@ -3026,14 +3858,16 @@
             result['TemplateName'] = self.template_name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('ClientToken') is not None:
             self.client_token = m.get('ClientToken')
+        if m.get('Commodity') is not None:
+            self.commodity_shrink = m.get('Commodity')
         if m.get('Parameters') is not None:
             self.parameters_shrink = m.get('Parameters')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('ServiceId') is not None:
             self.service_id = m.get('ServiceId')
         if m.get('ServiceInstanceId') is not None:
@@ -3046,37 +3880,43 @@
             self.template_name = m.get('TemplateName')
         return self
 
 
 class GetServiceEstimateCostResponseBody(TeaModel):
     def __init__(
         self,
+        commodity: Dict[str, Any] = None,
         request_id: str = None,
         resources: Dict[str, Any] = None,
     ):
+        self.commodity = commodity
         self.request_id = request_id
         self.resources = resources
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.commodity is not None:
+            result['Commodity'] = self.commodity
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.resources is not None:
             result['Resources'] = self.resources
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('Commodity') is not None:
+            self.commodity = m.get('Commodity')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         if m.get('Resources') is not None:
             self.resources = m.get('Resources')
         return self
 
 
@@ -3088,17 +3928,14 @@
         body: GetServiceEstimateCostResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -3126,15 +3963,17 @@
 
 class GetServiceInstanceRequest(TeaModel):
     def __init__(
         self,
         region_id: str = None,
         service_instance_id: str = None,
     ):
+        # This parameter is required.
         self.region_id = region_id
+        # This parameter is required.
         self.service_instance_id = service_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3567,16 +4406,17 @@
 
 class GetServiceInstanceResponseBody(TeaModel):
     def __init__(
         self,
         biz_status: str = None,
         create_time: str = None,
         enable_instance_ops: bool = None,
-        enable_user_prometheus: str = None,
+        enable_user_prometheus: bool = None,
         end_time: str = None,
+        grafana_dash_board_url: str = None,
         is_operated: bool = None,
         license_metadata: str = None,
         name: str = None,
         network_config: GetServiceInstanceResponseBodyNetworkConfig = None,
         operated_service_instance_id: str = None,
         operation_end_time: str = None,
         operation_start_time: str = None,
@@ -3602,14 +4442,15 @@
         user_id: int = None,
     ):
         self.biz_status = biz_status
         self.create_time = create_time
         self.enable_instance_ops = enable_instance_ops
         self.enable_user_prometheus = enable_user_prometheus
         self.end_time = end_time
+        self.grafana_dash_board_url = grafana_dash_board_url
         self.is_operated = is_operated
         self.license_metadata = license_metadata
         self.name = name
         self.network_config = network_config
         self.operated_service_instance_id = operated_service_instance_id
         self.operation_end_time = operation_end_time
         self.operation_start_time = operation_start_time
@@ -3656,14 +4497,16 @@
             result['CreateTime'] = self.create_time
         if self.enable_instance_ops is not None:
             result['EnableInstanceOps'] = self.enable_instance_ops
         if self.enable_user_prometheus is not None:
             result['EnableUserPrometheus'] = self.enable_user_prometheus
         if self.end_time is not None:
             result['EndTime'] = self.end_time
+        if self.grafana_dash_board_url is not None:
+            result['GrafanaDashBoardUrl'] = self.grafana_dash_board_url
         if self.is_operated is not None:
             result['IsOperated'] = self.is_operated
         if self.license_metadata is not None:
             result['LicenseMetadata'] = self.license_metadata
         if self.name is not None:
             result['Name'] = self.name
         if self.network_config is not None:
@@ -3726,14 +4569,16 @@
             self.create_time = m.get('CreateTime')
         if m.get('EnableInstanceOps') is not None:
             self.enable_instance_ops = m.get('EnableInstanceOps')
         if m.get('EnableUserPrometheus') is not None:
             self.enable_user_prometheus = m.get('EnableUserPrometheus')
         if m.get('EndTime') is not None:
             self.end_time = m.get('EndTime')
+        if m.get('GrafanaDashBoardUrl') is not None:
+            self.grafana_dash_board_url = m.get('GrafanaDashBoardUrl')
         if m.get('IsOperated') is not None:
             self.is_operated = m.get('IsOperated')
         if m.get('LicenseMetadata') is not None:
             self.license_metadata = m.get('LicenseMetadata')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('NetworkConfig') is not None:
@@ -3800,17 +4645,14 @@
         body: GetServiceInstanceResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -3832,19 +4674,344 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetServiceInstanceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetServiceTemplateParameterConstraintsRequestParameters(TeaModel):
+    def __init__(
+        self,
+        parameter_key: str = None,
+        parameter_value: str = None,
+    ):
+        self.parameter_key = parameter_key
+        self.parameter_value = parameter_value
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
+        if self.parameter_key is not None:
+            result['ParameterKey'] = self.parameter_key
+        if self.parameter_value is not None:
+            result['ParameterValue'] = self.parameter_value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ParameterKey') is not None:
+            self.parameter_key = m.get('ParameterKey')
+        if m.get('ParameterValue') is not None:
+            self.parameter_value = m.get('ParameterValue')
+        return self
+
+
+class GetServiceTemplateParameterConstraintsRequest(TeaModel):
+    def __init__(
+        self,
+        client_token: str = None,
+        deploy_region_id: str = None,
+        enable_private_vpc_connection: bool = None,
+        parameters: List[GetServiceTemplateParameterConstraintsRequestParameters] = None,
+        region_id: str = None,
+        service_id: str = None,
+        service_instance_id: str = None,
+        service_version: str = None,
+        template_name: str = None,
+    ):
+        self.client_token = client_token
+        # This parameter is required.
+        self.deploy_region_id = deploy_region_id
+        self.enable_private_vpc_connection = enable_private_vpc_connection
+        self.parameters = parameters
+        # This parameter is required.
+        self.region_id = region_id
+        # This parameter is required.
+        self.service_id = service_id
+        self.service_instance_id = service_instance_id
+        self.service_version = service_version
+        # This parameter is required.
+        self.template_name = template_name
+
+    def validate(self):
+        if self.parameters:
+            for k in self.parameters:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.client_token is not None:
+            result['ClientToken'] = self.client_token
+        if self.deploy_region_id is not None:
+            result['DeployRegionId'] = self.deploy_region_id
+        if self.enable_private_vpc_connection is not None:
+            result['EnablePrivateVpcConnection'] = self.enable_private_vpc_connection
+        result['Parameters'] = []
+        if self.parameters is not None:
+            for k in self.parameters:
+                result['Parameters'].append(k.to_map() if k else None)
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.service_id is not None:
+            result['ServiceId'] = self.service_id
+        if self.service_instance_id is not None:
+            result['ServiceInstanceId'] = self.service_instance_id
+        if self.service_version is not None:
+            result['ServiceVersion'] = self.service_version
+        if self.template_name is not None:
+            result['TemplateName'] = self.template_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ClientToken') is not None:
+            self.client_token = m.get('ClientToken')
+        if m.get('DeployRegionId') is not None:
+            self.deploy_region_id = m.get('DeployRegionId')
+        if m.get('EnablePrivateVpcConnection') is not None:
+            self.enable_private_vpc_connection = m.get('EnablePrivateVpcConnection')
+        self.parameters = []
+        if m.get('Parameters') is not None:
+            for k in m.get('Parameters'):
+                temp_model = GetServiceTemplateParameterConstraintsRequestParameters()
+                self.parameters.append(temp_model.from_map(k))
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ServiceId') is not None:
+            self.service_id = m.get('ServiceId')
+        if m.get('ServiceInstanceId') is not None:
+            self.service_instance_id = m.get('ServiceInstanceId')
+        if m.get('ServiceVersion') is not None:
+            self.service_version = m.get('ServiceVersion')
+        if m.get('TemplateName') is not None:
+            self.template_name = m.get('TemplateName')
+        return self
+
+
+class GetServiceTemplateParameterConstraintsResponseBodyParameterConstraintsOriginalConstraints(TeaModel):
+    def __init__(
+        self,
+        allowed_values: List[str] = None,
+        property_name: str = None,
+        resource_name: str = None,
+        resource_type: str = None,
+    ):
+        self.allowed_values = allowed_values
+        self.property_name = property_name
+        self.resource_name = resource_name
+        self.resource_type = resource_type
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
+        if self.allowed_values is not None:
+            result['AllowedValues'] = self.allowed_values
+        if self.property_name is not None:
+            result['PropertyName'] = self.property_name
+        if self.resource_name is not None:
+            result['ResourceName'] = self.resource_name
+        if self.resource_type is not None:
+            result['ResourceType'] = self.resource_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AllowedValues') is not None:
+            self.allowed_values = m.get('AllowedValues')
+        if m.get('PropertyName') is not None:
+            self.property_name = m.get('PropertyName')
+        if m.get('ResourceName') is not None:
+            self.resource_name = m.get('ResourceName')
+        if m.get('ResourceType') is not None:
+            self.resource_type = m.get('ResourceType')
+        return self
+
+
+class GetServiceTemplateParameterConstraintsResponseBodyParameterConstraints(TeaModel):
+    def __init__(
+        self,
+        allowed_values: List[str] = None,
+        association_parameter_names: List[str] = None,
+        behavior: str = None,
+        behavior_reason: str = None,
+        original_constraints: List[GetServiceTemplateParameterConstraintsResponseBodyParameterConstraintsOriginalConstraints] = None,
+        parameter_key: str = None,
+        type: str = None,
+    ):
+        self.allowed_values = allowed_values
+        self.association_parameter_names = association_parameter_names
+        self.behavior = behavior
+        self.behavior_reason = behavior_reason
+        self.original_constraints = original_constraints
+        self.parameter_key = parameter_key
+        self.type = type
+
+    def validate(self):
+        if self.original_constraints:
+            for k in self.original_constraints:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.allowed_values is not None:
+            result['AllowedValues'] = self.allowed_values
+        if self.association_parameter_names is not None:
+            result['AssociationParameterNames'] = self.association_parameter_names
+        if self.behavior is not None:
+            result['Behavior'] = self.behavior
+        if self.behavior_reason is not None:
+            result['BehaviorReason'] = self.behavior_reason
+        result['OriginalConstraints'] = []
+        if self.original_constraints is not None:
+            for k in self.original_constraints:
+                result['OriginalConstraints'].append(k.to_map() if k else None)
+        if self.parameter_key is not None:
+            result['ParameterKey'] = self.parameter_key
+        if self.type is not None:
+            result['Type'] = self.type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AllowedValues') is not None:
+            self.allowed_values = m.get('AllowedValues')
+        if m.get('AssociationParameterNames') is not None:
+            self.association_parameter_names = m.get('AssociationParameterNames')
+        if m.get('Behavior') is not None:
+            self.behavior = m.get('Behavior')
+        if m.get('BehaviorReason') is not None:
+            self.behavior_reason = m.get('BehaviorReason')
+        self.original_constraints = []
+        if m.get('OriginalConstraints') is not None:
+            for k in m.get('OriginalConstraints'):
+                temp_model = GetServiceTemplateParameterConstraintsResponseBodyParameterConstraintsOriginalConstraints()
+                self.original_constraints.append(temp_model.from_map(k))
+        if m.get('ParameterKey') is not None:
+            self.parameter_key = m.get('ParameterKey')
+        if m.get('Type') is not None:
+            self.type = m.get('Type')
+        return self
+
+
+class GetServiceTemplateParameterConstraintsResponseBody(TeaModel):
+    def __init__(
+        self,
+        family_constraints: List[str] = None,
+        parameter_constraints: List[GetServiceTemplateParameterConstraintsResponseBodyParameterConstraints] = None,
+        request_id: str = None,
+    ):
+        self.family_constraints = family_constraints
+        self.parameter_constraints = parameter_constraints
+        self.request_id = request_id
+
+    def validate(self):
+        if self.parameter_constraints:
+            for k in self.parameter_constraints:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.family_constraints is not None:
+            result['FamilyConstraints'] = self.family_constraints
+        result['ParameterConstraints'] = []
+        if self.parameter_constraints is not None:
+            for k in self.parameter_constraints:
+                result['ParameterConstraints'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('FamilyConstraints') is not None:
+            self.family_constraints = m.get('FamilyConstraints')
+        self.parameter_constraints = []
+        if m.get('ParameterConstraints') is not None:
+            for k in m.get('ParameterConstraints'):
+                temp_model = GetServiceTemplateParameterConstraintsResponseBodyParameterConstraints()
+                self.parameter_constraints.append(temp_model.from_map(k))
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class GetServiceTemplateParameterConstraintsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetServiceTemplateParameterConstraintsResponseBody = None,
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
+            temp_model = GetServiceTemplateParameterConstraintsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetUploadCredentialsRequest(TeaModel):
     def __init__(
         self,
         file_name: str = None,
     ):
+        # This parameter is required.
         self.file_name = file_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3993,17 +5160,14 @@
         body: GetUploadCredentialsResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -4186,17 +5350,14 @@
         body: ListAcrImageRepositoriesResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -4379,17 +5540,14 @@
         body: ListAcrImageTagsResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -4415,44 +5573,45 @@
         return self
 
 
 class ListArtifactVersionsRequest(TeaModel):
     def __init__(
         self,
         artifact_id: str = None,
-        max_result: int = None,
+        max_results: int = None,
         next_token: str = None,
     ):
+        # This parameter is required.
         self.artifact_id = artifact_id
-        self.max_result = max_result
+        self.max_results = max_results
         self.next_token = next_token
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.artifact_id is not None:
             result['ArtifactId'] = self.artifact_id
-        if self.max_result is not None:
-            result['MaxResult'] = self.max_result
+        if self.max_results is not None:
+            result['MaxResults'] = self.max_results
         if self.next_token is not None:
             result['NextToken'] = self.next_token
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('ArtifactId') is not None:
             self.artifact_id = m.get('ArtifactId')
-        if m.get('MaxResult') is not None:
-            self.max_result = m.get('MaxResult')
+        if m.get('MaxResults') is not None:
+            self.max_results = m.get('MaxResults')
         if m.get('NextToken') is not None:
             self.next_token = m.get('NextToken')
         return self
 
 
 class ListArtifactVersionsResponseBodyArtifacts(TeaModel):
     def __init__(
@@ -4620,17 +5779,14 @@
         body: ListArtifactVersionsResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -4973,17 +6129,14 @@
         body: ListArtifactsResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -5339,14 +6492,15 @@
             self.value = m.get('Value')
         return self
 
 
 class ListServiceInstancesResponseBodyServiceInstances(TeaModel):
     def __init__(
         self,
+        biz_status: str = None,
         create_time: str = None,
         enable_instance_ops: bool = None,
         end_time: str = None,
         is_operated: bool = None,
         name: str = None,
         operated_service_instance_id: str = None,
         operation_end_time: str = None,
@@ -5362,14 +6516,15 @@
         status: str = None,
         status_detail: str = None,
         tags: List[ListServiceInstancesResponseBodyServiceInstancesTags] = None,
         template_name: str = None,
         update_time: str = None,
         user_id: int = None,
     ):
+        self.biz_status = biz_status
         self.create_time = create_time
         self.enable_instance_ops = enable_instance_ops
         self.end_time = end_time
         self.is_operated = is_operated
         self.name = name
         self.operated_service_instance_id = operated_service_instance_id
         self.operation_end_time = operation_end_time
@@ -5399,14 +6554,16 @@
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.biz_status is not None:
+            result['BizStatus'] = self.biz_status
         if self.create_time is not None:
             result['CreateTime'] = self.create_time
         if self.enable_instance_ops is not None:
             result['EnableInstanceOps'] = self.enable_instance_ops
         if self.end_time is not None:
             result['EndTime'] = self.end_time
         if self.is_operated is not None:
@@ -5449,14 +6606,16 @@
             result['UpdateTime'] = self.update_time
         if self.user_id is not None:
             result['UserId'] = self.user_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('BizStatus') is not None:
+            self.biz_status = m.get('BizStatus')
         if m.get('CreateTime') is not None:
             self.create_time = m.get('CreateTime')
         if m.get('EnableInstanceOps') is not None:
             self.enable_instance_ops = m.get('EnableInstanceOps')
         if m.get('EndTime') is not None:
             self.end_time = m.get('EndTime')
         if m.get('IsOperated') is not None:
@@ -5571,17 +6730,14 @@
         body: ListServiceInstancesResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -5642,18 +6798,20 @@
 
 class ListServiceUsagesRequest(TeaModel):
     def __init__(
         self,
         filter: List[ListServiceUsagesRequestFilter] = None,
         max_results: int = None,
         next_token: str = None,
+        supplier_role: str = None,
     ):
         self.filter = filter
         self.max_results = max_results
         self.next_token = next_token
+        self.supplier_role = supplier_role
 
     def validate(self):
         if self.filter:
             for k in self.filter:
                 if k:
                     k.validate()
 
@@ -5667,125 +6825,59 @@
         if self.filter is not None:
             for k in self.filter:
                 result['Filter'].append(k.to_map() if k else None)
         if self.max_results is not None:
             result['MaxResults'] = self.max_results
         if self.next_token is not None:
             result['NextToken'] = self.next_token
+        if self.supplier_role is not None:
+            result['SupplierRole'] = self.supplier_role
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         self.filter = []
         if m.get('Filter') is not None:
             for k in m.get('Filter'):
                 temp_model = ListServiceUsagesRequestFilter()
                 self.filter.append(temp_model.from_map(k))
         if m.get('MaxResults') is not None:
             self.max_results = m.get('MaxResults')
         if m.get('NextToken') is not None:
             self.next_token = m.get('NextToken')
-        return self
-
-
-class ListServiceUsagesResponseBodyServiceUsagesUserInformation(TeaModel):
-    def __init__(
-        self,
-        company: str = None,
-        country: str = None,
-        email_address: str = None,
-        industry: str = None,
-        name: str = None,
-        source: str = None,
-        telephone: str = None,
-        title: str = None,
-    ):
-        self.company = company
-        self.country = country
-        self.email_address = email_address
-        self.industry = industry
-        self.name = name
-        self.source = source
-        self.telephone = telephone
-        self.title = title
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.company is not None:
-            result['Company'] = self.company
-        if self.country is not None:
-            result['Country'] = self.country
-        if self.email_address is not None:
-            result['EmailAddress'] = self.email_address
-        if self.industry is not None:
-            result['Industry'] = self.industry
-        if self.name is not None:
-            result['Name'] = self.name
-        if self.source is not None:
-            result['Source'] = self.source
-        if self.telephone is not None:
-            result['Telephone'] = self.telephone
-        if self.title is not None:
-            result['Title'] = self.title
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('Company') is not None:
-            self.company = m.get('Company')
-        if m.get('Country') is not None:
-            self.country = m.get('Country')
-        if m.get('EmailAddress') is not None:
-            self.email_address = m.get('EmailAddress')
-        if m.get('Industry') is not None:
-            self.industry = m.get('Industry')
-        if m.get('Name') is not None:
-            self.name = m.get('Name')
-        if m.get('Source') is not None:
-            self.source = m.get('Source')
-        if m.get('Telephone') is not None:
-            self.telephone = m.get('Telephone')
-        if m.get('Title') is not None:
-            self.title = m.get('Title')
+        if m.get('SupplierRole') is not None:
+            self.supplier_role = m.get('SupplierRole')
         return self
 
 
 class ListServiceUsagesResponseBodyServiceUsages(TeaModel):
     def __init__(
         self,
         comments: str = None,
         create_time: str = None,
         service_id: str = None,
         service_name: str = None,
         status: str = None,
         supplier_name: str = None,
         update_time: str = None,
         user_ali_uid: int = None,
-        user_information: ListServiceUsagesResponseBodyServiceUsagesUserInformation = None,
+        user_information: Dict[str, str] = None,
     ):
         self.comments = comments
         self.create_time = create_time
         self.service_id = service_id
         self.service_name = service_name
         self.status = status
         self.supplier_name = supplier_name
         self.update_time = update_time
         self.user_ali_uid = user_ali_uid
         self.user_information = user_information
 
     def validate(self):
-        if self.user_information:
-            self.user_information.validate()
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -5802,15 +6894,15 @@
         if self.supplier_name is not None:
             result['SupplierName'] = self.supplier_name
         if self.update_time is not None:
             result['UpdateTime'] = self.update_time
         if self.user_ali_uid is not None:
             result['UserAliUid'] = self.user_ali_uid
         if self.user_information is not None:
-            result['UserInformation'] = self.user_information.to_map()
+            result['UserInformation'] = self.user_information
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Comments') is not None:
             self.comments = m.get('Comments')
         if m.get('CreateTime') is not None:
@@ -5824,16 +6916,15 @@
         if m.get('SupplierName') is not None:
             self.supplier_name = m.get('SupplierName')
         if m.get('UpdateTime') is not None:
             self.update_time = m.get('UpdateTime')
         if m.get('UserAliUid') is not None:
             self.user_ali_uid = m.get('UserAliUid')
         if m.get('UserInformation') is not None:
-            temp_model = ListServiceUsagesResponseBodyServiceUsagesUserInformation()
-            self.user_information = temp_model.from_map(m['UserInformation'])
+            self.user_information = m.get('UserInformation')
         return self
 
 
 class ListServiceUsagesResponseBody(TeaModel):
     def __init__(
         self,
         max_results: int = None,
@@ -5900,17 +6991,14 @@
         body: ListServiceUsagesResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -6013,14 +7101,15 @@
         resource_group_id: str = None,
         tag: List[ListServicesRequestTag] = None,
     ):
         self.all_versions = all_versions
         self.filter = filter
         self.max_results = max_results
         self.next_token = next_token
+        # This parameter is required.
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         self.tag = tag
 
     def validate(self):
         if self.filter:
             for k in self.filter:
@@ -6078,14 +7167,53 @@
         if m.get('Tag') is not None:
             for k in m.get('Tag'):
                 temp_model = ListServicesRequestTag()
                 self.tag.append(temp_model.from_map(k))
         return self
 
 
+class ListServicesResponseBodyServicesCommodity(TeaModel):
+    def __init__(
+        self,
+        commodity_code: str = None,
+        saas_boost_metadata: str = None,
+        type: str = None,
+    ):
+        self.commodity_code = commodity_code
+        self.saas_boost_metadata = saas_boost_metadata
+        self.type = type
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
+        if self.commodity_code is not None:
+            result['CommodityCode'] = self.commodity_code
+        if self.saas_boost_metadata is not None:
+            result['SaasBoostMetadata'] = self.saas_boost_metadata
+        if self.type is not None:
+            result['Type'] = self.type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CommodityCode') is not None:
+            self.commodity_code = m.get('CommodityCode')
+        if m.get('SaasBoostMetadata') is not None:
+            self.saas_boost_metadata = m.get('SaasBoostMetadata')
+        if m.get('Type') is not None:
+            self.type = m.get('Type')
+        return self
+
+
 class ListServicesResponseBodyServicesServiceInfos(TeaModel):
     def __init__(
         self,
         image: str = None,
         locale: str = None,
         name: str = None,
         short_description: str = None,
@@ -6162,23 +7290,30 @@
 
 class ListServicesResponseBodyServices(TeaModel):
     def __init__(
         self,
         approval_type: str = None,
         artifact_id: str = None,
         artifact_version: str = None,
+        build_info: str = None,
+        categories: str = None,
+        commodity: ListServicesResponseBodyServicesCommodity = None,
         commodity_code: str = None,
         create_time: str = None,
         default_version: bool = None,
         deploy_type: str = None,
+        has_beta: bool = None,
+        has_draft: bool = None,
         latest_resell_source_service_version: str = None,
         publish_time: str = None,
         relation_type: str = None,
+        resell_apply_status: str = None,
         resell_service_id: str = None,
         resource_group_id: str = None,
+        service_discoverable: str = None,
         service_id: str = None,
         service_infos: List[ListServicesResponseBodyServicesServiceInfos] = None,
         service_type: str = None,
         share_type: str = None,
         source_image: str = None,
         source_service_id: str = None,
         source_service_version: str = None,
@@ -6188,27 +7323,35 @@
         supplier_url: str = None,
         tags: List[ListServicesResponseBodyServicesTags] = None,
         tenant_type: str = None,
         trial_type: str = None,
         update_time: str = None,
         version: str = None,
         version_name: str = None,
+        virtual_internet_service: str = None,
     ):
         self.approval_type = approval_type
         self.artifact_id = artifact_id
         self.artifact_version = artifact_version
+        self.build_info = build_info
+        self.categories = categories
+        self.commodity = commodity
         self.commodity_code = commodity_code
         self.create_time = create_time
         self.default_version = default_version
         self.deploy_type = deploy_type
+        self.has_beta = has_beta
+        self.has_draft = has_draft
         self.latest_resell_source_service_version = latest_resell_source_service_version
         self.publish_time = publish_time
         self.relation_type = relation_type
+        self.resell_apply_status = resell_apply_status
         self.resell_service_id = resell_service_id
         self.resource_group_id = resource_group_id
+        self.service_discoverable = service_discoverable
         self.service_id = service_id
         self.service_infos = service_infos
         self.service_type = service_type
         self.share_type = share_type
         self.source_image = source_image
         self.source_service_id = source_service_id
         self.source_service_version = source_service_version
@@ -6218,16 +7361,19 @@
         self.supplier_url = supplier_url
         self.tags = tags
         self.tenant_type = tenant_type
         self.trial_type = trial_type
         self.update_time = update_time
         self.version = version
         self.version_name = version_name
+        self.virtual_internet_service = virtual_internet_service
 
     def validate(self):
+        if self.commodity:
+            self.commodity.validate()
         if self.service_infos:
             for k in self.service_infos:
                 if k:
                     k.validate()
         if self.tags:
             for k in self.tags:
                 if k:
@@ -6241,32 +7387,46 @@
         result = dict()
         if self.approval_type is not None:
             result['ApprovalType'] = self.approval_type
         if self.artifact_id is not None:
             result['ArtifactId'] = self.artifact_id
         if self.artifact_version is not None:
             result['ArtifactVersion'] = self.artifact_version
+        if self.build_info is not None:
+            result['BuildInfo'] = self.build_info
+        if self.categories is not None:
+            result['Categories'] = self.categories
+        if self.commodity is not None:
+            result['Commodity'] = self.commodity.to_map()
         if self.commodity_code is not None:
             result['CommodityCode'] = self.commodity_code
         if self.create_time is not None:
             result['CreateTime'] = self.create_time
         if self.default_version is not None:
             result['DefaultVersion'] = self.default_version
         if self.deploy_type is not None:
             result['DeployType'] = self.deploy_type
+        if self.has_beta is not None:
+            result['HasBeta'] = self.has_beta
+        if self.has_draft is not None:
+            result['HasDraft'] = self.has_draft
         if self.latest_resell_source_service_version is not None:
             result['LatestResellSourceServiceVersion'] = self.latest_resell_source_service_version
         if self.publish_time is not None:
             result['PublishTime'] = self.publish_time
         if self.relation_type is not None:
             result['RelationType'] = self.relation_type
+        if self.resell_apply_status is not None:
+            result['ResellApplyStatus'] = self.resell_apply_status
         if self.resell_service_id is not None:
             result['ResellServiceId'] = self.resell_service_id
         if self.resource_group_id is not None:
             result['ResourceGroupId'] = self.resource_group_id
+        if self.service_discoverable is not None:
+            result['ServiceDiscoverable'] = self.service_discoverable
         if self.service_id is not None:
             result['ServiceId'] = self.service_id
         result['ServiceInfos'] = []
         if self.service_infos is not None:
             for k in self.service_infos:
                 result['ServiceInfos'].append(k.to_map() if k else None)
         if self.service_type is not None:
@@ -6297,42 +7457,59 @@
             result['TrialType'] = self.trial_type
         if self.update_time is not None:
             result['UpdateTime'] = self.update_time
         if self.version is not None:
             result['Version'] = self.version
         if self.version_name is not None:
             result['VersionName'] = self.version_name
+        if self.virtual_internet_service is not None:
+            result['VirtualInternetService'] = self.virtual_internet_service
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('ApprovalType') is not None:
             self.approval_type = m.get('ApprovalType')
         if m.get('ArtifactId') is not None:
             self.artifact_id = m.get('ArtifactId')
         if m.get('ArtifactVersion') is not None:
             self.artifact_version = m.get('ArtifactVersion')
+        if m.get('BuildInfo') is not None:
+            self.build_info = m.get('BuildInfo')
+        if m.get('Categories') is not None:
+            self.categories = m.get('Categories')
+        if m.get('Commodity') is not None:
+            temp_model = ListServicesResponseBodyServicesCommodity()
+            self.commodity = temp_model.from_map(m['Commodity'])
         if m.get('CommodityCode') is not None:
             self.commodity_code = m.get('CommodityCode')
         if m.get('CreateTime') is not None:
             self.create_time = m.get('CreateTime')
         if m.get('DefaultVersion') is not None:
             self.default_version = m.get('DefaultVersion')
         if m.get('DeployType') is not None:
             self.deploy_type = m.get('DeployType')
+        if m.get('HasBeta') is not None:
+            self.has_beta = m.get('HasBeta')
+        if m.get('HasDraft') is not None:
+            self.has_draft = m.get('HasDraft')
         if m.get('LatestResellSourceServiceVersion') is not None:
             self.latest_resell_source_service_version = m.get('LatestResellSourceServiceVersion')
         if m.get('PublishTime') is not None:
             self.publish_time = m.get('PublishTime')
         if m.get('RelationType') is not None:
             self.relation_type = m.get('RelationType')
+        if m.get('ResellApplyStatus') is not None:
+            self.resell_apply_status = m.get('ResellApplyStatus')
         if m.get('ResellServiceId') is not None:
             self.resell_service_id = m.get('ResellServiceId')
         if m.get('ResourceGroupId') is not None:
             self.resource_group_id = m.get('ResourceGroupId')
+        if m.get('ServiceDiscoverable') is not None:
+            self.service_discoverable = m.get('ServiceDiscoverable')
         if m.get('ServiceId') is not None:
             self.service_id = m.get('ServiceId')
         self.service_infos = []
         if m.get('ServiceInfos') is not None:
             for k in m.get('ServiceInfos'):
                 temp_model = ListServicesResponseBodyServicesServiceInfos()
                 self.service_infos.append(temp_model.from_map(k))
@@ -6365,14 +7542,16 @@
             self.trial_type = m.get('TrialType')
         if m.get('UpdateTime') is not None:
             self.update_time = m.get('UpdateTime')
         if m.get('Version') is not None:
             self.version = m.get('Version')
         if m.get('VersionName') is not None:
             self.version_name = m.get('VersionName')
+        if m.get('VirtualInternetService') is not None:
+            self.virtual_internet_service = m.get('VirtualInternetService')
         return self
 
 
 class ListServicesResponseBody(TeaModel):
     def __init__(
         self,
         max_results: int = None,
@@ -6439,17 +7618,14 @@
         body: ListServicesResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -6479,14 +7655,15 @@
     def __init__(
         self,
         resources: str = None,
         service_instance_id: str = None,
         service_instance_resources_action: str = None,
     ):
         self.resources = resources
+        # This parameter is required.
         self.service_instance_id = service_instance_id
         self.service_instance_resources_action = service_instance_resources_action
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -6549,17 +7726,14 @@
         body: ModifyServiceInstanceResourcesResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -6587,15 +7761,17 @@
 
 class PushMeteringDataRequest(TeaModel):
     def __init__(
         self,
         metering: str = None,
         service_instance_id: str = None,
     ):
+        # This parameter is required.
         self.metering = metering
+        # This parameter is required.
         self.service_instance_id = service_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6653,17 +7829,14 @@
         body: PushMeteringDataResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -6693,15 +7866,17 @@
     def __init__(
         self,
         client_token: str = None,
         region_id: str = None,
         service_id: str = None,
     ):
         self.client_token = client_token
+        # This parameter is required.
         self.region_id = region_id
+        # This parameter is required.
         self.service_id = service_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6769,17 +7944,14 @@
         body: RegisterServiceResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -6806,14 +7978,15 @@
 
 
 class ReleaseArtifactRequest(TeaModel):
     def __init__(
         self,
         artifact_id: str = None,
     ):
+        # This parameter is required.
         self.artifact_id = artifact_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6915,17 +8088,14 @@
         body: ReleaseArtifactResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -7019,18 +8189,21 @@
         self,
         artifact_id: str = None,
         artifact_property: UpdateArtifactRequestArtifactProperty = None,
         description: str = None,
         support_region_ids: List[str] = None,
         version_name: str = None,
     ):
+        # This parameter is required.
         self.artifact_id = artifact_id
+        # This parameter is required.
         self.artifact_property = artifact_property
         self.description = description
         self.support_region_ids = support_region_ids
+        # This parameter is required.
         self.version_name = version_name
 
     def validate(self):
         if self.artifact_property:
             self.artifact_property.validate()
 
     def to_map(self):
@@ -7072,18 +8245,21 @@
         self,
         artifact_id: str = None,
         artifact_property_shrink: str = None,
         description: str = None,
         support_region_ids: List[str] = None,
         version_name: str = None,
     ):
+        # This parameter is required.
         self.artifact_id = artifact_id
+        # This parameter is required.
         self.artifact_property_shrink = artifact_property_shrink
         self.description = description
         self.support_region_ids = support_region_ids
+        # This parameter is required.
         self.version_name = version_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7207,17 +8383,14 @@
         body: UpdateArtifactResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -7239,113 +8412,195 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = UpdateArtifactResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class UpdateServiceRequestServiceInfoAgreements(TeaModel):
+    def __init__(
+        self,
+        name: str = None,
+        url: str = None,
+    ):
+        self.name = name
+        self.url = url
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
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.url is not None:
+            result['Url'] = self.url
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('Url') is not None:
+            self.url = m.get('Url')
+        return self
+
+
 class UpdateServiceRequestServiceInfo(TeaModel):
     def __init__(
         self,
+        agreements: List[UpdateServiceRequestServiceInfoAgreements] = None,
         image: str = None,
         locale: str = None,
         long_description_url: str = None,
         name: str = None,
         short_description: str = None,
     ):
+        self.agreements = agreements
         self.image = image
         self.locale = locale
         self.long_description_url = long_description_url
         self.name = name
         self.short_description = short_description
 
     def validate(self):
-        pass
+        if self.agreements:
+            for k in self.agreements:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        result['Agreements'] = []
+        if self.agreements is not None:
+            for k in self.agreements:
+                result['Agreements'].append(k.to_map() if k else None)
         if self.image is not None:
             result['Image'] = self.image
         if self.locale is not None:
             result['Locale'] = self.locale
         if self.long_description_url is not None:
             result['LongDescriptionUrl'] = self.long_description_url
         if self.name is not None:
             result['Name'] = self.name
         if self.short_description is not None:
             result['ShortDescription'] = self.short_description
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        self.agreements = []
+        if m.get('Agreements') is not None:
+            for k in m.get('Agreements'):
+                temp_model = UpdateServiceRequestServiceInfoAgreements()
+                self.agreements.append(temp_model.from_map(k))
         if m.get('Image') is not None:
             self.image = m.get('Image')
         if m.get('Locale') is not None:
             self.locale = m.get('Locale')
         if m.get('LongDescriptionUrl') is not None:
             self.long_description_url = m.get('LongDescriptionUrl')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('ShortDescription') is not None:
             self.short_description = m.get('ShortDescription')
         return self
 
 
+class UpdateServiceRequestUpdateOption(TeaModel):
+    def __init__(
+        self,
+        update_from: str = None,
+    ):
+        self.update_from = update_from
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
+        if self.update_from is not None:
+            result['UpdateFrom'] = self.update_from
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('UpdateFrom') is not None:
+            self.update_from = m.get('UpdateFrom')
+        return self
+
+
 class UpdateServiceRequest(TeaModel):
     def __init__(
         self,
         alarm_metadata: str = None,
         client_token: str = None,
         deploy_metadata: str = None,
         deploy_type: str = None,
         duration: int = None,
         is_support_operated: bool = None,
         license_metadata: str = None,
         log_metadata: str = None,
         operation_metadata: str = None,
         policy_names: str = None,
         region_id: str = None,
+        resellable: bool = None,
         service_id: str = None,
         service_info: List[UpdateServiceRequestServiceInfo] = None,
         service_type: str = None,
         service_version: str = None,
         tenant_type: str = None,
         trial_duration: int = None,
+        update_option: UpdateServiceRequestUpdateOption = None,
         upgrade_metadata: str = None,
         version_name: str = None,
     ):
         self.alarm_metadata = alarm_metadata
         self.client_token = client_token
         self.deploy_metadata = deploy_metadata
         self.deploy_type = deploy_type
         self.duration = duration
         self.is_support_operated = is_support_operated
         self.license_metadata = license_metadata
         self.log_metadata = log_metadata
         self.operation_metadata = operation_metadata
         self.policy_names = policy_names
+        # This parameter is required.
         self.region_id = region_id
+        self.resellable = resellable
+        # This parameter is required.
         self.service_id = service_id
         self.service_info = service_info
         self.service_type = service_type
         self.service_version = service_version
         self.tenant_type = tenant_type
         self.trial_duration = trial_duration
+        self.update_option = update_option
         self.upgrade_metadata = upgrade_metadata
         self.version_name = version_name
 
     def validate(self):
         if self.service_info:
             for k in self.service_info:
                 if k:
                     k.validate()
+        if self.update_option:
+            self.update_option.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -7367,28 +8622,32 @@
             result['LogMetadata'] = self.log_metadata
         if self.operation_metadata is not None:
             result['OperationMetadata'] = self.operation_metadata
         if self.policy_names is not None:
             result['PolicyNames'] = self.policy_names
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.resellable is not None:
+            result['Resellable'] = self.resellable
         if self.service_id is not None:
             result['ServiceId'] = self.service_id
         result['ServiceInfo'] = []
         if self.service_info is not None:
             for k in self.service_info:
                 result['ServiceInfo'].append(k.to_map() if k else None)
         if self.service_type is not None:
             result['ServiceType'] = self.service_type
         if self.service_version is not None:
             result['ServiceVersion'] = self.service_version
         if self.tenant_type is not None:
             result['TenantType'] = self.tenant_type
         if self.trial_duration is not None:
             result['TrialDuration'] = self.trial_duration
+        if self.update_option is not None:
+            result['UpdateOption'] = self.update_option.to_map()
         if self.upgrade_metadata is not None:
             result['UpgradeMetadata'] = self.upgrade_metadata
         if self.version_name is not None:
             result['VersionName'] = self.version_name
         return result
 
     def from_map(self, m: dict = None):
@@ -7411,14 +8670,16 @@
             self.log_metadata = m.get('LogMetadata')
         if m.get('OperationMetadata') is not None:
             self.operation_metadata = m.get('OperationMetadata')
         if m.get('PolicyNames') is not None:
             self.policy_names = m.get('PolicyNames')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('Resellable') is not None:
+            self.resellable = m.get('Resellable')
         if m.get('ServiceId') is not None:
             self.service_id = m.get('ServiceId')
         self.service_info = []
         if m.get('ServiceInfo') is not None:
             for k in m.get('ServiceInfo'):
                 temp_model = UpdateServiceRequestServiceInfo()
                 self.service_info.append(temp_model.from_map(k))
@@ -7426,14 +8687,272 @@
             self.service_type = m.get('ServiceType')
         if m.get('ServiceVersion') is not None:
             self.service_version = m.get('ServiceVersion')
         if m.get('TenantType') is not None:
             self.tenant_type = m.get('TenantType')
         if m.get('TrialDuration') is not None:
             self.trial_duration = m.get('TrialDuration')
+        if m.get('UpdateOption') is not None:
+            temp_model = UpdateServiceRequestUpdateOption()
+            self.update_option = temp_model.from_map(m['UpdateOption'])
+        if m.get('UpgradeMetadata') is not None:
+            self.upgrade_metadata = m.get('UpgradeMetadata')
+        if m.get('VersionName') is not None:
+            self.version_name = m.get('VersionName')
+        return self
+
+
+class UpdateServiceShrinkRequestServiceInfoAgreements(TeaModel):
+    def __init__(
+        self,
+        name: str = None,
+        url: str = None,
+    ):
+        self.name = name
+        self.url = url
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
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.url is not None:
+            result['Url'] = self.url
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('Url') is not None:
+            self.url = m.get('Url')
+        return self
+
+
+class UpdateServiceShrinkRequestServiceInfo(TeaModel):
+    def __init__(
+        self,
+        agreements: List[UpdateServiceShrinkRequestServiceInfoAgreements] = None,
+        image: str = None,
+        locale: str = None,
+        long_description_url: str = None,
+        name: str = None,
+        short_description: str = None,
+    ):
+        self.agreements = agreements
+        self.image = image
+        self.locale = locale
+        self.long_description_url = long_description_url
+        self.name = name
+        self.short_description = short_description
+
+    def validate(self):
+        if self.agreements:
+            for k in self.agreements:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Agreements'] = []
+        if self.agreements is not None:
+            for k in self.agreements:
+                result['Agreements'].append(k.to_map() if k else None)
+        if self.image is not None:
+            result['Image'] = self.image
+        if self.locale is not None:
+            result['Locale'] = self.locale
+        if self.long_description_url is not None:
+            result['LongDescriptionUrl'] = self.long_description_url
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.short_description is not None:
+            result['ShortDescription'] = self.short_description
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.agreements = []
+        if m.get('Agreements') is not None:
+            for k in m.get('Agreements'):
+                temp_model = UpdateServiceShrinkRequestServiceInfoAgreements()
+                self.agreements.append(temp_model.from_map(k))
+        if m.get('Image') is not None:
+            self.image = m.get('Image')
+        if m.get('Locale') is not None:
+            self.locale = m.get('Locale')
+        if m.get('LongDescriptionUrl') is not None:
+            self.long_description_url = m.get('LongDescriptionUrl')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('ShortDescription') is not None:
+            self.short_description = m.get('ShortDescription')
+        return self
+
+
+class UpdateServiceShrinkRequest(TeaModel):
+    def __init__(
+        self,
+        alarm_metadata: str = None,
+        client_token: str = None,
+        deploy_metadata: str = None,
+        deploy_type: str = None,
+        duration: int = None,
+        is_support_operated: bool = None,
+        license_metadata: str = None,
+        log_metadata: str = None,
+        operation_metadata: str = None,
+        policy_names: str = None,
+        region_id: str = None,
+        resellable: bool = None,
+        service_id: str = None,
+        service_info: List[UpdateServiceShrinkRequestServiceInfo] = None,
+        service_type: str = None,
+        service_version: str = None,
+        tenant_type: str = None,
+        trial_duration: int = None,
+        update_option_shrink: str = None,
+        upgrade_metadata: str = None,
+        version_name: str = None,
+    ):
+        self.alarm_metadata = alarm_metadata
+        self.client_token = client_token
+        self.deploy_metadata = deploy_metadata
+        self.deploy_type = deploy_type
+        self.duration = duration
+        self.is_support_operated = is_support_operated
+        self.license_metadata = license_metadata
+        self.log_metadata = log_metadata
+        self.operation_metadata = operation_metadata
+        self.policy_names = policy_names
+        # This parameter is required.
+        self.region_id = region_id
+        self.resellable = resellable
+        # This parameter is required.
+        self.service_id = service_id
+        self.service_info = service_info
+        self.service_type = service_type
+        self.service_version = service_version
+        self.tenant_type = tenant_type
+        self.trial_duration = trial_duration
+        self.update_option_shrink = update_option_shrink
+        self.upgrade_metadata = upgrade_metadata
+        self.version_name = version_name
+
+    def validate(self):
+        if self.service_info:
+            for k in self.service_info:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.alarm_metadata is not None:
+            result['AlarmMetadata'] = self.alarm_metadata
+        if self.client_token is not None:
+            result['ClientToken'] = self.client_token
+        if self.deploy_metadata is not None:
+            result['DeployMetadata'] = self.deploy_metadata
+        if self.deploy_type is not None:
+            result['DeployType'] = self.deploy_type
+        if self.duration is not None:
+            result['Duration'] = self.duration
+        if self.is_support_operated is not None:
+            result['IsSupportOperated'] = self.is_support_operated
+        if self.license_metadata is not None:
+            result['LicenseMetadata'] = self.license_metadata
+        if self.log_metadata is not None:
+            result['LogMetadata'] = self.log_metadata
+        if self.operation_metadata is not None:
+            result['OperationMetadata'] = self.operation_metadata
+        if self.policy_names is not None:
+            result['PolicyNames'] = self.policy_names
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resellable is not None:
+            result['Resellable'] = self.resellable
+        if self.service_id is not None:
+            result['ServiceId'] = self.service_id
+        result['ServiceInfo'] = []
+        if self.service_info is not None:
+            for k in self.service_info:
+                result['ServiceInfo'].append(k.to_map() if k else None)
+        if self.service_type is not None:
+            result['ServiceType'] = self.service_type
+        if self.service_version is not None:
+            result['ServiceVersion'] = self.service_version
+        if self.tenant_type is not None:
+            result['TenantType'] = self.tenant_type
+        if self.trial_duration is not None:
+            result['TrialDuration'] = self.trial_duration
+        if self.update_option_shrink is not None:
+            result['UpdateOption'] = self.update_option_shrink
+        if self.upgrade_metadata is not None:
+            result['UpgradeMetadata'] = self.upgrade_metadata
+        if self.version_name is not None:
+            result['VersionName'] = self.version_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AlarmMetadata') is not None:
+            self.alarm_metadata = m.get('AlarmMetadata')
+        if m.get('ClientToken') is not None:
+            self.client_token = m.get('ClientToken')
+        if m.get('DeployMetadata') is not None:
+            self.deploy_metadata = m.get('DeployMetadata')
+        if m.get('DeployType') is not None:
+            self.deploy_type = m.get('DeployType')
+        if m.get('Duration') is not None:
+            self.duration = m.get('Duration')
+        if m.get('IsSupportOperated') is not None:
+            self.is_support_operated = m.get('IsSupportOperated')
+        if m.get('LicenseMetadata') is not None:
+            self.license_metadata = m.get('LicenseMetadata')
+        if m.get('LogMetadata') is not None:
+            self.log_metadata = m.get('LogMetadata')
+        if m.get('OperationMetadata') is not None:
+            self.operation_metadata = m.get('OperationMetadata')
+        if m.get('PolicyNames') is not None:
+            self.policy_names = m.get('PolicyNames')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('Resellable') is not None:
+            self.resellable = m.get('Resellable')
+        if m.get('ServiceId') is not None:
+            self.service_id = m.get('ServiceId')
+        self.service_info = []
+        if m.get('ServiceInfo') is not None:
+            for k in m.get('ServiceInfo'):
+                temp_model = UpdateServiceShrinkRequestServiceInfo()
+                self.service_info.append(temp_model.from_map(k))
+        if m.get('ServiceType') is not None:
+            self.service_type = m.get('ServiceType')
+        if m.get('ServiceVersion') is not None:
+            self.service_version = m.get('ServiceVersion')
+        if m.get('TenantType') is not None:
+            self.tenant_type = m.get('TenantType')
+        if m.get('TrialDuration') is not None:
+            self.trial_duration = m.get('TrialDuration')
+        if m.get('UpdateOption') is not None:
+            self.update_option_shrink = m.get('UpdateOption')
         if m.get('UpgradeMetadata') is not None:
             self.upgrade_metadata = m.get('UpgradeMetadata')
         if m.get('VersionName') is not None:
             self.version_name = m.get('VersionName')
         return self
 
 
@@ -7472,17 +8991,14 @@
         body: UpdateServiceResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -7504,7 +9020,505 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = UpdateServiceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class UpdateServiceInstanceAttributeRequest(TeaModel):
+    def __init__(
+        self,
+        end_time: str = None,
+        region_id: str = None,
+        service_instance_id: str = None,
+    ):
+        # Use the UTC time format: yyyy-MM-ddTHH:mmZ
+        self.end_time = end_time
+        # This parameter is required.
+        self.region_id = region_id
+        # This parameter is required.
+        self.service_instance_id = service_instance_id
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
+        if self.end_time is not None:
+            result['EndTime'] = self.end_time
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.service_instance_id is not None:
+            result['ServiceInstanceId'] = self.service_instance_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('EndTime') is not None:
+            self.end_time = m.get('EndTime')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ServiceInstanceId') is not None:
+            self.service_instance_id = m.get('ServiceInstanceId')
+        return self
+
+
+class UpdateServiceInstanceAttributeResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
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
+class UpdateServiceInstanceAttributeResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: UpdateServiceInstanceAttributeResponseBody = None,
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
+            temp_model = UpdateServiceInstanceAttributeResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class UpdateServiceInstanceSpecRequest(TeaModel):
+    def __init__(
+        self,
+        client_token: str = None,
+        enable_user_prometheus: bool = None,
+        operation_name: str = None,
+        parameters: Dict[str, Any] = None,
+        predefined_parameters_name: str = None,
+        service_instance_id: str = None,
+    ):
+        self.client_token = client_token
+        self.enable_user_prometheus = enable_user_prometheus
+        self.operation_name = operation_name
+        self.parameters = parameters
+        self.predefined_parameters_name = predefined_parameters_name
+        self.service_instance_id = service_instance_id
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
+        if self.client_token is not None:
+            result['ClientToken'] = self.client_token
+        if self.enable_user_prometheus is not None:
+            result['EnableUserPrometheus'] = self.enable_user_prometheus
+        if self.operation_name is not None:
+            result['OperationName'] = self.operation_name
+        if self.parameters is not None:
+            result['Parameters'] = self.parameters
+        if self.predefined_parameters_name is not None:
+            result['PredefinedParametersName'] = self.predefined_parameters_name
+        if self.service_instance_id is not None:
+            result['ServiceInstanceId'] = self.service_instance_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ClientToken') is not None:
+            self.client_token = m.get('ClientToken')
+        if m.get('EnableUserPrometheus') is not None:
+            self.enable_user_prometheus = m.get('EnableUserPrometheus')
+        if m.get('OperationName') is not None:
+            self.operation_name = m.get('OperationName')
+        if m.get('Parameters') is not None:
+            self.parameters = m.get('Parameters')
+        if m.get('PredefinedParametersName') is not None:
+            self.predefined_parameters_name = m.get('PredefinedParametersName')
+        if m.get('ServiceInstanceId') is not None:
+            self.service_instance_id = m.get('ServiceInstanceId')
+        return self
+
+
+class UpdateServiceInstanceSpecShrinkRequest(TeaModel):
+    def __init__(
+        self,
+        client_token: str = None,
+        enable_user_prometheus: bool = None,
+        operation_name: str = None,
+        parameters_shrink: str = None,
+        predefined_parameters_name: str = None,
+        service_instance_id: str = None,
+    ):
+        self.client_token = client_token
+        self.enable_user_prometheus = enable_user_prometheus
+        self.operation_name = operation_name
+        self.parameters_shrink = parameters_shrink
+        self.predefined_parameters_name = predefined_parameters_name
+        self.service_instance_id = service_instance_id
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
+        if self.client_token is not None:
+            result['ClientToken'] = self.client_token
+        if self.enable_user_prometheus is not None:
+            result['EnableUserPrometheus'] = self.enable_user_prometheus
+        if self.operation_name is not None:
+            result['OperationName'] = self.operation_name
+        if self.parameters_shrink is not None:
+            result['Parameters'] = self.parameters_shrink
+        if self.predefined_parameters_name is not None:
+            result['PredefinedParametersName'] = self.predefined_parameters_name
+        if self.service_instance_id is not None:
+            result['ServiceInstanceId'] = self.service_instance_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ClientToken') is not None:
+            self.client_token = m.get('ClientToken')
+        if m.get('EnableUserPrometheus') is not None:
+            self.enable_user_prometheus = m.get('EnableUserPrometheus')
+        if m.get('OperationName') is not None:
+            self.operation_name = m.get('OperationName')
+        if m.get('Parameters') is not None:
+            self.parameters_shrink = m.get('Parameters')
+        if m.get('PredefinedParametersName') is not None:
+            self.predefined_parameters_name = m.get('PredefinedParametersName')
+        if m.get('ServiceInstanceId') is not None:
+            self.service_instance_id = m.get('ServiceInstanceId')
+        return self
+
+
+class UpdateServiceInstanceSpecResponseBody(TeaModel):
+    def __init__(
+        self,
+        order_id: str = None,
+        request_id: str = None,
+    ):
+        self.order_id = order_id
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
+        if self.order_id is not None:
+            result['OrderId'] = self.order_id
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('OrderId') is not None:
+            self.order_id = m.get('OrderId')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class UpdateServiceInstanceSpecResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: UpdateServiceInstanceSpecResponseBody = None,
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
+            temp_model = UpdateServiceInstanceSpecResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class UpgradeServiceInstanceRequest(TeaModel):
+    def __init__(
+        self,
+        client_token: str = None,
+        dry_run: str = None,
+        parameters: Dict[str, Any] = None,
+        region_id: str = None,
+        service_instance_id: str = None,
+        service_version: str = None,
+    ):
+        self.client_token = client_token
+        self.dry_run = dry_run
+        self.parameters = parameters
+        self.region_id = region_id
+        self.service_instance_id = service_instance_id
+        self.service_version = service_version
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
+        if self.client_token is not None:
+            result['ClientToken'] = self.client_token
+        if self.dry_run is not None:
+            result['DryRun'] = self.dry_run
+        if self.parameters is not None:
+            result['Parameters'] = self.parameters
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.service_instance_id is not None:
+            result['ServiceInstanceId'] = self.service_instance_id
+        if self.service_version is not None:
+            result['ServiceVersion'] = self.service_version
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ClientToken') is not None:
+            self.client_token = m.get('ClientToken')
+        if m.get('DryRun') is not None:
+            self.dry_run = m.get('DryRun')
+        if m.get('Parameters') is not None:
+            self.parameters = m.get('Parameters')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ServiceInstanceId') is not None:
+            self.service_instance_id = m.get('ServiceInstanceId')
+        if m.get('ServiceVersion') is not None:
+            self.service_version = m.get('ServiceVersion')
+        return self
+
+
+class UpgradeServiceInstanceShrinkRequest(TeaModel):
+    def __init__(
+        self,
+        client_token: str = None,
+        dry_run: str = None,
+        parameters_shrink: str = None,
+        region_id: str = None,
+        service_instance_id: str = None,
+        service_version: str = None,
+    ):
+        self.client_token = client_token
+        self.dry_run = dry_run
+        self.parameters_shrink = parameters_shrink
+        self.region_id = region_id
+        self.service_instance_id = service_instance_id
+        self.service_version = service_version
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
+        if self.client_token is not None:
+            result['ClientToken'] = self.client_token
+        if self.dry_run is not None:
+            result['DryRun'] = self.dry_run
+        if self.parameters_shrink is not None:
+            result['Parameters'] = self.parameters_shrink
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.service_instance_id is not None:
+            result['ServiceInstanceId'] = self.service_instance_id
+        if self.service_version is not None:
+            result['ServiceVersion'] = self.service_version
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ClientToken') is not None:
+            self.client_token = m.get('ClientToken')
+        if m.get('DryRun') is not None:
+            self.dry_run = m.get('DryRun')
+        if m.get('Parameters') is not None:
+            self.parameters_shrink = m.get('Parameters')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ServiceInstanceId') is not None:
+            self.service_instance_id = m.get('ServiceInstanceId')
+        if m.get('ServiceVersion') is not None:
+            self.service_version = m.get('ServiceVersion')
+        return self
+
+
+class UpgradeServiceInstanceResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        service_instance_id: str = None,
+        status: str = None,
+        upgrade_required_parameters: List[str] = None,
+    ):
+        self.request_id = request_id
+        self.service_instance_id = service_instance_id
+        self.status = status
+        self.upgrade_required_parameters = upgrade_required_parameters
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
+        if self.service_instance_id is not None:
+            result['ServiceInstanceId'] = self.service_instance_id
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.upgrade_required_parameters is not None:
+            result['UpgradeRequiredParameters'] = self.upgrade_required_parameters
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('ServiceInstanceId') is not None:
+            self.service_instance_id = m.get('ServiceInstanceId')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('UpgradeRequiredParameters') is not None:
+            self.upgrade_required_parameters = m.get('UpgradeRequiredParameters')
+        return self
+
+
+class UpgradeServiceInstanceResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: UpgradeServiceInstanceResponseBody = None,
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
+            temp_model = UpgradeServiceInstanceResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
```

### Comparing `alibabacloud_computenestsupplier20210521-2.3.2/alibabacloud_computenestsupplier20210521.egg-info/PKG-INFO` & `alibabacloud_computenestsupplier20210521-3.0.0/alibabacloud_computenestsupplier20210521.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-computenestsupplier20210521
-Version: 2.3.2
+Version: 3.0.0
 Summary: Alibaba Cloud ComputeNestSupplier (20210521) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/computenestsupplier-20210521/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_computenestsupplier20210521-2.3.2/alibabacloud_computenestsupplier20210521.egg-info/SOURCES.txt` & `alibabacloud_computenestsupplier20210521-3.0.0/alibabacloud_computenestsupplier20210521.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_computenestsupplier20210521-2.3.2/setup.py` & `alibabacloud_computenestsupplier20210521-3.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_computenestsupplier20210521.
 
-Created on 08/09/2023
+Created on 30/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_computenestsupplier20210521"
 NAME = "alibabacloud_computenestsupplier20210521" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ComputeNestSupplier (20210521) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.11, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
+    "alibabacloud_tea_util>=0.3.12, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.9, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
```

