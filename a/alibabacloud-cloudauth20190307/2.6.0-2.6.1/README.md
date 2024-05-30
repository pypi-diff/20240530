# Comparing `tmp/alibabacloud_cloudauth20190307-2.6.0.tar.gz` & `tmp/alibabacloud_cloudauth20190307-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cloudauth20190307-2.6.0.tar", last modified: Fri Apr 26 07:31:47 2024, max compression
+gzip compressed data, was "dist/alibabacloud_cloudauth20190307-2.6.1.tar", last modified: Thu May 30 17:11:27 2024, max compression
```

## Comparing `alibabacloud_cloudauth20190307-2.6.0.tar` & `alibabacloud_cloudauth20190307-2.6.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 07:31:47.000000 alibabacloud_cloudauth20190307-2.6.0/
--rw-r--r--   0 root         (0) root         (0)     1530 2024-04-26 07:31:47.000000 alibabacloud_cloudauth20190307-2.6.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-26 07:31:47.000000 alibabacloud_cloudauth20190307-2.6.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-26 07:31:47.000000 alibabacloud_cloudauth20190307-2.6.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2449 2024-04-26 07:31:47.000000 alibabacloud_cloudauth20190307-2.6.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1119 2024-04-26 07:31:47.000000 alibabacloud_cloudauth20190307-2.6.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1204 2024-04-26 07:31:47.000000 alibabacloud_cloudauth20190307-2.6.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 07:31:47.000000 alibabacloud_cloudauth20190307-2.6.0/alibabacloud_cloudauth20190307/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-26 07:31:47.000000 alibabacloud_cloudauth20190307-2.6.0/alibabacloud_cloudauth20190307/__init__.py
--rw-r--r--   0 root         (0) root         (0)   117681 2024-04-26 07:31:47.000000 alibabacloud_cloudauth20190307-2.6.0/alibabacloud_cloudauth20190307/client.py
--rw-r--r--   0 root         (0) root         (0)   193806 2024-04-26 07:31:47.000000 alibabacloud_cloudauth20190307-2.6.0/alibabacloud_cloudauth20190307/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 07:31:47.000000 alibabacloud_cloudauth20190307-2.6.0/alibabacloud_cloudauth20190307.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2449 2024-04-26 07:31:47.000000 alibabacloud_cloudauth20190307-2.6.0/alibabacloud_cloudauth20190307.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      468 2024-04-26 07:31:47.000000 alibabacloud_cloudauth20190307-2.6.0/alibabacloud_cloudauth20190307.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 07:31:47.000000 alibabacloud_cloudauth20190307-2.6.0/alibabacloud_cloudauth20190307.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      316 2024-04-26 07:31:47.000000 alibabacloud_cloudauth20190307-2.6.0/alibabacloud_cloudauth20190307.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-04-26 07:31:47.000000 alibabacloud_cloudauth20190307-2.6.0/alibabacloud_cloudauth20190307.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-26 07:31:47.000000 alibabacloud_cloudauth20190307-2.6.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2838 2024-04-26 07:31:47.000000 alibabacloud_cloudauth20190307-2.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 17:11:27.000000 alibabacloud_cloudauth20190307-2.6.1/
+-rw-r--r--   0 root         (0) root         (0)     1590 2024-05-30 17:11:26.000000 alibabacloud_cloudauth20190307-2.6.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-30 17:11:26.000000 alibabacloud_cloudauth20190307-2.6.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-30 17:11:26.000000 alibabacloud_cloudauth20190307-2.6.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2449 2024-05-30 17:11:27.000000 alibabacloud_cloudauth20190307-2.6.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1119 2024-05-30 17:11:26.000000 alibabacloud_cloudauth20190307-2.6.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1204 2024-05-30 17:11:26.000000 alibabacloud_cloudauth20190307-2.6.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 17:11:27.000000 alibabacloud_cloudauth20190307-2.6.1/alibabacloud_cloudauth20190307/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-30 17:11:26.000000 alibabacloud_cloudauth20190307-2.6.1/alibabacloud_cloudauth20190307/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   136573 2024-05-30 17:11:26.000000 alibabacloud_cloudauth20190307-2.6.1/alibabacloud_cloudauth20190307/client.py
+-rw-r--r--   0 root         (0) root         (0)   195104 2024-05-30 17:11:26.000000 alibabacloud_cloudauth20190307-2.6.1/alibabacloud_cloudauth20190307/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 17:11:27.000000 alibabacloud_cloudauth20190307-2.6.1/alibabacloud_cloudauth20190307.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2449 2024-05-30 17:11:27.000000 alibabacloud_cloudauth20190307-2.6.1/alibabacloud_cloudauth20190307.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      468 2024-05-30 17:11:27.000000 alibabacloud_cloudauth20190307-2.6.1/alibabacloud_cloudauth20190307.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 17:11:27.000000 alibabacloud_cloudauth20190307-2.6.1/alibabacloud_cloudauth20190307.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      316 2024-05-30 17:11:27.000000 alibabacloud_cloudauth20190307-2.6.1/alibabacloud_cloudauth20190307.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-30 17:11:27.000000 alibabacloud_cloudauth20190307-2.6.1/alibabacloud_cloudauth20190307.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-30 17:11:27.000000 alibabacloud_cloudauth20190307-2.6.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2838 2024-05-30 17:11:26.000000 alibabacloud_cloudauth20190307-2.6.1/setup.py
```

### Comparing `alibabacloud_cloudauth20190307-2.6.0/ChangeLog.md` & `alibabacloud_cloudauth20190307-2.6.1/ChangeLog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2024-04-26 Version: 2.6.0
+- Support API CredentialVerify.
+
+
 2024-04-10 Version: 2.5.0
 - Support API BankMetaVerify.
 - Support API DescribePageFaceVerifyData.
 - Support API MobileDetect.
 - Support API MobileOnlineStatus.
 - Support API MobileOnlineTime.
```

### Comparing `alibabacloud_cloudauth20190307-2.6.0/LICENSE` & `alibabacloud_cloudauth20190307-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth20190307-2.6.0/PKG-INFO` & `alibabacloud_cloudauth20190307-2.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cloudauth20190307
-Version: 2.6.0
+Version: 2.6.1
 Summary: Alibaba Cloud ID Verification (20190307) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloudauth20190307-2.6.0/README-CN.md` & `alibabacloud_cloudauth20190307-2.6.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth20190307-2.6.0/README.md` & `alibabacloud_cloudauth20190307-2.6.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth20190307-2.6.0/alibabacloud_cloudauth20190307/client.py` & `alibabacloud_cloudauth20190307-2.6.1/alibabacloud_cloudauth20190307/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 from alibabacloud_endpoint_util.client import Client as EndpointUtilClient
 from alibabacloud_cloudauth20190307 import models as cloudauth_20190307_models
 from alibabacloud_tea_util import models as util_models
 from alibabacloud_openapi_util.client import Client as OpenApiUtilClient
 from alibabacloud_openplatform20191219.client import Client as OpenPlatformClient
 from alibabacloud_openplatform20191219 import models as open_platform_models
 from alibabacloud_oss_sdk import models as oss_models
+from alibabacloud_oss_sdk.client import Client as OSSClient
 from alibabacloud_tea_fileform import models as file_form_models
 from alibabacloud_oss_util import models as ossutil_models
-from alibabacloud_oss_sdk.client import Client as OSSClient
 
 
 class Client(OpenApiClient):
     """
     *\
     """
     def __init__(
@@ -48,14 +48,21 @@
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
     def a_igcface_verify_with_options(
         self,
         request: cloudauth_20190307_models.AIGCFaceVerifyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.AIGCFaceVerifyResponse:
+        """
+        @summary 新增AIGC人脸检测能力
+        
+        @param request: AIGCFaceVerifyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: AIGCFaceVerifyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.face_contrast_picture_url):
             query['FaceContrastPictureUrl'] = request.face_contrast_picture_url
         if not UtilClient.is_unset(request.oss_bucket_name):
             query['OssBucketName'] = request.oss_bucket_name
         if not UtilClient.is_unset(request.oss_object_name):
@@ -90,14 +97,21 @@
         )
 
     async def a_igcface_verify_with_options_async(
         self,
         request: cloudauth_20190307_models.AIGCFaceVerifyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.AIGCFaceVerifyResponse:
+        """
+        @summary 新增AIGC人脸检测能力
+        
+        @param request: AIGCFaceVerifyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: AIGCFaceVerifyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.face_contrast_picture_url):
             query['FaceContrastPictureUrl'] = request.face_contrast_picture_url
         if not UtilClient.is_unset(request.oss_bucket_name):
             query['OssBucketName'] = request.oss_bucket_name
         if not UtilClient.is_unset(request.oss_object_name):
@@ -131,29 +145,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def a_igcface_verify(
         self,
         request: cloudauth_20190307_models.AIGCFaceVerifyRequest,
     ) -> cloudauth_20190307_models.AIGCFaceVerifyResponse:
+        """
+        @summary 新增AIGC人脸检测能力
+        
+        @param request: AIGCFaceVerifyRequest
+        @return: AIGCFaceVerifyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.a_igcface_verify_with_options(request, runtime)
 
     async def a_igcface_verify_async(
         self,
         request: cloudauth_20190307_models.AIGCFaceVerifyRequest,
     ) -> cloudauth_20190307_models.AIGCFaceVerifyResponse:
+        """
+        @summary 新增AIGC人脸检测能力
+        
+        @param request: AIGCFaceVerifyRequest
+        @return: AIGCFaceVerifyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.a_igcface_verify_with_options_async(request, runtime)
 
     def bank_meta_verify_with_options(
         self,
         request: cloudauth_20190307_models.BankMetaVerifyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.BankMetaVerifyResponse:
+        """
+        @summary 银行卡要素核验接口
+        
+        @param request: BankMetaVerifyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: BankMetaVerifyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.bank_card):
             query['BankCard'] = request.bank_card
         if not UtilClient.is_unset(request.identify_num):
             query['IdentifyNum'] = request.identify_num
         if not UtilClient.is_unset(request.mobile):
@@ -186,14 +219,21 @@
         )
 
     async def bank_meta_verify_with_options_async(
         self,
         request: cloudauth_20190307_models.BankMetaVerifyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.BankMetaVerifyResponse:
+        """
+        @summary 银行卡要素核验接口
+        
+        @param request: BankMetaVerifyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: BankMetaVerifyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.bank_card):
             query['BankCard'] = request.bank_card
         if not UtilClient.is_unset(request.identify_num):
             query['IdentifyNum'] = request.identify_num
         if not UtilClient.is_unset(request.mobile):
@@ -225,29 +265,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def bank_meta_verify(
         self,
         request: cloudauth_20190307_models.BankMetaVerifyRequest,
     ) -> cloudauth_20190307_models.BankMetaVerifyResponse:
+        """
+        @summary 银行卡要素核验接口
+        
+        @param request: BankMetaVerifyRequest
+        @return: BankMetaVerifyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.bank_meta_verify_with_options(request, runtime)
 
     async def bank_meta_verify_async(
         self,
         request: cloudauth_20190307_models.BankMetaVerifyRequest,
     ) -> cloudauth_20190307_models.BankMetaVerifyResponse:
+        """
+        @summary 银行卡要素核验接口
+        
+        @param request: BankMetaVerifyRequest
+        @return: BankMetaVerifyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.bank_meta_verify_with_options_async(request, runtime)
 
     def compare_face_verify_with_options(
         self,
         request: cloudauth_20190307_models.CompareFaceVerifyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.CompareFaceVerifyResponse:
+        """
+        @param request: CompareFaceVerifyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CompareFaceVerifyResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.crop):
             body['Crop'] = request.crop
         if not UtilClient.is_unset(request.outer_order_no):
             body['OuterOrderNo'] = request.outer_order_no
         if not UtilClient.is_unset(request.product_code):
@@ -294,14 +351,19 @@
         )
 
     async def compare_face_verify_with_options_async(
         self,
         request: cloudauth_20190307_models.CompareFaceVerifyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.CompareFaceVerifyResponse:
+        """
+        @param request: CompareFaceVerifyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CompareFaceVerifyResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.crop):
             body['Crop'] = request.crop
         if not UtilClient.is_unset(request.outer_order_no):
             body['OuterOrderNo'] = request.outer_order_no
         if not UtilClient.is_unset(request.product_code):
@@ -347,29 +409,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def compare_face_verify(
         self,
         request: cloudauth_20190307_models.CompareFaceVerifyRequest,
     ) -> cloudauth_20190307_models.CompareFaceVerifyResponse:
+        """
+        @param request: CompareFaceVerifyRequest
+        @return: CompareFaceVerifyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.compare_face_verify_with_options(request, runtime)
 
     async def compare_face_verify_async(
         self,
         request: cloudauth_20190307_models.CompareFaceVerifyRequest,
     ) -> cloudauth_20190307_models.CompareFaceVerifyResponse:
+        """
+        @param request: CompareFaceVerifyRequest
+        @return: CompareFaceVerifyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.compare_face_verify_with_options_async(request, runtime)
 
     def compare_faces_with_options(
         self,
         request: cloudauth_20190307_models.CompareFacesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.CompareFacesResponse:
+        """
+        @param request: CompareFacesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CompareFacesResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.source_image_type):
             body['SourceImageType'] = request.source_image_type
         if not UtilClient.is_unset(request.source_image_value):
             body['SourceImageValue'] = request.source_image_value
         if not UtilClient.is_unset(request.target_image_type):
@@ -396,14 +471,19 @@
         )
 
     async def compare_faces_with_options_async(
         self,
         request: cloudauth_20190307_models.CompareFacesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.CompareFacesResponse:
+        """
+        @param request: CompareFacesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CompareFacesResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.source_image_type):
             body['SourceImageType'] = request.source_image_type
         if not UtilClient.is_unset(request.source_image_value):
             body['SourceImageValue'] = request.source_image_value
         if not UtilClient.is_unset(request.target_image_type):
@@ -429,29 +509,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def compare_faces(
         self,
         request: cloudauth_20190307_models.CompareFacesRequest,
     ) -> cloudauth_20190307_models.CompareFacesResponse:
+        """
+        @param request: CompareFacesRequest
+        @return: CompareFacesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.compare_faces_with_options(request, runtime)
 
     async def compare_faces_async(
         self,
         request: cloudauth_20190307_models.CompareFacesRequest,
     ) -> cloudauth_20190307_models.CompareFacesResponse:
+        """
+        @param request: CompareFacesRequest
+        @return: CompareFacesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.compare_faces_with_options_async(request, runtime)
 
     def contrast_face_verify_with_options(
         self,
         request: cloudauth_20190307_models.ContrastFaceVerifyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.ContrastFaceVerifyResponse:
+        """
+        @param request: ContrastFaceVerifyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ContrastFaceVerifyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.model):
             query['Model'] = request.model
         body = {}
         if not UtilClient.is_unset(request.cert_name):
             body['CertName'] = request.cert_name
@@ -510,14 +603,19 @@
         )
 
     async def contrast_face_verify_with_options_async(
         self,
         request: cloudauth_20190307_models.ContrastFaceVerifyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.ContrastFaceVerifyResponse:
+        """
+        @param request: ContrastFaceVerifyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ContrastFaceVerifyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.model):
             query['Model'] = request.model
         body = {}
         if not UtilClient.is_unset(request.cert_name):
             body['CertName'] = request.cert_name
@@ -575,36 +673,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def contrast_face_verify(
         self,
         request: cloudauth_20190307_models.ContrastFaceVerifyRequest,
     ) -> cloudauth_20190307_models.ContrastFaceVerifyResponse:
+        """
+        @param request: ContrastFaceVerifyRequest
+        @return: ContrastFaceVerifyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.contrast_face_verify_with_options(request, runtime)
 
     async def contrast_face_verify_async(
         self,
         request: cloudauth_20190307_models.ContrastFaceVerifyRequest,
     ) -> cloudauth_20190307_models.ContrastFaceVerifyResponse:
+        """
+        @param request: ContrastFaceVerifyRequest
+        @return: ContrastFaceVerifyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.contrast_face_verify_with_options_async(request, runtime)
 
     def contrast_face_verify_advance(
         self,
         request: cloudauth_20190307_models.ContrastFaceVerifyAdvanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.ContrastFaceVerifyResponse:
         # Step 0: init client
         access_key_id = self._credential.get_access_key_id()
         access_key_secret = self._credential.get_access_key_secret()
         security_token = self._credential.get_security_token()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
-        if UtilClient.is_unset(open_platform_endpoint):
+        if UtilClient.empty(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
         auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
@@ -616,20 +722,21 @@
         auth_client = OpenPlatformClient(auth_config)
         auth_request = open_platform_models.AuthorizeFileUploadRequest(
             product='Cloudauth',
             region_id=self._region_id
         )
         auth_response = open_platform_models.AuthorizeFileUploadResponse()
         oss_config = oss_models.Config(
+            access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             type='access_key',
             protocol=self._protocol,
             region_id=self._region_id
         )
-        oss_client = None
+        oss_client = OSSClient(oss_config)
         file_obj = file_form_models.FileField()
         oss_header = oss_models.PostObjectRequestHeader()
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         contrast_face_verify_req = cloudauth_20190307_models.ContrastFaceVerifyRequest()
         OpenApiUtilClient.convert(request, contrast_face_verify_req)
@@ -667,15 +774,15 @@
     ) -> cloudauth_20190307_models.ContrastFaceVerifyResponse:
         # Step 0: init client
         access_key_id = await self._credential.get_access_key_id_async()
         access_key_secret = await self._credential.get_access_key_secret_async()
         security_token = await self._credential.get_security_token_async()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
-        if UtilClient.is_unset(open_platform_endpoint):
+        if UtilClient.empty(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
         auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
@@ -687,20 +794,21 @@
         auth_client = OpenPlatformClient(auth_config)
         auth_request = open_platform_models.AuthorizeFileUploadRequest(
             product='Cloudauth',
             region_id=self._region_id
         )
         auth_response = open_platform_models.AuthorizeFileUploadResponse()
         oss_config = oss_models.Config(
+            access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             type='access_key',
             protocol=self._protocol,
             region_id=self._region_id
         )
-        oss_client = None
+        oss_client = OSSClient(oss_config)
         file_obj = file_form_models.FileField()
         oss_header = oss_models.PostObjectRequestHeader()
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         contrast_face_verify_req = cloudauth_20190307_models.ContrastFaceVerifyRequest()
         OpenApiUtilClient.convert(request, contrast_face_verify_req)
@@ -732,14 +840,19 @@
         return contrast_face_verify_resp
 
     def create_auth_key_with_options(
         self,
         request: cloudauth_20190307_models.CreateAuthKeyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.CreateAuthKeyResponse:
+        """
+        @param request: CreateAuthKeyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateAuthKeyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.auth_years):
             query['AuthYears'] = request.auth_years
         if not UtilClient.is_unset(request.biz_type):
             query['BizType'] = request.biz_type
         if not UtilClient.is_unset(request.test):
@@ -766,14 +879,19 @@
         )
 
     async def create_auth_key_with_options_async(
         self,
         request: cloudauth_20190307_models.CreateAuthKeyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.CreateAuthKeyResponse:
+        """
+        @param request: CreateAuthKeyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateAuthKeyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.auth_years):
             query['AuthYears'] = request.auth_years
         if not UtilClient.is_unset(request.biz_type):
             query['BizType'] = request.biz_type
         if not UtilClient.is_unset(request.test):
@@ -799,29 +917,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_auth_key(
         self,
         request: cloudauth_20190307_models.CreateAuthKeyRequest,
     ) -> cloudauth_20190307_models.CreateAuthKeyResponse:
+        """
+        @param request: CreateAuthKeyRequest
+        @return: CreateAuthKeyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_auth_key_with_options(request, runtime)
 
     async def create_auth_key_async(
         self,
         request: cloudauth_20190307_models.CreateAuthKeyRequest,
     ) -> cloudauth_20190307_models.CreateAuthKeyResponse:
+        """
+        @param request: CreateAuthKeyRequest
+        @return: CreateAuthKeyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_auth_key_with_options_async(request, runtime)
 
     def create_verify_setting_with_options(
         self,
         request: cloudauth_20190307_models.CreateVerifySettingRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.CreateVerifySettingResponse:
+        """
+        @param request: CreateVerifySettingRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateVerifySettingResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.biz_name):
             query['BizName'] = request.biz_name
         if not UtilClient.is_unset(request.biz_type):
             query['BizType'] = request.biz_type
         if not UtilClient.is_unset(request.guide_step):
@@ -852,14 +983,19 @@
         )
 
     async def create_verify_setting_with_options_async(
         self,
         request: cloudauth_20190307_models.CreateVerifySettingRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.CreateVerifySettingResponse:
+        """
+        @param request: CreateVerifySettingRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateVerifySettingResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.biz_name):
             query['BizName'] = request.biz_name
         if not UtilClient.is_unset(request.biz_type):
             query['BizType'] = request.biz_type
         if not UtilClient.is_unset(request.guide_step):
@@ -889,29 +1025,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_verify_setting(
         self,
         request: cloudauth_20190307_models.CreateVerifySettingRequest,
     ) -> cloudauth_20190307_models.CreateVerifySettingResponse:
+        """
+        @param request: CreateVerifySettingRequest
+        @return: CreateVerifySettingResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_verify_setting_with_options(request, runtime)
 
     async def create_verify_setting_async(
         self,
         request: cloudauth_20190307_models.CreateVerifySettingRequest,
     ) -> cloudauth_20190307_models.CreateVerifySettingResponse:
+        """
+        @param request: CreateVerifySettingRequest
+        @return: CreateVerifySettingResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_verify_setting_with_options_async(request, runtime)
 
     def credential_verify_with_options(
         self,
         request: cloudauth_20190307_models.CredentialVerifyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.CredentialVerifyResponse:
+        """
+        @summary 凭证核验
+        
+        @param request: CredentialVerifyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CredentialVerifyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.cert_num):
             query['CertNum'] = request.cert_num
         if not UtilClient.is_unset(request.cred_name):
             query['CredName'] = request.cred_name
         if not UtilClient.is_unset(request.cred_type):
@@ -920,14 +1071,16 @@
             query['IdentifyNum'] = request.identify_num
         if not UtilClient.is_unset(request.image_url):
             query['ImageUrl'] = request.image_url
         if not UtilClient.is_unset(request.is_check):
             query['IsCheck'] = request.is_check
         if not UtilClient.is_unset(request.is_ocr):
             query['IsOCR'] = request.is_ocr
+        if not UtilClient.is_unset(request.merchant_id):
+            query['MerchantId'] = request.merchant_id
         if not UtilClient.is_unset(request.user_name):
             query['UserName'] = request.user_name
         body = {}
         if not UtilClient.is_unset(request.image_context):
             body['ImageContext'] = request.image_context
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query),
@@ -950,14 +1103,21 @@
         )
 
     async def credential_verify_with_options_async(
         self,
         request: cloudauth_20190307_models.CredentialVerifyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.CredentialVerifyResponse:
+        """
+        @summary 凭证核验
+        
+        @param request: CredentialVerifyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CredentialVerifyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.cert_num):
             query['CertNum'] = request.cert_num
         if not UtilClient.is_unset(request.cred_name):
             query['CredName'] = request.cred_name
         if not UtilClient.is_unset(request.cred_type):
@@ -966,14 +1126,16 @@
             query['IdentifyNum'] = request.identify_num
         if not UtilClient.is_unset(request.image_url):
             query['ImageUrl'] = request.image_url
         if not UtilClient.is_unset(request.is_check):
             query['IsCheck'] = request.is_check
         if not UtilClient.is_unset(request.is_ocr):
             query['IsOCR'] = request.is_ocr
+        if not UtilClient.is_unset(request.merchant_id):
+            query['MerchantId'] = request.merchant_id
         if not UtilClient.is_unset(request.user_name):
             query['UserName'] = request.user_name
         body = {}
         if not UtilClient.is_unset(request.image_context):
             body['ImageContext'] = request.image_context
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query),
@@ -995,29 +1157,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def credential_verify(
         self,
         request: cloudauth_20190307_models.CredentialVerifyRequest,
     ) -> cloudauth_20190307_models.CredentialVerifyResponse:
+        """
+        @summary 凭证核验
+        
+        @param request: CredentialVerifyRequest
+        @return: CredentialVerifyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.credential_verify_with_options(request, runtime)
 
     async def credential_verify_async(
         self,
         request: cloudauth_20190307_models.CredentialVerifyRequest,
     ) -> cloudauth_20190307_models.CredentialVerifyResponse:
+        """
+        @summary 凭证核验
+        
+        @param request: CredentialVerifyRequest
+        @return: CredentialVerifyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.credential_verify_with_options_async(request, runtime)
 
     def describe_device_info_with_options(
         self,
         request: cloudauth_20190307_models.DescribeDeviceInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.DescribeDeviceInfoResponse:
+        """
+        @param request: DescribeDeviceInfoRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDeviceInfoResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.biz_type):
             query['BizType'] = request.biz_type
         if not UtilClient.is_unset(request.current_page):
             query['CurrentPage'] = request.current_page
         if not UtilClient.is_unset(request.device_id):
@@ -1050,14 +1229,19 @@
         )
 
     async def describe_device_info_with_options_async(
         self,
         request: cloudauth_20190307_models.DescribeDeviceInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.DescribeDeviceInfoResponse:
+        """
+        @param request: DescribeDeviceInfoRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDeviceInfoResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.biz_type):
             query['BizType'] = request.biz_type
         if not UtilClient.is_unset(request.current_page):
             query['CurrentPage'] = request.current_page
         if not UtilClient.is_unset(request.device_id):
@@ -1089,29 +1273,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_device_info(
         self,
         request: cloudauth_20190307_models.DescribeDeviceInfoRequest,
     ) -> cloudauth_20190307_models.DescribeDeviceInfoResponse:
+        """
+        @param request: DescribeDeviceInfoRequest
+        @return: DescribeDeviceInfoResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_device_info_with_options(request, runtime)
 
     async def describe_device_info_async(
         self,
         request: cloudauth_20190307_models.DescribeDeviceInfoRequest,
     ) -> cloudauth_20190307_models.DescribeDeviceInfoResponse:
+        """
+        @param request: DescribeDeviceInfoRequest
+        @return: DescribeDeviceInfoResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_device_info_with_options_async(request, runtime)
 
     def describe_face_verify_with_options(
         self,
         request: cloudauth_20190307_models.DescribeFaceVerifyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.DescribeFaceVerifyResponse:
+        """
+        @param request: DescribeFaceVerifyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeFaceVerifyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.certify_id):
             query['CertifyId'] = request.certify_id
         if not UtilClient.is_unset(request.picture_return_type):
             query['PictureReturnType'] = request.picture_return_type
         if not UtilClient.is_unset(request.scene_id):
@@ -1136,14 +1333,19 @@
         )
 
     async def describe_face_verify_with_options_async(
         self,
         request: cloudauth_20190307_models.DescribeFaceVerifyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.DescribeFaceVerifyResponse:
+        """
+        @param request: DescribeFaceVerifyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeFaceVerifyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.certify_id):
             query['CertifyId'] = request.certify_id
         if not UtilClient.is_unset(request.picture_return_type):
             query['PictureReturnType'] = request.picture_return_type
         if not UtilClient.is_unset(request.scene_id):
@@ -1167,28 +1369,41 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_face_verify(
         self,
         request: cloudauth_20190307_models.DescribeFaceVerifyRequest,
     ) -> cloudauth_20190307_models.DescribeFaceVerifyResponse:
+        """
+        @param request: DescribeFaceVerifyRequest
+        @return: DescribeFaceVerifyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_face_verify_with_options(request, runtime)
 
     async def describe_face_verify_async(
         self,
         request: cloudauth_20190307_models.DescribeFaceVerifyRequest,
     ) -> cloudauth_20190307_models.DescribeFaceVerifyResponse:
+        """
+        @param request: DescribeFaceVerifyRequest
+        @return: DescribeFaceVerifyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_face_verify_with_options_async(request, runtime)
 
     def describe_oss_upload_token_with_options(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.DescribeOssUploadTokenResponse:
+        """
+        @param request: DescribeOssUploadTokenRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeOssUploadTokenResponse
+        """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
             action='DescribeOssUploadToken',
             version='2019-03-07',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -1202,14 +1417,19 @@
             self.call_api(params, req, runtime)
         )
 
     async def describe_oss_upload_token_with_options_async(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.DescribeOssUploadTokenResponse:
+        """
+        @param request: DescribeOssUploadTokenRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeOssUploadTokenResponse
+        """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
             action='DescribeOssUploadToken',
             version='2019-03-07',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -1220,26 +1440,39 @@
         )
         return TeaCore.from_map(
             cloudauth_20190307_models.DescribeOssUploadTokenResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_oss_upload_token(self) -> cloudauth_20190307_models.DescribeOssUploadTokenResponse:
+        """
+        @return: DescribeOssUploadTokenResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_oss_upload_token_with_options(runtime)
 
     async def describe_oss_upload_token_async(self) -> cloudauth_20190307_models.DescribeOssUploadTokenResponse:
+        """
+        @return: DescribeOssUploadTokenResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_oss_upload_token_with_options_async(runtime)
 
     def describe_page_face_verify_data_with_options(
         self,
         request: cloudauth_20190307_models.DescribePageFaceVerifyDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.DescribePageFaceVerifyDataResponse:
+        """
+        @summary Open API新增金融级数据统计API
+        
+        @param request: DescribePageFaceVerifyDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribePageFaceVerifyDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.current_page):
             query['CurrentPage'] = request.current_page
         if not UtilClient.is_unset(request.end_date):
             query['EndDate'] = request.end_date
         if not UtilClient.is_unset(request.page_size):
@@ -1270,14 +1503,21 @@
         )
 
     async def describe_page_face_verify_data_with_options_async(
         self,
         request: cloudauth_20190307_models.DescribePageFaceVerifyDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.DescribePageFaceVerifyDataResponse:
+        """
+        @summary Open API新增金融级数据统计API
+        
+        @param request: DescribePageFaceVerifyDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribePageFaceVerifyDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.current_page):
             query['CurrentPage'] = request.current_page
         if not UtilClient.is_unset(request.end_date):
             query['EndDate'] = request.end_date
         if not UtilClient.is_unset(request.page_size):
@@ -1307,29 +1547,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_page_face_verify_data(
         self,
         request: cloudauth_20190307_models.DescribePageFaceVerifyDataRequest,
     ) -> cloudauth_20190307_models.DescribePageFaceVerifyDataResponse:
+        """
+        @summary Open API新增金融级数据统计API
+        
+        @param request: DescribePageFaceVerifyDataRequest
+        @return: DescribePageFaceVerifyDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_page_face_verify_data_with_options(request, runtime)
 
     async def describe_page_face_verify_data_async(
         self,
         request: cloudauth_20190307_models.DescribePageFaceVerifyDataRequest,
     ) -> cloudauth_20190307_models.DescribePageFaceVerifyDataResponse:
+        """
+        @summary Open API新增金融级数据统计API
+        
+        @param request: DescribePageFaceVerifyDataRequest
+        @return: DescribePageFaceVerifyDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_page_face_verify_data_with_options_async(request, runtime)
 
     def describe_smart_statistics_page_list_with_options(
         self,
         request: cloudauth_20190307_models.DescribeSmartStatisticsPageListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.DescribeSmartStatisticsPageListResponse:
+        """
+        @param request: DescribeSmartStatisticsPageListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeSmartStatisticsPageListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.current_page):
             query['CurrentPage'] = request.current_page
         if not UtilClient.is_unset(request.end_date):
             query['EndDate'] = request.end_date
         if not UtilClient.is_unset(request.page_size):
@@ -1360,14 +1617,19 @@
         )
 
     async def describe_smart_statistics_page_list_with_options_async(
         self,
         request: cloudauth_20190307_models.DescribeSmartStatisticsPageListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.DescribeSmartStatisticsPageListResponse:
+        """
+        @param request: DescribeSmartStatisticsPageListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeSmartStatisticsPageListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.current_page):
             query['CurrentPage'] = request.current_page
         if not UtilClient.is_unset(request.end_date):
             query['EndDate'] = request.end_date
         if not UtilClient.is_unset(request.page_size):
@@ -1397,29 +1659,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_smart_statistics_page_list(
         self,
         request: cloudauth_20190307_models.DescribeSmartStatisticsPageListRequest,
     ) -> cloudauth_20190307_models.DescribeSmartStatisticsPageListResponse:
+        """
+        @param request: DescribeSmartStatisticsPageListRequest
+        @return: DescribeSmartStatisticsPageListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_smart_statistics_page_list_with_options(request, runtime)
 
     async def describe_smart_statistics_page_list_async(
         self,
         request: cloudauth_20190307_models.DescribeSmartStatisticsPageListRequest,
     ) -> cloudauth_20190307_models.DescribeSmartStatisticsPageListResponse:
+        """
+        @param request: DescribeSmartStatisticsPageListRequest
+        @return: DescribeSmartStatisticsPageListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_smart_statistics_page_list_with_options_async(request, runtime)
 
     def describe_verify_result_with_options(
         self,
         request: cloudauth_20190307_models.DescribeVerifyResultRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.DescribeVerifyResultResponse:
+        """
+        @param request: DescribeVerifyResultRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeVerifyResultResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.biz_id):
             query['BizId'] = request.biz_id
         if not UtilClient.is_unset(request.biz_type):
             query['BizType'] = request.biz_type
         req = open_api_models.OpenApiRequest(
@@ -1442,14 +1717,19 @@
         )
 
     async def describe_verify_result_with_options_async(
         self,
         request: cloudauth_20190307_models.DescribeVerifyResultRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.DescribeVerifyResultResponse:
+        """
+        @param request: DescribeVerifyResultRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeVerifyResultResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.biz_id):
             query['BizId'] = request.biz_id
         if not UtilClient.is_unset(request.biz_type):
             query['BizType'] = request.biz_type
         req = open_api_models.OpenApiRequest(
@@ -1471,29 +1751,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_verify_result(
         self,
         request: cloudauth_20190307_models.DescribeVerifyResultRequest,
     ) -> cloudauth_20190307_models.DescribeVerifyResultResponse:
+        """
+        @param request: DescribeVerifyResultRequest
+        @return: DescribeVerifyResultResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_verify_result_with_options(request, runtime)
 
     async def describe_verify_result_async(
         self,
         request: cloudauth_20190307_models.DescribeVerifyResultRequest,
     ) -> cloudauth_20190307_models.DescribeVerifyResultResponse:
+        """
+        @param request: DescribeVerifyResultRequest
+        @return: DescribeVerifyResultResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_verify_result_with_options_async(request, runtime)
 
     def describe_verify_sdkwith_options(
         self,
         request: cloudauth_20190307_models.DescribeVerifySDKRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.DescribeVerifySDKResponse:
+        """
+        @param request: DescribeVerifySDKRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeVerifySDKResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.task_id):
             query['TaskId'] = request.task_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -1514,14 +1807,19 @@
         )
 
     async def describe_verify_sdkwith_options_async(
         self,
         request: cloudauth_20190307_models.DescribeVerifySDKRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.DescribeVerifySDKResponse:
+        """
+        @param request: DescribeVerifySDKRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeVerifySDKResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.task_id):
             query['TaskId'] = request.task_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -1541,29 +1839,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_verify_sdk(
         self,
         request: cloudauth_20190307_models.DescribeVerifySDKRequest,
     ) -> cloudauth_20190307_models.DescribeVerifySDKResponse:
+        """
+        @param request: DescribeVerifySDKRequest
+        @return: DescribeVerifySDKResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_verify_sdkwith_options(request, runtime)
 
     async def describe_verify_sdk_async(
         self,
         request: cloudauth_20190307_models.DescribeVerifySDKRequest,
     ) -> cloudauth_20190307_models.DescribeVerifySDKResponse:
+        """
+        @param request: DescribeVerifySDKRequest
+        @return: DescribeVerifySDKResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_verify_sdkwith_options_async(request, runtime)
 
     def describe_verify_token_with_options(
         self,
         request: cloudauth_20190307_models.DescribeVerifyTokenRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.DescribeVerifyTokenResponse:
+        """
+        @param request: DescribeVerifyTokenRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeVerifyTokenResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.biz_id):
             query['BizId'] = request.biz_id
         if not UtilClient.is_unset(request.biz_type):
             query['BizType'] = request.biz_type
         if not UtilClient.is_unset(request.callback_seed):
@@ -1612,14 +1923,19 @@
         )
 
     async def describe_verify_token_with_options_async(
         self,
         request: cloudauth_20190307_models.DescribeVerifyTokenRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.DescribeVerifyTokenResponse:
+        """
+        @param request: DescribeVerifyTokenRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeVerifyTokenResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.biz_id):
             query['BizId'] = request.biz_id
         if not UtilClient.is_unset(request.biz_type):
             query['BizType'] = request.biz_type
         if not UtilClient.is_unset(request.callback_seed):
@@ -1667,29 +1983,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_verify_token(
         self,
         request: cloudauth_20190307_models.DescribeVerifyTokenRequest,
     ) -> cloudauth_20190307_models.DescribeVerifyTokenResponse:
+        """
+        @param request: DescribeVerifyTokenRequest
+        @return: DescribeVerifyTokenResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_verify_token_with_options(request, runtime)
 
     async def describe_verify_token_async(
         self,
         request: cloudauth_20190307_models.DescribeVerifyTokenRequest,
     ) -> cloudauth_20190307_models.DescribeVerifyTokenResponse:
+        """
+        @param request: DescribeVerifyTokenRequest
+        @return: DescribeVerifyTokenResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_verify_token_with_options_async(request, runtime)
 
     def detect_face_attributes_with_options(
         self,
         request: cloudauth_20190307_models.DetectFaceAttributesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.DetectFaceAttributesResponse:
+        """
+        @param request: DetectFaceAttributesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DetectFaceAttributesResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.biz_type):
             body['BizType'] = request.biz_type
         if not UtilClient.is_unset(request.material_value):
             body['MaterialValue'] = request.material_value
         req = open_api_models.OpenApiRequest(
@@ -1712,14 +2041,19 @@
         )
 
     async def detect_face_attributes_with_options_async(
         self,
         request: cloudauth_20190307_models.DetectFaceAttributesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.DetectFaceAttributesResponse:
+        """
+        @param request: DetectFaceAttributesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DetectFaceAttributesResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.biz_type):
             body['BizType'] = request.biz_type
         if not UtilClient.is_unset(request.material_value):
             body['MaterialValue'] = request.material_value
         req = open_api_models.OpenApiRequest(
@@ -1741,29 +2075,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def detect_face_attributes(
         self,
         request: cloudauth_20190307_models.DetectFaceAttributesRequest,
     ) -> cloudauth_20190307_models.DetectFaceAttributesResponse:
+        """
+        @param request: DetectFaceAttributesRequest
+        @return: DetectFaceAttributesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.detect_face_attributes_with_options(request, runtime)
 
     async def detect_face_attributes_async(
         self,
         request: cloudauth_20190307_models.DetectFaceAttributesRequest,
     ) -> cloudauth_20190307_models.DetectFaceAttributesResponse:
+        """
+        @param request: DetectFaceAttributesRequest
+        @return: DetectFaceAttributesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.detect_face_attributes_with_options_async(request, runtime)
 
     def id_2meta_verify_with_options(
         self,
         request: cloudauth_20190307_models.Id2MetaVerifyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.Id2MetaVerifyResponse:
+        """
+        @summary 身份二要素接口
+        
+        @param request: Id2MetaVerifyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: Id2MetaVerifyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.identify_num):
             query['IdentifyNum'] = request.identify_num
         if not UtilClient.is_unset(request.param_type):
             query['ParamType'] = request.param_type
         if not UtilClient.is_unset(request.user_name):
@@ -1788,14 +2137,21 @@
         )
 
     async def id_2meta_verify_with_options_async(
         self,
         request: cloudauth_20190307_models.Id2MetaVerifyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.Id2MetaVerifyResponse:
+        """
+        @summary 身份二要素接口
+        
+        @param request: Id2MetaVerifyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: Id2MetaVerifyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.identify_num):
             query['IdentifyNum'] = request.identify_num
         if not UtilClient.is_unset(request.param_type):
             query['ParamType'] = request.param_type
         if not UtilClient.is_unset(request.user_name):
@@ -1819,29 +2175,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def id_2meta_verify(
         self,
         request: cloudauth_20190307_models.Id2MetaVerifyRequest,
     ) -> cloudauth_20190307_models.Id2MetaVerifyResponse:
+        """
+        @summary 身份二要素接口
+        
+        @param request: Id2MetaVerifyRequest
+        @return: Id2MetaVerifyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.id_2meta_verify_with_options(request, runtime)
 
     async def id_2meta_verify_async(
         self,
         request: cloudauth_20190307_models.Id2MetaVerifyRequest,
     ) -> cloudauth_20190307_models.Id2MetaVerifyResponse:
+        """
+        @summary 身份二要素接口
+        
+        @param request: Id2MetaVerifyRequest
+        @return: Id2MetaVerifyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.id_2meta_verify_with_options_async(request, runtime)
 
     def init_face_verify_with_options(
         self,
         request: cloudauth_20190307_models.InitFaceVerifyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.InitFaceVerifyResponse:
+        """
+        @param request: InitFaceVerifyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: InitFaceVerifyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.birthday):
             query['Birthday'] = request.birthday
         if not UtilClient.is_unset(request.callback_token):
             query['CallbackToken'] = request.callback_token
         if not UtilClient.is_unset(request.callback_url):
@@ -1928,14 +2301,19 @@
         )
 
     async def init_face_verify_with_options_async(
         self,
         request: cloudauth_20190307_models.InitFaceVerifyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.InitFaceVerifyResponse:
+        """
+        @param request: InitFaceVerifyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: InitFaceVerifyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.birthday):
             query['Birthday'] = request.birthday
         if not UtilClient.is_unset(request.callback_token):
             query['CallbackToken'] = request.callback_token
         if not UtilClient.is_unset(request.callback_url):
@@ -2021,29 +2399,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def init_face_verify(
         self,
         request: cloudauth_20190307_models.InitFaceVerifyRequest,
     ) -> cloudauth_20190307_models.InitFaceVerifyResponse:
+        """
+        @param request: InitFaceVerifyRequest
+        @return: InitFaceVerifyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.init_face_verify_with_options(request, runtime)
 
     async def init_face_verify_async(
         self,
         request: cloudauth_20190307_models.InitFaceVerifyRequest,
     ) -> cloudauth_20190307_models.InitFaceVerifyResponse:
+        """
+        @param request: InitFaceVerifyRequest
+        @return: InitFaceVerifyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.init_face_verify_with_options_async(request, runtime)
 
     def liveness_face_verify_with_options(
         self,
         request: cloudauth_20190307_models.LivenessFaceVerifyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.LivenessFaceVerifyResponse:
+        """
+        @param request: LivenessFaceVerifyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: LivenessFaceVerifyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.model):
             query['Model'] = request.model
         body = {}
         if not UtilClient.is_unset(request.certify_id):
             body['CertifyId'] = request.certify_id
@@ -2092,14 +2483,19 @@
         )
 
     async def liveness_face_verify_with_options_async(
         self,
         request: cloudauth_20190307_models.LivenessFaceVerifyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.LivenessFaceVerifyResponse:
+        """
+        @param request: LivenessFaceVerifyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: LivenessFaceVerifyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.model):
             query['Model'] = request.model
         body = {}
         if not UtilClient.is_unset(request.certify_id):
             body['CertifyId'] = request.certify_id
@@ -2147,29 +2543,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def liveness_face_verify(
         self,
         request: cloudauth_20190307_models.LivenessFaceVerifyRequest,
     ) -> cloudauth_20190307_models.LivenessFaceVerifyResponse:
+        """
+        @param request: LivenessFaceVerifyRequest
+        @return: LivenessFaceVerifyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.liveness_face_verify_with_options(request, runtime)
 
     async def liveness_face_verify_async(
         self,
         request: cloudauth_20190307_models.LivenessFaceVerifyRequest,
     ) -> cloudauth_20190307_models.LivenessFaceVerifyResponse:
+        """
+        @param request: LivenessFaceVerifyRequest
+        @return: LivenessFaceVerifyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.liveness_face_verify_with_options_async(request, runtime)
 
     def mobile_3meta_detail_verify_with_options(
         self,
         request: cloudauth_20190307_models.Mobile3MetaDetailVerifyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.Mobile3MetaDetailVerifyResponse:
+        """
+        @summary 手机三要素详版接口
+        
+        @param request: Mobile3MetaDetailVerifyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: Mobile3MetaDetailVerifyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.identify_num):
             query['IdentifyNum'] = request.identify_num
         if not UtilClient.is_unset(request.mobile):
             query['Mobile'] = request.mobile
         if not UtilClient.is_unset(request.param_type):
@@ -2196,14 +2607,21 @@
         )
 
     async def mobile_3meta_detail_verify_with_options_async(
         self,
         request: cloudauth_20190307_models.Mobile3MetaDetailVerifyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.Mobile3MetaDetailVerifyResponse:
+        """
+        @summary 手机三要素详版接口
+        
+        @param request: Mobile3MetaDetailVerifyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: Mobile3MetaDetailVerifyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.identify_num):
             query['IdentifyNum'] = request.identify_num
         if not UtilClient.is_unset(request.mobile):
             query['Mobile'] = request.mobile
         if not UtilClient.is_unset(request.param_type):
@@ -2229,29 +2647,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def mobile_3meta_detail_verify(
         self,
         request: cloudauth_20190307_models.Mobile3MetaDetailVerifyRequest,
     ) -> cloudauth_20190307_models.Mobile3MetaDetailVerifyResponse:
+        """
+        @summary 手机三要素详版接口
+        
+        @param request: Mobile3MetaDetailVerifyRequest
+        @return: Mobile3MetaDetailVerifyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.mobile_3meta_detail_verify_with_options(request, runtime)
 
     async def mobile_3meta_detail_verify_async(
         self,
         request: cloudauth_20190307_models.Mobile3MetaDetailVerifyRequest,
     ) -> cloudauth_20190307_models.Mobile3MetaDetailVerifyResponse:
+        """
+        @summary 手机三要素详版接口
+        
+        @param request: Mobile3MetaDetailVerifyRequest
+        @return: Mobile3MetaDetailVerifyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.mobile_3meta_detail_verify_with_options_async(request, runtime)
 
     def mobile_3meta_simple_verify_with_options(
         self,
         request: cloudauth_20190307_models.Mobile3MetaSimpleVerifyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.Mobile3MetaSimpleVerifyResponse:
+        """
+        @summary 手机号三要素简版接口
+        
+        @param request: Mobile3MetaSimpleVerifyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: Mobile3MetaSimpleVerifyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.identify_num):
             query['IdentifyNum'] = request.identify_num
         if not UtilClient.is_unset(request.mobile):
             query['Mobile'] = request.mobile
         if not UtilClient.is_unset(request.param_type):
@@ -2278,14 +2715,21 @@
         )
 
     async def mobile_3meta_simple_verify_with_options_async(
         self,
         request: cloudauth_20190307_models.Mobile3MetaSimpleVerifyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.Mobile3MetaSimpleVerifyResponse:
+        """
+        @summary 手机号三要素简版接口
+        
+        @param request: Mobile3MetaSimpleVerifyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: Mobile3MetaSimpleVerifyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.identify_num):
             query['IdentifyNum'] = request.identify_num
         if not UtilClient.is_unset(request.mobile):
             query['Mobile'] = request.mobile
         if not UtilClient.is_unset(request.param_type):
@@ -2311,29 +2755,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def mobile_3meta_simple_verify(
         self,
         request: cloudauth_20190307_models.Mobile3MetaSimpleVerifyRequest,
     ) -> cloudauth_20190307_models.Mobile3MetaSimpleVerifyResponse:
+        """
+        @summary 手机号三要素简版接口
+        
+        @param request: Mobile3MetaSimpleVerifyRequest
+        @return: Mobile3MetaSimpleVerifyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.mobile_3meta_simple_verify_with_options(request, runtime)
 
     async def mobile_3meta_simple_verify_async(
         self,
         request: cloudauth_20190307_models.Mobile3MetaSimpleVerifyRequest,
     ) -> cloudauth_20190307_models.Mobile3MetaSimpleVerifyResponse:
+        """
+        @summary 手机号三要素简版接口
+        
+        @param request: Mobile3MetaSimpleVerifyRequest
+        @return: Mobile3MetaSimpleVerifyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.mobile_3meta_simple_verify_with_options_async(request, runtime)
 
     def mobile_detect_with_options(
         self,
         request: cloudauth_20190307_models.MobileDetectRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.MobileDetectResponse:
+        """
+        @summary 号码检测
+        
+        @param request: MobileDetectRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: MobileDetectResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.mobiles):
             query['Mobiles'] = request.mobiles
         if not UtilClient.is_unset(request.param_type):
             query['ParamType'] = request.param_type
         req = open_api_models.OpenApiRequest(
@@ -2356,14 +2819,21 @@
         )
 
     async def mobile_detect_with_options_async(
         self,
         request: cloudauth_20190307_models.MobileDetectRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.MobileDetectResponse:
+        """
+        @summary 号码检测
+        
+        @param request: MobileDetectRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: MobileDetectResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.mobiles):
             query['Mobiles'] = request.mobiles
         if not UtilClient.is_unset(request.param_type):
             query['ParamType'] = request.param_type
         req = open_api_models.OpenApiRequest(
@@ -2385,29 +2855,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def mobile_detect(
         self,
         request: cloudauth_20190307_models.MobileDetectRequest,
     ) -> cloudauth_20190307_models.MobileDetectResponse:
+        """
+        @summary 号码检测
+        
+        @param request: MobileDetectRequest
+        @return: MobileDetectResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.mobile_detect_with_options(request, runtime)
 
     async def mobile_detect_async(
         self,
         request: cloudauth_20190307_models.MobileDetectRequest,
     ) -> cloudauth_20190307_models.MobileDetectResponse:
+        """
+        @summary 号码检测
+        
+        @param request: MobileDetectRequest
+        @return: MobileDetectResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.mobile_detect_with_options_async(request, runtime)
 
     def mobile_online_status_with_options(
         self,
         request: cloudauth_20190307_models.MobileOnlineStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.MobileOnlineStatusResponse:
+        """
+        @summary 查询手机号在网状态
+        
+        @param request: MobileOnlineStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: MobileOnlineStatusResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.mobile):
             query['Mobile'] = request.mobile
         if not UtilClient.is_unset(request.param_type):
             query['ParamType'] = request.param_type
         req = open_api_models.OpenApiRequest(
@@ -2430,14 +2919,21 @@
         )
 
     async def mobile_online_status_with_options_async(
         self,
         request: cloudauth_20190307_models.MobileOnlineStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.MobileOnlineStatusResponse:
+        """
+        @summary 查询手机号在网状态
+        
+        @param request: MobileOnlineStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: MobileOnlineStatusResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.mobile):
             query['Mobile'] = request.mobile
         if not UtilClient.is_unset(request.param_type):
             query['ParamType'] = request.param_type
         req = open_api_models.OpenApiRequest(
@@ -2459,29 +2955,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def mobile_online_status(
         self,
         request: cloudauth_20190307_models.MobileOnlineStatusRequest,
     ) -> cloudauth_20190307_models.MobileOnlineStatusResponse:
+        """
+        @summary 查询手机号在网状态
+        
+        @param request: MobileOnlineStatusRequest
+        @return: MobileOnlineStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.mobile_online_status_with_options(request, runtime)
 
     async def mobile_online_status_async(
         self,
         request: cloudauth_20190307_models.MobileOnlineStatusRequest,
     ) -> cloudauth_20190307_models.MobileOnlineStatusResponse:
+        """
+        @summary 查询手机号在网状态
+        
+        @param request: MobileOnlineStatusRequest
+        @return: MobileOnlineStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.mobile_online_status_with_options_async(request, runtime)
 
     def mobile_online_time_with_options(
         self,
         request: cloudauth_20190307_models.MobileOnlineTimeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.MobileOnlineTimeResponse:
+        """
+        @summary 查询手机号在网时长
+        
+        @param request: MobileOnlineTimeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: MobileOnlineTimeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.mobile):
             query['Mobile'] = request.mobile
         if not UtilClient.is_unset(request.param_type):
             query['ParamType'] = request.param_type
         req = open_api_models.OpenApiRequest(
@@ -2504,14 +3019,21 @@
         )
 
     async def mobile_online_time_with_options_async(
         self,
         request: cloudauth_20190307_models.MobileOnlineTimeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.MobileOnlineTimeResponse:
+        """
+        @summary 查询手机号在网时长
+        
+        @param request: MobileOnlineTimeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: MobileOnlineTimeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.mobile):
             query['Mobile'] = request.mobile
         if not UtilClient.is_unset(request.param_type):
             query['ParamType'] = request.param_type
         req = open_api_models.OpenApiRequest(
@@ -2533,29 +3055,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def mobile_online_time(
         self,
         request: cloudauth_20190307_models.MobileOnlineTimeRequest,
     ) -> cloudauth_20190307_models.MobileOnlineTimeResponse:
+        """
+        @summary 查询手机号在网时长
+        
+        @param request: MobileOnlineTimeRequest
+        @return: MobileOnlineTimeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.mobile_online_time_with_options(request, runtime)
 
     async def mobile_online_time_async(
         self,
         request: cloudauth_20190307_models.MobileOnlineTimeRequest,
     ) -> cloudauth_20190307_models.MobileOnlineTimeResponse:
+        """
+        @summary 查询手机号在网时长
+        
+        @param request: MobileOnlineTimeRequest
+        @return: MobileOnlineTimeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.mobile_online_time_with_options_async(request, runtime)
 
     def modify_device_info_with_options(
         self,
         request: cloudauth_20190307_models.ModifyDeviceInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.ModifyDeviceInfoResponse:
+        """
+        @param request: ModifyDeviceInfoRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDeviceInfoResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.biz_type):
             query['BizType'] = request.biz_type
         if not UtilClient.is_unset(request.device_id):
             query['DeviceId'] = request.device_id
         if not UtilClient.is_unset(request.duration):
@@ -2584,14 +3123,19 @@
         )
 
     async def modify_device_info_with_options_async(
         self,
         request: cloudauth_20190307_models.ModifyDeviceInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.ModifyDeviceInfoResponse:
+        """
+        @param request: ModifyDeviceInfoRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDeviceInfoResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.biz_type):
             query['BizType'] = request.biz_type
         if not UtilClient.is_unset(request.device_id):
             query['DeviceId'] = request.device_id
         if not UtilClient.is_unset(request.duration):
@@ -2619,29 +3163,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_device_info(
         self,
         request: cloudauth_20190307_models.ModifyDeviceInfoRequest,
     ) -> cloudauth_20190307_models.ModifyDeviceInfoResponse:
+        """
+        @param request: ModifyDeviceInfoRequest
+        @return: ModifyDeviceInfoResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_device_info_with_options(request, runtime)
 
     async def modify_device_info_async(
         self,
         request: cloudauth_20190307_models.ModifyDeviceInfoRequest,
     ) -> cloudauth_20190307_models.ModifyDeviceInfoResponse:
+        """
+        @param request: ModifyDeviceInfoRequest
+        @return: ModifyDeviceInfoResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_device_info_with_options_async(request, runtime)
 
     def verify_material_with_options(
         self,
         request: cloudauth_20190307_models.VerifyMaterialRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.VerifyMaterialResponse:
+        """
+        @param request: VerifyMaterialRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: VerifyMaterialResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.biz_id):
             query['BizId'] = request.biz_id
         if not UtilClient.is_unset(request.biz_type):
             query['BizType'] = request.biz_type
         if not UtilClient.is_unset(request.face_image_url):
@@ -2676,14 +3233,19 @@
         )
 
     async def verify_material_with_options_async(
         self,
         request: cloudauth_20190307_models.VerifyMaterialRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.VerifyMaterialResponse:
+        """
+        @param request: VerifyMaterialRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: VerifyMaterialResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.biz_id):
             query['BizId'] = request.biz_id
         if not UtilClient.is_unset(request.biz_type):
             query['BizType'] = request.biz_type
         if not UtilClient.is_unset(request.face_image_url):
@@ -2717,16 +3279,24 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def verify_material(
         self,
         request: cloudauth_20190307_models.VerifyMaterialRequest,
     ) -> cloudauth_20190307_models.VerifyMaterialResponse:
+        """
+        @param request: VerifyMaterialRequest
+        @return: VerifyMaterialResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.verify_material_with_options(request, runtime)
 
     async def verify_material_async(
         self,
         request: cloudauth_20190307_models.VerifyMaterialRequest,
     ) -> cloudauth_20190307_models.VerifyMaterialResponse:
+        """
+        @param request: VerifyMaterialRequest
+        @return: VerifyMaterialResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.verify_material_with_options_async(request, runtime)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alibabacloud_cloudauth20190307-2.6.0/alibabacloud_cloudauth20190307/models.py` & `alibabacloud_cloudauth20190307-2.6.1/alibabacloud_cloudauth20190307/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1316,19 +1316,22 @@
         biz_name: str = None,
         biz_type: str = None,
         guide_step: bool = None,
         privacy_step: bool = None,
         result_step: bool = None,
         solution: str = None,
     ):
+        # This parameter is required.
         self.biz_name = biz_name
+        # This parameter is required.
         self.biz_type = biz_type
         self.guide_step = guide_step
         self.privacy_step = privacy_step
         self.result_step = result_step
+        # This parameter is required.
         self.solution = solution
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1466,24 +1469,26 @@
         cred_name: str = None,
         cred_type: str = None,
         identify_num: str = None,
         image_context: str = None,
         image_url: str = None,
         is_check: str = None,
         is_ocr: str = None,
+        merchant_id: str = None,
         user_name: str = None,
     ):
         self.cert_num = cert_num
         self.cred_name = cred_name
         self.cred_type = cred_type
         self.identify_num = identify_num
         self.image_context = image_context
         self.image_url = image_url
         self.is_check = is_check
         self.is_ocr = is_ocr
+        self.merchant_id = merchant_id
         self.user_name = user_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1503,14 +1508,16 @@
             result['ImageContext'] = self.image_context
         if self.image_url is not None:
             result['ImageUrl'] = self.image_url
         if self.is_check is not None:
             result['IsCheck'] = self.is_check
         if self.is_ocr is not None:
             result['IsOCR'] = self.is_ocr
+        if self.merchant_id is not None:
+            result['MerchantId'] = self.merchant_id
         if self.user_name is not None:
             result['UserName'] = self.user_name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('CertNum') is not None:
@@ -1525,29 +1532,33 @@
             self.image_context = m.get('ImageContext')
         if m.get('ImageUrl') is not None:
             self.image_url = m.get('ImageUrl')
         if m.get('IsCheck') is not None:
             self.is_check = m.get('IsCheck')
         if m.get('IsOCR') is not None:
             self.is_ocr = m.get('IsOCR')
+        if m.get('MerchantId') is not None:
+            self.merchant_id = m.get('MerchantId')
         if m.get('UserName') is not None:
             self.user_name = m.get('UserName')
         return self
 
 
 class CredentialVerifyResponseBodyResultObject(TeaModel):
     def __init__(
         self,
+        material_info: str = None,
         ocr_info: str = None,
         result: str = None,
         risk_score: Dict[str, str] = None,
         risk_tag: str = None,
         verify_detail: str = None,
         verify_result: str = None,
     ):
+        self.material_info = material_info
         self.ocr_info = ocr_info
         self.result = result
         self.risk_score = risk_score
         self.risk_tag = risk_tag
         self.verify_detail = verify_detail
         self.verify_result = verify_result
 
@@ -1556,14 +1567,16 @@
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.material_info is not None:
+            result['MaterialInfo'] = self.material_info
         if self.ocr_info is not None:
             result['OcrInfo'] = self.ocr_info
         if self.result is not None:
             result['Result'] = self.result
         if self.risk_score is not None:
             result['RiskScore'] = self.risk_score
         if self.risk_tag is not None:
@@ -1572,14 +1585,16 @@
             result['VerifyDetail'] = self.verify_detail
         if self.verify_result is not None:
             result['VerifyResult'] = self.verify_result
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('MaterialInfo') is not None:
+            self.material_info = m.get('MaterialInfo')
         if m.get('OcrInfo') is not None:
             self.ocr_info = m.get('OcrInfo')
         if m.get('Result') is not None:
             self.result = m.get('Result')
         if m.get('RiskScore') is not None:
             self.risk_score = m.get('RiskScore')
         if m.get('RiskTag') is not None:
@@ -2501,19 +2516,24 @@
         current_page: str = None,
         end_date: str = None,
         page_size: str = None,
         scene_id: str = None,
         service_code: str = None,
         start_date: str = None,
     ):
+        # This parameter is required.
         self.current_page = current_page
+        # This parameter is required.
         self.end_date = end_date
+        # This parameter is required.
         self.page_size = page_size
+        # This parameter is required.
         self.scene_id = scene_id
         self.service_code = service_code
+        # This parameter is required.
         self.start_date = start_date
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2723,15 +2743,17 @@
 
 class DescribeVerifyResultRequest(TeaModel):
     def __init__(
         self,
         biz_id: str = None,
         biz_type: str = None,
     ):
+        # This parameter is required.
         self.biz_id = biz_id
+        # This parameter is required.
         self.biz_type = biz_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3007,14 +3029,15 @@
 
 
 class DescribeVerifySDKRequest(TeaModel):
     def __init__(
         self,
         task_id: str = None,
     ):
+        # This parameter is required.
         self.task_id = task_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3122,15 +3145,17 @@
         name: str = None,
         passed_redirect_url: str = None,
         user_id: str = None,
         user_ip: str = None,
         user_phone_number: str = None,
         user_regist_time: int = None,
     ):
+        # This parameter is required.
         self.biz_id = biz_id
+        # This parameter is required.
         self.biz_type = biz_type
         self.callback_seed = callback_seed
         self.callback_url = callback_url
         self.face_retained_image_url = face_retained_image_url
         self.failed_redirect_url = failed_redirect_url
         self.id_card_back_image_url = id_card_back_image_url
         self.id_card_front_image_url = id_card_front_image_url
@@ -3372,14 +3397,15 @@
 class DetectFaceAttributesRequest(TeaModel):
     def __init__(
         self,
         biz_type: str = None,
         material_value: str = None,
     ):
         self.biz_type = biz_type
+        # This parameter is required.
         self.material_value = material_value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5410,14 +5436,15 @@
         biz_type: str = None,
         device_id: str = None,
         duration: str = None,
         expired_day: str = None,
         user_device_id: str = None,
     ):
         self.biz_type = biz_type
+        # This parameter is required.
         self.device_id = device_id
         self.duration = duration
         self.expired_day = expired_day
         self.user_device_id = user_device_id
 
     def validate(self):
         pass
@@ -5561,20 +5588,25 @@
         face_image_url: str = None,
         id_card_back_image_url: str = None,
         id_card_front_image_url: str = None,
         id_card_number: str = None,
         name: str = None,
         user_id: str = None,
     ):
+        # This parameter is required.
         self.biz_id = biz_id
+        # This parameter is required.
         self.biz_type = biz_type
+        # This parameter is required.
         self.face_image_url = face_image_url
         self.id_card_back_image_url = id_card_back_image_url
         self.id_card_front_image_url = id_card_front_image_url
+        # This parameter is required.
         self.id_card_number = id_card_number
+        # This parameter is required.
         self.name = name
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
```

### Comparing `alibabacloud_cloudauth20190307-2.6.0/alibabacloud_cloudauth20190307.egg-info/PKG-INFO` & `alibabacloud_cloudauth20190307-2.6.1/alibabacloud_cloudauth20190307.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cloudauth20190307
-Version: 2.6.0
+Version: 2.6.1
 Summary: Alibaba Cloud ID Verification (20190307) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloudauth20190307-2.6.0/setup.py` & `alibabacloud_cloudauth20190307-2.6.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,33 +20,33 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cloudauth20190307.
 
-Created on 26/04/2024
+Created on 30/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cloudauth20190307"
 NAME = "alibabacloud_cloudauth20190307" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ID Verification (20190307) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.11, <1.0.0",
+    "alibabacloud_tea_util>=0.3.12, <1.0.0",
     "alibabacloud_oss_sdk>=0.1.0, <1.0.0",
     "alibabacloud_openplatform20191219>=2.0.0, <3.0.0",
     "alibabacloud_oss_util>=0.0.5, <1.0.0",
     "alibabacloud_tea_fileform>=0.0.3, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.8, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.9, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
```

