# Comparing `tmp/mb_pytorch-1.0.54.tar.gz` & `tmp/mb_pytorch-1.0.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mb_pytorch-1.0.54.tar", last modified: Tue May 28 03:59:33 2024, max compression
+gzip compressed data, was "mb_pytorch-1.0.55.tar", last modified: Thu May 30 04:54:03 2024, max compression
```

## Comparing `mb_pytorch-1.0.54.tar` & `mb_pytorch-1.0.55.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-28 03:59:33.696313 mb_pytorch-1.0.54/
--rw-r--r--   0 malav     (1000) malav     (1000)      206 2024-05-28 03:59:33.696313 mb_pytorch-1.0.54/PKG-INFO
--rw-rw-r--   0 malav     (1000) malav     (1000)      742 2024-05-06 17:42:04.000000 mb_pytorch-1.0.54/README.md
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-28 03:59:33.692314 mb_pytorch-1.0.54/mb_pytorch/
--rw-rw-r--   0 malav     (1000) malav     (1000)       97 2024-05-06 17:42:04.000000 mb_pytorch-1.0.54/mb_pytorch/__init__.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-28 03:59:33.692314 mb_pytorch-1.0.54/mb_pytorch/classification/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-15 16:38:04.000000 mb_pytorch-1.0.54/mb_pytorch/classification/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     7166 2024-05-06 17:42:04.000000 mb_pytorch-1.0.54/mb_pytorch/classification/training.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-28 03:59:33.692314 mb_pytorch-1.0.54/mb_pytorch/dataloader/
--rw-rw-r--   0 malav     (1000) malav     (1000)       44 2024-05-28 02:55:26.000000 mb_pytorch-1.0.54/mb_pytorch/dataloader/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)    16093 2024-05-28 03:59:17.000000 mb_pytorch-1.0.54/mb_pytorch/dataloader/loader.py
--rw-rw-r--   0 malav     (1000) malav     (1000)    19206 2024-05-27 21:31:06.000000 mb_pytorch-1.0.54/mb_pytorch/dataloader/loader_old.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-28 03:59:33.692314 mb_pytorch-1.0.54/mb_pytorch/detection/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-15 16:38:14.000000 mb_pytorch-1.0.54/mb_pytorch/detection/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     6567 2024-05-27 20:31:19.000000 mb_pytorch-1.0.54/mb_pytorch/detection/training.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-28 03:59:33.692314 mb_pytorch-1.0.54/mb_pytorch/metalearning/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.54/mb_pytorch/metalearning/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1385 2024-05-06 17:42:04.000000 mb_pytorch-1.0.54/mb_pytorch/metalearning/meta_utils.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1030 2024-05-28 02:54:17.000000 mb_pytorch-1.0.54/mb_pytorch/metalearning/proto_dataloader.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     2861 2024-05-06 17:42:04.000000 mb_pytorch-1.0.54/mb_pytorch/metalearning/prototypical.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-28 03:59:33.692314 mb_pytorch-1.0.54/mb_pytorch/models/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.54/mb_pytorch/models/__init__.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-28 03:59:33.692314 mb_pytorch-1.0.54/mb_pytorch/models/blocks/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.54/mb_pytorch/models/blocks/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     2801 2024-05-06 17:42:04.000000 mb_pytorch-1.0.54/mb_pytorch/models/blocks/attention_block.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     3629 2024-05-06 17:42:04.000000 mb_pytorch-1.0.54/mb_pytorch/models/blocks/cnn.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     4783 2024-05-06 17:42:04.000000 mb_pytorch-1.0.54/mb_pytorch/models/blocks/conv_block.py
--rw-rw-r--   0 malav     (1000) malav     (1000)      920 2024-05-06 17:42:04.000000 mb_pytorch-1.0.54/mb_pytorch/models/blocks/conv_with_relu.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     2256 2024-05-06 17:42:04.000000 mb_pytorch-1.0.54/mb_pytorch/models/blocks/model_out.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1184 2024-05-06 17:42:04.000000 mb_pytorch-1.0.54/mb_pytorch/models/blocks/rnn.py
--rw-rw-r--   0 malav     (1000) malav     (1000)    21087 2024-05-06 17:42:04.000000 mb_pytorch-1.0.54/mb_pytorch/models/extra_models.py
--rw-rw-r--   0 malav     (1000) malav     (1000)      920 2024-05-06 17:42:04.000000 mb_pytorch-1.0.54/mb_pytorch/models/lenet.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     3921 2024-05-17 14:58:48.000000 mb_pytorch-1.0.54/mb_pytorch/models/modelloader.py
--rw-rw-r--   0 malav     (1000) malav     (1000)    10784 2024-05-06 17:42:04.000000 mb_pytorch-1.0.54/mb_pytorch/models/unet_models.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-28 03:59:33.692314 mb_pytorch-1.0.54/mb_pytorch/segmentation/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-15 16:59:50.000000 mb_pytorch-1.0.54/mb_pytorch/segmentation/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     4800 2024-05-28 02:54:27.000000 mb_pytorch-1.0.54/mb_pytorch/segmentation/training.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-28 03:59:33.692314 mb_pytorch-1.0.54/mb_pytorch/training/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-15 16:59:41.000000 mb_pytorch-1.0.54/mb_pytorch/training/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1630 2024-05-06 17:42:04.000000 mb_pytorch-1.0.54/mb_pytorch/training/accelerate_train.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1454 2024-05-28 02:54:35.000000 mb_pytorch-1.0.54/mb_pytorch/training/train_params.py
--rw-rw-r--   0 malav     (1000) malav     (1000)      144 2024-05-06 17:42:04.000000 mb_pytorch-1.0.54/mb_pytorch/training/training.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-28 03:59:33.696313 mb_pytorch-1.0.54/mb_pytorch/utils/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.54/mb_pytorch/utils/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1055 2024-05-06 17:42:04.000000 mb_pytorch-1.0.54/mb_pytorch/utils/compiler.py
--rw-rw-r--   0 malav     (1000) malav     (1000)      257 2024-05-06 17:42:04.000000 mb_pytorch-1.0.54/mb_pytorch/utils/dist.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     3391 2024-05-06 17:42:04.000000 mb_pytorch-1.0.54/mb_pytorch/utils/extra_utils.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     7085 2024-05-28 02:55:11.000000 mb_pytorch-1.0.54/mb_pytorch/utils/generate_emb.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     2582 2024-05-06 17:42:04.000000 mb_pytorch-1.0.54/mb_pytorch/utils/losses.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1199 2024-05-06 17:42:04.000000 mb_pytorch-1.0.54/mb_pytorch/utils/metrics.py
--rw-rw-r--   0 malav     (1000) malav     (1000)      207 2024-05-28 03:59:25.000000 mb_pytorch-1.0.54/mb_pytorch/utils/version.py
--rw-rw-r--   0 malav     (1000) malav     (1000)    10620 2024-05-23 19:25:11.000000 mb_pytorch-1.0.54/mb_pytorch/utils/viewer.py
--rw-rw-r--   0 malav     (1000) malav     (1000)      994 2024-05-06 17:42:04.000000 mb_pytorch-1.0.54/mb_pytorch/utils/yaml_reader.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-28 03:59:33.696313 mb_pytorch-1.0.54/mb_pytorch.egg-info/
--rw-r--r--   0 malav     (1000) malav     (1000)      206 2024-05-28 03:59:33.000000 mb_pytorch-1.0.54/mb_pytorch.egg-info/PKG-INFO
--rw-rw-r--   0 malav     (1000) malav     (1000)     1643 2024-05-28 03:59:33.000000 mb_pytorch-1.0.54/mb_pytorch.egg-info/SOURCES.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)        1 2024-05-28 03:59:33.000000 mb_pytorch-1.0.54/mb_pytorch.egg-info/dependency_links.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)       27 2024-05-28 03:59:33.000000 mb_pytorch-1.0.54/mb_pytorch.egg-info/requires.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)       19 2024-05-28 03:59:33.000000 mb_pytorch-1.0.54/mb_pytorch.egg-info/top_level.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)       81 2024-05-06 17:42:04.000000 mb_pytorch-1.0.54/pyproject.toml
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-28 03:59:33.696313 mb_pytorch-1.0.54/scripts/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.54/scripts/__init__.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-28 03:59:33.696313 mb_pytorch-1.0.54/scripts/extra_utils/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.54/scripts/extra_utils/__init__.py
--rwxrwxr-x   0 malav     (1000) malav     (1000)     1314 2024-05-28 02:54:47.000000 mb_pytorch-1.0.54/scripts/extra_utils/dataload_results.py
--rw-rw-r--   0 malav     (1000) malav     (1000)       38 2024-05-28 03:59:33.696313 mb_pytorch-1.0.54/setup.cfg
--rw-rw-r--   0 malav     (1000) malav     (1000)      818 2024-05-06 17:42:04.000000 mb_pytorch-1.0.54/setup.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 04:54:03.787999 mb_pytorch-1.0.55/
+-rw-r--r--   0 malav     (1000) malav     (1000)      206 2024-05-30 04:54:03.787999 mb_pytorch-1.0.55/PKG-INFO
+-rw-rw-r--   0 malav     (1000) malav     (1000)      742 2024-05-06 17:42:04.000000 mb_pytorch-1.0.55/README.md
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 04:54:03.779999 mb_pytorch-1.0.55/mb_pytorch/
+-rw-rw-r--   0 malav     (1000) malav     (1000)       97 2024-05-06 17:42:04.000000 mb_pytorch-1.0.55/mb_pytorch/__init__.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 04:54:03.783999 mb_pytorch-1.0.55/mb_pytorch/classification/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-15 16:38:04.000000 mb_pytorch-1.0.55/mb_pytorch/classification/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     7166 2024-05-06 17:42:04.000000 mb_pytorch-1.0.55/mb_pytorch/classification/training.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 04:54:03.783999 mb_pytorch-1.0.55/mb_pytorch/dataloader/
+-rw-rw-r--   0 malav     (1000) malav     (1000)       44 2024-05-28 02:55:26.000000 mb_pytorch-1.0.55/mb_pytorch/dataloader/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)    16093 2024-05-28 03:59:17.000000 mb_pytorch-1.0.55/mb_pytorch/dataloader/loader.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)    19206 2024-05-27 21:31:06.000000 mb_pytorch-1.0.55/mb_pytorch/dataloader/loader_old.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 04:54:03.783999 mb_pytorch-1.0.55/mb_pytorch/detection/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-15 16:38:14.000000 mb_pytorch-1.0.55/mb_pytorch/detection/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     6567 2024-05-27 20:31:19.000000 mb_pytorch-1.0.55/mb_pytorch/detection/training.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 04:54:03.783999 mb_pytorch-1.0.55/mb_pytorch/metalearning/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.55/mb_pytorch/metalearning/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1385 2024-05-06 17:42:04.000000 mb_pytorch-1.0.55/mb_pytorch/metalearning/meta_utils.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1030 2024-05-28 02:54:17.000000 mb_pytorch-1.0.55/mb_pytorch/metalearning/proto_dataloader.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     2861 2024-05-06 17:42:04.000000 mb_pytorch-1.0.55/mb_pytorch/metalearning/prototypical.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 04:54:03.783999 mb_pytorch-1.0.55/mb_pytorch/models/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.55/mb_pytorch/models/__init__.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 04:54:03.783999 mb_pytorch-1.0.55/mb_pytorch/models/blocks/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.55/mb_pytorch/models/blocks/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     2801 2024-05-06 17:42:04.000000 mb_pytorch-1.0.55/mb_pytorch/models/blocks/attention_block.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     3629 2024-05-06 17:42:04.000000 mb_pytorch-1.0.55/mb_pytorch/models/blocks/cnn.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     4783 2024-05-06 17:42:04.000000 mb_pytorch-1.0.55/mb_pytorch/models/blocks/conv_block.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)      920 2024-05-06 17:42:04.000000 mb_pytorch-1.0.55/mb_pytorch/models/blocks/conv_with_relu.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     2256 2024-05-06 17:42:04.000000 mb_pytorch-1.0.55/mb_pytorch/models/blocks/model_out.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1184 2024-05-06 17:42:04.000000 mb_pytorch-1.0.55/mb_pytorch/models/blocks/rnn.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)    21087 2024-05-06 17:42:04.000000 mb_pytorch-1.0.55/mb_pytorch/models/extra_models.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)      920 2024-05-06 17:42:04.000000 mb_pytorch-1.0.55/mb_pytorch/models/lenet.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     3921 2024-05-17 14:58:48.000000 mb_pytorch-1.0.55/mb_pytorch/models/modelloader.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)    10784 2024-05-06 17:42:04.000000 mb_pytorch-1.0.55/mb_pytorch/models/unet_models.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 04:54:03.787999 mb_pytorch-1.0.55/mb_pytorch/segmentation/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-15 16:59:50.000000 mb_pytorch-1.0.55/mb_pytorch/segmentation/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     4800 2024-05-28 02:54:27.000000 mb_pytorch-1.0.55/mb_pytorch/segmentation/training.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 04:54:03.787999 mb_pytorch-1.0.55/mb_pytorch/training/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-15 16:59:41.000000 mb_pytorch-1.0.55/mb_pytorch/training/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1630 2024-05-06 17:42:04.000000 mb_pytorch-1.0.55/mb_pytorch/training/accelerate_train.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1454 2024-05-28 02:54:35.000000 mb_pytorch-1.0.55/mb_pytorch/training/train_params.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)      144 2024-05-06 17:42:04.000000 mb_pytorch-1.0.55/mb_pytorch/training/training.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 04:54:03.787999 mb_pytorch-1.0.55/mb_pytorch/utils/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.55/mb_pytorch/utils/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1055 2024-05-06 17:42:04.000000 mb_pytorch-1.0.55/mb_pytorch/utils/compiler.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)      257 2024-05-06 17:42:04.000000 mb_pytorch-1.0.55/mb_pytorch/utils/dist.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     3391 2024-05-06 17:42:04.000000 mb_pytorch-1.0.55/mb_pytorch/utils/extra_utils.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     7085 2024-05-28 02:55:11.000000 mb_pytorch-1.0.55/mb_pytorch/utils/generate_emb.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     2582 2024-05-06 17:42:04.000000 mb_pytorch-1.0.55/mb_pytorch/utils/losses.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1199 2024-05-06 17:42:04.000000 mb_pytorch-1.0.55/mb_pytorch/utils/metrics.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)      207 2024-05-30 04:53:52.000000 mb_pytorch-1.0.55/mb_pytorch/utils/version.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)    10620 2024-05-23 19:25:11.000000 mb_pytorch-1.0.55/mb_pytorch/utils/viewer.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)      994 2024-05-06 17:42:04.000000 mb_pytorch-1.0.55/mb_pytorch/utils/yaml_reader.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 04:54:03.787999 mb_pytorch-1.0.55/mb_pytorch.egg-info/
+-rw-r--r--   0 malav     (1000) malav     (1000)      206 2024-05-30 04:54:03.000000 mb_pytorch-1.0.55/mb_pytorch.egg-info/PKG-INFO
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1643 2024-05-30 04:54:03.000000 mb_pytorch-1.0.55/mb_pytorch.egg-info/SOURCES.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)        1 2024-05-30 04:54:03.000000 mb_pytorch-1.0.55/mb_pytorch.egg-info/dependency_links.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)       27 2024-05-30 04:54:03.000000 mb_pytorch-1.0.55/mb_pytorch.egg-info/requires.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)       19 2024-05-30 04:54:03.000000 mb_pytorch-1.0.55/mb_pytorch.egg-info/top_level.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)       81 2024-05-06 17:42:04.000000 mb_pytorch-1.0.55/pyproject.toml
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 04:54:03.787999 mb_pytorch-1.0.55/scripts/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.55/scripts/__init__.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 04:54:03.787999 mb_pytorch-1.0.55/scripts/extra_utils/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.55/scripts/extra_utils/__init__.py
+-rwxrwxr-x   0 malav     (1000) malav     (1000)     1314 2024-05-28 02:54:47.000000 mb_pytorch-1.0.55/scripts/extra_utils/dataload_results.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)       38 2024-05-30 04:54:03.787999 mb_pytorch-1.0.55/setup.cfg
+-rw-rw-r--   0 malav     (1000) malav     (1000)      818 2024-05-06 17:42:04.000000 mb_pytorch-1.0.55/setup.py
```

### Comparing `mb_pytorch-1.0.54/README.md` & `mb_pytorch-1.0.55/README.md`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.54/mb_pytorch/classification/training.py` & `mb_pytorch-1.0.55/mb_pytorch/classification/training.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.54/mb_pytorch/dataloader/loader.py` & `mb_pytorch-1.0.55/mb_pytorch/dataloader/loader.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.54/mb_pytorch/dataloader/loader_old.py` & `mb_pytorch-1.0.55/mb_pytorch/dataloader/loader_old.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.54/mb_pytorch/detection/training.py` & `mb_pytorch-1.0.55/mb_pytorch/detection/training.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.54/mb_pytorch/metalearning/meta_utils.py` & `mb_pytorch-1.0.55/mb_pytorch/metalearning/meta_utils.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.54/mb_pytorch/metalearning/proto_dataloader.py` & `mb_pytorch-1.0.55/mb_pytorch/metalearning/proto_dataloader.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.54/mb_pytorch/metalearning/prototypical.py` & `mb_pytorch-1.0.55/mb_pytorch/metalearning/prototypical.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.54/mb_pytorch/models/blocks/attention_block.py` & `mb_pytorch-1.0.55/mb_pytorch/models/blocks/attention_block.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.54/mb_pytorch/models/blocks/cnn.py` & `mb_pytorch-1.0.55/mb_pytorch/models/blocks/cnn.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.54/mb_pytorch/models/blocks/conv_block.py` & `mb_pytorch-1.0.55/mb_pytorch/models/blocks/conv_block.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.54/mb_pytorch/models/blocks/conv_with_relu.py` & `mb_pytorch-1.0.55/mb_pytorch/models/blocks/conv_with_relu.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.54/mb_pytorch/models/blocks/model_out.py` & `mb_pytorch-1.0.55/mb_pytorch/models/blocks/model_out.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.54/mb_pytorch/models/blocks/rnn.py` & `mb_pytorch-1.0.55/mb_pytorch/models/blocks/rnn.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.54/mb_pytorch/models/extra_models.py` & `mb_pytorch-1.0.55/mb_pytorch/models/extra_models.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.54/mb_pytorch/models/lenet.py` & `mb_pytorch-1.0.55/mb_pytorch/models/lenet.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.54/mb_pytorch/models/modelloader.py` & `mb_pytorch-1.0.55/mb_pytorch/models/modelloader.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.54/mb_pytorch/models/unet_models.py` & `mb_pytorch-1.0.55/mb_pytorch/models/unet_models.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.54/mb_pytorch/segmentation/training.py` & `mb_pytorch-1.0.55/mb_pytorch/segmentation/training.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.54/mb_pytorch/training/accelerate_train.py` & `mb_pytorch-1.0.55/mb_pytorch/training/accelerate_train.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.54/mb_pytorch/training/train_params.py` & `mb_pytorch-1.0.55/mb_pytorch/training/train_params.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.54/mb_pytorch/utils/compiler.py` & `mb_pytorch-1.0.55/mb_pytorch/utils/compiler.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.54/mb_pytorch/utils/extra_utils.py` & `mb_pytorch-1.0.55/mb_pytorch/utils/extra_utils.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.54/mb_pytorch/utils/generate_emb.py` & `mb_pytorch-1.0.55/mb_pytorch/utils/generate_emb.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.54/mb_pytorch/utils/losses.py` & `mb_pytorch-1.0.55/mb_pytorch/utils/losses.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.54/mb_pytorch/utils/metrics.py` & `mb_pytorch-1.0.55/mb_pytorch/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.54/mb_pytorch/utils/viewer.py` & `mb_pytorch-1.0.55/mb_pytorch/utils/viewer.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.54/mb_pytorch/utils/yaml_reader.py` & `mb_pytorch-1.0.55/mb_pytorch/utils/yaml_reader.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.54/mb_pytorch.egg-info/SOURCES.txt` & `mb_pytorch-1.0.55/mb_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.54/scripts/extra_utils/dataload_results.py` & `mb_pytorch-1.0.55/scripts/extra_utils/dataload_results.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.54/setup.py` & `mb_pytorch-1.0.55/setup.py`

 * *Files identical despite different names*

