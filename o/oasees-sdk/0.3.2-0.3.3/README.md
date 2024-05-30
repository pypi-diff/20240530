# Comparing `tmp/oasees_sdk-0.3.2.tar.gz` & `tmp/oasees_sdk-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oasees_sdk-0.3.2.tar", max compression
+gzip compressed data, was "oasees_sdk-0.3.3.tar", max compression
```

## Comparing `oasees_sdk-0.3.2.tar` & `oasees_sdk-0.3.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     4870 2024-05-28 16:04:12.456607 oasees_sdk-0.3.2/README.md
--rw-r--r--   0        0        0      619 2024-05-29 10:42:55.900090 oasees_sdk-0.3.2/pyproject.toml
--rw-r--r--   0        0        0    20827 2024-05-29 08:39:46.120797 oasees_sdk-0.3.2/src/oasees_sdk/cli/__pycache__/cli.cpython-310.pyc
--rw-r--r--   0        0        0    33029 2024-05-24 13:19:35.008849 oasees_sdk-0.3.2/src/oasees_sdk/cli/cli.py
--rw-r--r--   0        0        0       18 2024-05-10 14:31:20.743803 oasees_sdk-0.3.2/src/oasees_sdk/oasees_sdk/__init__.py
--rw-r--r--   0        0        0      177 2024-05-29 10:17:44.127715 oasees_sdk-0.3.2/src/oasees_sdk/oasees_sdk/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1263 2024-05-29 10:17:44.559713 oasees_sdk-0.3.2/src/oasees_sdk/oasees_sdk/__pycache__/cluster_ipfs_upload.cpython-310.pyc
--rw-r--r--   0        0        0     1841 2024-05-29 10:17:44.555713 oasees_sdk-0.3.2/src/oasees_sdk/oasees_sdk/__pycache__/deploy_pipeline.cpython-310.pyc
--rw-r--r--   0        0        0     9078 2024-05-29 10:33:09.879030 oasees_sdk-0.3.2/src/oasees_sdk/oasees_sdk/__pycache__/sdk.cpython-310.pyc
--rw-r--r--   0        0        0      887 2024-05-10 14:31:20.755803 oasees_sdk-0.3.2/src/oasees_sdk/oasees_sdk/cluster_ipfs_upload.py
--rw-r--r--   0        0        0     1934 2024-05-10 14:31:20.699804 oasees_sdk-0.3.2/src/oasees_sdk/oasees_sdk/deploy_pipeline.py
--rw-r--r--   0        0        0    11113 2024-05-29 10:42:25.404243 oasees_sdk-0.3.2/src/oasees_sdk/oasees_sdk/sdk.py
--rw-r--r--   0        0        0     5934 1970-01-01 00:00:00.000000 oasees_sdk-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     4870 2024-05-28 16:04:12.456607 oasees_sdk-0.3.3/README.md
+-rw-r--r--   0        0        0      619 2024-05-30 14:15:40.973680 oasees_sdk-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0    20827 2024-05-29 08:39:46.120797 oasees_sdk-0.3.3/src/oasees_sdk/cli/__pycache__/cli.cpython-310.pyc
+-rw-r--r--   0        0        0    33424 2024-05-30 11:13:00.076930 oasees_sdk-0.3.3/src/oasees_sdk/cli/cli.py
+-rw-r--r--   0        0        0       18 2024-05-10 14:31:20.743803 oasees_sdk-0.3.3/src/oasees_sdk/oasees_sdk/__init__.py
+-rw-r--r--   0        0        0      177 2024-05-29 10:17:44.127715 oasees_sdk-0.3.3/src/oasees_sdk/oasees_sdk/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1263 2024-05-29 10:17:44.559713 oasees_sdk-0.3.3/src/oasees_sdk/oasees_sdk/__pycache__/cluster_ipfs_upload.cpython-310.pyc
+-rw-r--r--   0        0        0     1841 2024-05-29 10:17:44.555713 oasees_sdk-0.3.3/src/oasees_sdk/oasees_sdk/__pycache__/deploy_pipeline.cpython-310.pyc
+-rw-r--r--   0        0        0     9078 2024-05-29 10:33:09.879030 oasees_sdk-0.3.3/src/oasees_sdk/oasees_sdk/__pycache__/sdk.cpython-310.pyc
+-rw-r--r--   0        0        0      887 2024-05-10 14:31:20.755803 oasees_sdk-0.3.3/src/oasees_sdk/oasees_sdk/cluster_ipfs_upload.py
+-rw-r--r--   0        0        0     1934 2024-05-10 14:31:20.699804 oasees_sdk-0.3.3/src/oasees_sdk/oasees_sdk/deploy_pipeline.py
+-rw-r--r--   0        0        0    11113 2024-05-29 10:42:25.404243 oasees_sdk-0.3.3/src/oasees_sdk/oasees_sdk/sdk.py
+-rw-r--r--   0        0        0     5934 1970-01-01 00:00:00.000000 oasees_sdk-0.3.3/PKG-INFO
```

### Comparing `oasees_sdk-0.3.2/README.md` & `oasees_sdk-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `oasees_sdk-0.3.2/pyproject.toml` & `oasees_sdk-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "oasees_sdk"
-version = "0.3.2"
+version = "0.3.3"
 description = "Oasees SDK"
 authors = [
     "Example Author <author@example.com>",
 ]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `oasees_sdk-0.3.2/src/oasees_sdk/cli/__pycache__/cli.cpython-310.pyc` & `oasees_sdk-0.3.3/src/oasees_sdk/cli/__pycache__/cli.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `oasees_sdk-0.3.2/src/oasees_sdk/cli/cli.py` & `oasees_sdk-0.3.3/src/oasees_sdk/cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,22 +281,27 @@
             click.echo("Enter a valid role (master / agent)")
     except FileNotFoundError:
         click.echo("Error: Uninstall executable not found.")
 
 @cli.command()
 @click.option('--ip', required=True, help="The cluster's master ip address.")
 @click.option('--token', required=True, help="The cluster's master token.")
-def join_cluster(ip,token):
-    '''Joins the current machine to the specified cluster.'''
+@click.option('--iface', required=False, help="The network interface you want to join with (tun0 if you're using a VPN connection).")
+def join_cluster(ip,token,iface):
+    '''Joins the current machine to the specified cluster, using the specified interface if one is provided.'''
     try:
         mkdir_1 = subprocess.run(['sudo','mkdir','/etc/rancher'], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
         mkdir_2 = subprocess.run(['sudo','mkdir','/etc/rancher/k3s'], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
         echo = subprocess.run(['sudo','sh', '-c','echo "mirrors:\n  docker.io:\n  registry.k8s.io:" > /etc/rancher/k3s/registries.yaml'], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
         curl = subprocess.Popen(['curl','-sfL', 'https://get.k3s.io'], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
-        result = subprocess.check_output(['sh','-'], env={'K3S_URL' : 'https://'+ip+':6443', 'K3S_TOKEN': token}, stdin=curl.stdout)
+
+        if(iface):
+            result = subprocess.check_output(['sh','-s','-','--flannel-iface', iface], env={'K3S_URL' : 'https://'+ip+':6443', 'K3S_TOKEN': token}, stdin=curl.stdout)
+        else:
+            result = subprocess.check_output(['sh','-'], env={'K3S_URL' : 'https://'+ip+':6443', 'K3S_TOKEN': token}, stdin=curl.stdout)
         click.echo(result)
         curl.wait()
     except FileNotFoundError:
         click.echo("Error: K3S cluster could not be joined.\n")
             
 
 @cli.command()
```

### Comparing `oasees_sdk-0.3.2/src/oasees_sdk/oasees_sdk/__pycache__/cluster_ipfs_upload.cpython-310.pyc` & `oasees_sdk-0.3.3/src/oasees_sdk/oasees_sdk/__pycache__/cluster_ipfs_upload.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `oasees_sdk-0.3.2/src/oasees_sdk/oasees_sdk/__pycache__/deploy_pipeline.cpython-310.pyc` & `oasees_sdk-0.3.3/src/oasees_sdk/oasees_sdk/__pycache__/deploy_pipeline.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `oasees_sdk-0.3.2/src/oasees_sdk/oasees_sdk/__pycache__/sdk.cpython-310.pyc` & `oasees_sdk-0.3.3/src/oasees_sdk/oasees_sdk/__pycache__/sdk.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `oasees_sdk-0.3.2/src/oasees_sdk/oasees_sdk/cluster_ipfs_upload.py` & `oasees_sdk-0.3.3/src/oasees_sdk/oasees_sdk/cluster_ipfs_upload.py`

 * *Files identical despite different names*

### Comparing `oasees_sdk-0.3.2/src/oasees_sdk/oasees_sdk/deploy_pipeline.py` & `oasees_sdk-0.3.3/src/oasees_sdk/oasees_sdk/deploy_pipeline.py`

 * *Files identical despite different names*

### Comparing `oasees_sdk-0.3.2/src/oasees_sdk/oasees_sdk/sdk.py` & `oasees_sdk-0.3.3/src/oasees_sdk/oasees_sdk/sdk.py`

 * *Files identical despite different names*

### Comparing `oasees_sdk-0.3.2/PKG-INFO` & `oasees_sdk-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oasees_sdk
-Version: 0.3.2
+Version: 0.3.3
 Summary: Oasees SDK
 Author: Example Author
 Author-email: author@example.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

