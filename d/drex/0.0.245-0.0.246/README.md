# Comparing `tmp/drex-0.0.245.tar.gz` & `tmp/drex-0.0.246.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drex-0.0.245.tar", last modified: Tue May 14 08:24:08 2024, max compression
+gzip compressed data, was "drex-0.0.246.tar", last modified: Thu May 30 08:31:18 2024, max compression
```

## Comparing `drex-0.0.245.tar` & `drex-0.0.246.tar`

### file list

```diff
@@ -1,64 +1,86 @@
-drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-05-14 08:24:08.386727 drex-0.0.245/
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      134 2024-05-07 19:41:35.000000 drex-0.0.245/.gitignore
--rw-r--r--   0 domizzi   (1000) domizzi   (1000)      770 2024-05-14 08:24:08.386727 drex-0.0.245/PKG-INFO
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      335 2024-04-26 19:47:39.000000 drex-0.0.245/README.md
-drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-05-14 08:24:08.378728 drex-0.0.245/data/
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     4011 2024-04-19 16:55:19.000000 drex-0.0.245/data/100MB.csv
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     2929 2024-04-22 09:11:47.000000 drex-0.0.245/data/10MB.csv
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     2933 2024-04-22 09:11:39.000000 drex-0.0.245/data/1MB.csv
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     2903 2024-03-26 20:01:25.000000 drex-0.0.245/data/200MB.csv
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     3915 2024-04-22 09:06:02.000000 drex-0.0.245/data/50MB.csv
-drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-05-14 08:24:08.378728 drex-0.0.245/drex/
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        0 2024-03-28 21:09:29.000000 drex-0.0.245/drex/__init__.py
-drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-05-14 08:24:08.378728 drex-0.0.245/drex/inputs/
-drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-05-14 08:24:08.382727 drex-0.0.245/drex/inputs/data/
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)   865236 2024-05-06 07:31:37.000000 drex-0.0.245/drex/inputs/data/FB-2009_samples_24_times_1hr_0.csv
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      260 2024-05-06 07:31:37.000000 drex-0.0.245/drex/inputs/data/README.md
-drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-05-14 08:24:08.382727 drex-0.0.245/drex/inputs/data/raw/
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)   198743 2024-05-06 07:31:37.000000 drex-0.0.245/drex/inputs/data/raw/FB-2009_samples_24_times_1hr_0.tsv
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)   223858 2024-05-06 07:31:37.000000 drex-0.0.245/drex/inputs/data/raw/FB-2009_samples_24_times_1hr_1.tsv
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)   898688 2024-05-06 07:31:37.000000 drex-0.0.245/drex/inputs/data/raw/FB-2010_samples_24_times_1hr_0.tsv
-drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-05-14 08:24:08.386727 drex-0.0.245/drex/inputs/nodes/
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)   163124 2024-05-06 07:31:37.000000 drex-0.0.245/drex/inputs/nodes/4-Lifetime-AFR.png
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      209 2024-05-06 07:31:37.000000 drex-0.0.245/drex/inputs/nodes/README.md
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     1551 2024-05-06 07:31:37.000000 drex-0.0.245/drex/inputs/nodes/from_backblaze.txt
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      244 2024-05-06 07:31:37.000000 drex-0.0.245/drex/inputs/nodes/nodes_1.csv
-drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-05-14 08:24:08.386727 drex-0.0.245/drex/inputs/parsing_code/
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     2767 2024-05-06 07:31:37.000000 drex-0.0.245/drex/inputs/parsing_code/parse_SWIM_map_reduce.py
-drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-05-14 08:24:08.386727 drex-0.0.245/drex/schedulers/
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      955 2024-04-25 10:11:30.000000 drex-0.0.245/drex/schedulers/algorithm1.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)    10608 2024-05-03 10:48:23.000000 drex-0.0.245/drex/schedulers/algorithm2.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     8333 2024-05-03 10:48:23.000000 drex-0.0.245/drex/schedulers/algorithm3.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)    16176 2024-05-03 10:48:23.000000 drex-0.0.245/drex/schedulers/algorithm4.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     9549 2024-05-06 13:16:07.000000 drex-0.0.245/drex/schedulers/hdfs.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     1915 2024-05-03 10:48:23.000000 drex-0.0.245/drex/schedulers/random.py
-drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-05-14 08:24:08.386727 drex-0.0.245/drex/utils/
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        0 2024-03-28 21:06:13.000000 drex-0.0.245/drex/utils/__init__.py
-drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-05-14 08:24:08.386727 drex-0.0.245/drex/utils/hdfs/
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        0 2024-05-06 10:47:45.000000 drex-0.0.245/drex/utils/hdfs/__init__.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      656 2024-05-06 11:01:03.000000 drex-0.0.245/drex/utils/hdfs/functions.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     1486 2024-04-25 20:04:38.000000 drex-0.0.245/drex/utils/load_data.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)    10547 2024-03-26 19:02:20.000000 drex-0.0.245/drex/utils/poibin.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     2034 2024-04-26 09:10:23.000000 drex-0.0.245/drex/utils/prediction.py
-drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-05-14 08:24:08.386727 drex-0.0.245/drex/utils/reliability/
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        0 2024-03-28 21:06:19.000000 drex-0.0.245/drex/utils/reliability/__init__.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     5540 2024-05-08 12:01:59.000000 drex-0.0.245/drex/utils/reliability/fragment_handler.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     8261 2024-05-08 13:12:17.000000 drex-0.0.245/drex/utils/reliability/ida.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     6674 2024-05-08 11:22:43.000000 drex-0.0.245/drex/utils/reliability/utils.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)    16237 2024-05-03 10:48:23.000000 drex-0.0.245/drex/utils/tool_functions.py
-drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-05-14 08:24:08.386727 drex-0.0.245/drex.egg-info/
--rw-r--r--   0 domizzi   (1000) domizzi   (1000)      770 2024-05-14 08:24:08.000000 drex-0.0.245/drex.egg-info/PKG-INFO
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     1318 2024-05-14 08:24:08.000000 drex-0.0.245/drex.egg-info/SOURCES.txt
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        1 2024-05-14 08:24:08.000000 drex-0.0.245/drex.egg-info/dependency_links.txt
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)       32 2024-05-14 08:24:08.000000 drex-0.0.245/drex.egg-info/requires.txt
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        5 2024-05-14 08:24:08.000000 drex-0.0.245/drex.egg-info/top_level.txt
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      629 2024-05-14 08:23:56.000000 drex-0.0.245/pyproject.toml
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)       38 2024-05-14 08:24:08.386727 drex-0.0.245/setup.cfg
-drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-05-14 08:24:08.386727 drex-0.0.245/test/
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        0 2024-04-17 11:45:13.000000 drex-0.0.245/test/__init__.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     5943 2024-05-06 13:14:06.000000 drex-0.0.245/test/drex-test.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      414 2024-04-25 20:04:38.000000 drex-0.0.245/test/filter_data.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     1203 2024-05-06 10:25:22.000000 drex-0.0.245/test/hdfs-test.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     1622 2024-05-08 13:12:48.000000 drex-0.0.245/test/test-ida.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     1230 2024-05-08 08:13:25.000000 drex-0.0.245/test/test-ida2.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     2757 2024-04-26 09:02:34.000000 drex-0.0.245/test/test_linearregression.py
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-05-30 08:31:18.158870 drex-0.0.246/
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      134 2024-05-07 19:41:35.000000 drex-0.0.246/.gitignore
+-rw-r--r--   0 domizzi   (1000) domizzi   (1000)      770 2024-05-30 08:31:18.158870 drex-0.0.246/PKG-INFO
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      335 2024-04-26 19:47:39.000000 drex-0.0.246/README.md
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-05-30 08:31:18.146870 drex-0.0.246/data/
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     4011 2024-04-19 16:55:19.000000 drex-0.0.246/data/100MB.csv
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     2929 2024-04-22 09:11:47.000000 drex-0.0.246/data/10MB.csv
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     2933 2024-04-22 09:11:39.000000 drex-0.0.246/data/1MB.csv
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     2903 2024-03-26 20:01:25.000000 drex-0.0.246/data/200MB.csv
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     3915 2024-04-22 09:06:02.000000 drex-0.0.246/data/50MB.csv
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-05-30 08:31:18.146870 drex-0.0.246/drex/
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        0 2024-03-28 21:09:29.000000 drex-0.0.246/drex/__init__.py
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-05-30 08:31:18.142869 drex-0.0.246/drex/inputs/
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-05-30 08:31:18.146870 drex-0.0.246/drex/inputs/data/
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)   865236 2024-05-06 07:31:37.000000 drex-0.0.246/drex/inputs/data/FB-2009_samples_24_times_1hr_0.csv
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      260 2024-05-06 07:31:37.000000 drex-0.0.246/drex/inputs/data/README.md
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-05-30 08:31:18.146870 drex-0.0.246/drex/inputs/data/raw/
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)   198743 2024-05-06 07:31:37.000000 drex-0.0.246/drex/inputs/data/raw/FB-2009_samples_24_times_1hr_0.tsv
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)   223858 2024-05-06 07:31:37.000000 drex-0.0.246/drex/inputs/data/raw/FB-2009_samples_24_times_1hr_1.tsv
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)   898688 2024-05-06 07:31:37.000000 drex-0.0.246/drex/inputs/data/raw/FB-2010_samples_24_times_1hr_0.tsv
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-05-30 08:31:18.150869 drex-0.0.246/drex/inputs/nodes/
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      350 2024-05-20 19:47:17.000000 drex-0.0.246/drex/inputs/nodes/10_most_unreliable_nodes.csv
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      349 2024-05-20 19:47:17.000000 drex-0.0.246/drex/inputs/nodes/10_most_used_nodes.csv
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)   163124 2024-05-06 07:31:37.000000 drex-0.0.246/drex/inputs/nodes/4-Lifetime-AFR.png
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      209 2024-05-06 07:31:37.000000 drex-0.0.246/drex/inputs/nodes/README.md
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     1850 2024-05-20 19:47:17.000000 drex-0.0.246/drex/inputs/nodes/from_backblaze.txt
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-05-30 08:31:18.150869 drex-0.0.246/drex/inputs/parsing_code/
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     2767 2024-05-06 07:31:37.000000 drex-0.0.246/drex/inputs/parsing_code/parse_SWIM_map_reduce.py
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-05-30 08:31:18.150869 drex-0.0.246/drex/schedulers/
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      953 2024-05-22 19:52:48.000000 drex-0.0.246/drex/schedulers/algorithm1.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)    10960 2024-05-22 19:52:48.000000 drex-0.0.246/drex/schedulers/algorithm2.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     8369 2024-05-22 19:52:48.000000 drex-0.0.246/drex/schedulers/algorithm3.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)    16212 2024-05-22 19:52:48.000000 drex-0.0.246/drex/schedulers/algorithm4.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)    10501 2024-05-17 21:37:32.000000 drex-0.0.246/drex/schedulers/hdfs.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     1915 2024-05-03 10:48:23.000000 drex-0.0.246/drex/schedulers/random.py
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-05-30 08:31:18.150869 drex-0.0.246/drex/utils/
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        0 2024-03-28 21:06:13.000000 drex-0.0.246/drex/utils/__init__.py
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-05-30 08:31:18.154870 drex-0.0.246/drex/utils/hdfs/
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        0 2024-05-06 10:47:45.000000 drex-0.0.246/drex/utils/hdfs/__init__.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     1649 2024-05-17 21:37:32.000000 drex-0.0.246/drex/utils/hdfs/functions.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     1486 2024-04-25 20:04:38.000000 drex-0.0.246/drex/utils/load_data.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)    10547 2024-03-26 19:02:20.000000 drex-0.0.246/drex/utils/poibin.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     2034 2024-04-26 09:10:23.000000 drex-0.0.246/drex/utils/prediction.py
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-05-30 08:31:18.154870 drex-0.0.246/drex/utils/reliability/
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        0 2024-03-28 21:06:19.000000 drex-0.0.246/drex/utils/reliability/__init__.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     5553 2024-05-30 08:29:14.000000 drex-0.0.246/drex/utils/reliability/fragment_handler.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     8261 2024-05-08 13:12:17.000000 drex-0.0.246/drex/utils/reliability/ida.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     6674 2024-05-08 11:22:43.000000 drex-0.0.246/drex/utils/reliability/utils.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)    16923 2024-05-22 19:52:48.000000 drex-0.0.246/drex/utils/tool_functions.py
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-05-30 08:31:18.158870 drex-0.0.246/drex.egg-info/
+-rw-r--r--   0 domizzi   (1000) domizzi   (1000)      770 2024-05-30 08:31:18.000000 drex-0.0.246/drex.egg-info/PKG-INFO
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     2030 2024-05-30 08:31:18.000000 drex-0.0.246/drex.egg-info/SOURCES.txt
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        1 2024-05-30 08:31:18.000000 drex-0.0.246/drex.egg-info/dependency_links.txt
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)       32 2024-05-30 08:31:18.000000 drex-0.0.246/drex.egg-info/requires.txt
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        5 2024-05-30 08:31:18.000000 drex-0.0.246/drex.egg-info/top_level.txt
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-05-30 08:31:18.154870 drex-0.0.246/plot/
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-05-30 08:31:18.154870 drex-0.0.246/plot/data/
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)    23344 2024-05-30 08:29:14.000000 drex-0.0.246/plot/data/outputfiles_10_100MB.csv
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)    32462 2024-05-30 08:29:14.000000 drex-0.0.246/plot/data/outputfiles_10_1MB.csv
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     2369 2024-05-30 08:29:14.000000 drex-0.0.246/plot/data/outputfiles_1_100MB.csv
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     3273 2024-05-30 08:29:14.000000 drex-0.0.246/plot/data/outputfiles_1_10MB.csv
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     4850 2024-05-30 08:29:14.000000 drex-0.0.246/plot/data/outputtimes_10_100MB.csv
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     5471 2024-05-30 08:29:14.000000 drex-0.0.246/plot/data/outputtimes_10_1MB.csv
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     4137 2024-05-30 08:29:14.000000 drex-0.0.246/plot/data/outputtimes_1_100MB.csv
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     4852 2024-05-30 08:29:14.000000 drex-0.0.246/plot/data/outputtimes_1_10MB.csv
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     3607 2024-05-30 08:29:14.000000 drex-0.0.246/plot/plot.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)    13768 2024-05-30 08:29:14.000000 drex-0.0.246/plot/total_chunk_time_10_100MB.pdf
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)    13712 2024-05-30 08:29:14.000000 drex-0.0.246/plot/total_chunk_time_1_100MB.pdf
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)    13629 2024-05-30 08:29:14.000000 drex-0.0.246/plot/total_scheduling_time_10_100MB.pdf
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)    13606 2024-05-30 08:29:14.000000 drex-0.0.246/plot/total_scheduling_time_1_100MB.pdf
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)    13462 2024-05-30 08:29:14.000000 drex-0.0.246/plot/total_simulation_time_10_100MB.pdf
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)    13481 2024-05-30 08:29:14.000000 drex-0.0.246/plot/total_simulation_time_1_100MB.pdf
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)    13966 2024-05-30 08:29:14.000000 drex-0.0.246/plot/total_storage_used_10_100MB.pdf
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)    13962 2024-05-30 08:29:14.000000 drex-0.0.246/plot/total_storage_used_1_100MB.pdf
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)    13519 2024-05-30 08:29:14.000000 drex-0.0.246/plot/total_upload_time_10_100MB.pdf
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)    13518 2024-05-30 08:29:14.000000 drex-0.0.246/plot/total_upload_time_1_100MB.pdf
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      629 2024-05-30 08:31:05.000000 drex-0.0.246/pyproject.toml
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)       38 2024-05-30 08:31:18.158870 drex-0.0.246/setup.cfg
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-05-30 08:31:18.158870 drex-0.0.246/test/
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        0 2024-04-17 11:45:13.000000 drex-0.0.246/test/__init__.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     5833 2024-05-22 19:52:48.000000 drex-0.0.246/test/drex-test.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      414 2024-04-25 20:04:38.000000 drex-0.0.246/test/filter_data.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     1203 2024-05-06 10:25:22.000000 drex-0.0.246/test/hdfs-test.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     1622 2024-05-08 13:12:48.000000 drex-0.0.246/test/test-ida.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     1230 2024-05-08 08:13:25.000000 drex-0.0.246/test/test-ida2.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     2757 2024-04-26 09:02:34.000000 drex-0.0.246/test/test_linearregression.py
```

### Comparing `drex-0.0.245/PKG-INFO` & `drex-0.0.246/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drex
-Version: 0.0.245
+Version: 0.0.246
 Summary: DRex package
 Author-email: "Maxime, Dante, Haochen" <dantsanc@pa.uc3m.es>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `drex-0.0.245/data/100MB.csv` & `drex-0.0.246/data/100MB.csv`

 * *Files identical despite different names*

### Comparing `drex-0.0.245/data/10MB.csv` & `drex-0.0.246/data/10MB.csv`

 * *Files identical despite different names*

### Comparing `drex-0.0.245/data/1MB.csv` & `drex-0.0.246/data/1MB.csv`

 * *Files identical despite different names*

### Comparing `drex-0.0.245/data/200MB.csv` & `drex-0.0.246/data/200MB.csv`

 * *Files identical despite different names*

### Comparing `drex-0.0.245/data/50MB.csv` & `drex-0.0.246/data/50MB.csv`

 * *Files identical despite different names*

### Comparing `drex-0.0.245/drex/inputs/data/FB-2009_samples_24_times_1hr_0.csv` & `drex-0.0.246/drex/inputs/data/FB-2009_samples_24_times_1hr_0.csv`

 * *Files identical despite different names*

### Comparing `drex-0.0.245/drex/inputs/data/raw/FB-2009_samples_24_times_1hr_0.tsv` & `drex-0.0.246/drex/inputs/data/raw/FB-2009_samples_24_times_1hr_0.tsv`

 * *Files identical despite different names*

### Comparing `drex-0.0.245/drex/inputs/data/raw/FB-2009_samples_24_times_1hr_1.tsv` & `drex-0.0.246/drex/inputs/data/raw/FB-2009_samples_24_times_1hr_1.tsv`

 * *Files identical despite different names*

### Comparing `drex-0.0.245/drex/inputs/data/raw/FB-2010_samples_24_times_1hr_0.tsv` & `drex-0.0.246/drex/inputs/data/raw/FB-2010_samples_24_times_1hr_0.tsv`

 * *Files identical despite different names*

### Comparing `drex-0.0.245/drex/inputs/nodes/4-Lifetime-AFR.png` & `drex-0.0.246/drex/inputs/nodes/4-Lifetime-AFR.png`

 * *Files identical despite different names*

### Comparing `drex-0.0.245/drex/inputs/parsing_code/parse_SWIM_map_reduce.py` & `drex-0.0.246/drex/inputs/parsing_code/parse_SWIM_map_reduce.py`

 * *Files identical despite different names*

### Comparing `drex-0.0.245/drex/schedulers/algorithm1.py` & `drex-0.0.246/drex/schedulers/algorithm1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from drex.utils.tool_functions import *
 import time
 
 def algorithm1(number_of_nodes, reliability_threshold, reliability_of_nodes, node_sizes, file_size):
 	"""
 	Return the full set of nodes and choose K as big as possible
 	"""
-	
 	start = time.time()
 	
 	N = number_of_nodes
 	K = get_max_K_from_reliability_threshold_and_nodes_chosen(N, reliability_threshold, reliability_of_nodes)
 	
 	if (K == -1):
 		print("ERROR: No K was found for Algorithm 1.")
```

### Comparing `drex-0.0.245/drex/schedulers/algorithm2.py` & `drex-0.0.246/drex/schedulers/algorithm2.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,22 @@
 
 def algorithm2(number_of_nodes, reliability_of_nodes, bandwidths, reliability_threshold, file_size, real_records, node_sizes, predictor):
     """
     Choose fastest N and biggest K
     """
     start = time.time()
 
+    # ~ print("In alg2")
+    # ~ print("file_size:", file_size)
+    # ~ print("number_of_nodes:", number_of_nodes)
+    # ~ print("node_sizes:", node_sizes)
+    # ~ print("reliability_of_nodes:", reliability_of_nodes)
+    # ~ print("reliability_threshold:", reliability_threshold)
+    # ~ print("bandwidths:", bandwidths)
+
     min_time = sys.maxsize
     min_N = -1
     min_K = -1
     set_of_nodes_chosen = []
     set_of_nodes = list(range(0, number_of_nodes))
 
     for i in range(3, number_of_nodes + 1):
@@ -199,12 +207,12 @@
         exit(1)
 	
     node_sizes = update_node_sizes(
         min_set_of_nodes_chosen, min_K, file_size, node_sizes)
 	
     end = time.time()
 
-    print("\nAlgorithm 2 chose N =", min_N, "and K =", min_K, "with the set of nodes:",
+    print("\nalgorithm2_work_with_reduced_set_of_nodes chose N =", min_N, "and K =", min_K, "with the set of nodes:",
           min_set_of_nodes_chosen, "It took", end - start, "seconds.")
 
     return list(min_set_of_nodes_chosen), min_N, min_K, node_sizes
```

### Comparing `drex-0.0.245/drex/schedulers/algorithm3.py` & `drex-0.0.246/drex/schedulers/algorithm3.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,10 +188,10 @@
 	min_K = set_of_possible_solutions[set_of_solution_on_pareto[min_index]][1]
 	min_set_of_nodes_chosen = set_of_possible_solutions[set_of_solution_on_pareto[min_index]][2]
 	
 	node_sizes = update_node_sizes(min_set_of_nodes_chosen, min_K, file_size, node_sizes)
 	
 	end = time.time()
 	
-	print("\nAlgorithm 3 chose N =", min_N, "and K =", min_K, "with the set of nodes:", min_set_of_nodes_chosen, "It took", end - start, "seconds.")
+	print("\nalgorithm3_look_at_reduced_set_of_possibilities chose N =", min_N, "and K =", min_K, "with the set of nodes:", min_set_of_nodes_chosen, "It took", end - start, "seconds.")
 	
 	return list(min_set_of_nodes_chosen), min_N, min_K, node_sizes
```

### Comparing `drex-0.0.245/drex/schedulers/algorithm4.py` & `drex-0.0.246/drex/schedulers/algorithm4.py`

 * *Files 1% similar despite different names*

```diff
@@ -318,11 +318,11 @@
     min_set_of_nodes_chosen = set_of_possible_solutions[set_of_solution_on_pareto[best_index]][2]
 
     node_sizes = update_node_sizes(
         min_set_of_nodes_chosen, min_K, file_size, node_sizes)
 
     end = time.time()
 
-    print("\nAlgorithm 4 chose N =", min_N, "and K =", min_K, "with the set of nodes:",
+    print("\nalgorithm4_look_at_reduced_set_of_possibilities chose N =", min_N, "and K =", min_K, "with the set of nodes:",
           min_set_of_nodes_chosen, "It took", end - start, "seconds.")
 
     return list(min_set_of_nodes_chosen), min_N, min_K, node_sizes
```

### Comparing `drex-0.0.245/drex/schedulers/hdfs.py` & `drex-0.0.246/drex/schedulers/hdfs.py`

 * *Files 19% similar despite different names*

```diff
@@ -67,36 +67,50 @@
     # ~ print("set_of_nodes_chosen after mem check", set_of_nodes_chosen)
     set_of_nodes_chosen = sorted(set_of_nodes_chosen)
     # ~ print("set_of_nodes_chosen after sort", set_of_nodes_chosen)
 
     # Need to do this after the potnetial switch of nodes of course
     reliability_of_nodes_chosen = [reliability_of_nodes[node] for node in set_of_nodes_chosen]
     
-    # Loop until the sum meets the threshold
+    # Check if the reliability threshold is met. Else replace the worst node in terms of reliability with
+    # the best one that is not yet in the set of nodes chosen. The same code is copy and pasted and used in
+    # hdfs_reed_solomon
     loop = 0
-    # ~ print("R chosen before:", reliability_of_nodes_chosen)
     while reliability_thresold_met(N, 1, reliability_threshold, reliability_of_nodes_chosen) == False:
-        # ~ print("Reliability issue")
         if (loop > number_of_nodes - N):
             print(f"ERROR: hdfs_three_replications could not find a solution. (loop: {loop}, number nodes {number_of_nodes}), N: {N}")
             exit(1)
-        # Find the index of the lowest reliability value
-        min_reliability_index = reliability_of_nodes_chosen.index(max(reliability_of_nodes_chosen))
         
-        # Find the index of the highest new reliability value
-        highest_new_reliability = min(filter(lambda x: x not in reliability_of_nodes_chosen, reliability_of_nodes))
-        highest_new_reliability_index = reliability_of_nodes.index(highest_new_reliability)
+        # Find the index of the lowest reliability value
+        index = 0
+        index_min_reliability = 0
+        min_reliability = -1
+        for i in reliability_of_nodes_chosen:
+            if min_reliability < i:
+                min_reliability = i
+                index_min_reliability = index
+            index += 1
+                
+        # Find the index of the highest new reliability value that is not already being used
+        index = 0
+        index_max_reliability = 0
+        max_reliability = 2
+        for i in reliability_of_nodes:
+            if max_reliability > i and set_of_nodes[index] not in set_of_nodes_chosen:
+                max_reliability = i
+                index_max_reliability = index
+            index += 1
         
         # Replace the lowest reliability value with the corresponding value from reliability_of_nodes
-        reliability_of_nodes_chosen[min_reliability_index] = highest_new_reliability
+        reliability_of_nodes_chosen[index_min_reliability] = max_reliability
         
         # Update the corresponding node in set_of_nodes_chosen
-        set_of_nodes_chosen[min_reliability_index] = highest_new_reliability_index
+        set_of_nodes_chosen[index_min_reliability] = set_of_nodes[index_max_reliability]
         loop += 1
-        
+                
     # Custom code for update node size cause we have inconsistent data sizes
     j = 0
     for i in set_of_nodes_chosen:
         node_sizes[i] = node_sizes[i] - size_to_stores[j]
         j += 1
     
     end = time.time()
@@ -107,15 +121,15 @@
     elif mode == "real":
         print("\nHDFS 3 replications real chose the set of nodes:", set_of_nodes_chosen, "and will remove the coprresponding size from these nodes:", size_to_stores, "It took", end - start, "seconds.")
         return set_of_nodes_chosen, node_sizes, size_to_stores
     else: 
         print("Wrong mode passed to hdfs 3 replications. It must be \"simulation\" or \"real\"")
         exit(1)
     
-def hdfs_reed_solomon(number_of_nodes, reliability_threshold, reliability_of_nodes, node_sizes, file_size, bandwidths, RS1, RS2, mode):
+def hdfs_reed_solomon(number_of_nodes, reliability_threshold, reliability_of_nodes, node_sizes, file_size, bandwidths, RS1, RS2):
     """
     Uses reed solomon and the fastest nodes first
     N = RS2 and to get K need to do file_size/(((1/(RS1/(RS1+RS2)))*100)/RS2)
     """
     
     start = time.time()
 	
@@ -158,48 +172,63 @@
                 print("ERROR: hdfs_three_replications could not find a solution.")
                 exit(1)
         j += 1
     
     set_of_nodes_chosen = sorted(set_of_nodes_chosen)
     # ~ print(set_of_nodes_chosen)
     
-    # Need to do this after the potnetial switch of nodes of course
+    # Need to do this after the potential switch of nodes of course
     reliability_of_nodes_chosen = [reliability_of_nodes[node] for node in set_of_nodes_chosen]
     
-    # Loop until the sum meets the threshold
+    # Check if the reliability threshold is met. Else replace the worst node in terms of reliability with
+    # the best one that is not yet in the set of nodes chosen. The same code is copy and pasted and used in
+    # hdfs_three_replications
     loop = 0
-    # ~ print("R chosen before:", reliability_of_nodes_chosen)
     while reliability_thresold_met(N, 1, reliability_threshold, reliability_of_nodes_chosen) == False:
         if (loop > number_of_nodes - N):
-            print("ERROR: hdfs_three_replications could not find a solution.")
+            print(f"ERROR: hdfs_three_replications could not find a solution. (loop: {loop}, number nodes {number_of_nodes}), N: {N}")
             exit(1)
-        # Find the index of the lowest reliability value
-        min_reliability_index = reliability_of_nodes_chosen.index(max(reliability_of_nodes_chosen))
         
-        # Find the index of the highest new reliability value
-        highest_new_reliability = min(filter(lambda x: x not in reliability_of_nodes_chosen, reliability_of_nodes))
-        highest_new_reliability_index = reliability_of_nodes.index(highest_new_reliability)
+        # Find the index of the lowest reliability value
+        index = 0
+        index_min_reliability = 0
+        min_reliability = -1
+        for i in reliability_of_nodes_chosen:
+            if min_reliability < i:
+                min_reliability = i
+                index_min_reliability = index
+            index += 1
+                
+        # Find the index of the highest new reliability value that is not already being used
+        index = 0
+        index_max_reliability = 0
+        max_reliability = 2
+        for i in reliability_of_nodes:
+            if max_reliability > i and set_of_nodes[index] not in set_of_nodes_chosen:
+                max_reliability = i
+                index_max_reliability = index
+            index += 1
         
         # Replace the lowest reliability value with the corresponding value from reliability_of_nodes
-        reliability_of_nodes_chosen[min_reliability_index] = highest_new_reliability
+        reliability_of_nodes_chosen[index_min_reliability] = max_reliability
         
         # Update the corresponding node in set_of_nodes_chosen
-        set_of_nodes_chosen[min_reliability_index] = highest_new_reliability_index
+        set_of_nodes_chosen[index_min_reliability] = set_of_nodes[index_max_reliability]
         loop += 1
-        
+                
     # Custom code for update node size cause we have inconsistent data sizes
     j = 0
     for i in set_of_nodes_chosen:
         node_sizes[i] = node_sizes[i] - size_to_stores[j]
         j += 1
     
     end = time.time()
 		    
-    if mode == "simulation":
-        print("\nHDFS Reed Solomon (", RS1, ",", RS2, ") simulation chose N =", N, "and K =", K, "with the set of nodes:", set_of_nodes_chosen, "It took", end - start, "seconds.")
-        return set_of_nodes_chosen, N, K, node_sizes
-    elif mode == "real":
-        print("\nHDFS Reed Solomon (", RS1, ",", RS2, ") real chose the set of nodes:", set_of_nodes_chosen, "and will remove the coprresponding size from these nodes:", size_to_stores, "It took", end - start, "seconds.")
-        return set_of_nodes_chosen, node_sizes, size_to_stores
-    else: 
-        print("Wrong mode passed to HDFS Reed Solomon (", RS1, ",", RS2, "). It must be \"simulation\" or \"real\"")
-        exit(1)
+    # ~ if mode == "simulation":
+        # ~ print("\nHDFS Reed Solomon (", RS1, ",", RS2, ") simulation chose N =", N, "and K =", K, "with the set of nodes:", set_of_nodes_chosen, "It took", end - start, "seconds.")
+        # ~ return set_of_nodes_chosen, N, K, node_sizes
+    # ~ elif mode == "real":
+    print("\nHDFS Reed Solomon (", RS1, ",", RS2, ") real chose the set of nodes:", set_of_nodes_chosen, "and will remove the corresponding size from these nodes:", size_to_stores, "It took", end - start, "seconds.")
+    return set_of_nodes_chosen, N, K, node_sizes, size_to_stores
+    # ~ else: 
+        # ~ print("Wrong mode passed to HDFS Reed Solomon (", RS1, ",", RS2, "). It must be \"simulation\" or \"real\"")
+        # ~ exit(1)
```

### Comparing `drex-0.0.245/drex/schedulers/random.py` & `drex-0.0.246/drex/schedulers/random.py`

 * *Files identical despite different names*

### Comparing `drex-0.0.245/drex/utils/load_data.py` & `drex-0.0.246/drex/utils/load_data.py`

 * *Files identical despite different names*

### Comparing `drex-0.0.245/drex/utils/poibin.py` & `drex-0.0.246/drex/utils/poibin.py`

 * *Files identical despite different names*

### Comparing `drex-0.0.245/drex/utils/prediction.py` & `drex-0.0.246/drex/utils/prediction.py`

 * *Files identical despite different names*

### Comparing `drex-0.0.245/drex/utils/reliability/fragment_handler.py` & `drex-0.0.246/drex/utils/reliability/fragment_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,21 +125,21 @@
             else: 
                 indices.add(idx)
             
             # check if the fragments have the same values of the parameters m, n, p, original_file_hash
             if (m,n,p)!=(m_, n_,p_):
                 raise ValueError("These fragments are not derived from the same file.")
             
-            print(over255)
-            print(fragment.content[over255])
+            # ~ print(over255)
+            # ~ print(fragment.content[over255])
             fragment.content = fragment.content.astype(np.uint16)
             fragment.content[over255] = 256
-            print(fragment.content[over255])
+            # ~ print(fragment.content[over255])
             data_fragments.append((idx+1,fragment.content))
             count+=1
         else: 
             break
         
     if count<m: 
         raise ValueError("There are duplicate fragments. The total number of different fragments are insufficient to assemble the file.")
     
-    return (m_, n_, p_, data_fragments, )
+    return (m_, n_, p_, data_fragments, )
```

### Comparing `drex-0.0.245/drex/utils/reliability/ida.py` & `drex-0.0.246/drex/utils/reliability/ida.py`

 * *Files identical despite different names*

### Comparing `drex-0.0.245/drex/utils/reliability/utils.py` & `drex-0.0.246/drex/utils/reliability/utils.py`

 * *Files identical despite different names*

### Comparing `drex-0.0.245/drex/utils/tool_functions.py` & `drex-0.0.246/drex/utils/tool_functions.py`

 * *Files 11% similar despite different names*

```diff
@@ -315,17 +315,34 @@
                 set_of_nodes.remove(j)
         index_in_tab += 1
                 # deleted_nodes += 1
     return reduced_set_of_nodes
     
 def update_node_sizes(set_of_nodes_chosen, K, file_size, node_sizes):
 	for i in set_of_nodes_chosen:
-		node_sizes[i] = node_sizes[i] - file_size/K
+		node_sizes[i] = node_sizes[i] - (file_size)/K
 	return node_sizes
 
+def probability_of_failure(failure_rate, data_duration_on_system):
+    """
+    Calculate the probability of failure over a given period given the annual failure rate.
+
+    Parameters:
+    failure_rate (float): Annual failure rate as a percentage (e.g., 5 for 5%).
+    data_duration_on_system (int): Time period in days that the data must remain on the system. Default is 1 year.
+
+    Returns:
+    float: Probability of failure over the given period.
+    """
+    data_duration_on_system = data_duration_on_system/365 # Convert in years
+    lambda_rate = failure_rate / 100
+    probability_failure = 1 - math.exp(-lambda_rate * data_duration_on_system)
+    return probability_failure
+
+
 def exponential_function(x, x1, y1, x2, y2):
     """
     x is the free memory on the node
     Example usage of exponential for algorithm 4
 	x1 = 100 # max node
 	y1 = 1
 	x2 = 10 # min data
```

### Comparing `drex-0.0.245/drex.egg-info/PKG-INFO` & `drex-0.0.246/drex.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drex
-Version: 0.0.245
+Version: 0.0.246
 Summary: DRex package
 Author-email: "Maxime, Dante, Haochen" <dantsanc@pa.uc3m.es>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `drex-0.0.245/pyproject.toml` & `drex-0.0.246/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=64.0", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "drex"
-version = "0.0.245"
+version = "0.0.246"
 authors = [
   { name="Maxime, Dante, Haochen", email="dantsanc@pa.uc3m.es" },
 ]
 description = "DRex package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `drex-0.0.245/test/drex-test.py` & `drex-0.0.246/test/drex-test.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,35 +20,37 @@
 set_of_nodes = list(range(0, number_of_nodes))
 print("There are", number_of_nodes, "nodes.")
 
 # Numpy arrays of probability of failure each node over the data timeframe
 p = []
 for i in range(0, number_of_nodes):
     p.append(random.uniform(0.1, 0.15))
+# ~ p = [0.1, 0.8, 0.7, 0.9, 0.9, 0.05, 0.9, 0.8, 0.9, 0.9]
+
 # Bandwidth to write on the storage nodes in MB/s
 bandwidths = []
 for i in range(0, number_of_nodes):
     bandwidths.append(random.uniform(10, 15))
 
-# Storage size of each node
+# Storage size of each node in B
 node_sizes = []  # Node sizes updated with data
 total_node_size = 0
 for i in range(0, number_of_nodes):
-    node_sizes.append(random.uniform(600, 800))
+    node_sizes.append(random.uniform(600, 800)*1024*1024)
     total_node_size += node_sizes[i]
 max_node_size = max(node_sizes)
 
 # Threshold we want to meet
 reliability_threshold = 0.99
 
 # To manage the real time obtained in experiments
 real_records = RealRecords(dir_data="data/")
 
 # File size in MB
-file_size = 200.4
+file_size = 5
 # TODO update this value when new data arrives in the system or if we have access to all data sizes
 min_data_size = file_size
 
 predictor = Predictor()  # Update for different file sizes
 
 # We need to allow a maximum difference allowed to consider two nodes are similar
 maximum_difference_allowed = 0.20  # 10%
@@ -126,26 +128,25 @@
 """
 # ~ set_of_nodes_chosen, N, K, node_sizes = random_schedule(number_of_nodes, p, reliability_threshold, node_sizes, file_size)
 
 """
 HDFS replicate everything three times
 Time for 100 nodes: 0 seconds
 """
-set_of_nodes_chosen, N, K, node_sizes = hdfs_three_replications(number_of_nodes, reliability_threshold, p, node_sizes, file_size, bandwidths, "simulation")
+# ~ set_of_nodes_chosen, N, K, node_sizes = hdfs_three_replications(number_of_nodes, reliability_threshold, p, node_sizes, file_size, bandwidths, "simulation")
 # ~ set_of_nodes_chosen, node_sizes, size_to_remove_from_nodes = hdfs_three_replications(number_of_nodes, reliability_threshold, p, node_sizes, file_size, bandwidths, "real")
 
-print(set_of_nodes_chosen, N, K, node_sizes)
-
 """
 HDFS with Reed-Solomon
 RS1 and RS2 corresponds the value in RS(x,y) meaning that for RS1 data block 
 you have RS2 parity blocks
 Please provide a mode being either "simulation" or "real" to indicate if you want the 
 real value of K (a float) or a rounded value for real experiments (an integer)
 Time for 100 nodes: seconds
 """
-RS1 = 10
-RS2 = 4
+# ~ RS1 = 10
+# ~ RS2 = 4
 # ~ RS1 = 6
 # ~ RS2 = 3
-#set_of_nodes_chosen, N, K, node_sizes = hdfs_reed_solomon(number_of_nodes, reliability_threshold, p, node_sizes, file_size, bandwidths, RS1, RS2, "simulation")
-#set_of_nodes_chosen, node_sizes, size_to_remove_from_nodes = hdfs_reed_solomon(number_of_nodes, reliability_threshold, p, node_sizes, file_size, bandwidths, RS1, RS2, "real")
+RS1 = 6
+RS2 = 3
+set_of_nodes_chosen, N, K, node_sizes, size_to_remove_from_nodes = hdfs_reed_solomon(number_of_nodes, reliability_threshold, p, node_sizes, file_size, bandwidths, RS1, RS2)
```

### Comparing `drex-0.0.245/test/hdfs-test.py` & `drex-0.0.246/test/hdfs-test.py`

 * *Files identical despite different names*

### Comparing `drex-0.0.245/test/test-ida.py` & `drex-0.0.246/test/test-ida.py`

 * *Files identical despite different names*

### Comparing `drex-0.0.245/test/test-ida2.py` & `drex-0.0.246/test/test-ida2.py`

 * *Files identical despite different names*

### Comparing `drex-0.0.245/test/test_linearregression.py` & `drex-0.0.246/test/test_linearregression.py`

 * *Files identical despite different names*

