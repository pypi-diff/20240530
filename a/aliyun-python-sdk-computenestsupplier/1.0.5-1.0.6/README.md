# Comparing `tmp/aliyun-python-sdk-computenestsupplier-1.0.5.tar.gz` & `tmp/aliyun-python-sdk-computenestsupplier-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-computenestsupplier-1.0.5.tar", last modified: Tue May 23 05:32:19 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-computenestsupplier-1.0.6.tar", last modified: Thu May 30 06:58:45 2024, max compression
```

## Comparing `aliyun-python-sdk-computenestsupplier-1.0.5.tar` & `aliyun-python-sdk-computenestsupplier-1.0.6.tar`

### file list

```diff
@@ -1,38 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:32:19.000000 aliyun-python-sdk-computenestsupplier-1.0.5/
--rw-r--r--   0 root         (0) root         (0)      575 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1617 2023-05-23 05:32:19.000000 aliyun-python-sdk-computenestsupplier-1.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      559 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:32:19.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyun_python_sdk_computenestsupplier.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1617 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyun_python_sdk_computenestsupplier.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1878 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyun_python_sdk_computenestsupplier.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyun_python_sdk_computenestsupplier.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyun_python_sdk_computenestsupplier.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyun_python_sdk_computenestsupplier.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:32:19.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1088 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:32:19.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:32:19.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/
--rw-r--r--   0 root         (0) root         (0)     2778 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/CreateArtifactRequest.py
--rw-r--r--   0 root         (0) root         (0)     6253 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/CreateServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1708 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/DeleteArtifactRequest.py
--rw-r--r--   0 root         (0) root         (0)     1891 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/DeleteServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1750 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/GetArtifactRepositoryCredentialsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1905 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/GetArtifactRequest.py
--rw-r--r--   0 root         (0) root         (0)     2536 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/GetServiceEstimateCostRequest.py
--rw-r--r--   0 root         (0) root         (0)     1537 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/GetServiceInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1688 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/GetServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1487 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/GetUploadCredentialsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1869 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/ListArtifactVersionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2217 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/ListArtifactsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2845 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/ListServiceInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2223 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/ListServiceUsagesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3050 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/ListServicesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1489 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/ReleaseArtifactRequest.py
--rw-r--r--   0 root         (0) root         (0)     2420 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/UpdateArtifactRequest.py
--rw-r--r--   0 root         (0) root         (0)     5446 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/UpdateServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-05-23 05:32:19.000000 aliyun-python-sdk-computenestsupplier-1.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2532 2023-05-23 05:32:18.000000 aliyun-python-sdk-computenestsupplier-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/
+-rw-r--r--   0 root         (0) root         (0)      575 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1617 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      559 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyun_python_sdk_computenestsupplier.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1617 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyun_python_sdk_computenestsupplier.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3023 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyun_python_sdk_computenestsupplier.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyun_python_sdk_computenestsupplier.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyun_python_sdk_computenestsupplier.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyun_python_sdk_computenestsupplier.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/
+-rw-r--r--   0 root         (0) root         (0)     2429 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/AddServiceSharedAccountsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2116 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/ContinueDeployServiceInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3418 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/CreateArtifactRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3838 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/CreateServiceInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     8152 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/CreateServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1708 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/DeleteArtifactRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1828 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/DeleteServiceInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1891 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/DeleteServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/DeployServiceInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1750 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/GetArtifactRepositoryCredentialsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1905 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/GetArtifactRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2978 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/GetServiceEstimateCostRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1537 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/GetServiceInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2396 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/GetServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3431 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/GetServiceTemplateParameterConstraintsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/GetUploadCredentialsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2076 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/ListAcrImageRepositoriesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/ListAcrImageTagsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1877 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/ListArtifactVersionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2859 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/ListArtifactsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3068 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/ListServiceInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2426 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/ListServiceUsagesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3052 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/ListServicesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2057 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/ModifyServiceInstanceResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1712 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/PushMeteringDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1680 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/RegisterServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/ReleaseArtifactRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2420 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/UpdateArtifactRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1734 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/UpdateServiceInstanceAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2676 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/UpdateServiceInstanceSpecRequest.py
+-rw-r--r--   0 root         (0) root         (0)     6879 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/UpdateServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2315 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/UpgradeServiceInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2532 2024-05-30 06:58:45.000000 aliyun-python-sdk-computenestsupplier-1.0.6/setup.py
```

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.5/LICENSE` & `aliyun-python-sdk-computenestsupplier-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.5/PKG-INFO` & `aliyun-python-sdk-computenestsupplier-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-computenestsupplier
-Version: 1.0.5
+Version: 1.0.6
 Summary: The computenestsupplier module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-computenestsupplier
```

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.5/README.rst` & `aliyun-python-sdk-computenestsupplier-1.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.5/aliyun_python_sdk_computenestsupplier.egg-info/PKG-INFO` & `aliyun-python-sdk-computenestsupplier-1.0.6/aliyun_python_sdk_computenestsupplier.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-computenestsupplier
-Version: 1.0.5
+Version: 1.0.6
 Summary: The computenestsupplier module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-computenestsupplier
```

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.5/aliyun_python_sdk_computenestsupplier.egg-info/SOURCES.txt` & `aliyun-python-sdk-computenestsupplier-1.0.6/aliyun_python_sdk_computenestsupplier.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,26 +7,40 @@
 aliyun_python_sdk_computenestsupplier.egg-info/SOURCES.txt
 aliyun_python_sdk_computenestsupplier.egg-info/dependency_links.txt
 aliyun_python_sdk_computenestsupplier.egg-info/requires.txt
 aliyun_python_sdk_computenestsupplier.egg-info/top_level.txt
 aliyunsdkcomputenestsupplier/__init__.py
 aliyunsdkcomputenestsupplier/endpoint.py
 aliyunsdkcomputenestsupplier/request/__init__.py
+aliyunsdkcomputenestsupplier/request/v20210521/AddServiceSharedAccountsRequest.py
+aliyunsdkcomputenestsupplier/request/v20210521/ContinueDeployServiceInstanceRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/CreateArtifactRequest.py
+aliyunsdkcomputenestsupplier/request/v20210521/CreateServiceInstanceRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/CreateServiceRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/DeleteArtifactRequest.py
+aliyunsdkcomputenestsupplier/request/v20210521/DeleteServiceInstancesRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/DeleteServiceRequest.py
+aliyunsdkcomputenestsupplier/request/v20210521/DeployServiceInstanceRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/GetArtifactRepositoryCredentialsRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/GetArtifactRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/GetServiceEstimateCostRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/GetServiceInstanceRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/GetServiceRequest.py
+aliyunsdkcomputenestsupplier/request/v20210521/GetServiceTemplateParameterConstraintsRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/GetUploadCredentialsRequest.py
+aliyunsdkcomputenestsupplier/request/v20210521/ListAcrImageRepositoriesRequest.py
+aliyunsdkcomputenestsupplier/request/v20210521/ListAcrImageTagsRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/ListArtifactVersionsRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/ListArtifactsRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/ListServiceInstancesRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/ListServiceUsagesRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/ListServicesRequest.py
+aliyunsdkcomputenestsupplier/request/v20210521/ModifyServiceInstanceResourcesRequest.py
+aliyunsdkcomputenestsupplier/request/v20210521/PushMeteringDataRequest.py
+aliyunsdkcomputenestsupplier/request/v20210521/RegisterServiceRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/ReleaseArtifactRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/UpdateArtifactRequest.py
+aliyunsdkcomputenestsupplier/request/v20210521/UpdateServiceInstanceAttributeRequest.py
+aliyunsdkcomputenestsupplier/request/v20210521/UpdateServiceInstanceSpecRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/UpdateServiceRequest.py
+aliyunsdkcomputenestsupplier/request/v20210521/UpgradeServiceInstanceRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/__init__.py
```

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/endpoint.py` & `aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/CreateArtifactRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/CreateArtifactRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,14 +32,28 @@
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_Description(self): # String
 		return self.get_query_params().get('Description')
 
 	def set_Description(self, Description):  # String
 		self.add_query_param('Description', Description)
+	def get_ResourceGroupId(self): # String
+		return self.get_query_params().get('ResourceGroupId')
+
+	def set_ResourceGroupId(self, ResourceGroupId):  # String
+		self.add_query_param('ResourceGroupId', ResourceGroupId)
+	def get_Tags(self): # RepeatList
+		return self.get_query_params().get('Tag')
+
+	def set_Tags(self, Tag):  # RepeatList
+		for depth1 in range(len(Tag)):
+			if Tag[depth1].get('Value') is not None:
+				self.add_query_param('Tag.' + str(depth1 + 1) + '.Value', Tag[depth1].get('Value'))
+			if Tag[depth1].get('Key') is not None:
+				self.add_query_param('Tag.' + str(depth1 + 1) + '.Key', Tag[depth1].get('Key'))
 	def get_SupportRegionIdss(self): # RepeatList
 		return self.get_query_params().get('SupportRegionIds')
 
 	def set_SupportRegionIdss(self, SupportRegionIds):  # RepeatList
 		for depth1 in range(len(SupportRegionIds)):
 			self.add_query_param('SupportRegionIds.' + str(depth1 + 1), SupportRegionIds[depth1])
 	def get_ArtifactType(self): # String
```

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/CreateServiceRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/UpdateServiceRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,31 +15,37 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkcomputenestsupplier.endpoint import endpoint_data
+import json
 
-class CreateServiceRequest(RpcRequest):
+class UpdateServiceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ComputeNestSupplier', '2021-05-21', 'CreateService')
+		RpcRequest.__init__(self, 'ComputeNestSupplier', '2021-05-21', 'UpdateService')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_AlarmMetadata(self): # String
 		return self.get_query_params().get('AlarmMetadata')
 
 	def set_AlarmMetadata(self, AlarmMetadata):  # String
 		self.add_query_param('AlarmMetadata', AlarmMetadata)
+	def get_Resellable(self): # Boolean
+		return self.get_query_params().get('Resellable')
+
+	def set_Resellable(self, Resellable):  # Boolean
+		self.add_query_param('Resellable', Resellable)
 	def get_ClientToken(self): # String
 		return self.get_query_params().get('ClientToken')
 
 	def set_ClientToken(self, ClientToken):  # String
 		self.add_query_param('ClientToken', ClientToken)
 	def get_PolicyNames(self): # String
 		return self.get_query_params().get('PolicyNames')
@@ -52,43 +58,19 @@
 	def set_LicenseMetadata(self, LicenseMetadata):  # String
 		self.add_query_param('LicenseMetadata', LicenseMetadata)
 	def get_Duration(self): # Long
 		return self.get_query_params().get('Duration')
 
 	def set_Duration(self, Duration):  # Long
 		self.add_query_param('Duration', Duration)
-	def get_ResourceGroupId(self): # String
-		return self.get_query_params().get('ResourceGroupId')
-
-	def set_ResourceGroupId(self, ResourceGroupId):  # String
-		self.add_query_param('ResourceGroupId', ResourceGroupId)
-	def get_ApprovalType(self): # String
-		return self.get_query_params().get('ApprovalType')
-
-	def set_ApprovalType(self, ApprovalType):  # String
-		self.add_query_param('ApprovalType', ApprovalType)
-	def get_TrialDuration(self): # Long
+	def get_TrialDuration(self): # Integer
 		return self.get_query_params().get('TrialDuration')
 
-	def set_TrialDuration(self, TrialDuration):  # Long
+	def set_TrialDuration(self, TrialDuration):  # Integer
 		self.add_query_param('TrialDuration', TrialDuration)
-	def get_ShareType(self): # String
-		return self.get_query_params().get('ShareType')
-
-	def set_ShareType(self, ShareType):  # String
-		self.add_query_param('ShareType', ShareType)
-	def get_Tags(self): # RepeatList
-		return self.get_query_params().get('Tag')
-
-	def set_Tags(self, Tag):  # RepeatList
-		for depth1 in range(len(Tag)):
-			if Tag[depth1].get('Value') is not None:
-				self.add_query_param('Tag.' + str(depth1 + 1) + '.Value', Tag[depth1].get('Value'))
-			if Tag[depth1].get('Key') is not None:
-				self.add_query_param('Tag.' + str(depth1 + 1) + '.Key', Tag[depth1].get('Key'))
 	def get_UpgradeMetadata(self): # String
 		return self.get_query_params().get('UpgradeMetadata')
 
 	def set_UpgradeMetadata(self, UpgradeMetadata):  # String
 		self.add_query_param('UpgradeMetadata', UpgradeMetadata)
 	def get_DeployMetadata(self): # String
 		return self.get_query_params().get('DeployMetadata')
@@ -106,27 +88,50 @@
 	def set_IsSupportOperated(self, IsSupportOperated):  # Boolean
 		self.add_query_param('IsSupportOperated', IsSupportOperated)
 	def get_TenantType(self): # String
 		return self.get_query_params().get('TenantType')
 
 	def set_TenantType(self, TenantType):  # String
 		self.add_query_param('TenantType', TenantType)
+	def get_ServiceVersion(self): # String
+		return self.get_query_params().get('ServiceVersion')
+
+	def set_ServiceVersion(self, ServiceVersion):  # String
+		self.add_query_param('ServiceVersion', ServiceVersion)
+	def get_LogMetadata(self): # String
+		return self.get_query_params().get('LogMetadata')
+
+	def set_LogMetadata(self, LogMetadata):  # String
+		self.add_query_param('LogMetadata', LogMetadata)
 	def get_ServiceInfos(self): # RepeatList
 		return self.get_query_params().get('ServiceInfo')
 
 	def set_ServiceInfos(self, ServiceInfo):  # RepeatList
 		for depth1 in range(len(ServiceInfo)):
 			if ServiceInfo[depth1].get('ShortDescription') is not None:
 				self.add_query_param('ServiceInfo.' + str(depth1 + 1) + '.ShortDescription', ServiceInfo[depth1].get('ShortDescription'))
 			if ServiceInfo[depth1].get('Image') is not None:
 				self.add_query_param('ServiceInfo.' + str(depth1 + 1) + '.Image', ServiceInfo[depth1].get('Image'))
 			if ServiceInfo[depth1].get('Name') is not None:
 				self.add_query_param('ServiceInfo.' + str(depth1 + 1) + '.Name', ServiceInfo[depth1].get('Name'))
+			if ServiceInfo[depth1].get('Agreements') is not None:
+				for depth2 in range(len(ServiceInfo[depth1].get('Agreements'))):
+					if ServiceInfo[depth1].get('Agreements')[depth2].get('Name') is not None:
+						self.add_query_param('ServiceInfo.' + str(depth1 + 1) + '.Agreements.'  + str(depth2 + 1) + '.Name', ServiceInfo[depth1].get('Agreements')[depth2].get('Name'))
+					if ServiceInfo[depth1].get('Agreements')[depth2].get('Url') is not None:
+						self.add_query_param('ServiceInfo.' + str(depth1 + 1) + '.Agreements.'  + str(depth2 + 1) + '.Url', ServiceInfo[depth1].get('Agreements')[depth2].get('Url'))
 			if ServiceInfo[depth1].get('Locale') is not None:
 				self.add_query_param('ServiceInfo.' + str(depth1 + 1) + '.Locale', ServiceInfo[depth1].get('Locale'))
+			if ServiceInfo[depth1].get('LongDescriptionUrl') is not None:
+				self.add_query_param('ServiceInfo.' + str(depth1 + 1) + '.LongDescriptionUrl', ServiceInfo[depth1].get('LongDescriptionUrl'))
+	def get_UpdateOption(self): # Struct
+		return self.get_query_params().get('UpdateOption')
+
+	def set_UpdateOption(self, UpdateOption):  # Struct
+		self.add_query_param("UpdateOption", json.dumps(UpdateOption))
 	def get_ServiceId(self): # String
 		return self.get_query_params().get('ServiceId')
 
 	def set_ServiceId(self, ServiceId):  # String
 		self.add_query_param('ServiceId', ServiceId)
 	def get_VersionName(self): # String
 		return self.get_query_params().get('VersionName')
```

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/DeleteArtifactRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/DeleteArtifactRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/DeleteServiceRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/DeleteServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/GetArtifactRepositoryCredentialsRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/GetArtifactRepositoryCredentialsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/GetArtifactRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/GetArtifactRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/GetServiceEstimateCostRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/UpgradeServiceInstanceRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,48 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkcomputenestsupplier.endpoint import endpoint_data
 
-class GetServiceEstimateCostRequest(RpcRequest):
+class UpgradeServiceInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ComputeNestSupplier', '2021-05-21', 'GetServiceEstimateCost')
+		RpcRequest.__init__(self, 'ComputeNestSupplier', '2021-05-21', 'UpgradeServiceInstance')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ClientToken(self): # String
 		return self.get_query_params().get('ClientToken')
 
 	def set_ClientToken(self, ClientToken):  # String
 		self.add_query_param('ClientToken', ClientToken)
+	def get_ServiceInstanceId(self): # String
+		return self.get_query_params().get('ServiceInstanceId')
+
+	def set_ServiceInstanceId(self, ServiceInstanceId):  # String
+		self.add_query_param('ServiceInstanceId', ServiceInstanceId)
+	def get_DryRun(self): # String
+		return self.get_query_params().get('DryRun')
+
+	def set_DryRun(self, DryRun):  # String
+		self.add_query_param('DryRun', DryRun)
 	def get_ServiceVersion(self): # String
 		return self.get_query_params().get('ServiceVersion')
 
 	def set_ServiceVersion(self, ServiceVersion):  # String
 		self.add_query_param('ServiceVersion', ServiceVersion)
-	def get_TemplateName(self): # String
-		return self.get_query_params().get('TemplateName')
-
-	def set_TemplateName(self, TemplateName):  # String
-		self.add_query_param('TemplateName', TemplateName)
-	def get_ServiceId(self): # String
-		return self.get_query_params().get('ServiceId')
-
-	def set_ServiceId(self, ServiceId):  # String
-		self.add_query_param('ServiceId', ServiceId)
 	def get_Parameters(self): # String
 		return self.get_query_params().get('Parameters')
 
 	def set_Parameters(self, Parameters):  # String
 		self.add_query_param('Parameters', Parameters)
-	def get_ServiceInstanceId(self): # String
-		return self.get_query_params().get('ServiceInstanceId')
-
-	def set_ServiceInstanceId(self, ServiceInstanceId):  # String
-		self.add_query_param('ServiceInstanceId', ServiceInstanceId)
```

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/GetServiceInstanceRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/GetServiceInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/GetServiceRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/PushMeteringDataRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,28 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkcomputenestsupplier.endpoint import endpoint_data
 
-class GetServiceRequest(RpcRequest):
+class PushMeteringDataRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ComputeNestSupplier', '2021-05-21', 'GetService')
+		RpcRequest.__init__(self, 'ComputeNestSupplier', '2021-05-21', 'PushMeteringData')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_ServiceVersion(self): # String
-		return self.get_query_params().get('ServiceVersion')
+	def get_Metering(self): # String
+		return self.get_query_params().get('Metering')
 
-	def set_ServiceVersion(self, ServiceVersion):  # String
-		self.add_query_param('ServiceVersion', ServiceVersion)
-	def get_ServiceId(self): # String
-		return self.get_query_params().get('ServiceId')
+	def set_Metering(self, Metering):  # String
+		self.add_query_param('Metering', Metering)
+	def get_ServiceInstanceId(self): # String
+		return self.get_query_params().get('ServiceInstanceId')
 
-	def set_ServiceId(self, ServiceId):  # String
-		self.add_query_param('ServiceId', ServiceId)
+	def set_ServiceInstanceId(self, ServiceInstanceId):  # String
+		self.add_query_param('ServiceInstanceId', ServiceInstanceId)
```

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/GetUploadCredentialsRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/GetUploadCredentialsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/ListArtifactVersionsRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/ListArtifactVersionsRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_NextToken(self): # String
 		return self.get_query_params().get('NextToken')
 
 	def set_NextToken(self, NextToken):  # String
 		self.add_query_param('NextToken', NextToken)
-	def get_MaxResult(self): # String
-		return self.get_query_params().get('MaxResult')
+	def get_MaxResults(self): # Integer
+		return self.get_query_params().get('MaxResults')
 
-	def set_MaxResult(self, MaxResult):  # String
-		self.add_query_param('MaxResult', MaxResult)
+	def set_MaxResults(self, MaxResults):  # Integer
+		self.add_query_param('MaxResults', MaxResults)
 	def get_ArtifactId(self): # String
 		return self.get_query_params().get('ArtifactId')
 
 	def set_ArtifactId(self, ArtifactId):  # String
 		self.add_query_param('ArtifactId', ArtifactId)
```

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/ListArtifactsRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/ListServiceUsagesRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,38 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkcomputenestsupplier.endpoint import endpoint_data
 
-class ListArtifactsRequest(RpcRequest):
+class ListServiceUsagesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ComputeNestSupplier', '2021-05-21', 'ListArtifacts')
+		RpcRequest.__init__(self, 'ComputeNestSupplier', '2021-05-21', 'ListServiceUsages')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_NextToken(self): # String
 		return self.get_query_params().get('NextToken')
 
 	def set_NextToken(self, NextToken):  # String
 		self.add_query_param('NextToken', NextToken)
+	def get_SupplierRole(self): # String
+		return self.get_query_params().get('SupplierRole')
+
+	def set_SupplierRole(self, SupplierRole):  # String
+		self.add_query_param('SupplierRole', SupplierRole)
 	def get_Filters(self): # RepeatList
 		return self.get_query_params().get('Filter')
 
 	def set_Filters(self, Filter):  # RepeatList
 		for depth1 in range(len(Filter)):
-			if Filter[depth1].get('Values') is not None:
-				for depth2 in range(len(Filter[depth1].get('Values'))):
-					self.add_query_param('Filter.' + str(depth1 + 1) + '.Values.' + str(depth2 + 1), Filter[depth1].get('Values')[depth2])
 			if Filter[depth1].get('Name') is not None:
 				self.add_query_param('Filter.' + str(depth1 + 1) + '.Name', Filter[depth1].get('Name'))
-	def get_MaxResults(self): # String
+			if Filter[depth1].get('Value') is not None:
+				for depth2 in range(len(Filter[depth1].get('Value'))):
+					self.add_query_param('Filter.' + str(depth1 + 1) + '.Value.' + str(depth2 + 1), Filter[depth1].get('Value')[depth2])
+	def get_MaxResults(self): # Integer
 		return self.get_query_params().get('MaxResults')
 
-	def set_MaxResults(self, MaxResults):  # String
+	def set_MaxResults(self, MaxResults):  # Integer
 		self.add_query_param('MaxResults', MaxResults)
```

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/ListServiceInstancesRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/ListServiceInstancesRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,14 +27,19 @@
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_ResourceGroupId(self): # String
+		return self.get_query_params().get('ResourceGroupId')
+
+	def set_ResourceGroupId(self, ResourceGroupId):  # String
+		self.add_query_param('ResourceGroupId', ResourceGroupId)
 	def get_NextToken(self): # String
 		return self.get_query_params().get('NextToken')
 
 	def set_NextToken(self, NextToken):  # String
 		self.add_query_param('NextToken', NextToken)
 	def get_Tags(self): # RepeatList
 		return self.get_query_params().get('Tag')
@@ -56,12 +61,12 @@
 	def set_Filters(self, Filter):  # RepeatList
 		for depth1 in range(len(Filter)):
 			if Filter[depth1].get('Name') is not None:
 				self.add_query_param('Filter.' + str(depth1 + 1) + '.Name', Filter[depth1].get('Name'))
 			if Filter[depth1].get('Value') is not None:
 				for depth2 in range(len(Filter[depth1].get('Value'))):
 					self.add_query_param('Filter.' + str(depth1 + 1) + '.Value.' + str(depth2 + 1), Filter[depth1].get('Value')[depth2])
-	def get_MaxResults(self): # String
+	def get_MaxResults(self): # Integer
 		return self.get_query_params().get('MaxResults')
 
-	def set_MaxResults(self, MaxResults):  # String
+	def set_MaxResults(self, MaxResults):  # Integer
 		self.add_query_param('MaxResults', MaxResults)
```

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/ListServiceUsagesRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/DeleteServiceInstancesRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,38 +16,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkcomputenestsupplier.endpoint import endpoint_data
 
-class ListServiceUsagesRequest(RpcRequest):
+class DeleteServiceInstancesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ComputeNestSupplier', '2021-05-21', 'ListServiceUsages')
+		RpcRequest.__init__(self, 'ComputeNestSupplier', '2021-05-21', 'DeleteServiceInstances')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_NextToken(self): # String
-		return self.get_query_params().get('NextToken')
+	def get_ClientToken(self): # String
+		return self.get_query_params().get('ClientToken')
 
-	def set_NextToken(self, NextToken):  # String
-		self.add_query_param('NextToken', NextToken)
-	def get_Filters(self): # RepeatList
-		return self.get_query_params().get('Filter')
+	def set_ClientToken(self, ClientToken):  # String
+		self.add_query_param('ClientToken', ClientToken)
+	def get_ServiceInstanceIds(self): # RepeatList
+		return self.get_query_params().get('ServiceInstanceId')
 
-	def set_Filters(self, Filter):  # RepeatList
-		for depth1 in range(len(Filter)):
-			if Filter[depth1].get('Name') is not None:
-				self.add_query_param('Filter.' + str(depth1 + 1) + '.Name', Filter[depth1].get('Name'))
-			if Filter[depth1].get('Value') is not None:
-				for depth2 in range(len(Filter[depth1].get('Value'))):
-					self.add_query_param('Filter.' + str(depth1 + 1) + '.Value.' + str(depth2 + 1), Filter[depth1].get('Value')[depth2])
-	def get_MaxResults(self): # Integer
-		return self.get_query_params().get('MaxResults')
-
-	def set_MaxResults(self, MaxResults):  # Integer
-		self.add_query_param('MaxResults', MaxResults)
+	def set_ServiceInstanceIds(self, ServiceInstanceId):  # RepeatList
+		for depth1 in range(len(ServiceInstanceId)):
+			self.add_query_param('ServiceInstanceId.' + str(depth1 + 1), ServiceInstanceId[depth1])
```

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/ListServicesRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/ListServicesRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,12 +61,12 @@
 	def set_Filters(self, Filter):  # RepeatList
 		for depth1 in range(len(Filter)):
 			if Filter[depth1].get('Name') is not None:
 				self.add_query_param('Filter.' + str(depth1 + 1) + '.Name', Filter[depth1].get('Name'))
 			if Filter[depth1].get('Value') is not None:
 				for depth2 in range(len(Filter[depth1].get('Value'))):
 					self.add_query_param('Filter.' + str(depth1 + 1) + '.Value.' + str(depth2 + 1), Filter[depth1].get('Value')[depth2])
-	def get_MaxResults(self): # String
+	def get_MaxResults(self): # Integer
 		return self.get_query_params().get('MaxResults')
 
-	def set_MaxResults(self, MaxResults):  # String
+	def set_MaxResults(self, MaxResults):  # Integer
 		self.add_query_param('MaxResults', MaxResults)
```

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/ReleaseArtifactRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/ReleaseArtifactRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/UpdateArtifactRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/UpdateArtifactRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.5/aliyunsdkcomputenestsupplier/request/v20210521/UpdateServiceRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.6/aliyunsdkcomputenestsupplier/request/v20210521/CreateServiceInstanceRequest.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,111 +16,82 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkcomputenestsupplier.endpoint import endpoint_data
 
-class UpdateServiceRequest(RpcRequest):
+class CreateServiceInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ComputeNestSupplier', '2021-05-21', 'UpdateService')
+		RpcRequest.__init__(self, 'ComputeNestSupplier', '2021-05-21', 'CreateServiceInstance')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_AlarmMetadata(self): # String
-		return self.get_query_params().get('AlarmMetadata')
-
-	def set_AlarmMetadata(self, AlarmMetadata):  # String
-		self.add_query_param('AlarmMetadata', AlarmMetadata)
 	def get_ClientToken(self): # String
 		return self.get_query_params().get('ClientToken')
 
 	def set_ClientToken(self, ClientToken):  # String
 		self.add_query_param('ClientToken', ClientToken)
-	def get_PolicyNames(self): # String
-		return self.get_query_params().get('PolicyNames')
+	def get_UserId(self): # String
+		return self.get_query_params().get('UserId')
 
-	def set_PolicyNames(self, PolicyNames):  # String
-		self.add_query_param('PolicyNames', PolicyNames)
-	def get_LicenseMetadata(self): # String
-		return self.get_query_params().get('LicenseMetadata')
-
-	def set_LicenseMetadata(self, LicenseMetadata):  # String
-		self.add_query_param('LicenseMetadata', LicenseMetadata)
-	def get_Duration(self): # Long
-		return self.get_query_params().get('Duration')
-
-	def set_Duration(self, Duration):  # Long
-		self.add_query_param('Duration', Duration)
-	def get_TrialDuration(self): # Integer
-		return self.get_query_params().get('TrialDuration')
-
-	def set_TrialDuration(self, TrialDuration):  # Integer
-		self.add_query_param('TrialDuration', TrialDuration)
-	def get_UpgradeMetadata(self): # String
-		return self.get_query_params().get('UpgradeMetadata')
-
-	def set_UpgradeMetadata(self, UpgradeMetadata):  # String
-		self.add_query_param('UpgradeMetadata', UpgradeMetadata)
-	def get_DeployMetadata(self): # String
-		return self.get_query_params().get('DeployMetadata')
-
-	def set_DeployMetadata(self, DeployMetadata):  # String
-		self.add_query_param('DeployMetadata', DeployMetadata)
-	def get_ServiceType(self): # String
-		return self.get_query_params().get('ServiceType')
-
-	def set_ServiceType(self, ServiceType):  # String
-		self.add_query_param('ServiceType', ServiceType)
-	def get_IsSupportOperated(self): # Boolean
-		return self.get_query_params().get('IsSupportOperated')
-
-	def set_IsSupportOperated(self, IsSupportOperated):  # Boolean
-		self.add_query_param('IsSupportOperated', IsSupportOperated)
-	def get_TenantType(self): # String
-		return self.get_query_params().get('TenantType')
+	def set_UserId(self, UserId):  # String
+		self.add_query_param('UserId', UserId)
+	def get_ResourceGroupId(self): # String
+		return self.get_query_params().get('ResourceGroupId')
+
+	def set_ResourceGroupId(self, ResourceGroupId):  # String
+		self.add_query_param('ResourceGroupId', ResourceGroupId)
+	def get_TemplateName(self): # String
+		return self.get_query_params().get('TemplateName')
+
+	def set_TemplateName(self, TemplateName):  # String
+		self.add_query_param('TemplateName', TemplateName)
+	def get_Tags(self): # RepeatList
+		return self.get_query_params().get('Tag')
+
+	def set_Tags(self, Tag):  # RepeatList
+		for depth1 in range(len(Tag)):
+			if Tag[depth1].get('Value') is not None:
+				self.add_query_param('Tag.' + str(depth1 + 1) + '.Value', Tag[depth1].get('Value'))
+			if Tag[depth1].get('Key') is not None:
+				self.add_query_param('Tag.' + str(depth1 + 1) + '.Key', Tag[depth1].get('Key'))
+	def get_DryRun(self): # Boolean
+		return self.get_query_params().get('DryRun')
+
+	def set_DryRun(self, DryRun):  # Boolean
+		self.add_query_param('DryRun', DryRun)
+	def get_EndTime(self): # String
+		return self.get_query_params().get('EndTime')
+
+	def set_EndTime(self, EndTime):  # String
+		self.add_query_param('EndTime', EndTime)
+	def get_SpecificationName(self): # String
+		return self.get_query_params().get('SpecificationName')
+
+	def set_SpecificationName(self, SpecificationName):  # String
+		self.add_query_param('SpecificationName', SpecificationName)
+	def get_Name(self): # String
+		return self.get_query_params().get('Name')
 
-	def set_TenantType(self, TenantType):  # String
-		self.add_query_param('TenantType', TenantType)
+	def set_Name(self, Name):  # String
+		self.add_query_param('Name', Name)
 	def get_ServiceVersion(self): # String
 		return self.get_query_params().get('ServiceVersion')
 
 	def set_ServiceVersion(self, ServiceVersion):  # String
 		self.add_query_param('ServiceVersion', ServiceVersion)
-	def get_ServiceInfos(self): # RepeatList
-		return self.get_query_params().get('ServiceInfo')
-
-	def set_ServiceInfos(self, ServiceInfo):  # RepeatList
-		for depth1 in range(len(ServiceInfo)):
-			if ServiceInfo[depth1].get('ShortDescription') is not None:
-				self.add_query_param('ServiceInfo.' + str(depth1 + 1) + '.ShortDescription', ServiceInfo[depth1].get('ShortDescription'))
-			if ServiceInfo[depth1].get('Image') is not None:
-				self.add_query_param('ServiceInfo.' + str(depth1 + 1) + '.Image', ServiceInfo[depth1].get('Image'))
-			if ServiceInfo[depth1].get('Name') is not None:
-				self.add_query_param('ServiceInfo.' + str(depth1 + 1) + '.Name', ServiceInfo[depth1].get('Name'))
-			if ServiceInfo[depth1].get('Locale') is not None:
-				self.add_query_param('ServiceInfo.' + str(depth1 + 1) + '.Locale', ServiceInfo[depth1].get('Locale'))
 	def get_ServiceId(self): # String
 		return self.get_query_params().get('ServiceId')
 
 	def set_ServiceId(self, ServiceId):  # String
 		self.add_query_param('ServiceId', ServiceId)
-	def get_VersionName(self): # String
-		return self.get_query_params().get('VersionName')
-
-	def set_VersionName(self, VersionName):  # String
-		self.add_query_param('VersionName', VersionName)
-	def get_OperationMetadata(self): # String
-		return self.get_query_params().get('OperationMetadata')
-
-	def set_OperationMetadata(self, OperationMetadata):  # String
-		self.add_query_param('OperationMetadata', OperationMetadata)
-	def get_DeployType(self): # String
-		return self.get_query_params().get('DeployType')
+	def get_Parameters(self): # String
+		return self.get_query_params().get('Parameters')
 
-	def set_DeployType(self, DeployType):  # String
-		self.add_query_param('DeployType', DeployType)
+	def set_Parameters(self, Parameters):  # String
+		self.add_query_param('Parameters', Parameters)
```

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.5/setup.py` & `aliyun-python-sdk-computenestsupplier-1.0.6/setup.py`

 * *Files identical despite different names*

