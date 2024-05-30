# Comparing `tmp/bk_audit-1.2.1.tar.gz` & `tmp/bk_audit-1.2.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bk_audit-1.2.1.tar", last modified: Mon Apr 22 03:54:48 2024, max compression
+gzip compressed data, was "bk_audit-1.2.2b0.tar", last modified: Thu May 30 07:00:56 2024, max compression
```

## Comparing `bk_audit-1.2.1.tar` & `bk_audit-1.2.2b0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:54:48.852488 bk_audit-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-22 03:54:35.000000 bk_audit-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-22 03:54:48.852488 bk_audit-1.2.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:54:48.844488 bk_audit-1.2.1/bk_audit/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:54:48.848488 bk_audit-1.2.1/bk_audit/constants/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/constants/contrib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/constants/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/constants/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:54:48.848488 bk_audit-1.2.1/bk_audit/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:54:48.848488 bk_audit-1.2.1/bk_audit/contrib/bk_audit/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/contrib/bk_audit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/contrib/bk_audit/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/contrib/bk_audit/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/contrib/bk_audit/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:54:48.848488 bk_audit-1.2.1/bk_audit/contrib/django/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/contrib/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/contrib/django/formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/contrib/django/loggers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6253 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/contrib/django/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:54:48.848488 bk_audit-1.2.1/bk_audit/contrib/opentelemetry/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/contrib/opentelemetry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/contrib/opentelemetry/exporters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/contrib/opentelemetry/processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/contrib/opentelemetry/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/contrib/opentelemetry/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:54:48.852488 bk_audit-1.2.1/bk_audit/log/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/log/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/log/exporters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/log/formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)    10990 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/log/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/log/queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:54:48.852488 bk_audit-1.2.1/bk_audit/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-22 03:54:35.000000 bk_audit-1.2.1/bk_audit/utils/time_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:54:48.852488 bk_audit-1.2.1/bk_audit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-22 03:54:48.000000 bk_audit-1.2.1/bk_audit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-22 03:54:48.000000 bk_audit-1.2.1/bk_audit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 03:54:48.000000 bk_audit-1.2.1/bk_audit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-22 03:54:48.000000 bk_audit-1.2.1/bk_audit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-22 03:54:48.000000 bk_audit-1.2.1/bk_audit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-04-22 03:54:35.000000 bk_audit-1.2.1/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 03:54:48.852488 bk_audit-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-22 03:54:35.000000 bk_audit-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:54:48.852488 bk_audit-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-04-22 03:54:35.000000 bk_audit-1.2.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-04-22 03:54:35.000000 bk_audit-1.2.1/tests/test_django.py
--rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-04-22 03:54:35.000000 bk_audit-1.2.1/tests/test_ot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-22 03:54:35.000000 bk_audit-1.2.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:00:56.640255 bk_audit-1.2.2b0/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 07:00:42.000000 bk_audit-1.2.2b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-05-30 07:00:56.640255 bk_audit-1.2.2b0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:00:56.632255 bk_audit-1.2.2b0/bk_audit/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-30 07:00:42.000000 bk_audit-1.2.2b0/bk_audit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-05-30 07:00:42.000000 bk_audit-1.2.2b0/bk_audit/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:00:56.636255 bk_audit-1.2.2b0/bk_audit/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-30 07:00:42.000000 bk_audit-1.2.2b0/bk_audit/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-30 07:00:42.000000 bk_audit-1.2.2b0/bk_audit/constants/contrib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-30 07:00:42.000000 bk_audit-1.2.2b0/bk_audit/constants/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-30 07:00:42.000000 bk_audit-1.2.2b0/bk_audit/constants/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:00:56.636255 bk_audit-1.2.2b0/bk_audit/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-30 07:00:42.000000 bk_audit-1.2.2b0/bk_audit/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:00:56.636255 bk_audit-1.2.2b0/bk_audit/contrib/bk_audit/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-30 07:00:42.000000 bk_audit-1.2.2b0/bk_audit/contrib/bk_audit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-30 07:00:42.000000 bk_audit-1.2.2b0/bk_audit/contrib/bk_audit/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-30 07:00:42.000000 bk_audit-1.2.2b0/bk_audit/contrib/bk_audit/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-30 07:00:42.000000 bk_audit-1.2.2b0/bk_audit/contrib/bk_audit/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:00:56.636255 bk_audit-1.2.2b0/bk_audit/contrib/django/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-30 07:00:42.000000 bk_audit-1.2.2b0/bk_audit/contrib/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-05-30 07:00:42.000000 bk_audit-1.2.2b0/bk_audit/contrib/django/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-30 07:00:42.000000 bk_audit-1.2.2b0/bk_audit/contrib/django/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6103 2024-05-30 07:00:42.000000 bk_audit-1.2.2b0/bk_audit/contrib/django/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:00:56.636255 bk_audit-1.2.2b0/bk_audit/contrib/opentelemetry/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-30 07:00:42.000000 bk_audit-1.2.2b0/bk_audit/contrib/opentelemetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-30 07:00:42.000000 bk_audit-1.2.2b0/bk_audit/contrib/opentelemetry/exporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-30 07:00:42.000000 bk_audit-1.2.2b0/bk_audit/contrib/opentelemetry/processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-30 07:00:42.000000 bk_audit-1.2.2b0/bk_audit/contrib/opentelemetry/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-30 07:00:42.000000 bk_audit-1.2.2b0/bk_audit/contrib/opentelemetry/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:00:56.636255 bk_audit-1.2.2b0/bk_audit/log/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-30 07:00:42.000000 bk_audit-1.2.2b0/bk_audit/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-05-30 07:00:42.000000 bk_audit-1.2.2b0/bk_audit/log/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-30 07:00:42.000000 bk_audit-1.2.2b0/bk_audit/log/exporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-05-30 07:00:42.000000 bk_audit-1.2.2b0/bk_audit/log/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10990 2024-05-30 07:00:42.000000 bk_audit-1.2.2b0/bk_audit/log/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-30 07:00:42.000000 bk_audit-1.2.2b0/bk_audit/log/queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:00:56.640255 bk_audit-1.2.2b0/bk_audit/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-30 07:00:42.000000 bk_audit-1.2.2b0/bk_audit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-30 07:00:42.000000 bk_audit-1.2.2b0/bk_audit/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-30 07:00:42.000000 bk_audit-1.2.2b0/bk_audit/utils/time_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:00:56.640255 bk_audit-1.2.2b0/bk_audit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-05-30 07:00:56.000000 bk_audit-1.2.2b0/bk_audit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-30 07:00:56.000000 bk_audit-1.2.2b0/bk_audit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 07:00:56.000000 bk_audit-1.2.2b0/bk_audit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-30 07:00:56.000000 bk_audit-1.2.2b0/bk_audit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-30 07:00:56.000000 bk_audit-1.2.2b0/bk_audit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-05-30 07:00:42.000000 bk_audit-1.2.2b0/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 07:00:56.640255 bk_audit-1.2.2b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-30 07:00:42.000000 bk_audit-1.2.2b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:00:56.640255 bk_audit-1.2.2b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-05-30 07:00:42.000000 bk_audit-1.2.2b0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-05-30 07:00:42.000000 bk_audit-1.2.2b0/tests/test_django.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-05-30 07:00:42.000000 bk_audit-1.2.2b0/tests/test_ot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-30 07:00:42.000000 bk_audit-1.2.2b0/tests/test_utils.py
```

### Comparing `bk_audit-1.2.1/PKG-INFO` & `bk_audit-1.2.2b0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: bk-audit
-Version: 1.2.1
+Version: 1.2.2b0
 Summary: Bk Audit SDK
 Home-page: https://bk.tencent.com
 Author: blueking
 Author-email: blueking@tencent.com
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires: bk_iam
-Requires: packaging
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, <4
 Description-Content-Type: text/markdown
 Provides-Extra: opentelemetry
 Requires-Dist: protobuf>=3.19.5; extra == "opentelemetry"
-Requires-Dist: opentelemetry-api<1.13.0,>=1.7.1; extra == "opentelemetry"
-Requires-Dist: opentelemetry-sdk<1.13.0,>=1.7.1; extra == "opentelemetry"
-Requires-Dist: opentelemetry-exporter-otlp<1.13.0,>=1.7.1; extra == "opentelemetry"
+Requires-Dist: opentelemetry-api>=1.20.0; extra == "opentelemetry"
+Requires-Dist: opentelemetry-sdk>=1.20.0; extra == "opentelemetry"
+Requires-Dist: opentelemetry-exporter-otlp>=1.20.0; extra == "opentelemetry"
 Provides-Extra: bk-resource
 Requires-Dist: bk_resource>=0.4.0; extra == "bk-resource"
 
 ![logo.png](https://github.com/TencentBlueKing/bk-audit-python-sdk/blob/master/assests/logo.png)
 
 [![license](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat)](https://github.com/TencentBlueKing/bk-audit-python-sdk/blob/master/LICENSE.txt)
-[![Release Version](https://img.shields.io/badge/release-1.2.1-brightgreen.svg)](https://github.com/TencentBlueKing/bk-audit-python-sdk/releases)
+[![Release Version](https://img.shields.io/badge/release-1.2.2-brightgreen.svg)](https://github.com/TencentBlueKing/bk-audit-python-sdk/releases)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/TencentBlueKing/bk-audit-python-sdk/pulls)
 [![codecov](https://codecov.io/github/TencentBlueKing/bk-audit-python-sdk/branch/master/graph/badge.svg?token=CUG20ZMOVQ)](https://codecov.io/github/TencentBlueKing/bk-audit-python-sdk)
 [![Test](https://github.com/TencentBlueKing/bk-audit-python-sdk/actions/workflows/unittest_py3.yml/badge.svg)](https://github.com/TencentBlueKing/bk-audit-python-sdk/actions/workflows/unittest_py3.yml)
 
 [(English Documents Available)](https://github.com/TencentBlueKing/bk-audit-python-sdk/blob/master/readme_en.md)
 
 ## Overview
```

### Comparing `bk_audit-1.2.1/bk_audit/__init__.py` & `bk_audit-1.2.2b0/bk_audit/__init__.py`

 * *Files identical despite different names*

### Comparing `bk_audit-1.2.1/bk_audit/client.py` & `bk_audit-1.2.2b0/bk_audit/client.py`

 * *Files identical despite different names*

### Comparing `bk_audit-1.2.1/bk_audit/constants/__init__.py` & `bk_audit-1.2.2b0/bk_audit/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `bk_audit-1.2.1/bk_audit/constants/contrib.py` & `bk_audit-1.2.2b0/bk_audit/constants/contrib.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,30 +12,16 @@
 an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND,
 either express or implied. See the License for the
 specific language governing permissions and limitations under the License.
 We undertake not to change the open source license (MIT license) applicable
 to the current version of the project delivered to anyone in the future.
 """
 
-from packaging import version
-
 DJANGO_SETTING_NAME = "BK_AUDIT_SETTINGS"
 
 
 class LoggingDefaultConfig:
     """Logging 默认配置"""
 
     HANDLER_CLS = "logging.handlers.RotatingFileHandler"
     FILE_MAX_BYTES = 1024 * 1024 * 100  # 10M
     FILE_BACKUP_COUNT = 5
-
-
-class OTVersion:
-    """OT 更新版本"""
-
-    # _log release
-    # https://github.com/open-telemetry/opentelemetry-python/releases/tag/v1.7.1
-    v1_7_1 = version.parse("1.7.1")
-
-    # Change OTLPHandler to LoggingHandler
-    # https://github.com/open-telemetry/opentelemetry-python/pull/2528
-    v1_11_0 = version.parse("1.11.0")
```

### Comparing `bk_audit-1.2.1/bk_audit/constants/log.py` & `bk_audit-1.2.2b0/bk_audit/constants/log.py`

 * *Files identical despite different names*

### Comparing `bk_audit-1.2.1/bk_audit/constants/utils.py` & `bk_audit-1.2.2b0/bk_audit/constants/utils.py`

 * *Files identical despite different names*

### Comparing `bk_audit-1.2.1/bk_audit/contrib/__init__.py` & `bk_audit-1.2.2b0/bk_audit/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `bk_audit-1.2.1/bk_audit/contrib/bk_audit/__init__.py` & `bk_audit-1.2.2b0/bk_audit/contrib/bk_audit/__init__.py`

 * *Files identical despite different names*

### Comparing `bk_audit-1.2.1/bk_audit/contrib/bk_audit/apps.py` & `bk_audit-1.2.2b0/bk_audit/contrib/bk_audit/apps.py`

 * *Files identical despite different names*

### Comparing `bk_audit-1.2.1/bk_audit/contrib/bk_audit/client.py` & `bk_audit-1.2.2b0/bk_audit/contrib/bk_audit/client.py`

 * *Files identical despite different names*

### Comparing `bk_audit-1.2.1/bk_audit/contrib/bk_audit/settings.py` & `bk_audit-1.2.2b0/bk_audit/contrib/bk_audit/settings.py`

 * *Files identical despite different names*

### Comparing `bk_audit-1.2.1/bk_audit/contrib/django/__init__.py` & `bk_audit-1.2.2b0/bk_audit/contrib/django/__init__.py`

 * *Files identical despite different names*

### Comparing `bk_audit-1.2.1/bk_audit/contrib/django/formatters.py` & `bk_audit-1.2.2b0/bk_audit/contrib/django/formatters.py`

 * *Files identical despite different names*

### Comparing `bk_audit-1.2.1/bk_audit/contrib/django/loggers.py` & `bk_audit-1.2.2b0/bk_audit/contrib/django/loggers.py`

 * *Files identical despite different names*

### Comparing `bk_audit-1.2.1/bk_audit/contrib/django/resources.py` & `bk_audit-1.2.2b0/bk_audit/contrib/django/resources.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 specific language governing permissions and limitations under the License.
 We undertake not to change the open source license (MIT license) applicable
 to the current version of the project delivered to anyone in the future.
 """
 
 import abc
 import datetime
-import sys
-from typing import Optional, Union
+from functools import cached_property
+from typing import Optional, TypedDict, Union
 
 from bk_resource import Resource
 from bk_resource.base import Empty
 from blueapps.core.exceptions import BlueException
 from django.utils.module_loading import import_string
 from iam import Action as SimpleAction
 from iam import Resource as SimpleResourceType
@@ -35,21 +35,14 @@
 from bk_audit.log.models import (
     AuditAction,
     AuditContext,
     AuditInstance,
     AuditResourceType,
 )
 
-if sys.version_info >= (3, 8):
-    from functools import cached_property
-    from typing import TypedDict
-else:
-    cached_property = property
-    from typing_extensions import TypedDict
-
 
 # noinspection PyCompatibility
 class AuditEvent(TypedDict):
     action: Union[AuditAction, SimpleAction, Action]
     resource_type: Optional[Union[AuditResourceType, SimpleResourceType, ResourceType]]
     instance: Optional[AuditInstance]
     audit_context: Optional[AuditContext]
```

### Comparing `bk_audit-1.2.1/bk_audit/contrib/opentelemetry/__init__.py` & `bk_audit-1.2.2b0/bk_audit/contrib/opentelemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `bk_audit-1.2.1/bk_audit/contrib/opentelemetry/exporters.py` & `bk_audit-1.2.2b0/bk_audit/contrib/opentelemetry/exporters.py`

 * *Files identical despite different names*

### Comparing `bk_audit-1.2.1/bk_audit/contrib/opentelemetry/processor.py` & `bk_audit-1.2.2b0/bk_audit/contrib/opentelemetry/processor.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND,
 either express or implied. See the License for the
 specific language governing permissions and limitations under the License.
 We undertake not to change the open source license (MIT license) applicable
 to the current version of the project delivered to anyone in the future.
 """
 
-from opentelemetry.sdk._logs.export import BatchLogProcessor
+from opentelemetry.sdk._logs.export import BatchLogRecordProcessor
 
 
-class LazyBatchLogProcessor(BatchLogProcessor):
+class LazyBatchLogProcessor(BatchLogRecordProcessor):
     def __init__(self, *args, **kwargs):
         super(LazyBatchLogProcessor, self).__init__(*args, **kwargs)
         # shutdown
         self._shutdown = True
         with self._condition:
             self._condition.notify_all()
         self._worker_thread.join()
@@ -48,8 +48,8 @@
             self._worker_thread.join()
         # shutdown exporter
         self._exporter.shutdown()
 
     def force_flush(self, timeout_millis=None):
         if self._shutdown or self._worker_thread is None:
             return True
-        super().force_flush(timeout_millis)
+        super(LazyBatchLogProcessor, self).force_flush(timeout_millis)
```

### Comparing `bk_audit-1.2.1/bk_audit/contrib/opentelemetry/setup.py` & `bk_audit-1.2.2b0/bk_audit/contrib/opentelemetry/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,31 +16,23 @@
 to the current version of the project delivered to anyone in the future.
 """
 
 import logging
 import os
 from typing import Type
 
+from opentelemetry._logs import set_logger_provider
 from opentelemetry.exporter.otlp.proto.grpc._log_exporter import OTLPLogExporter
-from opentelemetry.sdk._logs import (
-    LogEmitterProvider,
-    LogProcessor,
-    set_log_emitter_provider,
-)
-from opentelemetry.sdk._logs.export import SimpleLogProcessor
+from opentelemetry.sdk._logs import LoggerProvider, LoggingHandler, LogRecordProcessor
+from opentelemetry.sdk._logs.export import SimpleLogRecordProcessor
 from opentelemetry.sdk.resources import Resource
-from opentelemetry.sdk.version import __version__ as _ot_version
-from packaging import version
 
-from bk_audit.constants.contrib import OTVersion
 from bk_audit.constants.utils import OT_LOGGER_NAME
 from bk_audit.contrib.opentelemetry.processor import LazyBatchLogProcessor
 
-OT_VERSION = version.parse(_ot_version)
-
 
 def setup(
     client,
     bk_data_id=None,
     bk_data_token=None,
     endpoint=None,
 ):
@@ -52,38 +44,34 @@
     @param bk_data_id: Data ID
     @type bk_data_token: str
     @param bk_data_token: Data Token
     @type endpoint: str
     @param endpoint: 上报地址
     """
 
-    if OT_VERSION < OTVersion.v1_11_0:
-        from opentelemetry.sdk._logs import OTLPHandler as LoggingHandler
-    else:
-        from opentelemetry.sdk._logs import LoggingHandler
-
     # init service config
     service_name = client.service_name
     bk_data_id = bk_data_id or int(os.getenv("BKAPP_OTEL_LOG_BK_DATA_ID", -1))
     bk_data_token = bk_data_token or os.getenv("BKAPP_OTEL_LOG_BK_DATA_TOKEN", "")
 
     # init log emitter
-    log_emitter_provider = LogEmitterProvider(
+    logger_provider = LoggerProvider(
         resource=Resource.create(
-            {"service.name": service_name, "bk_data_id": bk_data_id, "bk.data.token": bk_data_token}
+            {
+                "service.name": service_name,
+                "bk_data_id": bk_data_id,
+                "bk.data.token": bk_data_token,
+            }
         )
     )
-    set_log_emitter_provider(log_emitter_provider)
+    set_logger_provider(logger_provider)
 
     # init exporter
-    processor: Type[LogProcessor] = LazyBatchLogProcessor
+    processor: Type[LogRecordProcessor] = LazyBatchLogProcessor
     if os.getenv("BKAPP_USE_SIMPLE_LOG_PROCESSOR"):
-        processor = SimpleLogProcessor
+        processor = SimpleLogRecordProcessor
     exporter = OTLPLogExporter(endpoint=endpoint or os.getenv("BKAPP_OTEL_LOG_ENDPOINT"))
-    log_emitter_provider.add_log_processor(processor(exporter))
+    logger_provider.add_log_record_processor(processor(exporter))
 
     # init logging
-    handler = LoggingHandler(
-        level=logging.NOTSET,
-        log_emitter=log_emitter_provider.get_log_emitter(service_name),
-    )
+    handler = LoggingHandler(level=logging.NOTSET, logger_provider=logger_provider)
     logging.getLogger(OT_LOGGER_NAME).addHandler(handler)
```

### Comparing `bk_audit-1.2.1/bk_audit/contrib/opentelemetry/utils.py` & `bk_audit-1.2.2b0/bk_audit/contrib/opentelemetry/utils.py`

 * *Files identical despite different names*

### Comparing `bk_audit-1.2.1/bk_audit/log/__init__.py` & `bk_audit-1.2.2b0/bk_audit/log/__init__.py`

 * *Files identical despite different names*

### Comparing `bk_audit-1.2.1/bk_audit/log/base.py` & `bk_audit-1.2.2b0/bk_audit/log/base.py`

 * *Files identical despite different names*

### Comparing `bk_audit-1.2.1/bk_audit/log/exporters.py` & `bk_audit-1.2.2b0/bk_audit/log/exporters.py`

 * *Files identical despite different names*

### Comparing `bk_audit-1.2.1/bk_audit/log/formatters.py` & `bk_audit-1.2.2b0/bk_audit/log/formatters.py`

 * *Files identical despite different names*

### Comparing `bk_audit-1.2.1/bk_audit/log/models.py` & `bk_audit-1.2.2b0/bk_audit/log/models.py`

 * *Files identical despite different names*

### Comparing `bk_audit-1.2.1/bk_audit/log/queue.py` & `bk_audit-1.2.2b0/bk_audit/log/queue.py`

 * *Files identical despite different names*

### Comparing `bk_audit-1.2.1/bk_audit/utils/__init__.py` & `bk_audit-1.2.2b0/bk_audit/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bk_audit-1.2.1/bk_audit/utils/decorators.py` & `bk_audit-1.2.2b0/bk_audit/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `bk_audit-1.2.1/bk_audit/utils/time_tool.py` & `bk_audit-1.2.2b0/bk_audit/utils/time_tool.py`

 * *Files identical despite different names*

### Comparing `bk_audit-1.2.1/bk_audit.egg-info/PKG-INFO` & `bk_audit-1.2.2b0/bk_audit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: bk-audit
-Version: 1.2.1
+Version: 1.2.2b0
 Summary: Bk Audit SDK
 Home-page: https://bk.tencent.com
 Author: blueking
 Author-email: blueking@tencent.com
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires: bk_iam
-Requires: packaging
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, <4
 Description-Content-Type: text/markdown
 Provides-Extra: opentelemetry
 Requires-Dist: protobuf>=3.19.5; extra == "opentelemetry"
-Requires-Dist: opentelemetry-api<1.13.0,>=1.7.1; extra == "opentelemetry"
-Requires-Dist: opentelemetry-sdk<1.13.0,>=1.7.1; extra == "opentelemetry"
-Requires-Dist: opentelemetry-exporter-otlp<1.13.0,>=1.7.1; extra == "opentelemetry"
+Requires-Dist: opentelemetry-api>=1.20.0; extra == "opentelemetry"
+Requires-Dist: opentelemetry-sdk>=1.20.0; extra == "opentelemetry"
+Requires-Dist: opentelemetry-exporter-otlp>=1.20.0; extra == "opentelemetry"
 Provides-Extra: bk-resource
 Requires-Dist: bk_resource>=0.4.0; extra == "bk-resource"
 
 ![logo.png](https://github.com/TencentBlueKing/bk-audit-python-sdk/blob/master/assests/logo.png)
 
 [![license](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat)](https://github.com/TencentBlueKing/bk-audit-python-sdk/blob/master/LICENSE.txt)
-[![Release Version](https://img.shields.io/badge/release-1.2.1-brightgreen.svg)](https://github.com/TencentBlueKing/bk-audit-python-sdk/releases)
+[![Release Version](https://img.shields.io/badge/release-1.2.2-brightgreen.svg)](https://github.com/TencentBlueKing/bk-audit-python-sdk/releases)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/TencentBlueKing/bk-audit-python-sdk/pulls)
 [![codecov](https://codecov.io/github/TencentBlueKing/bk-audit-python-sdk/branch/master/graph/badge.svg?token=CUG20ZMOVQ)](https://codecov.io/github/TencentBlueKing/bk-audit-python-sdk)
 [![Test](https://github.com/TencentBlueKing/bk-audit-python-sdk/actions/workflows/unittest_py3.yml/badge.svg)](https://github.com/TencentBlueKing/bk-audit-python-sdk/actions/workflows/unittest_py3.yml)
 
 [(English Documents Available)](https://github.com/TencentBlueKing/bk-audit-python-sdk/blob/master/readme_en.md)
 
 ## Overview
```

### Comparing `bk_audit-1.2.1/bk_audit.egg-info/SOURCES.txt` & `bk_audit-1.2.2b0/bk_audit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bk_audit-1.2.1/readme.md` & `bk_audit-1.2.2b0/readme.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ![logo.png](https://github.com/TencentBlueKing/bk-audit-python-sdk/blob/master/assests/logo.png)
 
 [![license](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat)](https://github.com/TencentBlueKing/bk-audit-python-sdk/blob/master/LICENSE.txt)
-[![Release Version](https://img.shields.io/badge/release-1.2.1-brightgreen.svg)](https://github.com/TencentBlueKing/bk-audit-python-sdk/releases)
+[![Release Version](https://img.shields.io/badge/release-1.2.2-brightgreen.svg)](https://github.com/TencentBlueKing/bk-audit-python-sdk/releases)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/TencentBlueKing/bk-audit-python-sdk/pulls)
 [![codecov](https://codecov.io/github/TencentBlueKing/bk-audit-python-sdk/branch/master/graph/badge.svg?token=CUG20ZMOVQ)](https://codecov.io/github/TencentBlueKing/bk-audit-python-sdk)
 [![Test](https://github.com/TencentBlueKing/bk-audit-python-sdk/actions/workflows/unittest_py3.yml/badge.svg)](https://github.com/TencentBlueKing/bk-audit-python-sdk/actions/workflows/unittest_py3.yml)
 
 [(English Documents Available)](https://github.com/TencentBlueKing/bk-audit-python-sdk/blob/master/readme_en.md)
 
 ## Overview
```

### Comparing `bk_audit-1.2.1/setup.py` & `bk_audit-1.2.2b0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 current_directory = os.path.abspath(os.path.dirname(__file__))
 readme_path = os.path.join(current_directory, "readme.md")
 with open(readme_path) as f:
     readme = f.read()
 
 setup(
     name="bk-audit",
-    version="1.2.1",
+    version="1.2.2b0",
     author="blueking",
     url="https://bk.tencent.com",
     author_email="blueking@tencent.com",
     description="Bk Audit SDK",
     long_description=readme,
     long_description_content_type="text/markdown",
     packages=[
@@ -42,23 +42,22 @@
         "bk_audit.contrib.django",
         "bk_audit.contrib.opentelemetry",
         "bk_audit.log",
         "bk_audit.utils",
     ],
     requires=[
         "bk_iam",
-        "packaging",
     ],
     extras_require={
         # OT 仅支持 Py3.6 及以上版本
         "opentelemetry": [
             "protobuf>=3.19.5",
-            "opentelemetry-api>=1.7.1,<1.13.0",
-            "opentelemetry-sdk>=1.7.1,<1.13.0",
-            "opentelemetry-exporter-otlp>=1.7.1,<1.13.0",
+            "opentelemetry-api>=1.20.0",
+            "opentelemetry-sdk>=1.20.0",
+            "opentelemetry-exporter-otlp>=1.20.0",
         ],
         # BKResource 仅支持 Py3.6 及以上版本
         "bk_resource": [
             "bk_resource>=0.4.0",
         ],
     },
     classifiers=[
```

### Comparing `bk_audit-1.2.1/tests/test_client.py` & `bk_audit-1.2.2b0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `bk_audit-1.2.1/tests/test_django.py` & `bk_audit-1.2.2b0/tests/test_django.py`

 * *Files identical despite different names*

### Comparing `bk_audit-1.2.1/tests/test_ot.py` & `bk_audit-1.2.2b0/tests/test_ot.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 from unittest import TestCase
 from unittest.mock import Mock, patch
 
 from opentelemetry.exporter.otlp.proto.grpc._log_exporter import OTLPLogExporter
 from opentelemetry.sdk._logs import LogData, LogRecord
 from opentelemetry.sdk.util.instrumentation import InstrumentationScope
 
-from bk_audit.constants.contrib import OTVersion
 from bk_audit.contrib.opentelemetry.exporters import OTLogExporter
 from bk_audit.contrib.opentelemetry.processor import LazyBatchLogProcessor
 from bk_audit.contrib.opentelemetry.setup import setup
 from bk_audit.contrib.opentelemetry.utils import (
     BaseServiceNameHandler,
     ServiceNameHandler,
 )
@@ -53,20 +52,14 @@
         result_content = object()
         self.client.add_event(action=VIEW_FILE, audit_context=CONTEXT, result_content={"content": result_content})
 
     def test_setup(self):
         """测试OT初始化"""
         setup(self.client)
 
-    @patch("bk_audit.contrib.opentelemetry.setup.OT_VERSION", OTVersion.v1_7_1)
-    def test_setup_1_7_1(self):
-        """测试OT初始化(v1.7.1)"""
-        with self.assertRaises(ImportError):
-            setup(self.client)
-
     def test_service_name(self):
         """测试基类"""
         self.assertEqual(BaseServiceNameHandler(str()).get_service_name(), None)
 
     @patch("bk_audit.contrib.opentelemetry.utils.ServiceNameHandler.is_celery_beat", Mock(return_value=True))
     def test_service_name_beat(self):
         """测试服务名处理Beat"""
```

### Comparing `bk_audit-1.2.1/tests/test_utils.py` & `bk_audit-1.2.2b0/tests/test_utils.py`

 * *Files identical despite different names*

