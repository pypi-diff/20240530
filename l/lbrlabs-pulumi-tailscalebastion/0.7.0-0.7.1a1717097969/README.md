# Comparing `tmp/lbrlabs_pulumi_tailscalebastion-0.7.0.tar.gz` & `tmp/lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lbrlabs_pulumi_tailscalebastion-0.7.0.tar", last modified: Fri Apr 12 18:28:38 2024, max compression
+gzip compressed data, was "dist/lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969.tar", last modified: Thu May 30 19:43:52 2024, max compression
```

## Comparing `lbrlabs_pulumi_tailscalebastion-0.7.0.tar` & `lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:28:38.000000 lbrlabs_pulumi_tailscalebastion-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-12 18:28:38.000000 lbrlabs_pulumi_tailscalebastion-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-12 18:28:37.000000 lbrlabs_pulumi_tailscalebastion-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:28:38.000000 lbrlabs_pulumi_tailscalebastion-0.7.0/lbrlabs_pulumi_tailscalebastion/
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-12 18:28:37.000000 lbrlabs_pulumi_tailscalebastion-0.7.0/lbrlabs_pulumi_tailscalebastion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8090 2024-04-12 18:28:37.000000 lbrlabs_pulumi_tailscalebastion-0.7.0/lbrlabs_pulumi_tailscalebastion/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:28:38.000000 lbrlabs_pulumi_tailscalebastion-0.7.0/lbrlabs_pulumi_tailscalebastion/aws/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-12 18:28:37.000000 lbrlabs_pulumi_tailscalebastion-0.7.0/lbrlabs_pulumi_tailscalebastion/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15956 2024-04-12 18:28:37.000000 lbrlabs_pulumi_tailscalebastion-0.7.0/lbrlabs_pulumi_tailscalebastion/aws/bastion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:28:38.000000 lbrlabs_pulumi_tailscalebastion-0.7.0/lbrlabs_pulumi_tailscalebastion/azure/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-12 18:28:37.000000 lbrlabs_pulumi_tailscalebastion-0.7.0/lbrlabs_pulumi_tailscalebastion/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12838 2024-04-12 18:28:37.000000 lbrlabs_pulumi_tailscalebastion-0.7.0/lbrlabs_pulumi_tailscalebastion/azure/bastion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:28:38.000000 lbrlabs_pulumi_tailscalebastion-0.7.0/lbrlabs_pulumi_tailscalebastion/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-12 18:28:37.000000 lbrlabs_pulumi_tailscalebastion-0.7.0/lbrlabs_pulumi_tailscalebastion/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-04-12 18:28:37.000000 lbrlabs_pulumi_tailscalebastion-0.7.0/lbrlabs_pulumi_tailscalebastion/kubernetes/bastion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-04-12 18:28:37.000000 lbrlabs_pulumi_tailscalebastion-0.7.0/lbrlabs_pulumi_tailscalebastion/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-12 18:28:37.000000 lbrlabs_pulumi_tailscalebastion-0.7.0/lbrlabs_pulumi_tailscalebastion/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 18:28:37.000000 lbrlabs_pulumi_tailscalebastion-0.7.0/lbrlabs_pulumi_tailscalebastion/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:28:38.000000 lbrlabs_pulumi_tailscalebastion-0.7.0/lbrlabs_pulumi_tailscalebastion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-12 18:28:38.000000 lbrlabs_pulumi_tailscalebastion-0.7.0/lbrlabs_pulumi_tailscalebastion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-12 18:28:38.000000 lbrlabs_pulumi_tailscalebastion-0.7.0/lbrlabs_pulumi_tailscalebastion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 18:28:38.000000 lbrlabs_pulumi_tailscalebastion-0.7.0/lbrlabs_pulumi_tailscalebastion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 18:28:38.000000 lbrlabs_pulumi_tailscalebastion-0.7.0/lbrlabs_pulumi_tailscalebastion.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-12 18:28:38.000000 lbrlabs_pulumi_tailscalebastion-0.7.0/lbrlabs_pulumi_tailscalebastion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-12 18:28:38.000000 lbrlabs_pulumi_tailscalebastion-0.7.0/lbrlabs_pulumi_tailscalebastion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 18:28:38.000000 lbrlabs_pulumi_tailscalebastion-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-12 18:28:37.000000 lbrlabs_pulumi_tailscalebastion-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:43:52.000000 lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969/
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-30 19:43:52.000000 lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-30 19:43:52.000000 lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:43:52.000000 lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969/lbrlabs_pulumi_tailscalebastion/
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-30 19:43:52.000000 lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969/lbrlabs_pulumi_tailscalebastion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8090 2024-05-30 19:43:52.000000 lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969/lbrlabs_pulumi_tailscalebastion/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:43:52.000000 lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969/lbrlabs_pulumi_tailscalebastion/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-30 19:43:52.000000 lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969/lbrlabs_pulumi_tailscalebastion/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15956 2024-05-30 19:43:52.000000 lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969/lbrlabs_pulumi_tailscalebastion/aws/bastion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:43:52.000000 lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969/lbrlabs_pulumi_tailscalebastion/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-30 19:43:52.000000 lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969/lbrlabs_pulumi_tailscalebastion/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12838 2024-05-30 19:43:52.000000 lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969/lbrlabs_pulumi_tailscalebastion/azure/bastion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:43:52.000000 lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969/lbrlabs_pulumi_tailscalebastion/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-30 19:43:52.000000 lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969/lbrlabs_pulumi_tailscalebastion/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-05-30 19:43:52.000000 lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969/lbrlabs_pulumi_tailscalebastion/kubernetes/bastion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-05-30 19:43:52.000000 lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969/lbrlabs_pulumi_tailscalebastion/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-30 19:43:52.000000 lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969/lbrlabs_pulumi_tailscalebastion/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:43:52.000000 lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969/lbrlabs_pulumi_tailscalebastion/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:43:52.000000 lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969/lbrlabs_pulumi_tailscalebastion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-30 19:43:52.000000 lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969/lbrlabs_pulumi_tailscalebastion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-30 19:43:52.000000 lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969/lbrlabs_pulumi_tailscalebastion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 19:43:52.000000 lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969/lbrlabs_pulumi_tailscalebastion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 19:43:52.000000 lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969/lbrlabs_pulumi_tailscalebastion.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-30 19:43:52.000000 lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969/lbrlabs_pulumi_tailscalebastion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-30 19:43:52.000000 lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969/lbrlabs_pulumi_tailscalebastion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 19:43:52.000000 lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-30 19:43:52.000000 lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969/setup.py
```

### Comparing `lbrlabs_pulumi_tailscalebastion-0.7.0/PKG-INFO` & `lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbrlabs_pulumi_tailscalebastion
-Version: 0.7.0
+Version: 0.7.1a1717097969
 Summary: A Pulumi package for creating a tailscale bastion in AWS.
 Home-page: UNKNOWN
 License: UNKNOWN
 Project-URL: Repository, https://github.com/lbrlabs/pulumi-tailscale-bastion
 Description: # Pulumi Tailscale Bastion
         
         This repo provides a [multi-language](https://www.pulumi.com/blog/pulumiup-pulumi-packages-multi-language-components/) component that creates a [Tailscale](https://tailscale.com/) [Subnet Router](https://tailscale.com/kb/1019/subnets/) in your chosen cloud provider
```

### Comparing `lbrlabs_pulumi_tailscalebastion-0.7.0/README.md` & `lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969/README.md`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_tailscalebastion-0.7.0/lbrlabs_pulumi_tailscalebastion/__init__.py` & `lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969/lbrlabs_pulumi_tailscalebastion/__init__.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_tailscalebastion-0.7.0/lbrlabs_pulumi_tailscalebastion/_utilities.py` & `lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969/lbrlabs_pulumi_tailscalebastion/_utilities.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_tailscalebastion-0.7.0/lbrlabs_pulumi_tailscalebastion/aws/bastion.py` & `lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969/lbrlabs_pulumi_tailscalebastion/aws/bastion.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_tailscalebastion-0.7.0/lbrlabs_pulumi_tailscalebastion/azure/bastion.py` & `lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969/lbrlabs_pulumi_tailscalebastion/azure/bastion.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_tailscalebastion-0.7.0/lbrlabs_pulumi_tailscalebastion/kubernetes/bastion.py` & `lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969/lbrlabs_pulumi_tailscalebastion/kubernetes/bastion.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_tailscalebastion-0.7.0/lbrlabs_pulumi_tailscalebastion/provider.py` & `lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969/lbrlabs_pulumi_tailscalebastion/provider.py`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_tailscalebastion-0.7.0/lbrlabs_pulumi_tailscalebastion.egg-info/PKG-INFO` & `lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969/lbrlabs_pulumi_tailscalebastion.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbrlabs-pulumi-tailscalebastion
-Version: 0.7.0
+Version: 0.7.1a1717097969
 Summary: A Pulumi package for creating a tailscale bastion in AWS.
 Home-page: UNKNOWN
 License: UNKNOWN
 Project-URL: Repository, https://github.com/lbrlabs/pulumi-tailscale-bastion
 Description: # Pulumi Tailscale Bastion
         
         This repo provides a [multi-language](https://www.pulumi.com/blog/pulumiup-pulumi-packages-multi-language-components/) component that creates a [Tailscale](https://tailscale.com/) [Subnet Router](https://tailscale.com/kb/1019/subnets/) in your chosen cloud provider
```

### Comparing `lbrlabs_pulumi_tailscalebastion-0.7.0/lbrlabs_pulumi_tailscalebastion.egg-info/SOURCES.txt` & `lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969/lbrlabs_pulumi_tailscalebastion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lbrlabs_pulumi_tailscalebastion-0.7.0/setup.py` & `lbrlabs_pulumi_tailscalebastion-0.7.1a1717097969/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.7.0"
+VERSION = "0.7.1a1717097969"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "tailscale-bastion Pulumi Package - Development Version"
```

