# Comparing `tmp/aliyun-python-sdk-videoenhan-1.0.8.tar.gz` & `tmp/aliyun-python-sdk-videoenhan-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-videoenhan-1.0.8.tar", last modified: Tue Apr 13 02:28:42 2021, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-videoenhan-1.0.9.tar", last modified: Thu Sep 29 09:25:29 2022, max compression
```

## Comparing `aliyun-python-sdk-videoenhan-1.0.8.tar` & `aliyun-python-sdk-videoenhan-1.0.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 02:28:42.000000 aliyun-python-sdk-videoenhan-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      575 2021-04-13 02:28:41.000000 aliyun-python-sdk-videoenhan-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2021-04-13 02:28:41.000000 aliyun-python-sdk-videoenhan-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1572 2021-04-13 02:28:42.000000 aliyun-python-sdk-videoenhan-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      541 2021-04-13 02:28:41.000000 aliyun-python-sdk-videoenhan-1.0.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 02:28:42.000000 aliyun-python-sdk-videoenhan-1.0.8/aliyun_python_sdk_videoenhan.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1572 2021-04-13 02:28:42.000000 aliyun-python-sdk-videoenhan-1.0.8/aliyun_python_sdk_videoenhan.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1659 2021-04-13 02:28:42.000000 aliyun-python-sdk-videoenhan-1.0.8/aliyun_python_sdk_videoenhan.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-13 02:28:42.000000 aliyun-python-sdk-videoenhan-1.0.8/aliyun_python_sdk_videoenhan.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2021-04-13 02:28:42.000000 aliyun-python-sdk-videoenhan-1.0.8/aliyun_python_sdk_videoenhan.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2021-04-13 02:28:42.000000 aliyun-python-sdk-videoenhan-1.0.8/aliyun_python_sdk_videoenhan.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 02:28:42.000000 aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/
--rw-r--r--   0 root         (0) root         (0)       21 2021-04-13 02:28:41.000000 aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1088 2021-04-13 02:28:41.000000 aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 02:28:42.000000 aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/request/
--rw-r--r--   0 root         (0) root         (0)        0 2021-04-13 02:28:41.000000 aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 02:28:42.000000 aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/request/v20200320/
--rw-r--r--   0 root         (0) root         (0)     1913 2021-04-13 02:28:41.000000 aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/request/v20200320/AbstractEcommerceVideoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1601 2021-04-13 02:28:41.000000 aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/request/v20200320/AbstractFilmVideoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1607 2021-04-13 02:28:41.000000 aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/request/v20200320/AddFaceVideoTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     2121 2021-04-13 02:28:41.000000 aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/request/v20200320/AdjustVideoColorRequest.py
--rw-r--r--   0 root         (0) root         (0)     2579 2021-04-13 02:28:41.000000 aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/request/v20200320/ChangeVideoSizeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1965 2021-04-13 02:28:41.000000 aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/request/v20200320/ConvertHdrVideoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1625 2021-04-13 02:28:41.000000 aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/request/v20200320/DeleteFaceVideoTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     2501 2021-04-13 02:28:41.000000 aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/request/v20200320/EnhanceVideoQualityRequest.py
--rw-r--r--   0 root         (0) root         (0)     2110 2021-04-13 02:28:41.000000 aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/request/v20200320/EraseVideoLogoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1953 2021-04-13 02:28:41.000000 aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/request/v20200320/EraseVideoSubtitlesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3550 2021-04-13 02:28:41.000000 aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/request/v20200320/GenerateVideoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1435 2021-04-13 02:28:41.000000 aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/request/v20200320/GetAsyncJobResultRequest.py
--rw-r--r--   0 root         (0) root         (0)     1781 2021-04-13 02:28:41.000000 aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/request/v20200320/InterpolateVideoFrameRequest.py
--rw-r--r--   0 root         (0) root         (0)     1785 2021-04-13 02:28:41.000000 aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/request/v20200320/MergeVideoFaceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1801 2021-04-13 02:28:41.000000 aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/request/v20200320/MergeVideoModelFaceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1623 2021-04-13 02:28:41.000000 aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/request/v20200320/QueryFaceVideoTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     1607 2021-04-13 02:28:41.000000 aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/request/v20200320/SuperResolveVideoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1781 2021-04-13 02:28:41.000000 aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/request/v20200320/ToneSdrVideoRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-04-13 02:28:41.000000 aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/request/v20200320/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-04-13 02:28:42.000000 aliyun-python-sdk-videoenhan-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2487 2021-04-13 02:28:41.000000 aliyun-python-sdk-videoenhan-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 09:25:29.000000 aliyun-python-sdk-videoenhan-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      575 2022-09-29 09:25:29.000000 aliyun-python-sdk-videoenhan-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2022-09-29 09:25:29.000000 aliyun-python-sdk-videoenhan-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1572 2022-09-29 09:25:29.000000 aliyun-python-sdk-videoenhan-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      541 2022-09-29 09:25:29.000000 aliyun-python-sdk-videoenhan-1.0.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 09:25:29.000000 aliyun-python-sdk-videoenhan-1.0.9/aliyun_python_sdk_videoenhan.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1572 2022-09-29 09:25:29.000000 aliyun-python-sdk-videoenhan-1.0.9/aliyun_python_sdk_videoenhan.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1659 2022-09-29 09:25:29.000000 aliyun-python-sdk-videoenhan-1.0.9/aliyun_python_sdk_videoenhan.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-29 09:25:29.000000 aliyun-python-sdk-videoenhan-1.0.9/aliyun_python_sdk_videoenhan.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2022-09-29 09:25:29.000000 aliyun-python-sdk-videoenhan-1.0.9/aliyun_python_sdk_videoenhan.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2022-09-29 09:25:29.000000 aliyun-python-sdk-videoenhan-1.0.9/aliyun_python_sdk_videoenhan.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 09:25:29.000000 aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-09-29 09:25:29.000000 aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2022-09-29 09:25:29.000000 aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 09:25:29.000000 aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-09-29 09:25:29.000000 aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 09:25:29.000000 aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/request/v20200320/
+-rw-r--r--   0 root         (0) root         (0)     1991 2022-09-29 09:25:29.000000 aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/request/v20200320/AbstractEcommerceVideoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1643 2022-09-29 09:25:29.000000 aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/request/v20200320/AbstractFilmVideoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1647 2022-09-29 09:25:29.000000 aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/request/v20200320/AddFaceVideoTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2211 2022-09-29 09:25:29.000000 aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/request/v20200320/AdjustVideoColorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2753 2022-09-29 09:25:29.000000 aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/request/v20200320/ChangeVideoSizeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2045 2022-09-29 09:25:29.000000 aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/request/v20200320/ConvertHdrVideoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1665 2022-09-29 09:25:29.000000 aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/request/v20200320/DeleteFaceVideoTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2641 2022-09-29 09:25:29.000000 aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/request/v20200320/EnhanceVideoQualityRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2147 2022-09-29 09:25:29.000000 aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/request/v20200320/EraseVideoLogoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2039 2022-09-29 09:25:29.000000 aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/request/v20200320/EraseVideoSubtitlesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3761 2022-09-29 09:25:29.000000 aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/request/v20200320/GenerateVideoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2022-09-29 09:25:29.000000 aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/request/v20200320/GetAsyncJobResultRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1843 2022-09-29 09:25:29.000000 aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/request/v20200320/InterpolateVideoFrameRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1843 2022-09-29 09:25:29.000000 aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/request/v20200320/MergeVideoFaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1859 2022-09-29 09:25:29.000000 aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/request/v20200320/MergeVideoModelFaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1665 2022-09-29 09:25:29.000000 aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/request/v20200320/QueryFaceVideoTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1649 2022-09-29 09:25:29.000000 aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/request/v20200320/SuperResolveVideoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1841 2022-09-29 09:25:29.000000 aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/request/v20200320/ToneSdrVideoRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-09-29 09:25:29.000000 aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/request/v20200320/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2022-09-29 09:25:29.000000 aliyun-python-sdk-videoenhan-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2487 2022-09-29 09:25:29.000000 aliyun-python-sdk-videoenhan-1.0.9/setup.py
```

### Comparing `aliyun-python-sdk-videoenhan-1.0.8/LICENSE` & `aliyun-python-sdk-videoenhan-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-videoenhan-1.0.8/PKG-INFO` & `aliyun-python-sdk-videoenhan-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-videoenhan
-Version: 1.0.8
+Version: 1.0.9
 Summary: The videoenhan module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-videoenhan
```

### Comparing `aliyun-python-sdk-videoenhan-1.0.8/README.rst` & `aliyun-python-sdk-videoenhan-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-videoenhan-1.0.8/aliyun_python_sdk_videoenhan.egg-info/PKG-INFO` & `aliyun-python-sdk-videoenhan-1.0.9/aliyun_python_sdk_videoenhan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-videoenhan
-Version: 1.0.8
+Version: 1.0.9
 Summary: The videoenhan module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-videoenhan
```

### Comparing `aliyun-python-sdk-videoenhan-1.0.8/aliyun_python_sdk_videoenhan.egg-info/SOURCES.txt` & `aliyun-python-sdk-videoenhan-1.0.9/aliyun_python_sdk_videoenhan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/endpoint.py` & `aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/request/v20200320/AbstractEcommerceVideoRequest.py` & `aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/request/v20200320/AbstractEcommerceVideoRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,37 +20,34 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvideoenhan.endpoint import endpoint_data
 
 class AbstractEcommerceVideoRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'videoenhan', '2020-03-20', 'AbstractEcommerceVideo','videoenhan')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_Duration(self):
+	def get_Duration(self): # Float
 		return self.get_body_params().get('Duration')
 
-	def set_Duration(self,Duration):
+	def set_Duration(self, Duration):  # Float
 		self.add_body_params('Duration', Duration)
+	def get_Height(self): # Integer
+		return self.get_body_params().get('Height')
 
-	def get_VideoUrl(self):
+	def set_Height(self, Height):  # Integer
+		self.add_body_params('Height', Height)
+	def get_VideoUrl(self): # String
 		return self.get_body_params().get('VideoUrl')
 
-	def set_VideoUrl(self,VideoUrl):
+	def set_VideoUrl(self, VideoUrl):  # String
 		self.add_body_params('VideoUrl', VideoUrl)
-
-	def get_Width(self):
+	def get_Width(self): # Integer
 		return self.get_body_params().get('Width')
 
-	def set_Width(self,Width):
+	def set_Width(self, Width):  # Integer
 		self.add_body_params('Width', Width)
-
-	def get_Height(self):
-		return self.get_body_params().get('Height')
-
-	def set_Height(self,Height):
-		self.add_body_params('Height', Height)
```

### Comparing `aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/request/v20200320/AbstractFilmVideoRequest.py` & `aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/request/v20200320/AbstractFilmVideoRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,25 +20,24 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvideoenhan.endpoint import endpoint_data
 
 class AbstractFilmVideoRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'videoenhan', '2020-03-20', 'AbstractFilmVideo','videoenhan')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_Length(self):
+	def get_Length(self): # Integer
 		return self.get_body_params().get('Length')
 
-	def set_Length(self,Length):
+	def set_Length(self, Length):  # Integer
 		self.add_body_params('Length', Length)
-
-	def get_VideoUrl(self):
+	def get_VideoUrl(self): # String
 		return self.get_body_params().get('VideoUrl')
 
-	def set_VideoUrl(self,VideoUrl):
-		self.add_body_params('VideoUrl', VideoUrl)
+	def set_VideoUrl(self, VideoUrl):  # String
+		self.add_body_params('VideoUrl', VideoUrl)
```

### Comparing `aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/request/v20200320/AddFaceVideoTemplateRequest.py` & `aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/request/v20200320/AddFaceVideoTemplateRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,25 +20,24 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvideoenhan.endpoint import endpoint_data
 
 class AddFaceVideoTemplateRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'videoenhan', '2020-03-20', 'AddFaceVideoTemplate','videoenhan')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_UserId(self):
+	def get_UserId(self): # String
 		return self.get_body_params().get('UserId')
 
-	def set_UserId(self,UserId):
+	def set_UserId(self, UserId):  # String
 		self.add_body_params('UserId', UserId)
-
-	def get_VideoURL(self):
+	def get_VideoURL(self): # String
 		return self.get_body_params().get('VideoURL')
 
-	def set_VideoURL(self,VideoURL):
-		self.add_body_params('VideoURL', VideoURL)
+	def set_VideoURL(self, VideoURL):  # String
+		self.add_body_params('VideoURL', VideoURL)
```

### Comparing `aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/request/v20200320/AdjustVideoColorRequest.py` & `aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/request/v20200320/EraseVideoSubtitlesRequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,47 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvideoenhan.endpoint import endpoint_data
 
-class AdjustVideoColorRequest(RpcRequest):
+class EraseVideoSubtitlesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'videoenhan', '2020-03-20', 'AdjustVideoColor','videoenhan')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'videoenhan', '2020-03-20', 'EraseVideoSubtitles','videoenhan')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_BH(self): # Float
+		return self.get_body_params().get('BH')
 
-	def get_Mode(self):
-		return self.get_body_params().get('Mode')
-
-	def set_Mode(self,Mode):
-		self.add_body_params('Mode', Mode)
-
-	def get_VideoUrl(self):
+	def set_BH(self, BH):  # Float
+		self.add_body_params('BH', BH)
+	def get_BW(self): # Float
+		return self.get_body_params().get('BW')
+
+	def set_BW(self, BW):  # Float
+		self.add_body_params('BW', BW)
+	def get_BX(self): # Float
+		return self.get_body_params().get('BX')
+
+	def set_BX(self, BX):  # Float
+		self.add_body_params('BX', BX)
+	def get_BY(self): # Float
+		return self.get_body_params().get('BY')
+
+	def set_BY(self, BY):  # Float
+		self.add_body_params('BY', BY)
+	def get_VideoUrl(self): # String
 		return self.get_body_params().get('VideoUrl')
 
-	def set_VideoUrl(self,VideoUrl):
+	def set_VideoUrl(self, VideoUrl):  # String
 		self.add_body_params('VideoUrl', VideoUrl)
-
-	def get_VideoBitrate(self):
-		return self.get_body_params().get('VideoBitrate')
-
-	def set_VideoBitrate(self,VideoBitrate):
-		self.add_body_params('VideoBitrate', VideoBitrate)
-
-	def get_VideoCodec(self):
-		return self.get_body_params().get('VideoCodec')
-
-	def set_VideoCodec(self,VideoCodec):
-		self.add_body_params('VideoCodec', VideoCodec)
-
-	def get_VideoFormat(self):
-		return self.get_body_params().get('VideoFormat')
-
-	def set_VideoFormat(self,VideoFormat):
-		self.add_body_params('VideoFormat', VideoFormat)
```

### Comparing `aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/request/v20200320/ChangeVideoSizeRequest.py` & `aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/request/v20200320/EnhanceVideoQualityRequest.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,71 +16,53 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvideoenhan.endpoint import endpoint_data
 
-class ChangeVideoSizeRequest(RpcRequest):
+class EnhanceVideoQualityRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'videoenhan', '2020-03-20', 'ChangeVideoSize','videoenhan')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'videoenhan', '2020-03-20', 'EnhanceVideoQuality','videoenhan')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_HDRFormat(self): # String
+		return self.get_body_params().get('HDRFormat')
 
-	def get_Height(self):
-		return self.get_body_params().get('Height')
-
-	def set_Height(self,Height):
-		self.add_body_params('Height', Height)
-
-	def get_B(self):
-		return self.get_body_params().get('B')
-
-	def set_B(self,B):
-		self.add_body_params('B', B)
-
-	def get_FillType(self):
-		return self.get_body_params().get('FillType')
-
-	def set_FillType(self,FillType):
-		self.add_body_params('FillType', FillType)
-
-	def get_G(self):
-		return self.get_body_params().get('G')
-
-	def set_G(self,G):
-		self.add_body_params('G', G)
-
-	def get_CropType(self):
-		return self.get_body_params().get('CropType')
-
-	def set_CropType(self,CropType):
-		self.add_body_params('CropType', CropType)
-
-	def get_R(self):
-		return self.get_body_params().get('R')
-
-	def set_R(self,R):
-		self.add_body_params('R', R)
-
-	def get_VideoUrl(self):
-		return self.get_body_params().get('VideoUrl')
-
-	def set_VideoUrl(self,VideoUrl):
-		self.add_body_params('VideoUrl', VideoUrl)
-
-	def get_Width(self):
-		return self.get_body_params().get('Width')
-
-	def set_Width(self,Width):
-		self.add_body_params('Width', Width)
-
-	def get_Tightness(self):
-		return self.get_body_params().get('Tightness')
+	def set_HDRFormat(self, HDRFormat):  # String
+		self.add_body_params('HDRFormat', HDRFormat)
+	def get_FrameRate(self): # Integer
+		return self.get_body_params().get('FrameRate')
+
+	def set_FrameRate(self, FrameRate):  # Integer
+		self.add_body_params('FrameRate', FrameRate)
+	def get_MaxIlluminance(self): # Integer
+		return self.get_body_params().get('MaxIlluminance')
+
+	def set_MaxIlluminance(self, MaxIlluminance):  # Integer
+		self.add_body_params('MaxIlluminance', MaxIlluminance)
+	def get_Bitrate(self): # Integer
+		return self.get_body_params().get('Bitrate')
+
+	def set_Bitrate(self, Bitrate):  # Integer
+		self.add_body_params('Bitrate', Bitrate)
+	def get_OutPutWidth(self): # Integer
+		return self.get_body_params().get('OutPutWidth')
+
+	def set_OutPutWidth(self, OutPutWidth):  # Integer
+		self.add_body_params('OutPutWidth', OutPutWidth)
+	def get_OutPutHeight(self): # Integer
+		return self.get_body_params().get('OutPutHeight')
+
+	def set_OutPutHeight(self, OutPutHeight):  # Integer
+		self.add_body_params('OutPutHeight', OutPutHeight)
+	def get_VideoURL(self): # String
+		return self.get_body_params().get('VideoURL')
 
-	def set_Tightness(self,Tightness):
-		self.add_body_params('Tightness', Tightness)
+	def set_VideoURL(self, VideoURL):  # String
+		self.add_body_params('VideoURL', VideoURL)
```

### Comparing `aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/request/v20200320/ConvertHdrVideoRequest.py` & `aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/request/v20200320/ConvertHdrVideoRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,37 +20,34 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvideoenhan.endpoint import endpoint_data
 
 class ConvertHdrVideoRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'videoenhan', '2020-03-20', 'ConvertHdrVideo','videoenhan')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_HDRFormat(self):
+	def get_HDRFormat(self): # String
 		return self.get_body_params().get('HDRFormat')
 
-	def set_HDRFormat(self,HDRFormat):
+	def set_HDRFormat(self, HDRFormat):  # String
 		self.add_body_params('HDRFormat', HDRFormat)
-
-	def get_MaxIlluminance(self):
+	def get_MaxIlluminance(self): # Integer
 		return self.get_body_params().get('MaxIlluminance')
 
-	def set_MaxIlluminance(self,MaxIlluminance):
+	def set_MaxIlluminance(self, MaxIlluminance):  # Integer
 		self.add_body_params('MaxIlluminance', MaxIlluminance)
-
-	def get_Bitrate(self):
+	def get_Bitrate(self): # Integer
 		return self.get_body_params().get('Bitrate')
 
-	def set_Bitrate(self,Bitrate):
+	def set_Bitrate(self, Bitrate):  # Integer
 		self.add_body_params('Bitrate', Bitrate)
-
-	def get_VideoURL(self):
+	def get_VideoURL(self): # String
 		return self.get_body_params().get('VideoURL')
 
-	def set_VideoURL(self,VideoURL):
-		self.add_body_params('VideoURL', VideoURL)
+	def set_VideoURL(self, VideoURL):  # String
+		self.add_body_params('VideoURL', VideoURL)
```

### Comparing `aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/request/v20200320/DeleteFaceVideoTemplateRequest.py` & `aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/request/v20200320/DeleteFaceVideoTemplateRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,25 +20,24 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvideoenhan.endpoint import endpoint_data
 
 class DeleteFaceVideoTemplateRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'videoenhan', '2020-03-20', 'DeleteFaceVideoTemplate','videoenhan')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_UserId(self):
+	def get_UserId(self): # String
 		return self.get_body_params().get('UserId')
 
-	def set_UserId(self,UserId):
+	def set_UserId(self, UserId):  # String
 		self.add_body_params('UserId', UserId)
-
-	def get_TemplateId(self):
+	def get_TemplateId(self): # String
 		return self.get_body_params().get('TemplateId')
 
-	def set_TemplateId(self,TemplateId):
-		self.add_body_params('TemplateId', TemplateId)
+	def set_TemplateId(self, TemplateId):  # String
+		self.add_body_params('TemplateId', TemplateId)
```

### Comparing `aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/request/v20200320/EraseVideoLogoRequest.py` & `aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/request/v20200320/EraseVideoLogoRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,33 +20,32 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvideoenhan.endpoint import endpoint_data
 
 class EraseVideoLogoRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'videoenhan', '2020-03-20', 'EraseVideoLogo','videoenhan')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_Boxess(self):
+	def get_Boxess(self): # RepeatList
 		return self.get_body_params().get('Boxes')
 
-	def set_Boxess(self, Boxess):
-		for depth1 in range(len(Boxess)):
-			if Boxess[depth1].get('W') is not None:
-				self.add_body_params('Boxes.' + str(depth1 + 1) + '.W', Boxess[depth1].get('W'))
-			if Boxess[depth1].get('H') is not None:
-				self.add_body_params('Boxes.' + str(depth1 + 1) + '.H', Boxess[depth1].get('H'))
-			if Boxess[depth1].get('X') is not None:
-				self.add_body_params('Boxes.' + str(depth1 + 1) + '.X', Boxess[depth1].get('X'))
-			if Boxess[depth1].get('Y') is not None:
-				self.add_body_params('Boxes.' + str(depth1 + 1) + '.Y', Boxess[depth1].get('Y'))
-
-	def get_VideoUrl(self):
+	def set_Boxess(self, Boxes):  # RepeatList
+		for depth1 in range(len(Boxes)):
+			if Boxes[depth1].get('W') is not None:
+				self.add_body_params('Boxes.' + str(depth1 + 1) + '.W', Boxes[depth1].get('W'))
+			if Boxes[depth1].get('H') is not None:
+				self.add_body_params('Boxes.' + str(depth1 + 1) + '.H', Boxes[depth1].get('H'))
+			if Boxes[depth1].get('X') is not None:
+				self.add_body_params('Boxes.' + str(depth1 + 1) + '.X', Boxes[depth1].get('X'))
+			if Boxes[depth1].get('Y') is not None:
+				self.add_body_params('Boxes.' + str(depth1 + 1) + '.Y', Boxes[depth1].get('Y'))
+	def get_VideoUrl(self): # String
 		return self.get_body_params().get('VideoUrl')
 
-	def set_VideoUrl(self,VideoUrl):
-		self.add_body_params('VideoUrl', VideoUrl)
+	def set_VideoUrl(self, VideoUrl):  # String
+		self.add_body_params('VideoUrl', VideoUrl)
```

### Comparing `aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/request/v20200320/EraseVideoSubtitlesRequest.py` & `aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/request/v20200320/AdjustVideoColorRequest.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,47 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvideoenhan.endpoint import endpoint_data
 
-class EraseVideoSubtitlesRequest(RpcRequest):
+class AdjustVideoColorRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'videoenhan', '2020-03-20', 'EraseVideoSubtitles','videoenhan')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'videoenhan', '2020-03-20', 'AdjustVideoColor','videoenhan')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_Mode(self): # String
+		return self.get_body_params().get('Mode')
 
-	def get_BH(self):
-		return self.get_body_params().get('BH')
-
-	def set_BH(self,BH):
-		self.add_body_params('BH', BH)
-
-	def get_VideoUrl(self):
+	def set_Mode(self, Mode):  # String
+		self.add_body_params('Mode', Mode)
+	def get_VideoUrl(self): # String
 		return self.get_body_params().get('VideoUrl')
 
-	def set_VideoUrl(self,VideoUrl):
+	def set_VideoUrl(self, VideoUrl):  # String
 		self.add_body_params('VideoUrl', VideoUrl)
+	def get_VideoBitrate(self): # Long
+		return self.get_body_params().get('VideoBitrate')
 
-	def get_BW(self):
-		return self.get_body_params().get('BW')
-
-	def set_BW(self,BW):
-		self.add_body_params('BW', BW)
-
-	def get_BX(self):
-		return self.get_body_params().get('BX')
-
-	def set_BX(self,BX):
-		self.add_body_params('BX', BX)
-
-	def get_BY(self):
-		return self.get_body_params().get('BY')
+	def set_VideoBitrate(self, VideoBitrate):  # Long
+		self.add_body_params('VideoBitrate', VideoBitrate)
+	def get_VideoCodec(self): # String
+		return self.get_body_params().get('VideoCodec')
+
+	def set_VideoCodec(self, VideoCodec):  # String
+		self.add_body_params('VideoCodec', VideoCodec)
+	def get_VideoFormat(self): # String
+		return self.get_body_params().get('VideoFormat')
 
-	def set_BY(self,BY):
-		self.add_body_params('BY', BY)
+	def set_VideoFormat(self, VideoFormat):  # String
+		self.add_body_params('VideoFormat', VideoFormat)
```

### Comparing `aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/request/v20200320/GenerateVideoRequest.py` & `aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/request/v20200320/GenerateVideoRequest.py`

 * *Files 27% similar despite different names*

```diff
@@ -20,85 +20,75 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvideoenhan.endpoint import endpoint_data
 
 class GenerateVideoRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'videoenhan', '2020-03-20', 'GenerateVideo','videoenhan')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_TransitionStyle(self):
+	def get_TransitionStyle(self): # String
 		return self.get_body_params().get('TransitionStyle')
 
-	def set_TransitionStyle(self,TransitionStyle):
+	def set_TransitionStyle(self, TransitionStyle):  # String
 		self.add_body_params('TransitionStyle', TransitionStyle)
-
-	def get_Scene(self):
+	def get_Scene(self): # String
 		return self.get_body_params().get('Scene')
 
-	def set_Scene(self,Scene):
+	def set_Scene(self, Scene):  # String
 		self.add_body_params('Scene', Scene)
-
-	def get_Duration(self):
+	def get_Duration(self): # Float
 		return self.get_body_params().get('Duration')
 
-	def set_Duration(self,Duration):
+	def set_Duration(self, Duration):  # Float
 		self.add_body_params('Duration', Duration)
-
-	def get_PuzzleEffect(self):
+	def get_PuzzleEffect(self): # Boolean
 		return self.get_body_params().get('PuzzleEffect')
 
-	def set_PuzzleEffect(self,PuzzleEffect):
+	def set_PuzzleEffect(self, PuzzleEffect):  # Boolean
 		self.add_body_params('PuzzleEffect', PuzzleEffect)
-
-	def get_Height(self):
+	def get_Height(self): # Integer
 		return self.get_body_params().get('Height')
 
-	def set_Height(self,Height):
+	def set_Height(self, Height):  # Integer
 		self.add_body_params('Height', Height)
-
-	def get_DurationAdaption(self):
+	def get_DurationAdaption(self): # Boolean
 		return self.get_body_params().get('DurationAdaption')
 
-	def set_DurationAdaption(self,DurationAdaption):
+	def set_DurationAdaption(self, DurationAdaption):  # Boolean
 		self.add_body_params('DurationAdaption', DurationAdaption)
-
-	def get_FileLists(self):
+	def get_FileLists(self): # RepeatList
 		return self.get_body_params().get('FileList')
 
-	def set_FileLists(self, FileLists):
-		for depth1 in range(len(FileLists)):
-			if FileLists[depth1].get('FileName') is not None:
-				self.add_body_params('FileList.' + str(depth1 + 1) + '.FileName', FileLists[depth1].get('FileName'))
-			if FileLists[depth1].get('FileUrl') is not None:
-				self.add_body_params('FileList.' + str(depth1 + 1) + '.FileUrl', FileLists[depth1].get('FileUrl'))
-			if FileLists[depth1].get('Type') is not None:
-				self.add_body_params('FileList.' + str(depth1 + 1) + '.Type', FileLists[depth1].get('Type'))
-
-	def get_Mute(self):
+	def set_FileLists(self, FileList):  # RepeatList
+		for depth1 in range(len(FileList)):
+			if FileList[depth1].get('FileName') is not None:
+				self.add_body_params('FileList.' + str(depth1 + 1) + '.FileName', FileList[depth1].get('FileName'))
+			if FileList[depth1].get('FileUrl') is not None:
+				self.add_body_params('FileList.' + str(depth1 + 1) + '.FileUrl', FileList[depth1].get('FileUrl'))
+			if FileList[depth1].get('Type') is not None:
+				self.add_body_params('FileList.' + str(depth1 + 1) + '.Type', FileList[depth1].get('Type'))
+	def get_Mute(self): # Boolean
 		return self.get_body_params().get('Mute')
 
-	def set_Mute(self,Mute):
+	def set_Mute(self, Mute):  # Boolean
 		self.add_body_params('Mute', Mute)
-
-	def get_SmartEffect(self):
+	def get_SmartEffect(self): # Boolean
 		return self.get_body_params().get('SmartEffect')
 
-	def set_SmartEffect(self,SmartEffect):
+	def set_SmartEffect(self, SmartEffect):  # Boolean
 		self.add_body_params('SmartEffect', SmartEffect)
-
-	def get_Width(self):
+	def get_Width(self): # Integer
 		return self.get_body_params().get('Width')
 
-	def set_Width(self,Width):
+	def set_Width(self, Width):  # Integer
 		self.add_body_params('Width', Width)
-
-	def get_Style(self):
+	def get_Style(self): # String
 		return self.get_body_params().get('Style')
 
-	def set_Style(self,Style):
-		self.add_body_params('Style', Style)
+	def set_Style(self, Style):  # String
+		self.add_body_params('Style', Style)
```

### Comparing `aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/request/v20200320/GetAsyncJobResultRequest.py` & `aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/request/v20200320/GetAsyncJobResultRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,19 +20,19 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvideoenhan.endpoint import endpoint_data
 
 class GetAsyncJobResultRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'videoenhan', '2020-03-20', 'GetAsyncJobResult','videoenhan')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_JobId(self):
+	def get_JobId(self): # String
 		return self.get_body_params().get('JobId')
 
-	def set_JobId(self,JobId):
-		self.add_body_params('JobId', JobId)
+	def set_JobId(self, JobId):  # String
+		self.add_body_params('JobId', JobId)
```

### Comparing `aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/request/v20200320/InterpolateVideoFrameRequest.py` & `aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/request/v20200320/InterpolateVideoFrameRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,31 +20,29 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvideoenhan.endpoint import endpoint_data
 
 class InterpolateVideoFrameRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'videoenhan', '2020-03-20', 'InterpolateVideoFrame','videoenhan')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_FrameRate(self):
+	def get_FrameRate(self): # Integer
 		return self.get_body_params().get('FrameRate')
 
-	def set_FrameRate(self,FrameRate):
+	def set_FrameRate(self, FrameRate):  # Integer
 		self.add_body_params('FrameRate', FrameRate)
-
-	def get_Bitrate(self):
+	def get_Bitrate(self): # Integer
 		return self.get_body_params().get('Bitrate')
 
-	def set_Bitrate(self,Bitrate):
+	def set_Bitrate(self, Bitrate):  # Integer
 		self.add_body_params('Bitrate', Bitrate)
-
-	def get_VideoURL(self):
+	def get_VideoURL(self): # String
 		return self.get_body_params().get('VideoURL')
 
-	def set_VideoURL(self,VideoURL):
-		self.add_body_params('VideoURL', VideoURL)
+	def set_VideoURL(self, VideoURL):  # String
+		self.add_body_params('VideoURL', VideoURL)
```

### Comparing `aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/request/v20200320/MergeVideoFaceRequest.py` & `aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/request/v20200320/MergeVideoFaceRequest.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,31 +20,29 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvideoenhan.endpoint import endpoint_data
 
 class MergeVideoFaceRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'videoenhan', '2020-03-20', 'MergeVideoFace','videoenhan')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_PostURL(self):
-		return self.get_body_params().get('PostURL')
-
-	def set_PostURL(self,PostURL):
-		self.add_body_params('PostURL', PostURL)
-
-	def get_ReferenceURL(self):
+	def get_ReferenceURL(self): # String
 		return self.get_body_params().get('ReferenceURL')
 
-	def set_ReferenceURL(self,ReferenceURL):
+	def set_ReferenceURL(self, ReferenceURL):  # String
 		self.add_body_params('ReferenceURL', ReferenceURL)
+	def get_PostURL(self): # String
+		return self.get_body_params().get('PostURL')
 
-	def get_VideoURL(self):
+	def set_PostURL(self, PostURL):  # String
+		self.add_body_params('PostURL', PostURL)
+	def get_VideoURL(self): # String
 		return self.get_body_params().get('VideoURL')
 
-	def set_VideoURL(self,VideoURL):
-		self.add_body_params('VideoURL', VideoURL)
+	def set_VideoURL(self, VideoURL):  # String
+		self.add_body_params('VideoURL', VideoURL)
```

### Comparing `aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/request/v20200320/MergeVideoModelFaceRequest.py` & `aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/request/v20200320/MergeVideoModelFaceRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,31 +20,29 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvideoenhan.endpoint import endpoint_data
 
 class MergeVideoModelFaceRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'videoenhan', '2020-03-20', 'MergeVideoModelFace','videoenhan')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_FaceImageURL(self):
+	def get_FaceImageURL(self): # String
 		return self.get_body_params().get('FaceImageURL')
 
-	def set_FaceImageURL(self,FaceImageURL):
+	def set_FaceImageURL(self, FaceImageURL):  # String
 		self.add_body_params('FaceImageURL', FaceImageURL)
-
-	def get_UserId(self):
+	def get_UserId(self): # String
 		return self.get_body_params().get('UserId')
 
-	def set_UserId(self,UserId):
+	def set_UserId(self, UserId):  # String
 		self.add_body_params('UserId', UserId)
-
-	def get_TemplateId(self):
+	def get_TemplateId(self): # String
 		return self.get_body_params().get('TemplateId')
 
-	def set_TemplateId(self,TemplateId):
-		self.add_body_params('TemplateId', TemplateId)
+	def set_TemplateId(self, TemplateId):  # String
+		self.add_body_params('TemplateId', TemplateId)
```

### Comparing `aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/request/v20200320/QueryFaceVideoTemplateRequest.py` & `aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/request/v20200320/QueryFaceVideoTemplateRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,25 +20,24 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvideoenhan.endpoint import endpoint_data
 
 class QueryFaceVideoTemplateRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'videoenhan', '2020-03-20', 'QueryFaceVideoTemplate','videoenhan')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_UserId(self):
+	def get_UserId(self): # String
 		return self.get_query_params().get('UserId')
 
-	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
-
-	def get_TemplateId(self):
+	def set_UserId(self, UserId):  # String
+		self.add_query_param('UserId', UserId)
+	def get_TemplateId(self): # String
 		return self.get_query_params().get('TemplateId')
 
-	def set_TemplateId(self,TemplateId):
-		self.add_query_param('TemplateId',TemplateId)
+	def set_TemplateId(self, TemplateId):  # String
+		self.add_query_param('TemplateId', TemplateId)
```

### Comparing `aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/request/v20200320/SuperResolveVideoRequest.py` & `aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/request/v20200320/SuperResolveVideoRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,25 +20,24 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvideoenhan.endpoint import endpoint_data
 
 class SuperResolveVideoRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'videoenhan', '2020-03-20', 'SuperResolveVideo','videoenhan')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_BitRate(self):
+	def get_BitRate(self): # Integer
 		return self.get_body_params().get('BitRate')
 
-	def set_BitRate(self,BitRate):
+	def set_BitRate(self, BitRate):  # Integer
 		self.add_body_params('BitRate', BitRate)
-
-	def get_VideoUrl(self):
+	def get_VideoUrl(self): # String
 		return self.get_body_params().get('VideoUrl')
 
-	def set_VideoUrl(self,VideoUrl):
-		self.add_body_params('VideoUrl', VideoUrl)
+	def set_VideoUrl(self, VideoUrl):  # String
+		self.add_body_params('VideoUrl', VideoUrl)
```

### Comparing `aliyun-python-sdk-videoenhan-1.0.8/aliyunsdkvideoenhan/request/v20200320/ToneSdrVideoRequest.py` & `aliyun-python-sdk-videoenhan-1.0.9/aliyunsdkvideoenhan/request/v20200320/ToneSdrVideoRequest.py`

 * *Files 25% similar despite different names*

```diff
@@ -20,31 +20,29 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkvideoenhan.endpoint import endpoint_data
 
 class ToneSdrVideoRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'videoenhan', '2020-03-20', 'ToneSdrVideo','videoenhan')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_RecolorModel(self):
-		return self.get_body_params().get('RecolorModel')
-
-	def set_RecolorModel(self,RecolorModel):
-		self.add_body_params('RecolorModel', RecolorModel)
-
-	def get_Bitrate(self):
+	def get_Bitrate(self): # Integer
 		return self.get_body_params().get('Bitrate')
 
-	def set_Bitrate(self,Bitrate):
+	def set_Bitrate(self, Bitrate):  # Integer
 		self.add_body_params('Bitrate', Bitrate)
+	def get_RecolorModel(self): # String
+		return self.get_body_params().get('RecolorModel')
 
-	def get_VideoURL(self):
+	def set_RecolorModel(self, RecolorModel):  # String
+		self.add_body_params('RecolorModel', RecolorModel)
+	def get_VideoURL(self): # String
 		return self.get_body_params().get('VideoURL')
 
-	def set_VideoURL(self,VideoURL):
-		self.add_body_params('VideoURL', VideoURL)
+	def set_VideoURL(self, VideoURL):  # String
+		self.add_body_params('VideoURL', VideoURL)
```

### Comparing `aliyun-python-sdk-videoenhan-1.0.8/setup.py` & `aliyun-python-sdk-videoenhan-1.0.9/setup.py`

 * *Files identical despite different names*

