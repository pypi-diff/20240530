# Comparing `tmp/tencentcloud-sdk-python-lke-3.0.1158.tar.gz` & `tmp/tencentcloud-sdk-python-lke-3.0.1159.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-lke-3.0.1158.tar", last modified: Wed May 29 20:49:12 2024, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-lke-3.0.1159.tar", last modified: Thu May 30 20:59:46 2024, max compression
```

## Comparing `tencentcloud-sdk-python-lke-3.0.1158.tar` & `tencentcloud-sdk-python-lke-3.0.1159.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:49:12.000000 tencentcloud-sdk-python-lke-3.0.1158/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:49:12.000000 tencentcloud-sdk-python-lke-3.0.1158/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      631 2024-05-29 20:49:12.000000 tencentcloud-sdk-python-lke-3.0.1158/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:49:12.000000 tencentcloud-sdk-python-lke-3.0.1158/tencentcloud/lke/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-29 20:49:12.000000 tencentcloud-sdk-python-lke-3.0.1158/tencentcloud/lke/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:49:12.000000 tencentcloud-sdk-python-lke-3.0.1158/tencentcloud/lke/v20231130/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-29 20:49:12.000000 tencentcloud-sdk-python-lke-3.0.1158/tencentcloud/lke/v20231130/__init__.py
--rw-r--r--   0 root         (0) root         (0)      961 2024-05-29 20:49:12.000000 tencentcloud-sdk-python-lke-3.0.1158/tencentcloud/lke/v20231130/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   384266 2024-05-29 20:49:12.000000 tencentcloud-sdk-python-lke-3.0.1158/tencentcloud/lke/v20231130/models.py
--rw-r--r--   0 root         (0) root         (0)    66494 2024-05-29 20:49:12.000000 tencentcloud-sdk-python-lke-3.0.1158/tencentcloud/lke/v20231130/lke_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:49:12.000000 tencentcloud-sdk-python-lke-3.0.1158/tencentcloud_sdk_python_lke.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 20:49:12.000000 tencentcloud-sdk-python-lke-3.0.1158/tencentcloud_sdk_python_lke.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-29 20:49:12.000000 tencentcloud-sdk-python-lke-3.0.1158/tencentcloud_sdk_python_lke.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-05-29 20:49:12.000000 tencentcloud-sdk-python-lke-3.0.1158/tencentcloud_sdk_python_lke.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      495 2024-05-29 20:49:12.000000 tencentcloud-sdk-python-lke-3.0.1158/tencentcloud_sdk_python_lke.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1660 2024-05-29 20:49:12.000000 tencentcloud-sdk-python-lke-3.0.1158/tencentcloud_sdk_python_lke.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2024-05-29 20:49:12.000000 tencentcloud-sdk-python-lke-3.0.1158/README.rst
--rw-r--r--   0 root         (0) root         (0)     1073 2024-05-29 20:49:12.000000 tencentcloud-sdk-python-lke-3.0.1158/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2024-05-29 20:49:12.000000 tencentcloud-sdk-python-lke-3.0.1158/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1660 2024-05-29 20:49:12.000000 tencentcloud-sdk-python-lke-3.0.1158/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      631 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/tencentcloud/lke/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/tencentcloud/lke/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/tencentcloud/lke/v20231130/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/tencentcloud/lke/v20231130/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      961 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/tencentcloud/lke/v20231130/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   384334 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/tencentcloud/lke/v20231130/models.py
+-rw-r--r--   0 root         (0) root         (0)    66422 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/tencentcloud/lke/v20231130/lke_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/tencentcloud_sdk_python_lke.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/tencentcloud_sdk_python_lke.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/tencentcloud_sdk_python_lke.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/tencentcloud_sdk_python_lke.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/tencentcloud_sdk_python_lke.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1660 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/tencentcloud_sdk_python_lke.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1660 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/PKG-INFO
```

### Comparing `tencentcloud-sdk-python-lke-3.0.1158/tencentcloud/__init__.py` & `tencentcloud-sdk-python-lke-3.0.1159/tencentcloud/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.1158'
+__version__ = '3.0.1159'
```

### Comparing `tencentcloud-sdk-python-lke-3.0.1158/tencentcloud/lke/v20231130/errorcodes.py` & `tencentcloud-sdk-python-lke-3.0.1159/tencentcloud/lke/v20231130/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lke-3.0.1158/tencentcloud/lke/v20231130/models.py` & `tencentcloud-sdk-python-lke-3.0.1159/tencentcloud/lke/v20231130/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -666,17 +666,17 @@
 
     """
 
     def __init__(self):
         r"""
         :param _Name: 应用名称
         :type Name: str
-        :param _Avatar: 机器人头像
+        :param _Avatar: 应用头像
         :type Avatar: str
-        :param _Desc: 机器人描述
+        :param _Desc: 应用描述
         :type Desc: str
         """
         self._Name = None
         self._Avatar = None
         self._Desc = None
 
     @property
@@ -12877,21 +12877,21 @@
 class SaveDocRequest(AbstractModel):
     """SaveDoc请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _BotBizId: 机器人ID
+        :param _BotBizId: 应用ID
         :type BotBizId: str
         :param _FileName: 文件名
         :type FileName: str
         :param _FileType: 文件类型(md|txt|docx|pdf|xlsx)
         :type FileType: str
-        :param _CosUrl: cos路径
+        :param _CosUrl: 平台cos路径，与DescribeStorageCredential接口查询UploadPath参数保持一致
         :type CosUrl: str
         :param _ETag: ETag 全称为 Entity Tag，是对象被创建时标识对象内容的信息标签，可用于检查对象的内容是否发生变化
         :type ETag: str
         :param _CosHash: cos_hash x-cos-hash-crc64ecma 头部中的 CRC64编码进行校验上传到云端的文件和本地文件的一致性
         :type CosHash: str
         :param _Size: 文件大小
         :type Size: str
```

### Comparing `tencentcloud-sdk-python-lke-3.0.1158/tencentcloud/lke/v20231130/lke_client.py` & `tencentcloud-sdk-python-lke-3.0.1159/tencentcloud/lke/v20231130/lke_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateApp(self, request):
-        """创建只是引擎应用，包括：知识管理应用、知识摘要应用、标签提取应用。
+        """创建知识引擎应用。
 
         :param request: Request instance for CreateApp.
         :type request: :class:`tencentcloud.lke.v20231130.models.CreateAppRequest`
         :rtype: :class:`tencentcloud.lke.v20231130.models.CreateAppResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-lke-3.0.1158/tencentcloud_sdk_python_lke.egg-info/PKG-INFO` & `tencentcloud-sdk-python-lke-3.0.1159/tencentcloud_sdk_python_lke.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lke
-Version: 3.0.1158
+Version: 3.0.1159
 Summary: Tencent Cloud Lke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lke-3.0.1158/README.rst` & `tencentcloud-sdk-python-lke-3.0.1159/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lke-3.0.1158/setup.py` & `tencentcloud-sdk-python-lke-3.0.1159/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-lke',
-    install_requires=["tencentcloud-sdk-python-common==3.0.1158"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.1159"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Lke SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-lke-3.0.1158/PKG-INFO` & `tencentcloud-sdk-python-lke-3.0.1159/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lke
-Version: 3.0.1158
+Version: 3.0.1159
 Summary: Tencent Cloud Lke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

