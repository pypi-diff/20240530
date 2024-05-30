# Comparing `tmp/luma-ml-0.8.2.tar.gz` & `tmp/luma-ml-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luma-ml-0.8.2.tar", last modified: Sun May 26 19:19:09 2024, max compression
+gzip compressed data, was "luma-ml-0.9.0.tar", last modified: Thu May 30 20:01:40 2024, max compression
```

## Comparing `luma-ml-0.8.2.tar` & `luma-ml-0.9.0.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.881916 luma-ml-0.8.2/
--rw-r--r--   0 chanlee    (501) staff       (20)    35149 2023-11-07 13:17:31.000000 luma-ml-0.8.2/LICENSE
--rw-r--r--   0 chanlee    (501) staff       (20)     5554 2024-05-26 19:19:09.881562 luma-ml-0.8.2/PKG-INFO
--rw-r--r--   0 chanlee    (501) staff       (20)     4948 2024-05-26 19:18:32.000000 luma-ml-0.8.2/README.md
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.865170 luma-ml-0.8.2/luma/
--rw-r--r--   0 chanlee    (501) staff       (20)    11481 2024-05-26 12:21:52.000000 luma-ml-0.8.2/luma/__import__.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1502 2024-05-26 11:11:06.000000 luma-ml-0.8.2/luma/__init__.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.866495 luma-ml-0.8.2/luma/classifier/
--rw-r--r--   0 chanlee    (501) staff       (20)    12563 2024-05-13 11:38:17.000000 luma-ml-0.8.2/luma/classifier/discriminant.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7935 2024-05-13 11:35:13.000000 luma-ml-0.8.2/luma/classifier/logistic.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5541 2024-05-23 16:46:06.000000 luma-ml-0.8.2/luma/classifier/naive_bayes.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9070 2024-05-13 11:30:20.000000 luma-ml-0.8.2/luma/classifier/neighbors.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9174 2024-05-13 11:33:07.000000 luma-ml-0.8.2/luma/classifier/svm.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9806 2024-05-13 11:36:04.000000 luma-ml-0.8.2/luma/classifier/tree.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.868006 luma-ml-0.8.2/luma/clustering/
--rw-r--r--   0 chanlee    (501) staff       (20)    18057 2024-05-13 11:42:50.000000 luma-ml-0.8.2/luma/clustering/affinity.py
--rw-r--r--   0 chanlee    (501) staff       (20)    17889 2024-05-13 11:50:11.000000 luma-ml-0.8.2/luma/clustering/density.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7697 2024-05-13 11:51:42.000000 luma-ml-0.8.2/luma/clustering/hierarchy.py
--rw-r--r--   0 chanlee    (501) staff       (20)    18307 2024-05-13 11:55:03.000000 luma-ml-0.8.2/luma/clustering/kmeans.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8192 2024-05-13 11:55:57.000000 luma-ml-0.8.2/luma/clustering/mixture.py
--rw-r--r--   0 chanlee    (501) staff       (20)    11602 2024-05-13 11:57:37.000000 luma-ml-0.8.2/luma/clustering/spectral.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.868744 luma-ml-0.8.2/luma/core/
--rw-r--r--   0 chanlee    (501) staff       (20)     5924 2024-05-13 11:58:02.000000 luma-ml-0.8.2/luma/core/base.py
--rw-r--r--   0 chanlee    (501) staff       (20)      446 2024-05-13 11:58:51.000000 luma-ml-0.8.2/luma/core/main.py
--rw-r--r--   0 chanlee    (501) staff       (20)    11013 2024-05-13 12:05:21.000000 luma-ml-0.8.2/luma/core/super.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.870212 luma-ml-0.8.2/luma/ensemble/
--rw-r--r--   0 chanlee    (501) staff       (20)    10046 2024-05-13 12:09:42.000000 luma-ml-0.8.2/luma/ensemble/bagging.py
--rw-r--r--   0 chanlee    (501) staff       (20)    19721 2024-05-13 12:15:52.000000 luma-ml-0.8.2/luma/ensemble/boost.py
--rw-r--r--   0 chanlee    (501) staff       (20)    10280 2024-05-13 12:20:38.000000 luma-ml-0.8.2/luma/ensemble/forest.py
--rw-r--r--   0 chanlee    (501) staff       (20)    14109 2024-05-13 12:31:18.000000 luma-ml-0.8.2/luma/ensemble/stack.py
--rw-r--r--   0 chanlee    (501) staff       (20)     6779 2024-05-13 12:36:00.000000 luma-ml-0.8.2/luma/ensemble/vote.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.871143 luma-ml-0.8.2/luma/interface/
--rw-r--r--   0 chanlee    (501) staff       (20)     1294 2024-05-13 12:36:06.000000 luma-ml-0.8.2/luma/interface/exception.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7413 2024-05-17 07:30:53.000000 luma-ml-0.8.2/luma/interface/typing.py
--rw-r--r--   0 chanlee    (501) staff       (20)    16195 2024-05-13 15:45:21.000000 luma-ml-0.8.2/luma/interface/util.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.871908 luma-ml-0.8.2/luma/metric/
--rw-r--r--   0 chanlee    (501) staff       (20)     1654 2024-04-24 15:30:21.000000 luma-ml-0.8.2/luma/metric/classification.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5917 2024-05-13 15:46:55.000000 luma-ml-0.8.2/luma/metric/clustering.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1788 2024-05-13 15:46:57.000000 luma-ml-0.8.2/luma/metric/distance.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1842 2024-05-13 15:46:59.000000 luma-ml-0.8.2/luma/metric/regression.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.872079 luma-ml-0.8.2/luma/migrate/
--rw-r--r--   0 chanlee    (501) staff       (20)     3764 2024-05-13 16:18:47.000000 luma-ml-0.8.2/luma/migrate/port.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.872809 luma-ml-0.8.2/luma/model_selection/
--rw-r--r--   0 chanlee    (501) staff       (20)     3438 2024-05-13 16:20:58.000000 luma-ml-0.8.2/luma/model_selection/cv.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8041 2024-05-13 16:29:29.000000 luma-ml-0.8.2/luma/model_selection/fold.py
--rw-r--r--   0 chanlee    (501) staff       (20)    12244 2024-05-13 16:35:00.000000 luma-ml-0.8.2/luma/model_selection/search.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5736 2024-05-13 16:40:23.000000 luma-ml-0.8.2/luma/model_selection/split.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.874312 luma-ml-0.8.2/luma/neural/
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.875392 luma-ml-0.8.2/luma/neural/_layers/
--rw-r--r--   0 chanlee    (501) staff       (20)     6748 2024-05-12 09:16:35.000000 luma-ml-0.8.2/luma/neural/_layers/_act.py
--rw-r--r--   0 chanlee    (501) staff       (20)    19314 2024-05-26 11:53:00.000000 luma-ml-0.8.2/luma/neural/_layers/_conv.py
--rw-r--r--   0 chanlee    (501) staff       (20)     4144 2024-05-23 16:58:05.000000 luma-ml-0.8.2/luma/neural/_layers/_drop.py
--rw-r--r--   0 chanlee    (501) staff       (20)     2313 2024-05-12 09:17:05.000000 luma-ml-0.8.2/luma/neural/_layers/_linear.py
--rw-r--r--   0 chanlee    (501) staff       (20)    10790 2024-05-16 17:20:47.000000 luma-ml-0.8.2/luma/neural/_layers/_norm.py
--rw-r--r--   0 chanlee    (501) staff       (20)    29777 2024-05-26 11:24:51.000000 luma-ml-0.8.2/luma/neural/_layers/_pool.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.876366 luma-ml-0.8.2/luma/neural/_models/
--rw-r--r--   0 chanlee    (501) staff       (20)    13100 2024-05-18 09:06:30.000000 luma-ml-0.8.2/luma/neural/_models/_alex.py
--rw-r--r--   0 chanlee    (501) staff       (20)     6471 2024-05-26 12:18:12.000000 luma-ml-0.8.2/luma/neural/_models/_inception.py
--rw-r--r--   0 chanlee    (501) staff       (20)    12758 2024-05-17 07:23:08.000000 luma-ml-0.8.2/luma/neural/_models/_lenet.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9639 2024-05-17 07:21:18.000000 luma-ml-0.8.2/luma/neural/_models/_simple.py
--rw-r--r--   0 chanlee    (501) staff       (20)    23945 2024-05-24 18:22:17.000000 luma-ml-0.8.2/luma/neural/_models/_vgg.py
--rw-r--r--   0 chanlee    (501) staff       (20)    12024 2024-05-13 17:00:56.000000 luma-ml-0.8.2/luma/neural/base.py
--rw-r--r--   0 chanlee    (501) staff       (20)    24180 2024-05-26 11:59:07.000000 luma-ml-0.8.2/luma/neural/block.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1319 2024-05-09 19:24:30.000000 luma-ml-0.8.2/luma/neural/init.py
--rw-r--r--   0 chanlee    (501) staff       (20)    33776 2024-05-26 11:55:46.000000 luma-ml-0.8.2/luma/neural/layer.py
--rw-r--r--   0 chanlee    (501) staff       (20)     3111 2024-05-13 19:10:16.000000 luma-ml-0.8.2/luma/neural/loss.py
--rw-r--r--   0 chanlee    (501) staff       (20)    46067 2024-05-26 19:16:21.000000 luma-ml-0.8.2/luma/neural/network.py
--rw-r--r--   0 chanlee    (501) staff       (20)    21132 2024-05-09 17:12:02.000000 luma-ml-0.8.2/luma/neural/optimizer.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8582 2024-05-13 19:27:55.000000 luma-ml-0.8.2/luma/neural/single.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.876636 luma-ml-0.8.2/luma/pipe/
--rw-r--r--   0 chanlee    (501) staff       (20)     7308 2024-05-13 19:32:18.000000 luma-ml-0.8.2/luma/pipe/pipeline.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.877357 luma-ml-0.8.2/luma/preprocessing/
--rw-r--r--   0 chanlee    (501) staff       (20)     5295 2024-04-21 11:36:14.000000 luma-ml-0.8.2/luma/preprocessing/encoder.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5533 2024-04-21 11:36:15.000000 luma-ml-0.8.2/luma/preprocessing/imputer.py
--rw-r--r--   0 chanlee    (501) staff       (20)     3653 2024-05-13 19:32:35.000000 luma-ml-0.8.2/luma/preprocessing/outlier.py
--rw-r--r--   0 chanlee    (501) staff       (20)     2624 2024-05-13 19:33:29.000000 luma-ml-0.8.2/luma/preprocessing/scaler.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.878150 luma-ml-0.8.2/luma/reduction/
--rw-r--r--   0 chanlee    (501) staff       (20)    19163 2024-05-26 19:19:09.000000 luma-ml-0.8.2/luma/reduction/linear.py
--rw-r--r--   0 chanlee    (501) staff       (20)    40387 2024-05-13 19:55:48.000000 luma-ml-0.8.2/luma/reduction/manifold.py
--rw-r--r--   0 chanlee    (501) staff       (20)    17019 2024-05-14 09:45:27.000000 luma-ml-0.8.2/luma/reduction/selection.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.879488 luma-ml-0.8.2/luma/regressor/
--rw-r--r--   0 chanlee    (501) staff       (20)    19882 2024-05-14 09:56:22.000000 luma-ml-0.8.2/luma/regressor/general.py
--rw-r--r--   0 chanlee    (501) staff       (20)    12687 2024-05-14 10:03:42.000000 luma-ml-0.8.2/luma/regressor/linear.py
--rw-r--r--   0 chanlee    (501) staff       (20)     6755 2024-05-14 10:04:13.000000 luma-ml-0.8.2/luma/regressor/neighbors.py
--rw-r--r--   0 chanlee    (501) staff       (20)     3098 2024-05-14 10:05:44.000000 luma-ml-0.8.2/luma/regressor/poly.py
--rw-r--r--   0 chanlee    (501) staff       (20)    11070 2024-05-14 14:33:09.000000 luma-ml-0.8.2/luma/regressor/robust.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7805 2024-05-14 14:45:46.000000 luma-ml-0.8.2/luma/regressor/svm.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7415 2024-05-14 14:59:17.000000 luma-ml-0.8.2/luma/regressor/tree.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.879838 luma-ml-0.8.2/luma/visual/
--rw-r--r--   0 chanlee    (501) staff       (20)     3045 2024-04-13 08:30:32.000000 luma-ml-0.8.2/luma/visual/eda.py
--rw-r--r--   0 chanlee    (501) staff       (20)    25027 2024-05-23 17:04:49.000000 luma-ml-0.8.2/luma/visual/eval.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.880727 luma-ml-0.8.2/luma_ml.egg-info/
--rw-r--r--   0 chanlee    (501) staff       (20)     5554 2024-05-26 19:19:09.000000 luma-ml-0.8.2/luma_ml.egg-info/PKG-INFO
--rw-r--r--   0 chanlee    (501) staff       (20)     2000 2024-05-26 19:19:09.000000 luma-ml-0.8.2/luma_ml.egg-info/SOURCES.txt
--rw-r--r--   0 chanlee    (501) staff       (20)        1 2024-05-26 19:19:09.000000 luma-ml-0.8.2/luma_ml.egg-info/dependency_links.txt
--rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-05-26 19:19:09.000000 luma-ml-0.8.2/luma_ml.egg-info/requires.txt
--rw-r--r--   0 chanlee    (501) staff       (20)       17 2024-05-26 19:19:09.000000 luma-ml-0.8.2/luma_ml.egg-info/top_level.txt
--rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-05-26 19:19:09.881987 luma-ml-0.8.2/setup.cfg
--rw-r--r--   0 chanlee    (501) staff       (20)      842 2024-05-26 19:18:56.000000 luma-ml-0.8.2/setup.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-26 19:19:09.881083 luma-ml-0.8.2/test/
--rw-r--r--   0 chanlee    (501) staff       (20)      647 2024-04-29 02:58:00.000000 luma-ml-0.8.2/test/__act.py
--rw-r--r--   0 chanlee    (501) staff       (20)      429 2024-05-18 16:19:55.000000 luma-ml-0.8.2/test/__test.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.036328 luma-ml-0.9.0/
+-rw-r--r--   0 chanlee    (501) staff       (20)    35149 2023-11-07 13:17:31.000000 luma-ml-0.9.0/LICENSE
+-rw-r--r--   0 chanlee    (501) staff       (20)     5554 2024-05-30 20:01:40.035961 luma-ml-0.9.0/PKG-INFO
+-rw-r--r--   0 chanlee    (501) staff       (20)     4948 2024-05-30 20:00:23.000000 luma-ml-0.9.0/README.md
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.004246 luma-ml-0.9.0/luma/
+-rw-r--r--   0 chanlee    (501) staff       (20)    11653 2024-05-30 16:18:18.000000 luma-ml-0.9.0/luma/__import__.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1502 2024-05-26 11:11:06.000000 luma-ml-0.9.0/luma/__init__.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.006842 luma-ml-0.9.0/luma/classifier/
+-rw-r--r--   0 chanlee    (501) staff       (20)    12563 2024-05-13 11:38:17.000000 luma-ml-0.9.0/luma/classifier/discriminant.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7935 2024-05-13 11:35:13.000000 luma-ml-0.9.0/luma/classifier/logistic.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5541 2024-05-23 16:46:06.000000 luma-ml-0.9.0/luma/classifier/naive_bayes.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9070 2024-05-13 11:30:20.000000 luma-ml-0.9.0/luma/classifier/neighbors.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9174 2024-05-13 11:33:07.000000 luma-ml-0.9.0/luma/classifier/svm.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9806 2024-05-13 11:36:04.000000 luma-ml-0.9.0/luma/classifier/tree.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.009974 luma-ml-0.9.0/luma/clustering/
+-rw-r--r--   0 chanlee    (501) staff       (20)    18057 2024-05-13 11:42:50.000000 luma-ml-0.9.0/luma/clustering/affinity.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    17889 2024-05-13 11:50:11.000000 luma-ml-0.9.0/luma/clustering/density.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7697 2024-05-13 11:51:42.000000 luma-ml-0.9.0/luma/clustering/hierarchy.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    18307 2024-05-13 11:55:03.000000 luma-ml-0.9.0/luma/clustering/kmeans.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8192 2024-05-13 11:55:57.000000 luma-ml-0.9.0/luma/clustering/mixture.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    11602 2024-05-13 11:57:37.000000 luma-ml-0.9.0/luma/clustering/spectral.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.011616 luma-ml-0.9.0/luma/core/
+-rw-r--r--   0 chanlee    (501) staff       (20)     5924 2024-05-13 11:58:02.000000 luma-ml-0.9.0/luma/core/base.py
+-rw-r--r--   0 chanlee    (501) staff       (20)      446 2024-05-13 11:58:51.000000 luma-ml-0.9.0/luma/core/main.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    11013 2024-05-13 12:05:21.000000 luma-ml-0.9.0/luma/core/super.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.014590 luma-ml-0.9.0/luma/ensemble/
+-rw-r--r--   0 chanlee    (501) staff       (20)    10046 2024-05-13 12:09:42.000000 luma-ml-0.9.0/luma/ensemble/bagging.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    19721 2024-05-13 12:15:52.000000 luma-ml-0.9.0/luma/ensemble/boost.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    10280 2024-05-13 12:20:38.000000 luma-ml-0.9.0/luma/ensemble/forest.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    14109 2024-05-13 12:31:18.000000 luma-ml-0.9.0/luma/ensemble/stack.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     6779 2024-05-13 12:36:00.000000 luma-ml-0.9.0/luma/ensemble/vote.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.015968 luma-ml-0.9.0/luma/interface/
+-rw-r--r--   0 chanlee    (501) staff       (20)     1294 2024-05-13 12:36:06.000000 luma-ml-0.9.0/luma/interface/exception.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7413 2024-05-17 07:30:53.000000 luma-ml-0.9.0/luma/interface/typing.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    16347 2024-05-27 18:40:22.000000 luma-ml-0.9.0/luma/interface/util.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.017330 luma-ml-0.9.0/luma/metric/
+-rw-r--r--   0 chanlee    (501) staff       (20)     1654 2024-04-24 15:30:21.000000 luma-ml-0.9.0/luma/metric/classification.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5917 2024-05-13 15:46:55.000000 luma-ml-0.9.0/luma/metric/clustering.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1788 2024-05-13 15:46:57.000000 luma-ml-0.9.0/luma/metric/distance.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1842 2024-05-13 15:46:59.000000 luma-ml-0.9.0/luma/metric/regression.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.017536 luma-ml-0.9.0/luma/migrate/
+-rw-r--r--   0 chanlee    (501) staff       (20)     3764 2024-05-13 16:18:47.000000 luma-ml-0.9.0/luma/migrate/port.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.019417 luma-ml-0.9.0/luma/model_selection/
+-rw-r--r--   0 chanlee    (501) staff       (20)     3438 2024-05-13 16:20:58.000000 luma-ml-0.9.0/luma/model_selection/cv.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8041 2024-05-13 16:29:29.000000 luma-ml-0.9.0/luma/model_selection/fold.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    12244 2024-05-13 16:35:00.000000 luma-ml-0.9.0/luma/model_selection/search.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5736 2024-05-13 16:40:23.000000 luma-ml-0.9.0/luma/model_selection/split.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.021681 luma-ml-0.9.0/luma/neural/
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.023406 luma-ml-0.9.0/luma/neural/_layers/
+-rw-r--r--   0 chanlee    (501) staff       (20)     6748 2024-05-12 09:16:35.000000 luma-ml-0.9.0/luma/neural/_layers/_act.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    19314 2024-05-27 19:00:28.000000 luma-ml-0.9.0/luma/neural/_layers/_conv.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     4144 2024-05-23 16:58:05.000000 luma-ml-0.9.0/luma/neural/_layers/_drop.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     2313 2024-05-12 09:17:05.000000 luma-ml-0.9.0/luma/neural/_layers/_linear.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    10790 2024-05-30 19:49:07.000000 luma-ml-0.9.0/luma/neural/_layers/_norm.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    29777 2024-05-26 11:24:51.000000 luma-ml-0.9.0/luma/neural/_layers/_pool.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.025074 luma-ml-0.9.0/luma/neural/_models/
+-rw-r--r--   0 chanlee    (501) staff       (20)    13097 2024-05-29 08:01:04.000000 luma-ml-0.9.0/luma/neural/_models/_alex.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    13040 2024-05-30 19:37:12.000000 luma-ml-0.9.0/luma/neural/_models/_inception.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    12760 2024-05-29 08:01:42.000000 luma-ml-0.9.0/luma/neural/_models/_lenet.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9639 2024-05-29 08:00:44.000000 luma-ml-0.9.0/luma/neural/_models/_simple.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    23952 2024-05-29 08:01:18.000000 luma-ml-0.9.0/luma/neural/_models/_vgg.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    12024 2024-05-29 08:04:38.000000 luma-ml-0.9.0/luma/neural/base.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    54303 2024-05-30 20:01:17.000000 luma-ml-0.9.0/luma/neural/block.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1319 2024-05-09 19:24:30.000000 luma-ml-0.9.0/luma/neural/init.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    34300 2024-05-30 19:15:29.000000 luma-ml-0.9.0/luma/neural/layer.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     3111 2024-05-13 19:10:16.000000 luma-ml-0.9.0/luma/neural/loss.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    49671 2024-05-30 20:01:31.000000 luma-ml-0.9.0/luma/neural/network.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    21132 2024-05-09 17:12:02.000000 luma-ml-0.9.0/luma/neural/optimizer.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8582 2024-05-13 19:27:55.000000 luma-ml-0.9.0/luma/neural/single.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.025316 luma-ml-0.9.0/luma/pipe/
+-rw-r--r--   0 chanlee    (501) staff       (20)     7308 2024-05-13 19:32:18.000000 luma-ml-0.9.0/luma/pipe/pipeline.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.027259 luma-ml-0.9.0/luma/preprocessing/
+-rw-r--r--   0 chanlee    (501) staff       (20)     5295 2024-04-21 11:36:14.000000 luma-ml-0.9.0/luma/preprocessing/encoder.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5533 2024-04-21 11:36:15.000000 luma-ml-0.9.0/luma/preprocessing/imputer.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     3653 2024-05-13 19:32:35.000000 luma-ml-0.9.0/luma/preprocessing/outlier.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     2624 2024-05-13 19:33:29.000000 luma-ml-0.9.0/luma/preprocessing/scaler.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.029014 luma-ml-0.9.0/luma/reduction/
+-rw-r--r--   0 chanlee    (501) staff       (20)    19163 2024-05-26 19:19:09.000000 luma-ml-0.9.0/luma/reduction/linear.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    40387 2024-05-13 19:55:48.000000 luma-ml-0.9.0/luma/reduction/manifold.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    17019 2024-05-14 09:45:27.000000 luma-ml-0.9.0/luma/reduction/selection.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.032657 luma-ml-0.9.0/luma/regressor/
+-rw-r--r--   0 chanlee    (501) staff       (20)    19882 2024-05-14 09:56:22.000000 luma-ml-0.9.0/luma/regressor/general.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    12687 2024-05-14 10:03:42.000000 luma-ml-0.9.0/luma/regressor/linear.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     6755 2024-05-14 10:04:13.000000 luma-ml-0.9.0/luma/regressor/neighbors.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     3098 2024-05-14 10:05:44.000000 luma-ml-0.9.0/luma/regressor/poly.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    11070 2024-05-14 14:33:09.000000 luma-ml-0.9.0/luma/regressor/robust.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7805 2024-05-14 14:45:46.000000 luma-ml-0.9.0/luma/regressor/svm.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7415 2024-05-14 14:59:17.000000 luma-ml-0.9.0/luma/regressor/tree.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.033262 luma-ml-0.9.0/luma/visual/
+-rw-r--r--   0 chanlee    (501) staff       (20)     3045 2024-04-13 08:30:32.000000 luma-ml-0.9.0/luma/visual/eda.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    25027 2024-05-23 17:04:49.000000 luma-ml-0.9.0/luma/visual/eval.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.034601 luma-ml-0.9.0/luma_ml.egg-info/
+-rw-r--r--   0 chanlee    (501) staff       (20)     5554 2024-05-30 20:01:39.000000 luma-ml-0.9.0/luma_ml.egg-info/PKG-INFO
+-rw-r--r--   0 chanlee    (501) staff       (20)     2000 2024-05-30 20:01:39.000000 luma-ml-0.9.0/luma_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)        1 2024-05-30 20:01:39.000000 luma-ml-0.9.0/luma_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-05-30 20:01:39.000000 luma-ml-0.9.0/luma_ml.egg-info/requires.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)       17 2024-05-30 20:01:39.000000 luma-ml-0.9.0/luma_ml.egg-info/top_level.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-05-30 20:01:40.036404 luma-ml-0.9.0/setup.cfg
+-rw-r--r--   0 chanlee    (501) staff       (20)      842 2024-05-30 20:00:56.000000 luma-ml-0.9.0/setup.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.035282 luma-ml-0.9.0/test/
+-rw-r--r--   0 chanlee    (501) staff       (20)      647 2024-04-29 02:58:00.000000 luma-ml-0.9.0/test/__act.py
+-rw-r--r--   0 chanlee    (501) staff       (20)      429 2024-05-18 16:19:55.000000 luma-ml-0.9.0/test/__test.py
```

### Comparing `luma-ml-0.8.2/LICENSE` & `luma-ml-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/PKG-INFO` & `luma-ml-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luma-ml
-Version: 0.8.2
+Version: 0.9.0
 Summary: A Comprehensive Python Module for Machine Learning and Data Science
 Home-page: https://github.com/ChanLumerico/luma
 Author: ChanLumerico
 Author-email: greensox284@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">
             <img src="https://github.com/ChanLumerico/luma/raw/main/others/luma.png" alt="logo" width="75" height="75">
         </a>
         <h1 class="main-title">LUMA</h1>
         <p class="subtitle">A Comprehensive Python Module for Machine Learning and Data Science</p>
         <img alt="pypi-version" src="https://img.shields.io/pypi/v/luma-ml?logo=python&logoColor=white&color=blue">
         <img alt="pypi-downloads" src="https://img.shields.io/pypi/dm/luma-ml">
-        <img src="https://img.shields.io/badge/total downloads-6.04k-red">
+        <img src="https://img.shields.io/badge/total downloads-6.41k-red">
         <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ChanLumerico/luma?color=yellow">
         <img alt="Code Style" src="https://img.shields.io/badge/code%20style-black-000000.svg">
         <div class="module">
             <h3 class="module-header">Submodules</h3>
             <table>
                 <tr>
                     <th>Name</th>
@@ -108,19 +108,19 @@
         </div>
         <h2></h2>
         <div class="others">
             <h3 class="others-header">Others</h3>
             <table>
                 <tr>
                     <td>Latest Version</td>
-                    <td>0.8.2</td>
+                    <td>0.9.0</td>
                 </tr>
                 <tr>
                     <td>Lines of Code</td>
-                    <td>~25.3K</td>
+                    <td>~26.5K</td>
                 </tr>
                 <tr>
                     <td>Requirement</td>
                     <td>Python 3.12 or later</td>
                 </tr>
                 <tr>
                     <td>Dependencies</td>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: luma-ml Version: 0.8.2 Summary: A Comprehensive
+Metadata-Version: 2.1 Name: luma-ml Version: 0.9.0 Summary: A Comprehensive
 Python Module for Machine Learning and Data Science Home-page: https://
 github.com/ChanLumerico/luma Author: ChanLumerico Author-email:
 greensox284@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Requires-Python: >=3.12
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 numpy Requires-Dist: scipy Requires-Dist: pandas Requires-Dist: matplotlib
 Requires-Dist: seaborn
 _[_l_o_g_o_]
 ************ LLUUMMAA ************
 A Comprehensive Python Module for Machine Learning and Data Science
 [pypi-version][pypi-downloads][https://img.shields.io/badge/total downloads-
-6.04k-red][GitHub code size in bytes][Code Style]
+6.41k-red][GitHub code size in bytes][Code Style]
 ******** SSuubbmmoodduulleess ********
 NNaammee                 DDeessccrriippttiioonn
 luma.classifier      Toolkit for classification models including various
                      algorithms.
 luma.clustering      Focuses on unsupervised learning and clustering
                      algorithms.
 luma.core            Foundational backbone providing essential data structures
@@ -33,12 +33,12 @@
 luma.reduction       Dimensionality reduction techniques for high-dimensional
                      datasets.
 luma.regressor       Comprehensive range of regression algorithms.
 luma.visual          Tools for model visualization and data plotting.
 ******** SSttrruuccttuurree ********
 [structure]
 ******** OOtthheerrss ********
-Latest Version 0.8.2
-Lines of Code  ~25.3K
+Latest Version 0.9.0
+Lines of Code  ~26.5K
 Requirement    Python 3.12 or later
 Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn
 Documentation  _L_U_M_A_ _N_o_t_i_o_n_ _D_o_c_u_m_e_n_t
```

### Comparing `luma-ml-0.8.2/README.md` & `luma-ml-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">
             <img src="https://github.com/ChanLumerico/luma/raw/main/others/luma.png" alt="logo" width="75" height="75">
         </a>
         <h1 class="main-title">LUMA</h1>
         <p class="subtitle">A Comprehensive Python Module for Machine Learning and Data Science</p>
         <img alt="pypi-version" src="https://img.shields.io/pypi/v/luma-ml?logo=python&logoColor=white&color=blue">
         <img alt="pypi-downloads" src="https://img.shields.io/pypi/dm/luma-ml">
-        <img src="https://img.shields.io/badge/total downloads-6.04k-red">
+        <img src="https://img.shields.io/badge/total downloads-6.41k-red">
         <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ChanLumerico/luma?color=yellow">
         <img alt="Code Style" src="https://img.shields.io/badge/code%20style-black-000000.svg">
         <div class="module">
             <h3 class="module-header">Submodules</h3>
             <table>
                 <tr>
                     <th>Name</th>
@@ -89,19 +89,19 @@
         </div>
         <h2></h2>
         <div class="others">
             <h3 class="others-header">Others</h3>
             <table>
                 <tr>
                     <td>Latest Version</td>
-                    <td>0.8.2</td>
+                    <td>0.9.0</td>
                 </tr>
                 <tr>
                     <td>Lines of Code</td>
-                    <td>~25.3K</td>
+                    <td>~26.5K</td>
                 </tr>
                 <tr>
                     <td>Requirement</td>
                     <td>Python 3.12 or later</td>
                 </tr>
                 <tr>
                     <td>Dependencies</td>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 _[_l_o_g_o_]
 ************ LLUUMMAA ************
 A Comprehensive Python Module for Machine Learning and Data Science
 [pypi-version][pypi-downloads][https://img.shields.io/badge/total downloads-
-6.04k-red][GitHub code size in bytes][Code Style]
+6.41k-red][GitHub code size in bytes][Code Style]
 ******** SSuubbmmoodduulleess ********
 NNaammee                 DDeessccrriippttiioonn
 luma.classifier      Toolkit for classification models including various
                      algorithms.
 luma.clustering      Focuses on unsupervised learning and clustering
                      algorithms.
 luma.core            Foundational backbone providing essential data structures
@@ -24,12 +24,12 @@
 luma.reduction       Dimensionality reduction techniques for high-dimensional
                      datasets.
 luma.regressor       Comprehensive range of regression algorithms.
 luma.visual          Tools for model visualization and data plotting.
 ******** SSttrruuccttuurree ********
 [structure]
 ******** OOtthheerrss ********
-Latest Version 0.8.2
-Lines of Code  ~25.3K
+Latest Version 0.9.0
+Lines of Code  ~26.5K
 Requirement    Python 3.12 or later
 Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn
 Documentation  _L_U_M_A_ _N_o_t_i_o_n_ _D_o_c_u_m_e_n_t
```

### Comparing `luma-ml-0.8.2/luma/__import__.py` & `luma-ml-0.9.0/luma/__import__.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,14 +115,18 @@
 from luma.neural.init import KaimingInit, XavierInit
 from luma.neural.block import (
     ConvBlock1D,
     ConvBlock2D,
     ConvBlock3D,
     DenseBlock,
     InceptionBlock,
+    InceptionBlockV2A,
+    InceptionBlockV2B,
+    InceptionBlockV2C,
+    InceptionBlockV2R,
 )
 from luma.neural.network import SimpleMLP, SimpleCNN
 from luma.neural.network import (
     LeNet_1,
     LeNet_4,
     LeNet_5,
     AlexNet,
@@ -287,21 +291,22 @@
     LpPooling1D, LpPooling2D, LpPooling3D
     Dropout, Dropout1D, Dropout2D, Dropout3D,
     BatchNorm1D, BatchNorm2D, BatchNorm3D,
     LocalResponseNorm, LayerNorm,
     Dense, Flatten, Activation,
     Sequential
 
+    ConvBlock1D, ConvBlock2D, ConvBlock3D, DenseBlock,
+    InceptionBlock, InceptionBlockV2A, InceptionBlockV2B,
+    InceptionBlockV2C, InceptionBlockV2R
+
     CrossEntropy, BinaryCrossEntropy, MSELoss
 
     KaimingInit, XavierInit
 
-    ConvBlock1D, ConvBlock2D, ConvBlock3D, DenseBlock,
-    InceptionBlock
-
     SimpleMLP, SimpleCNN, LeNet_1, LeNet_4, LeNet_5, AlexNet,
     ZFNet, VGGNet_11, VGGNet_13, VGGNet_16, VGGNet_19,
     Inception_V1, Inception_V2, Inception_V3
 
     # ------------------- [ luma.metric ] ----------------------
     Accuracy, Precision, Recall, F1Score, Specificity
```

### Comparing `luma-ml-0.8.2/luma/__init__.py` & `luma-ml-0.9.0/luma/__init__.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/classifier/discriminant.py` & `luma-ml-0.9.0/luma/classifier/discriminant.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/classifier/logistic.py` & `luma-ml-0.9.0/luma/classifier/logistic.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/classifier/naive_bayes.py` & `luma-ml-0.9.0/luma/classifier/naive_bayes.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/classifier/neighbors.py` & `luma-ml-0.9.0/luma/classifier/neighbors.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/classifier/svm.py` & `luma-ml-0.9.0/luma/classifier/svm.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/classifier/tree.py` & `luma-ml-0.9.0/luma/classifier/tree.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/clustering/affinity.py` & `luma-ml-0.9.0/luma/clustering/affinity.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/clustering/density.py` & `luma-ml-0.9.0/luma/clustering/density.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/clustering/hierarchy.py` & `luma-ml-0.9.0/luma/clustering/hierarchy.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/clustering/kmeans.py` & `luma-ml-0.9.0/luma/clustering/kmeans.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/clustering/mixture.py` & `luma-ml-0.9.0/luma/clustering/mixture.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/clustering/spectral.py` & `luma-ml-0.9.0/luma/clustering/spectral.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/core/base.py` & `luma-ml-0.9.0/luma/core/base.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/core/super.py` & `luma-ml-0.9.0/luma/core/super.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/ensemble/bagging.py` & `luma-ml-0.9.0/luma/ensemble/bagging.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/ensemble/boost.py` & `luma-ml-0.9.0/luma/ensemble/boost.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/ensemble/forest.py` & `luma-ml-0.9.0/luma/ensemble/forest.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/ensemble/stack.py` & `luma-ml-0.9.0/luma/ensemble/stack.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/ensemble/vote.py` & `luma-ml-0.9.0/luma/ensemble/vote.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/interface/exception.py` & `luma-ml-0.9.0/luma/interface/exception.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/interface/typing.py` & `luma-ml-0.9.0/luma/interface/typing.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/interface/util.py` & `luma-ml-0.9.0/luma/interface/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -408,15 +408,20 @@
     @classmethod
     def validate_type(cls, param_type) -> TypeGuard[Scalar]:
         return param_type in (int, float)
 
     def check(self, param_name: str, param_value: Any) -> None:
         if param_value is None:
             return
-        self._type_check(param_value)
+        if isinstance(param_value, (tuple, list)):
+            for element in param_value:
+                self._type_check(element)
+        else:
+            self._type_check(param_value)
+
         if not self.condition(param_value):
             raise InvalidRangeError(param_value, param_name, self.param_range)
 
     def _type_check(self, param_value: Any) -> None:
         if not isinstance(param_value, self.param_type):
             raise UnsupportedParameterError(param_value)
```

### Comparing `luma-ml-0.8.2/luma/metric/classification.py` & `luma-ml-0.9.0/luma/metric/classification.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/metric/clustering.py` & `luma-ml-0.9.0/luma/metric/clustering.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/metric/distance.py` & `luma-ml-0.9.0/luma/metric/distance.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/metric/regression.py` & `luma-ml-0.9.0/luma/metric/regression.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/migrate/port.py` & `luma-ml-0.9.0/luma/migrate/port.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/model_selection/cv.py` & `luma-ml-0.9.0/luma/model_selection/cv.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/model_selection/fold.py` & `luma-ml-0.9.0/luma/model_selection/fold.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/model_selection/search.py` & `luma-ml-0.9.0/luma/model_selection/search.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/model_selection/split.py` & `luma-ml-0.9.0/luma/model_selection/split.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/neural/_layers/_act.py` & `luma-ml-0.9.0/luma/neural/_layers/_act.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/neural/_layers/_conv.py` & `luma-ml-0.9.0/luma/neural/_layers/_conv.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/neural/_layers/_drop.py` & `luma-ml-0.9.0/luma/neural/_layers/_drop.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/neural/_layers/_linear.py` & `luma-ml-0.9.0/luma/neural/_layers/_linear.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/neural/_layers/_norm.py` & `luma-ml-0.9.0/luma/neural/_layers/_norm.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/neural/_layers/_pool.py` & `luma-ml-0.9.0/luma/neural/_layers/_pool.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/neural/_models/_alex.py` & `luma-ml-0.9.0/luma/neural/_models/_alex.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from dataclasses import asdict
 
 from luma.core.super import Estimator, Evaluator, Optimizer, Supervised
 from luma.interface.typing import Matrix, Tensor, Vector
 from luma.interface.util import InitUtil
 from luma.metric.classification import Accuracy
 
+from luma.neural import loss
 from luma.neural.base import Loss, NeuralModel
-from luma.neural.loss import CrossEntropy
 from luma.neural.block import ConvBlock2D, DenseBlock, ConvBlockArgs, DenseBlockArgs
 from luma.neural.layer import (
     Activation,
     Dense,
     Flatten,
     LocalResponseNorm,
     Sequential,
@@ -22,15 +22,15 @@
 
 
 class _AlexNet(Estimator, Supervised, NeuralModel):
     def __init__(
         self,
         optimizer: Optimizer,
         activation: Activation.FuncType = Activation.ReLU,
-        loss: Loss = CrossEntropy(),
+        loss: Loss = loss.CrossEntropy(),
         initializer: InitUtil.InitStr = None,
         out_features: int = 1000,
         batch_size: int = 128,
         n_epochs: int = 100,
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
         lambda_: float = 0.0,
@@ -235,15 +235,15 @@
 
 
 class _ZFNet(Estimator, Supervised, NeuralModel):
     def __init__(
         self,
         optimizer: Optimizer,
         activation: Activation.FuncType = Activation.ReLU,
-        loss: Loss = CrossEntropy(),
+        loss: Loss = loss.CrossEntropy(),
         initializer: InitUtil.InitStr = None,
         out_features: int = 1000,
         batch_size: int = 128,
         n_epochs: int = 100,
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
         lambda_: float = 0.0,
```

### Comparing `luma-ml-0.8.2/luma/neural/_models/_lenet.py` & `luma-ml-0.9.0/luma/neural/_models/_lenet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from typing import Self, override
 
 from luma.core.super import Estimator, Evaluator, Optimizer, Supervised
 from luma.interface.typing import Matrix, Tensor, Vector
 from luma.interface.util import InitUtil
 from luma.metric.classification import Accuracy
 
+from luma.neural import loss
 from luma.neural.base import Loss, NeuralModel
 from luma.neural.block import ConvBlock2D, DenseBlock
 from luma.neural.layer import Activation, Dense, Flatten, Sequential
-from luma.neural.loss import CrossEntropy
 
 
 __all__ = ("_LeNet_1", "_LeNet_4", "_LeNet_5")
 
 
 class _LeNet_1(Estimator, Supervised, NeuralModel):
     def __init__(
         self,
         optimizer: Optimizer,
         activation: Activation.FuncType = Activation.Tanh,
-        loss: Loss = CrossEntropy(),
+        loss: Loss = loss.CrossEntropy(),
         initializer: InitUtil.InitStr = None,
         out_features: int = 10,
         batch_size: int = 100,
         n_epochs: int = 100,
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
         lambda_: float = 0.0,
@@ -143,15 +143,15 @@
 
 
 class _LeNet_4(Estimator, Supervised, NeuralModel):
     def __init__(
         self,
         optimizer: Optimizer,
         activation: Activation.FuncType = Activation.Tanh,
-        loss: Loss = CrossEntropy(),
+        loss: Loss = loss.CrossEntropy(),
         initializer: InitUtil.InitStr = None,
         out_features: int = 10,
         batch_size: int = 100,
         n_epochs: int = 100,
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
         lambda_: float = 0.0,
@@ -282,15 +282,15 @@
 
 
 class _LeNet_5(Estimator, Supervised, NeuralModel):
     def __init__(
         self,
         optimizer: Optimizer,
         activation: Activation.FuncType = Activation.Tanh,
-        loss: Loss = CrossEntropy(),
+        loss: Loss = loss.CrossEntropy(),
         initializer: InitUtil.InitStr = None,
         out_features: int = 10,
         batch_size: int = 100,
         n_epochs: int = 100,
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
         lambda_: float = 0.0,
```

### Comparing `luma-ml-0.8.2/luma/neural/_models/_simple.py` & `luma-ml-0.9.0/luma/neural/_models/_simple.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/neural/_models/_vgg.py` & `luma-ml-0.9.0/luma/neural/_models/_vgg.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from dataclasses import asdict
 
 from luma.core.super import Estimator, Evaluator, Optimizer, Supervised
 from luma.interface.typing import Matrix, Tensor, Vector
 from luma.interface.util import InitUtil
 from luma.metric.classification import Accuracy
 
+from luma.neural import loss
 from luma.neural.base import Loss, NeuralModel
-from luma.neural.loss import CrossEntropy
 from luma.neural.block import ConvBlock2D, DenseBlock, ConvBlockArgs, DenseBlockArgs
 from luma.neural.layer import (
     Activation,
     Dense,
     Flatten,
     Sequential,
 )
@@ -26,15 +26,15 @@
 
 
 class _VGGNet_11(Estimator, Supervised, NeuralModel):
     def __init__(
         self,
         optimizer: Optimizer,
         activation: Activation.FuncType = Activation.ReLU,
-        loss: Loss = CrossEntropy(),
+        loss: Loss = loss.CrossEntropy(),
         initializer: InitUtil.InitStr = None,
         out_features: int = 1000,
         batch_size: int = 128,
         n_epochs: int = 100,
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
         lambda_: float = 0.0,
@@ -198,15 +198,15 @@
 
 
 class _VGGNet_13(Estimator, Supervised, NeuralModel):
     def __init__(
         self,
         optimizer: Optimizer,
         activation: Activation.FuncType = Activation.ReLU,
-        loss: Loss = CrossEntropy(),
+        loss: Loss = loss.CrossEntropy(),
         initializer: InitUtil.InitStr = None,
         out_features: int = 1000,
         batch_size: int = 128,
         n_epochs: int = 100,
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
         lambda_: float = 0.0,
@@ -382,15 +382,15 @@
 
 
 class _VGGNet_16(Estimator, Supervised, NeuralModel):
     def __init__(
         self,
         optimizer: Optimizer,
         activation: Activation.FuncType = Activation.ReLU,
-        loss: Loss = CrossEntropy(),
+        loss: Loss = loss.CrossEntropy(),
         initializer: InitUtil.InitStr = None,
         out_features: int = 1000,
         batch_size: int = 128,
         n_epochs: int = 100,
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
         lambda_: float = 0.0,
@@ -578,15 +578,15 @@
 
 
 class _VGGNet_19(Estimator, Supervised, NeuralModel):
     def __init__(
         self,
         optimizer: Optimizer,
         activation: Activation.FuncType = Activation.ReLU,
-        loss: Loss = CrossEntropy(),
+        loss: Loss = loss.CrossEntropy(),
         initializer: InitUtil.InitStr = None,
         out_features: int = 1000,
         batch_size: int = 128,
         n_epochs: int = 100,
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
         lambda_: float = 0.0,
```

### Comparing `luma-ml-0.8.2/luma/neural/base.py` & `luma-ml-0.9.0/luma/neural/base.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/neural/init.py` & `luma-ml-0.9.0/luma/neural/init.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/neural/layer.py` & `luma-ml-0.9.0/luma/neural/layer.py`

 * *Files 3% similar despite different names*

```diff
@@ -931,14 +931,17 @@
         self,
         in_shape: Tuple[int] | int,
         epsilon: float = 1e-5,
     ) -> None:
         super().__init__(in_shape, epsilon)
 
 
+type LayerLike = Sequential | Layer
+
+
 class Sequential(Layer):
     """
     Sequential represents a linear arrangement of layers in a neural network
     model. Each layer is added sequentially, with data flowing from one layer
     to the next in the order they are added. This organization simplifies the
     construction of neural networks, especially for straightforward architectures,
     by mirroring the logical flow of data from input through hidden layers to
@@ -990,17 +993,17 @@
 
     out = model(X, is_train=True) # model.forward(X, is_train=True)
     model.backward(d_out) # assume d_out is the gradient w.r.t. loss
     model.update()
     ```
     """
 
-    def __init__(self, *layers: Layer | tuple[str, Layer] | None) -> None:
+    def __init__(self, *layers: LayerLike | tuple[str, LayerLike] | None) -> None:
         super().__init__()
-        self.layers: List[tuple[str, Layer]] = list()
+        self.layers: List[tuple[str, LayerLike]] = list()
         for layer in layers:
             self.add(layer)
 
     def forward(self, X: TensorLike, is_train: bool = False) -> TensorLike:
         self.input_ = X
         out = X
         for _, layer in self.layers:
@@ -1032,40 +1035,50 @@
     def _check_no_optimizer(self) -> None:
         if self.optimizer is None:
             raise RuntimeError(
                 f"'{self}' has no optimizer! "
                 + f"Call '{self}().set_optimizer' to assign an optimizer."
             )
 
-    def add(self, layer: Layer | tuple[str, Layer] | None) -> None:
+    def add(self, layer: LayerLike | tuple[str, LayerLike] | None) -> None:
         if layer is None:
             return
         if not isinstance(layer, tuple):
             layer = (str(layer), layer)
         self.layers.append(layer)
 
         if self.optimizer is not None:
             self.set_optimizer(self.optimizer)
 
     def extend(
         self,
-        *layers: Self | Layer | tuple[str, Layer] | None,
+        *layers: LayerLike | tuple[str, LayerLike] | None,
         deep_add: bool = True,
     ) -> None:
         for layer in layers:
             new_layer = layer
             if isinstance(layer, tuple):
                 name, layer = layer
                 new_layer = (name, layer)
             if hasattr(layer, "layers") and deep_add:
                 for sub_layer in layer.layers:
                     self.add(sub_layer)
                 continue
             self.add(new_layer)
 
+    def override_method(self, func_name: str, func: callable) -> None:
+        if not hasattr(self, func_name):
+            raise RuntimeError(f"'{str(self)}' has no method called '{func_name}'!")
+        if not callable(getattr(self, func_name)):
+            raise TypeError(f"'{func_name}' it not a method!")
+        if not callable(func):
+            raise TypeError(f"Provided method '{func}' it not a method!")
+
+        setattr(self, func_name, func)
+
     @override
     @property
     def param_size(self) -> Tuple[int, int]:
         w_size, b_size = 0, 0
         for _, layer in self.layers:
             w_, b_ = layer.param_size
             w_size += w_
@@ -1074,15 +1087,15 @@
         return w_size, b_size
 
     def out_shape(self, in_shape: Tuple[int]) -> Tuple[int]:
         for _, layer in self.layers:
             in_shape = layer.out_shape(in_shape)
         return in_shape
 
-    def __add__(self, other: Layer | tuple[str, Layer] | None) -> Self:
+    def __add__(self, other: LayerLike | tuple[str, LayerLike] | None) -> Self:
         if isinstance(other, (Layer, tuple)):
             self.add(other)
         else:
             raise TypeError(
                 "Unsupported operand type(s) for +: '{}' and '{}'".format(
                     type(self).__name__, type(other).__name__
                 )
```

### Comparing `luma-ml-0.8.2/luma/neural/loss.py` & `luma-ml-0.9.0/luma/neural/loss.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/neural/network.py` & `luma-ml-0.9.0/luma/neural/network.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Literal
 
 from luma.core.super import Optimizer
 from luma.interface.util import InitUtil
 
+from luma.neural import loss
 from luma.neural.base import Loss
 from luma.neural.layer import Activation
-from luma.neural.loss import CrossEntropy
 
 from luma.neural._models import _simple, _lenet, _alex, _vgg, _inception
 
 
 __all__ = (
     "SimpleMLP",
     "SimpleCNN",
@@ -383,15 +383,15 @@
 
     """
 
     def __init__(
         self,
         optimizer: Optimizer,
         activation: Activation.FuncType = Activation.Tanh,
-        loss: Loss = CrossEntropy(),
+        loss: Loss = loss.CrossEntropy(),
         initializer: InitUtil.InitStr = None,
         out_features: int = 10,
         batch_size: int = 100,
         n_epochs: int = 100,
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
         lambda_: float = 0,
@@ -484,15 +484,15 @@
     Code Recognition." Neural Computation, vol. 1, no. 4, 1989, pp. 541-551.
     """
 
     def __init__(
         self,
         optimizer: Optimizer,
         activation: Activation.FuncType = Activation.Tanh,
-        loss: Loss = CrossEntropy(),
+        loss: Loss = loss.CrossEntropy(),
         initializer: InitUtil.InitStr = None,
         out_features: int = 10,
         batch_size: int = 100,
         n_epochs: int = 100,
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
         lambda_: float = 0,
@@ -588,15 +588,15 @@
     Code Recognition." Neural Computation, vol. 1, no. 4, 1989, pp. 541-551.
     """
 
     def __init__(
         self,
         optimizer: Optimizer,
         activation: Activation.FuncType = Activation.Tanh,
-        loss: Loss = CrossEntropy(),
+        loss: Loss = loss.CrossEntropy(),
         initializer: InitUtil.InitStr = None,
         out_features: int = 10,
         batch_size: int = 100,
         n_epochs: int = 100,
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
         lambda_: float = 0,
@@ -702,15 +702,15 @@
 
     """
 
     def __init__(
         self,
         optimizer: Optimizer,
         activation: Activation.FuncType = Activation.ReLU,
-        loss: Loss = CrossEntropy(),
+        loss: Loss = loss.CrossEntropy(),
         initializer: InitUtil.InitStr = None,
         out_features: int = 1000,
         batch_size: int = 100,
         n_epochs: int = 100,
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
         lambda_: float = 0,
@@ -816,15 +816,15 @@
 
     """
 
     def __init__(
         self,
         optimizer: Optimizer,
         activation: Activation.FuncType = Activation.ReLU,
-        loss: Loss = CrossEntropy(),
+        loss: Loss = loss.CrossEntropy(),
         initializer: InitUtil.InitStr = None,
         out_features: int = 1000,
         batch_size: int = 100,
         n_epochs: int = 100,
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
         lambda_: float = 0,
@@ -932,15 +932,15 @@
     Large-Scale Image Recognition." arXiv preprint arXiv:1409.1556, 2014.
     """
 
     def __init__(
         self,
         optimizer: Optimizer,
         activation: Activation.FuncType = Activation.ReLU,
-        loss: Loss = CrossEntropy(),
+        loss: Loss = loss.CrossEntropy(),
         initializer: InitUtil.InitStr = None,
         out_features: int = 1000,
         batch_size: int = 100,
         n_epochs: int = 100,
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
         lambda_: float = 0,
@@ -1051,15 +1051,15 @@
     Large-Scale Image Recognition." arXiv preprint arXiv:1409.1556, 2014.
     """
 
     def __init__(
         self,
         optimizer: Optimizer,
         activation: Activation.FuncType = Activation.ReLU,
-        loss: Loss = CrossEntropy(),
+        loss: Loss = loss.CrossEntropy(),
         initializer: InitUtil.InitStr = None,
         out_features: int = 1000,
         batch_size: int = 100,
         n_epochs: int = 100,
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
         lambda_: float = 0,
@@ -1173,15 +1173,15 @@
     Large-Scale Image Recognition." arXiv preprint arXiv:1409.1556, 2014.
     """
 
     def __init__(
         self,
         optimizer: Optimizer,
         activation: Activation.FuncType = Activation.ReLU,
-        loss: Loss = CrossEntropy(),
+        loss: Loss = loss.CrossEntropy(),
         initializer: InitUtil.InitStr = None,
         out_features: int = 1000,
         batch_size: int = 100,
         n_epochs: int = 100,
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
         lambda_: float = 0,
@@ -1298,15 +1298,15 @@
     Large-Scale Image Recognition." arXiv preprint arXiv:1409.1556, 2014.
     """
 
     def __init__(
         self,
         optimizer: Optimizer,
         activation: Activation.FuncType = Activation.ReLU,
-        loss: Loss = CrossEntropy(),
+        loss: Loss = loss.CrossEntropy(),
         initializer: InitUtil.InitStr = None,
         out_features: int = 1000,
         batch_size: int = 100,
         n_epochs: int = 100,
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
         lambda_: float = 0,
@@ -1357,27 +1357,27 @@
     ```py
     ConvBlock2D(3, 64, filter_size=7, pool_mode="max") ->
     ConvBlock2D(64, 64, filter_size=1, do_pooling=False) ->
     ConvBlock2D(64, 192, filter_size=3, pool_mode="max") ->
     ```
     Inception Blocks:
     ```py
-    InceptionBlock(192, 64, 96, 128, 16, 32, 32) ->  # Inception_3a
-    InceptionBlock(256, 128, 128, 192, 32, 96, 64) ->  # Inception_3b
-    Pooling2D(3, 2, mode="max")
-
-    InceptionBlock(480, 192, 96, 208, 16, 48, 64) ->  # Inception_4a
-    InceptionBlock(512, 160, 112, 224, 24, 64, 64) ->  # Inception_4b
-    InceptionBlock(512, 128, 128, 256, 24, 64, 64) ->  # Inception_4c
-    InceptionBlock(512, 112, 144, 288, 32, 64, 64) ->  # Inception_4d
-    InceptionBlock(528, 256, 160, 320, 32, 128, 128) ->  # Inception_4e
-    Pooling2D(3, 2, mode="max")
+    InceptionBlock(192) ->  # Inception_3a
+    InceptionBlock(256) ->  # Inception_3b
+    Pooling2D(3, 2, mode="max") ->
+
+    InceptionBlock(480) ->  # Inception_4a
+    InceptionBlock(512) ->  # Inception_4b
+    InceptionBlock(512) ->  # Inception_4c
+    InceptionBlock(512) ->  # Inception_4d
+    InceptionBlock(528) ->  # Inception_4e
+    Pooling2D(3, 2, mode="max") ->
 
-    InceptionBlock(832, 256, 160, 320, 32, 128, 128) ->  # Inception_5a
-    InceptionBlock(832, 384, 192, 384, 48, 128, 128) ->  # Inception_5b
+    InceptionBlock(832) ->  # Inception_5a
+    InceptionBlock(832) ->  # Inception_5b
     GlobalAvgPooling2D() ->
     ```
     Fully Connected Layers:
     ```py
     Flatten -> Dense(1024, 1000)
     ```
     Output:
@@ -1424,15 +1424,15 @@
     2015, pp. 1-9.
     """
 
     def __init__(
         self,
         optimizer: Optimizer,
         activation: Activation.FuncType = Activation.ReLU,
-        loss: Loss = CrossEntropy(),
+        loss: Loss = loss.CrossEntropy(),
         initializer: InitUtil.InitStr = None,
         out_features: int = 1000,
         batch_size: int = 128,
         n_epochs: int = 100,
         learning_rate: float = 0.01,
         valid_size: float = 0.1,
         lambda_: float = 0.0,
@@ -1460,12 +1460,132 @@
             shuffle,
             random_state,
             deep_verbose,
         )
 
 
 class Inception_V2(_inception._Inception_V2):
-    NotImplemented
+    """
+    Inception v2, an improvement of the original Inception architecture,
+    enhances computational efficiency and accuracy in deep learning models.
+    It introduces the factorization of convolutions and additional
+    normalization techniques to reduce the number of parameters and improve
+    training stability. These modifications allow for deeper and more
+    complex neural networks with improved performance.
+
+    Structure
+    ---------
+    Input:
+    ```py
+    Tensor[..., 3, 299, 299]
+    ```
+    Introductory Convolutions:
+    ```py
+    ConvBlock2D(3, 32, filter_size=3, stride=2) ->
+    ConvBlock2D(32, 32, filter_size=3, stride=1) ->
+    ConvBlock2D(32, 64, filter_size=3, stride=1) ->
+    Pooling2D(3, 2, mode="max") ->
+
+    ConvBlock2D(64, 80, filter_size=3, stride=1) ->
+    ConvBlock2D(80, 192, filter_size=3, stride=2) ->
+    ConvBlock2D(192, 288, filter_size=3, stride=1) ->
+    ```
+    Inception Blocks:
+    ```py
+    3x InceptionBlockV2A(288) ->  # Inception_3
+    InceptionBlockV2R(288) ->  # Inception_Rx1
+
+    5x InceptionBlockV2B(768) ->  # Inception_4
+    InceptionBlockV2R(768) ->  # Inception_Rx2
+
+    2x InceptionBlockV2C([1280, 2048]) ->  # Inception_5
+    GlobalAvgPooling2D() ->
+    ```
+    Fully Connected Layers:
+    ```py
+    Flatten -> Dense(2048, 1000)
+    ```
+    Output:
+    ```py
+    Matrix[..., 1000]
+    ```
+    Parameter Size:
+    ```txt
+    24,974,688 weights, 20,136 biases -> 24,994,824 params
+    ```
+    Parameters
+    ----------
+    `activation` : FuncType, default=Activation.ReLU
+        Type of activation function
+    `optimizer` : Optimizer
+        Type of optimizer for weight update
+    `loss` : Loss, default=CrossEntropy()
+        Type of loss function
+    `initializer` : InitStr, default=None
+        Type of weight initializer
+    `out_features` : int, default=1000
+        Number of output features
+    `batch_size` : int, default=100
+        Size of a single mini-batch
+    `n_epochs` : int, default=100
+        Number of epochs for training
+    `learning_rate` : float, default=0.01
+        Step size during optimization process
+    `valid_size` : float, default=0.1
+        Fractional size of validation set
+    `lambda_` : float, default=0.0
+        L2 regularization strength
+    `early_stopping` : bool, default=False
+        Whether to early-stop the training when the valid score stagnates
+    `patience` : int, default=10
+        Number of epochs to wait until early-stopping
+    `shuffle` : bool, default=True
+        Whethter to shuffle the data at the beginning of every epoch
+
+    References
+    ----------
+    1. Szegedy, Christian, et al. “Going Deeper with Convolutions.” Proceedings
+    of the IEEE Conference on Computer Vision and Pattern Recognition (CVPR),
+    2015, pp. 1-9.
+    """
+
+    def __init__(
+        self,
+        optimizer: Optimizer,
+        activation: Activation.FuncType = Activation.ReLU,
+        loss: Loss = loss.CrossEntropy(),
+        initializer: InitUtil.InitStr = None,
+        out_features: int = 1000,
+        batch_size: int = 128,
+        n_epochs: int = 100,
+        learning_rate: float = 0.01,
+        valid_size: float = 0.1,
+        lambda_: float = 0.0,
+        dropout_rate: float = 0.4,
+        early_stopping: bool = False,
+        patience: int = 10,
+        shuffle: bool = True,
+        random_state: int | None = None,
+        deep_verbose: bool = False,
+    ) -> None:
+        super().__init__(
+            optimizer,
+            activation,
+            loss,
+            initializer,
+            out_features,
+            batch_size,
+            n_epochs,
+            learning_rate,
+            valid_size,
+            lambda_,
+            dropout_rate,
+            early_stopping,
+            patience,
+            shuffle,
+            random_state,
+            deep_verbose,
+        )
 
 
 class Inception_V3(_inception._Inception_V3):
     NotImplemented
```

### Comparing `luma-ml-0.8.2/luma/neural/optimizer.py` & `luma-ml-0.9.0/luma/neural/optimizer.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/neural/single.py` & `luma-ml-0.9.0/luma/neural/single.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/pipe/pipeline.py` & `luma-ml-0.9.0/luma/pipe/pipeline.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/preprocessing/encoder.py` & `luma-ml-0.9.0/luma/preprocessing/encoder.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/preprocessing/imputer.py` & `luma-ml-0.9.0/luma/preprocessing/imputer.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/preprocessing/outlier.py` & `luma-ml-0.9.0/luma/preprocessing/outlier.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/preprocessing/scaler.py` & `luma-ml-0.9.0/luma/preprocessing/scaler.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/reduction/linear.py` & `luma-ml-0.9.0/luma/reduction/linear.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/reduction/manifold.py` & `luma-ml-0.9.0/luma/reduction/manifold.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/reduction/selection.py` & `luma-ml-0.9.0/luma/reduction/selection.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/regressor/general.py` & `luma-ml-0.9.0/luma/regressor/general.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/regressor/linear.py` & `luma-ml-0.9.0/luma/regressor/linear.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/regressor/neighbors.py` & `luma-ml-0.9.0/luma/regressor/neighbors.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/regressor/poly.py` & `luma-ml-0.9.0/luma/regressor/poly.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/regressor/robust.py` & `luma-ml-0.9.0/luma/regressor/robust.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/regressor/svm.py` & `luma-ml-0.9.0/luma/regressor/svm.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/regressor/tree.py` & `luma-ml-0.9.0/luma/regressor/tree.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/visual/eda.py` & `luma-ml-0.9.0/luma/visual/eda.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma/visual/eval.py` & `luma-ml-0.9.0/luma/visual/eval.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/luma_ml.egg-info/PKG-INFO` & `luma-ml-0.9.0/luma_ml.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luma-ml
-Version: 0.8.2
+Version: 0.9.0
 Summary: A Comprehensive Python Module for Machine Learning and Data Science
 Home-page: https://github.com/ChanLumerico/luma
 Author: ChanLumerico
 Author-email: greensox284@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">
             <img src="https://github.com/ChanLumerico/luma/raw/main/others/luma.png" alt="logo" width="75" height="75">
         </a>
         <h1 class="main-title">LUMA</h1>
         <p class="subtitle">A Comprehensive Python Module for Machine Learning and Data Science</p>
         <img alt="pypi-version" src="https://img.shields.io/pypi/v/luma-ml?logo=python&logoColor=white&color=blue">
         <img alt="pypi-downloads" src="https://img.shields.io/pypi/dm/luma-ml">
-        <img src="https://img.shields.io/badge/total downloads-6.04k-red">
+        <img src="https://img.shields.io/badge/total downloads-6.41k-red">
         <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ChanLumerico/luma?color=yellow">
         <img alt="Code Style" src="https://img.shields.io/badge/code%20style-black-000000.svg">
         <div class="module">
             <h3 class="module-header">Submodules</h3>
             <table>
                 <tr>
                     <th>Name</th>
@@ -108,19 +108,19 @@
         </div>
         <h2></h2>
         <div class="others">
             <h3 class="others-header">Others</h3>
             <table>
                 <tr>
                     <td>Latest Version</td>
-                    <td>0.8.2</td>
+                    <td>0.9.0</td>
                 </tr>
                 <tr>
                     <td>Lines of Code</td>
-                    <td>~25.3K</td>
+                    <td>~26.5K</td>
                 </tr>
                 <tr>
                     <td>Requirement</td>
                     <td>Python 3.12 or later</td>
                 </tr>
                 <tr>
                     <td>Dependencies</td>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: luma-ml Version: 0.8.2 Summary: A Comprehensive
+Metadata-Version: 2.1 Name: luma-ml Version: 0.9.0 Summary: A Comprehensive
 Python Module for Machine Learning and Data Science Home-page: https://
 github.com/ChanLumerico/luma Author: ChanLumerico Author-email:
 greensox284@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Requires-Python: >=3.12
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 numpy Requires-Dist: scipy Requires-Dist: pandas Requires-Dist: matplotlib
 Requires-Dist: seaborn
 _[_l_o_g_o_]
 ************ LLUUMMAA ************
 A Comprehensive Python Module for Machine Learning and Data Science
 [pypi-version][pypi-downloads][https://img.shields.io/badge/total downloads-
-6.04k-red][GitHub code size in bytes][Code Style]
+6.41k-red][GitHub code size in bytes][Code Style]
 ******** SSuubbmmoodduulleess ********
 NNaammee                 DDeessccrriippttiioonn
 luma.classifier      Toolkit for classification models including various
                      algorithms.
 luma.clustering      Focuses on unsupervised learning and clustering
                      algorithms.
 luma.core            Foundational backbone providing essential data structures
@@ -33,12 +33,12 @@
 luma.reduction       Dimensionality reduction techniques for high-dimensional
                      datasets.
 luma.regressor       Comprehensive range of regression algorithms.
 luma.visual          Tools for model visualization and data plotting.
 ******** SSttrruuccttuurree ********
 [structure]
 ******** OOtthheerrss ********
-Latest Version 0.8.2
-Lines of Code  ~25.3K
+Latest Version 0.9.0
+Lines of Code  ~26.5K
 Requirement    Python 3.12 or later
 Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn
 Documentation  _L_U_M_A_ _N_o_t_i_o_n_ _D_o_c_u_m_e_n_t
```

### Comparing `luma-ml-0.8.2/luma_ml.egg-info/SOURCES.txt` & `luma-ml-0.9.0/luma_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `luma-ml-0.8.2/setup.py` & `luma-ml-0.9.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="luma-ml",
-    version="0.8.2",
+    version="0.9.0",
     author="ChanLumerico",
     author_email="greensox284@gmail.com",
     description="A Comprehensive Python Module for Machine Learning and Data Science",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ChanLumerico/luma",
     packages=setuptools.find_namespace_packages(),
```

### Comparing `luma-ml-0.8.2/test/__act.py` & `luma-ml-0.9.0/test/__act.py`

 * *Files identical despite different names*

