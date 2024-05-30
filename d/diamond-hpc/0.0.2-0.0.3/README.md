# Comparing `tmp/diamond-hpc-0.0.2.tar.gz` & `tmp/diamond-hpc-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diamond-hpc-0.0.2.tar", last modified: Tue May 28 00:21:53 2024, max compression
+gzip compressed data, was "diamond-hpc-0.0.3.tar", last modified: Thu May 30 03:44:36 2024, max compression
```

## Comparing `diamond-hpc-0.0.2.tar` & `diamond-hpc-0.0.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-05-28 00:21:53.236606 diamond-hpc-0.0.2/
--rw-r--r--   0 hotine    (1000) hotine    (1000)     1069 2024-05-21 23:35:15.000000 diamond-hpc-0.0.2/LICENSE
--rw-r--r--   0 hotine    (1000) hotine    (1000)     1484 2024-05-28 00:21:53.236606 diamond-hpc-0.0.2/PKG-INFO
--rw-r--r--   0 hotine    (1000) hotine    (1000)      977 2024-05-27 23:53:29.000000 diamond-hpc-0.0.2/README.md
-drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-05-28 00:21:53.236606 diamond-hpc-0.0.2/diamond/
--rw-r--r--   0 hotine    (1000) hotine    (1000)        0 2024-05-21 23:35:15.000000 diamond-hpc-0.0.2/diamond/__init__.py
-drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-05-28 00:21:53.236606 diamond-hpc-0.0.2/diamond/container/
--rw-r--r--   0 hotine    (1000) hotine    (1000)        0 2024-05-21 23:35:15.000000 diamond-hpc-0.0.2/diamond/container/__init__.py
--rw-r--r--   0 hotine    (1000) hotine    (1000)     7107 2024-05-21 23:35:15.000000 diamond-hpc-0.0.2/diamond/container/container.py
-drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-05-28 00:21:53.236606 diamond-hpc-0.0.2/diamond/container/custom_image_builder/
--rw-r--r--   0 hotine    (1000) hotine    (1000)       55 2024-05-21 23:35:15.000000 diamond-hpc-0.0.2/diamond/container/custom_image_builder/__init__.py
-drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-05-28 00:21:53.236606 diamond-hpc-0.0.2/diamond/container/custom_image_builder/exception/
--rw-r--r--   0 hotine    (1000) hotine    (1000)      142 2024-05-21 23:35:15.000000 diamond-hpc-0.0.2/diamond/container/custom_image_builder/exception/ImageBuilderException.py
--rw-r--r--   0 hotine    (1000) hotine    (1000)      143 2024-05-21 23:35:15.000000 diamond-hpc-0.0.2/diamond/container/custom_image_builder/exception/RegisterImageException.py
--rw-r--r--   0 hotine    (1000) hotine    (1000)        0 2024-05-21 23:35:15.000000 diamond-hpc-0.0.2/diamond/container/custom_image_builder/exception/__init__.py
--rw-r--r--   0 hotine    (1000) hotine    (1000)     7174 2024-05-27 23:08:58.000000 diamond-hpc-0.0.2/diamond/container/custom_image_builder/image_builder.py
-drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-05-28 00:21:53.236606 diamond-hpc-0.0.2/diamond/diamond_client/
--rw-r--r--   0 hotine    (1000) hotine    (1000)        0 2024-05-27 17:23:42.000000 diamond-hpc-0.0.2/diamond/diamond_client/__init__.py
--rw-r--r--   0 hotine    (1000) hotine    (1000)     1701 2024-05-28 00:16:31.000000 diamond-hpc-0.0.2/diamond/diamond_client/diamond_client.py
-drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-05-28 00:21:53.236606 diamond-hpc-0.0.2/diamond/diamond_client/templates/
--rw-r--r--   0 hotine    (1000) hotine    (1000)      772 2024-05-28 00:00:08.000000 diamond-hpc-0.0.2/diamond/diamond_client/templates/task_template
-drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-05-28 00:21:53.236606 diamond-hpc-0.0.2/diamond/wrapper/
--rw-r--r--   0 hotine    (1000) hotine    (1000)        0 2024-05-21 23:35:15.000000 diamond-hpc-0.0.2/diamond/wrapper/__init__.py
--rw-r--r--   0 hotine    (1000) hotine    (1000)     1911 2024-05-27 23:53:38.000000 diamond-hpc-0.0.2/diamond/wrapper/wrapper.py
-drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-05-28 00:21:53.236606 diamond-hpc-0.0.2/diamond_hpc.egg-info/
--rw-r--r--   0 hotine    (1000) hotine    (1000)     1484 2024-05-28 00:21:53.000000 diamond-hpc-0.0.2/diamond_hpc.egg-info/PKG-INFO
--rw-r--r--   0 hotine    (1000) hotine    (1000)      814 2024-05-28 00:21:53.000000 diamond-hpc-0.0.2/diamond_hpc.egg-info/SOURCES.txt
--rw-r--r--   0 hotine    (1000) hotine    (1000)        1 2024-05-28 00:21:53.000000 diamond-hpc-0.0.2/diamond_hpc.egg-info/dependency_links.txt
--rw-r--r--   0 hotine    (1000) hotine    (1000)       61 2024-05-28 00:21:53.000000 diamond-hpc-0.0.2/diamond_hpc.egg-info/entry_points.txt
--rw-r--r--   0 hotine    (1000) hotine    (1000)       71 2024-05-28 00:21:53.000000 diamond-hpc-0.0.2/diamond_hpc.egg-info/requires.txt
--rw-r--r--   0 hotine    (1000) hotine    (1000)        8 2024-05-28 00:21:53.000000 diamond-hpc-0.0.2/diamond_hpc.egg-info/top_level.txt
--rw-r--r--   0 hotine    (1000) hotine    (1000)       38 2024-05-28 00:21:53.236606 diamond-hpc-0.0.2/setup.cfg
--rw-r--r--   0 hotine    (1000) hotine    (1000)      971 2024-05-28 00:21:45.000000 diamond-hpc-0.0.2/setup.py
+drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-05-30 03:44:36.752491 diamond-hpc-0.0.3/
+-rw-r--r--   0 hotine    (1000) hotine    (1000)     1069 2024-05-21 23:35:15.000000 diamond-hpc-0.0.3/LICENSE
+-rw-r--r--   0 hotine    (1000) hotine    (1000)     1484 2024-05-30 03:44:36.752491 diamond-hpc-0.0.3/PKG-INFO
+-rw-r--r--   0 hotine    (1000) hotine    (1000)      977 2024-05-28 00:38:00.000000 diamond-hpc-0.0.3/README.md
+drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-05-30 03:44:36.752491 diamond-hpc-0.0.3/diamond/
+-rw-r--r--   0 hotine    (1000) hotine    (1000)        0 2024-05-21 23:35:15.000000 diamond-hpc-0.0.3/diamond/__init__.py
+drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-05-30 03:44:36.752491 diamond-hpc-0.0.3/diamond/container/
+-rw-r--r--   0 hotine    (1000) hotine    (1000)        0 2024-05-21 23:35:15.000000 diamond-hpc-0.0.3/diamond/container/__init__.py
+-rw-r--r--   0 hotine    (1000) hotine    (1000)     7107 2024-05-21 23:35:15.000000 diamond-hpc-0.0.3/diamond/container/container.py
+drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-05-30 03:44:36.752491 diamond-hpc-0.0.3/diamond/container/custom_image_builder/
+-rw-r--r--   0 hotine    (1000) hotine    (1000)       55 2024-05-21 23:35:15.000000 diamond-hpc-0.0.3/diamond/container/custom_image_builder/__init__.py
+drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-05-30 03:44:36.752491 diamond-hpc-0.0.3/diamond/container/custom_image_builder/exception/
+-rw-r--r--   0 hotine    (1000) hotine    (1000)      142 2024-05-21 23:35:15.000000 diamond-hpc-0.0.3/diamond/container/custom_image_builder/exception/ImageBuilderException.py
+-rw-r--r--   0 hotine    (1000) hotine    (1000)      143 2024-05-21 23:35:15.000000 diamond-hpc-0.0.3/diamond/container/custom_image_builder/exception/RegisterImageException.py
+-rw-r--r--   0 hotine    (1000) hotine    (1000)        0 2024-05-21 23:35:15.000000 diamond-hpc-0.0.3/diamond/container/custom_image_builder/exception/__init__.py
+-rw-r--r--   0 hotine    (1000) hotine    (1000)     7174 2024-05-28 00:38:00.000000 diamond-hpc-0.0.3/diamond/container/custom_image_builder/image_builder.py
+drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-05-30 03:44:36.752491 diamond-hpc-0.0.3/diamond/diamond_client/
+-rw-r--r--   0 hotine    (1000) hotine    (1000)        0 2024-05-28 00:38:00.000000 diamond-hpc-0.0.3/diamond/diamond_client/__init__.py
+-rw-r--r--   0 hotine    (1000) hotine    (1000)     2788 2024-05-30 03:43:25.000000 diamond-hpc-0.0.3/diamond/diamond_client/diamond_client.py
+drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-05-30 03:44:36.752491 diamond-hpc-0.0.3/diamond/diamond_client/templates/
+-rw-r--r--   0 hotine    (1000) hotine    (1000)      772 2024-05-28 00:38:00.000000 diamond-hpc-0.0.3/diamond/diamond_client/templates/task_template
+drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-05-30 03:44:36.752491 diamond-hpc-0.0.3/diamond/wrapper/
+-rw-r--r--   0 hotine    (1000) hotine    (1000)        0 2024-05-21 23:35:15.000000 diamond-hpc-0.0.3/diamond/wrapper/__init__.py
+-rw-r--r--   0 hotine    (1000) hotine    (1000)     2210 2024-05-30 03:43:25.000000 diamond-hpc-0.0.3/diamond/wrapper/wrapper.py
+drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-05-30 03:44:36.752491 diamond-hpc-0.0.3/diamond_hpc.egg-info/
+-rw-r--r--   0 hotine    (1000) hotine    (1000)     1484 2024-05-30 03:44:36.000000 diamond-hpc-0.0.3/diamond_hpc.egg-info/PKG-INFO
+-rw-r--r--   0 hotine    (1000) hotine    (1000)      814 2024-05-30 03:44:36.000000 diamond-hpc-0.0.3/diamond_hpc.egg-info/SOURCES.txt
+-rw-r--r--   0 hotine    (1000) hotine    (1000)        1 2024-05-30 03:44:36.000000 diamond-hpc-0.0.3/diamond_hpc.egg-info/dependency_links.txt
+-rw-r--r--   0 hotine    (1000) hotine    (1000)       61 2024-05-30 03:44:36.000000 diamond-hpc-0.0.3/diamond_hpc.egg-info/entry_points.txt
+-rw-r--r--   0 hotine    (1000) hotine    (1000)       71 2024-05-30 03:44:36.000000 diamond-hpc-0.0.3/diamond_hpc.egg-info/requires.txt
+-rw-r--r--   0 hotine    (1000) hotine    (1000)        8 2024-05-30 03:44:36.000000 diamond-hpc-0.0.3/diamond_hpc.egg-info/top_level.txt
+-rw-r--r--   0 hotine    (1000) hotine    (1000)       38 2024-05-30 03:44:36.752491 diamond-hpc-0.0.3/setup.cfg
+-rw-r--r--   0 hotine    (1000) hotine    (1000)      971 2024-05-30 03:43:25.000000 diamond-hpc-0.0.3/setup.py
```

### Comparing `diamond-hpc-0.0.2/LICENSE` & `diamond-hpc-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `diamond-hpc-0.0.2/PKG-INFO` & `diamond-hpc-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diamond-hpc
-Version: 0.0.2
+Version: 0.0.3
 Summary: Diamond is a Python package for running tasks on HPC.
 Home-page: https://github.com/Diamond-Proj/Diamond
 Author: Haotian XIE, Gengcong YANG
 Author-email: hotinexie@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `diamond-hpc-0.0.2/README.md` & `diamond-hpc-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `diamond-hpc-0.0.2/diamond/container/container.py` & `diamond-hpc-0.0.3/diamond/container/container.py`

 * *Files identical despite different names*

### Comparing `diamond-hpc-0.0.2/diamond/container/custom_image_builder/image_builder.py` & `diamond-hpc-0.0.3/diamond/container/custom_image_builder/image_builder.py`

 * *Files identical despite different names*

### Comparing `diamond-hpc-0.0.2/diamond/diamond_client/templates/task_template` & `diamond-hpc-0.0.3/diamond/diamond_client/templates/task_template`

 * *Files identical despite different names*

### Comparing `diamond-hpc-0.0.2/diamond/wrapper/wrapper.py` & `diamond-hpc-0.0.3/diamond/wrapper/wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,9 +40,18 @@
 @click.option('--base_image', required=True, help='Base image name in docker hub')
 def register_container(endpoint_id: str,work_path: str,image_file_name: str,base_image: str):
     diamond = DiamondClient()
     container_id = diamond.register_container(endpoint_id, work_path, image_file_name, base_image)
     click.echo(f"The container id is {container_id}")
 
 
+@cli.command()
+def get_oauth2_url_and_login():
+    diamond = DiamondClient()
+    auth_client = diamond.get_auth_client()
+    click.echo(diamond.get_oauth2_url(auth_client))
+    auth_code = input("Please input the auth code: ")
+    click.echo(diamond.oauth2_login_by_token(auth_client, auth_code))
+
+
 if __name__ == '__main__':
     cli()
```

### Comparing `diamond-hpc-0.0.2/diamond_hpc.egg-info/PKG-INFO` & `diamond-hpc-0.0.3/diamond_hpc.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diamond-hpc
-Version: 0.0.2
+Version: 0.0.3
 Summary: Diamond is a Python package for running tasks on HPC.
 Home-page: https://github.com/Diamond-Proj/Diamond
 Author: Haotian XIE, Gengcong YANG
 Author-email: hotinexie@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `diamond-hpc-0.0.2/diamond_hpc.egg-info/SOURCES.txt` & `diamond-hpc-0.0.3/diamond_hpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `diamond-hpc-0.0.2/setup.py` & `diamond-hpc-0.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="diamond-hpc",
-    version="0.0.2",
+    version="0.0.3",
     author="Haotian XIE, Gengcong YANG",
     author_email="hotinexie@gmail.com",
     description="Diamond is a Python package for running tasks on HPC.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Diamond-Proj/Diamond",
     packages=find_packages(),
```

