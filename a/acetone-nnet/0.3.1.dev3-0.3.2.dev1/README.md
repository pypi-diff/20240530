# Comparing `tmp/acetone_nnet-0.3.1.dev3.tar.gz` & `tmp/acetone_nnet-0.3.2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acetone_nnet-0.3.1.dev3.tar", last modified: Mon May 27 06:39:21 2024, max compression
+gzip compressed data, was "acetone_nnet-0.3.2.dev1.tar", last modified: Thu May 30 11:57:20 2024, max compression
```

## Comparing `acetone_nnet-0.3.1.dev3.tar` & `acetone_nnet-0.3.2.dev1.tar`

### file list

```diff
@@ -1,153 +1,155 @@
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-27 06:39:21.576202 acetone_nnet-0.3.1.dev3/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      521 2024-04-16 11:45:42.000000 acetone_nnet-0.3.1.dev3/AUTHORS.md
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7652 2024-03-15 08:14:43.000000 acetone_nnet-0.3.1.dev3/COPYING
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    35149 2024-03-15 08:14:43.000000 acetone_nnet-0.3.1.dev3/LICENSE
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6684 2024-05-27 06:39:21.575202 acetone_nnet-0.3.1.dev3/PKG-INFO
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5294 2024-05-14 06:41:04.000000 acetone_nnet-0.3.1.dev3/README.md
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2070 2024-05-27 06:39:05.000000 acetone_nnet-0.3.1.dev3/pyproject.toml
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       38 2024-05-27 06:39:21.576202 acetone_nnet-0.3.1.dev3/setup.cfg
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-27 06:39:21.238198 acetone_nnet-0.3.1.dev3/src/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-27 06:39:21.261198 acetone_nnet-0.3.1.dev3/src/acetone_nnet/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1974 2024-05-23 08:02:27.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-27 06:39:21.262199 acetone_nnet-0.3.1.dev3/src/acetone_nnet/bin/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3252 2024-04-19 14:31:39.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/bin/bin_acetone.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2769 2024-05-24 15:34:10.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/cli_acetone.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3921 2024-05-15 08:22:05.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/cli_compare.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-27 06:39:21.262199 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4184 2024-05-16 06:28:50.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/Layer.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1896 2024-04-17 13:07:48.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5245 2024-05-24 08:55:18.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/activation_functions.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-27 06:39:21.264198 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3826 2024-05-23 14:34:41.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/AddBias.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6435 2024-05-24 06:37:23.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/BatchNormalization.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-27 06:39:21.266198 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1972 2024-05-24 08:54:29.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1599 2024-05-15 08:12:34.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7432 2024-05-24 08:55:08.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1958 2024-05-24 08:54:22.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1592 2024-05-15 08:13:03.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1591 2024-05-15 08:13:08.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1969 2024-05-24 08:54:13.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1969 2024-05-24 08:54:37.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1382 2024-04-15 09:49:48.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7493 2024-05-24 08:55:41.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Concatenate.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-27 06:39:21.266198 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     8516 2024-05-24 08:55:53.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2993 2024-04-15 11:39:05.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6263 2024-05-15 08:10:38.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5339 2024-04-15 06:50:17.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4918 2024-05-15 14:39:50.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1355 2024-04-15 09:50:26.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4311 2024-05-23 11:45:23.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Dense.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4833 2024-05-23 09:59:18.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Dot.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3419 2024-05-24 08:55:24.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Flatten.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6165 2024-05-23 14:35:13.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Gather.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    11596 2024-05-24 08:54:47.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3574 2024-05-24 08:55:32.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Input.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5156 2024-05-23 09:45:10.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/MatMul.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-27 06:39:21.267198 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3207 2024-05-13 13:41:16.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3632 2024-05-13 13:41:10.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4530 2024-05-24 06:51:11.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3669 2024-05-13 13:41:04.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3929 2024-05-13 13:41:00.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1282 2024-04-15 09:51:29.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-27 06:39:21.268199 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1838 2024-05-15 07:56:30.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1721 2024-05-15 07:56:01.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7926 2024-05-24 06:28:37.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1234 2024-04-15 09:51:58.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-27 06:39:21.269199 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    14511 2024-05-23 15:03:15.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6989 2024-05-23 14:48:34.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6096 2024-05-15 07:37:55.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5660 2024-05-23 14:50:00.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1267 2024-04-15 09:52:28.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2798 2024-05-24 14:23:30.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Softmax.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2223 2024-04-16 15:00:06.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    29388 2024-05-23 08:56:40.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/neural_network.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-27 06:39:21.269199 acetone_nnet-0.3.1.dev3/src/acetone_nnet/debug_tools/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1320 2024-05-23 08:01:52.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/debug_tools/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2644 2024-05-23 08:37:10.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/debug_tools/debug_keras.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3744 2024-05-24 09:53:46.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/debug_tools/debug_onnx.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3553 2024-05-22 14:16:11.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/debug_tools/debug_tools.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-27 06:39:21.270198 acetone_nnet-0.3.1.dev3/src/acetone_nnet/format_importer/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-27 06:39:21.270198 acetone_nnet-0.3.1.dev3/src/acetone_nnet/format_importer/H5_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    18708 2024-05-22 15:28:07.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/format_importer/H5_importer/parser_h5.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-27 06:39:21.270198 acetone_nnet-0.3.1.dev3/src/acetone_nnet/format_importer/JSON_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7571 2024-05-14 15:19:20.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/format_importer/JSON_importer/JSON_from_keras_model.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    14564 2024-05-22 15:27:00.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-27 06:39:21.270198 acetone_nnet-0.3.1.dev3/src/acetone_nnet/format_importer/NNET_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3927 2024-05-14 15:17:50.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5379 2024-05-14 15:15:39.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-27 06:39:21.271199 acetone_nnet-0.3.1.dev3/src/acetone_nnet/format_importer/ONNX_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    32928 2024-05-24 08:54:58.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4509 2024-05-14 14:54:21.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2754 2024-05-14 14:53:00.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/format_importer/parser.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-27 06:39:21.271199 acetone_nnet-0.3.1.dev3/src/acetone_nnet/graph/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5719 2024-05-15 08:15:19.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/graph/graph_interpretor.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-27 06:39:21.338199 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1046 2024-04-15 06:29:33.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-27 06:39:21.429201 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-27 06:39:21.489201 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Conv/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1625 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      832 2024-05-13 08:47:00.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      681 2024-05-13 08:46:52.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      872 2024-05-13 08:46:45.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      683 2024-05-13 08:47:06.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      143 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_indirect_gemm.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      375 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_std_gemm.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      875 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      868 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-27 06:39:21.507201 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Gemm/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      225 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Gemm/template_Gemm.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      847 2024-05-17 07:06:52.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      699 2024-05-17 07:07:01.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      742 2024-05-17 07:07:09.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      724 2024-05-17 07:07:16.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-27 06:39:21.510201 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Pad/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1266 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      669 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1001 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      604 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      507 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Pad/template_Wrap_Pad.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-27 06:39:21.539202 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Resize/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1768 2024-05-03 11:58:23.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6868 2024-05-06 08:26:35.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1021 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1689 2024-05-02 13:54:50.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      778 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      352 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/template_AddBiase.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      532 2024-04-17 09:50:38.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2282 2024-04-18 12:38:10.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1274 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      699 2024-05-13 09:26:54.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/template_Dense.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      733 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/template_Dot.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      567 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/template_Flatten.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1284 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/template_Gather.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      658 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      831 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/template_MatMul.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1350 2024-05-21 10:14:20.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      312 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/template_Softmax.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-27 06:39:21.552202 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/memory_layout/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      118 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/memory_layout/template_channels_first_output.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      448 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/memory_layout/template_channels_last_output.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-27 06:39:21.562202 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/normalization/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      341 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/normalization/template_normalization_cst_in_global_var_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      238 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/normalization/template_normalization_cst_in_header_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      167 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/normalization/template_post_processing.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      512 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      237 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/template_Makefile.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1030 2024-05-21 10:01:05.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/template_global_var_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1060 2024-05-21 10:01:00.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/template_header_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1137 2024-05-15 09:26:59.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/template_main_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1633 2024-05-16 07:42:59.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/template_source_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      227 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/template_test_dataset_header.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       96 2024-04-11 15:00:57.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/template_test_dataset_source.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-27 06:39:21.575202 acetone_nnet-0.3.1.dev3/src/acetone_nnet.egg-info/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6684 2024-05-27 06:39:21.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet.egg-info/PKG-INFO
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7098 2024-05-27 06:39:21.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet.egg-info/SOURCES.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)        1 2024-05-27 06:39:21.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet.egg-info/dependency_links.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      146 2024-05-27 06:39:21.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet.egg-info/entry_points.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       82 2024-05-27 06:39:21.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet.egg-info/requires.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       13 2024-05-27 06:39:21.000000 acetone_nnet-0.3.1.dev3/src/acetone_nnet.egg-info/top_level.txt
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:20.008391 acetone_nnet-0.3.2.dev1/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      521 2024-04-16 11:45:42.000000 acetone_nnet-0.3.2.dev1/AUTHORS.md
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7652 2024-03-15 08:14:43.000000 acetone_nnet-0.3.2.dev1/COPYING
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    35149 2024-03-15 08:14:43.000000 acetone_nnet-0.3.2.dev1/LICENSE
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7139 2024-05-30 11:57:20.008391 acetone_nnet-0.3.2.dev1/PKG-INFO
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5749 2024-05-27 09:13:18.000000 acetone_nnet-0.3.2.dev1/README.md
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2070 2024-05-30 11:57:02.000000 acetone_nnet-0.3.2.dev1/pyproject.toml
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       38 2024-05-30 11:57:20.008391 acetone_nnet-0.3.2.dev1/setup.cfg
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.609386 acetone_nnet-0.3.2.dev1/src/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.648387 acetone_nnet-0.3.2.dev1/src/acetone_nnet/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1861 2024-05-30 10:00:06.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.650387 acetone_nnet-0.3.2.dev1/src/acetone_nnet/bin/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3252 2024-04-19 14:31:39.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/bin/bin_acetone.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2764 2024-05-29 09:10:29.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/cli_acetone.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3921 2024-05-15 08:22:05.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/cli_compare.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.651387 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4184 2024-05-16 06:28:50.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/Layer.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1912 2024-05-30 09:59:54.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5245 2024-05-24 08:55:18.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/activation_functions.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.653387 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3826 2024-05-23 14:34:41.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/AddBias.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6435 2024-05-24 06:37:23.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/BatchNormalization.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.655387 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1972 2024-05-24 08:54:29.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1599 2024-05-15 08:12:34.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7432 2024-05-24 08:55:08.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1958 2024-05-24 08:54:22.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1592 2024-05-15 08:13:03.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1591 2024-05-15 08:13:08.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1969 2024-05-24 08:54:13.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1969 2024-05-24 08:54:37.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1382 2024-04-15 09:49:48.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7493 2024-05-24 08:55:41.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Concatenate.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.656387 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     8516 2024-05-30 09:14:00.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2993 2024-04-15 11:39:05.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6263 2024-05-15 08:10:38.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5339 2024-04-15 06:50:17.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4918 2024-05-15 14:39:50.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1355 2024-04-15 09:50:26.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4311 2024-05-23 11:45:23.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Dense.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4833 2024-05-23 09:59:18.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Dot.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3419 2024-05-24 08:55:24.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Flatten.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6165 2024-05-23 14:35:13.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Gather.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    11596 2024-05-24 08:54:47.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3574 2024-05-24 08:55:32.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Input.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5156 2024-05-23 09:45:10.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/MatMul.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.657387 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3207 2024-05-13 13:41:16.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3632 2024-05-13 13:41:10.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4530 2024-05-24 06:51:11.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3669 2024-05-13 13:41:04.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3929 2024-05-13 13:41:00.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1282 2024-04-15 09:51:29.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.658387 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1838 2024-05-15 07:56:30.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1721 2024-05-15 07:56:01.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7926 2024-05-24 06:28:37.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1234 2024-04-15 09:51:58.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.658387 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    14511 2024-05-23 15:03:15.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6989 2024-05-23 14:48:34.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6096 2024-05-15 07:37:55.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5660 2024-05-23 14:50:00.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1267 2024-04-15 09:52:28.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2799 2024-05-29 11:45:24.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Softmax.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5494 2024-05-30 11:54:16.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Transpose.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2274 2024-05-30 09:59:44.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    29413 2024-05-27 11:46:21.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/neural_network.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.659387 acetone_nnet-0.3.2.dev1/src/acetone_nnet/debug_tools/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1370 2024-05-29 07:00:39.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/debug_tools/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2644 2024-05-27 09:32:00.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/debug_tools/debug_keras.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3744 2024-05-27 09:35:47.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/debug_tools/debug_onnx.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4417 2024-05-29 06:27:31.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/debug_tools/debug_tools.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.659387 acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.659387 acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/H5_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    18708 2024-05-22 15:28:07.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/H5_importer/parser_h5.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.660387 acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/JSON_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7571 2024-05-14 15:19:20.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/JSON_importer/JSON_from_keras_model.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    14564 2024-05-22 15:27:00.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.660387 acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/NNET_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3927 2024-05-14 15:17:50.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5381 2024-05-29 07:48:10.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.661387 acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/ONNX_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    33832 2024-05-30 11:56:07.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4509 2024-05-28 14:07:15.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2754 2024-05-14 14:53:00.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/parser.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.661387 acetone_nnet-0.3.2.dev1/src/acetone_nnet/graph/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5719 2024-05-15 08:15:19.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/graph/graph_interpretor.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.734388 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1046 2024-04-15 06:29:33.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.840389 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.887390 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Conv/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1625 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      832 2024-05-13 08:47:00.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      681 2024-05-13 08:46:52.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      872 2024-05-13 08:46:45.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      683 2024-05-13 08:47:06.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      143 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_indirect_gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      375 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_std_gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      875 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      868 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.911390 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Gemm/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      225 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Gemm/template_Gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      847 2024-05-17 07:06:52.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      699 2024-05-17 07:07:01.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      742 2024-05-17 07:07:09.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      724 2024-05-17 07:07:16.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.914390 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Pad/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1266 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      669 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1001 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      604 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      507 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Pad/template_Wrap_Pad.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.962391 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Resize/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1768 2024-05-03 11:58:23.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6868 2024-05-06 08:26:35.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1021 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1689 2024-05-02 13:54:50.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      778 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      352 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_AddBiase.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      532 2024-04-17 09:50:38.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2282 2024-04-18 12:38:10.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1274 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      699 2024-05-13 09:26:54.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_Dense.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      733 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_Dot.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      567 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_Flatten.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1284 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_Gather.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      656 2024-05-30 07:17:26.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      831 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_MatMul.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1350 2024-05-21 10:14:20.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      312 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_Softmax.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      493 2024-05-30 09:52:09.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_Transpose.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.981391 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/memory_layout/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      118 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/memory_layout/template_channels_first_output.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      448 2024-05-29 14:00:27.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/memory_layout/template_channels_last_output.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:19.996391 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/normalization/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      341 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/normalization/template_normalization_cst_in_global_var_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      238 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/normalization/template_normalization_cst_in_header_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      167 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/normalization/template_post_processing.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      512 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      237 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/template_Makefile.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1030 2024-05-21 10:01:05.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/template_global_var_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1060 2024-05-21 10:01:00.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/template_header_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1137 2024-05-15 09:26:59.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/template_main_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1633 2024-05-16 07:42:59.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/template_source_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      227 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/template_test_dataset_header.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       96 2024-04-11 15:00:57.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/template_test_dataset_source.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-30 11:57:20.007391 acetone_nnet-0.3.2.dev1/src/acetone_nnet.egg-info/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7139 2024-05-30 11:57:19.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet.egg-info/PKG-INFO
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7209 2024-05-30 11:57:19.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet.egg-info/SOURCES.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)        1 2024-05-30 11:57:19.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet.egg-info/dependency_links.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      146 2024-05-30 11:57:19.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet.egg-info/entry_points.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       82 2024-05-30 11:57:19.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet.egg-info/requires.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       13 2024-05-30 11:57:19.000000 acetone_nnet-0.3.2.dev1/src/acetone_nnet.egg-info/top_level.txt
```

### Comparing `acetone_nnet-0.3.1.dev3/AUTHORS.md` & `acetone_nnet-0.3.2.dev1/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/COPYING` & `acetone_nnet-0.3.2.dev1/COPYING`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/LICENSE` & `acetone_nnet-0.3.2.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/PKG-INFO` & `acetone_nnet-0.3.2.dev1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acetone-nnet
-Version: 0.3.1.dev3
+Version: 0.3.2.dev1
 Summary: Predictable programming framework for ML applications in safety-critical systems.
 Author-email: Yanis AIT-AISSA <Yanis.AIT-AISSA@student.isae-supaero.fr>, Thomas CARLE <Thomas.Carle@irit.fr>, Iryna DE ALBUQUERQUE SILVA <Iryna.De_Albuquerque_Silva@onera.fr>, Adrien GAUFFRIAU <Adrien.Gauffriau@airbus.com>, Benjamin LESAGE <benjamin.lesage@onera.fr>, Claire PAGETTI <Claire.Pagetti@onera.fr>
 Project-URL: Repository, https://github.com/onera/acetone/
 Project-URL: Bug Tracker, https://github.com/onera/acetone/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
@@ -28,14 +28,22 @@
 # ACETONE
 Predictable programming framework for ML applications in safety-critical systems.
 
 This repo contains the code of the framework presented in the ECRTS'22 paper  ["ACETONE: Predictable programming framework for ML applications in safety-critical systems"](https://drops.dagstuhl.de/entities/document/10.4230/LIPIcs.ECRTS.2022.3).
 
 This framework generate a C code corresponding to a neural network given as input.
 
+## Package
+
+The corresponding package is named [acetone-nnet](https://pypi.org/project/acetone-nnet/). 
+
+The folder [tests/examples](./tests/examples/) give examples on how to use the main functionnalities of the package (code generation and debug mode)
+
+The folder [tests/check_installation](./tests/check_installation/) give a file with a few quick test checking some main, functionalities of the package, as an quick verification of the installation.
+
 
 ## Code architecture
 
 You'll find in the home directory the files regarding the licencing and copyright of the framework:
 
 * [AUTHORS.md](./AUTHORS.md)
 * [LICENSE](./LICENSE)
```

### Comparing `acetone_nnet-0.3.1.dev3/README.md` & `acetone_nnet-0.3.2.dev1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 # ACETONE
 Predictable programming framework for ML applications in safety-critical systems.
 
 This repo contains the code of the framework presented in the ECRTS'22 paper  ["ACETONE: Predictable programming framework for ML applications in safety-critical systems"](https://drops.dagstuhl.de/entities/document/10.4230/LIPIcs.ECRTS.2022.3).
 
 This framework generate a C code corresponding to a neural network given as input.
 
+## Package
+
+The corresponding package is named [acetone-nnet](https://pypi.org/project/acetone-nnet/). 
+
+The folder [tests/examples](./tests/examples/) give examples on how to use the main functionnalities of the package (code generation and debug mode)
+
+The folder [tests/check_installation](./tests/check_installation/) give a file with a few quick test checking some main, functionalities of the package, as an quick verification of the installation.
+
 
 ## Code architecture
 
 You'll find in the home directory the files regarding the licencing and copyright of the framework:
 
 * [AUTHORS.md](./AUTHORS.md)
 * [LICENSE](./LICENSE)
```

### Comparing `acetone_nnet-0.3.1.dev3/pyproject.toml` & `acetone_nnet-0.3.2.dev1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
 
 [project]
 name = "acetone-nnet"
-version = "0.3.1.dev3"
+version = "0.3.2.dev1"
 requires-python = ">=3.10, <3.12"
 
 authors = [
     { name="Yanis AIT-AISSA", email="Yanis.AIT-AISSA@student.isae-supaero.fr"},
     { name="Thomas CARLE", email="Thomas.Carle@irit.fr" },
     { name="Iryna DE ALBUQUERQUE SILVA", email="Iryna.De_Albuquerque_Silva@onera.fr" },
     { name="Adrien GAUFFRIAU", email="Adrien.Gauffriau@airbus.com" },
```

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/__init__.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,30 +17,27 @@
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
 from . import code_generator
 from .code_generator import (
     CodeGenerator, Layer,
-    Add_Bias, Concatenate, Dense, Dot, Flatten, Gather, Gemm, InputLayer, MatMul, Softmax, BatchNormalization,
+    Add_Bias, Concatenate, Dense, Dot, Flatten, Gather, Gemm, InputLayer, MatMul, 
+    Softmax, BatchNormalization, Transpose,
     Add, Average, Broadcast, Divide, Maximum, Minimum, Multiply, Subtract,
     Conv2D, Conv2D_6loops, Conv2D_gemm, Conv2D_indirect_gemm, Conv2D_std_gemm,
     Pad, Edge_pad, Wrap_pad, Reflect_pad, Constant_Pad,
     Pooling2D, MaxPooling2D, AveragePooling2D,
     Resize, ResizeCubic, ResizeLinear, ResizeNearest,
     ActivationFunctions, Linear, Sigmoid, ReLu, TanH, Exponential, Logarithm, Clip, LeakyReLu
 )
 
 from . import debug_tools
-from .debug_tools import (
-    debug_onnx, debug_keras, 
-    compare_result, extract_outputs_c, extract_outputs_python
-)
 
 from .cli_acetone import cli_acetone
 from .cli_compare import cli_compare
 
 __all__ = (
     "cli_acetone", "cli_compare",
     code_generator.__all__,
-    debug_tools.__all__
+    debug_tools
 )
```

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/bin/bin_acetone.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/bin/bin_acetone.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/cli_acetone.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/cli_acetone.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from .code_generator.neural_network import CodeGenerator
 
 def cli_acetone(model_file:str, function_name:str, nb_tests:int, conv_algorithm:str, output_dir:str, test_dataset_file:str|None=None, normalize:bool=False ):
     print("C CODE GENERATOR FOR NEURAL NETWORKS")
 
     pathlib.Path(output_dir).mkdir(parents=True, exist_ok=True)
 
-    net = CodeGenerator(file = model_file, test_dataset_file = test_dataset_file, function_name = function_name, nb_tests = nb_tests, conv_algorithm = conv_algorithm, normalize = normalize)
+    net = CodeGenerator(file = model_file, test_dataset = test_dataset_file, function_name = function_name, nb_tests = nb_tests, conv_algorithm = conv_algorithm, normalize = normalize)
     net.generate_c_files(output_dir)
     net.compute_inference(output_dir)
 
     
 if __name__ == "__main__":
 
     parser = argparse.ArgumentParser(description='C code generator for neural networks')
```

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/cli_compare.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/cli_compare.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/Layer.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/Layer.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/__init__.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,16 @@
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
 from . import layers
 from .layers import (
-    Add_Bias, Concatenate, Dense, Dot, Flatten, Gather, Gemm, InputLayer, MatMul, Softmax, BatchNormalization,
+    Add_Bias, Concatenate, Dense, Dot, Flatten, Gather, Gemm, InputLayer, MatMul, 
+    Softmax, BatchNormalization, Transpose,
     Add, Average, Broadcast, Divide, Maximum, Minimum, Multiply, Subtract,
     Conv2D, Conv2D_6loops, Conv2D_gemm, Conv2D_indirect_gemm, Conv2D_std_gemm,
     Pad, Edge_pad, Wrap_pad, Reflect_pad, Constant_Pad,
     Pooling2D, MaxPooling2D, AveragePooling2D,
     Resize, ResizeCubic, ResizeLinear, ResizeNearest
 )
```

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/activation_functions.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/activation_functions.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/AddBias.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/AddBias.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/BatchNormalization.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/BatchNormalization.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Concatenate.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Concatenate.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Dense.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Dense.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Dot.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Dot.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Flatten.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Flatten.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Gather.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Gather.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Gemm.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Input.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Input.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/MatMul.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/MatMul.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/Softmax.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/Softmax.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,14 @@
         with open(self.template_path+'layers/template_Softmax.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
     
     def forward_path_layer(self, input:np.ndarray):
-        if len(input.shape) == 1:
-            input = np.expand_dims(input,0)
+        if len(input.shape) == 3:
+            input = np.expand_dims(input, 0)
             
         exp = np.exp(input, dtype=np.float)
         output = exp/np.sum(exp, keepdims=1, axis=self.axis)
 
         return output
```

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/layers/__init__.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/layers/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from .Flatten import Flatten
 from .Gather import Gather
 from .Gemm import Gemm
 from .Input import InputLayer
 from .MatMul import MatMul
 from .Softmax import Softmax
 from .BatchNormalization import BatchNormalization
+from .Transpose import Transpose
 
 from . import Broadcast_layers
 from .Broadcast_layers import Add, Average, Broadcast, Divide, Maximum, Minimum, Multiply, Subtract 
 
 from . import Conv_layers
 from .Conv_layers import Conv2D, Conv2D_6loops, Conv2D_gemm, Conv2D_indirect_gemm, Conv2D_std_gemm
 
@@ -43,14 +44,15 @@
 from .Pooling_layers import Pooling2D, AveragePooling2D, MaxPooling2D
 
 from . import Resize_layers
 from .Resize_layers import Resize, ResizeCubic, ResizeLinear, ResizeNearest
 
 
 __all__ = (
-    "Add_Bias", "Concatenate", "Dense", "Dot", "Flatten", "Gather", "Gemm", "InputLayer", "MatMul", "Softmax", "BatchNormalization",
+    "Add_Bias", "Concatenate", "Dense", "Dot", "Flatten", "Gather", "Gemm", "InputLayer", "MatMul", 
+    "Softmax", "BatchNormalization", "Transpose",
     Broadcast_layers.__all__,
     Conv_layers.__all__,
     Pad_layers.__all__,
     Pooling_layers.__all__,
     Resize_layers.__all__
 )
```

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/code_generator/neural_network.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/code_generator/neural_network.py`

 * *Files 0% similar despite different names*

```diff
@@ -404,15 +404,15 @@
         if any(isinstance(layer, ResizeCubic) for layer in self.layers):
             mustach_hash['is_cubic_interpolation'] = True
             
         if any(isinstance(layer, ResizeLinear) for layer in self.layers):
             mustach_hash['is_linear_interpolation'] = True
         
         if self.debug_mode:
-            mustach_hash['debug_file'] = "debug_file.txt"
+            mustach_hash['debug_file'] = self.c_files_directory + "debug_file.txt"
         
         mustach_hash['layers'] = []
         for layer in self.layers:
             layer_hash = {'inference_function':layer.generate_inference_code_layer(), 'path':layer.path, 'size':layer.size}
             
             if layer in self.dict_cst:
                 layer_hash['cst'] = True
```

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/debug_tools/__init__.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/debug_tools/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,13 +18,13 @@
  ******************************************************************************
 """
 
 from .debug_keras import debug_keras
 
 from .debug_onnx import debug_onnx
 
-from .debug_tools import compare_result, extract_outputs_c, extract_outputs_python
+from .debug_tools import compare_result, extract_outputs_c, extract_outputs_python, reorder_outputs_python
 
 __all__ = (
     "debug_keras", "debug_onnx",
-    "compare_result", "extract_outputs_c", "extract_outputs_python"
+    "compare_result", "extract_outputs_c", "extract_outputs_python", "reorder_outputs_python"
 )
```

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/debug_tools/debug_keras.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/debug_tools/debug_keras.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/debug_tools/debug_onnx.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/debug_tools/debug_onnx.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     onnx_result.append(onnx_result.pop(0))
     
     for i in range(len(onnx_result)):
         onnx_result[i] = onnx_result[i].ravel().flatten()
     
     return onnx_result
 
-def debug_onnx(target_model:onnx.ModelProto|str, dataset:np.ndarray, debug_target:list=[], otpimize_inputs:bool = False, to_save:bool = False, path:str = ''):
+def debug_onnx(target_model:onnx.ModelProto|str, dataset:np.ndarray, debug_target:list=[], to_save:bool = False, path:str = '', otpimize_inputs:bool = False):
     # Loading the model
     if type(target_model) == str:
         model = onnx.load(target_model)
     else:
         model = target_model
 
     # Tensor output name and inidce for acetone debug
```

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/debug_tools/debug_tools.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/debug_tools/debug_tools.py`

 * *Files 26% similar despite different names*

```diff
@@ -28,25 +28,36 @@
 
         if verbose:
             print(msg)
         
         return False
     
     correct = True
+    count = 0
+    first = None
     for i in range(len(acetone_result)):
         print('--------------------------------------------')
         print('Comparing',targets[i])
         try:
-            np.testing.assert_allclose(acetone_result[i],reference_result[i],atol=1e-06,rtol=1e-06)
+            np.testing.assert_allclose(acetone_result[i],reference_result[i],atol=5e-06,rtol=5e-06)
         except AssertionError as msg:
             print("Error: output value of",targets[i],"incorrect")
             correct = False
+            count += 1
+            if not first:
+                first = targets[i]
             if verbose:
                 print(msg)
         print('--------------------------------------------')
+    
+    if verbose:
+        print("++++++++++++++++++++++++++++++++++++++++++++")
+        print("Total number of error:",count,"/",len(acetone_result))
+        print("First error at",first)
+        print("++++++++++++++++++++++++++++++++++++++++++++")
 
     return correct
 
 def extract_outputs_c(path_to_output:str, data_type:str, nb_targets:int):
     list_result = []
     targets = []
     to_transpose = False
@@ -87,8 +98,22 @@
     targets = []
     for indice in targets_indice:
         for i in range(len(result_python[1])):
             if indice == int(result_python[1][i][-1]):
                 outputs.append(result_python[0][i])
                 targets.append(result_python[1][i])
 
-    return outputs, targets
+    return outputs, targets
+
+def reorder_outputs_python(outputs_python:list, targets_python:list):
+    ordered_outputs = []
+    ordered_targets = []
+
+    dictionary = {}
+    for i in range(len(targets_python)):
+        dictionary[int(targets_python[i].split(" ")[-1])] = (outputs_python[i], targets_python[i])
+
+    for element in sorted(dictionary.items(), key=lambda item:item[0]):
+        ordered_outputs.append(element[1][0])
+        ordered_targets.append(element[1][1])
+    
+    return ordered_outputs, ordered_targets
```

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/format_importer/H5_importer/parser_h5.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/H5_importer/parser_h5.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/format_importer/JSON_importer/JSON_from_keras_model.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/JSON_importer/JSON_from_keras_model.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     #ranges de normalisation 
     #weights
     #biaises
 
     layers = []
     maxRoad = 1
     dict_cst = {}
-    data_type = float
+    data_type = 'float'
     data_type_py = np.float32
 
     with open(file_to_parse) as f:
      
         line = f.readline()
 
         while line[0:2] == "//": # ignore header lines with credits
```

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,23 +24,22 @@
 
 from ...code_generator.layers import (
     AveragePooling2D, MaxPooling2D,
     Conv2D_6loops, Conv2D_std_gemm, Conv2D_indirect_gemm,
     Edge_pad, Wrap_pad, Reflect_pad, Constant_Pad,
     Add, Multiply, Subtract, Divide, Maximum, Minimum, Average,
     ResizeCubic, ResizeLinear, ResizeNearest,
-    Concatenate, InputLayer, Softmax,  Dot, Gather, Gemm, MatMul, Add_Bias, BatchNormalization
+    Concatenate, InputLayer, Softmax,  Dot, Gather, Gemm, MatMul, Add_Bias, BatchNormalization, Transpose
 )
 
 from ...code_generator.activation_functions import Linear, ReLu, Sigmoid, TanH, Clip, Exponential, Logarithm, LeakyReLu
 
 ###### Utility functions ######
 
 def create_conv2d_obj(algorithm:str, **kwargs):
-       
     if '6loops' in algorithm:
         return Conv2D_6loops(**kwargs)
 
     elif 'std_gemm' in algorithm:
         return Conv2D_std_gemm(**kwargs)   
 
     elif 'indirect_gemm' in algorithm:
@@ -52,24 +51,33 @@
         return ResizeNearest(**kwargs)
     
     elif mode == b'linear':
         return ResizeLinear(**kwargs)
     
     elif mode == b'cubic':
         return ResizeCubic(**kwargs)
+    
+    else:
+        raise ValueError("Error: mode "+mode.decode()+" not implemented")
 
 def create_pad_obj(mode:bytes, **kwargs):
     if mode == b'constant':
         return Constant_Pad(**kwargs)
+    
     elif mode == b'edge':
         return Edge_pad(**kwargs)
+    
     elif mode == b'wrap':
         return Wrap_pad(**kwargs)
+    
     elif mode == b'reflect':
         return Reflect_pad(**kwargs)
+    
+    else:
+        raise ValueError("Error: mode "+mode.decode()+" not implemented")
 
 #Go find the constant named initialzer_name in model(an onnx model)
 def look_for_initializer(initializer_name:str, model:onnx.ModelProto):
     if (initializer_name == ''):
         return []
     for initializer in model.graph.initializer:
         if (initializer.name == initializer_name):
@@ -127,15 +135,18 @@
 def create_Softmax(node:onnx.NodeProto, idx:int, dict_input:dict, dict_output:dict, model:onnx.ModelProto):
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = node.input
     dict_output[node.output[0]] = idx
     attributs = extract_attribut(node)
     if 'axis' not in attributs:
-        attributs['axis'] = -1
+        if model.opset_import[0].version < 13:
+            attributs['axis'] = 1
+        else:
+            attributs['axis'] = -1
     return Softmax(idx = idx,
                     size = size,
                     axis = attributs['axis'])
 
 
 #Create a layer Conv
 def create_Conv(node:onnx.NodeProto, idx:int, dict_input:dict, dict_output:dict, model:onnx.ModelProto, conv_algorithm:str):
@@ -405,14 +416,27 @@
                               epsilon = attributs['epsilon'],
                               scale = onnx.numpy_helper.to_array(scale),
                               biases = onnx.numpy_helper.to_array(biases),
                               mean = onnx.numpy_helper.to_array(mean),
                               var = onnx.numpy_helper.to_array(var),
                               activation_function = Linear())
 
+def create_Transpose(node:onnx.NodeProto, idx:int, dict_input:dict, dict_output:dict, model:onnx.ModelProto):
+    input_shape = get_shape(node.input[0],model)
+    output_shape = get_shape(node.output[0],model)
+    size = find_size(output_shape)
+    dict_input[idx] = node.input
+    dict_output[node.output[0]] = idx
+    attributs = extract_attribut(node)
+    return Transpose(idx = idx,
+                     size = size,
+                     input_shape = input_shape,
+                     perm = attributs['perm'],
+                     activation_function = Linear())
+
 
 
 ### Pooling layers ###
 
 #Create a layer MaxPool
 def create_MaxPool(node:onnx.NodeProto, idx:int, dict_input:dict, dict_output:dict, model:onnx.ModelProto):
     input_shape = get_shape(node.input[0],model)
@@ -671,14 +695,15 @@
          "Conv":create_Conv, 
          "Resize":create_Resize,
          "Pad":create_Pad,
          "Concat":create_Concat,
          "Gather":create_Gather,
          "Gemm":create_Gemm,
          "MatMul":create_MatMul,
+         "Transpose":create_Transpose,
          "MaxPool":create_MaxPool,
          "AveragePool":create_AveragePool,
          "GlobalAveragePool":create_GlobalAveragePool,
          "Add":create_Add,
          "Mul":create_Mul,
          "Div":create_Div,
          "Sub":create_Sub,
```

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/format_importer/parser.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/format_importer/parser.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/graph/graph_interpretor.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/graph/graph_interpretor.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/__init__.py` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/template_Dense.c.tpl` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_Dense.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/template_Dot.c.tpl` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_Dot.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/template_Flatten.c.tpl` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_Flatten.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/template_Gather.c.tpl` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_Gather.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
     // {{name}}_{{idx}}
 {{^channels_last}}
-    // Charging the input in channels_first
+    // Loading the input in channels_first
     for (k = 0; k < {{size}}; ++k)
     {
         output_{{road}}[k] = nn_input[k];
     }
 {{/channels_last}}
 {{#channels_last}}
-    // Charging the input and changing it from channels_last to channels_first format
+    // Loading the input and changing it from channels_last to channels_first format
     for(f = 0; f < {{input_channels}}; ++f)
     {
         for (i = 0; i < {{input_height}}; ++i)
         {
             for (j = 0; j < {{input_width}};  ++j)
             {
                 output_{{road}}[(i + {{input_height}}*f)*{{input_width}} + j] = nn_input[(i*{{input_width}} + j)*{{input_channels}} + f];
```

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/template_MatMul.c.tpl` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_MatMul.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/template_global_var_file.c.tpl` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/template_global_var_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/template_header_file.c.tpl` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/template_header_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/template_main_file.c.tpl` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/template_main_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet/templates/template_source_file.c.tpl` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet/templates/template_source_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet.egg-info/PKG-INFO` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acetone-nnet
-Version: 0.3.1.dev3
+Version: 0.3.2.dev1
 Summary: Predictable programming framework for ML applications in safety-critical systems.
 Author-email: Yanis AIT-AISSA <Yanis.AIT-AISSA@student.isae-supaero.fr>, Thomas CARLE <Thomas.Carle@irit.fr>, Iryna DE ALBUQUERQUE SILVA <Iryna.De_Albuquerque_Silva@onera.fr>, Adrien GAUFFRIAU <Adrien.Gauffriau@airbus.com>, Benjamin LESAGE <benjamin.lesage@onera.fr>, Claire PAGETTI <Claire.Pagetti@onera.fr>
 Project-URL: Repository, https://github.com/onera/acetone/
 Project-URL: Bug Tracker, https://github.com/onera/acetone/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
@@ -28,14 +28,22 @@
 # ACETONE
 Predictable programming framework for ML applications in safety-critical systems.
 
 This repo contains the code of the framework presented in the ECRTS'22 paper  ["ACETONE: Predictable programming framework for ML applications in safety-critical systems"](https://drops.dagstuhl.de/entities/document/10.4230/LIPIcs.ECRTS.2022.3).
 
 This framework generate a C code corresponding to a neural network given as input.
 
+## Package
+
+The corresponding package is named [acetone-nnet](https://pypi.org/project/acetone-nnet/). 
+
+The folder [tests/examples](./tests/examples/) give examples on how to use the main functionnalities of the package (code generation and debug mode)
+
+The folder [tests/check_installation](./tests/check_installation/) give a file with a few quick test checking some main, functionalities of the package, as an quick verification of the installation.
+
 
 ## Code architecture
 
 You'll find in the home directory the files regarding the licencing and copyright of the framework:
 
 * [AUTHORS.md](./AUTHORS.md)
 * [LICENSE](./LICENSE)
```

### Comparing `acetone_nnet-0.3.1.dev3/src/acetone_nnet.egg-info/SOURCES.txt` & `acetone_nnet-0.3.2.dev1/src/acetone_nnet.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 src/acetone_nnet/code_generator/layers/Dot.py
 src/acetone_nnet/code_generator/layers/Flatten.py
 src/acetone_nnet/code_generator/layers/Gather.py
 src/acetone_nnet/code_generator/layers/Gemm.py
 src/acetone_nnet/code_generator/layers/Input.py
 src/acetone_nnet/code_generator/layers/MatMul.py
 src/acetone_nnet/code_generator/layers/Softmax.py
+src/acetone_nnet/code_generator/layers/Transpose.py
 src/acetone_nnet/code_generator/layers/__init__.py
 src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py
 src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py
 src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py
 src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py
 src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py
 src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py
@@ -88,14 +89,15 @@
 src/acetone_nnet/templates/layers/template_Dot.c.tpl
 src/acetone_nnet/templates/layers/template_Flatten.c.tpl
 src/acetone_nnet/templates/layers/template_Gather.c.tpl
 src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl
 src/acetone_nnet/templates/layers/template_MatMul.c.tpl
 src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl
 src/acetone_nnet/templates/layers/template_Softmax.c.tpl
+src/acetone_nnet/templates/layers/template_Transpose.c.tpl
 src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl
 src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl
 src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl
 src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl
 src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl
 src/acetone_nnet/templates/layers/Conv/template_Conv_indirect_gemm.c.tpl
 src/acetone_nnet/templates/layers/Conv/template_Conv_std_gemm.c.tpl
```

