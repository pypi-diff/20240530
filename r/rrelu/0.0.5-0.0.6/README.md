# Comparing `tmp/rrelu-0.0.5.tar.gz` & `tmp/rrelu-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rrelu-0.0.5.tar", last modified: Thu May 30 11:38:03 2024, max compression
+gzip compressed data, was "rrelu-0.0.6.tar", last modified: Thu May 30 12:45:11 2024, max compression
```

## Comparing `rrelu-0.0.5.tar` & `rrelu-0.0.6.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 11:38:03.314320 rrelu-0.0.5/
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     1079 2024-05-30 11:37:03.000000 rrelu-0.0.5/LICENSE.txt
--rw-rw-r--   0 a4000     (1000) a4000     (1000)        0 2024-05-30 11:37:03.000000 rrelu-0.0.5/MANIFEST.in
--rw-r--r--   0 a4000     (1000) a4000     (1000)     3650 2024-05-30 11:38:03.314320 rrelu-0.0.5/PKG-INFO
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     2977 2024-05-30 11:37:03.000000 rrelu-0.0.5/README.md
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      554 2024-05-30 11:37:03.000000 rrelu-0.0.5/pyproject.toml
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      696 2024-05-30 11:38:03.314320 rrelu-0.0.5/setup.cfg
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      898 2024-05-30 11:37:03.000000 rrelu-0.0.5/setup.py
-drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 11:38:03.306320 rrelu-0.0.5/src/
-drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 11:38:03.306320 rrelu-0.0.5/src/rrelu/
--rw-rw-r--   0 a4000     (1000) a4000     (1000)        2 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/__init__.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     3547 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/eval.py
-drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 11:38:03.310320 rrelu-0.0.5/src/rrelu/models/
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      260 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/models/__init__.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     2881 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/models/alexnet.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     1232 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/models/alexnet_cifar100.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     2965 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/models/lenet.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     4839 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/models/resnet.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     4848 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/models/resnet_cifar100.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     2560 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/models/vgg.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     2580 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/models/vgg_cifar100.py
-drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 11:38:03.310320 rrelu-0.0.5/src/rrelu/pytorchfi/
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      170 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/pytorchfi/__init__.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)    21661 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/pytorchfi/core.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)    21717 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/pytorchfi/core_train.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)    10480 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/pytorchfi/neuron_error_models.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      115 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/pytorchfi/util.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)    22096 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/pytorchfi/weight_error_models.py
-drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 11:38:03.310320 rrelu-0.0.5/src/rrelu/relu_bound/
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      173 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/relu_bound/__init__.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      829 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/relu_bound/bound_fitact.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     1082 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/relu_bound/bound_proact.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)       95 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/relu_bound/bound_relu.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      761 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/relu_bound/bound_tresh.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      766 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/relu_bound/bound_zero.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     5070 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/search.py
-drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 11:38:03.314320 rrelu-0.0.5/src/rrelu/search_bound/
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      161 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/search_bound/__init__.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)    10420 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/search_bound/fitact.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)    18037 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/search_bound/ftclip.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)    18122 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/search_bound/proact.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     1718 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/search_bound/ranger.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)    11543 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/setup.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)    13480 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/train.py
-drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 11:38:03.314320 rrelu-0.0.5/src/rrelu/utils/
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      172 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/utils/__init__.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     1659 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/utils/distributed.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     2811 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/utils/init.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     1094 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/utils/lr_scheduler.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     1218 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/utils/metric.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     3612 2024-05-30 11:37:03.000000 rrelu-0.0.5/src/rrelu/utils/misc.py
-drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 11:38:03.314320 rrelu-0.0.5/src/rrelu.egg-info/
--rw-r--r--   0 a4000     (1000) a4000     (1000)     3650 2024-05-30 11:38:03.000000 rrelu-0.0.5/src/rrelu.egg-info/PKG-INFO
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     1290 2024-05-30 11:38:03.000000 rrelu-0.0.5/src/rrelu.egg-info/SOURCES.txt
--rw-rw-r--   0 a4000     (1000) a4000     (1000)        1 2024-05-30 11:38:03.000000 rrelu-0.0.5/src/rrelu.egg-info/dependency_links.txt
--rw-rw-r--   0 a4000     (1000) a4000     (1000)        6 2024-05-30 11:38:03.000000 rrelu-0.0.5/src/rrelu.egg-info/top_level.txt
+drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 12:45:11.555160 rrelu-0.0.6/
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     1079 2024-05-30 12:38:45.000000 rrelu-0.0.6/LICENSE.txt
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)        0 2024-05-30 12:38:45.000000 rrelu-0.0.6/MANIFEST.in
+-rw-r--r--   0 a4000     (1000) a4000     (1000)     3650 2024-05-30 12:45:11.555160 rrelu-0.0.6/PKG-INFO
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     2977 2024-05-30 12:38:45.000000 rrelu-0.0.6/README.md
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      554 2024-05-30 12:38:45.000000 rrelu-0.0.6/pyproject.toml
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      696 2024-05-30 12:45:11.555160 rrelu-0.0.6/setup.cfg
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      898 2024-05-30 12:38:45.000000 rrelu-0.0.6/setup.py
+drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 12:45:11.543160 rrelu-0.0.6/src/
+drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 12:45:11.547160 rrelu-0.0.6/src/rrelu/
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      108 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/__init__.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     3547 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/eval.py
+drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 12:45:11.551160 rrelu-0.0.6/src/rrelu/models/
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      260 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/models/__init__.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     2881 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/models/alexnet.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     1232 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/models/alexnet_cifar100.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     2965 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/models/lenet.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     4839 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/models/resnet.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     4848 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/models/resnet_cifar100.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     2560 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/models/vgg.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     2580 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/models/vgg_cifar100.py
+drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 12:45:11.551160 rrelu-0.0.6/src/rrelu/pytorchfi/
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      170 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/pytorchfi/__init__.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)    21661 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/pytorchfi/core.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)    21717 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/pytorchfi/core_train.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)    10480 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/pytorchfi/neuron_error_models.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      115 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/pytorchfi/util.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)    22096 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/pytorchfi/weight_error_models.py
+drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 12:45:11.551160 rrelu-0.0.6/src/rrelu/relu_bound/
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      173 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/relu_bound/__init__.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      829 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/relu_bound/bound_fitact.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     1082 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/relu_bound/bound_proact.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)       95 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/relu_bound/bound_relu.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      761 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/relu_bound/bound_tresh.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      766 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/relu_bound/bound_zero.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     5070 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/search.py
+drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 12:45:11.551160 rrelu-0.0.6/src/rrelu/search_bound/
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      161 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/search_bound/__init__.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)    10420 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/search_bound/fitact.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)    18037 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/search_bound/ftclip.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)    18122 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/search_bound/proact.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     1718 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/search_bound/ranger.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)    11543 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/setup.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)    13480 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/train.py
+drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 12:45:11.555160 rrelu-0.0.6/src/rrelu/utils/
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      172 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/utils/__init__.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     1659 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/utils/distributed.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     2811 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/utils/init.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     1094 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/utils/lr_scheduler.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     1218 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/utils/metric.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     3612 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/utils/misc.py
+drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 12:45:11.555160 rrelu-0.0.6/src/rrelu.egg-info/
+-rw-r--r--   0 a4000     (1000) a4000     (1000)     3650 2024-05-30 12:45:11.000000 rrelu-0.0.6/src/rrelu.egg-info/PKG-INFO
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     1290 2024-05-30 12:45:11.000000 rrelu-0.0.6/src/rrelu.egg-info/SOURCES.txt
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)        1 2024-05-30 12:45:11.000000 rrelu-0.0.6/src/rrelu.egg-info/dependency_links.txt
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)        6 2024-05-30 12:45:11.000000 rrelu-0.0.6/src/rrelu.egg-info/top_level.txt
```

### Comparing `rrelu-0.0.5/LICENSE.txt` & `rrelu-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.5/PKG-INFO` & `rrelu-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rrelu
-Version: 0.0.5
+Version: 0.0.6
 Summary: generate reliable relu activation function for DNNs
 Home-page: https://github.com/hamidmousavi0/reliable-relu-toolbox
 Author: Seyedhamidreza Mousavi
 Author-email: Seyedhamidreza Mousavi <seyedhamidreza.mousavi@mdu.se>
 Project-URL: Homepage, https://github.com/hamidmousavi0/reliable-relu-toolbox
 Project-URL: Issues, https://github.com/hamidmousavi0/reliable-relu-toolbox/issues
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rrelu Version: 0.0.5 Summary: generate reliable
+Metadata-Version: 2.1 Name: rrelu Version: 0.0.6 Summary: generate reliable
 relu activation function for DNNs Home-page: https://github.com/hamidmousavi0/
 reliable-relu-toolbox Author: Seyedhamidreza Mousavi Author-email:
 Seyedhamidreza Mousavi
 mdu.se> Project-URL: Homepage, https://github.com/hamidmousavi0/reliable-relu-
 toolbox Project-URL: Issues, https://github.com/hamidmousavi0/reliable-relu-
 toolbox/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
```

### Comparing `rrelu-0.0.5/README.md` & `rrelu-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.5/pyproject.toml` & `rrelu-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "rrelu"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Seyedhamidreza Mousavi", email="seyedhamidreza.mousavi@mdu.se" },
 ]
 description = "generate reliable relu activation function for DNNs"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `rrelu-0.0.5/setup.cfg` & `rrelu-0.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rrelu
-version = 0.0.5
+version = 0.0.6
 author = Seyedhamidreza Mousavi
 author_email = seyedhamidreza.mousavi@mdu.se
 description = generate reliable relu activation function for DNNs
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/hamidmousavi0/reliable-relu-toolbox
 project_urls =
```

### Comparing `rrelu-0.0.5/setup.py` & `rrelu-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "rrelu",
-    version = "0.0.5",
+    version = "0.0.6",
     author = "Seyedhamidreza Mousavi",
     author_email = "seyedhamidreza.mousavi@mdu.se",
     description = "generate reliable relu activation function for DNNs",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/hamidmousavi0/reliable-relu-toolbox",
     project_urls = {
```

### Comparing `rrelu-0.0.5/src/rrelu/eval.py` & `rrelu-0.0.6/src/rrelu/eval.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.5/src/rrelu/models/alexnet.py` & `rrelu-0.0.6/src/rrelu/models/alexnet.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.5/src/rrelu/models/alexnet_cifar100.py` & `rrelu-0.0.6/src/rrelu/models/alexnet_cifar100.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.5/src/rrelu/models/lenet.py` & `rrelu-0.0.6/src/rrelu/models/lenet.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.5/src/rrelu/models/resnet.py` & `rrelu-0.0.6/src/rrelu/models/resnet.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.5/src/rrelu/models/resnet_cifar100.py` & `rrelu-0.0.6/src/rrelu/models/resnet_cifar100.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.5/src/rrelu/models/vgg.py` & `rrelu-0.0.6/src/rrelu/models/vgg.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.5/src/rrelu/models/vgg_cifar100.py` & `rrelu-0.0.6/src/rrelu/models/vgg_cifar100.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.5/src/rrelu/pytorchfi/core.py` & `rrelu-0.0.6/src/rrelu/pytorchfi/core.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.5/src/rrelu/pytorchfi/core_train.py` & `rrelu-0.0.6/src/rrelu/pytorchfi/core_train.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.5/src/rrelu/pytorchfi/neuron_error_models.py` & `rrelu-0.0.6/src/rrelu/pytorchfi/neuron_error_models.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.5/src/rrelu/pytorchfi/weight_error_models.py` & `rrelu-0.0.6/src/rrelu/pytorchfi/weight_error_models.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.5/src/rrelu/relu_bound/bound_fitact.py` & `rrelu-0.0.6/src/rrelu/relu_bound/bound_fitact.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.5/src/rrelu/relu_bound/bound_proact.py` & `rrelu-0.0.6/src/rrelu/relu_bound/bound_proact.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.5/src/rrelu/relu_bound/bound_tresh.py` & `rrelu-0.0.6/src/rrelu/relu_bound/bound_tresh.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.5/src/rrelu/relu_bound/bound_zero.py` & `rrelu-0.0.6/src/rrelu/relu_bound/bound_zero.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.5/src/rrelu/search.py` & `rrelu-0.0.6/src/rrelu/search.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.5/src/rrelu/search_bound/fitact.py` & `rrelu-0.0.6/src/rrelu/search_bound/fitact.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.5/src/rrelu/search_bound/ftclip.py` & `rrelu-0.0.6/src/rrelu/search_bound/ftclip.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.5/src/rrelu/search_bound/proact.py` & `rrelu-0.0.6/src/rrelu/search_bound/proact.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.5/src/rrelu/search_bound/ranger.py` & `rrelu-0.0.6/src/rrelu/search_bound/ranger.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.5/src/rrelu/setup.py` & `rrelu-0.0.6/src/rrelu/setup.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.5/src/rrelu/train.py` & `rrelu-0.0.6/src/rrelu/train.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.5/src/rrelu/utils/distributed.py` & `rrelu-0.0.6/src/rrelu/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.5/src/rrelu/utils/init.py` & `rrelu-0.0.6/src/rrelu/utils/init.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.5/src/rrelu/utils/lr_scheduler.py` & `rrelu-0.0.6/src/rrelu/utils/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.5/src/rrelu/utils/metric.py` & `rrelu-0.0.6/src/rrelu/utils/metric.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.5/src/rrelu/utils/misc.py` & `rrelu-0.0.6/src/rrelu/utils/misc.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.5/src/rrelu.egg-info/PKG-INFO` & `rrelu-0.0.6/src/rrelu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rrelu
-Version: 0.0.5
+Version: 0.0.6
 Summary: generate reliable relu activation function for DNNs
 Home-page: https://github.com/hamidmousavi0/reliable-relu-toolbox
 Author: Seyedhamidreza Mousavi
 Author-email: Seyedhamidreza Mousavi <seyedhamidreza.mousavi@mdu.se>
 Project-URL: Homepage, https://github.com/hamidmousavi0/reliable-relu-toolbox
 Project-URL: Issues, https://github.com/hamidmousavi0/reliable-relu-toolbox/issues
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rrelu Version: 0.0.5 Summary: generate reliable
+Metadata-Version: 2.1 Name: rrelu Version: 0.0.6 Summary: generate reliable
 relu activation function for DNNs Home-page: https://github.com/hamidmousavi0/
 reliable-relu-toolbox Author: Seyedhamidreza Mousavi Author-email:
 Seyedhamidreza Mousavi
 mdu.se> Project-URL: Homepage, https://github.com/hamidmousavi0/reliable-relu-
 toolbox Project-URL: Issues, https://github.com/hamidmousavi0/reliable-relu-
 toolbox/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
```

### Comparing `rrelu-0.0.5/src/rrelu.egg-info/SOURCES.txt` & `rrelu-0.0.6/src/rrelu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

