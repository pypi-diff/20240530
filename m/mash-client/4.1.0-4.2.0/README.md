# Comparing `tmp/mash-client-4.1.0.tar.gz` & `tmp/mash_client-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mash-client-4.1.0.tar", last modified: Wed Dec  7 19:52:47 2022, max compression
+gzip compressed data, was "mash_client-4.2.0.tar", last modified: Thu May 30 14:12:02 2024, max compression
```

## Comparing `mash-client-4.1.0.tar` & `mash_client-4.2.0.tar`

### file list

```diff
@@ -1,50 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 19:52:47.588014 mash-client-4.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     6420 2022-12-07 19:52:39.000000 mash-client-4.1.0/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2022-12-07 19:52:39.000000 mash-client-4.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    32403 2022-12-07 19:52:39.000000 mash-client-4.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      287 2022-12-07 19:52:39.000000 mash-client-4.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2022-12-07 19:52:47.588014 mash-client-4.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2022-12-07 19:52:39.000000 mash-client-4.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 19:52:47.584014 mash-client-4.1.0/man/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 19:52:47.588014 mash-client-4.1.0/man/man5/
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2022-12-07 19:52:39.000000 mash-client-4.1.0/man/man5/mash_client.conf.5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 19:52:47.588014 mash-client-4.1.0/mash_client/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2022-12-07 19:52:39.000000 mash-client-4.1.0/mash_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 19:52:47.588014 mash-client-4.1.0/mash_client/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2022-12-07 19:52:39.000000 mash-client-4.1.0/mash_client/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 19:52:47.588014 mash-client-4.1.0/mash_client/cli/account/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2022-12-07 19:52:39.000000 mash-client-4.1.0/mash_client/cli/account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7466 2022-12-07 19:52:39.000000 mash-client-4.1.0/mash_client/cli/account/aliyun.py
--rw-r--r--   0 runner    (1001) docker     (123)     7299 2022-12-07 19:52:39.000000 mash-client-4.1.0/mash_client/cli/account/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     7710 2022-12-07 19:52:39.000000 mash-client-4.1.0/mash_client/cli/account/ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2022-12-07 19:52:39.000000 mash-client-4.1.0/mash_client/cli/account/gce.py
--rw-r--r--   0 runner    (1001) docker     (123)     7697 2022-12-07 19:52:39.000000 mash-client-4.1.0/mash_client/cli/account/oci.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 19:52:47.588014 mash-client-4.1.0/mash_client/cli/auth/
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2022-12-07 19:52:39.000000 mash-client-4.1.0/mash_client/cli/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2022-12-07 19:52:39.000000 mash-client-4.1.0/mash_client/cli/auth/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     5211 2022-12-07 19:52:39.000000 mash-client-4.1.0/mash_client/cli/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 19:52:47.588014 mash-client-4.1.0/mash_client/cli/job/
--rw-r--r--   0 runner    (1001) docker     (123)     6833 2022-12-07 19:52:39.000000 mash-client-4.1.0/mash_client/cli/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2022-12-07 19:52:39.000000 mash-client-4.1.0/mash_client/cli/job/aliyun.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2022-12-07 19:52:39.000000 mash-client-4.1.0/mash_client/cli/job/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2022-12-07 19:52:39.000000 mash-client-4.1.0/mash_client/cli/job/ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2022-12-07 19:52:39.000000 mash-client-4.1.0/mash_client/cli/job/gce.py
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2022-12-07 19:52:39.000000 mash-client-4.1.0/mash_client/cli/job/oci.py
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2022-12-07 19:52:39.000000 mash-client-4.1.0/mash_client/cli/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    13801 2022-12-07 19:52:39.000000 mash-client-4.1.0/mash_client/cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6106 2022-12-07 19:52:39.000000 mash-client-4.1.0/mash_client/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2022-12-07 19:52:39.000000 mash-client-4.1.0/mash_client/mash_client_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 19:52:47.588014 mash-client-4.1.0/mash_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2022-12-07 19:52:47.000000 mash-client-4.1.0/mash_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2022-12-07 19:52:47.000000 mash-client-4.1.0/mash_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-07 19:52:47.000000 mash-client-4.1.0/mash_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2022-12-07 19:52:47.000000 mash-client-4.1.0/mash_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-07 19:52:47.000000 mash-client-4.1.0/mash_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      129 2022-12-07 19:52:47.000000 mash-client-4.1.0/mash_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2022-12-07 19:52:47.000000 mash-client-4.1.0/mash_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 19:52:47.588014 mash-client-4.1.0/package/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2022-12-07 19:52:39.000000 mash-client-4.1.0/package/mash-client.spec
--rw-r--r--   0 runner    (1001) docker     (123)       87 2022-12-07 19:52:39.000000 mash-client-4.1.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2022-12-07 19:52:39.000000 mash-client-4.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      330 2022-12-07 19:52:47.592014 mash-client-4.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2022-12-07 19:52:39.000000 mash-client-4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:12:02.650372 mash_client-4.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-30 14:11:54.000000 mash_client-4.2.0/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-05-30 14:11:54.000000 mash_client-4.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    32403 2024-05-30 14:11:54.000000 mash_client-4.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-30 14:11:54.000000 mash_client-4.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-05-30 14:12:02.650372 mash_client-4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-30 14:11:54.000000 mash_client-4.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:12:02.638372 mash_client-4.2.0/man/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:12:02.638372 mash_client-4.2.0/man/man5/
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-30 14:11:54.000000 mash_client-4.2.0/man/man5/mash_client.conf.5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:12:02.642372 mash_client-4.2.0/mash_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-30 14:11:54.000000 mash_client-4.2.0/mash_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:12:02.642372 mash_client-4.2.0/mash_client/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-05-30 14:11:54.000000 mash_client-4.2.0/mash_client/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:12:02.642372 mash_client-4.2.0/mash_client/cli/account/
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-30 14:11:54.000000 mash_client-4.2.0/mash_client/cli/account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7466 2024-05-30 14:11:54.000000 mash_client-4.2.0/mash_client/cli/account/aliyun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-05-30 14:11:54.000000 mash_client-4.2.0/mash_client/cli/account/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7710 2024-05-30 14:11:54.000000 mash_client-4.2.0/mash_client/cli/account/ec2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-05-30 14:11:54.000000 mash_client-4.2.0/mash_client/cli/account/gce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7697 2024-05-30 14:11:54.000000 mash_client-4.2.0/mash_client/cli/account/oci.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:12:02.642372 mash_client-4.2.0/mash_client/cli/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-30 14:11:54.000000 mash_client-4.2.0/mash_client/cli/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-05-30 14:11:54.000000 mash_client-4.2.0/mash_client/cli/auth/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-30 14:11:54.000000 mash_client-4.2.0/mash_client/cli/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:12:02.642372 mash_client-4.2.0/mash_client/cli/job/
+-rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-05-30 14:11:54.000000 mash_client-4.2.0/mash_client/cli/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-05-30 14:11:54.000000 mash_client-4.2.0/mash_client/cli/job/aliyun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-30 14:11:54.000000 mash_client-4.2.0/mash_client/cli/job/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-30 14:11:54.000000 mash_client-4.2.0/mash_client/cli/job/ec2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-30 14:11:54.000000 mash_client-4.2.0/mash_client/cli/job/gce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-30 14:11:54.000000 mash_client-4.2.0/mash_client/cli/job/oci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6196 2024-05-30 14:11:54.000000 mash_client-4.2.0/mash_client/cli/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13801 2024-05-30 14:11:54.000000 mash_client-4.2.0/mash_client/cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6106 2024-05-30 14:11:54.000000 mash_client-4.2.0/mash_client/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-30 14:11:54.000000 mash_client-4.2.0/mash_client/mash_client_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:12:02.646371 mash_client-4.2.0/mash_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-05-30 14:12:02.000000 mash_client-4.2.0/mash_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-30 14:12:02.000000 mash_client-4.2.0/mash_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 14:12:02.000000 mash_client-4.2.0/mash_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-30 14:12:02.000000 mash_client-4.2.0/mash_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 14:12:02.000000 mash_client-4.2.0/mash_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-30 14:12:02.000000 mash_client-4.2.0/mash_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 14:12:02.000000 mash_client-4.2.0/mash_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:12:02.642372 mash_client-4.2.0/package/
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-30 14:11:54.000000 mash_client-4.2.0/package/mash-client.spec
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-30 14:11:54.000000 mash_client-4.2.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-30 14:11:54.000000 mash_client-4.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-30 14:12:02.650372 mash_client-4.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-30 14:11:54.000000 mash_client-4.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:12:02.646371 mash_client-4.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-05-30 14:11:54.000000 mash_client-4.2.0/tests/test_aliyun_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-30 14:11:54.000000 mash_client-4.2.0/tests/test_aliyun_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-05-30 14:11:54.000000 mash_client-4.2.0/tests/test_auth_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-05-30 14:11:54.000000 mash_client-4.2.0/tests/test_azure_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-30 14:11:54.000000 mash_client-4.2.0/tests/test_azure_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-30 14:11:54.000000 mash_client-4.2.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-30 14:11:54.000000 mash_client-4.2.0/tests/test_cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-30 14:11:54.000000 mash_client-4.2.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-05-30 14:11:54.000000 mash_client-4.2.0/tests/test_ec2_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-30 14:11:54.000000 mash_client-4.2.0/tests/test_ec2_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-05-30 14:11:54.000000 mash_client-4.2.0/tests/test_gce_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-30 14:11:54.000000 mash_client-4.2.0/tests/test_gce_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-05-30 14:11:54.000000 mash_client-4.2.0/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-05-30 14:11:54.000000 mash_client-4.2.0/tests/test_oci_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-30 14:11:54.000000 mash_client-4.2.0/tests/test_oci_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-05-30 14:11:54.000000 mash_client-4.2.0/tests/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-05-30 14:11:54.000000 mash_client-4.2.0/tests/test_user.py
```

### Comparing `mash-client-4.1.0/CHANGES.md` & `mash_client-4.2.0/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+v4.2.0 (2024-05-30)
+===================
+
+- Update spec to build for 3.11
+- Update python version support
+
 v4.1.0 (2022-12-07)
 ===================
 
 - Add option to create refresh token with no expiry
 
 v4.0.1 (2021-12-17)
 ===================
```

### Comparing `mash-client-4.1.0/CONTRIBUTING.md` & `mash_client-4.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mash-client-4.1.0/LICENSE` & `mash_client-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mash-client-4.1.0/PKG-INFO` & `mash_client-4.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,47 @@
 Metadata-Version: 2.1
 Name: mash-client
-Version: 4.1.0
+Version: 4.2.0
 Summary: CLI client for interfacing with a MASH server.
 Home-page: https://github.com/SUSE-enceladus/mash-client
 Author: SUSE
 Author-email: public-cloud-dev@susecloud.net
 License: GPLv3+
 Keywords: mash-client mash client
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.4
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: Click
+Requires-Dist: requests
+Requires-Dist: PyYAML
+Requires-Dist: PyJWT
+Provides-Extra: dev
+Requires-Dist: Click; extra == "dev"
+Requires-Dist: requests; extra == "dev"
+Requires-Dist: PyYAML; extra == "dev"
+Requires-Dist: PyJWT; extra == "dev"
+Requires-Dist: bumpversion; extra == "dev"
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: Sphinx; extra == "dev"
+Requires-Dist: sphinx-click; extra == "dev"
 
 ![Build Status](https://github.com/SUSE-Enceladus/mash-client/workflows/Continuous%20testing%20&%20Linting/badge.svg?branch=master)
 [![Documentation Status](https://readthedocs.org/projects/mash-client/badge/?version=latest)](https://mash-client.readthedocs.io/en/latest/?badge=latest)
 [![Py Versions](https://img.shields.io/pypi/pyversions/mash-client.svg)](https://pypi.org/project/mash-client/)
 [![License](https://img.shields.io/pypi/l/mash-client.svg)](https://pypi.org/project/mash-client/)
 
 **mash-client**
```

### Comparing `mash-client-4.1.0/README.md` & `mash_client-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mash-client-4.1.0/man/man5/mash_client.conf.5` & `mash_client-4.2.0/man/man5/mash_client.conf.5`

 * *Files identical despite different names*

### Comparing `mash-client-4.1.0/mash_client/__init__.py` & `mash_client-4.2.0/mash_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 __author__ = """SUSE"""
 __email__ = 'public-cloud-dev@susecloud.net'
-__version__ = '4.1.0'
+__version__ = '4.2.0'
```

### Comparing `mash-client-4.1.0/mash_client/cli/__init__.py` & `mash_client-4.2.0/mash_client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `mash-client-4.1.0/mash_client/cli/account/__init__.py` & `mash_client-4.2.0/mash_client/cli/account/__init__.py`

 * *Files identical despite different names*

### Comparing `mash-client-4.1.0/mash_client/cli/account/aliyun.py` & `mash_client-4.2.0/mash_client/cli/account/aliyun.py`

 * *Files identical despite different names*

### Comparing `mash-client-4.1.0/mash_client/cli/account/azure.py` & `mash_client-4.2.0/mash_client/cli/account/azure.py`

 * *Files identical despite different names*

### Comparing `mash-client-4.1.0/mash_client/cli/account/ec2.py` & `mash_client-4.2.0/mash_client/cli/account/ec2.py`

 * *Files identical despite different names*

### Comparing `mash-client-4.1.0/mash_client/cli/account/gce.py` & `mash_client-4.2.0/mash_client/cli/account/gce.py`

 * *Files identical despite different names*

### Comparing `mash-client-4.1.0/mash_client/cli/account/oci.py` & `mash_client-4.2.0/mash_client/cli/account/oci.py`

 * *Files identical despite different names*

### Comparing `mash-client-4.1.0/mash_client/cli/auth/__init__.py` & `mash_client-4.2.0/mash_client/cli/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `mash-client-4.1.0/mash_client/cli/auth/token.py` & `mash_client-4.2.0/mash_client/cli/auth/token.py`

 * *Files identical despite different names*

### Comparing `mash-client-4.1.0/mash_client/cli/config.py` & `mash_client-4.2.0/mash_client/cli/config.py`

 * *Files identical despite different names*

### Comparing `mash-client-4.1.0/mash_client/cli/job/__init__.py` & `mash_client-4.2.0/mash_client/cli/job/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,17 @@
 
     with handle_errors(config_data['log_level'], config_data['no_color']):
         result = get_job(config_data, job_id)
 
         if not show_data:
             with suppress(KeyError):
                 del result['data']
+        elif 'test_results' in result['data']:
+            # Retrieved via `mash job test-results` command
+            del result['data']['test_results']
 
         echo_dict(result, config_data['no_color'])
 
 
 @click.command()
 @click.option(
     '--job-id',
```

### Comparing `mash-client-4.1.0/mash_client/cli/job/aliyun.py` & `mash_client-4.2.0/mash_client/cli/job/aliyun.py`

 * *Files identical despite different names*

### Comparing `mash-client-4.1.0/mash_client/cli/job/azure.py` & `mash_client-4.2.0/mash_client/cli/job/azure.py`

 * *Files identical despite different names*

### Comparing `mash-client-4.1.0/mash_client/cli/job/ec2.py` & `mash_client-4.2.0/mash_client/cli/job/ec2.py`

 * *Files identical despite different names*

### Comparing `mash-client-4.1.0/mash_client/cli/job/gce.py` & `mash_client-4.2.0/mash_client/cli/job/gce.py`

 * *Files identical despite different names*

### Comparing `mash-client-4.1.0/mash_client/cli/job/oci.py` & `mash_client-4.2.0/mash_client/cli/job/oci.py`

 * *Files identical despite different names*

### Comparing `mash-client-4.1.0/mash_client/cli/user.py` & `mash_client-4.2.0/mash_client/cli/user.py`

 * *Files identical despite different names*

### Comparing `mash-client-4.1.0/mash_client/cli_utils.py` & `mash_client-4.2.0/mash_client/cli_utils.py`

 * *Files identical despite different names*

### Comparing `mash-client-4.1.0/mash_client/controller.py` & `mash_client-4.2.0/mash_client/controller.py`

 * *Files identical despite different names*

### Comparing `mash-client-4.1.0/mash_client/mash_client_exceptions.py` & `mash_client-4.2.0/mash_client/mash_client_exceptions.py`

 * *Files identical despite different names*

### Comparing `mash-client-4.1.0/mash_client.egg-info/PKG-INFO` & `mash_client-4.2.0/mash_client.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,47 @@
 Metadata-Version: 2.1
 Name: mash-client
-Version: 4.1.0
+Version: 4.2.0
 Summary: CLI client for interfacing with a MASH server.
 Home-page: https://github.com/SUSE-enceladus/mash-client
 Author: SUSE
 Author-email: public-cloud-dev@susecloud.net
 License: GPLv3+
 Keywords: mash-client mash client
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.4
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: Click
+Requires-Dist: requests
+Requires-Dist: PyYAML
+Requires-Dist: PyJWT
+Provides-Extra: dev
+Requires-Dist: Click; extra == "dev"
+Requires-Dist: requests; extra == "dev"
+Requires-Dist: PyYAML; extra == "dev"
+Requires-Dist: PyJWT; extra == "dev"
+Requires-Dist: bumpversion; extra == "dev"
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: Sphinx; extra == "dev"
+Requires-Dist: sphinx-click; extra == "dev"
 
 ![Build Status](https://github.com/SUSE-Enceladus/mash-client/workflows/Continuous%20testing%20&%20Linting/badge.svg?branch=master)
 [![Documentation Status](https://readthedocs.org/projects/mash-client/badge/?version=latest)](https://mash-client.readthedocs.io/en/latest/?badge=latest)
 [![Py Versions](https://img.shields.io/pypi/pyversions/mash-client.svg)](https://pypi.org/project/mash-client/)
 [![License](https://img.shields.io/pypi/l/mash-client.svg)](https://pypi.org/project/mash-client/)
 
 **mash-client**
```

### Comparing `mash-client-4.1.0/package/mash-client.spec` & `mash_client-4.2.0/package/mash-client.spec`

 * *Files 12% similar despite different names*

```diff
@@ -11,61 +11,70 @@
 # case the license is the MIT License). An "Open Source License" is a
 # license that conforms to the Open Source Definition (Version 1.9)
 # published by the Open Source Initiative.
 
 # Please submit bugfixes or comments via http://bugs.opensuse.org/
 #
 
+%define python python
+%{?sle15_python_module_pythons}
 
 Name:           mash-client
-Version:        4.1.0
+Version:        4.2.0
 Release:        0
 Summary:        Command line utility for MASH server
 License:        GPL-3.0-or-later
 Group:          Development/Languages/Python
 URL:            https://github.com/SUSE-enceladus/mash-client
 Source:         https://files.pythonhosted.org/packages/source/p/mash-client/%{name}-%{version}.tar.gz
 BuildRequires:  python-rpm-macros
-BuildRequires:  python3-devel
-BuildRequires:  python3-setuptools
-BuildRequires:  python3-click
-BuildRequires:  python3-click-man
-BuildRequires:  python3-requests
-BuildRequires:  python3-PyYAML
-BuildRequires:  python3-PyJWT
-Requires:       python3-click
-Requires:       python3-requests
-Requires:       python3-PyYAML
-Requires:       python3-PyJWT
+BuildRequires:  fdupes
+BuildRequires:  %{python_module devel}
+BuildRequires:  %{python_module setuptools}
+BuildRequires:  %{python_module wheel}
+BuildRequires:  %{python_module pip}
+BuildRequires:  %{python_module click}
+BuildRequires:  %{python_module click-man}
+BuildRequires:  %{python_module requests}
+BuildRequires:  %{python_module PyYAML}
+BuildRequires:  %{python_module PyJWT}
+Requires:       python-click
+Requires:       python-requests
+Requires:       python-PyYAML
+Requires:       python-PyJWT
 BuildArch:      noarch
+%python_subpackages
 
 %description
 mash-client provides a command line utility to interface
 with a MASH server instance.
 
 %prep
 %setup -q
 
 %build
-python3 setup.py build
+%pyproject_wheel
 mkdir -p man/man1
-python3 setup.py --command-packages=click_man.commands man_pages --target man/man1
+%python_exec setup.py --command-packages=click_man.commands man_pages --target man/man1
 
 %install
-python3 setup.py install --prefix=%{_prefix} --root=%{buildroot}
+%pyproject_install
+
 install -d -m 755 %{buildroot}/%{_mandir}/man1
 install -d -m 755 %{buildroot}/%{_mandir}/man5
 install -m 644 man/man1/*.1 %{buildroot}/%{_mandir}/man1
 install -m 644 man/man5/*.5 %{buildroot}/%{_mandir}/man5
 gzip %{buildroot}/%{_mandir}/man1/*
 gzip %{buildroot}/%{_mandir}/man5/*
+%{python_expand %fdupes %{buildroot}%{$python_sitelib}}
 
 %files
 %defattr(-,root,root)
 %license LICENSE
 %doc CHANGES.md CONTRIBUTING.md README.md
 %{_mandir}/man1/*
 %{_mandir}/man5/*
 %{_bindir}/mash
-%{python3_sitelib}/*
+%{python_sitelib}/*
 
 %changelog
+
```

### Comparing `mash-client-4.1.0/setup.py` & `mash_client-4.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 with open('requirements-dev.txt') as req_file:
     dev_requirements = requirements + req_file.read().splitlines()[2:]
 
 
 setup(
     name='mash-client',
-    version='4.1.0',
+    version='4.2.0',
     description="CLI client for interfacing with a MASH server.",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="SUSE",
     author_email='public-cloud-dev@susecloud.net',
     url='https://github.com/SUSE-enceladus/mash-client',
     packages=find_packages(),
@@ -48,15 +48,15 @@
     },
     entry_points={
         'console_scripts': [
             'mash=mash_client.cli:main'
         ]
     },
     include_package_data=True,
-    python_requires='>=3.4',
+    python_requires='>=3.8',
     install_requires=requirements,
     extras_require={
         'dev': dev_requirements
     },
     license='GPLv3+',
     zip_safe=False,
     keywords='mash-client mash client',
@@ -65,14 +65,14 @@
         'Environment :: Console',
         'Intended Audience :: Developers',
         'Topic :: Utilities',
         'License :: OSI Approved :: '
         'GNU General Public License v3 or later (GPLv3+)',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
 )
```

