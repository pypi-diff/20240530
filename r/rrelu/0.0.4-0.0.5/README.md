# Comparing `tmp/rrelu-0.0.4.tar.gz` & `tmp/rrelu-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rrelu-0.0.4.tar", last modified: Thu May 30 11:01:17 2024, max compression
+gzip compressed data, was "rrelu-0.0.5.tar", last modified: Thu May 30 11:38:03 2024, max compression
```

## Comparing `rrelu-0.0.4.tar` & `rrelu-0.0.5.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 11:01:17.856551 rrelu-0.0.4/
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     1079 2024-05-30 10:41:58.000000 rrelu-0.0.4/LICENSE.txt
--rw-rw-r--   0 a4000     (1000) a4000     (1000)        0 2024-05-30 10:41:58.000000 rrelu-0.0.4/MANIFEST.in
--rw-r--r--   0 a4000     (1000) a4000     (1000)     3619 2024-05-30 11:01:17.856551 rrelu-0.0.4/PKG-INFO
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     2946 2024-05-30 10:41:58.000000 rrelu-0.0.4/README.md
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      554 2024-05-30 11:01:08.000000 rrelu-0.0.4/pyproject.toml
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      696 2024-05-30 11:01:17.856551 rrelu-0.0.4/setup.cfg
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      898 2024-05-30 11:00:57.000000 rrelu-0.0.4/setup.py
-drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 11:01:17.848551 rrelu-0.0.4/src/
-drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 11:01:17.848551 rrelu-0.0.4/src/rrelu/
--rw-rw-r--   0 a4000     (1000) a4000     (1000)        0 2024-05-30 10:59:25.000000 rrelu-0.0.4/src/rrelu/__init__.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     3528 2024-05-30 10:41:58.000000 rrelu-0.0.4/src/rrelu/eval.py
-drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 11:01:17.852551 rrelu-0.0.4/src/rrelu/models/
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      175 2024-05-30 10:41:58.000000 rrelu-0.0.4/src/rrelu/models/__init__.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     2875 2024-05-30 10:41:58.000000 rrelu-0.0.4/src/rrelu/models/alexnet.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     1232 2024-05-30 10:41:58.000000 rrelu-0.0.4/src/rrelu/models/alexnet_cifar100.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     2965 2024-05-30 10:41:58.000000 rrelu-0.0.4/src/rrelu/models/lenet.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     4839 2024-05-30 10:41:58.000000 rrelu-0.0.4/src/rrelu/models/resnet.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     4848 2024-05-30 10:41:58.000000 rrelu-0.0.4/src/rrelu/models/resnet_cifar100.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     2560 2024-05-30 10:41:58.000000 rrelu-0.0.4/src/rrelu/models/vgg.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     2580 2024-05-30 10:41:58.000000 rrelu-0.0.4/src/rrelu/models/vgg_cifar100.py
-drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 11:01:17.852551 rrelu-0.0.4/src/rrelu/pytorchfi/
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      109 2024-05-30 10:41:58.000000 rrelu-0.0.4/src/rrelu/pytorchfi/__init__.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)    21655 2024-05-30 10:41:58.000000 rrelu-0.0.4/src/rrelu/pytorchfi/core.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)    21711 2024-05-30 10:41:58.000000 rrelu-0.0.4/src/rrelu/pytorchfi/core_train.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)    10468 2024-05-30 10:41:58.000000 rrelu-0.0.4/src/rrelu/pytorchfi/neuron_error_models.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      115 2024-05-30 10:41:58.000000 rrelu-0.0.4/src/rrelu/pytorchfi/util.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)    22084 2024-05-30 10:41:58.000000 rrelu-0.0.4/src/rrelu/pytorchfi/weight_error_models.py
-drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 11:01:17.856551 rrelu-0.0.4/src/rrelu/relu_bound/
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      108 2024-05-30 10:41:58.000000 rrelu-0.0.4/src/rrelu/relu_bound/__init__.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      823 2024-05-30 10:41:58.000000 rrelu-0.0.4/src/rrelu/relu_bound/bound_fitact.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     1076 2024-05-30 10:41:58.000000 rrelu-0.0.4/src/rrelu/relu_bound/bound_proact.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)       95 2024-05-30 10:41:58.000000 rrelu-0.0.4/src/rrelu/relu_bound/bound_relu.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      754 2024-05-30 10:41:58.000000 rrelu-0.0.4/src/rrelu/relu_bound/bound_tresh.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      759 2024-05-30 10:41:58.000000 rrelu-0.0.4/src/rrelu/relu_bound/bound_zero.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     5052 2024-05-30 10:41:58.000000 rrelu-0.0.4/src/rrelu/search.py
-drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 11:01:17.856551 rrelu-0.0.4/src/rrelu/search_bound/
--rw-rw-r--   0 a4000     (1000) a4000     (1000)       88 2024-05-30 10:41:58.000000 rrelu-0.0.4/src/rrelu/search_bound/__init__.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)    10390 2024-05-30 10:41:58.000000 rrelu-0.0.4/src/rrelu/search_bound/fitact.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)    17994 2024-05-30 10:41:58.000000 rrelu-0.0.4/src/rrelu/search_bound/ftclip.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)    18074 2024-05-30 10:41:58.000000 rrelu-0.0.4/src/rrelu/search_bound/proact.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     1718 2024-05-30 10:41:58.000000 rrelu-0.0.4/src/rrelu/search_bound/ranger.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)    11519 2024-05-30 10:41:58.000000 rrelu-0.0.4/src/rrelu/setup.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)    13425 2024-05-30 10:41:58.000000 rrelu-0.0.4/src/rrelu/train.py
-drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 11:01:17.856551 rrelu-0.0.4/src/rrelu/utils/
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      116 2024-05-30 10:41:58.000000 rrelu-0.0.4/src/rrelu/utils/__init__.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     1659 2024-05-30 10:41:58.000000 rrelu-0.0.4/src/rrelu/utils/distributed.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     2811 2024-05-30 10:41:58.000000 rrelu-0.0.4/src/rrelu/utils/init.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     1094 2024-05-30 10:41:58.000000 rrelu-0.0.4/src/rrelu/utils/lr_scheduler.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     1218 2024-05-30 10:41:58.000000 rrelu-0.0.4/src/rrelu/utils/metric.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     3612 2024-05-30 10:41:58.000000 rrelu-0.0.4/src/rrelu/utils/misc.py
-drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 11:01:17.856551 rrelu-0.0.4/src/rrelu.egg-info/
--rw-r--r--   0 a4000     (1000) a4000     (1000)     3619 2024-05-30 11:01:17.000000 rrelu-0.0.4/src/rrelu.egg-info/PKG-INFO
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     1290 2024-05-30 11:01:17.000000 rrelu-0.0.4/src/rrelu.egg-info/SOURCES.txt
--rw-rw-r--   0 a4000     (1000) a4000     (1000)        1 2024-05-30 11:01:17.000000 rrelu-0.0.4/src/rrelu.egg-info/dependency_links.txt
--rw-rw-r--   0 a4000     (1000) a4000     (1000)        6 2024-05-30 11:01:17.000000 rrelu-0.0.4/src/rrelu.egg-info/top_level.txt
+drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 11:38:03.314320 rrelu-0.0.5/
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     1079 2024-05-30 11:37:03.000000 rrelu-0.0.5/LICENSE.txt
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)        0 2024-05-30 11:37:03.000000 rrelu-0.0.5/MANIFEST.in
+-rw-r--r--   0 a4000     (1000) a4000     (1000)     3650 2024-05-30 11:38:03.314320 rrelu-0.0.5/PKG-INFO
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     2977 2024-05-30 11:37:03.000000 rrelu-0.0.5/README.md
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      554 2024-05-30 11:37:03.000000 rrelu-0.0.5/pyproject.toml
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      696 2024-05-30 11:38:03.314320 rrelu-0.0.5/setup.cfg
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      898 2024-05-30 11:37:03.000000 rrelu-0.0.5/setup.py
+drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 11:38:03.306320 rrelu-0.0.5/src/
+drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 11:38:03.306320 rrelu-0.0.5/src/rrelu/
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)        2 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/__init__.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     3547 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/eval.py
+drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 11:38:03.310320 rrelu-0.0.5/src/rrelu/models/
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      260 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/models/__init__.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     2881 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/models/alexnet.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     1232 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/models/alexnet_cifar100.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     2965 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/models/lenet.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     4839 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/models/resnet.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     4848 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/models/resnet_cifar100.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     2560 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/models/vgg.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     2580 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/models/vgg_cifar100.py
+drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 11:38:03.310320 rrelu-0.0.5/src/rrelu/pytorchfi/
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      170 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/pytorchfi/__init__.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)    21661 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/pytorchfi/core.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)    21717 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/pytorchfi/core_train.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)    10480 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/pytorchfi/neuron_error_models.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      115 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/pytorchfi/util.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)    22096 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/pytorchfi/weight_error_models.py
+drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 11:38:03.310320 rrelu-0.0.5/src/rrelu/relu_bound/
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      173 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/relu_bound/__init__.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      829 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/relu_bound/bound_fitact.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     1082 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/relu_bound/bound_proact.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)       95 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/relu_bound/bound_relu.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      761 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/relu_bound/bound_tresh.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      766 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/relu_bound/bound_zero.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     5070 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/search.py
+drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 11:38:03.314320 rrelu-0.0.5/src/rrelu/search_bound/
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      161 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/search_bound/__init__.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)    10420 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/search_bound/fitact.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)    18037 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/search_bound/ftclip.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)    18122 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/search_bound/proact.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     1718 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/search_bound/ranger.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)    11543 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/setup.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)    13480 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/train.py
+drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 11:38:03.314320 rrelu-0.0.5/src/rrelu/utils/
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      172 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/utils/__init__.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     1659 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/utils/distributed.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     2811 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/utils/init.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     1094 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/utils/lr_scheduler.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     1218 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/utils/metric.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     3612 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/utils/misc.py
+drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 11:38:03.314320 rrelu-0.0.5/src/rrelu.egg-info/
+-rw-r--r--   0 a4000     (1000) a4000     (1000)     3650 2024-05-30 11:38:03.000000 rrelu-0.0.5/src/rrelu.egg-info/PKG-INFO
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     1290 2024-05-30 11:38:03.000000 rrelu-0.0.5/src/rrelu.egg-info/SOURCES.txt
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)        1 2024-05-30 11:38:03.000000 rrelu-0.0.5/src/rrelu.egg-info/dependency_links.txt
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)        6 2024-05-30 11:38:03.000000 rrelu-0.0.5/src/rrelu.egg-info/top_level.txt
```

### Comparing `rrelu-0.0.4/LICENSE.txt` & `rrelu-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.4/PKG-INFO` & `rrelu-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rrelu
-Version: 0.0.4
+Version: 0.0.5
 Summary: generate reliable relu activation function for DNNs
 Home-page: https://github.com/hamidmousavi0/reliable-relu-toolbox
 Author: Seyedhamidreza Mousavi
 Author-email: Seyedhamidreza Mousavi <seyedhamidreza.mousavi@mdu.se>
 Project-URL: Homepage, https://github.com/hamidmousavi0/reliable-relu-toolbox
 Project-URL: Issues, https://github.com/hamidmousavi0/reliable-relu-toolbox/issues
 Classifier: Programming Language :: Python :: 3
@@ -34,15 +34,15 @@
 * **ProAct** (the proposed algorithm) ([code](https://github.com/hamidmousavi0/reliable-relu-toolbox/blob/master/src/search_bound/proact.py)).
 * **FitAct** ([paper](https://arxiv.org/pdf/2112.13544) and [code](https://github.com/hamidmousavi0/reliable-relu-toolbox/blob/master/src/search_bound/fitact.py)).
 * **FtClipAct** ([paper](https://arxiv.org/pdf/1912.00941) and [code](https://github.com/hamidmousavi0/reliable-relu-toolbox/blob/master/src/search_bound/ftclip.py)).
 * **Ranger** ([paper](https://arxiv.org/pdf/2003.13874) and [code](https://github.com/hamidmousavi0/reliable-relu-toolbox/blob/master/src/search_bound/ranger.py)).
 
 ## Usage
 
-Download on PyPI [here]().
+Download on PyPI [here](https://pypi.org/project/rrelu/).
 
 ### Installing
 
 **From Pip**
 
 Install using `pip install rrelu`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rrelu Version: 0.0.4 Summary: generate reliable
+Metadata-Version: 2.1 Name: rrelu Version: 0.0.5 Summary: generate reliable
 relu activation function for DNNs Home-page: https://github.com/hamidmousavi0/
 reliable-relu-toolbox Author: Seyedhamidreza Mousavi Author-email:
 Seyedhamidreza Mousavi
 mdu.se> Project-URL: Homepage, https://github.com/hamidmousavi0/reliable-relu-
 toolbox Project-URL: Issues, https://github.com/hamidmousavi0/reliable-relu-
 toolbox/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
@@ -28,21 +28,21 @@
 toolbox/blob/master/src/search_bound/proact.py)). * **FitAct** ([paper](https:/
 /arxiv.org/pdf/2112.13544) and [code](https://github.com/hamidmousavi0/
 reliable-relu-toolbox/blob/master/src/search_bound/fitact.py)). * **FtClipAct**
 ([paper](https://arxiv.org/pdf/1912.00941) and [code](https://github.com/
 hamidmousavi0/reliable-relu-toolbox/blob/master/src/search_bound/ftclip.py)). *
 **Ranger** ([paper](https://arxiv.org/pdf/2003.13874) and [code](https://
 github.com/hamidmousavi0/reliable-relu-toolbox/blob/master/src/search_bound/
-ranger.py)). ## Usage Download on PyPI [here](). ### Installing **From Pip**
-Install using `pip install rrelu` **From Source** Download this repository into
-your project folder. ### Importing Import the entire package: ```python import
-rrelu ``` Import a specific module: ```python from rrelu.search_bound import
-proact_bounds ``` ### Testing -- running and evaluating algorithms: ```python
-torchpack dist-run -np 1 python rrelu.search.py --dataset "dataset name
-(CIFAR10, CIFAR100)" --data_path "path to the dataset" --model "name of the
-model" --init_from "pretrained file path" \ --name_relu_bound "name of bounded
-relu" --name_serach_bound "name of the search algorithm" --bounds_type "type of
-thresholds" --bitflip "value representaiton" ``` ## Code ### Structure The main
-source code of framework is held in `src/rrelu`, which carries `search_bounds`,
-`relu_bounds` , `extended pytorchfi` and other implementations. ## Citation
-View the [published paper](). If you use or reference rrelu, please cite: ```
-```
+ranger.py)). ## Usage Download on PyPI [here](https://pypi.org/project/rrelu/).
+### Installing **From Pip** Install using `pip install rrelu` **From Source**
+Download this repository into your project folder. ### Importing Import the
+entire package: ```python import rrelu ``` Import a specific module: ```python
+from rrelu.search_bound import proact_bounds ``` ### Testing -- running and
+evaluating algorithms: ```python torchpack dist-run -np 1 python
+rrelu.search.py --dataset "dataset name (CIFAR10, CIFAR100)" --data_path "path
+to the dataset" --model "name of the model" --init_from "pretrained file path"
+\ --name_relu_bound "name of bounded relu" --name_serach_bound "name of the
+search algorithm" --bounds_type "type of thresholds" --bitflip "value
+representaiton" ``` ## Code ### Structure The main source code of framework is
+held in `src/rrelu`, which carries `search_bounds`, `relu_bounds` , `extended
+pytorchfi` and other implementations. ## Citation View the [published paper]().
+If you use or reference rrelu, please cite: ``` ```
```

### Comparing `rrelu-0.0.4/README.md` & `rrelu-0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 * **ProAct** (the proposed algorithm) ([code](https://github.com/hamidmousavi0/reliable-relu-toolbox/blob/master/src/search_bound/proact.py)).
 * **FitAct** ([paper](https://arxiv.org/pdf/2112.13544) and [code](https://github.com/hamidmousavi0/reliable-relu-toolbox/blob/master/src/search_bound/fitact.py)).
 * **FtClipAct** ([paper](https://arxiv.org/pdf/1912.00941) and [code](https://github.com/hamidmousavi0/reliable-relu-toolbox/blob/master/src/search_bound/ftclip.py)).
 * **Ranger** ([paper](https://arxiv.org/pdf/2003.13874) and [code](https://github.com/hamidmousavi0/reliable-relu-toolbox/blob/master/src/search_bound/ranger.py)).
 
 ## Usage
 
-Download on PyPI [here]().
+Download on PyPI [here](https://pypi.org/project/rrelu/).
 
 ### Installing
 
 **From Pip**
 
 Install using `pip install rrelu`
```

#### html2text {}

```diff
@@ -18,21 +18,21 @@
 toolbox/blob/master/src/search_bound/proact.py)). * **FitAct** ([paper](https:/
 /arxiv.org/pdf/2112.13544) and [code](https://github.com/hamidmousavi0/
 reliable-relu-toolbox/blob/master/src/search_bound/fitact.py)). * **FtClipAct**
 ([paper](https://arxiv.org/pdf/1912.00941) and [code](https://github.com/
 hamidmousavi0/reliable-relu-toolbox/blob/master/src/search_bound/ftclip.py)). *
 **Ranger** ([paper](https://arxiv.org/pdf/2003.13874) and [code](https://
 github.com/hamidmousavi0/reliable-relu-toolbox/blob/master/src/search_bound/
-ranger.py)). ## Usage Download on PyPI [here](). ### Installing **From Pip**
-Install using `pip install rrelu` **From Source** Download this repository into
-your project folder. ### Importing Import the entire package: ```python import
-rrelu ``` Import a specific module: ```python from rrelu.search_bound import
-proact_bounds ``` ### Testing -- running and evaluating algorithms: ```python
-torchpack dist-run -np 1 python rrelu.search.py --dataset "dataset name
-(CIFAR10, CIFAR100)" --data_path "path to the dataset" --model "name of the
-model" --init_from "pretrained file path" \ --name_relu_bound "name of bounded
-relu" --name_serach_bound "name of the search algorithm" --bounds_type "type of
-thresholds" --bitflip "value representaiton" ``` ## Code ### Structure The main
-source code of framework is held in `src/rrelu`, which carries `search_bounds`,
-`relu_bounds` , `extended pytorchfi` and other implementations. ## Citation
-View the [published paper](). If you use or reference rrelu, please cite: ```
-```
+ranger.py)). ## Usage Download on PyPI [here](https://pypi.org/project/rrelu/).
+### Installing **From Pip** Install using `pip install rrelu` **From Source**
+Download this repository into your project folder. ### Importing Import the
+entire package: ```python import rrelu ``` Import a specific module: ```python
+from rrelu.search_bound import proact_bounds ``` ### Testing -- running and
+evaluating algorithms: ```python torchpack dist-run -np 1 python
+rrelu.search.py --dataset "dataset name (CIFAR10, CIFAR100)" --data_path "path
+to the dataset" --model "name of the model" --init_from "pretrained file path"
+\ --name_relu_bound "name of bounded relu" --name_serach_bound "name of the
+search algorithm" --bounds_type "type of thresholds" --bitflip "value
+representaiton" ``` ## Code ### Structure The main source code of framework is
+held in `src/rrelu`, which carries `search_bounds`, `relu_bounds` , `extended
+pytorchfi` and other implementations. ## Citation View the [published paper]().
+If you use or reference rrelu, please cite: ``` ```
```

### Comparing `rrelu-0.0.4/pyproject.toml` & `rrelu-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "rrelu"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Seyedhamidreza Mousavi", email="seyedhamidreza.mousavi@mdu.se" },
 ]
 description = "generate reliable relu activation function for DNNs"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `rrelu-0.0.4/setup.cfg` & `rrelu-0.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rrelu
-version = 0.0.4
+version = 0.0.5
 author = Seyedhamidreza Mousavi
 author_email = seyedhamidreza.mousavi@mdu.se
 description = generate reliable relu activation function for DNNs
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/hamidmousavi0/reliable-relu-toolbox
 project_urls =
```

### Comparing `rrelu-0.0.4/setup.py` & `rrelu-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "rrelu",
-    version = "0.0.4",
+    version = "0.0.5",
     author = "Seyedhamidreza Mousavi",
     author_email = "seyedhamidreza.mousavi@mdu.se",
     description = "generate reliable relu activation function for DNNs",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/hamidmousavi0/reliable-relu-toolbox",
     project_urls = {
```

### Comparing `rrelu-0.0.4/src/rrelu/eval.py` & `rrelu-0.0.5/src/rrelu/eval.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import argparse
 import os
 from fxpmath import Fxp
 import torch.backends.cudnn
 import torch.nn as nn
 from torchpack import distributed as dist
 
-from setup import build_data_loader, build_model
-from train import eval,eval_fault
-from utils import load_state_dict_from_file
+from rrelu.setup import build_data_loader, build_model
+from rrelu.train import eval,eval_fault
+from rrelu.utils import load_state_dict_from_file
 
 parser = argparse.ArgumentParser()
 parser.add_argument(
     "--gpu", type=str, default=None
 )  # used in single machine experiments
 parser.add_argument("--batch_size", type=int, default=100)
 parser.add_argument("--n_worker", type=int, default=8)
@@ -93,8 +93,8 @@
     val_results = eval(model, data_loader_dict)
     val_results_fault = eval_fault(model,data_loader_dict,args.fault_rate,args.iterations,args.bitflip,args.n_word,args.n_frac,args.n_int,args.q_bit)
 
     for key, val in val_results.items():
         print(key, ": ", val)
     print("###########################################\n")
     for key, val in val_results_fault.items():
-        print(key, ": ", val)
+        print(key, ": ", val)
```

### Comparing `rrelu-0.0.4/src/rrelu/models/alexnet.py` & `rrelu-0.0.5/src/rrelu/models/alexnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch.optim as optim
 import torchvision.transforms as transforms
 import torch.nn as nn
-from relu_bound.bound_relu import Relu_bound
+from rrelu.relu_bound.bound_relu import Relu_bound
 class AlexNet_model(nn.Module):
     def __init__(self, n_classes=10,dropout_rate=0.0):
         super(AlexNet_model, self).__init__()
         self.conv1 =  nn.Conv2d(3, 64, kernel_size=3, stride=2, padding=1)
         self.relu1 = nn.ReLU()
         self.maxpool1 =  nn.MaxPool2d(kernel_size=2, stride=2)
         self.conv2 = nn.Conv2d(64, 192, kernel_size=3, padding=2)
```

### Comparing `rrelu-0.0.4/src/rrelu/models/alexnet_cifar100.py` & `rrelu-0.0.5/src/rrelu/models/alexnet_cifar100.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.4/src/rrelu/models/lenet.py` & `rrelu-0.0.5/src/rrelu/models/lenet.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.4/src/rrelu/models/resnet.py` & `rrelu-0.0.5/src/rrelu/models/resnet.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.4/src/rrelu/models/resnet_cifar100.py` & `rrelu-0.0.5/src/rrelu/models/resnet_cifar100.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.4/src/rrelu/models/vgg.py` & `rrelu-0.0.5/src/rrelu/models/vgg.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.4/src/rrelu/models/vgg_cifar100.py` & `rrelu-0.0.5/src/rrelu/models/vgg_cifar100.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.4/src/rrelu/pytorchfi/core.py` & `rrelu-0.0.5/src/rrelu/pytorchfi/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import copy
 import logging
 import warnings
 from typing import List
 
 import torch
 import torch.nn as nn
-from relu_bound.bound_relu import Relu_bound
+from rrelu.relu_bound.bound_relu import Relu_bound
 
 class FaultInjection:
     def __init__(
         self,
         model,
         batch_size: int,
         input_shape: List[int] = None,
```

### Comparing `rrelu-0.0.4/src/rrelu/pytorchfi/core_train.py` & `rrelu-0.0.5/src/rrelu/pytorchfi/core_train.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import copy
 import logging
 import warnings
 from typing import List
 
 import torch
 import torch.nn as nn
-from relu_bound.bound_relu import Relu_bound
+from rrelu.relu_bound.bound_relu import Relu_bound
 
 class FaultInjection:
     def __init__(
         self,
         model,
         batch_size: int,
         input_shape: List[int] = None,
```

### Comparing `rrelu-0.0.4/src/rrelu/pytorchfi/neuron_error_models.py` & `rrelu-0.0.5/src/rrelu/pytorchfi/neuron_error_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """pytorchfi.error_models provides different error models out-of-the-box for use."""
 
 import logging
 import random
 
 import torch
 
-from pytorchfi import core
-from pytorchfi.util import random_value
+from rrelu.pytorchfi import core
+from rrelu.pytorchfi.util import random_value
 
 # Helper Functions
 
 
 def random_batch_element(pfi: core.FaultInjection):
     return random.randint(0, pfi.batch_size - 1)
```

### Comparing `rrelu-0.0.4/src/rrelu/pytorchfi/weight_error_models.py` & `rrelu-0.0.5/src/rrelu/pytorchfi/weight_error_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """pytorchfi.error_models provides different error models out-of-the-box for use."""
 
 import random
 from fxpmath import Fxp
-import pytorchfi.core as core 
-from pytorchfi.util import random_value
+import rrelu.pytorchfi.core as core 
+from rrelu.pytorchfi.util import random_value
 import logging
 import torch
 import numpy as np
 def random_weight_location(pfi, layer: int = -1):
     if layer == -1:
         layer = random.randint(0, pfi.get_total_layers() - 1)
```

### Comparing `rrelu-0.0.4/src/rrelu/relu_bound/bound_fitact.py` & `rrelu-0.0.5/src/rrelu/relu_bound/bound_fitact.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import torch
 import torch.nn as nn
-from relu_bound.bound_relu import Relu_bound
+from rrelu.relu_bound.bound_relu import Relu_bound
 class bounded_relu_fitact(nn.Module,Relu_bound):
     def __init__(self,bounds,tresh=None,alpha = None,k=-20):
         super().__init__()
         bounds_param={}
         param_name= "bounds_param"
         self.tresh = None
         bounds_param[param_name] = nn.Parameter(data=bounds.cuda(), requires_grad=True)
```

### Comparing `rrelu-0.0.4/src/rrelu/relu_bound/bound_proact.py` & `rrelu-0.0.5/src/rrelu/relu_bound/bound_proact.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 import torch
 import torch.nn as nn
-from relu_bound.bound_relu import Relu_bound
+from rrelu.relu_bound.bound_relu import Relu_bound
 import torch.nn.functional as F
 
 class bounded_hyrelu_proact(nn.Module,Relu_bound):
     def __init__(self,bounds=None,tresh=None,alpha_param = None,k=-20):
         super().__init__()
         bounds_param={}
         param_name1= "bounds_param"
```

### Comparing `rrelu-0.0.4/src/rrelu/relu_bound/bound_tresh.py` & `rrelu-0.0.5/src/rrelu/relu_bound/bound_tresh.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 import torch
 import torch.nn as nn
-from relu_bound.bound_relu import Relu_bound
+from rrelu.relu_bound.bound_relu import Relu_bound
 class bounded_relu_tresh(nn.Module,Relu_bound):
     '''
     Bound the relu activatoin and back the values to treshold
     ------------------------------------
     bound : the bound for the activation
     -------------------------------------
     pytorch module with forward function
@@ -14,8 +14,8 @@
         super().__init__()
         self.bounds = bounds
         self.tresh = tresh
     def forward(self, input):
         # input = torch.nan_to_num(input)
         output = torch.ones_like(input) * input
         output[torch.gt(input,self.bounds)] = self.tresh
-        return torch.maximum(torch.tensor(0.0),output)       
+        return torch.maximum(torch.tensor(0.0),output)
```

### Comparing `rrelu-0.0.4/src/rrelu/relu_bound/bound_zero.py` & `rrelu-0.0.5/src/rrelu/relu_bound/bound_zero.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import torch
 import torch.nn as nn
-from relu_bound.bound_relu import Relu_bound
+from rrelu.relu_bound.bound_relu import Relu_bound
 class bounded_relu_zero(nn.Module,Relu_bound):
     '''
     Bound the relu activatoin and back the values to zero
     ------------------------------------
     bound : the bound for the activation
     --------------------------------------
     pytorch module with forward function
@@ -13,8 +13,8 @@
         super().__init__()
         self.bounds = bounds
         self.tresh = None
     def forward(self, input):
         # input = torch.nan_to_num(input)
         output = torch.ones_like(input) * input
         output[torch.gt(input,self.bounds)] = torch.tensor(0.0)
-        return torch.maximum(torch.tensor(0.0),output)      
+        return torch.maximum(torch.tensor(0.0),output)
```

### Comparing `rrelu-0.0.4/src/rrelu/search.py` & `rrelu-0.0.5/src/rrelu/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import argparse
 import os
 import torch.backends.cudnn
 import torch.nn as nn
 from fxpmath import Fxp
 from torchpack import distributed as dist
 import copy
-from setup import build_data_loader, build_model ,replace_act,replace_act_all
-from utils import load_state_dict_from_file
-from train import eval_fault,eval
+from rrelu.setup import build_data_loader, build_model ,replace_act,replace_act_all
+from rrelu.utils import load_state_dict_from_file
+from rrelu.train import eval_fault,eval
 import random
 import numpy as np 
 parser = argparse.ArgumentParser()
 parser.add_argument(
     "--gpu", type=str, default=None
 )  # used in single machine experiments
 parser.add_argument("--batch_size", type=int, default=128)
```

### Comparing `rrelu-0.0.4/src/rrelu/search_bound/fitact.py` & `rrelu-0.0.5/src/rrelu/search_bound/fitact.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 import torch.nn as nn
 import torch
 import copy
 import numpy as np
 import warnings
 import sys; 
 import setup 
-from relu_bound.bound_fitact import bounded_relu_fitact
+from rrelu.relu_bound.bound_fitact import bounded_relu_fitact
 import os
 import argparse
-from utils.metric import accuracy,AverageMeter
-from utils.lr_scheduler import CosineLRwithWarmup
-from utils.distributed import DistributedMetric
-from search_bound.ranger import Ranger_bounds
+from rrelu.utils.metric import accuracy,AverageMeter
+from rrelu.utils.lr_scheduler import CosineLRwithWarmup
+from rrelu.utils.distributed import DistributedMetric
+from rrelu.search_bound.ranger import Ranger_bounds
 import random
 import time
 from tqdm import tqdm
 from torchpack import distributed as dist
 parser = argparse.ArgumentParser()
 parser.add_argument("--path", type=str, metavar="DIR", help="run directory",default="./pretrained_models/teachers/vgg16_bound_layer_relu_float/checkpoint")
 parser.add_argument("--base_batch_size", type=int, default=128)
```

### Comparing `rrelu-0.0.4/src/rrelu/search_bound/ftclip.py` & `rrelu-0.0.5/src/rrelu/search_bound/ftclip.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import sys
 import torch
 import numpy as np
 import torch
 import copy
 import torch.nn as nn 
 import setup 
-from pytorchfi.core import FaultInjection
-from utils.distributed import DistributedMetric
+from rrelu.pytorchfi.core import FaultInjection
+from rrelu.utils.distributed import DistributedMetric
 from tqdm import tqdm
 from torchpack import distributed as dist
-from utils import load_state_dict_from_file
-from utils.metric import accuracy
-from pytorchfi.weight_error_models import bit_flip_weight_IEEE,bit_flip_weight_fixed,bit_flip_weight_int
-from relu_bound.bound_zero import bounded_relu_zero 
-from relu_bound.bound_relu import Relu_bound
+from rrelu.utils import load_state_dict_from_file
+from rrelu.utils.metric import accuracy
+from rrelu.pytorchfi.weight_error_models import bit_flip_weight_IEEE,bit_flip_weight_fixed,bit_flip_weight_int
+from rrelu.relu_bound.bound_zero import bounded_relu_zero 
+from rrelu.relu_bound.bound_relu import Relu_bound
 import random
 activation={}
 def get_activation(name):
     def hook(model, input, output):
         activation[name] = output
     return hook
 
@@ -394,8 +394,8 @@
         n_frac = n_frac, 
         n_int = n_int, 
     )
 
 
 
 
-###############################################################################################
+###############################################################################################
```

### Comparing `rrelu-0.0.4/src/rrelu/search_bound/proact.py` & `rrelu-0.0.5/src/rrelu/search_bound/proact.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 import torch.nn as nn
 import torch
 import copy
 import numpy as np
 import warnings
 import sys;
 import setup 
-from relu_bound.bound_proact import bounded_hyrelu_proact
-from relu_bound.bound_zero import bounded_relu_zero
+from rrelu.relu_bound.bound_proact import bounded_hyrelu_proact
+from rrelu.relu_bound.bound_zero import bounded_relu_zero
 import os
 import argparse
 from typing import Dict, Optional
-from relu_bound.bound_relu import Relu_bound
-from pytorchfi.weight_error_models import multi_weight_inj_float,multi_weight_inj_fixed,multi_weight_inj_int
-from utils.metric import accuracy,AverageMeter
-from utils.lr_scheduler import CosineLRwithWarmup
-from utils.distributed import DistributedMetric
+from rrelu.relu_bound.bound_relu import Relu_bound
+from rrelu.pytorchfi.weight_error_models import multi_weight_inj_float,multi_weight_inj_fixed,multi_weight_inj_int
+from rrelu.utils.metric import accuracy,AverageMeter
+from rrelu.utils.lr_scheduler import CosineLRwithWarmup
+from rrelu.utils.distributed import DistributedMetric
 import random
-from pytorchfi.core import FaultInjection
+from rrelu.pytorchfi.core import FaultInjection
 import torch.nn.functional as F
 import time
 from tqdm import tqdm
 from torchpack import distributed as dist
 parser = argparse.ArgumentParser()
 parser.add_argument("--path", type=str, metavar="DIR", help="run directory",default="pretrained_models/lenet_mnist")
 parser.add_argument("--base_batch_size", type=int, default=128)
```

### Comparing `rrelu-0.0.4/src/rrelu/search_bound/ranger.py` & `rrelu-0.0.5/src/rrelu/search_bound/ranger.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.4/src/rrelu/setup.py` & `rrelu-0.0.5/src/rrelu/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,35 +3,35 @@
 import os.path
 from typing import Dict, Optional, Tuple, Type
 
 import torch
 import torch.nn as nn
 import torchvision.datasets as datasets
 import torchvision.transforms as transforms
-from models.vgg import make_layers,cfg
-from models import (
+from rrelu.models.vgg import make_layers,cfg
+from rrelu.models import (
    Lenet,
    VGG,
    AlexNet_model,
    ResNet50,
    VGG16,
    LeNet_cifar,
    AlexNet_cifar100,
    VGG16_cifar100,
    ResNet50_cifar100,
 )
-from relu_bound import (
+from rrelu.relu_bound import (
     bounded_relu_zero,
     bounded_relu_tresh,
     bounded_relu_fitact,
     bounded_hyrelu_proact
 
 )
 
-from search_bound import (
+from rrelu.search_bound import (
     FtClipAct_bounds,
     Ranger_bounds,
     fitact_bounds,
     proact_bounds
 
 )
 __all__ = ["build_data_loader", "build_model", "replace_act","find_bounds"]
```

### Comparing `rrelu-0.0.4/src/rrelu/train.py` & `rrelu-0.0.5/src/rrelu/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import torch.nn as nn 
 import torch.optim as optim 
 import torch
 from torch import autograd
 from typing import Dict
-from utils.distributed import DistributedMetric
+from rrelu.utils.distributed import DistributedMetric
 import argparse
 import copy
 import os
 import time
 import warnings
 from typing import Dict, Optional
-from setup import build_data_loader,build_model
+from rrelu.setup import build_data_loader,build_model
 import numpy as np
 import torch
 import torch.nn as nn
 import yaml
 from torchpack import distributed as dist
 from tqdm import tqdm
-from utils.metric import accuracy,AverageMeter
-from utils.lr_scheduler import CosineLRwithWarmup
-from utils.init import load_state_dict,init_modules
-from utils import load_state_dict_from_file
-from pytorchfi.weight_error_models import multi_weight_inj_fixed,multi_weight_inj_float,multi_weight_inj_int
-from relu_bound.bound_relu import Relu_bound
-from pytorchfi.core import FaultInjection
+from rrelu.utils.metric import accuracy,AverageMeter
+from rrelu.utils.lr_scheduler import CosineLRwithWarmup
+from rrelu.utils.init import load_state_dict,init_modules
+from rrelu.utils import load_state_dict_from_file
+from rrelu.pytorchfi.weight_error_models import multi_weight_inj_fixed,multi_weight_inj_float,multi_weight_inj_int
+from rrelu.relu_bound.bound_relu import Relu_bound
+from rrelu.pytorchfi.core import FaultInjection
 import random 
 import numpy as np
 import matplotlib.pyplot as plt
 parser = argparse.ArgumentParser()
 
 parser.add_argument("--path", type=str, metavar="DIR", help="run directory",default="pretrained_models/resnet50_cifar100")
 parser.add_argument("--dataset", type=str, help="dataset",default="cifar100")
@@ -383,8 +383,8 @@
     generator.manual_seed(args.manual_seed)
     model = nn.parallel.DistributedDataParallel(
         model.cuda(), device_ids=[dist.local_rank()]
     )
     train(model, data_provider, args.path, args.resume)
     # eval_fault(model,data_provider,1e-3)
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `rrelu-0.0.4/src/rrelu/utils/distributed.py` & `rrelu-0.0.5/src/rrelu/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.4/src/rrelu/utils/init.py` & `rrelu-0.0.5/src/rrelu/utils/init.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.4/src/rrelu/utils/lr_scheduler.py` & `rrelu-0.0.5/src/rrelu/utils/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.4/src/rrelu/utils/metric.py` & `rrelu-0.0.5/src/rrelu/utils/metric.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.4/src/rrelu/utils/misc.py` & `rrelu-0.0.5/src/rrelu/utils/misc.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.4/src/rrelu.egg-info/PKG-INFO` & `rrelu-0.0.5/src/rrelu.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rrelu
-Version: 0.0.4
+Version: 0.0.5
 Summary: generate reliable relu activation function for DNNs
 Home-page: https://github.com/hamidmousavi0/reliable-relu-toolbox
 Author: Seyedhamidreza Mousavi
 Author-email: Seyedhamidreza Mousavi <seyedhamidreza.mousavi@mdu.se>
 Project-URL: Homepage, https://github.com/hamidmousavi0/reliable-relu-toolbox
 Project-URL: Issues, https://github.com/hamidmousavi0/reliable-relu-toolbox/issues
 Classifier: Programming Language :: Python :: 3
@@ -34,15 +34,15 @@
 * **ProAct** (the proposed algorithm) ([code](https://github.com/hamidmousavi0/reliable-relu-toolbox/blob/master/src/search_bound/proact.py)).
 * **FitAct** ([paper](https://arxiv.org/pdf/2112.13544) and [code](https://github.com/hamidmousavi0/reliable-relu-toolbox/blob/master/src/search_bound/fitact.py)).
 * **FtClipAct** ([paper](https://arxiv.org/pdf/1912.00941) and [code](https://github.com/hamidmousavi0/reliable-relu-toolbox/blob/master/src/search_bound/ftclip.py)).
 * **Ranger** ([paper](https://arxiv.org/pdf/2003.13874) and [code](https://github.com/hamidmousavi0/reliable-relu-toolbox/blob/master/src/search_bound/ranger.py)).
 
 ## Usage
 
-Download on PyPI [here]().
+Download on PyPI [here](https://pypi.org/project/rrelu/).
 
 ### Installing
 
 **From Pip**
 
 Install using `pip install rrelu`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rrelu Version: 0.0.4 Summary: generate reliable
+Metadata-Version: 2.1 Name: rrelu Version: 0.0.5 Summary: generate reliable
 relu activation function for DNNs Home-page: https://github.com/hamidmousavi0/
 reliable-relu-toolbox Author: Seyedhamidreza Mousavi Author-email:
 Seyedhamidreza Mousavi
 mdu.se> Project-URL: Homepage, https://github.com/hamidmousavi0/reliable-relu-
 toolbox Project-URL: Issues, https://github.com/hamidmousavi0/reliable-relu-
 toolbox/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
@@ -28,21 +28,21 @@
 toolbox/blob/master/src/search_bound/proact.py)). * **FitAct** ([paper](https:/
 /arxiv.org/pdf/2112.13544) and [code](https://github.com/hamidmousavi0/
 reliable-relu-toolbox/blob/master/src/search_bound/fitact.py)). * **FtClipAct**
 ([paper](https://arxiv.org/pdf/1912.00941) and [code](https://github.com/
 hamidmousavi0/reliable-relu-toolbox/blob/master/src/search_bound/ftclip.py)). *
 **Ranger** ([paper](https://arxiv.org/pdf/2003.13874) and [code](https://
 github.com/hamidmousavi0/reliable-relu-toolbox/blob/master/src/search_bound/
-ranger.py)). ## Usage Download on PyPI [here](). ### Installing **From Pip**
-Install using `pip install rrelu` **From Source** Download this repository into
-your project folder. ### Importing Import the entire package: ```python import
-rrelu ``` Import a specific module: ```python from rrelu.search_bound import
-proact_bounds ``` ### Testing -- running and evaluating algorithms: ```python
-torchpack dist-run -np 1 python rrelu.search.py --dataset "dataset name
-(CIFAR10, CIFAR100)" --data_path "path to the dataset" --model "name of the
-model" --init_from "pretrained file path" \ --name_relu_bound "name of bounded
-relu" --name_serach_bound "name of the search algorithm" --bounds_type "type of
-thresholds" --bitflip "value representaiton" ``` ## Code ### Structure The main
-source code of framework is held in `src/rrelu`, which carries `search_bounds`,
-`relu_bounds` , `extended pytorchfi` and other implementations. ## Citation
-View the [published paper](). If you use or reference rrelu, please cite: ```
-```
+ranger.py)). ## Usage Download on PyPI [here](https://pypi.org/project/rrelu/).
+### Installing **From Pip** Install using `pip install rrelu` **From Source**
+Download this repository into your project folder. ### Importing Import the
+entire package: ```python import rrelu ``` Import a specific module: ```python
+from rrelu.search_bound import proact_bounds ``` ### Testing -- running and
+evaluating algorithms: ```python torchpack dist-run -np 1 python
+rrelu.search.py --dataset "dataset name (CIFAR10, CIFAR100)" --data_path "path
+to the dataset" --model "name of the model" --init_from "pretrained file path"
+\ --name_relu_bound "name of bounded relu" --name_serach_bound "name of the
+search algorithm" --bounds_type "type of thresholds" --bitflip "value
+representaiton" ``` ## Code ### Structure The main source code of framework is
+held in `src/rrelu`, which carries `search_bounds`, `relu_bounds` , `extended
+pytorchfi` and other implementations. ## Citation View the [published paper]().
+If you use or reference rrelu, please cite: ``` ```
```

### Comparing `rrelu-0.0.4/src/rrelu.egg-info/SOURCES.txt` & `rrelu-0.0.5/src/rrelu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

