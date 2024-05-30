# Comparing `tmp/aliyun-python-sdk-cams-1.0.8.tar.gz` & `tmp/aliyun-python-sdk-cams-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-cams-1.0.8.tar", last modified: Thu Oct 19 07:11:41 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-cams-1.0.9.tar", last modified: Thu Apr 11 01:18:15 2024, max compression
```

## Comparing `aliyun-python-sdk-cams-1.0.8.tar` & `aliyun-python-sdk-cams-1.0.9.tar`

### file list

```diff
@@ -1,61 +1,78 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      575 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1542 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      529 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyun_python_sdk_cams.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1542 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyun_python_sdk_cams.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3055 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyun_python_sdk_cams.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyun_python_sdk_cams.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyun_python_sdk_cams.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyun_python_sdk_cams.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/
--rw-r--r--   0 root         (0) root         (0)       21 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1088 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/
--rw-r--r--   0 root         (0) root         (0)     2231 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/AddChatappPhoneNumberRequest.py
--rw-r--r--   0 root         (0) root         (0)     2643 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/BeeBotAssociateRequest.py
--rw-r--r--   0 root         (0) root         (0)     3407 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/BeeBotChatRequest.py
--rw-r--r--   0 root         (0) root         (0)     1441 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/ChatappBindWabaRequest.py
--rw-r--r--   0 root         (0) root         (0)     1471 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/ChatappEmbedSignUpRequest.py
--rw-r--r--   0 root         (0) root         (0)     1687 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/ChatappMigrationRegisterRequest.py
--rw-r--r--   0 root         (0) root         (0)     1878 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/ChatappMigrationVerifiedRequest.py
--rw-r--r--   0 root         (0) root         (0)     1693 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/ChatappPhoneNumberDeregisterRequest.py
--rw-r--r--   0 root         (0) root         (0)     1689 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/ChatappPhoneNumberRegisterRequest.py
--rw-r--r--   0 root         (0) root         (0)     1486 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/ChatappSyncPhoneNumberRequest.py
--rw-r--r--   0 root         (0) root         (0)     1875 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/ChatappVerifyAndRegisterRequest.py
--rw-r--r--   0 root         (0) root         (0)     1902 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/CreateChatappMigrationInitiateRequest.py
--rw-r--r--   0 root         (0) root         (0)     3451 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/CreateChatappTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     2051 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/DeleteChatappTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     1661 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/EnableWhatsappROIMetricRequest.py
--rw-r--r--   0 root         (0) root         (0)     2365 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/GetChatappPhoneNumberMetricRequest.py
--rw-r--r--   0 root         (0) root         (0)     2439 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/GetChatappTemplateDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     2747 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/GetChatappTemplateMetricRequest.py
--rw-r--r--   0 root         (0) root         (0)     1500 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/GetChatappUploadAuthorizationRequest.py
--rw-r--r--   0 root         (0) root         (0)     2009 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/GetChatappVerifyCodeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1675 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/GetCommerceSettingRequest.py
--rw-r--r--   0 root         (0) root         (0)     2017 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/GetMigrationVerifyCodeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1701 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/GetPhoneNumberVerificationStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1673 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/GetPreValidatePhoneIdRequest.py
--rw-r--r--   0 root         (0) root         (0)     2302 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/GetWhatsappConnectionCatalogRequest.py
--rw-r--r--   0 root         (0) root         (0)     1421 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/IsvGetAppIdRequest.py
--rw-r--r--   0 root         (0) root         (0)     2757 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/ListChatappTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     2954 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/ListProductCatalogRequest.py
--rw-r--r--   0 root         (0) root         (0)     3105 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/ListProductRequest.py
--rw-r--r--   0 root         (0) root         (0)     3253 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/ModifyChatappTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     2835 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/ModifyPhoneBusinessProfileRequest.py
--rw-r--r--   0 root         (0) root         (0)     1655 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/QueryChatappBindWabaRequest.py
--rw-r--r--   0 root         (0) root         (0)     1663 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/QueryChatappPhoneNumbersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1689 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/QueryPhoneBusinessProfileRequest.py
--rw-r--r--   0 root         (0) root         (0)     1651 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/QueryWabaBusinessInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     4249 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/SendChatappMassMessageRequest.py
--rw-r--r--   0 root         (0) root         (0)     5763 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/SendChatappMessageRequest.py
--rw-r--r--   0 root         (0) root         (0)     2638 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/SubmitIsvCustomerTermsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2079 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/UpdateAccountWebhookRequest.py
--rw-r--r--   0 root         (0) root         (0)     2091 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/UpdateCommerceSettingRequest.py
--rw-r--r--   0 root         (0) root         (0)     2481 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/UpdatePhoneWebhookRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2457 2023-10-19 07:11:41.000000 aliyun-python-sdk-cams-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      575 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1542 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      529 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyun_python_sdk_cams.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1542 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyun_python_sdk_cams.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4070 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyun_python_sdk_cams.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyun_python_sdk_cams.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyun_python_sdk_cams.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyun_python_sdk_cams.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/
+-rw-r--r--   0 root         (0) root         (0)     2231 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/AddChatappPhoneNumberRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2643 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/BeeBotAssociateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3407 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/BeeBotChatRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/ChatappBindWabaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1471 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/ChatappEmbedSignUpRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1687 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/ChatappMigrationRegisterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1878 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/ChatappMigrationVerifiedRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1693 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/ChatappPhoneNumberDeregisterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/ChatappPhoneNumberRegisterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1486 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/ChatappSyncPhoneNumberRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1875 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/ChatappVerifyAndRegisterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1902 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/CreateChatappMigrationInitiateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3451 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/CreateChatappTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1851 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/CreateFlowRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2127 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/CreatePhoneMessageQrdlRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2636 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/DeleteChatappTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2057 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/DeleteFlowRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1859 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/DeletePhoneMessageQrdlRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1633 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/DeprecateFlowRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1661 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/EnableWhatsappROIMetricRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2365 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/GetChatappPhoneNumberMetricRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2642 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/GetChatappTemplateDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2747 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/GetChatappTemplateMetricRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/GetChatappUploadAuthorizationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2009 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/GetChatappVerifyCodeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1675 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/GetCommerceSettingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1641 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/GetFlowJSONAssestRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1641 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/GetFlowPreviewUrlRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1621 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/GetFlowRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2017 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/GetMigrationVerifyCodeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1851 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/GetPermissionByCodeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1691 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/GetPhoneEncryptionPublicKeyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/GetPhoneNumberVerificationStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1673 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/GetPreValidatePhoneIdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2302 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/GetWhatsappConnectionCatalogRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1617 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/IsvGetAppIdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2757 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/ListChatappTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2403 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/ListFlowRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1677 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/ListPhoneMessageQrdlRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2954 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/ListProductCatalogRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3105 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/ListProductRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3455 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/ModifyChatappTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2017 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/ModifyFlowRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2996 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/ModifyPhoneBusinessProfileRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1629 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/PublishFlowRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1655 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/QueryChatappBindWabaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1830 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/QueryChatappPhoneNumbersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/QueryPhoneBusinessProfileRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1651 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/QueryWabaBusinessInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4451 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/SendChatappMassMessageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     6167 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/SendChatappMessageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2638 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/SubmitIsvCustomerTermsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2079 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/UpdateAccountWebhookRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2091 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/UpdateCommerceSettingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1823 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/UpdateFlowJSONAssetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1941 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/UpdatePhoneEncryptionPublicKeyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2305 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/UpdatePhoneMessageQrdlRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2481 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/UpdatePhoneWebhookRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-04-11 01:18:15.000000 aliyun-python-sdk-cams-1.0.9/setup.py
```

### Comparing `aliyun-python-sdk-cams-1.0.8/LICENSE` & `aliyun-python-sdk-cams-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.8/PKG-INFO` & `aliyun-python-sdk-cams-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-cams
-Version: 1.0.8
+Version: 1.0.9
 Summary: The cams module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-cams
```

### Comparing `aliyun-python-sdk-cams-1.0.8/README.rst` & `aliyun-python-sdk-cams-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyun_python_sdk_cams.egg-info/PKG-INFO` & `aliyun-python-sdk-cams-1.0.9/aliyun_python_sdk_cams.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-cams
-Version: 1.0.8
+Version: 1.0.9
 Summary: The cams module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-cams
```

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyun_python_sdk_cams.egg-info/SOURCES.txt` & `aliyun-python-sdk-cams-1.0.9/aliyun_python_sdk_cams.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -20,36 +20,53 @@
 aliyunsdkcams/request/v20200606/ChatappMigrationVerifiedRequest.py
 aliyunsdkcams/request/v20200606/ChatappPhoneNumberDeregisterRequest.py
 aliyunsdkcams/request/v20200606/ChatappPhoneNumberRegisterRequest.py
 aliyunsdkcams/request/v20200606/ChatappSyncPhoneNumberRequest.py
 aliyunsdkcams/request/v20200606/ChatappVerifyAndRegisterRequest.py
 aliyunsdkcams/request/v20200606/CreateChatappMigrationInitiateRequest.py
 aliyunsdkcams/request/v20200606/CreateChatappTemplateRequest.py
+aliyunsdkcams/request/v20200606/CreateFlowRequest.py
+aliyunsdkcams/request/v20200606/CreatePhoneMessageQrdlRequest.py
 aliyunsdkcams/request/v20200606/DeleteChatappTemplateRequest.py
+aliyunsdkcams/request/v20200606/DeleteFlowRequest.py
+aliyunsdkcams/request/v20200606/DeletePhoneMessageQrdlRequest.py
+aliyunsdkcams/request/v20200606/DeprecateFlowRequest.py
 aliyunsdkcams/request/v20200606/EnableWhatsappROIMetricRequest.py
 aliyunsdkcams/request/v20200606/GetChatappPhoneNumberMetricRequest.py
 aliyunsdkcams/request/v20200606/GetChatappTemplateDetailRequest.py
 aliyunsdkcams/request/v20200606/GetChatappTemplateMetricRequest.py
 aliyunsdkcams/request/v20200606/GetChatappUploadAuthorizationRequest.py
 aliyunsdkcams/request/v20200606/GetChatappVerifyCodeRequest.py
 aliyunsdkcams/request/v20200606/GetCommerceSettingRequest.py
+aliyunsdkcams/request/v20200606/GetFlowJSONAssestRequest.py
+aliyunsdkcams/request/v20200606/GetFlowPreviewUrlRequest.py
+aliyunsdkcams/request/v20200606/GetFlowRequest.py
 aliyunsdkcams/request/v20200606/GetMigrationVerifyCodeRequest.py
+aliyunsdkcams/request/v20200606/GetPermissionByCodeRequest.py
+aliyunsdkcams/request/v20200606/GetPhoneEncryptionPublicKeyRequest.py
 aliyunsdkcams/request/v20200606/GetPhoneNumberVerificationStatusRequest.py
 aliyunsdkcams/request/v20200606/GetPreValidatePhoneIdRequest.py
 aliyunsdkcams/request/v20200606/GetWhatsappConnectionCatalogRequest.py
 aliyunsdkcams/request/v20200606/IsvGetAppIdRequest.py
 aliyunsdkcams/request/v20200606/ListChatappTemplateRequest.py
+aliyunsdkcams/request/v20200606/ListFlowRequest.py
+aliyunsdkcams/request/v20200606/ListPhoneMessageQrdlRequest.py
 aliyunsdkcams/request/v20200606/ListProductCatalogRequest.py
 aliyunsdkcams/request/v20200606/ListProductRequest.py
 aliyunsdkcams/request/v20200606/ModifyChatappTemplateRequest.py
+aliyunsdkcams/request/v20200606/ModifyFlowRequest.py
 aliyunsdkcams/request/v20200606/ModifyPhoneBusinessProfileRequest.py
+aliyunsdkcams/request/v20200606/PublishFlowRequest.py
 aliyunsdkcams/request/v20200606/QueryChatappBindWabaRequest.py
 aliyunsdkcams/request/v20200606/QueryChatappPhoneNumbersRequest.py
 aliyunsdkcams/request/v20200606/QueryPhoneBusinessProfileRequest.py
 aliyunsdkcams/request/v20200606/QueryWabaBusinessInfoRequest.py
 aliyunsdkcams/request/v20200606/SendChatappMassMessageRequest.py
 aliyunsdkcams/request/v20200606/SendChatappMessageRequest.py
 aliyunsdkcams/request/v20200606/SubmitIsvCustomerTermsRequest.py
 aliyunsdkcams/request/v20200606/UpdateAccountWebhookRequest.py
 aliyunsdkcams/request/v20200606/UpdateCommerceSettingRequest.py
+aliyunsdkcams/request/v20200606/UpdateFlowJSONAssetRequest.py
+aliyunsdkcams/request/v20200606/UpdatePhoneEncryptionPublicKeyRequest.py
+aliyunsdkcams/request/v20200606/UpdatePhoneMessageQrdlRequest.py
 aliyunsdkcams/request/v20200606/UpdatePhoneWebhookRequest.py
 aliyunsdkcams/request/v20200606/__init__.py
```

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/endpoint.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/AddChatappPhoneNumberRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/AddChatappPhoneNumberRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/BeeBotAssociateRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/BeeBotAssociateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/BeeBotChatRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/BeeBotChatRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/ChatappBindWabaRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/ChatappBindWabaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/ChatappEmbedSignUpRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/ChatappEmbedSignUpRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/ChatappMigrationRegisterRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/ChatappMigrationRegisterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/ChatappMigrationVerifiedRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/ChatappMigrationVerifiedRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/ChatappPhoneNumberDeregisterRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/ChatappPhoneNumberDeregisterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/ChatappPhoneNumberRegisterRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/ChatappPhoneNumberRegisterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/ChatappSyncPhoneNumberRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/ChatappSyncPhoneNumberRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/ChatappVerifyAndRegisterRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/ChatappVerifyAndRegisterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/CreateChatappMigrationInitiateRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/CreateChatappMigrationInitiateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/CreateChatappTemplateRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/CreateChatappTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/DeleteChatappTemplateRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/QueryChatappPhoneNumbersRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,38 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkcams.endpoint import endpoint_data
 
-class DeleteChatappTemplateRequest(RpcRequest):
+class QueryChatappPhoneNumbersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'cams', '2020-06-06', 'DeleteChatappTemplate','cams')
+		RpcRequest.__init__(self, 'cams', '2020-06-06', 'QueryChatappPhoneNumbers','cams')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_CustWabaId(self): # String
-		return self.get_query_params().get('CustWabaId')
-
-	def set_CustWabaId(self, CustWabaId):  # String
-		self.add_query_param('CustWabaId', CustWabaId)
 	def get_IsvCode(self): # String
 		return self.get_query_params().get('IsvCode')
 
 	def set_IsvCode(self, IsvCode):  # String
 		self.add_query_param('IsvCode', IsvCode)
 	def get_CustSpaceId(self): # String
 		return self.get_query_params().get('CustSpaceId')
 
 	def set_CustSpaceId(self, CustSpaceId):  # String
 		self.add_query_param('CustSpaceId', CustSpaceId)
-	def get_TemplateCode(self): # String
-		return self.get_query_params().get('TemplateCode')
+	def get_Status(self): # String
+		return self.get_query_params().get('Status')
 
-	def set_TemplateCode(self, TemplateCode):  # String
-		self.add_query_param('TemplateCode', TemplateCode)
+	def set_Status(self, Status):  # String
+		self.add_query_param('Status', Status)
```

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/EnableWhatsappROIMetricRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/EnableWhatsappROIMetricRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/GetChatappPhoneNumberMetricRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/GetChatappPhoneNumberMetricRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/GetChatappTemplateDetailRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/GetChatappTemplateMetricRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,48 +16,58 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkcams.endpoint import endpoint_data
 
-class GetChatappTemplateDetailRequest(RpcRequest):
+class GetChatappTemplateMetricRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'cams', '2020-06-06', 'GetChatappTemplateDetail','cams')
+		RpcRequest.__init__(self, 'cams', '2020-06-06', 'GetChatappTemplateMetric','cams')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_Language(self): # String
 		return self.get_query_params().get('Language')
 
 	def set_Language(self, Language):  # String
 		self.add_query_param('Language', Language)
-	def get_CustWabaId(self): # String
-		return self.get_query_params().get('CustWabaId')
-
-	def set_CustWabaId(self, CustWabaId):  # String
-		self.add_query_param('CustWabaId', CustWabaId)
 	def get_TemplateType(self): # String
 		return self.get_query_params().get('TemplateType')
 
 	def set_TemplateType(self, TemplateType):  # String
 		self.add_query_param('TemplateType', TemplateType)
+	def get_End(self): # Long
+		return self.get_query_params().get('End')
+
+	def set_End(self, End):  # Long
+		self.add_query_param('End', End)
 	def get_IsvCode(self): # String
 		return self.get_query_params().get('IsvCode')
 
 	def set_IsvCode(self, IsvCode):  # String
 		self.add_query_param('IsvCode', IsvCode)
+	def get_Start(self): # Long
+		return self.get_query_params().get('Start')
+
+	def set_Start(self, Start):  # Long
+		self.add_query_param('Start', Start)
 	def get_CustSpaceId(self): # String
 		return self.get_query_params().get('CustSpaceId')
 
 	def set_CustSpaceId(self, CustSpaceId):  # String
 		self.add_query_param('CustSpaceId', CustSpaceId)
+	def get_Granularity(self): # String
+		return self.get_query_params().get('Granularity')
+
+	def set_Granularity(self, Granularity):  # String
+		self.add_query_param('Granularity', Granularity)
 	def get_TemplateCode(self): # String
 		return self.get_query_params().get('TemplateCode')
 
 	def set_TemplateCode(self, TemplateCode):  # String
 		self.add_query_param('TemplateCode', TemplateCode)
```

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/GetChatappTemplateMetricRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/GetChatappTemplateDetailRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,58 +16,53 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkcams.endpoint import endpoint_data
 
-class GetChatappTemplateMetricRequest(RpcRequest):
+class GetChatappTemplateDetailRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'cams', '2020-06-06', 'GetChatappTemplateMetric','cams')
+		RpcRequest.__init__(self, 'cams', '2020-06-06', 'GetChatappTemplateDetail','cams')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_Language(self): # String
 		return self.get_query_params().get('Language')
 
 	def set_Language(self, Language):  # String
 		self.add_query_param('Language', Language)
+	def get_CustWabaId(self): # String
+		return self.get_query_params().get('CustWabaId')
+
+	def set_CustWabaId(self, CustWabaId):  # String
+		self.add_query_param('CustWabaId', CustWabaId)
 	def get_TemplateType(self): # String
 		return self.get_query_params().get('TemplateType')
 
 	def set_TemplateType(self, TemplateType):  # String
 		self.add_query_param('TemplateType', TemplateType)
-	def get_End(self): # Long
-		return self.get_query_params().get('End')
+	def get_TemplateName(self): # String
+		return self.get_query_params().get('TemplateName')
 
-	def set_End(self, End):  # Long
-		self.add_query_param('End', End)
+	def set_TemplateName(self, TemplateName):  # String
+		self.add_query_param('TemplateName', TemplateName)
 	def get_IsvCode(self): # String
 		return self.get_query_params().get('IsvCode')
 
 	def set_IsvCode(self, IsvCode):  # String
 		self.add_query_param('IsvCode', IsvCode)
-	def get_Start(self): # Long
-		return self.get_query_params().get('Start')
-
-	def set_Start(self, Start):  # Long
-		self.add_query_param('Start', Start)
 	def get_CustSpaceId(self): # String
 		return self.get_query_params().get('CustSpaceId')
 
 	def set_CustSpaceId(self, CustSpaceId):  # String
 		self.add_query_param('CustSpaceId', CustSpaceId)
-	def get_Granularity(self): # String
-		return self.get_query_params().get('Granularity')
-
-	def set_Granularity(self, Granularity):  # String
-		self.add_query_param('Granularity', Granularity)
 	def get_TemplateCode(self): # String
 		return self.get_query_params().get('TemplateCode')
 
 	def set_TemplateCode(self, TemplateCode):  # String
 		self.add_query_param('TemplateCode', TemplateCode)
```

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/GetChatappUploadAuthorizationRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/GetChatappUploadAuthorizationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/GetChatappVerifyCodeRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/GetChatappVerifyCodeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/GetCommerceSettingRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/GetCommerceSettingRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/GetMigrationVerifyCodeRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/GetMigrationVerifyCodeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/GetPhoneNumberVerificationStatusRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/GetPhoneNumberVerificationStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/GetPreValidatePhoneIdRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/GetPreValidatePhoneIdRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/GetWhatsappConnectionCatalogRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/GetWhatsappConnectionCatalogRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/IsvGetAppIdRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/IsvGetAppIdRequest.py`

 * *Files 17% similar despite different names*

```diff
@@ -32,7 +32,12 @@
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_Type(self): # String
 		return self.get_body_params().get('Type')
 
 	def set_Type(self, Type):  # String
 		self.add_body_params('Type', Type)
+	def get_Permissions(self): # String
+		return self.get_body_params().get('Permissions')
+
+	def set_Permissions(self, Permissions):  # String
+		self.add_body_params('Permissions', Permissions)
```

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/ListChatappTemplateRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/ListChatappTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/ListProductCatalogRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/ListProductCatalogRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/ListProductRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/ListProductRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/ModifyChatappTemplateRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/ModifyChatappTemplateRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,19 @@
 	def set_Example(self, Example):  # Map
 		self.add_body_params("Example", json.dumps(Example))
 	def get_TemplateType(self): # String
 		return self.get_body_params().get('TemplateType')
 
 	def set_TemplateType(self, TemplateType):  # String
 		self.add_body_params('TemplateType', TemplateType)
+	def get_TemplateName(self): # String
+		return self.get_body_params().get('TemplateName')
+
+	def set_TemplateName(self, TemplateName):  # String
+		self.add_body_params('TemplateName', TemplateName)
 	def get_IsvCode(self): # String
 		return self.get_body_params().get('IsvCode')
 
 	def set_IsvCode(self, IsvCode):  # String
 		self.add_body_params('IsvCode', IsvCode)
 	def get_CustSpaceId(self): # String
 		return self.get_body_params().get('CustSpaceId')
```

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/ModifyPhoneBusinessProfileRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/ModifyPhoneBusinessProfileRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,19 @@
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_PhoneNumber(self): # String
 		return self.get_query_params().get('PhoneNumber')
 
 	def set_PhoneNumber(self, PhoneNumber):  # String
 		self.add_query_param('PhoneNumber', PhoneNumber)
+	def get_About(self): # String
+		return self.get_query_params().get('About')
+
+	def set_About(self, About):  # String
+		self.add_query_param('About', About)
 	def get_Description(self): # String
 		return self.get_query_params().get('Description')
 
 	def set_Description(self, Description):  # String
 		self.add_query_param('Description', Description)
 	def get_Vertical(self): # String
 		return self.get_query_params().get('Vertical')
```

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/QueryChatappBindWabaRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/QueryChatappBindWabaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/QueryChatappPhoneNumbersRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/QueryWabaBusinessInfoRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,28 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkcams.endpoint import endpoint_data
 
-class QueryChatappPhoneNumbersRequest(RpcRequest):
+class QueryWabaBusinessInfoRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'cams', '2020-06-06', 'QueryChatappPhoneNumbers','cams')
+		RpcRequest.__init__(self, 'cams', '2020-06-06', 'QueryWabaBusinessInfo','cams')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_IsvCode(self): # String
-		return self.get_query_params().get('IsvCode')
+	def get_WabaId(self): # String
+		return self.get_query_params().get('WabaId')
 
-	def set_IsvCode(self, IsvCode):  # String
-		self.add_query_param('IsvCode', IsvCode)
+	def set_WabaId(self, WabaId):  # String
+		self.add_query_param('WabaId', WabaId)
 	def get_CustSpaceId(self): # String
 		return self.get_query_params().get('CustSpaceId')
 
 	def set_CustSpaceId(self, CustSpaceId):  # String
 		self.add_query_param('CustSpaceId', CustSpaceId)
```

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/QueryPhoneBusinessProfileRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/QueryPhoneBusinessProfileRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/QueryWabaBusinessInfoRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/GetPermissionByCodeRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,29 +15,35 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkcams.endpoint import endpoint_data
+import json
 
-class QueryWabaBusinessInfoRequest(RpcRequest):
+class GetPermissionByCodeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'cams', '2020-06-06', 'QueryWabaBusinessInfo','cams')
+		RpcRequest.__init__(self, 'cams', '2020-06-06', 'GetPermissionByCode','cams')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_WabaId(self): # String
-		return self.get_query_params().get('WabaId')
+	def get_Code(self): # String
+		return self.get_body_params().get('Code')
 
-	def set_WabaId(self, WabaId):  # String
-		self.add_query_param('WabaId', WabaId)
+	def set_Code(self, Code):  # String
+		self.add_body_params('Code', Code)
+	def get_Permissions(self): # Array
+		return self.get_body_params().get('Permissions')
+
+	def set_Permissions(self, Permissions):  # Array
+		self.add_body_params("Permissions", json.dumps(Permissions))
 	def get_CustSpaceId(self): # String
-		return self.get_query_params().get('CustSpaceId')
+		return self.get_body_params().get('CustSpaceId')
 
 	def set_CustSpaceId(self, CustSpaceId):  # String
-		self.add_query_param('CustSpaceId', CustSpaceId)
+		self.add_body_params('CustSpaceId', CustSpaceId)
```

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/SendChatappMassMessageRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/SendChatappMassMessageRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -58,14 +58,19 @@
 	def set_ChannelType(self, ChannelType):  # String
 		self.add_body_params('ChannelType', ChannelType)
 	def get_From(self): # String
 		return self.get_body_params().get('From')
 
 	def set_From(self, _From):  # String
 		self.add_body_params('From', _From)
+	def get_TemplateName(self): # String
+		return self.get_body_params().get('TemplateName')
+
+	def set_TemplateName(self, TemplateName):  # String
+		self.add_body_params('TemplateName', TemplateName)
 	def get_Tag(self): # String
 		return self.get_body_params().get('Tag')
 
 	def set_Tag(self, Tag):  # String
 		self.add_body_params('Tag', Tag)
 	def get_FallBackRule(self): # String
 		return self.get_body_params().get('FallBackRule')
```

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/SendChatappMessageRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/SendChatappMessageRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,64 +28,34 @@
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_ProductAction(self): # Struct
-		return self.get_body_params().get('ProductAction')
-
-	def set_ProductAction(self, ProductAction):  # Struct
-		self.add_body_params("ProductAction", json.dumps(ProductAction))
-	def get_MessageType(self): # String
-		return self.get_body_params().get('MessageType')
-
-	def set_MessageType(self, MessageType):  # String
-		self.add_body_params('MessageType', MessageType)
 	def get_Language(self): # String
 		return self.get_body_params().get('Language')
 
 	def set_Language(self, Language):  # String
 		self.add_body_params('Language', Language)
-	def get_CustWabaId(self): # String
-		return self.get_body_params().get('CustWabaId')
-
-	def set_CustWabaId(self, CustWabaId):  # String
-		self.add_body_params('CustWabaId', CustWabaId)
 	def get_Type(self): # String
 		return self.get_body_params().get('Type')
 
 	def set_Type(self, Type):  # String
 		self.add_body_params('Type', Type)
 	def get_FallBackContent(self): # String
 		return self.get_body_params().get('FallBackContent')
 
 	def set_FallBackContent(self, FallBackContent):  # String
 		self.add_body_params('FallBackContent', FallBackContent)
-	def get_Content(self): # String
-		return self.get_query_params().get('Content')
-
-	def set_Content(self, Content):  # String
-		self.add_query_param('Content', Content)
-	def get_TemplateParams(self): # Map
-		return self.get_body_params().get('TemplateParams')
-
-	def set_TemplateParams(self, TemplateParams):  # Map
-		self.add_body_params("TemplateParams", json.dumps(TemplateParams))
 	def get_Payload(self): # Array
 		return self.get_query_params().get('Payload')
 
 	def set_Payload(self, Payload):  # Array
 		self.add_query_param("Payload", json.dumps(Payload))
-	def get_ChannelType(self): # String
-		return self.get_body_params().get('ChannelType')
-
-	def set_ChannelType(self, ChannelType):  # String
-		self.add_body_params('ChannelType', ChannelType)
 	def get_From(self): # String
 		return self.get_body_params().get('From')
 
 	def set_From(self, _From):  # String
 		self.add_body_params('From', _From)
 	def get_Tag(self): # String
 		return self.get_body_params().get('Tag')
@@ -93,29 +63,79 @@
 	def set_Tag(self, Tag):  # String
 		self.add_body_params('Tag', Tag)
 	def get_FallBackRule(self): # String
 		return self.get_body_params().get('FallBackRule')
 
 	def set_FallBackRule(self, FallBackRule):  # String
 		self.add_body_params('FallBackRule', FallBackRule)
-	def get_TrackingData(self): # String
-		return self.get_body_params().get('TrackingData')
+	def get_FlowAction(self): # Struct
+		return self.get_body_params().get('FlowAction')
 
-	def set_TrackingData(self, TrackingData):  # String
-		self.add_body_params('TrackingData', TrackingData)
+	def set_FlowAction(self, FlowAction):  # Struct
+		self.add_body_params("FlowAction", json.dumps(FlowAction))
 	def get_TaskId(self): # String
 		return self.get_body_params().get('TaskId')
 
 	def set_TaskId(self, TaskId):  # String
 		self.add_body_params('TaskId', TaskId)
 	def get_IsvCode(self): # String
 		return self.get_body_params().get('IsvCode')
 
 	def set_IsvCode(self, IsvCode):  # String
 		self.add_body_params('IsvCode', IsvCode)
+	def get_CustSpaceId(self): # String
+		return self.get_body_params().get('CustSpaceId')
+
+	def set_CustSpaceId(self, CustSpaceId):  # String
+		self.add_body_params('CustSpaceId', CustSpaceId)
+	def get_TemplateCode(self): # String
+		return self.get_body_params().get('TemplateCode')
+
+	def set_TemplateCode(self, TemplateCode):  # String
+		self.add_body_params('TemplateCode', TemplateCode)
+	def get_ProductAction(self): # Struct
+		return self.get_body_params().get('ProductAction')
+
+	def set_ProductAction(self, ProductAction):  # Struct
+		self.add_body_params("ProductAction", json.dumps(ProductAction))
+	def get_MessageType(self): # String
+		return self.get_body_params().get('MessageType')
+
+	def set_MessageType(self, MessageType):  # String
+		self.add_body_params('MessageType', MessageType)
+	def get_CustWabaId(self): # String
+		return self.get_body_params().get('CustWabaId')
+
+	def set_CustWabaId(self, CustWabaId):  # String
+		self.add_body_params('CustWabaId', CustWabaId)
+	def get_Content(self): # String
+		return self.get_query_params().get('Content')
+
+	def set_Content(self, Content):  # String
+		self.add_query_param('Content', Content)
+	def get_TemplateParams(self): # Map
+		return self.get_body_params().get('TemplateParams')
+
+	def set_TemplateParams(self, TemplateParams):  # Map
+		self.add_body_params("TemplateParams", json.dumps(TemplateParams))
+	def get_ChannelType(self): # String
+		return self.get_body_params().get('ChannelType')
+
+	def set_ChannelType(self, ChannelType):  # String
+		self.add_body_params('ChannelType', ChannelType)
+	def get_TemplateName(self): # String
+		return self.get_body_params().get('TemplateName')
+
+	def set_TemplateName(self, TemplateName):  # String
+		self.add_body_params('TemplateName', TemplateName)
+	def get_TrackingData(self): # String
+		return self.get_body_params().get('TrackingData')
+
+	def set_TrackingData(self, TrackingData):  # String
+		self.add_body_params('TrackingData', TrackingData)
 	def get_ContextMessageId(self): # String
 		return self.get_body_params().get('ContextMessageId')
 
 	def set_ContextMessageId(self, ContextMessageId):  # String
 		self.add_body_params('ContextMessageId', ContextMessageId)
 	def get_Label(self): # String
 		return self.get_body_params().get('Label')
@@ -133,22 +153,12 @@
 	def set_Ttl(self, Ttl):  # Integer
 		self.add_body_params('Ttl', Ttl)
 	def get_FallBackDuration(self): # Integer
 		return self.get_body_params().get('FallBackDuration')
 
 	def set_FallBackDuration(self, FallBackDuration):  # Integer
 		self.add_body_params('FallBackDuration', FallBackDuration)
-	def get_CustSpaceId(self): # String
-		return self.get_body_params().get('CustSpaceId')
-
-	def set_CustSpaceId(self, CustSpaceId):  # String
-		self.add_body_params('CustSpaceId', CustSpaceId)
 	def get_To(self): # String
 		return self.get_body_params().get('To')
 
 	def set_To(self, To):  # String
 		self.add_body_params('To', To)
-	def get_TemplateCode(self): # String
-		return self.get_body_params().get('TemplateCode')
-
-	def set_TemplateCode(self, TemplateCode):  # String
-		self.add_body_params('TemplateCode', TemplateCode)
```

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/SubmitIsvCustomerTermsRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/SubmitIsvCustomerTermsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/UpdateAccountWebhookRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/UpdateAccountWebhookRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/UpdateCommerceSettingRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/UpdateCommerceSettingRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.8/aliyunsdkcams/request/v20200606/UpdatePhoneWebhookRequest.py` & `aliyun-python-sdk-cams-1.0.9/aliyunsdkcams/request/v20200606/UpdatePhoneWebhookRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.8/setup.py` & `aliyun-python-sdk-cams-1.0.9/setup.py`

 * *Files identical despite different names*

