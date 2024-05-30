# Comparing `tmp/k8ctl-0.0.3-py3-none-any.whl.zip` & `tmp/k8ctl-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 9965 bytes, number of entries: 9
--rw-r--r--  2.0 unx        0 b- defN 24-May-30 05:37 k8ctl/__init__.py
--rw-r--r--  2.0 unx     1200 b- defN 24-May-30 05:37 k8ctl/helper.py
--rw-r--r--  2.0 unx    15374 b- defN 24-May-30 05:37 k8ctl/k8ctl.py
--rw-r--r--  2.0 unx    11357 b- defN 24-May-30 05:37 k8ctl-0.0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     1481 b- defN 24-May-30 05:37 k8ctl-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-30 05:37 k8ctl-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       38 b- defN 24-May-30 05:37 k8ctl-0.0.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 24-May-30 05:37 k8ctl-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      684 b- defN 24-May-30 05:37 k8ctl-0.0.3.dist-info/RECORD
-9 files, 30232 bytes uncompressed, 8793 bytes compressed:  70.9%
+Zip file size: 10127 bytes, number of entries: 9
+-rw-r--r--  2.0 unx        0 b- defN 24-May-30 10:24 k8ctl/__init__.py
+-rw-r--r--  2.0 unx     1246 b- defN 24-May-30 10:24 k8ctl/helper.py
+-rw-r--r--  2.0 unx    16623 b- defN 24-May-30 10:24 k8ctl/k8ctl.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-May-30 10:24 k8ctl-0.0.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1481 b- defN 24-May-30 10:24 k8ctl-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-30 10:24 k8ctl-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       38 b- defN 24-May-30 10:24 k8ctl-0.0.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 24-May-30 10:24 k8ctl-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      684 b- defN 24-May-30 10:24 k8ctl-0.0.4.dist-info/RECORD
+9 files, 31527 bytes uncompressed, 8955 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: k8ctl/helper.py
 Comment: 
 
 Filename: k8ctl/k8ctl.py
 Comment: 
 
-Filename: k8ctl-0.0.3.dist-info/LICENSE
+Filename: k8ctl-0.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: k8ctl-0.0.3.dist-info/METADATA
+Filename: k8ctl-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: k8ctl-0.0.3.dist-info/WHEEL
+Filename: k8ctl-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: k8ctl-0.0.3.dist-info/entry_points.txt
+Filename: k8ctl-0.0.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: k8ctl-0.0.3.dist-info/top_level.txt
+Filename: k8ctl-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: k8ctl-0.0.3.dist-info/RECORD
+Filename: k8ctl-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## k8ctl/helper.py

```diff
@@ -29,8 +29,12 @@
 def current_cluster():
     '''
     Get the current cluster
     '''
     cmd = "kubectl config current-context"
     result = subprocess.run(cmd, shell=True, check=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
 
-    return result.stdout.decode('utf-8').strip()
+    return result.stdout.decode('utf-8').strip()
+
+
+def hello_world():
+    print("Hello World")
```

## k8ctl/k8ctl.py

```diff
@@ -1,19 +1,63 @@
 import click
 import subprocess
 import os
-import helper
+# import helper
 # import logging
 
 rancher_url = os.getenv("RANCHER_URL")
 
 # log = logging.getLogger(__name__)
 # log.setLevel(logging.DEBUG)
 # log.addHandler(logging.StreamHandler())
 
+## helper functions
+
+def check_token_validlity():
+    '''
+    Check if the token is still valid
+    '''
+    result = subprocess.run("kubectl get po", shell=True, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
+
+    return result.returncode
+
+def list_env(app):
+    '''
+    List all environment variables
+    '''
+    cmd = """kubectl get secret {}""".format(app) + ''' -o jsonpath="{.data}" '''
+    cmd2= cmd + """ | jq -r 'to_entries|map("\(.key)=\(.value | @base64d)")|.[]' """
+
+    result = subprocess.run(cmd, shell=True, stdout=subprocess.DEVNULL, stderr=subprocess.PIPE)
+
+    # checking whether the secret exists
+    if result.returncode != 0:
+        print("Failed to list the environment variables. May be app not found")
+        return 404
+    
+    result2 = subprocess.run(cmd2, shell=True, check=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, input=result.stdout)
+
+    return result2.stdout.decode('utf-8').strip()
+
+def current_cluster():
+    '''
+    Get the current cluster
+    '''
+    cmd = "kubectl config current-context"
+    result = subprocess.run(cmd, shell=True, check=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+
+    return result.stdout.decode('utf-8').strip()
+
+
+def hello_world():
+    print("Hello World")
+
+
+## Program starts here
+
 @click.group()
 def k8ctl():
     '''
     k8ctl is a command line tool for managing rancher multicluster kubernetes environments
     '''
     pass
 
@@ -133,15 +177,15 @@
         click.echo(f"No")
         return 1
     elif dummy == cluster:
         current_cluster.returncode = 0
     else:
         current_cluster.returncode = 1
 
-    if current_cluster.returncode == 0 and helper.check_token_validlity() == 0:
+    if current_cluster.returncode == 0 and check_token_validlity() == 0:
         click.echo(f"Already logged into {cluster}")
         return 0
     
     elif result.returncode != 0:
         click.echo(f"Cluster {cluster} config not found")
 
         subprocess.run(f"touch ~/.kube/{cluster}", shell=True, check=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
@@ -153,15 +197,15 @@
             click.echo("Failed to switch to the cluster")
             return 1
         else:
             click.echo(f"{cluster} config is stored in ~/.kube/")
             
     copy_config = subprocess.run(f"cp ~/.kube/{cluster} ~/.kube/config", shell=True, check=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
     
-    if helper.check_token_validlity() != 0:
+    if check_token_validlity() != 0:
         click.echo("Token has expired. So, logging in again")
 
         subprocess.run(f"> ~/.kube/{cluster}", shell=True, check=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
 
         with open(os.path.expanduser(f"~/.kube/{cluster}"), "w") as f:
             config_write = subprocess.run(f"rancher cluster kf {cluster}", shell=True, stdout=f, stderr=subprocess.PIPE, text=True)
         
@@ -223,15 +267,15 @@
             try:
                 env_vars.append(input())
             except EOFError:
                 break
 
     env_vars = dict([env_var.split('=', 1) for env_var in env_vars])
 
-    last_env = helper.list_env(app).strip()
+    last_env = list_env(app).strip()
     last_env = dict([env.split('=', 1) for env in last_env.split('\n')])
 
     for key, value in env_vars.items():
         last_env[key] = value
 
     with open("/tmp/env_{}.env".format(app), "w") as f:
         for key, value in last_env.items():
@@ -324,15 +368,15 @@
 @click.option('--app', '-a', prompt=True, help='The application name to deploy', required=True)
 def psql(app):
     '''
     Connect to the application database
     '''
 
     # get the db url
-    env_vars = helper.list_env(app)
+    env_vars = list_env(app)
     if env_vars == 404:
         return
 
     # split with first '='
     env_vars = dict([env_var.split('=', 1) for env_var in env_vars.split('\n')])
 
     if "DASHBOARD_DB_URL" not in env_vars and "DB_URL" not in env_vars and "DATABASE_URL" not in env_vars:
```

## Comparing `k8ctl-0.0.3.dist-info/LICENSE` & `k8ctl-0.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `k8ctl-0.0.3.dist-info/METADATA` & `k8ctl-0.0.4.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k8ctl
-Version: 0.0.3
+Version: 0.0.4
 Author: Kishorekarthik P
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 
 # k8ctl
```

