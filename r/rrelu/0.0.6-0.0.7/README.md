# Comparing `tmp/rrelu-0.0.6.tar.gz` & `tmp/rrelu-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rrelu-0.0.6.tar", last modified: Thu May 30 12:45:11 2024, max compression
+gzip compressed data, was "rrelu-0.0.7.tar", last modified: Thu May 30 13:10:46 2024, max compression
```

## Comparing `rrelu-0.0.6.tar` & `rrelu-0.0.7.tar`

### file list

```diff
@@ -1,56 +1,53 @@
-drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 12:45:11.555160 rrelu-0.0.6/
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     1079 2024-05-30 12:38:45.000000 rrelu-0.0.6/LICENSE.txt
--rw-rw-r--   0 a4000     (1000) a4000     (1000)        0 2024-05-30 12:38:45.000000 rrelu-0.0.6/MANIFEST.in
--rw-r--r--   0 a4000     (1000) a4000     (1000)     3650 2024-05-30 12:45:11.555160 rrelu-0.0.6/PKG-INFO
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     2977 2024-05-30 12:38:45.000000 rrelu-0.0.6/README.md
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      554 2024-05-30 12:38:45.000000 rrelu-0.0.6/pyproject.toml
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      696 2024-05-30 12:45:11.555160 rrelu-0.0.6/setup.cfg
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      898 2024-05-30 12:38:45.000000 rrelu-0.0.6/setup.py
-drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 12:45:11.543160 rrelu-0.0.6/src/
-drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 12:45:11.547160 rrelu-0.0.6/src/rrelu/
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      108 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/__init__.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     3547 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/eval.py
-drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 12:45:11.551160 rrelu-0.0.6/src/rrelu/models/
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      260 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/models/__init__.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     2881 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/models/alexnet.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     1232 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/models/alexnet_cifar100.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     2965 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/models/lenet.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     4839 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/models/resnet.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     4848 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/models/resnet_cifar100.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     2560 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/models/vgg.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     2580 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/models/vgg_cifar100.py
-drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 12:45:11.551160 rrelu-0.0.6/src/rrelu/pytorchfi/
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      170 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/pytorchfi/__init__.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)    21661 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/pytorchfi/core.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)    21717 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/pytorchfi/core_train.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)    10480 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/pytorchfi/neuron_error_models.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      115 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/pytorchfi/util.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)    22096 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/pytorchfi/weight_error_models.py
-drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 12:45:11.551160 rrelu-0.0.6/src/rrelu/relu_bound/
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      173 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/relu_bound/__init__.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      829 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/relu_bound/bound_fitact.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     1082 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/relu_bound/bound_proact.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)       95 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/relu_bound/bound_relu.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      761 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/relu_bound/bound_tresh.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      766 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/relu_bound/bound_zero.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     5070 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/search.py
-drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 12:45:11.551160 rrelu-0.0.6/src/rrelu/search_bound/
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      161 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/search_bound/__init__.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)    10420 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/search_bound/fitact.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)    18037 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/search_bound/ftclip.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)    18122 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/search_bound/proact.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     1718 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/search_bound/ranger.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)    11543 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/setup.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)    13480 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/train.py
-drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 12:45:11.555160 rrelu-0.0.6/src/rrelu/utils/
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      172 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/utils/__init__.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     1659 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/utils/distributed.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     2811 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/utils/init.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     1094 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/utils/lr_scheduler.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     1218 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/utils/metric.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     3612 2024-05-30 12:38:45.000000 rrelu-0.0.6/src/rrelu/utils/misc.py
-drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 12:45:11.555160 rrelu-0.0.6/src/rrelu.egg-info/
--rw-r--r--   0 a4000     (1000) a4000     (1000)     3650 2024-05-30 12:45:11.000000 rrelu-0.0.6/src/rrelu.egg-info/PKG-INFO
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     1290 2024-05-30 12:45:11.000000 rrelu-0.0.6/src/rrelu.egg-info/SOURCES.txt
--rw-rw-r--   0 a4000     (1000) a4000     (1000)        1 2024-05-30 12:45:11.000000 rrelu-0.0.6/src/rrelu.egg-info/dependency_links.txt
--rw-rw-r--   0 a4000     (1000) a4000     (1000)        6 2024-05-30 12:45:11.000000 rrelu-0.0.6/src/rrelu.egg-info/top_level.txt
+drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 13:10:46.283969 rrelu-0.0.7/
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     1079 2024-05-30 13:09:13.000000 rrelu-0.0.7/LICENSE.txt
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)        0 2024-05-30 13:09:13.000000 rrelu-0.0.7/MANIFEST.in
+-rw-r--r--   0 a4000     (1000) a4000     (1000)     3735 2024-05-30 13:10:46.283969 rrelu-0.0.7/PKG-INFO
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     3062 2024-05-30 13:09:13.000000 rrelu-0.0.7/README.md
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      554 2024-05-30 13:09:13.000000 rrelu-0.0.7/pyproject.toml
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      696 2024-05-30 13:10:46.283969 rrelu-0.0.7/setup.cfg
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      898 2024-05-30 13:09:13.000000 rrelu-0.0.7/setup.py
+drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 13:10:46.275969 rrelu-0.0.7/src/
+drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 13:10:46.275969 rrelu-0.0.7/src/rrelu/
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)        2 2024-05-30 13:09:13.000000 rrelu-0.0.7/src/rrelu/__init__.py
+drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 13:10:46.279969 rrelu-0.0.7/src/rrelu/models/
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      260 2024-05-30 13:09:13.000000 rrelu-0.0.7/src/rrelu/models/__init__.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     2881 2024-05-30 13:09:13.000000 rrelu-0.0.7/src/rrelu/models/alexnet.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     1232 2024-05-30 13:09:13.000000 rrelu-0.0.7/src/rrelu/models/alexnet_cifar100.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     2965 2024-05-30 13:09:13.000000 rrelu-0.0.7/src/rrelu/models/lenet.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     4839 2024-05-30 13:09:13.000000 rrelu-0.0.7/src/rrelu/models/resnet.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     4848 2024-05-30 13:09:13.000000 rrelu-0.0.7/src/rrelu/models/resnet_cifar100.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     2560 2024-05-30 13:09:13.000000 rrelu-0.0.7/src/rrelu/models/vgg.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     2580 2024-05-30 13:09:13.000000 rrelu-0.0.7/src/rrelu/models/vgg_cifar100.py
+drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 13:10:46.279969 rrelu-0.0.7/src/rrelu/pytorchfi/
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      170 2024-05-30 13:09:13.000000 rrelu-0.0.7/src/rrelu/pytorchfi/__init__.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)    21661 2024-05-30 13:09:13.000000 rrelu-0.0.7/src/rrelu/pytorchfi/core.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)    21717 2024-05-30 13:09:13.000000 rrelu-0.0.7/src/rrelu/pytorchfi/core_train.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)    10480 2024-05-30 13:09:13.000000 rrelu-0.0.7/src/rrelu/pytorchfi/neuron_error_models.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      115 2024-05-30 13:09:13.000000 rrelu-0.0.7/src/rrelu/pytorchfi/util.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)    22096 2024-05-30 13:09:13.000000 rrelu-0.0.7/src/rrelu/pytorchfi/weight_error_models.py
+drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 13:10:46.279969 rrelu-0.0.7/src/rrelu/relu_bound/
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      173 2024-05-30 13:09:13.000000 rrelu-0.0.7/src/rrelu/relu_bound/__init__.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      829 2024-05-30 13:09:13.000000 rrelu-0.0.7/src/rrelu/relu_bound/bound_fitact.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     1082 2024-05-30 13:09:13.000000 rrelu-0.0.7/src/rrelu/relu_bound/bound_proact.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)       95 2024-05-30 13:09:13.000000 rrelu-0.0.7/src/rrelu/relu_bound/bound_relu.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      761 2024-05-30 13:09:13.000000 rrelu-0.0.7/src/rrelu/relu_bound/bound_tresh.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      766 2024-05-30 13:09:13.000000 rrelu-0.0.7/src/rrelu/relu_bound/bound_zero.py
+drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 13:10:46.283969 rrelu-0.0.7/src/rrelu/search_bound/
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      161 2024-05-30 13:09:13.000000 rrelu-0.0.7/src/rrelu/search_bound/__init__.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)    10406 2024-05-30 13:09:13.000000 rrelu-0.0.7/src/rrelu/search_bound/fitact.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)    18023 2024-05-30 13:09:13.000000 rrelu-0.0.7/src/rrelu/search_bound/ftclip.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)    18108 2024-05-30 13:09:13.000000 rrelu-0.0.7/src/rrelu/search_bound/proact.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     1718 2024-05-30 13:09:13.000000 rrelu-0.0.7/src/rrelu/search_bound/ranger.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)    11543 2024-05-30 13:09:13.000000 rrelu-0.0.7/src/rrelu/setups.py
+drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 13:10:46.283969 rrelu-0.0.7/src/rrelu/utils/
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      172 2024-05-30 13:09:13.000000 rrelu-0.0.7/src/rrelu/utils/__init__.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     1659 2024-05-30 13:09:13.000000 rrelu-0.0.7/src/rrelu/utils/distributed.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     2811 2024-05-30 13:09:13.000000 rrelu-0.0.7/src/rrelu/utils/init.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     1094 2024-05-30 13:09:13.000000 rrelu-0.0.7/src/rrelu/utils/lr_scheduler.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     1218 2024-05-30 13:09:13.000000 rrelu-0.0.7/src/rrelu/utils/metric.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     3612 2024-05-30 13:09:13.000000 rrelu-0.0.7/src/rrelu/utils/misc.py
+drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 13:10:46.283969 rrelu-0.0.7/src/rrelu.egg-info/
+-rw-r--r--   0 a4000     (1000) a4000     (1000)     3735 2024-05-30 13:10:46.000000 rrelu-0.0.7/src/rrelu.egg-info/PKG-INFO
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     1234 2024-05-30 13:10:46.000000 rrelu-0.0.7/src/rrelu.egg-info/SOURCES.txt
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)        1 2024-05-30 13:10:46.000000 rrelu-0.0.7/src/rrelu.egg-info/dependency_links.txt
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)        6 2024-05-30 13:10:46.000000 rrelu-0.0.7/src/rrelu.egg-info/top_level.txt
```

### Comparing `rrelu-0.0.6/LICENSE.txt` & `rrelu-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.6/PKG-INFO` & `rrelu-0.0.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rrelu
-Version: 0.0.6
+Version: 0.0.7
 Summary: generate reliable relu activation function for DNNs
 Home-page: https://github.com/hamidmousavi0/reliable-relu-toolbox
 Author: Seyedhamidreza Mousavi
 Author-email: Seyedhamidreza Mousavi <seyedhamidreza.mousavi@mdu.se>
 Project-URL: Homepage, https://github.com/hamidmousavi0/reliable-relu-toolbox
 Project-URL: Issues, https://github.com/hamidmousavi0/reliable-relu-toolbox/issues
 Classifier: Programming Language :: Python :: 3
@@ -33,25 +33,24 @@
 
 * **ProAct** (the proposed algorithm) ([code](https://github.com/hamidmousavi0/reliable-relu-toolbox/blob/master/src/search_bound/proact.py)).
 * **FitAct** ([paper](https://arxiv.org/pdf/2112.13544) and [code](https://github.com/hamidmousavi0/reliable-relu-toolbox/blob/master/src/search_bound/fitact.py)).
 * **FtClipAct** ([paper](https://arxiv.org/pdf/1912.00941) and [code](https://github.com/hamidmousavi0/reliable-relu-toolbox/blob/master/src/search_bound/ftclip.py)).
 * **Ranger** ([paper](https://arxiv.org/pdf/2003.13874) and [code](https://github.com/hamidmousavi0/reliable-relu-toolbox/blob/master/src/search_bound/ranger.py)).
 
 ## Usage
-
-Download on PyPI [here](https://pypi.org/project/rrelu/).
+If you want to use the bounded relu functions and search algorithms you can 
+Download the rrelu on PyPI [here](https://pypi.org/project/rrelu/).
 
 ### Installing
 
 **From Pip**
 
 Install using `pip install rrelu`
 
 **From Source**
-
 Download this repository into your project folder.
 
 ### Importing
 
 Import the entire package:
 
 ```python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rrelu Version: 0.0.6 Summary: generate reliable
+Metadata-Version: 2.1 Name: rrelu Version: 0.0.7 Summary: generate reliable
 relu activation function for DNNs Home-page: https://github.com/hamidmousavi0/
 reliable-relu-toolbox Author: Seyedhamidreza Mousavi Author-email:
 Seyedhamidreza Mousavi
 mdu.se> Project-URL: Homepage, https://github.com/hamidmousavi0/reliable-relu-
 toolbox Project-URL: Issues, https://github.com/hamidmousavi0/reliable-relu-
 toolbox/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
@@ -28,20 +28,21 @@
 toolbox/blob/master/src/search_bound/proact.py)). * **FitAct** ([paper](https:/
 /arxiv.org/pdf/2112.13544) and [code](https://github.com/hamidmousavi0/
 reliable-relu-toolbox/blob/master/src/search_bound/fitact.py)). * **FtClipAct**
 ([paper](https://arxiv.org/pdf/1912.00941) and [code](https://github.com/
 hamidmousavi0/reliable-relu-toolbox/blob/master/src/search_bound/ftclip.py)). *
 **Ranger** ([paper](https://arxiv.org/pdf/2003.13874) and [code](https://
 github.com/hamidmousavi0/reliable-relu-toolbox/blob/master/src/search_bound/
-ranger.py)). ## Usage Download on PyPI [here](https://pypi.org/project/rrelu/).
-### Installing **From Pip** Install using `pip install rrelu` **From Source**
-Download this repository into your project folder. ### Importing Import the
-entire package: ```python import rrelu ``` Import a specific module: ```python
-from rrelu.search_bound import proact_bounds ``` ### Testing -- running and
-evaluating algorithms: ```python torchpack dist-run -np 1 python
+ranger.py)). ## Usage If you want to use the bounded relu functions and search
+algorithms you can Download the rrelu on PyPI [here](https://pypi.org/project/
+rrelu/). ### Installing **From Pip** Install using `pip install rrelu` **From
+Source** Download this repository into your project folder. ### Importing
+Import the entire package: ```python import rrelu ``` Import a specific module:
+```python from rrelu.search_bound import proact_bounds ``` ### Testing -
+- running and evaluating algorithms: ```python torchpack dist-run -np 1 python
 rrelu.search.py --dataset "dataset name (CIFAR10, CIFAR100)" --data_path "path
 to the dataset" --model "name of the model" --init_from "pretrained file path"
 \ --name_relu_bound "name of bounded relu" --name_serach_bound "name of the
 search algorithm" --bounds_type "type of thresholds" --bitflip "value
 representaiton" ``` ## Code ### Structure The main source code of framework is
 held in `src/rrelu`, which carries `search_bounds`, `relu_bounds` , `extended
 pytorchfi` and other implementations. ## Citation View the [published paper]().
```

### Comparing `rrelu-0.0.6/README.md` & `rrelu-0.0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -17,25 +17,24 @@
 
 * **ProAct** (the proposed algorithm) ([code](https://github.com/hamidmousavi0/reliable-relu-toolbox/blob/master/src/search_bound/proact.py)).
 * **FitAct** ([paper](https://arxiv.org/pdf/2112.13544) and [code](https://github.com/hamidmousavi0/reliable-relu-toolbox/blob/master/src/search_bound/fitact.py)).
 * **FtClipAct** ([paper](https://arxiv.org/pdf/1912.00941) and [code](https://github.com/hamidmousavi0/reliable-relu-toolbox/blob/master/src/search_bound/ftclip.py)).
 * **Ranger** ([paper](https://arxiv.org/pdf/2003.13874) and [code](https://github.com/hamidmousavi0/reliable-relu-toolbox/blob/master/src/search_bound/ranger.py)).
 
 ## Usage
-
-Download on PyPI [here](https://pypi.org/project/rrelu/).
+If you want to use the bounded relu functions and search algorithms you can 
+Download the rrelu on PyPI [here](https://pypi.org/project/rrelu/).
 
 ### Installing
 
 **From Pip**
 
 Install using `pip install rrelu`
 
 **From Source**
-
 Download this repository into your project folder.
 
 ### Importing
 
 Import the entire package:
 
 ```python
```

#### html2text {}

```diff
@@ -18,20 +18,21 @@
 toolbox/blob/master/src/search_bound/proact.py)). * **FitAct** ([paper](https:/
 /arxiv.org/pdf/2112.13544) and [code](https://github.com/hamidmousavi0/
 reliable-relu-toolbox/blob/master/src/search_bound/fitact.py)). * **FtClipAct**
 ([paper](https://arxiv.org/pdf/1912.00941) and [code](https://github.com/
 hamidmousavi0/reliable-relu-toolbox/blob/master/src/search_bound/ftclip.py)). *
 **Ranger** ([paper](https://arxiv.org/pdf/2003.13874) and [code](https://
 github.com/hamidmousavi0/reliable-relu-toolbox/blob/master/src/search_bound/
-ranger.py)). ## Usage Download on PyPI [here](https://pypi.org/project/rrelu/).
-### Installing **From Pip** Install using `pip install rrelu` **From Source**
-Download this repository into your project folder. ### Importing Import the
-entire package: ```python import rrelu ``` Import a specific module: ```python
-from rrelu.search_bound import proact_bounds ``` ### Testing -- running and
-evaluating algorithms: ```python torchpack dist-run -np 1 python
+ranger.py)). ## Usage If you want to use the bounded relu functions and search
+algorithms you can Download the rrelu on PyPI [here](https://pypi.org/project/
+rrelu/). ### Installing **From Pip** Install using `pip install rrelu` **From
+Source** Download this repository into your project folder. ### Importing
+Import the entire package: ```python import rrelu ``` Import a specific module:
+```python from rrelu.search_bound import proact_bounds ``` ### Testing -
+- running and evaluating algorithms: ```python torchpack dist-run -np 1 python
 rrelu.search.py --dataset "dataset name (CIFAR10, CIFAR100)" --data_path "path
 to the dataset" --model "name of the model" --init_from "pretrained file path"
 \ --name_relu_bound "name of bounded relu" --name_serach_bound "name of the
 search algorithm" --bounds_type "type of thresholds" --bitflip "value
 representaiton" ``` ## Code ### Structure The main source code of framework is
 held in `src/rrelu`, which carries `search_bounds`, `relu_bounds` , `extended
 pytorchfi` and other implementations. ## Citation View the [published paper]().
```

### Comparing `rrelu-0.0.6/pyproject.toml` & `rrelu-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "rrelu"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Seyedhamidreza Mousavi", email="seyedhamidreza.mousavi@mdu.se" },
 ]
 description = "generate reliable relu activation function for DNNs"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `rrelu-0.0.6/setup.cfg` & `rrelu-0.0.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rrelu
-version = 0.0.6
+version = 0.0.7
 author = Seyedhamidreza Mousavi
 author_email = seyedhamidreza.mousavi@mdu.se
 description = generate reliable relu activation function for DNNs
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/hamidmousavi0/reliable-relu-toolbox
 project_urls =
```

### Comparing `rrelu-0.0.6/setup.py` & `rrelu-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "rrelu",
-    version = "0.0.6",
+    version = "0.0.7",
     author = "Seyedhamidreza Mousavi",
     author_email = "seyedhamidreza.mousavi@mdu.se",
     description = "generate reliable relu activation function for DNNs",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/hamidmousavi0/reliable-relu-toolbox",
     project_urls = {
```

### Comparing `rrelu-0.0.6/src/rrelu/models/alexnet.py` & `rrelu-0.0.7/src/rrelu/models/alexnet.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.6/src/rrelu/models/alexnet_cifar100.py` & `rrelu-0.0.7/src/rrelu/models/alexnet_cifar100.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.6/src/rrelu/models/lenet.py` & `rrelu-0.0.7/src/rrelu/models/lenet.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.6/src/rrelu/models/resnet.py` & `rrelu-0.0.7/src/rrelu/models/resnet.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.6/src/rrelu/models/resnet_cifar100.py` & `rrelu-0.0.7/src/rrelu/models/resnet_cifar100.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.6/src/rrelu/models/vgg.py` & `rrelu-0.0.7/src/rrelu/models/vgg.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.6/src/rrelu/models/vgg_cifar100.py` & `rrelu-0.0.7/src/rrelu/models/vgg_cifar100.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.6/src/rrelu/pytorchfi/core.py` & `rrelu-0.0.7/src/rrelu/pytorchfi/core.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.6/src/rrelu/pytorchfi/core_train.py` & `rrelu-0.0.7/src/rrelu/pytorchfi/core_train.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.6/src/rrelu/pytorchfi/neuron_error_models.py` & `rrelu-0.0.7/src/rrelu/pytorchfi/neuron_error_models.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.6/src/rrelu/pytorchfi/weight_error_models.py` & `rrelu-0.0.7/src/rrelu/pytorchfi/weight_error_models.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.6/src/rrelu/relu_bound/bound_fitact.py` & `rrelu-0.0.7/src/rrelu/relu_bound/bound_fitact.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.6/src/rrelu/relu_bound/bound_proact.py` & `rrelu-0.0.7/src/rrelu/relu_bound/bound_proact.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.6/src/rrelu/relu_bound/bound_tresh.py` & `rrelu-0.0.7/src/rrelu/relu_bound/bound_tresh.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.6/src/rrelu/relu_bound/bound_zero.py` & `rrelu-0.0.7/src/rrelu/relu_bound/bound_zero.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.6/src/rrelu/search_bound/fitact.py` & `rrelu-0.0.7/src/rrelu/search_bound/fitact.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import sys
 import torch.nn as nn
 import torch
 import copy
 import numpy as np
 import warnings
 import sys; 
-import setup 
 from rrelu.relu_bound.bound_fitact import bounded_relu_fitact
 import os
 import argparse
 from rrelu.utils.metric import accuracy,AverageMeter
 from rrelu.utils.lr_scheduler import CosineLRwithWarmup
 from rrelu.utils.distributed import DistributedMetric
 from rrelu.search_bound.ranger import Ranger_bounds
```

### Comparing `rrelu-0.0.6/src/rrelu/search_bound/ftclip.py` & `rrelu-0.0.7/src/rrelu/search_bound/ftclip.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import sys
 import torch
 import numpy as np
 import torch
 import copy
 import torch.nn as nn 
-import setup 
 from rrelu.pytorchfi.core import FaultInjection
 from rrelu.utils.distributed import DistributedMetric
 from tqdm import tqdm
 from torchpack import distributed as dist
 from rrelu.utils import load_state_dict_from_file
 from rrelu.utils.metric import accuracy
 from rrelu.pytorchfi.weight_error_models import bit_flip_weight_IEEE,bit_flip_weight_fixed,bit_flip_weight_int
```

### Comparing `rrelu-0.0.6/src/rrelu/search_bound/proact.py` & `rrelu-0.0.7/src/rrelu/search_bound/proact.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import sys
 import torch.nn as nn
 import torch
 import copy
 import numpy as np
 import warnings
 import sys;
-import setup 
 from rrelu.relu_bound.bound_proact import bounded_hyrelu_proact
 from rrelu.relu_bound.bound_zero import bounded_relu_zero
 import os
 import argparse
 from typing import Dict, Optional
 from rrelu.relu_bound.bound_relu import Relu_bound
 from rrelu.pytorchfi.weight_error_models import multi_weight_inj_float,multi_weight_inj_fixed,multi_weight_inj_int
```

### Comparing `rrelu-0.0.6/src/rrelu/search_bound/ranger.py` & `rrelu-0.0.7/src/rrelu/search_bound/ranger.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.6/src/rrelu/setup.py` & `rrelu-0.0.7/src/rrelu/setups.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.6/src/rrelu/utils/distributed.py` & `rrelu-0.0.7/src/rrelu/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.6/src/rrelu/utils/init.py` & `rrelu-0.0.7/src/rrelu/utils/init.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.6/src/rrelu/utils/lr_scheduler.py` & `rrelu-0.0.7/src/rrelu/utils/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.6/src/rrelu/utils/metric.py` & `rrelu-0.0.7/src/rrelu/utils/metric.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.6/src/rrelu/utils/misc.py` & `rrelu-0.0.7/src/rrelu/utils/misc.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.6/src/rrelu.egg-info/PKG-INFO` & `rrelu-0.0.7/src/rrelu.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rrelu
-Version: 0.0.6
+Version: 0.0.7
 Summary: generate reliable relu activation function for DNNs
 Home-page: https://github.com/hamidmousavi0/reliable-relu-toolbox
 Author: Seyedhamidreza Mousavi
 Author-email: Seyedhamidreza Mousavi <seyedhamidreza.mousavi@mdu.se>
 Project-URL: Homepage, https://github.com/hamidmousavi0/reliable-relu-toolbox
 Project-URL: Issues, https://github.com/hamidmousavi0/reliable-relu-toolbox/issues
 Classifier: Programming Language :: Python :: 3
@@ -33,25 +33,24 @@
 
 * **ProAct** (the proposed algorithm) ([code](https://github.com/hamidmousavi0/reliable-relu-toolbox/blob/master/src/search_bound/proact.py)).
 * **FitAct** ([paper](https://arxiv.org/pdf/2112.13544) and [code](https://github.com/hamidmousavi0/reliable-relu-toolbox/blob/master/src/search_bound/fitact.py)).
 * **FtClipAct** ([paper](https://arxiv.org/pdf/1912.00941) and [code](https://github.com/hamidmousavi0/reliable-relu-toolbox/blob/master/src/search_bound/ftclip.py)).
 * **Ranger** ([paper](https://arxiv.org/pdf/2003.13874) and [code](https://github.com/hamidmousavi0/reliable-relu-toolbox/blob/master/src/search_bound/ranger.py)).
 
 ## Usage
-
-Download on PyPI [here](https://pypi.org/project/rrelu/).
+If you want to use the bounded relu functions and search algorithms you can 
+Download the rrelu on PyPI [here](https://pypi.org/project/rrelu/).
 
 ### Installing
 
 **From Pip**
 
 Install using `pip install rrelu`
 
 **From Source**
-
 Download this repository into your project folder.
 
 ### Importing
 
 Import the entire package:
 
 ```python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rrelu Version: 0.0.6 Summary: generate reliable
+Metadata-Version: 2.1 Name: rrelu Version: 0.0.7 Summary: generate reliable
 relu activation function for DNNs Home-page: https://github.com/hamidmousavi0/
 reliable-relu-toolbox Author: Seyedhamidreza Mousavi Author-email:
 Seyedhamidreza Mousavi
 mdu.se> Project-URL: Homepage, https://github.com/hamidmousavi0/reliable-relu-
 toolbox Project-URL: Issues, https://github.com/hamidmousavi0/reliable-relu-
 toolbox/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
@@ -28,20 +28,21 @@
 toolbox/blob/master/src/search_bound/proact.py)). * **FitAct** ([paper](https:/
 /arxiv.org/pdf/2112.13544) and [code](https://github.com/hamidmousavi0/
 reliable-relu-toolbox/blob/master/src/search_bound/fitact.py)). * **FtClipAct**
 ([paper](https://arxiv.org/pdf/1912.00941) and [code](https://github.com/
 hamidmousavi0/reliable-relu-toolbox/blob/master/src/search_bound/ftclip.py)). *
 **Ranger** ([paper](https://arxiv.org/pdf/2003.13874) and [code](https://
 github.com/hamidmousavi0/reliable-relu-toolbox/blob/master/src/search_bound/
-ranger.py)). ## Usage Download on PyPI [here](https://pypi.org/project/rrelu/).
-### Installing **From Pip** Install using `pip install rrelu` **From Source**
-Download this repository into your project folder. ### Importing Import the
-entire package: ```python import rrelu ``` Import a specific module: ```python
-from rrelu.search_bound import proact_bounds ``` ### Testing -- running and
-evaluating algorithms: ```python torchpack dist-run -np 1 python
+ranger.py)). ## Usage If you want to use the bounded relu functions and search
+algorithms you can Download the rrelu on PyPI [here](https://pypi.org/project/
+rrelu/). ### Installing **From Pip** Install using `pip install rrelu` **From
+Source** Download this repository into your project folder. ### Importing
+Import the entire package: ```python import rrelu ``` Import a specific module:
+```python from rrelu.search_bound import proact_bounds ``` ### Testing -
+- running and evaluating algorithms: ```python torchpack dist-run -np 1 python
 rrelu.search.py --dataset "dataset name (CIFAR10, CIFAR100)" --data_path "path
 to the dataset" --model "name of the model" --init_from "pretrained file path"
 \ --name_relu_bound "name of bounded relu" --name_serach_bound "name of the
 search algorithm" --bounds_type "type of thresholds" --bitflip "value
 representaiton" ``` ## Code ### Structure The main source code of framework is
 held in `src/rrelu`, which carries `search_bounds`, `relu_bounds` , `extended
 pytorchfi` and other implementations. ## Citation View the [published paper]().
```

### Comparing `rrelu-0.0.6/src/rrelu.egg-info/SOURCES.txt` & `rrelu-0.0.7/src/rrelu.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 src/rrelu/__init__.py
-src/rrelu/eval.py
-src/rrelu/search.py
-src/rrelu/setup.py
-src/rrelu/train.py
+src/rrelu/setups.py
 src/rrelu.egg-info/PKG-INFO
 src/rrelu.egg-info/SOURCES.txt
 src/rrelu.egg-info/dependency_links.txt
 src/rrelu.egg-info/top_level.txt
 src/rrelu/models/__init__.py
 src/rrelu/models/alexnet.py
 src/rrelu/models/alexnet_cifar100.py
```

