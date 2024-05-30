# Comparing `tmp/tencentcloud-sdk-python-vtc-3.0.1158.tar.gz` & `tmp/tencentcloud-sdk-python-vtc-3.0.1159.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vtc-3.0.1158.tar", last modified: Wed May 29 21:11:50 2024, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vtc-3.0.1159.tar", last modified: Thu May 30 21:22:15 2024, max compression
```

## Comparing `tencentcloud-sdk-python-vtc-3.0.1158.tar` & `tencentcloud-sdk-python-vtc-3.0.1159.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 21:11:50.000000 tencentcloud-sdk-python-vtc-3.0.1158/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 21:11:50.000000 tencentcloud-sdk-python-vtc-3.0.1158/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 21:11:50.000000 tencentcloud-sdk-python-vtc-3.0.1158/tencentcloud/vtc/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-29 21:11:50.000000 tencentcloud-sdk-python-vtc-3.0.1158/tencentcloud/vtc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 21:11:50.000000 tencentcloud-sdk-python-vtc-3.0.1158/tencentcloud/vtc/v20240223/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-29 21:11:50.000000 tencentcloud-sdk-python-vtc-3.0.1158/tencentcloud/vtc/v20240223/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3445 2024-05-29 21:11:50.000000 tencentcloud-sdk-python-vtc-3.0.1158/tencentcloud/vtc/v20240223/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    18525 2024-05-29 21:11:50.000000 tencentcloud-sdk-python-vtc-3.0.1158/tencentcloud/vtc/v20240223/models.py
--rw-r--r--   0 root         (0) root         (0)     3748 2024-05-29 21:11:50.000000 tencentcloud-sdk-python-vtc-3.0.1158/tencentcloud/vtc/v20240223/vtc_client.py
--rw-r--r--   0 root         (0) root         (0)      631 2024-05-29 21:11:50.000000 tencentcloud-sdk-python-vtc-3.0.1158/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)      737 2024-05-29 21:11:50.000000 tencentcloud-sdk-python-vtc-3.0.1158/README.rst
--rw-r--r--   0 root         (0) root         (0)     1073 2024-05-29 21:11:50.000000 tencentcloud-sdk-python-vtc-3.0.1158/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2024-05-29 21:11:50.000000 tencentcloud-sdk-python-vtc-3.0.1158/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 21:11:50.000000 tencentcloud-sdk-python-vtc-3.0.1158/tencentcloud_sdk_python_vtc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 21:11:50.000000 tencentcloud-sdk-python-vtc-3.0.1158/tencentcloud_sdk_python_vtc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-29 21:11:50.000000 tencentcloud-sdk-python-vtc-3.0.1158/tencentcloud_sdk_python_vtc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-05-29 21:11:50.000000 tencentcloud-sdk-python-vtc-3.0.1158/tencentcloud_sdk_python_vtc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      495 2024-05-29 21:11:50.000000 tencentcloud-sdk-python-vtc-3.0.1158/tencentcloud_sdk_python_vtc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1660 2024-05-29 21:11:50.000000 tencentcloud-sdk-python-vtc-3.0.1158/tencentcloud_sdk_python_vtc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1660 2024-05-29 21:11:50.000000 tencentcloud-sdk-python-vtc-3.0.1158/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 21:22:15.000000 tencentcloud-sdk-python-vtc-3.0.1159/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 21:22:15.000000 tencentcloud-sdk-python-vtc-3.0.1159/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 21:22:15.000000 tencentcloud-sdk-python-vtc-3.0.1159/tencentcloud/vtc/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 21:22:15.000000 tencentcloud-sdk-python-vtc-3.0.1159/tencentcloud/vtc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 21:22:15.000000 tencentcloud-sdk-python-vtc-3.0.1159/tencentcloud/vtc/v20240223/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 21:22:15.000000 tencentcloud-sdk-python-vtc-3.0.1159/tencentcloud/vtc/v20240223/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3445 2024-05-30 21:22:15.000000 tencentcloud-sdk-python-vtc-3.0.1159/tencentcloud/vtc/v20240223/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    18525 2024-05-30 21:22:15.000000 tencentcloud-sdk-python-vtc-3.0.1159/tencentcloud/vtc/v20240223/models.py
+-rw-r--r--   0 root         (0) root         (0)     3748 2024-05-30 21:22:15.000000 tencentcloud-sdk-python-vtc-3.0.1159/tencentcloud/vtc/v20240223/vtc_client.py
+-rw-r--r--   0 root         (0) root         (0)      631 2024-05-30 21:22:15.000000 tencentcloud-sdk-python-vtc-3.0.1159/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      737 2024-05-30 21:22:15.000000 tencentcloud-sdk-python-vtc-3.0.1159/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-05-30 21:22:15.000000 tencentcloud-sdk-python-vtc-3.0.1159/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2024-05-30 21:22:15.000000 tencentcloud-sdk-python-vtc-3.0.1159/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 21:22:15.000000 tencentcloud-sdk-python-vtc-3.0.1159/tencentcloud_sdk_python_vtc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 21:22:15.000000 tencentcloud-sdk-python-vtc-3.0.1159/tencentcloud_sdk_python_vtc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-30 21:22:15.000000 tencentcloud-sdk-python-vtc-3.0.1159/tencentcloud_sdk_python_vtc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-05-30 21:22:15.000000 tencentcloud-sdk-python-vtc-3.0.1159/tencentcloud_sdk_python_vtc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2024-05-30 21:22:15.000000 tencentcloud-sdk-python-vtc-3.0.1159/tencentcloud_sdk_python_vtc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1660 2024-05-30 21:22:15.000000 tencentcloud-sdk-python-vtc-3.0.1159/tencentcloud_sdk_python_vtc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1660 2024-05-30 21:22:15.000000 tencentcloud-sdk-python-vtc-3.0.1159/PKG-INFO
```

### Comparing `tencentcloud-sdk-python-vtc-3.0.1158/tencentcloud/vtc/v20240223/errorcodes.py` & `tencentcloud-sdk-python-vtc-3.0.1159/tencentcloud/vtc/v20240223/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vtc-3.0.1158/tencentcloud/vtc/v20240223/models.py` & `tencentcloud-sdk-python-vtc-3.0.1159/tencentcloud/vtc/v20240223/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vtc-3.0.1158/tencentcloud/vtc/v20240223/vtc_client.py` & `tencentcloud-sdk-python-vtc-3.0.1159/tencentcloud/vtc/v20240223/vtc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vtc-3.0.1158/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vtc-3.0.1159/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-vtc-3.0.1158/README.rst` & `tencentcloud-sdk-python-vtc-3.0.1159/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vtc-3.0.1158/setup.py` & `tencentcloud-sdk-python-vtc-3.0.1159/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-vtc',
-    install_requires=["tencentcloud-sdk-python-common==3.0.1158"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.1159"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Vtc SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-vtc-3.0.1158/tencentcloud_sdk_python_vtc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vtc-3.0.1159/tencentcloud_sdk_python_vtc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vtc
-Version: 3.0.1158
+Version: 3.0.1159
 Summary: Tencent Cloud Vtc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vtc-3.0.1158/PKG-INFO` & `tencentcloud-sdk-python-vtc-3.0.1159/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vtc
-Version: 3.0.1158
+Version: 3.0.1159
 Summary: Tencent Cloud Vtc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

