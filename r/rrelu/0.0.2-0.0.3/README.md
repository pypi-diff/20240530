# Comparing `tmp/rrelu-0.0.2.tar.gz` & `tmp/rrelu-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rrelu-0.0.2.tar", last modified: Thu May 30 10:46:02 2024, max compression
+gzip compressed data, was "rrelu-0.0.3.tar", last modified: Thu May 30 10:54:16 2024, max compression
```

## Comparing `rrelu-0.0.2.tar` & `rrelu-0.0.3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 10:46:02.452742 rrelu-0.0.2/
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     1079 2024-05-30 10:41:58.000000 rrelu-0.0.2/LICENSE.txt
--rw-rw-r--   0 a4000     (1000) a4000     (1000)        0 2024-05-30 10:41:58.000000 rrelu-0.0.2/MANIFEST.in
--rw-r--r--   0 a4000     (1000) a4000     (1000)     3619 2024-05-30 10:46:02.452742 rrelu-0.0.2/PKG-INFO
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     2946 2024-05-30 10:41:58.000000 rrelu-0.0.2/README.md
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      554 2024-05-30 10:45:47.000000 rrelu-0.0.2/pyproject.toml
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      696 2024-05-30 10:46:02.456742 rrelu-0.0.2/setup.cfg
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      898 2024-05-30 10:45:23.000000 rrelu-0.0.2/setup.py
-drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 10:46:02.444742 rrelu-0.0.2/src/
-drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 10:46:02.448742 rrelu-0.0.2/src/rrelu/
--rw-rw-r--   0 a4000     (1000) a4000     (1000)        0 2024-05-30 10:41:58.000000 rrelu-0.0.2/src/rrelu/__init__.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     3528 2024-05-30 10:41:58.000000 rrelu-0.0.2/src/rrelu/eval.py
-drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 10:46:02.448742 rrelu-0.0.2/src/rrelu/models/
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      175 2024-05-30 10:41:58.000000 rrelu-0.0.2/src/rrelu/models/__init__.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     2875 2024-05-30 10:41:58.000000 rrelu-0.0.2/src/rrelu/models/alexnet.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     1232 2024-05-30 10:41:58.000000 rrelu-0.0.2/src/rrelu/models/alexnet_cifar100.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     2965 2024-05-30 10:41:58.000000 rrelu-0.0.2/src/rrelu/models/lenet.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     4839 2024-05-30 10:41:58.000000 rrelu-0.0.2/src/rrelu/models/resnet.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     4848 2024-05-30 10:41:58.000000 rrelu-0.0.2/src/rrelu/models/resnet_cifar100.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     2560 2024-05-30 10:41:58.000000 rrelu-0.0.2/src/rrelu/models/vgg.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     2580 2024-05-30 10:41:58.000000 rrelu-0.0.2/src/rrelu/models/vgg_cifar100.py
-drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 10:46:02.448742 rrelu-0.0.2/src/rrelu/pytorchfi/
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      109 2024-05-30 10:41:58.000000 rrelu-0.0.2/src/rrelu/pytorchfi/__init__.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)    21655 2024-05-30 10:41:58.000000 rrelu-0.0.2/src/rrelu/pytorchfi/core.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)    21711 2024-05-30 10:41:58.000000 rrelu-0.0.2/src/rrelu/pytorchfi/core_train.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)    10468 2024-05-30 10:41:58.000000 rrelu-0.0.2/src/rrelu/pytorchfi/neuron_error_models.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      115 2024-05-30 10:41:58.000000 rrelu-0.0.2/src/rrelu/pytorchfi/util.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)    22084 2024-05-30 10:41:58.000000 rrelu-0.0.2/src/rrelu/pytorchfi/weight_error_models.py
-drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 10:46:02.452742 rrelu-0.0.2/src/rrelu/relu_bound/
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      108 2024-05-30 10:41:58.000000 rrelu-0.0.2/src/rrelu/relu_bound/__init__.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      823 2024-05-30 10:41:58.000000 rrelu-0.0.2/src/rrelu/relu_bound/bound_fitact.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     1076 2024-05-30 10:41:58.000000 rrelu-0.0.2/src/rrelu/relu_bound/bound_proact.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)       95 2024-05-30 10:41:58.000000 rrelu-0.0.2/src/rrelu/relu_bound/bound_relu.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      754 2024-05-30 10:41:58.000000 rrelu-0.0.2/src/rrelu/relu_bound/bound_tresh.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      759 2024-05-30 10:41:58.000000 rrelu-0.0.2/src/rrelu/relu_bound/bound_zero.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     5052 2024-05-30 10:41:58.000000 rrelu-0.0.2/src/rrelu/search.py
-drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 10:46:02.452742 rrelu-0.0.2/src/rrelu/search_bound/
--rw-rw-r--   0 a4000     (1000) a4000     (1000)       88 2024-05-30 10:41:58.000000 rrelu-0.0.2/src/rrelu/search_bound/__init__.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)    10390 2024-05-30 10:41:58.000000 rrelu-0.0.2/src/rrelu/search_bound/fitact.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)    17994 2024-05-30 10:41:58.000000 rrelu-0.0.2/src/rrelu/search_bound/ftclip.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)    18074 2024-05-30 10:41:58.000000 rrelu-0.0.2/src/rrelu/search_bound/proact.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     1718 2024-05-30 10:41:58.000000 rrelu-0.0.2/src/rrelu/search_bound/ranger.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)    11519 2024-05-30 10:41:58.000000 rrelu-0.0.2/src/rrelu/setup.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)    13425 2024-05-30 10:41:58.000000 rrelu-0.0.2/src/rrelu/train.py
-drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 10:46:02.452742 rrelu-0.0.2/src/rrelu/utils/
--rw-rw-r--   0 a4000     (1000) a4000     (1000)      116 2024-05-30 10:41:58.000000 rrelu-0.0.2/src/rrelu/utils/__init__.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     1659 2024-05-30 10:41:58.000000 rrelu-0.0.2/src/rrelu/utils/distributed.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     2811 2024-05-30 10:41:58.000000 rrelu-0.0.2/src/rrelu/utils/init.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     1094 2024-05-30 10:41:58.000000 rrelu-0.0.2/src/rrelu/utils/lr_scheduler.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     1218 2024-05-30 10:41:58.000000 rrelu-0.0.2/src/rrelu/utils/metric.py
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     3612 2024-05-30 10:41:58.000000 rrelu-0.0.2/src/rrelu/utils/misc.py
-drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 10:46:02.452742 rrelu-0.0.2/src/rrelu.egg-info/
--rw-r--r--   0 a4000     (1000) a4000     (1000)     3619 2024-05-30 10:46:02.000000 rrelu-0.0.2/src/rrelu.egg-info/PKG-INFO
--rw-rw-r--   0 a4000     (1000) a4000     (1000)     1290 2024-05-30 10:46:02.000000 rrelu-0.0.2/src/rrelu.egg-info/SOURCES.txt
--rw-rw-r--   0 a4000     (1000) a4000     (1000)        1 2024-05-30 10:46:02.000000 rrelu-0.0.2/src/rrelu.egg-info/dependency_links.txt
--rw-rw-r--   0 a4000     (1000) a4000     (1000)        6 2024-05-30 10:46:02.000000 rrelu-0.0.2/src/rrelu.egg-info/top_level.txt
+drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 10:54:16.708464 rrelu-0.0.3/
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     1079 2024-05-30 10:41:58.000000 rrelu-0.0.3/LICENSE.txt
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)        0 2024-05-30 10:41:58.000000 rrelu-0.0.3/MANIFEST.in
+-rw-r--r--   0 a4000     (1000) a4000     (1000)     3619 2024-05-30 10:54:16.708464 rrelu-0.0.3/PKG-INFO
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     2946 2024-05-30 10:41:58.000000 rrelu-0.0.3/README.md
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      554 2024-05-30 10:53:37.000000 rrelu-0.0.3/pyproject.toml
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      696 2024-05-30 10:54:16.708464 rrelu-0.0.3/setup.cfg
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      898 2024-05-30 10:53:26.000000 rrelu-0.0.3/setup.py
+drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 10:54:16.700464 rrelu-0.0.3/src/
+drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 10:54:16.700464 rrelu-0.0.3/src/rrelu/
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)       85 2024-05-30 10:52:22.000000 rrelu-0.0.3/src/rrelu/__init__.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     3528 2024-05-30 10:41:58.000000 rrelu-0.0.3/src/rrelu/eval.py
+drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 10:54:16.704464 rrelu-0.0.3/src/rrelu/models/
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      175 2024-05-30 10:41:58.000000 rrelu-0.0.3/src/rrelu/models/__init__.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     2875 2024-05-30 10:41:58.000000 rrelu-0.0.3/src/rrelu/models/alexnet.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     1232 2024-05-30 10:41:58.000000 rrelu-0.0.3/src/rrelu/models/alexnet_cifar100.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     2965 2024-05-30 10:41:58.000000 rrelu-0.0.3/src/rrelu/models/lenet.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     4839 2024-05-30 10:41:58.000000 rrelu-0.0.3/src/rrelu/models/resnet.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     4848 2024-05-30 10:41:58.000000 rrelu-0.0.3/src/rrelu/models/resnet_cifar100.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     2560 2024-05-30 10:41:58.000000 rrelu-0.0.3/src/rrelu/models/vgg.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     2580 2024-05-30 10:41:58.000000 rrelu-0.0.3/src/rrelu/models/vgg_cifar100.py
+drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 10:54:16.704464 rrelu-0.0.3/src/rrelu/pytorchfi/
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      109 2024-05-30 10:41:58.000000 rrelu-0.0.3/src/rrelu/pytorchfi/__init__.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)    21655 2024-05-30 10:41:58.000000 rrelu-0.0.3/src/rrelu/pytorchfi/core.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)    21711 2024-05-30 10:41:58.000000 rrelu-0.0.3/src/rrelu/pytorchfi/core_train.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)    10468 2024-05-30 10:41:58.000000 rrelu-0.0.3/src/rrelu/pytorchfi/neuron_error_models.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      115 2024-05-30 10:41:58.000000 rrelu-0.0.3/src/rrelu/pytorchfi/util.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)    22084 2024-05-30 10:41:58.000000 rrelu-0.0.3/src/rrelu/pytorchfi/weight_error_models.py
+drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 10:54:16.704464 rrelu-0.0.3/src/rrelu/relu_bound/
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      108 2024-05-30 10:41:58.000000 rrelu-0.0.3/src/rrelu/relu_bound/__init__.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      823 2024-05-30 10:41:58.000000 rrelu-0.0.3/src/rrelu/relu_bound/bound_fitact.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     1076 2024-05-30 10:41:58.000000 rrelu-0.0.3/src/rrelu/relu_bound/bound_proact.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)       95 2024-05-30 10:41:58.000000 rrelu-0.0.3/src/rrelu/relu_bound/bound_relu.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      754 2024-05-30 10:41:58.000000 rrelu-0.0.3/src/rrelu/relu_bound/bound_tresh.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      759 2024-05-30 10:41:58.000000 rrelu-0.0.3/src/rrelu/relu_bound/bound_zero.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     5052 2024-05-30 10:41:58.000000 rrelu-0.0.3/src/rrelu/search.py
+drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 10:54:16.708464 rrelu-0.0.3/src/rrelu/search_bound/
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)       88 2024-05-30 10:41:58.000000 rrelu-0.0.3/src/rrelu/search_bound/__init__.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)    10390 2024-05-30 10:41:58.000000 rrelu-0.0.3/src/rrelu/search_bound/fitact.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)    17994 2024-05-30 10:41:58.000000 rrelu-0.0.3/src/rrelu/search_bound/ftclip.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)    18074 2024-05-30 10:41:58.000000 rrelu-0.0.3/src/rrelu/search_bound/proact.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     1718 2024-05-30 10:41:58.000000 rrelu-0.0.3/src/rrelu/search_bound/ranger.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)    11519 2024-05-30 10:41:58.000000 rrelu-0.0.3/src/rrelu/setup.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)    13425 2024-05-30 10:41:58.000000 rrelu-0.0.3/src/rrelu/train.py
+drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 10:54:16.708464 rrelu-0.0.3/src/rrelu/utils/
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)      116 2024-05-30 10:41:58.000000 rrelu-0.0.3/src/rrelu/utils/__init__.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     1659 2024-05-30 10:41:58.000000 rrelu-0.0.3/src/rrelu/utils/distributed.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     2811 2024-05-30 10:41:58.000000 rrelu-0.0.3/src/rrelu/utils/init.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     1094 2024-05-30 10:41:58.000000 rrelu-0.0.3/src/rrelu/utils/lr_scheduler.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     1218 2024-05-30 10:41:58.000000 rrelu-0.0.3/src/rrelu/utils/metric.py
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     3612 2024-05-30 10:41:58.000000 rrelu-0.0.3/src/rrelu/utils/misc.py
+drwxrwxr-x   0 a4000     (1000) a4000     (1000)        0 2024-05-30 10:54:16.708464 rrelu-0.0.3/src/rrelu.egg-info/
+-rw-r--r--   0 a4000     (1000) a4000     (1000)     3619 2024-05-30 10:54:16.000000 rrelu-0.0.3/src/rrelu.egg-info/PKG-INFO
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)     1290 2024-05-30 10:54:16.000000 rrelu-0.0.3/src/rrelu.egg-info/SOURCES.txt
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)        1 2024-05-30 10:54:16.000000 rrelu-0.0.3/src/rrelu.egg-info/dependency_links.txt
+-rw-rw-r--   0 a4000     (1000) a4000     (1000)        6 2024-05-30 10:54:16.000000 rrelu-0.0.3/src/rrelu.egg-info/top_level.txt
```

### Comparing `rrelu-0.0.2/LICENSE.txt` & `rrelu-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.2/PKG-INFO` & `rrelu-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rrelu
-Version: 0.0.2
+Version: 0.0.3
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
-Metadata-Version: 2.1 Name: rrelu Version: 0.0.2 Summary: generate reliable
+Metadata-Version: 2.1 Name: rrelu Version: 0.0.3 Summary: generate reliable
 relu activation function for DNNs Home-page: https://github.com/hamidmousavi0/
 reliable-relu-toolbox Author: Seyedhamidreza Mousavi Author-email:
 Seyedhamidreza Mousavi
 mdu.se> Project-URL: Homepage, https://github.com/hamidmousavi0/reliable-relu-
 toolbox Project-URL: Issues, https://github.com/hamidmousavi0/reliable-relu-
 toolbox/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
```

### Comparing `rrelu-0.0.2/README.md` & `rrelu-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.2/pyproject.toml` & `rrelu-0.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "rrelu"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Seyedhamidreza Mousavi", email="seyedhamidreza.mousavi@mdu.se" },
 ]
 description = "generate reliable relu activation function for DNNs"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `rrelu-0.0.2/setup.cfg` & `rrelu-0.0.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rrelu
-version = 0.0.2
+version = 0.0.3
 author = Seyedhamidreza Mousavi
 author_email = seyedhamidreza.mousavi@mdu.se
 description = generate reliable relu activation function for DNNs
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/hamidmousavi0/reliable-relu-toolbox
 project_urls =
```

### Comparing `rrelu-0.0.2/setup.py` & `rrelu-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "rrelu",
-    version = "0.0.2",
+    version = "0.0.3",
     author = "Seyedhamidreza Mousavi",
     author_email = "seyedhamidreza.mousavi@mdu.se",
     description = "generate reliable relu activation function for DNNs",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/hamidmousavi0/reliable-relu-toolbox",
     project_urls = {
```

### Comparing `rrelu-0.0.2/src/rrelu/eval.py` & `rrelu-0.0.3/src/rrelu/eval.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.2/src/rrelu/models/alexnet.py` & `rrelu-0.0.3/src/rrelu/models/alexnet.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.2/src/rrelu/models/alexnet_cifar100.py` & `rrelu-0.0.3/src/rrelu/models/alexnet_cifar100.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.2/src/rrelu/models/lenet.py` & `rrelu-0.0.3/src/rrelu/models/lenet.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.2/src/rrelu/models/resnet.py` & `rrelu-0.0.3/src/rrelu/models/resnet.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.2/src/rrelu/models/resnet_cifar100.py` & `rrelu-0.0.3/src/rrelu/models/resnet_cifar100.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.2/src/rrelu/models/vgg.py` & `rrelu-0.0.3/src/rrelu/models/vgg.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.2/src/rrelu/models/vgg_cifar100.py` & `rrelu-0.0.3/src/rrelu/models/vgg_cifar100.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.2/src/rrelu/pytorchfi/core.py` & `rrelu-0.0.3/src/rrelu/pytorchfi/core.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.2/src/rrelu/pytorchfi/core_train.py` & `rrelu-0.0.3/src/rrelu/pytorchfi/core_train.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.2/src/rrelu/pytorchfi/neuron_error_models.py` & `rrelu-0.0.3/src/rrelu/pytorchfi/neuron_error_models.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.2/src/rrelu/pytorchfi/weight_error_models.py` & `rrelu-0.0.3/src/rrelu/pytorchfi/weight_error_models.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.2/src/rrelu/relu_bound/bound_fitact.py` & `rrelu-0.0.3/src/rrelu/relu_bound/bound_fitact.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.2/src/rrelu/relu_bound/bound_proact.py` & `rrelu-0.0.3/src/rrelu/relu_bound/bound_proact.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.2/src/rrelu/relu_bound/bound_tresh.py` & `rrelu-0.0.3/src/rrelu/relu_bound/bound_tresh.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.2/src/rrelu/relu_bound/bound_zero.py` & `rrelu-0.0.3/src/rrelu/relu_bound/bound_zero.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.2/src/rrelu/search.py` & `rrelu-0.0.3/src/rrelu/search.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.2/src/rrelu/search_bound/fitact.py` & `rrelu-0.0.3/src/rrelu/search_bound/fitact.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.2/src/rrelu/search_bound/ftclip.py` & `rrelu-0.0.3/src/rrelu/search_bound/ftclip.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.2/src/rrelu/search_bound/proact.py` & `rrelu-0.0.3/src/rrelu/search_bound/proact.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.2/src/rrelu/search_bound/ranger.py` & `rrelu-0.0.3/src/rrelu/search_bound/ranger.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.2/src/rrelu/setup.py` & `rrelu-0.0.3/src/rrelu/setup.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.2/src/rrelu/train.py` & `rrelu-0.0.3/src/rrelu/train.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.2/src/rrelu/utils/distributed.py` & `rrelu-0.0.3/src/rrelu/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.2/src/rrelu/utils/init.py` & `rrelu-0.0.3/src/rrelu/utils/init.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.2/src/rrelu/utils/lr_scheduler.py` & `rrelu-0.0.3/src/rrelu/utils/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.2/src/rrelu/utils/metric.py` & `rrelu-0.0.3/src/rrelu/utils/metric.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.2/src/rrelu/utils/misc.py` & `rrelu-0.0.3/src/rrelu/utils/misc.py`

 * *Files identical despite different names*

### Comparing `rrelu-0.0.2/src/rrelu.egg-info/PKG-INFO` & `rrelu-0.0.3/src/rrelu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rrelu
-Version: 0.0.2
+Version: 0.0.3
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
-Metadata-Version: 2.1 Name: rrelu Version: 0.0.2 Summary: generate reliable
+Metadata-Version: 2.1 Name: rrelu Version: 0.0.3 Summary: generate reliable
 relu activation function for DNNs Home-page: https://github.com/hamidmousavi0/
 reliable-relu-toolbox Author: Seyedhamidreza Mousavi Author-email:
 Seyedhamidreza Mousavi
 mdu.se> Project-URL: Homepage, https://github.com/hamidmousavi0/reliable-relu-
 toolbox Project-URL: Issues, https://github.com/hamidmousavi0/reliable-relu-
 toolbox/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
```

### Comparing `rrelu-0.0.2/src/rrelu.egg-info/SOURCES.txt` & `rrelu-0.0.3/src/rrelu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

