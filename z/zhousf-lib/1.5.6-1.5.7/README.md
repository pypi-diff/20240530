# Comparing `tmp/zhousf-lib-1.5.6.tar.gz` & `tmp/zhousf-lib-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhousf-lib-1.5.6.tar", last modified: Thu May  9 02:54:12 2024, max compression
+gzip compressed data, was "zhousf-lib-1.5.7.tar", last modified: Wed May 29 09:34:38 2024, max compression
```

## Comparing `zhousf-lib-1.5.6.tar` & `zhousf-lib-1.5.7.tar`

### file list

```diff
@@ -1,150 +1,153 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 02:54:12.049388 zhousf-lib-1.5.6/
--rw-rw-rw-   0        0        0     1086 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/LICENSE
--rw-rw-rw-   0        0        0     3232 2024-05-09 02:54:12.048388 zhousf-lib-1.5.6/PKG-INFO
--rw-rw-rw-   0        0        0     2338 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/README.md
--rw-rw-rw-   0        0        0       42 2024-05-09 02:54:12.049388 zhousf-lib-1.5.6/setup.cfg
--rw-rw-rw-   0        0        0     4535 2024-05-09 02:54:06.000000 zhousf-lib-1.5.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:54:10.989902 zhousf-lib-1.5.6/zhousf_lib.egg-info/
--rw-rw-rw-   0        0        0     3232 2024-05-09 02:54:10.000000 zhousf-lib-1.5.6/zhousf_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3912 2024-05-09 02:54:10.000000 zhousf-lib-1.5.6/zhousf_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 02:54:10.000000 zhousf-lib-1.5.6/zhousf_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-09 02:54:10.000000 zhousf-lib-1.5.6/zhousf_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-09 02:54:10.990902 zhousf-lib-1.5.6/zhousflib/
--rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:54:10.992904 zhousf-lib-1.5.6/zhousflib/ann/
--rw-rw-rw-   0        0        0     6638 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/ann/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.015599 zhousf-lib-1.5.6/zhousflib/ann/onnx/
--rw-rw-rw-   0        0        0     3170 2024-03-25 07:18:11.000000 zhousf-lib-1.5.6/zhousflib/ann/onnx/__init__.py
--rw-rw-rw-   0        0        0     6855 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/ann/onnx/onnx_to_trt.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.029679 zhousf-lib-1.5.6/zhousflib/ann/tensorrt/
--rw-rw-rw-   0        0        0       86 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/ann/tensorrt/__init__.py
--rw-rw-rw-   0        0        0     5990 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/ann/tensorrt/tensorrt_infer.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.067783 zhousf-lib-1.5.6/zhousflib/ann/torch/
--rw-rw-rw-   0        0        0     1251 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/ann/torch/__init__.py
--rw-rw-rw-   0        0        0     6881 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/ann/torch/torch_to_onnx.py
--rw-rw-rw-   0        0        0     5934 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/ann/torch/torch_to_script.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.070783 zhousf-lib-1.5.6/zhousflib/ann/transformers/
--rw-rw-rw-   0        0        0     1709 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/ann/transformers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.089859 zhousf-lib-1.5.6/zhousflib/database/
--rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/database/__init__.py
--rw-rw-rw-   0        0        0     2630 2024-04-24 02:58:49.000000 zhousf-lib-1.5.6/zhousflib/database/lmdb_master.py
--rw-rw-rw-   0        0        0     2860 2024-04-24 02:55:52.000000 zhousf-lib-1.5.6/zhousflib/database/tinydb_master.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.112859 zhousf-lib-1.5.6/zhousflib/datasets/
--rw-rw-rw-   0        0        0       84 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/datasets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.120193 zhousf-lib-1.5.6/zhousflib/datasets/classification/
--rw-rw-rw-   0        0        0       73 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/datasets/classification/__init__.py
--rw-rw-rw-   0        0        0     4897 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/datasets/classification/classification_dataset_split.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.189065 zhousf-lib-1.5.6/zhousflib/datasets/coco/
--rw-rw-rw-   0        0        0     1416 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/datasets/coco/__init__.py
--rw-rw-rw-   0        0        0     8259 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/datasets/coco/coco_bbox_extract.py
--rw-rw-rw-   0        0        0     5499 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/datasets/coco/coco_bbox_update.py
--rw-rw-rw-   0        0        0     6641 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/datasets/coco/coco_bbox_vis.py
--rw-rw-rw-   0        0        0     2896 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/datasets/coco/coco_dataset_merge.py
--rw-rw-rw-   0        0        0     4946 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/datasets/coco/coco_dataset_split.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.278433 zhousf-lib-1.5.6/zhousflib/datasets/labelme/
--rw-rw-rw-   0        0        0      981 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/datasets/labelme/__init__.py
--rw-rw-rw-   0        0        0     1276 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/datasets/labelme/labelme_bbox_update.py
--rw-rw-rw-   0        0        0     3906 2024-03-25 07:25:55.000000 zhousf-lib-1.5.6/zhousflib/datasets/labelme/labelme_clip.py
--rw-rw-rw-   0        0        0     8093 2024-03-25 07:25:54.000000 zhousf-lib-1.5.6/zhousflib/datasets/labelme/labelme_convert_coco.py
--rw-rw-rw-   0        0        0     9624 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/datasets/labelme/labelme_convert_seg.py
--rw-rw-rw-   0        0        0    10464 2024-03-25 07:25:54.000000 zhousf-lib-1.5.6/zhousflib/datasets/labelme/labelme_convert_uiex.py
--rw-rw-rw-   0        0        0     3832 2024-03-25 07:25:54.000000 zhousf-lib-1.5.6/zhousflib/datasets/labelme/labelme_dataset_clip.py
--rw-rw-rw-   0        0        0     1674 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/datasets/labelme/shape_convert.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.287567 zhousf-lib-1.5.6/zhousflib/datasets/segmentation/
--rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/datasets/segmentation/__init__.py
--rw-rw-rw-   0        0        0     2958 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/datasets/segmentation/seg_dataset_split.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.296589 zhousf-lib-1.5.6/zhousflib/decorator/
--rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/decorator/__init__.py
--rw-rw-rw-   0        0        0      504 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/decorator/except_util.py
--rw-rw-rw-   0        0        0     1094 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/decorator/interceptor_util.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.334598 zhousf-lib-1.5.6/zhousflib/file/
--rw-rw-rw-   0        0        0     1230 2024-01-30 02:48:23.000000 zhousf-lib-1.5.6/zhousflib/file/__init__.py
--rw-rw-rw-   0        0        0     3250 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/file/delete_file.py
--rw-rw-rw-   0        0        0     4725 2024-04-01 06:46:05.000000 zhousf-lib-1.5.6/zhousflib/file/download.py
--rw-rw-rw-   0        0        0     3227 2024-04-01 06:46:05.000000 zhousf-lib-1.5.6/zhousflib/file/zip_util.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.482673 zhousf-lib-1.5.6/zhousflib/font/
--rw-rw-rw-   0        0        0 15320040 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/font/SimSun.ttf
--rw-rw-rw-   0        0        0  2152796 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/font/Symbola.ttf
--rw-rw-rw-   0        0        0      765 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/font/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.592577 zhousf-lib-1.5.6/zhousflib/image/
--rw-rw-rw-   0        0        0     1159 2024-04-01 06:55:42.000000 zhousf-lib-1.5.6/zhousflib/image/__init__.py
--rw-rw-rw-   0        0        0     5599 2024-01-30 02:48:23.000000 zhousf-lib-1.5.6/zhousflib/image/cv.py
--rw-rw-rw-   0        0        0     6818 2024-04-01 06:55:42.000000 zhousf-lib-1.5.6/zhousflib/image/cv_util.py
--rw-rw-rw-   0        0        0     8570 2024-03-25 07:25:55.000000 zhousf-lib-1.5.6/zhousflib/image/img_util.py
--rw-rw-rw-   0        0        0     5768 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/image/nms_util.py
--rw-rw-rw-   0        0        0     8569 2024-03-25 07:25:55.000000 zhousf-lib-1.5.6/zhousflib/image/op.py
--rw-rw-rw-   0        0        0     4228 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/image/pil_util.py
--rw-rw-rw-   0        0        0    10277 2024-03-07 06:30:39.000000 zhousf-lib-1.5.6/zhousflib/image/similarity.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.604547 zhousf-lib-1.5.6/zhousflib/infer_framework/
--rw-rw-rw-   0        0        0       86 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/infer_framework/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.666102 zhousf-lib-1.5.6/zhousflib/infer_framework/fast_infer/
--rw-rw-rw-   0        0        0       86 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/infer_framework/fast_infer/__init__.py
--rw-rw-rw-   0        0        0      851 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/infer_framework/fast_infer/backend.py
--rw-rw-rw-   0        0        0     3594 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/infer_framework/fast_infer/backend_http.py
--rw-rw-rw-   0        0        0     3685 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/infer_framework/fast_infer/backend_onnx.py
--rw-rw-rw-   0        0        0      612 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/infer_framework/fast_infer/backend_original.py
--rw-rw-rw-   0        0        0     3152 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/infer_framework/fast_infer/backend_tensorrt.py
--rw-rw-rw-   0        0        0     2661 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/infer_framework/fast_infer/backend_torch_script.py
--rw-rw-rw-   0        0        0     7080 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/infer_framework/fast_infer/fast_infer.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.687091 zhousf-lib-1.5.6/zhousflib/infer_framework/triton/
--rw-rw-rw-   0        0        0     3124 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/infer_framework/triton/__init__.py
--rw-rw-rw-   0        0        0    12167 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/infer_framework/triton/client_http.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.697559 zhousf-lib-1.5.6/zhousflib/locust/
--rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/locust/__init__.py
--rw-rw-rw-   0        0        0     1525 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/locust/locust_demo.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.711587 zhousf-lib-1.5.6/zhousflib/metrics/
--rw-rw-rw-   0        0        0       76 2024-02-29 06:32:37.000000 zhousf-lib-1.5.6/zhousflib/metrics/__init__.py
--rw-rw-rw-   0        0        0     3429 2024-03-25 07:21:21.000000 zhousf-lib-1.5.6/zhousflib/metrics/f_score.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.760794 zhousf-lib-1.5.6/zhousflib/ml/
--rw-rw-rw-   0        0        0       99 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/ml/__init__.py
--rw-rw-rw-   0        0        0     4515 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/ml/feature_vector.py
--rw-rw-rw-   0        0        0     8568 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/ml/model_base.py
--rw-rw-rw-   0        0        0     2923 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/ml/model_cluster.py
--rw-rw-rw-   0        0        0    10995 2024-01-31 01:40:34.000000 zhousf-lib-1.5.6/zhousflib/ml/model_gbdt.py
--rw-rw-rw-   0        0        0     7630 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/ml/model_lr.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.784286 zhousf-lib-1.5.6/zhousflib/pandas/
--rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/pandas/__init__.py
--rw-rw-rw-   0        0        0     4839 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/pandas/openpyxl_util.py
--rw-rw-rw-   0        0        0     6180 2024-04-01 06:42:29.000000 zhousf-lib-1.5.6/zhousflib/pandas/pandas_util.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.819288 zhousf-lib-1.5.6/zhousflib/pdf/
--rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/pdf/__init__.py
--rw-rw-rw-   0        0        0     1847 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/pdf/export_image.py
--rw-rw-rw-   0        0        0     1465 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/pdf/pdfplumber_util.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.838437 zhousf-lib-1.5.6/zhousflib/so/
--rw-rw-rw-   0        0        0       85 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/so/__init__.py
--rw-rw-rw-   0        0        0     3840 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/so/project_to_so.py
--rw-rw-rw-   0        0        0      286 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/so/py_to_so.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.840407 zhousf-lib-1.5.6/zhousflib/text/
--rw-rw-rw-   0        0        0       87 2024-01-31 01:12:08.000000 zhousf-lib-1.5.6/zhousflib/text/__init__.py
--rw-rw-rw-   0        0        0     3141 2024-02-29 06:26:47.000000 zhousf-lib-1.5.6/zhousflib/text/similarity.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.860250 zhousf-lib-1.5.6/zhousflib/thread/
--rw-rw-rw-   0        0        0       60 2024-04-01 07:09:10.000000 zhousf-lib-1.5.6/zhousflib/thread/__init__.py
--rw-rw-rw-   0        0        0     2318 2024-04-08 01:21:36.000000 zhousf-lib-1.5.6/zhousflib/thread/thread_util.py
--rw-rw-rw-   0        0        0      829 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/thread/threadpool_util.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.878812 zhousf-lib-1.5.6/zhousflib/time/
--rw-rw-rw-   0        0        0     1159 2024-03-25 07:19:09.000000 zhousf-lib-1.5.6/zhousflib/time/__init__.py
--rw-rw-rw-   0        0        0     4671 2024-03-25 07:18:11.000000 zhousf-lib-1.5.6/zhousflib/time/time_util.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.999397 zhousf-lib-1.5.6/zhousflib/util/
--rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/util/__init__.py
--rw-rw-rw-   0        0        0     3143 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/util/calculater_util.py
--rw-rw-rw-   0        0        0     2161 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/util/char_util.py
--rw-rw-rw-   0        0        0     2703 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/util/dict_util.py
--rw-rw-rw-   0        0        0     2195 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/util/encrypt_util.py
--rw-rw-rw-   0        0        0    13480 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/util/iou_util.py
--rw-rw-rw-   0        0        0     3373 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/util/json_util.py
--rw-rw-rw-   0        0        0     5241 2024-04-29 05:35:07.000000 zhousf-lib-1.5.6/zhousflib/util/list_util.py
--rw-rw-rw-   0        0        0     1481 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/util/math_util.py
--rw-rw-rw-   0        0        0     1358 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/util/permission_util.py
--rw-rw-rw-   0        0        0     3526 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/util/poly_util.py
--rw-rw-rw-   0        0        0      527 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/util/random_util.py
--rw-rw-rw-   0        0        0     4692 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/util/re_util.py
--rw-rw-rw-   0        0        0      520 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/util/singleton.py
--rw-rw-rw-   0        0        0     5122 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/util/string_util.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:54:12.033155 zhousf-lib-1.5.6/zhousflib/web/
--rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/web/__init__.py
--rw-rw-rw-   0        0        0     4246 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/web/config.py
--rw-rw-rw-   0        0        0     1200 2024-03-21 07:56:35.000000 zhousf-lib-1.5.6/zhousflib/web/fast_api.py
--rw-rw-rw-   0        0        0     3107 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/web/log_util.py
--rw-rw-rw-   0        0        0     4497 2024-05-09 02:53:54.000000 zhousf-lib-1.5.6/zhousflib/web/logger.py
--rw-rw-rw-   0        0        0     1340 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/web/response.py
--rw-rw-rw-   0        0        0     6913 2024-04-01 08:27:11.000000 zhousf-lib-1.5.6/zhousflib/web/web.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:34:38.414334 zhousf-lib-1.5.7/
+-rw-rw-rw-   0        0        0     1086 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/LICENSE
+-rw-rw-rw-   0        0        0     3232 2024-05-29 09:34:38.413465 zhousf-lib-1.5.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2338 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-29 09:34:38.414334 zhousf-lib-1.5.7/setup.cfg
+-rw-rw-rw-   0        0        0     4535 2024-05-29 09:34:32.000000 zhousf-lib-1.5.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:34:37.383973 zhousf-lib-1.5.7/zhousf_lib.egg-info/
+-rw-rw-rw-   0        0        0     3232 2024-05-29 09:34:37.000000 zhousf-lib-1.5.7/zhousf_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4030 2024-05-29 09:34:37.000000 zhousf-lib-1.5.7/zhousf_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 09:34:37.000000 zhousf-lib-1.5.7/zhousf_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-29 09:34:37.000000 zhousf-lib-1.5.7/zhousf_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 09:34:37.385970 zhousf-lib-1.5.7/zhousflib/
+-rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:34:37.387996 zhousf-lib-1.5.7/zhousflib/ann/
+-rw-rw-rw-   0        0        0     6638 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/ann/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:34:37.412656 zhousf-lib-1.5.7/zhousflib/ann/onnx/
+-rw-rw-rw-   0        0        0     3170 2024-03-25 07:18:11.000000 zhousf-lib-1.5.7/zhousflib/ann/onnx/__init__.py
+-rw-rw-rw-   0        0        0     6855 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/ann/onnx/onnx_to_trt.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:34:37.427351 zhousf-lib-1.5.7/zhousflib/ann/tensorrt/
+-rw-rw-rw-   0        0        0       86 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/ann/tensorrt/__init__.py
+-rw-rw-rw-   0        0        0     5990 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/ann/tensorrt/tensorrt_infer.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:34:37.463495 zhousf-lib-1.5.7/zhousflib/ann/torch/
+-rw-rw-rw-   0        0        0     1251 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/ann/torch/__init__.py
+-rw-rw-rw-   0        0        0     6881 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/ann/torch/torch_to_onnx.py
+-rw-rw-rw-   0        0        0     5934 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/ann/torch/torch_to_script.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:34:37.465496 zhousf-lib-1.5.7/zhousflib/ann/transformers/
+-rw-rw-rw-   0        0        0     1709 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/ann/transformers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:34:37.486495 zhousf-lib-1.5.7/zhousflib/database/
+-rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/database/__init__.py
+-rw-rw-rw-   0        0        0     2630 2024-04-24 02:58:49.000000 zhousf-lib-1.5.7/zhousflib/database/lmdb_master.py
+-rw-rw-rw-   0        0        0     2860 2024-04-24 02:55:52.000000 zhousf-lib-1.5.7/zhousflib/database/tinydb_master.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:34:37.503043 zhousf-lib-1.5.7/zhousflib/datasets/
+-rw-rw-rw-   0        0        0       84 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/datasets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:34:37.514043 zhousf-lib-1.5.7/zhousflib/datasets/classification/
+-rw-rw-rw-   0        0        0       73 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/datasets/classification/__init__.py
+-rw-rw-rw-   0        0        0     4897 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/datasets/classification/classification_dataset_split.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:34:37.589273 zhousf-lib-1.5.7/zhousflib/datasets/coco/
+-rw-rw-rw-   0        0        0     1416 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/datasets/coco/__init__.py
+-rw-rw-rw-   0        0        0     8259 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/datasets/coco/coco_bbox_extract.py
+-rw-rw-rw-   0        0        0     5499 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/datasets/coco/coco_bbox_update.py
+-rw-rw-rw-   0        0        0     6641 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/datasets/coco/coco_bbox_vis.py
+-rw-rw-rw-   0        0        0     2896 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/datasets/coco/coco_dataset_merge.py
+-rw-rw-rw-   0        0        0     4946 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/datasets/coco/coco_dataset_split.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:34:37.680174 zhousf-lib-1.5.7/zhousflib/datasets/labelme/
+-rw-rw-rw-   0        0        0      981 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/datasets/labelme/__init__.py
+-rw-rw-rw-   0        0        0     1276 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/datasets/labelme/labelme_bbox_update.py
+-rw-rw-rw-   0        0        0     3906 2024-03-25 07:25:55.000000 zhousf-lib-1.5.7/zhousflib/datasets/labelme/labelme_clip.py
+-rw-rw-rw-   0        0        0     8093 2024-03-25 07:25:54.000000 zhousf-lib-1.5.7/zhousflib/datasets/labelme/labelme_convert_coco.py
+-rw-rw-rw-   0        0        0     9624 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/datasets/labelme/labelme_convert_seg.py
+-rw-rw-rw-   0        0        0    10464 2024-03-25 07:25:54.000000 zhousf-lib-1.5.7/zhousflib/datasets/labelme/labelme_convert_uiex.py
+-rw-rw-rw-   0        0        0     3832 2024-03-25 07:25:54.000000 zhousf-lib-1.5.7/zhousflib/datasets/labelme/labelme_dataset_clip.py
+-rw-rw-rw-   0        0        0     1674 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/datasets/labelme/shape_convert.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:34:37.696174 zhousf-lib-1.5.7/zhousflib/datasets/segmentation/
+-rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/datasets/segmentation/__init__.py
+-rw-rw-rw-   0        0        0     2958 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/datasets/segmentation/seg_dataset_split.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:34:37.707725 zhousf-lib-1.5.7/zhousflib/decorator/
+-rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/decorator/__init__.py
+-rw-rw-rw-   0        0        0      504 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/decorator/except_util.py
+-rw-rw-rw-   0        0        0     1094 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/decorator/interceptor_util.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:34:37.742725 zhousf-lib-1.5.7/zhousflib/file/
+-rw-rw-rw-   0        0        0     1230 2024-01-30 02:48:23.000000 zhousf-lib-1.5.7/zhousflib/file/__init__.py
+-rw-rw-rw-   0        0        0     3250 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/file/delete_file.py
+-rw-rw-rw-   0        0        0     4725 2024-04-01 06:46:05.000000 zhousf-lib-1.5.7/zhousflib/file/download.py
+-rw-rw-rw-   0        0        0     3227 2024-04-01 06:46:05.000000 zhousf-lib-1.5.7/zhousflib/file/zip_util.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:34:37.890984 zhousf-lib-1.5.7/zhousflib/font/
+-rw-rw-rw-   0        0        0 15320040 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/font/SimSun.ttf
+-rw-rw-rw-   0        0        0  2152796 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/font/Symbola.ttf
+-rw-rw-rw-   0        0        0      765 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/font/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:34:37.943560 zhousf-lib-1.5.7/zhousflib/image/
+-rw-rw-rw-   0        0        0     1159 2024-04-01 06:55:42.000000 zhousf-lib-1.5.7/zhousflib/image/__init__.py
+-rw-rw-rw-   0        0        0     5599 2024-01-30 02:48:23.000000 zhousf-lib-1.5.7/zhousflib/image/cv.py
+-rw-rw-rw-   0        0        0     6818 2024-04-01 06:55:42.000000 zhousf-lib-1.5.7/zhousflib/image/cv_util.py
+-rw-rw-rw-   0        0        0     8570 2024-03-25 07:25:55.000000 zhousf-lib-1.5.7/zhousflib/image/img_util.py
+-rw-rw-rw-   0        0        0     5768 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/image/nms_util.py
+-rw-rw-rw-   0        0        0     8569 2024-03-25 07:25:55.000000 zhousf-lib-1.5.7/zhousflib/image/op.py
+-rw-rw-rw-   0        0        0     4484 2024-05-28 08:40:26.000000 zhousf-lib-1.5.7/zhousflib/image/pil_util.py
+-rw-rw-rw-   0        0        0    10277 2024-03-07 06:30:39.000000 zhousf-lib-1.5.7/zhousflib/image/similarity.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:34:37.957588 zhousf-lib-1.5.7/zhousflib/infer_framework/
+-rw-rw-rw-   0        0        0       86 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/infer_framework/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:34:38.011387 zhousf-lib-1.5.7/zhousflib/infer_framework/fast_infer/
+-rw-rw-rw-   0        0        0       86 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/infer_framework/fast_infer/__init__.py
+-rw-rw-rw-   0        0        0     1072 2024-05-28 07:55:51.000000 zhousf-lib-1.5.7/zhousflib/infer_framework/fast_infer/backend.py
+-rw-rw-rw-   0        0        0    13914 2024-05-29 09:34:05.000000 zhousf-lib-1.5.7/zhousflib/infer_framework/fast_infer/backend_fastdeploy.py
+-rw-rw-rw-   0        0        0     3595 2024-05-28 07:55:51.000000 zhousf-lib-1.5.7/zhousflib/infer_framework/fast_infer/backend_http.py
+-rw-rw-rw-   0        0        0     3686 2024-05-28 07:55:51.000000 zhousf-lib-1.5.7/zhousflib/infer_framework/fast_infer/backend_onnx.py
+-rw-rw-rw-   0        0        0      614 2024-05-28 07:55:51.000000 zhousf-lib-1.5.7/zhousflib/infer_framework/fast_infer/backend_original.py
+-rw-rw-rw-   0        0        0     3153 2024-05-28 07:55:51.000000 zhousf-lib-1.5.7/zhousflib/infer_framework/fast_infer/backend_tensorrt.py
+-rw-rw-rw-   0        0        0     2662 2024-05-28 07:55:51.000000 zhousf-lib-1.5.7/zhousflib/infer_framework/fast_infer/backend_torch_script.py
+-rw-rw-rw-   0        0        0    11440 2024-05-29 09:33:39.000000 zhousf-lib-1.5.7/zhousflib/infer_framework/fast_infer/fast_infer.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:34:38.028386 zhousf-lib-1.5.7/zhousflib/infer_framework/triton/
+-rw-rw-rw-   0        0        0     3124 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/infer_framework/triton/__init__.py
+-rw-rw-rw-   0        0        0    12167 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/infer_framework/triton/client_http.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:34:38.039387 zhousf-lib-1.5.7/zhousflib/locust/
+-rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/locust/__init__.py
+-rw-rw-rw-   0        0        0     1525 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/locust/locust_demo.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:34:38.069054 zhousf-lib-1.5.7/zhousflib/metrics/
+-rw-rw-rw-   0        0        0       76 2024-02-29 06:32:37.000000 zhousf-lib-1.5.7/zhousflib/metrics/__init__.py
+-rw-rw-rw-   0        0        0     1360 2024-05-28 02:20:06.000000 zhousf-lib-1.5.7/zhousflib/metrics/cosine.py
+-rw-rw-rw-   0        0        0     3429 2024-03-25 07:21:21.000000 zhousf-lib-1.5.7/zhousflib/metrics/f_score.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:34:38.125622 zhousf-lib-1.5.7/zhousflib/ml/
+-rw-rw-rw-   0        0        0       99 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/ml/__init__.py
+-rw-rw-rw-   0        0        0     4515 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/ml/feature_vector.py
+-rw-rw-rw-   0        0        0     8568 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/ml/model_base.py
+-rw-rw-rw-   0        0        0     2923 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/ml/model_cluster.py
+-rw-rw-rw-   0        0        0    10995 2024-01-31 01:40:34.000000 zhousf-lib-1.5.7/zhousflib/ml/model_gbdt.py
+-rw-rw-rw-   0        0        0     7630 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/ml/model_lr.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:34:38.147622 zhousf-lib-1.5.7/zhousflib/pandas/
+-rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/pandas/__init__.py
+-rw-rw-rw-   0        0        0     4839 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/pandas/openpyxl_util.py
+-rw-rw-rw-   0        0        0     6180 2024-04-01 06:42:29.000000 zhousf-lib-1.5.7/zhousflib/pandas/pandas_util.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:34:38.172413 zhousf-lib-1.5.7/zhousflib/pdf/
+-rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/pdf/__init__.py
+-rw-rw-rw-   0        0        0     1847 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/pdf/export_image.py
+-rw-rw-rw-   0        0        0     1465 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/pdf/pdfplumber_util.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:34:38.190414 zhousf-lib-1.5.7/zhousflib/so/
+-rw-rw-rw-   0        0        0       85 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/so/__init__.py
+-rw-rw-rw-   0        0        0     3840 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/so/project_to_so.py
+-rw-rw-rw-   0        0        0      286 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/so/py_to_so.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:34:38.193415 zhousf-lib-1.5.7/zhousflib/text/
+-rw-rw-rw-   0        0        0       87 2024-01-31 01:12:08.000000 zhousf-lib-1.5.7/zhousflib/text/__init__.py
+-rw-rw-rw-   0        0        0     3141 2024-02-29 06:26:47.000000 zhousf-lib-1.5.7/zhousflib/text/similarity.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:34:38.213581 zhousf-lib-1.5.7/zhousflib/thread/
+-rw-rw-rw-   0        0        0       60 2024-04-01 07:09:10.000000 zhousf-lib-1.5.7/zhousflib/thread/__init__.py
+-rw-rw-rw-   0        0        0     2318 2024-04-08 01:21:36.000000 zhousf-lib-1.5.7/zhousflib/thread/thread_util.py
+-rw-rw-rw-   0        0        0      829 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/thread/threadpool_util.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:34:38.232555 zhousf-lib-1.5.7/zhousflib/time/
+-rw-rw-rw-   0        0        0     1159 2024-03-25 07:19:09.000000 zhousf-lib-1.5.7/zhousflib/time/__init__.py
+-rw-rw-rw-   0        0        0     4671 2024-03-25 07:18:11.000000 zhousf-lib-1.5.7/zhousflib/time/time_util.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:34:38.363448 zhousf-lib-1.5.7/zhousflib/util/
+-rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/util/__init__.py
+-rw-rw-rw-   0        0        0     3143 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/util/calculater_util.py
+-rw-rw-rw-   0        0        0     2161 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/util/char_util.py
+-rw-rw-rw-   0        0        0     2703 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/util/dict_util.py
+-rw-rw-rw-   0        0        0     2195 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/util/encrypt_util.py
+-rw-rw-rw-   0        0        0    13480 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/util/iou_util.py
+-rw-rw-rw-   0        0        0     3373 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/util/json_util.py
+-rw-rw-rw-   0        0        0     5241 2024-04-29 05:35:07.000000 zhousf-lib-1.5.7/zhousflib/util/list_util.py
+-rw-rw-rw-   0        0        0     1481 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/util/math_util.py
+-rw-rw-rw-   0        0        0    15970 2024-05-29 09:11:09.000000 zhousf-lib-1.5.7/zhousflib/util/ocr_vis_util.py
+-rw-rw-rw-   0        0        0     1358 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/util/permission_util.py
+-rw-rw-rw-   0        0        0     3796 2024-05-23 06:24:29.000000 zhousf-lib-1.5.7/zhousflib/util/poly_util.py
+-rw-rw-rw-   0        0        0      527 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/util/random_util.py
+-rw-rw-rw-   0        0        0     4692 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/util/re_util.py
+-rw-rw-rw-   0        0        0      520 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/util/singleton.py
+-rw-rw-rw-   0        0        0     5122 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/util/string_util.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:34:38.407332 zhousf-lib-1.5.7/zhousflib/web/
+-rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/web/__init__.py
+-rw-rw-rw-   0        0        0     4246 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/web/config.py
+-rw-rw-rw-   0        0        0     1200 2024-03-21 07:56:35.000000 zhousf-lib-1.5.7/zhousflib/web/fast_api.py
+-rw-rw-rw-   0        0        0     3107 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/web/log_util.py
+-rw-rw-rw-   0        0        0     4497 2024-05-09 02:53:54.000000 zhousf-lib-1.5.7/zhousflib/web/logger.py
+-rw-rw-rw-   0        0        0     1340 2024-01-23 07:44:48.000000 zhousf-lib-1.5.7/zhousflib/web/response.py
+-rw-rw-rw-   0        0        0     6913 2024-04-01 08:27:11.000000 zhousf-lib-1.5.7/zhousflib/web/web.py
```

### Comparing `zhousf-lib-1.5.6/LICENSE` & `zhousf-lib-1.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/PKG-INFO` & `zhousf-lib-1.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhousf-lib
-Version: 1.5.6
+Version: 1.5.7
 Summary: a python library of zhousf
 Home-page: https://github.com/MrZhousf/ZhousfLib
 Author: zhousf
 Author-email: 442553199@qq.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `zhousf-lib-1.5.6/README.md` & `zhousf-lib-1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/setup.py` & `zhousf-lib-1.5.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 # 打包：python setup.py upload
 NAME = 'zhousf-lib'
 DESCRIPTION = 'a python library of zhousf'
 URL = 'https://github.com/MrZhousf/ZhousfLib'
 EMAIL = '442553199@qq.com'
 AUTHOR = 'zhousf'
 REQUIRES_PYTHON = '>=3.6.13'
-VERSION = '1.5.6'
+VERSION = '1.5.7'
 PACKAGE_DATA = {'': ['*.yaml', '*.ttf', '*.txt', '*.md']}
 
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 # What packages are required for this module to be executed?
```

### Comparing `zhousf-lib-1.5.6/zhousf_lib.egg-info/PKG-INFO` & `zhousf-lib-1.5.7/zhousf_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhousf-lib
-Version: 1.5.6
+Version: 1.5.7
 Summary: a python library of zhousf
 Home-page: https://github.com/MrZhousf/ZhousfLib
 Author: zhousf
 Author-email: 442553199@qq.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `zhousf-lib-1.5.6/zhousf_lib.egg-info/SOURCES.txt` & `zhousf-lib-1.5.7/zhousf_lib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -54,25 +54,27 @@
 zhousflib/image/nms_util.py
 zhousflib/image/op.py
 zhousflib/image/pil_util.py
 zhousflib/image/similarity.py
 zhousflib/infer_framework/__init__.py
 zhousflib/infer_framework/fast_infer/__init__.py
 zhousflib/infer_framework/fast_infer/backend.py
+zhousflib/infer_framework/fast_infer/backend_fastdeploy.py
 zhousflib/infer_framework/fast_infer/backend_http.py
 zhousflib/infer_framework/fast_infer/backend_onnx.py
 zhousflib/infer_framework/fast_infer/backend_original.py
 zhousflib/infer_framework/fast_infer/backend_tensorrt.py
 zhousflib/infer_framework/fast_infer/backend_torch_script.py
 zhousflib/infer_framework/fast_infer/fast_infer.py
 zhousflib/infer_framework/triton/__init__.py
 zhousflib/infer_framework/triton/client_http.py
 zhousflib/locust/__init__.py
 zhousflib/locust/locust_demo.py
 zhousflib/metrics/__init__.py
+zhousflib/metrics/cosine.py
 zhousflib/metrics/f_score.py
 zhousflib/ml/__init__.py
 zhousflib/ml/feature_vector.py
 zhousflib/ml/model_base.py
 zhousflib/ml/model_cluster.py
 zhousflib/ml/model_gbdt.py
 zhousflib/ml/model_lr.py
@@ -97,14 +99,15 @@
 zhousflib/util/char_util.py
 zhousflib/util/dict_util.py
 zhousflib/util/encrypt_util.py
 zhousflib/util/iou_util.py
 zhousflib/util/json_util.py
 zhousflib/util/list_util.py
 zhousflib/util/math_util.py
+zhousflib/util/ocr_vis_util.py
 zhousflib/util/permission_util.py
 zhousflib/util/poly_util.py
 zhousflib/util/random_util.py
 zhousflib/util/re_util.py
 zhousflib/util/singleton.py
 zhousflib/util/string_util.py
 zhousflib/web/__init__.py
```

### Comparing `zhousf-lib-1.5.6/zhousflib/ann/__init__.py` & `zhousf-lib-1.5.7/zhousflib/ann/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/ann/onnx/__init__.py` & `zhousf-lib-1.5.7/zhousflib/ann/onnx/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/ann/onnx/onnx_to_trt.py` & `zhousf-lib-1.5.7/zhousflib/ann/onnx/onnx_to_trt.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/ann/tensorrt/tensorrt_infer.py` & `zhousf-lib-1.5.7/zhousflib/ann/tensorrt/tensorrt_infer.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/ann/torch/__init__.py` & `zhousf-lib-1.5.7/zhousflib/ann/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/ann/torch/torch_to_onnx.py` & `zhousf-lib-1.5.7/zhousflib/ann/torch/torch_to_onnx.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/ann/torch/torch_to_script.py` & `zhousf-lib-1.5.7/zhousflib/ann/torch/torch_to_script.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/ann/transformers/__init__.py` & `zhousf-lib-1.5.7/zhousflib/ann/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/database/lmdb_master.py` & `zhousf-lib-1.5.7/zhousflib/database/lmdb_master.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/database/tinydb_master.py` & `zhousf-lib-1.5.7/zhousflib/database/tinydb_master.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/datasets/classification/classification_dataset_split.py` & `zhousf-lib-1.5.7/zhousflib/datasets/classification/classification_dataset_split.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/datasets/coco/__init__.py` & `zhousf-lib-1.5.7/zhousflib/datasets/coco/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/datasets/coco/coco_bbox_extract.py` & `zhousf-lib-1.5.7/zhousflib/datasets/coco/coco_bbox_extract.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/datasets/coco/coco_bbox_update.py` & `zhousf-lib-1.5.7/zhousflib/datasets/coco/coco_bbox_update.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/datasets/coco/coco_bbox_vis.py` & `zhousf-lib-1.5.7/zhousflib/datasets/coco/coco_bbox_vis.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/datasets/coco/coco_dataset_merge.py` & `zhousf-lib-1.5.7/zhousflib/datasets/coco/coco_dataset_merge.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/datasets/coco/coco_dataset_split.py` & `zhousf-lib-1.5.7/zhousflib/datasets/coco/coco_dataset_split.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/datasets/labelme/__init__.py` & `zhousf-lib-1.5.7/zhousflib/datasets/labelme/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/datasets/labelme/labelme_bbox_update.py` & `zhousf-lib-1.5.7/zhousflib/datasets/labelme/labelme_bbox_update.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/datasets/labelme/labelme_clip.py` & `zhousf-lib-1.5.7/zhousflib/datasets/labelme/labelme_clip.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/datasets/labelme/labelme_convert_coco.py` & `zhousf-lib-1.5.7/zhousflib/datasets/labelme/labelme_convert_coco.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/datasets/labelme/labelme_convert_seg.py` & `zhousf-lib-1.5.7/zhousflib/datasets/labelme/labelme_convert_seg.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/datasets/labelme/labelme_convert_uiex.py` & `zhousf-lib-1.5.7/zhousflib/datasets/labelme/labelme_convert_uiex.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/datasets/labelme/labelme_dataset_clip.py` & `zhousf-lib-1.5.7/zhousflib/datasets/labelme/labelme_dataset_clip.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/datasets/labelme/shape_convert.py` & `zhousf-lib-1.5.7/zhousflib/datasets/labelme/shape_convert.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/datasets/segmentation/seg_dataset_split.py` & `zhousf-lib-1.5.7/zhousflib/datasets/segmentation/seg_dataset_split.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/decorator/interceptor_util.py` & `zhousf-lib-1.5.7/zhousflib/decorator/interceptor_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/file/__init__.py` & `zhousf-lib-1.5.7/zhousflib/file/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/file/delete_file.py` & `zhousf-lib-1.5.7/zhousflib/file/delete_file.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/file/download.py` & `zhousf-lib-1.5.7/zhousflib/file/download.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/file/zip_util.py` & `zhousf-lib-1.5.7/zhousflib/file/zip_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/font/SimSun.ttf` & `zhousf-lib-1.5.7/zhousflib/font/SimSun.ttf`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/font/Symbola.ttf` & `zhousf-lib-1.5.7/zhousflib/font/Symbola.ttf`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/font/__init__.py` & `zhousf-lib-1.5.7/zhousflib/font/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/image/__init__.py` & `zhousf-lib-1.5.7/zhousflib/image/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/image/cv.py` & `zhousf-lib-1.5.7/zhousflib/image/cv.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/image/cv_util.py` & `zhousf-lib-1.5.7/zhousflib/image/cv_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/image/img_util.py` & `zhousf-lib-1.5.7/zhousflib/image/img_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/image/nms_util.py` & `zhousf-lib-1.5.7/zhousflib/image/nms_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/image/op.py` & `zhousf-lib-1.5.7/zhousflib/image/op.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/image/pil_util.py` & `zhousf-lib-1.5.7/zhousflib/image/pil_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     x_min = min(arr[:, 0])
     y_min = min(arr[:, 1])
     x_max = max(arr[:, 0])
     y_max = max(arr[:, 1])
     return x_min, y_min, x_max, y_max
 
 
-def draw_rectangle(bbox: list, image_file: Path = None, image_size: list = None, font = None,
+def draw_rectangle(bbox: list, image_file: Path = None, image_size: list = None, font=None,
                    fill_transparent=255, show=True):
     """
     绘制矩形框
     :param bbox: [(label, x_min, y_min, x_max, y_max)]
     :param image_file: 空时以空白为背景进行绘制
     :param image_size:
     :param font: ImageFont.truetype(font_path, font_size, encoding="utf-8")
@@ -54,38 +54,43 @@
     :param image_file:
     :return:
     """
     image = Image.open(image_file)
     return [image.width, image.height]
 
 
-def draw_polygon(polygon: list, image_file: Path = None, image_size: list = None, font = None,
+def draw_polygon(polygon: list, image_file=None, image_size: list = None, font=None,
                  texts: list = None, fill_transparent=255, show=True):
     """
     绘制四边形
     :param polygon: [[[255, 376], [291, 409], [255, 443], [218, 409]], [[252, 140], [300, 140], [300, 189], [252, 189]]]
     :param image_file: 空时以空白为背景进行绘制
     :param image_size:
     :param font: ImageFont.truetype(font_path, font_size, encoding="utf-8")
     :param texts: box框的描述文本，长度等于polygon
     :param fill_transparent: 填充色透明度[0, 255]，当为-1时则不填充
     :param show:
     :return:
     """
+    import colorsys
+    from PIL import Image, ImageDraw
     hsv_tuples = [(1.0 * x / len(polygon), 1., 1.) for x in range(len(polygon))]
     colors = list(map(lambda x: colorsys.hsv_to_rgb(*x), hsv_tuples))
     colors = list(map(lambda x: (int(x[0] * 255), int(x[1] * 255), int(x[2] * 255)), colors))
     image_white = None
     if image_size is None:
         image_size = [500, 500]
     if image_file is None:
         image = Image.new('RGBA', (image_size[0], image_size[1]), (255, 255, 255))
         draw = ImageDraw.ImageDraw(image)
     else:
-        image = Image.open(image_file)
+        if isinstance(image_file, Path) or isinstance(image_file, str):
+            image = Image.open(image_file)
+        else:
+            image = Image.fromarray(image_file)
         if image.mode != "RGBA":
             image = image.convert('RGBA')
         image_white = Image.new('RGBA', (image.width, image.height), (255, 255, 255, 0))
         draw = ImageDraw.ImageDraw(image_white)
     for index, point in enumerate(polygon):
         draw_p = [(p[0], p[1]) for p in point]
         # 边框颜色
@@ -101,14 +106,16 @@
             draw.text(xy=(draw_p[0][0]+1, draw_p[0][1]+1), text=text, fill="black", font=font)
         else:
             draw.text(xy=(draw_p[0][0] + 1, draw_p[0][1] + 1), text=text, fill="black")
     if image_white is not None:
         image.paste(Image.alpha_composite(image, image_white))
     if show:
         image.show()
+    if image.mode == "RGBA":
+        image = image.convert('RGB')
     return image
 
 
 if __name__ == "__main__":
     # draw_rectangle([(218, 376, 291, 443)])
     draw_polygon([[[255, 376], [291, 409], [255, 443], [218, 409]], [[252, 140], [300, 140], [300, 189], [252, 189]]])
     pass
```

### Comparing `zhousf-lib-1.5.6/zhousflib/image/similarity.py` & `zhousf-lib-1.5.7/zhousflib/image/similarity.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/infer_framework/fast_infer/backend.py` & `zhousf-lib-1.5.7/zhousflib/infer_framework/fast_infer/backend.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,24 +12,29 @@
         pass
 
     @abc.abstractmethod
     def build(self, **kwargs):
         pass
 
     @abc.abstractmethod
-    def inference(self, inputs_list: list):
+    def inference(self, input_data, **kwargs):
         pass
 
     @staticmethod
     def to_numpy(tensor):
         return tensor.detach().cpu().numpy() if tensor.requires_grad else tensor.cpu().numpy()
 
     @staticmethod
     def get_file_by_suffix(model_dir: Path, suffix: str):
         return [file for file in model_dir.glob("*{0}".format(suffix))]
 
     @staticmethod
+    def get_file_path_by_suffix(model_dir: Path, suffix: str):
+        files = [str(file) for file in model_dir.glob("*{0}".format(suffix))]
+        return files[0] if len(files) > 0 else files
+
+    @staticmethod
     def pop(kwargs: dict, key: str):
         if len(kwargs) == 0 or len(key) == 0:
             return
         if key in kwargs:
             kwargs.pop(key)
```

### Comparing `zhousf-lib-1.5.6/zhousflib/infer_framework/fast_infer/backend_http.py` & `zhousf-lib-1.5.7/zhousflib/infer_framework/fast_infer/backend_http.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,18 +42,18 @@
         assert self.model_name is not None, "设置http后端时，model_name不能为空."
         assert self.model_version is not None, "设置http后端时，model_version不能为空."
 
         concurrency = kwargs.get("concurrency", 1)
         from zhousflib.infer_framework.triton import client_http
         self.model = client_http.ClientHttp(url=url, concurrency=concurrency, **kwargs)
 
-    def inference(self, inputs_list: list):
+    def inference(self, input_data, **kwargs):
         inputs = []
-        for i, input_ in enumerate(inputs_list):
-            inputs.append(self.to_numpy(inputs_list[i].int()))
+        for i, input_ in enumerate(input_data):
+            inputs.append(self.to_numpy(input_data[i].int()))
         # INT8|INT16|INT32|INT64|UINT8|UINT16|UINT32|UINT64|FP16|FP32|FP64
         d_type = self.http_inputs[0][1]
         if d_type == "INT16":
             data_arr = np.asarray(inputs, dtype=np.int16)
         elif d_type == "INT32":
             data_arr = np.asarray(inputs, dtype=np.int32)
         elif d_type == "INT64":
```

### Comparing `zhousf-lib-1.5.6/zhousflib/infer_framework/fast_infer/backend_onnx.py` & `zhousf-lib-1.5.7/zhousflib/infer_framework/fast_infer/backend_onnx.py`

 * *Files 10% similar despite different names*

```diff
@@ -66,13 +66,13 @@
 
         if kwargs.get("autoload", True):
             from zhousflib.ann.torch import torch_to_onnx
             self.model, _, _ = torch_to_onnx.load_onnx(self.model_dir, device_id=self.device_id, autoload_weights=False, autoload_tokenizer=False)
         print("加载onnx成功：{0}.".format(target_files[0]))
         return target_files[0]
 
-    def inference(self, inputs_list: list):
+    def inference(self, input_data, **kwargs):
         feed = {}
-        for i, input_ in enumerate(inputs_list):
-            feed[self.model.get_inputs()[i].name] = self.to_numpy(inputs_list[i])
+        for i, input_ in enumerate(input_data):
+            feed[self.model.get_inputs()[i].name] = self.to_numpy(input_data[i])
         result = self.model.run(None, feed)
         return result[0]
```

### Comparing `zhousf-lib-1.5.6/zhousflib/infer_framework/fast_infer/backend_tensorrt.py` & `zhousf-lib-1.5.7/zhousflib/infer_framework/fast_infer/backend_tensorrt.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,13 +58,13 @@
         if kwargs.get("autoload", True):
             from zhousflib.ann.tensorrt import tensorrt_infer
             self.model = tensorrt_infer.RTInfer(trt_file_path=self.model_dir.joinpath("model.trt"),
                                                 device_id=self.device_id, use_stack=True)
             print("加载tensorrt成功：{0}.".format(target_files[0]))
         return target_files[0]
 
-    def inference(self, inputs_list: list):
+    def inference(self, input_data, **kwargs):
         inputs = []
-        for i, input_ in enumerate(inputs_list):
-            inputs.append(self.to_numpy(inputs_list[i].int()))
+        for i, input_ in enumerate(input_data):
+            inputs.append(self.to_numpy(input_data[i].int()))
         result = self.model.infer(input_arr=np.asarray(inputs))
         return result[0]
```

### Comparing `zhousf-lib-1.5.6/zhousflib/infer_framework/fast_infer/backend_torch_script.py` & `zhousf-lib-1.5.7/zhousflib/infer_framework/fast_infer/backend_torch_script.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,12 +50,12 @@
 
         if kwargs.get("autoload", True):
             from zhousflib.ann.torch import torch_to_script
             self.model, _, _ = torch_to_script.load_script_model(self.model_dir, device_id=self.device_id)
             print("加载torchscript成功：{0}.".format(target_files[0]))
         return target_files[0]
 
-    def inference(self, inputs_list: list):
+    def inference(self, input_data, **kwargs):
         inputs = []
-        for i, input_ in enumerate(inputs_list):
-            inputs.append(inputs_list[i].squeeze(1).to(self.device))
+        for i, input_ in enumerate(input_data):
+            inputs.append(input_data[i].squeeze(1).to(self.device))
         return self.model(inputs)
```

### Comparing `zhousf-lib-1.5.6/zhousflib/infer_framework/triton/__init__.py` & `zhousf-lib-1.5.7/zhousflib/infer_framework/triton/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/infer_framework/triton/client_http.py` & `zhousf-lib-1.5.7/zhousflib/infer_framework/triton/client_http.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/locust/locust_demo.py` & `zhousf-lib-1.5.7/zhousflib/locust/locust_demo.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/metrics/f_score.py` & `zhousf-lib-1.5.7/zhousflib/metrics/f_score.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/ml/feature_vector.py` & `zhousf-lib-1.5.7/zhousflib/ml/feature_vector.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/ml/model_base.py` & `zhousf-lib-1.5.7/zhousflib/ml/model_base.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/ml/model_cluster.py` & `zhousf-lib-1.5.7/zhousflib/ml/model_cluster.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/ml/model_gbdt.py` & `zhousf-lib-1.5.7/zhousflib/ml/model_gbdt.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/ml/model_lr.py` & `zhousf-lib-1.5.7/zhousflib/ml/model_lr.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/pandas/openpyxl_util.py` & `zhousf-lib-1.5.7/zhousflib/pandas/openpyxl_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/pandas/pandas_util.py` & `zhousf-lib-1.5.7/zhousflib/pandas/pandas_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/pdf/export_image.py` & `zhousf-lib-1.5.7/zhousflib/pdf/export_image.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/pdf/pdfplumber_util.py` & `zhousf-lib-1.5.7/zhousflib/pdf/pdfplumber_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/so/project_to_so.py` & `zhousf-lib-1.5.7/zhousflib/so/project_to_so.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/text/similarity.py` & `zhousf-lib-1.5.7/zhousflib/text/similarity.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/thread/thread_util.py` & `zhousf-lib-1.5.7/zhousflib/thread/thread_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/thread/threadpool_util.py` & `zhousf-lib-1.5.7/zhousflib/thread/threadpool_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/time/__init__.py` & `zhousf-lib-1.5.7/zhousflib/time/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/time/time_util.py` & `zhousf-lib-1.5.7/zhousflib/time/time_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/util/calculater_util.py` & `zhousf-lib-1.5.7/zhousflib/util/calculater_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/util/char_util.py` & `zhousf-lib-1.5.7/zhousflib/util/char_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/util/dict_util.py` & `zhousf-lib-1.5.7/zhousflib/util/dict_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/util/encrypt_util.py` & `zhousf-lib-1.5.7/zhousflib/util/encrypt_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/util/iou_util.py` & `zhousf-lib-1.5.7/zhousflib/util/iou_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/util/json_util.py` & `zhousf-lib-1.5.7/zhousflib/util/json_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/util/list_util.py` & `zhousf-lib-1.5.7/zhousflib/util/list_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/util/math_util.py` & `zhousf-lib-1.5.7/zhousflib/util/math_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/util/permission_util.py` & `zhousf-lib-1.5.7/zhousflib/util/permission_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/util/poly_util.py` & `zhousf-lib-1.5.7/zhousflib/util/poly_util.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # @Author  : zhousf
 # @Function:
 import numpy as np
 
 import matplotlib.pyplot as plt
 import matplotlib.patches as mpathes
 from shapely import geometry
+from shapely.geometry import Polygon
 
 
 def in_poly(poly, point):
     """
     判断点是否在poly内，不包含poly边界
     :param poly: 多边形点坐标：[(0, 0), (1, 0), (1, 1), (0, 1)]
     :param point: 点坐标：(0.1, 0.5)
@@ -86,20 +87,31 @@
         poly = [(x_min, y_min), (x_max, y_min), (x_max, y_max), (x_min, y_max)]
         # 判断点是否在poly内，不包含poly边界
         if in_poly(poly=poly, point=point):
             return box
     return None
 
 
+def poly_area(points: list):
+    """
+    计算多边形的面积
+    :param points:
+    :return:
+    """
+    poly = Polygon(points)
+    return poly.area
+
+
 if __name__ == "__main__":
     # 判断点是否在poly内
     # poly = [(0, 0), (1, 0), (1, 1), (0, 1)]  # 多边形坐标
     # pt2 = (0.1, 0.5)  # 点坐标
     # print(in_poly(square, pt1))
     # 按照w,h对box进行网格划分
-    boxes_ = make_mesh([0, 0, 4000, 5000], 1280, 1280, show=True)
-    for box in boxes_:
-        print(box)
+    # boxes_ = make_mesh([0, 0, 4000, 5000], 1280, 1280, show=True)
+    # for box in boxes_:
+    #     print(box)
         # [(column_index, row_index, x_min, y_min, x_max, y_max)]
     # 查询点在哪个box中
     # query_box_position(boxes=boxes_, point=(1, 1))
+    print(poly_area([(0, 0), (0, 10), (10, 10), (10, 0)]))
     pass
```

### Comparing `zhousf-lib-1.5.6/zhousflib/util/random_util.py` & `zhousf-lib-1.5.7/zhousflib/util/random_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/util/re_util.py` & `zhousf-lib-1.5.7/zhousflib/util/re_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/util/singleton.py` & `zhousf-lib-1.5.7/zhousflib/util/singleton.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/util/string_util.py` & `zhousf-lib-1.5.7/zhousflib/util/string_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/web/config.py` & `zhousf-lib-1.5.7/zhousflib/web/config.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/web/fast_api.py` & `zhousf-lib-1.5.7/zhousflib/web/fast_api.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/web/log_util.py` & `zhousf-lib-1.5.7/zhousflib/web/log_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/web/logger.py` & `zhousf-lib-1.5.7/zhousflib/web/logger.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/web/response.py` & `zhousf-lib-1.5.7/zhousflib/web/response.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.6/zhousflib/web/web.py` & `zhousf-lib-1.5.7/zhousflib/web/web.py`

 * *Files identical despite different names*

