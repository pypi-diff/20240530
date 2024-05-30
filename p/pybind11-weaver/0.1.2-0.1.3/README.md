# Comparing `tmp/pybind11_weaver-0.1.2.tar.gz` & `tmp/pybind11_weaver-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybind11_weaver-0.1.2.tar", last modified: Mon Oct 30 08:22:36 2023, max compression
+gzip compressed data, was "pybind11_weaver-0.1.3.tar", last modified: Thu May 30 06:40:43 2024, max compression
```

## Comparing `pybind11_weaver-0.1.2.tar` & `pybind11_weaver-0.1.3.tar`

### file list

```diff
@@ -1,65 +1,72 @@
-drwxr-xr-x   0 edi       (1000) edi       (1000)        0 2023-10-30 08:22:36.736687 pybind11_weaver-0.1.2/
--rw-r--r--   0 edi       (1000) edi       (1000)       18 2023-09-03 13:56:40.000000 pybind11_weaver-0.1.2/.clang-format
--rw-r--r--   0 edi       (1000) edi       (1000)     3085 2023-09-03 05:19:20.000000 pybind11_weaver-0.1.2/.gitignore
--rw-r--r--   0 edi       (1000) edi       (1000)      193 2023-10-28 10:10:33.000000 pybind11_weaver-0.1.2/CMakeLists.txt
--rw-r--r--   0 edi       (1000) edi       (1000)     1068 2023-09-03 04:36:12.000000 pybind11_weaver-0.1.2/LICENSE
--rw-r--r--   0 edi       (1000) edi       (1000)       45 2023-09-03 04:36:12.000000 pybind11_weaver-0.1.2/MANIFEST.in
--rw-r--r--   0 edi       (1000) edi       (1000)     8849 2023-10-30 08:22:36.736687 pybind11_weaver-0.1.2/PKG-INFO
--rw-r--r--   0 edi       (1000) edi       (1000)     7807 2023-10-29 14:04:03.000000 pybind11_weaver-0.1.2/README.md
--rwxr-xr-x   0 edi       (1000) edi       (1000)      355 2023-10-28 10:21:01.000000 pybind11_weaver-0.1.2/build.sh
-drwxr-xr-x   0 edi       (1000) edi       (1000)        0 2023-10-30 08:22:36.726687 pybind11_weaver-0.1.2/pybind11_weaver/
--rw-r--r--   0 edi       (1000) edi       (1000)      138 2023-10-30 08:21:48.000000 pybind11_weaver-0.1.2/pybind11_weaver/__init__.py
--rw-r--r--   0 edi       (1000) edi       (1000)     4748 2023-10-26 12:23:02.000000 pybind11_weaver-0.1.2/pybind11_weaver/config.py
-drwxr-xr-x   0 edi       (1000) edi       (1000)        0 2023-10-30 08:22:36.726687 pybind11_weaver-0.1.2/pybind11_weaver/entity/
--rw-r--r--   0 edi       (1000) edi       (1000)     1226 2023-10-29 11:41:03.000000 pybind11_weaver-0.1.2/pybind11_weaver/entity/__init__.py
--rw-r--r--   0 edi       (1000) edi       (1000)     3559 2023-10-29 08:28:16.000000 pybind11_weaver-0.1.2/pybind11_weaver/entity/entity_base.py
--rw-r--r--   0 edi       (1000) edi       (1000)     1397 2023-10-27 21:50:07.000000 pybind11_weaver-0.1.2/pybind11_weaver/entity/enum.py
--rw-r--r--   0 edi       (1000) edi       (1000)     2222 2023-10-28 00:41:08.000000 pybind11_weaver-0.1.2/pybind11_weaver/entity/funktion.py
-drwxr-xr-x   0 edi       (1000) edi       (1000)        0 2023-10-30 08:22:36.736687 pybind11_weaver-0.1.2/pybind11_weaver/entity/klass/
--rw-r--r--   0 edi       (1000) edi       (1000)       31 2023-10-26 12:23:02.000000 pybind11_weaver-0.1.2/pybind11_weaver/entity/klass/__init__.py
--rw-r--r--   0 edi       (1000) edi       (1000)     1990 2023-10-28 09:41:10.000000 pybind11_weaver-0.1.2/pybind11_weaver/entity/klass/field.py
--rw-r--r--   0 edi       (1000) edi       (1000)     6455 2023-10-29 08:28:16.000000 pybind11_weaver-0.1.2/pybind11_weaver/entity/klass/klass.py
--rw-r--r--   0 edi       (1000) edi       (1000)     4003 2023-10-30 01:43:25.000000 pybind11_weaver-0.1.2/pybind11_weaver/entity/klass/method.py
--rw-r--r--   0 edi       (1000) edi       (1000)     6354 2023-10-30 08:13:41.000000 pybind11_weaver-0.1.2/pybind11_weaver/entity/klass/trampoline.py
--rw-r--r--   0 edi       (1000) edi       (1000)     1014 2023-10-26 12:23:02.000000 pybind11_weaver-0.1.2/pybind11_weaver/entity/namespace.py
--rw-r--r--   0 edi       (1000) edi       (1000)     6220 2023-10-29 02:39:49.000000 pybind11_weaver-0.1.2/pybind11_weaver/entity_tree.py
--rw-r--r--   0 edi       (1000) edi       (1000)     7993 2023-10-30 05:18:57.000000 pybind11_weaver-0.1.2/pybind11_weaver/gen_code.py
--rw-r--r--   0 edi       (1000) edi       (1000)     2691 2023-10-28 07:02:34.000000 pybind11_weaver-0.1.2/pybind11_weaver/gen_unit.py
-drwxr-xr-x   0 edi       (1000) edi       (1000)        0 2023-10-30 08:22:36.726687 pybind11_weaver-0.1.2/pybind11_weaver/include/
-drwxr-xr-x   0 edi       (1000) edi       (1000)        0 2023-10-30 08:22:36.736687 pybind11_weaver-0.1.2/pybind11_weaver/include/pybind11_weaver/
--rw-r--r--   0 edi       (1000) edi       (1000)     7136 2023-10-28 08:56:50.000000 pybind11_weaver-0.1.2/pybind11_weaver/include/pybind11_weaver/pybind11_weaver.h
--rw-r--r--   0 edi       (1000) edi       (1000)      929 2023-10-23 04:05:29.000000 pybind11_weaver-0.1.2/pybind11_weaver/main.py
-drwxr-xr-x   0 edi       (1000) edi       (1000)        0 2023-10-30 08:22:36.736687 pybind11_weaver-0.1.2/pybind11_weaver/third_party/
--rw-r--r--   0 edi       (1000) edi       (1000)     1163 2023-09-03 04:36:12.000000 pybind11_weaver-0.1.2/pybind11_weaver/third_party/ccsyspath.py
-drwxr-xr-x   0 edi       (1000) edi       (1000)        0 2023-10-30 08:22:36.736687 pybind11_weaver-0.1.2/pybind11_weaver/utils/
--rw-r--r--   0 edi       (1000) edi       (1000)     8749 2023-10-30 08:15:48.000000 pybind11_weaver-0.1.2/pybind11_weaver/utils/common.py
--rw-r--r--   0 edi       (1000) edi       (1000)    12999 2023-10-28 08:52:10.000000 pybind11_weaver-0.1.2/pybind11_weaver/utils/fn.py
--rw-r--r--   0 edi       (1000) edi       (1000)      879 2023-10-27 03:12:38.000000 pybind11_weaver-0.1.2/pybind11_weaver/utils/scope_list.py
-drwxr-xr-x   0 edi       (1000) edi       (1000)        0 2023-10-30 08:22:36.726687 pybind11_weaver-0.1.2/pybind11_weaver.egg-info/
--rw-r--r--   0 edi       (1000) edi       (1000)     8849 2023-10-30 08:22:36.000000 pybind11_weaver-0.1.2/pybind11_weaver.egg-info/PKG-INFO
--rw-r--r--   0 edi       (1000) edi       (1000)     1518 2023-10-30 08:22:36.000000 pybind11_weaver-0.1.2/pybind11_weaver.egg-info/SOURCES.txt
--rw-r--r--   0 edi       (1000) edi       (1000)        1 2023-10-30 08:22:36.000000 pybind11_weaver-0.1.2/pybind11_weaver.egg-info/dependency_links.txt
--rw-r--r--   0 edi       (1000) edi       (1000)       62 2023-10-30 08:22:36.000000 pybind11_weaver-0.1.2/pybind11_weaver.egg-info/entry_points.txt
--rw-r--r--   0 edi       (1000) edi       (1000)        1 2023-10-30 08:22:36.000000 pybind11_weaver-0.1.2/pybind11_weaver.egg-info/not-zip-safe
--rw-r--r--   0 edi       (1000) edi       (1000)       33 2023-10-30 08:22:36.000000 pybind11_weaver-0.1.2/pybind11_weaver.egg-info/requires.txt
--rw-r--r--   0 edi       (1000) edi       (1000)       16 2023-10-30 08:22:36.000000 pybind11_weaver-0.1.2/pybind11_weaver.egg-info/top_level.txt
--rw-r--r--   0 edi       (1000) edi       (1000)     1369 2023-10-29 13:37:08.000000 pybind11_weaver-0.1.2/pyproject.toml
-drwxr-xr-x   0 edi       (1000) edi       (1000)        0 2023-10-30 08:22:36.726687 pybind11_weaver-0.1.2/sample/
-drwxr-xr-x   0 edi       (1000) edi       (1000)        0 2023-10-30 08:22:36.736687 pybind11_weaver-0.1.2/sample/all_feature/
--rw-r--r--   0 edi       (1000) edi       (1000)     1822 2023-10-28 02:29:57.000000 pybind11_weaver-0.1.2/sample/all_feature/binding.cc
--rw-r--r--   0 edi       (1000) edi       (1000)      205 2023-10-26 12:23:02.000000 pybind11_weaver-0.1.2/sample/all_feature/cfg.yaml
--rw-r--r--   0 edi       (1000) edi       (1000)       94 2023-09-04 07:00:35.000000 pybind11_weaver-0.1.2/sample/all_feature/generate.sh
--rw-r--r--   0 edi       (1000) edi       (1000)     1522 2023-10-28 02:55:38.000000 pybind11_weaver-0.1.2/sample/all_feature/sample.cc
--rw-r--r--   0 edi       (1000) edi       (1000)     3247 2023-10-30 04:21:34.000000 pybind11_weaver-0.1.2/sample/all_feature/sample.h
--rw-r--r--   0 edi       (1000) edi       (1000)    60960 2023-10-30 08:21:10.000000 pybind11_weaver-0.1.2/sample/all_feature/sample_binding.cc.inc
--rw-r--r--   0 edi       (1000) edi       (1000)      868 2023-10-29 09:05:41.000000 pybind11_weaver-0.1.2/sample/all_feature/template_pb11_weaver_helper.h
--rw-r--r--   0 edi       (1000) edi       (1000)       49 2023-10-26 12:23:02.000000 pybind11_weaver-0.1.2/sample/all_feature/un_export.h
-drwxr-xr-x   0 edi       (1000) edi       (1000)        0 2023-10-30 08:22:36.736687 pybind11_weaver-0.1.2/sample/config/
--rw-r--r--   0 edi       (1000) edi       (1000)     1568 2023-10-23 08:32:38.000000 pybind11_weaver-0.1.2/sample/config/all_with_doc.yaml
--rw-r--r--   0 edi       (1000) edi       (1000)       38 2023-10-30 08:22:36.736687 pybind11_weaver-0.1.2/setup.cfg
-drwxr-xr-x   0 edi       (1000) edi       (1000)        0 2023-10-30 08:22:36.736687 pybind11_weaver-0.1.2/test/
--rw-r--r--   0 edi       (1000) edi       (1000)      621 2023-10-23 04:05:29.000000 pybind11_weaver-0.1.2/test/CMakeLists.txt
--rw-r--r--   0 edi       (1000) edi       (1000)     3097 2023-10-26 12:23:02.000000 pybind11_weaver-0.1.2/test/gen_unit_test.py
-drwxr-xr-x   0 edi       (1000) edi       (1000)        0 2023-10-30 08:22:36.736687 pybind11_weaver-0.1.2/test/sample_test/
--rw-r--r--   0 edi       (1000) edi       (1000)      980 2023-10-26 12:23:02.000000 pybind11_weaver-0.1.2/test/sample_test/CMakeLists.txt
--rw-r--r--   0 edi       (1000) edi       (1000)     4372 2023-10-29 11:22:41.000000 pybind11_weaver-0.1.2/test/sample_test/launch_module.py
+drwxr-xr-x   0 edi       (1000) edi       (1000)        0 2024-05-30 06:40:43.498525 pybind11_weaver-0.1.3/
+-rw-r--r--   0 edi       (1000) edi       (1000)       18 2023-09-03 13:56:40.000000 pybind11_weaver-0.1.3/.clang-format
+-rw-r--r--   0 edi       (1000) edi       (1000)     3085 2023-09-03 05:19:20.000000 pybind11_weaver-0.1.3/.gitignore
+-rw-r--r--   0 edi       (1000) edi       (1000)     1167 2023-10-31 03:46:11.000000 pybind11_weaver-0.1.3/CMakeLists.txt
+-rw-r--r--   0 edi       (1000) edi       (1000)     1068 2023-09-03 04:36:12.000000 pybind11_weaver-0.1.3/LICENSE
+-rw-r--r--   0 edi       (1000) edi       (1000)       45 2023-09-03 04:36:12.000000 pybind11_weaver-0.1.3/MANIFEST.in
+-rw-r--r--   0 edi       (1000) edi       (1000)     8467 2024-05-30 06:40:43.498525 pybind11_weaver-0.1.3/PKG-INFO
+-rw-r--r--   0 edi       (1000) edi       (1000)     7425 2023-11-06 02:45:37.000000 pybind11_weaver-0.1.3/README.md
+-rwxr-xr-x   0 edi       (1000) edi       (1000)      355 2023-10-28 10:21:01.000000 pybind11_weaver-0.1.3/build.sh
+drwxr-xr-x   0 edi       (1000) edi       (1000)        0 2024-05-30 06:40:43.488525 pybind11_weaver-0.1.3/pybind11_weaver/
+-rw-r--r--   0 edi       (1000) edi       (1000)      138 2024-05-30 06:40:35.000000 pybind11_weaver-0.1.3/pybind11_weaver/__init__.py
+-rw-r--r--   0 edi       (1000) edi       (1000)     5510 2024-05-26 10:52:48.000000 pybind11_weaver-0.1.3/pybind11_weaver/config.py
+drwxr-xr-x   0 edi       (1000) edi       (1000)        0 2024-05-30 06:40:43.488525 pybind11_weaver-0.1.3/pybind11_weaver/entity/
+-rw-r--r--   0 edi       (1000) edi       (1000)     1226 2023-10-29 11:41:03.000000 pybind11_weaver-0.1.3/pybind11_weaver/entity/__init__.py
+-rw-r--r--   0 edi       (1000) edi       (1000)     4141 2024-05-26 08:35:06.000000 pybind11_weaver-0.1.3/pybind11_weaver/entity/entity_base.py
+-rw-r--r--   0 edi       (1000) edi       (1000)     1405 2024-05-26 08:35:06.000000 pybind11_weaver-0.1.3/pybind11_weaver/entity/enum.py
+-rw-r--r--   0 edi       (1000) edi       (1000)     2222 2023-10-28 00:41:08.000000 pybind11_weaver-0.1.3/pybind11_weaver/entity/funktion.py
+drwxr-xr-x   0 edi       (1000) edi       (1000)        0 2024-05-30 06:40:43.488525 pybind11_weaver-0.1.3/pybind11_weaver/entity/klass/
+-rw-r--r--   0 edi       (1000) edi       (1000)       31 2023-10-26 12:23:02.000000 pybind11_weaver-0.1.3/pybind11_weaver/entity/klass/__init__.py
+-rw-r--r--   0 edi       (1000) edi       (1000)     1996 2024-05-27 03:59:21.000000 pybind11_weaver-0.1.3/pybind11_weaver/entity/klass/field.py
+-rw-r--r--   0 edi       (1000) edi       (1000)     6471 2024-05-26 08:35:06.000000 pybind11_weaver-0.1.3/pybind11_weaver/entity/klass/klass.py
+-rw-r--r--   0 edi       (1000) edi       (1000)     4003 2023-10-30 01:43:25.000000 pybind11_weaver-0.1.3/pybind11_weaver/entity/klass/method.py
+-rw-r--r--   0 edi       (1000) edi       (1000)     6378 2024-05-26 08:35:06.000000 pybind11_weaver-0.1.3/pybind11_weaver/entity/klass/trampoline.py
+-rw-r--r--   0 edi       (1000) edi       (1000)     1022 2024-05-26 08:35:06.000000 pybind11_weaver-0.1.3/pybind11_weaver/entity/namespace.py
+-rw-r--r--   0 edi       (1000) edi       (1000)     9312 2024-05-30 06:37:32.000000 pybind11_weaver-0.1.3/pybind11_weaver/entity_tree.py
+-rw-r--r--   0 edi       (1000) edi       (1000)     7992 2024-05-26 08:35:06.000000 pybind11_weaver-0.1.3/pybind11_weaver/gen_code.py
+-rw-r--r--   0 edi       (1000) edi       (1000)     2690 2024-05-26 08:35:06.000000 pybind11_weaver-0.1.3/pybind11_weaver/gen_unit.py
+drwxr-xr-x   0 edi       (1000) edi       (1000)        0 2024-05-30 06:40:43.488525 pybind11_weaver-0.1.3/pybind11_weaver/include/
+drwxr-xr-x   0 edi       (1000) edi       (1000)        0 2024-05-30 06:40:43.498525 pybind11_weaver-0.1.3/pybind11_weaver/include/pybind11_weaver/
+-rw-r--r--   0 edi       (1000) edi       (1000)     7136 2023-10-28 08:56:50.000000 pybind11_weaver-0.1.3/pybind11_weaver/include/pybind11_weaver/pybind11_weaver.h
+-rw-r--r--   0 edi       (1000) edi       (1000)      929 2023-10-23 04:05:29.000000 pybind11_weaver-0.1.3/pybind11_weaver/main.py
+drwxr-xr-x   0 edi       (1000) edi       (1000)        0 2024-05-30 06:40:43.498525 pybind11_weaver-0.1.3/pybind11_weaver/third_party/
+-rw-r--r--   0 edi       (1000) edi       (1000)     1163 2023-09-03 04:36:12.000000 pybind11_weaver-0.1.3/pybind11_weaver/third_party/ccsyspath.py
+drwxr-xr-x   0 edi       (1000) edi       (1000)        0 2024-05-30 06:40:43.498525 pybind11_weaver-0.1.3/pybind11_weaver/utils/
+-rw-r--r--   0 edi       (1000) edi       (1000)     8914 2024-05-27 02:23:45.000000 pybind11_weaver-0.1.3/pybind11_weaver/utils/common.py
+-rw-r--r--   0 edi       (1000) edi       (1000)    12999 2023-10-28 08:52:10.000000 pybind11_weaver-0.1.3/pybind11_weaver/utils/fn.py
+-rw-r--r--   0 edi       (1000) edi       (1000)      877 2024-05-30 06:37:59.000000 pybind11_weaver-0.1.3/pybind11_weaver/utils/scope_list.py
+drwxr-xr-x   0 edi       (1000) edi       (1000)        0 2024-05-30 06:40:43.498525 pybind11_weaver-0.1.3/pybind11_weaver.egg-info/
+-rw-r--r--   0 edi       (1000) edi       (1000)     8467 2024-05-30 06:40:43.000000 pybind11_weaver-0.1.3/pybind11_weaver.egg-info/PKG-INFO
+-rw-r--r--   0 edi       (1000) edi       (1000)     1685 2024-05-30 06:40:43.000000 pybind11_weaver-0.1.3/pybind11_weaver.egg-info/SOURCES.txt
+-rw-r--r--   0 edi       (1000) edi       (1000)        1 2024-05-30 06:40:43.000000 pybind11_weaver-0.1.3/pybind11_weaver.egg-info/dependency_links.txt
+-rw-r--r--   0 edi       (1000) edi       (1000)       62 2024-05-30 06:40:43.000000 pybind11_weaver-0.1.3/pybind11_weaver.egg-info/entry_points.txt
+-rw-r--r--   0 edi       (1000) edi       (1000)        1 2024-05-30 06:40:43.000000 pybind11_weaver-0.1.3/pybind11_weaver.egg-info/not-zip-safe
+-rw-r--r--   0 edi       (1000) edi       (1000)       33 2024-05-30 06:40:43.000000 pybind11_weaver-0.1.3/pybind11_weaver.egg-info/requires.txt
+-rw-r--r--   0 edi       (1000) edi       (1000)       16 2024-05-30 06:40:43.000000 pybind11_weaver-0.1.3/pybind11_weaver.egg-info/top_level.txt
+-rw-r--r--   0 edi       (1000) edi       (1000)     1352 2023-11-06 02:31:18.000000 pybind11_weaver-0.1.3/pyproject.toml
+-rw-r--r--   0 edi       (1000) edi       (1000)       32 2023-11-06 02:30:25.000000 pybind11_weaver-0.1.3/requirements.txt
+drwxr-xr-x   0 edi       (1000) edi       (1000)        0 2024-05-30 06:40:43.498525 pybind11_weaver-0.1.3/sample/
+-rw-r--r--   0 edi       (1000) edi       (1000)       29 2023-10-31 01:38:22.000000 pybind11_weaver-0.1.3/sample/CMakeLists.txt
+drwxr-xr-x   0 edi       (1000) edi       (1000)        0 2024-05-30 06:40:43.498525 pybind11_weaver-0.1.3/sample/all_feature/
+-rw-r--r--   0 edi       (1000) edi       (1000)      179 2023-10-31 03:33:20.000000 pybind11_weaver-0.1.3/sample/all_feature/CMakeLists.txt
+-rw-r--r--   0 edi       (1000) edi       (1000)    60713 2024-05-30 06:31:05.000000 pybind11_weaver-0.1.3/sample/all_feature/_binding.cc.inc
+-rw-r--r--   0 edi       (1000) edi       (1000)     1809 2023-10-31 03:06:18.000000 pybind11_weaver-0.1.3/sample/all_feature/binding.cc
+drwxr-xr-x   0 edi       (1000) edi       (1000)        0 2024-05-30 06:40:43.498525 pybind11_weaver-0.1.3/sample/all_feature/c_lib/
+-rw-r--r--   0 edi       (1000) edi       (1000)       46 2023-10-31 03:20:28.000000 pybind11_weaver-0.1.3/sample/all_feature/c_lib/CMakeLists.txt
+-rw-r--r--   0 edi       (1000) edi       (1000)     1521 2023-10-31 03:00:07.000000 pybind11_weaver-0.1.3/sample/all_feature/c_lib/c_lib.cc
+-rw-r--r--   0 edi       (1000) edi       (1000)     3250 2024-05-27 12:22:32.000000 pybind11_weaver-0.1.3/sample/all_feature/c_lib/c_lib.h
+-rw-r--r--   0 edi       (1000) edi       (1000)       49 2023-10-26 12:23:02.000000 pybind11_weaver-0.1.3/sample/all_feature/c_lib/not_exported.h
+-rw-r--r--   0 edi       (1000) edi       (1000)      204 2023-10-31 03:12:14.000000 pybind11_weaver-0.1.3/sample/all_feature/cfg.yaml
+-rw-r--r--   0 edi       (1000) edi       (1000)      873 2024-05-26 08:30:31.000000 pybind11_weaver-0.1.3/sample/all_feature/template_pb11_weaver_helper.h
+-rw-r--r--   0 edi       (1000) edi       (1000)       38 2024-05-30 06:40:43.498525 pybind11_weaver-0.1.3/setup.cfg
+drwxr-xr-x   0 edi       (1000) edi       (1000)        0 2024-05-30 06:40:43.498525 pybind11_weaver-0.1.3/test/
+-rw-r--r--   0 edi       (1000) edi       (1000)      133 2023-10-31 03:50:19.000000 pybind11_weaver-0.1.3/test/CMakeLists.txt
+drwxr-xr-x   0 edi       (1000) edi       (1000)        0 2024-05-30 06:40:43.498525 pybind11_weaver-0.1.3/test/config/
+-rw-r--r--   0 edi       (1000) edi       (1000)     2470 2023-11-02 11:22:45.000000 pybind11_weaver-0.1.3/test/config/config_with_doc.yaml
+-rw-r--r--   0 edi       (1000) edi       (1000)     3330 2023-11-02 15:45:11.000000 pybind11_weaver-0.1.3/test/config/test_config.py
+-rw-r--r--   0 edi       (1000) edi       (1000)      513 2023-11-02 02:55:52.000000 pybind11_weaver-0.1.3/test/gen_unit_test.py
+drwxr-xr-x   0 edi       (1000) edi       (1000)        0 2024-05-30 06:40:43.498525 pybind11_weaver-0.1.3/test/sample/
+-rw-r--r--   0 edi       (1000) edi       (1000)       29 2023-10-31 03:24:00.000000 pybind11_weaver-0.1.3/test/sample/CMakeLists.txt
+drwxr-xr-x   0 edi       (1000) edi       (1000)        0 2024-05-30 06:40:43.498525 pybind11_weaver-0.1.3/test/sample/all_feature/
+-rw-r--r--   0 edi       (1000) edi       (1000)      753 2023-10-31 04:00:20.000000 pybind11_weaver-0.1.3/test/sample/all_feature/CMakeLists.txt
+-rw-r--r--   0 edi       (1000) edi       (1000)     4396 2023-10-31 04:09:58.000000 pybind11_weaver-0.1.3/test/sample/all_feature/test_all_feature.py
```

### Comparing `pybind11_weaver-0.1.2/.gitignore` & `pybind11_weaver-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pybind11_weaver-0.1.2/LICENSE` & `pybind11_weaver-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pybind11_weaver-0.1.2/PKG-INFO` & `pybind11_weaver-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybind11_weaver
-Version: 0.1.2
+Version: 0.1.3
 Summary: A fully customizable pybind11 generator to help generate code for exsiting c/c++ library.
 License: MIT
 Project-URL: Homepage, https://github.com/edimetia3d/pybind11_weaver
 Project-URL: Documentation, https://github.com/edimetia3d/pybind11_weaver
 Project-URL: Repository, https://github.com/edimetia3d/pybind11_weaver
 Project-URL: Changelog, https://github.com/edimetia3d/pybind11_weaver/releases
 Keywords: pybind11,generator,codegen,gen
@@ -25,22 +25,23 @@
 
 # Pybind11 Weaver: Python Binding Code Generator
 
 **Pybind11 Weaver** is a powerful code generator designed to automate the generation of pybind11 code from C++ header
 files. It streamlines the process of creating Python bindings, enabling users to focus on writing critical pybind11 code
 and offloading the tedious work to Pybind11 Weaver.
 
-This tool takes a [sample.h](https://github.com/edimetia3d/pybind11_weaver/blob/main/sample/all_feature/sample.h) file
+This tool takes a [c_lib.h](https://github.com/edimetia3d/pybind11_weaver/blob/main/sample/all_feature/c_lib/c_lib.h)
+file
 and transforms it into
-a [sample_binding.cc.inc](https://github.com/edimetia3d/pybind11_weaver/blob/main/sample/all_feature/sample_binding.cc.inc)
+a [_binding.cc.inc](https://github.com/edimetia3d/pybind11_weaver/blob/main/sample/all_feature/_binding.cc.inc)
 file using [cfg.yaml](https://github.com/edimetia3d/pybind11_weaver/blob/main/sample/all_feature/cfg.yaml) as a guide.
 Following the binding with a single line `auto update_guard = DeclFn(m);`
 in [binding.cc](https://github.com/edimetia3d/pybind11_weaver/blob/main/sample/all_feature/binding.cc), all elements
 from the header file become accessible in Python as demonstrated in
-this [example](https://github.com/edimetia3d/pybind11_weaver/blob/main/test/sample_test/launch_module.py).
+this [example](https://github.com/edimetia3d/pybind11_weaver/blob/main/test/sample/all_feature/test_all_feature.py).
 
 A more pragmatic example is available in [pylibclang](https://github.com/edimetia3d/pylibclang), a comprehensive Python
 wrapper for libclang that uses Pybind11 Weaver to generate the binding code.
 
 1. Its practicality stems from the fact that **Pybind11 Weaver operates on it** as well. Indeed, Pybind11 Weaver is
    self-hosted and generates the binding code for its own use.
 2. Approximately 30k lines of C++ code are generated from a mere 10 lines
@@ -48,14 +49,18 @@
 3. Some [binding code](https://github.com/edimetia3d/pylibclang/blob/master/c_src/binding.cc) is manually crafted to
    handle special cases and integrates seamlessly with the generated code.
 
 [pylibtooling](https://github.com/edimetia3d/pylibtooling) is a much more advanced example that uses Pybind11 Weaver to
 generate the binding code for [libtooling](https://clang.llvm.org/docs/LibTooling.html), and will be used to demonstrate
 the capabilities of Pybind11 Weaver when working with large C++ only libraries.
 
+## Docs
+
+Check https://github.com/edimetia3d/pybind11_weaver/wiki
+
 ## Key Features
 
 1. **Highly Customizable:** While the default configuration is super simple and suitable for most cases, it allows for
    high customization.
 2. **Ease of Use:** As a pure Python package, a simple `pip install` gets it ready to work.
 3. **Versatility:** All generated code is under your control, you can easily modify/enhance/disable any part of
    generated
@@ -118,38 +123,14 @@
 6. Compile all code into a pybind11 module.
 7. Optionally, use [pybind11-stubgen](https://github.com/sizmailov/pybind11-stubgen) to generate `.pyi` stub files,
    enhancing readability for both humans and MYPY in a static way.
 8. Test the module in Python, find bugs, and go to step 5 to fix them.
 
 Also, if you encountered too many problems, you are welcome to open an issue at github, or create a PR to fix it.
 
-## Installation
-
-### Via PYPI
-
-```bash
-python3 -m pip install pybind11-weaver
-```
-
-### From Source
-
-* To install from source:
-
-```bash
-git clone https://github.com/edimetia3d/pybind11_weaver
-python3 -m pip install $(pwd)/pybind11_weaver/
-```
-
-* To run from source (Editable/Develop Mode):
-
-```bash
-git clone https://github.com/edimetia3d/pybind11_weaver
-python3 -m pip install -e $(pwd)/pybind11_weaver/ -v --config-settings editable_mode=compat
-```
-
 ## How it works
 
 The Pybind11 Weaver operates under the hood by utilizing [libclang](https://clang.llvm.org/), a library that parses C++
 header files. This enables us to obtain all APIs from the header file, which are then used to generate the binding code
 on your behalf.
 
 Notably, only header files are required, as we need declarations, not definitions. However, to ensure accurate parsing
```

### Comparing `pybind11_weaver-0.1.2/README.md` & `pybind11_weaver-0.1.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # Pybind11 Weaver: Python Binding Code Generator
 
 **Pybind11 Weaver** is a powerful code generator designed to automate the generation of pybind11 code from C++ header
 files. It streamlines the process of creating Python bindings, enabling users to focus on writing critical pybind11 code
 and offloading the tedious work to Pybind11 Weaver.
 
-This tool takes a [sample.h](https://github.com/edimetia3d/pybind11_weaver/blob/main/sample/all_feature/sample.h) file
+This tool takes a [c_lib.h](https://github.com/edimetia3d/pybind11_weaver/blob/main/sample/all_feature/c_lib/c_lib.h)
+file
 and transforms it into
-a [sample_binding.cc.inc](https://github.com/edimetia3d/pybind11_weaver/blob/main/sample/all_feature/sample_binding.cc.inc)
+a [_binding.cc.inc](https://github.com/edimetia3d/pybind11_weaver/blob/main/sample/all_feature/_binding.cc.inc)
 file using [cfg.yaml](https://github.com/edimetia3d/pybind11_weaver/blob/main/sample/all_feature/cfg.yaml) as a guide.
 Following the binding with a single line `auto update_guard = DeclFn(m);`
 in [binding.cc](https://github.com/edimetia3d/pybind11_weaver/blob/main/sample/all_feature/binding.cc), all elements
 from the header file become accessible in Python as demonstrated in
-this [example](https://github.com/edimetia3d/pybind11_weaver/blob/main/test/sample_test/launch_module.py).
+this [example](https://github.com/edimetia3d/pybind11_weaver/blob/main/test/sample/all_feature/test_all_feature.py).
 
 A more pragmatic example is available in [pylibclang](https://github.com/edimetia3d/pylibclang), a comprehensive Python
 wrapper for libclang that uses Pybind11 Weaver to generate the binding code.
 
 1. Its practicality stems from the fact that **Pybind11 Weaver operates on it** as well. Indeed, Pybind11 Weaver is
    self-hosted and generates the binding code for its own use.
 2. Approximately 30k lines of C++ code are generated from a mere 10 lines
@@ -23,14 +24,18 @@
 3. Some [binding code](https://github.com/edimetia3d/pylibclang/blob/master/c_src/binding.cc) is manually crafted to
    handle special cases and integrates seamlessly with the generated code.
 
 [pylibtooling](https://github.com/edimetia3d/pylibtooling) is a much more advanced example that uses Pybind11 Weaver to
 generate the binding code for [libtooling](https://clang.llvm.org/docs/LibTooling.html), and will be used to demonstrate
 the capabilities of Pybind11 Weaver when working with large C++ only libraries.
 
+## Docs
+
+Check https://github.com/edimetia3d/pybind11_weaver/wiki
+
 ## Key Features
 
 1. **Highly Customizable:** While the default configuration is super simple and suitable for most cases, it allows for
    high customization.
 2. **Ease of Use:** As a pure Python package, a simple `pip install` gets it ready to work.
 3. **Versatility:** All generated code is under your control, you can easily modify/enhance/disable any part of
    generated
@@ -93,38 +98,14 @@
 6. Compile all code into a pybind11 module.
 7. Optionally, use [pybind11-stubgen](https://github.com/sizmailov/pybind11-stubgen) to generate `.pyi` stub files,
    enhancing readability for both humans and MYPY in a static way.
 8. Test the module in Python, find bugs, and go to step 5 to fix them.
 
 Also, if you encountered too many problems, you are welcome to open an issue at github, or create a PR to fix it.
 
-## Installation
-
-### Via PYPI
-
-```bash
-python3 -m pip install pybind11-weaver
-```
-
-### From Source
-
-* To install from source:
-
-```bash
-git clone https://github.com/edimetia3d/pybind11_weaver
-python3 -m pip install $(pwd)/pybind11_weaver/
-```
-
-* To run from source (Editable/Develop Mode):
-
-```bash
-git clone https://github.com/edimetia3d/pybind11_weaver
-python3 -m pip install -e $(pwd)/pybind11_weaver/ -v --config-settings editable_mode=compat
-```
-
 ## How it works
 
 The Pybind11 Weaver operates under the hood by utilizing [libclang](https://clang.llvm.org/), a library that parses C++
 header files. This enables us to obtain all APIs from the header file, which are then used to generate the binding code
 on your behalf.
 
 Notably, only header files are required, as we need declarations, not definitions. However, to ensure accurate parsing
```

### Comparing `pybind11_weaver-0.1.2/pybind11_weaver/config.py` & `pybind11_weaver-0.1.3/pybind11_weaver/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from typing import List, Optional
 import glob
 import os
+import sysconfig
+from typing import List
 
-import yaml
 import attrs
-import sysconfig
 import pybind11
+import yaml
+
 import pybind11_weaver.third_party.ccsyspath as ccsyspath
 
 
 @attrs.define
 class IOConfig:
     inputs: List[str] = attrs.field(factory=list)
     output: str = ""
@@ -17,14 +18,16 @@
     root_module_namespace: str = ""
     _cxx_flags: List[str] = None
     extra_cxx_flags: List[str] = attrs.field(factory=list)
     gen_docstring: bool = True
     strict_visibility_mode: bool = False
 
     def normalize(self, common_config: "CommonConfig"):
+        if len(self.inputs) == 0 or self.output == "":
+            raise ValueError("Inputs and output can not be empty")
         self._cxx_flags = common_config.cxx_flags + self.extra_cxx_flags
         self._normalize_inputs()
 
     def _normalize_inputs(self):
         self.inputs = self._to_valid_include_path(self.inputs)
         self._inputs_to_relative_path()
 
@@ -64,70 +67,84 @@
             if f.startswith('"') and os.path.isabs(f[1:-1]):
                 f = f'"{_try_remove_abs_prefix(f[1:-1])}"'
                 self.inputs[i] = f
 
 
 @attrs.define
 class CommonConfig:
-    compiler: Optional[str] = None
+    compiler: str = ""
     cxx_flags: List[str] = attrs.field(factory=list)
     include_directories: List[str] = attrs.field(factory=list)
 
     def normalize(self):
         include_sys_flags = self._get_default_include_flags()
         include_usr_flags = ["-I" + path for path in self.include_directories]
         self.cxx_flags = self.cxx_flags + include_sys_flags + include_usr_flags
 
     def _get_default_include_flags(self) -> List[str]:
         try_to_use = ["c++", "g++", "clang++"]
         if os.environ.get("CXX") is not None:
             try_to_use = [os.environ.get("CXX")] + try_to_use
-        if self.compiler is not None:
+        if self.compiler != "":
             try_to_use = [self.compiler] + try_to_use
         cxx_sys_path = []
         for compiler in try_to_use:
             cxx_sys_path = ccsyspath.system_include_paths(compiler)
             if len(cxx_sys_path) > 0:
                 self.compiler = compiler
                 break
-        assert len(cxx_sys_path) > 0, "Can not find c++ headers"
         full_list = [d.decode("utf-8") for d in cxx_sys_path] + [
             sysconfig.get_path("include"),
             pybind11.get_include(),
         ]
         return ["-I" + path for path in full_list]
 
 
-def _safe_load_one_cls(cls, possible_values):
+def _safe_load_one_cls(cls, name, possible_v):
+    if not attrs.has(cls):
+        if hasattr(cls, "__origin__"):
+            assert cls.__origin__ == list
+            if not isinstance(possible_v, list):
+                raise ValueError(f"Expect '{name}' to be a list, but got {possible_v}")
+            element_t = cls.__args__[0]
+            values = []
+            for v in possible_v:
+                values.append(_safe_load_one_cls(element_t, f"value in {name}", v))
+            return values
+        else:
+            if not isinstance(possible_v, cls):
+                raise ValueError(f"Expect '{name}' to be a {cls}, but got {possible_v}")
+            return possible_v
     instance = cls()
     attrs.resolve_types(cls)
+    if not isinstance(possible_v, dict):
+        raise ValueError(f"Expect '{name}' to be a dict, but got {possible_v}")
     for field in attrs.fields(cls):
-        if field.name in possible_values:
-            if attrs.has(field.type):
-                setattr(instance, field.name,
-                        _safe_load_one_cls(field.type, possible_values[field.name]))
-            else:
-                setattr(instance, field.name, possible_values[field.name])
+        if field.name in possible_v:
+            setattr(instance, field.name,
+                    _safe_load_one_cls(field.type, f"{name}.{field.name}", possible_v[field.name]))
     return instance
 
 
 @attrs.define
 class MainConfig:
     common_config: CommonConfig = attrs.field(factory=CommonConfig)
     io_configs: List[IOConfig] = attrs.Factory(factory=list)
 
     @staticmethod
     def load(file_or_content: str) -> "MainConfig":
+        if len(file_or_content) == 0:
+            raise ValueError("file_or_content can not be empty")
         content = file_or_content
         if os.path.exists(content):  # it is a file
             with open(content, "r") as yml:
                 content = yml.read()
                 content = content.replace("${CFG_DIR}", os.path.dirname(os.path.abspath(file_or_content)))
         cfg = yaml.safe_load(content)
 
-        main_config = _safe_load_one_cls(MainConfig, cfg)
+        main_config = _safe_load_one_cls(MainConfig, "MainConfig", cfg)
         main_config.common_config.normalize()
         for i, io_config in enumerate(main_config.io_configs):
-            new_io_cfg = _safe_load_one_cls(IOConfig, io_config)
-            new_io_cfg.normalize(main_config.common_config)
-            main_config.io_configs[i] = new_io_cfg
+            io_config.normalize(main_config.common_config)
+        if len(main_config.io_configs) == 0:
+            raise ValueError("No IOConfig is specified")
         return main_config
```

### Comparing `pybind11_weaver-0.1.2/pybind11_weaver/entity/__init__.py` & `pybind11_weaver-0.1.3/pybind11_weaver/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `pybind11_weaver-0.1.2/pybind11_weaver/entity/entity_base.py` & `pybind11_weaver-0.1.3/pybind11_weaver/entity/entity_base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import abc
 import functools
-import weakref
 import logging
 from typing import Dict, List
 
 from pylibclang import cindex
 
 from pybind11_weaver import gen_unit
 
@@ -28,55 +27,69 @@
     Parent is responsible to manage the life cycle of its children, and children only hold a weakref to parent.
 
     """
 
     def __init__(self, gu: gen_unit.GenUnit, cursor: cindex.Cursor):
         self.gu = gu
         self.cursor = cursor
-        self._parent = None
         self.children: Dict[str, Entity] = {}
 
     def __contains__(self, item):
         return item in self.children
 
     def __getitem__(self, item: str):
         return self.children[item]
 
     def __setitem__(self, key, value):
         self.children[key] = value
 
-    def add_child(self, child: "Entity"):
-        if child.name in self.children:
-            if child.cursor.kind == cindex.CursorKind.CXCursor_Namespace:
-                assert len(child.children) == 0
-            else:
-                _logger.warning(
-                    f"Entity at {child.cursor.location} already exists, skip, previous one is {self.children[child.name].cursor.location}")
-        else:
-            self.children[child.name] = child
-        assert child.parent() is None
-        child._parent = weakref.ref(self)
-
-    def parent(self):
-        return None if self._parent is None else self._parent()
+    def python_name(self):
+        # todo: implement this, this name is used to access the exported C++ target in python code.
+        pass
 
     @property
     @functools.lru_cache
-    def name(self):
-        """Used to difference different entity instances in the same scope."""
+    def key_in_scope(self):
+        # todo: this could be replaced by reference_name, since that name is more strong unique.
+        """
+        Used as key to difference different entity instances in the same scope.
+
+        If two entity has the same key, it will be treated as a redefinition error when creating the entity tree.
+
+        Note, C++ does allow same name in same scope as long:
+        1. both are declaration
+        2. both are namespace
+        3. function overloading
+
+        In pybind11-weaver, to solve these 3 case, we will
+        1. ignore all redeclaration in same scope
+        2. merge all namespace with the same key
+        3. each function will use their signature as key, so that function overloading will map to different key.
+
+        """
         return self.cursor.displayname
 
     @abc.abstractmethod
     def reference_name(self) -> str:
-        """Used to reference this object in C++ code."""
+        """
+        This name will be used in the generated code to access the C++ target being exported. e.g. if the entity is a c++
+        class, this name will be the fully qualified class name, like `A::C::D::MyClass`
+
+        It is required to reference the c++ target in any place, apparently, this name will always be fully qualified,
+        so it is unique in the whole project.
+
+        """
         pass
 
     @abc.abstractmethod
     def get_pb11weaver_struct_name(self) -> str:
-        """Unique name of the entity, must be able to used as a C++ identifier."""
+        # todo: this name could be mangled from the reference_name.
+        """
+        Unique name of the entity, must be able to used as a C++ identifier.
+        """
         pass
 
     @abc.abstractmethod
     def init_default_pybind11_value(self, parent_scope_sym: str) -> str:
         """ An expression to create pybind 11 object on stack.
         
         Args:
```

### Comparing `pybind11_weaver-0.1.2/pybind11_weaver/entity/enum.py` & `pybind11_weaver-0.1.3/pybind11_weaver/entity/enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     def reference_name(self) -> str:
         return self.cursor.type.spelling
 
     def get_pb11weaver_struct_name(self) -> str:
         return self.cursor.type.spelling.replace("::", "_")
 
     def init_default_pybind11_value(self, parent_scope_sym: str) -> str:
-        code = f"{parent_scope_sym}, \"{self.name}\",pybind11::arithmetic()"
+        code = f"{parent_scope_sym}, \"{self.key_in_scope}\",pybind11::arithmetic()"
         if self.gu.io_config.gen_docstring:
             code = entity_base._inject_docstring(code, self.cursor, "append")
         return code
 
     def update_stmts(self, pybind11_obj_sym: str) -> List[str]:
         type_full_name = self.cursor.type.spelling
         code = []
```

### Comparing `pybind11_weaver-0.1.2/pybind11_weaver/entity/funktion.py` & `pybind11_weaver-0.1.3/pybind11_weaver/entity/funktion.py`

 * *Files identical despite different names*

### Comparing `pybind11_weaver-0.1.2/pybind11_weaver/entity/klass/field.py` & `pybind11_weaver-0.1.3/pybind11_weaver/entity/klass/field.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
 _logger = logging.getLogger(__name__)
 
 
 def _is_bindable(cursor: cindex.Cursor):
     c_type = common.remove_const_ref_pointer(cursor.type)
     canonical = c_type.get_canonical()
-    if int(canonical.kind) <= int(cindex.TypeKind.CXType_LastBuiltin) and int(canonical.kind) >= int(
-            cindex.TypeKind.CXType_FirstBuiltin):
+    if int(cindex.TypeKind.CXType_LastBuiltin) >= int(canonical.kind) >= int(cindex.TypeKind.CXType_FirstBuiltin) \
+            and not cursor.is_bitfield():
         return True
     if canonical.kind == cindex.TypeKind.CXType_Enum:
         return True
     if canonical.spelling in ["std::string", "std::basic_string<char>"]:
         return True
     return False
```

### Comparing `pybind11_weaver-0.1.2/pybind11_weaver/entity/klass/klass.py` & `pybind11_weaver-0.1.3/pybind11_weaver/entity/klass/klass.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,25 +19,25 @@
         entity_base.Entity.__init__(self, gu, cursor)
         assert cursor.kind in [cindex.CursorKind.CXCursor_ClassDecl, cindex.CursorKind.CXCursor_StructDecl]
         self.extra_methods_codes = []
         self._top_level_extra = []
         self._dependency = set()
 
     @property
-    def name(self):
+    def key_in_scope(self):
         return common.type_python_name(self.cursor.displayname)
 
     def reference_name(self) -> str:
         return common.safe_type_reference(self.cursor.type)
 
     def get_pb11weaver_struct_name(self) -> str:
         return common.type_python_name(scope_list.get_full_qualified_name(self.cursor))
 
     def init_default_pybind11_value(self, parent_scope_sym: str) -> str:
-        code = f'{parent_scope_sym},"{self.name}", pybind11::dynamic_attr()'
+        code = f'{parent_scope_sym},"{self.key_in_scope}", pybind11::dynamic_attr()'
         if self.gu.io_config.gen_docstring:
             code = entity_base._inject_docstring(code, self.cursor, "append")
         return code
 
     def update_stmts(self, pybind11_obj_sym: str) -> List[str]:
 
         # generate method binding first, because it will inject template argument using decl
```

### Comparing `pybind11_weaver-0.1.2/pybind11_weaver/entity/klass/method.py` & `pybind11_weaver-0.1.3/pybind11_weaver/entity/klass/method.py`

 * *Files identical despite different names*

### Comparing `pybind11_weaver-0.1.2/pybind11_weaver/entity/klass/trampoline.py` & `pybind11_weaver-0.1.3/pybind11_weaver/entity/klass/trampoline.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,23 +114,23 @@
             override_type=override_type,
             concreate_ref=concreate_ref,
             args=", ".join(args)
         )
 
     def get_virt_def(self, virt: Virtuals, nest_level: int) -> str:
         ret = ""
-        python_name = self.entity.name
+        python_name = self.entity.key_in_scope
         concreate_ref = self.entity.reference_name()
 
         def get_nest_str(nest_level: int) -> str:
             return "" if nest_level == 0 else str(nest_level)
 
         if virt.base is not None and not virt.base.is_empty():
             ret = self.get_virt_def(virt.base, nest_level + 1)
-            base_ref_name = f"PyTramp{self.entity.name}{get_nest_str(nest_level + 1)}<>"
+            base_ref_name = f"PyTramp{self.entity.key_in_scope}{get_nest_str(nest_level + 1)}<>"
         else:
             base_ref_name = self.entity.reference_name()
         methods = []
         for cursor in virt.virtuals:
             methods.append(self._get_method(cursor, "PYBIND11_OVERRIDE", concreate_ref))
         for cursor in virt.pure_virtuals:
             methods.append(self._get_method(cursor, "PYBIND11_OVERRIDE_PURE", concreate_ref))
@@ -143,15 +143,15 @@
         )
         return ret
 
     def get_defs(self) -> str:
         return self.get_virt_def(self._virt, 0)
 
     def get_trampoline_cls_name(self):
-        return f"PyTramp{self.entity.name}<>"
+        return f"PyTramp{self.entity.key_in_scope}<>"
 
     @staticmethod
     def detect_all_virtual_methods(cursor: cindex.Cursor, to_update: Virtuals):
         cursor, decls, subs = common.get_def_cls_cursor(cursor)
         if decls is None:
             return
         to_update.template_decls = decls
```

### Comparing `pybind11_weaver-0.1.2/pybind11_weaver/entity/namespace.py` & `pybind11_weaver-0.1.3/pybind11_weaver/entity/namespace.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         return self.reference_name().replace("::", "_")
 
     def reference_name(self) -> str:
         return scope_list.get_full_qualified_name(self.cursor, seperator="::")
 
     def init_default_pybind11_value(self, parent_scope_sym: str) -> str:
         module = f"static_cast<pybind11::module_&>({parent_scope_sym})"
-        code = f'{module}.def_submodule("{self.name}")'
+        code = f'{module}.def_submodule("{self.key_in_scope}")'
         return code
 
     def update_stmts(self, pybind11_obj_sym: str) -> List[str]:
         return []
 
     def default_pybind11_type_str(self) -> str:
         return f"pybind11::module_"
```

### Comparing `pybind11_weaver-0.1.2/pybind11_weaver/gen_code.py` & `pybind11_weaver-0.1.3/pybind11_weaver/gen_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 #ifndef PB11_WEAVER_DISABLE_{entity_struct_name}
 
 using {entity_struct_name} = {bind_struct_name}<>;
 
 #else
 
 struct {entity_struct_name} : public pybind11_weaver::DisabledEntity {{
-  explicit {entity_struct_name}(EntityScope parent_h){{}}
+  explicit {entity_struct_name}(EntityScope){{}}
   static const char * Key(){{ 
     return {unique_struct_key};
   }}
 }};
 
 #endif // PB11_WEAVER_DISABLE_{entity_struct_name}
 """
@@ -135,15 +135,15 @@
             create_entity_var_stmts.append(
                 f"auto {entity_obj_sym} = pybind11_weaver::CreateEntity<{entity_struct_name}>({parent_sym}, registry);")
 
             # generate updates
             update_entity_var_stmts.append(f"{entity_obj_sym}->Update();")
 
             # recursive call to children
-            ret = gen_binding_codes(entities[entity.name].children, entity_obj_sym + "->AsScope()", next_id + 1,
+            ret = gen_binding_codes(entities[entity.key_in_scope].children, entity_obj_sym + "->AsScope()", next_id + 1,
                                     generated_entities)
             entity_struct_decls += ret[0]
             create_entity_var_stmts += ret[1]
             update_entity_var_stmts += ret[2]
             exported_type += ret[3]
             next_id = ret[4]
 
@@ -151,15 +151,15 @@
 
 
 def gen_code(config_file: str):
     gus = gen_unit.load_all_gu(config_file)
     for gu in gus:
         # load entities
         entity_root = entity_tree.EntityTree(gu)
-        target_entities = entity_root.entities
+        target_entities = entity_root.children
         if gu.io_config.root_module_namespace != "":
             ns_s = gu.io_config.root_module_namespace.split("::")
             for ns in ns_s:
                 target_entities = target_entities[ns].children
         generated_entities = dict()
         entity_struct_decls, create_entity_var_stmts, update_entity_var_stmts, exported_type, _ = gen_binding_codes(
             entities=target_entities,
```

### Comparing `pybind11_weaver-0.1.2/pybind11_weaver/gen_unit.py` & `pybind11_weaver-0.1.3/pybind11_weaver/gen_unit.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from pybind11_weaver import config
 from pybind11_weaver.utils import common
 
 
 class GenUnit:
     io_config: config.IOConfig
     tu: cindex.TranslationUnit
-    unsaved_file = Tuple[str, str]
+    unsaved_file: Tuple[str, str]
 
     def __init__(self, io_config: config.IOConfig):
         self.io_config = io_config
         self._load_tu()
         self.creation_time: str = datetime.datetime.now().strftime("%m/%d/%Y, %H:%M:%S")
 
     def _load_tu(self, extra_content: str = ""):
```

### Comparing `pybind11_weaver-0.1.2/pybind11_weaver/include/pybind11_weaver/pybind11_weaver.h` & `pybind11_weaver-0.1.3/pybind11_weaver/include/pybind11_weaver/pybind11_weaver.h`

 * *Files identical despite different names*

### Comparing `pybind11_weaver-0.1.2/pybind11_weaver/main.py` & `pybind11_weaver-0.1.3/pybind11_weaver/main.py`

 * *Files identical despite different names*

### Comparing `pybind11_weaver-0.1.2/pybind11_weaver/third_party/ccsyspath.py` & `pybind11_weaver-0.1.3/pybind11_weaver/third_party/ccsyspath.py`

 * *Files identical despite different names*

### Comparing `pybind11_weaver-0.1.2/pybind11_weaver/utils/common.py` & `pybind11_weaver-0.1.3/pybind11_weaver/utils/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,17 @@
                 tokens.append(new_token)
             continue
     ret = "".join(tokens).replace(" ", "")
     return ret
 
 
 def safe_type_reference(type: cindex.Type, subs: Dict[str, str] = None) -> str:
+    """A safe_type_reference is a name that you can reference the type in C++ code at anywhere,
+    usually it is just the fully qualified name of the type.
+    """
     ret = type.get_canonical().spelling
     if "type-parameter" in ret:
         if subs is None:
             return type.spelling  # type is a template parameter
         else:
             return _sub_type_str(type.spelling, subs)
     return ret
```

### Comparing `pybind11_weaver-0.1.2/pybind11_weaver/utils/fn.py` & `pybind11_weaver-0.1.3/pybind11_weaver/utils/fn.py`

 * *Files identical despite different names*

### Comparing `pybind11_weaver-0.1.2/pybind11_weaver.egg-info/PKG-INFO` & `pybind11_weaver-0.1.3/pybind11_weaver.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pybind11-weaver
-Version: 0.1.2
+Name: pybind11_weaver
+Version: 0.1.3
 Summary: A fully customizable pybind11 generator to help generate code for exsiting c/c++ library.
 License: MIT
 Project-URL: Homepage, https://github.com/edimetia3d/pybind11_weaver
 Project-URL: Documentation, https://github.com/edimetia3d/pybind11_weaver
 Project-URL: Repository, https://github.com/edimetia3d/pybind11_weaver
 Project-URL: Changelog, https://github.com/edimetia3d/pybind11_weaver/releases
 Keywords: pybind11,generator,codegen,gen
@@ -25,22 +25,23 @@
 
 # Pybind11 Weaver: Python Binding Code Generator
 
 **Pybind11 Weaver** is a powerful code generator designed to automate the generation of pybind11 code from C++ header
 files. It streamlines the process of creating Python bindings, enabling users to focus on writing critical pybind11 code
 and offloading the tedious work to Pybind11 Weaver.
 
-This tool takes a [sample.h](https://github.com/edimetia3d/pybind11_weaver/blob/main/sample/all_feature/sample.h) file
+This tool takes a [c_lib.h](https://github.com/edimetia3d/pybind11_weaver/blob/main/sample/all_feature/c_lib/c_lib.h)
+file
 and transforms it into
-a [sample_binding.cc.inc](https://github.com/edimetia3d/pybind11_weaver/blob/main/sample/all_feature/sample_binding.cc.inc)
+a [_binding.cc.inc](https://github.com/edimetia3d/pybind11_weaver/blob/main/sample/all_feature/_binding.cc.inc)
 file using [cfg.yaml](https://github.com/edimetia3d/pybind11_weaver/blob/main/sample/all_feature/cfg.yaml) as a guide.
 Following the binding with a single line `auto update_guard = DeclFn(m);`
 in [binding.cc](https://github.com/edimetia3d/pybind11_weaver/blob/main/sample/all_feature/binding.cc), all elements
 from the header file become accessible in Python as demonstrated in
-this [example](https://github.com/edimetia3d/pybind11_weaver/blob/main/test/sample_test/launch_module.py).
+this [example](https://github.com/edimetia3d/pybind11_weaver/blob/main/test/sample/all_feature/test_all_feature.py).
 
 A more pragmatic example is available in [pylibclang](https://github.com/edimetia3d/pylibclang), a comprehensive Python
 wrapper for libclang that uses Pybind11 Weaver to generate the binding code.
 
 1. Its practicality stems from the fact that **Pybind11 Weaver operates on it** as well. Indeed, Pybind11 Weaver is
    self-hosted and generates the binding code for its own use.
 2. Approximately 30k lines of C++ code are generated from a mere 10 lines
@@ -48,14 +49,18 @@
 3. Some [binding code](https://github.com/edimetia3d/pylibclang/blob/master/c_src/binding.cc) is manually crafted to
    handle special cases and integrates seamlessly with the generated code.
 
 [pylibtooling](https://github.com/edimetia3d/pylibtooling) is a much more advanced example that uses Pybind11 Weaver to
 generate the binding code for [libtooling](https://clang.llvm.org/docs/LibTooling.html), and will be used to demonstrate
 the capabilities of Pybind11 Weaver when working with large C++ only libraries.
 
+## Docs
+
+Check https://github.com/edimetia3d/pybind11_weaver/wiki
+
 ## Key Features
 
 1. **Highly Customizable:** While the default configuration is super simple and suitable for most cases, it allows for
    high customization.
 2. **Ease of Use:** As a pure Python package, a simple `pip install` gets it ready to work.
 3. **Versatility:** All generated code is under your control, you can easily modify/enhance/disable any part of
    generated
@@ -118,38 +123,14 @@
 6. Compile all code into a pybind11 module.
 7. Optionally, use [pybind11-stubgen](https://github.com/sizmailov/pybind11-stubgen) to generate `.pyi` stub files,
    enhancing readability for both humans and MYPY in a static way.
 8. Test the module in Python, find bugs, and go to step 5 to fix them.
 
 Also, if you encountered too many problems, you are welcome to open an issue at github, or create a PR to fix it.
 
-## Installation
-
-### Via PYPI
-
-```bash
-python3 -m pip install pybind11-weaver
-```
-
-### From Source
-
-* To install from source:
-
-```bash
-git clone https://github.com/edimetia3d/pybind11_weaver
-python3 -m pip install $(pwd)/pybind11_weaver/
-```
-
-* To run from source (Editable/Develop Mode):
-
-```bash
-git clone https://github.com/edimetia3d/pybind11_weaver
-python3 -m pip install -e $(pwd)/pybind11_weaver/ -v --config-settings editable_mode=compat
-```
-
 ## How it works
 
 The Pybind11 Weaver operates under the hood by utilizing [libclang](https://clang.llvm.org/), a library that parses C++
 header files. This enables us to obtain all APIs from the header file, which are then used to generate the binding code
 on your behalf.
 
 Notably, only header files are required, as we need declarations, not definitions. However, to ensure accurate parsing
```

### Comparing `pybind11_weaver-0.1.2/pybind11_weaver.egg-info/SOURCES.txt` & `pybind11_weaver-0.1.3/pybind11_weaver.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 .gitignore
 CMakeLists.txt
 LICENSE
 MANIFEST.in
 README.md
 build.sh
 pyproject.toml
+requirements.txt
 setup.cfg
 pybind11_weaver/__init__.py
 pybind11_weaver/config.py
 pybind11_weaver/entity_tree.py
 pybind11_weaver/gen_code.py
 pybind11_weaver/gen_unit.py
 pybind11_weaver/main.py
@@ -31,20 +32,24 @@
 pybind11_weaver/entity/klass/method.py
 pybind11_weaver/entity/klass/trampoline.py
 pybind11_weaver/include/pybind11_weaver/pybind11_weaver.h
 pybind11_weaver/third_party/ccsyspath.py
 pybind11_weaver/utils/common.py
 pybind11_weaver/utils/fn.py
 pybind11_weaver/utils/scope_list.py
+sample/CMakeLists.txt
+sample/all_feature/CMakeLists.txt
+sample/all_feature/_binding.cc.inc
 sample/all_feature/binding.cc
 sample/all_feature/cfg.yaml
-sample/all_feature/generate.sh
-sample/all_feature/sample.cc
-sample/all_feature/sample.h
-sample/all_feature/sample_binding.cc.inc
 sample/all_feature/template_pb11_weaver_helper.h
-sample/all_feature/un_export.h
-sample/config/all_with_doc.yaml
+sample/all_feature/c_lib/CMakeLists.txt
+sample/all_feature/c_lib/c_lib.cc
+sample/all_feature/c_lib/c_lib.h
+sample/all_feature/c_lib/not_exported.h
 test/CMakeLists.txt
 test/gen_unit_test.py
-test/sample_test/CMakeLists.txt
-test/sample_test/launch_module.py
+test/config/config_with_doc.yaml
+test/config/test_config.py
+test/sample/CMakeLists.txt
+test/sample/all_feature/CMakeLists.txt
+test/sample/all_feature/test_all_feature.py
```

### Comparing `pybind11_weaver-0.1.2/pyproject.toml` & `pybind11_weaver-0.1.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -18,30 +18,25 @@
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: C++",
     "Topic :: Software Development :: Code Generators",
     "Topic :: Software Development :: Compilers"
 ]
-dependencies = [
-    "pylibclang",
-    "PyYAML",
-    "pybind11",
-    "attrs",
-]
-dynamic = ["version"]
+dynamic = ["version", "dependencies"]
 
 [project.urls]
 Homepage = "https://github.com/edimetia3d/pybind11_weaver"
 Documentation = "https://github.com/edimetia3d/pybind11_weaver"
 Repository = "https://github.com/edimetia3d/pybind11_weaver"
 Changelog = "https://github.com/edimetia3d/pybind11_weaver/releases"
 
 [tool.setuptools.dynamic]
 version = { attr = "pybind11_weaver.__VERSION__" }
+dependencies = { file = ["requirements.txt"] }
 
 [tool.setuptools]
 zip-safe = false
 include-package-data = true
 
 [tool.setuptools.packages.find]
 include = ["pybind11_weaver*"]
```

### Comparing `pybind11_weaver-0.1.2/sample/all_feature/binding.cc` & `pybind11_weaver-0.1.3/sample/all_feature/binding.cc`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 #include <pybind11/pybind11.h>
 
-#include "sample_binding.cc.inc"
+#include "_binding.cc.inc"
 
 // When you want to customize the binding of `XXXX`, you have 2 options:
 // a. Inherit the template class `Bind_XXXX<>` and implement
 //   all the virtual functions. By doing so, you have full control of the
 //   binding.
 // b. Inherit the class `Entity_XXXX` and override some virtual functions.
 //  By doing so, you can not change the type and the construction of the
@@ -40,14 +40,14 @@
   }
   const char *AddMethod_Method1() override {
     // just used to disable the original binding
     return nullptr;
   }
 };
 } // namespace
-PYBIND11_MODULE(all_feature_module, m) {
+PYBIND11_MODULE(all_feature, m) {
   pybind11_weaver::CustomBindingRegistry reg;
   reg.DisableBinding<Entity_disabled_space>();
   reg.DisableBinding<Entity_disabled_member_disabled_Foo>();
   reg.SetCustomBinding<CustomSweetHome>();
   auto update_guard = DeclFn(m, reg);
 }
```

### Comparing `pybind11_weaver-0.1.2/sample/all_feature/sample.cc` & `pybind11_weaver-0.1.3/sample/all_feature/c_lib/c_lib.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 //
 // License: MIT
 //
-#include "sample.h"
+#include "c_lib.h"
 
 void TopFunction(int) {}
 void TopFunction(std::string &) {}
 void HiddenTopFunction(int) {}
 UnexportedType *GetNotBoundType() { return nullptr; }
 double earth::creatures::Home::Method(std::string &, int) { return 0; }
 int earth::creatures::SweetHome::Method(int i) { return i; }
```

### Comparing `pybind11_weaver-0.1.2/sample/all_feature/sample.h` & `pybind11_weaver-0.1.3/sample/all_feature/c_lib/c_lib.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #ifndef PYBIND11_WEAVER_SAMPLE_H
 #define PYBIND11_WEAVER_SAMPLE_H
 
 #include <functional>
 #include <string>
 
-#include "un_export.h"
+#include "not_exported.h"
 /**
  * This is Function doc
  * @param i This is i doc
  */
 void TopFunction(int);
 void TopFunction(std::string &);
 inline void TopFunctionDef() {}
```

### Comparing `pybind11_weaver-0.1.2/sample/all_feature/sample_binding.cc.inc` & `pybind11_weaver-0.1.3/sample/all_feature/_binding.cc.inc`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
-// GENERATED AT 10/30/2023, 16:21:10
+// GENERATED AT 05/30/2024, 14:31:05
 
-#include "sample.h"
+#include "c_lib/c_lib.h"
 #include "template_pb11_weaver_helper.h"
 
 #ifndef GITHUB_COM_PYBIND11_WEAVER
 #define GITHUB_COM_PYBIND11_WEAVER
 #include <atomic>
 #include <functional>
 #include <map>
@@ -289,15 +289,15 @@
 #ifndef PB11_WEAVER_DISABLE_Entity_Foo_Q_R6int9_8
 
 using Entity_Foo_Q_R6int9_8 = Bind_Foo_Q_R6int9_8<>;
 
 #else
 
 struct Entity_Foo_Q_R6int9_8 : public pybind11_weaver::DisabledEntity {
-  explicit Entity_Foo_Q_R6int9_8(EntityScope parent_h) {}
+  explicit Entity_Foo_Q_R6int9_8(EntityScope) {}
   static const char *Key() { return "Foo_Q_R6int9_8"; }
 };
 
 #endif // PB11_WEAVER_DISABLE_Entity_Foo_Q_R6int9_8
 
 template <class Pybind11T = pybind11::module_ &>
 struct Bind_Foo_float_9 : public EntityBase {
@@ -336,15 +336,15 @@
 #ifndef PB11_WEAVER_DISABLE_Entity_Foo_float_9
 
 using Entity_Foo_float_9 = Bind_Foo_float_9<>;
 
 #else
 
 struct Entity_Foo_float_9 : public pybind11_weaver::DisabledEntity {
-  explicit Entity_Foo_float_9(EntityScope parent_h) {}
+  explicit Entity_Foo_float_9(EntityScope) {}
   static const char *Key() { return "Foo_float_9"; }
 };
 
 #endif // PB11_WEAVER_DISABLE_Entity_Foo_float_9
 
 template <class Pybind11T = pybind11::module_ &>
 struct Bind_GetNotBoundType : public EntityBase {
@@ -380,15 +380,15 @@
 #ifndef PB11_WEAVER_DISABLE_Entity_GetNotBoundType
 
 using Entity_GetNotBoundType = Bind_GetNotBoundType<>;
 
 #else
 
 struct Entity_GetNotBoundType : public pybind11_weaver::DisabledEntity {
-  explicit Entity_GetNotBoundType(EntityScope parent_h) {}
+  explicit Entity_GetNotBoundType(EntityScope) {}
   static const char *Key() { return "GetNotBoundType"; }
 };
 
 #endif // PB11_WEAVER_DISABLE_Entity_GetNotBoundType
 
 template <class Pybind11T = pybind11::module_>
 struct Bind_Q : public EntityBase {
@@ -412,15 +412,15 @@
 #ifndef PB11_WEAVER_DISABLE_Entity_Q
 
 using Entity_Q = Bind_Q<>;
 
 #else
 
 struct Entity_Q : public pybind11_weaver::DisabledEntity {
-  explicit Entity_Q(EntityScope parent_h) {}
+  explicit Entity_Q(EntityScope) {}
   static const char *Key() { return "Q"; }
 };
 
 #endif // PB11_WEAVER_DISABLE_Entity_Q
 
 template <class Pybind11T = pybind11::class_<Q::R<int>>>
 struct Bind_Q_R6int9 : public EntityBase {
@@ -447,15 +447,15 @@
 #ifndef PB11_WEAVER_DISABLE_Entity_Q_R6int9
 
 using Entity_Q_R6int9 = Bind_Q_R6int9<>;
 
 #else
 
 struct Entity_Q_R6int9 : public pybind11_weaver::DisabledEntity {
-  explicit Entity_Q_R6int9(EntityScope parent_h) {}
+  explicit Entity_Q_R6int9(EntityScope) {}
   static const char *Key() { return "Q_R6int9"; }
 };
 
 #endif // PB11_WEAVER_DISABLE_Entity_Q_R6int9
 
 template <class Pybind11T =
               pybind11::class_<template_ns::TemplateClass<double>>>
@@ -500,15 +500,15 @@
 using Entity_template_ns_TemplateClass6double9 =
     Bind_template_ns_TemplateClass6double9<>;
 
 #else
 
 struct Entity_template_ns_TemplateClass6double9
     : public pybind11_weaver::DisabledEntity {
-  explicit Entity_template_ns_TemplateClass6double9(EntityScope parent_h) {}
+  explicit Entity_template_ns_TemplateClass6double9(EntityScope) {}
   static const char *Key() { return "template_ns_TemplateClass6double9"; }
 };
 
 #endif // PB11_WEAVER_DISABLE_Entity_template_ns_TemplateClass6double9
 
 template <class Pybind11T = pybind11::module_ &>
 struct Bind_TopFunction : public EntityBase {
@@ -547,15 +547,15 @@
 #ifndef PB11_WEAVER_DISABLE_Entity_TopFunction
 
 using Entity_TopFunction = Bind_TopFunction<>;
 
 #else
 
 struct Entity_TopFunction : public pybind11_weaver::DisabledEntity {
-  explicit Entity_TopFunction(EntityScope parent_h) {}
+  explicit Entity_TopFunction(EntityScope) {}
   static const char *Key() { return "TopFunction"; }
 };
 
 #endif // PB11_WEAVER_DISABLE_Entity_TopFunction
 
 template <class Pybind11T = pybind11::module_ &>
 struct Bind_TopFunction1 : public EntityBase {
@@ -590,15 +590,15 @@
 #ifndef PB11_WEAVER_DISABLE_Entity_TopFunction1
 
 using Entity_TopFunction1 = Bind_TopFunction1<>;
 
 #else
 
 struct Entity_TopFunction1 : public pybind11_weaver::DisabledEntity {
-  explicit Entity_TopFunction1(EntityScope parent_h) {}
+  explicit Entity_TopFunction1(EntityScope) {}
   static const char *Key() { return "TopFunction1"; }
 };
 
 #endif // PB11_WEAVER_DISABLE_Entity_TopFunction1
 
 template <class Pybind11T = pybind11::module_ &>
 struct Bind_TopFunctionDef : public EntityBase {
@@ -633,15 +633,15 @@
 #ifndef PB11_WEAVER_DISABLE_Entity_TopFunctionDef
 
 using Entity_TopFunctionDef = Bind_TopFunctionDef<>;
 
 #else
 
 struct Entity_TopFunctionDef : public pybind11_weaver::DisabledEntity {
-  explicit Entity_TopFunctionDef(EntityScope parent_h) {}
+  explicit Entity_TopFunctionDef(EntityScope) {}
   static const char *Key() { return "TopFunctionDef"; }
 };
 
 #endif // PB11_WEAVER_DISABLE_Entity_TopFunctionDef
 
 template <class = void>
 class PyTrampVirtualBase6int9 : public VirtualBase<int> {
@@ -759,15 +759,15 @@
 #ifndef PB11_WEAVER_DISABLE_Entity_VirtualBase6int9
 
 using Entity_VirtualBase6int9 = Bind_VirtualBase6int9<>;
 
 #else
 
 struct Entity_VirtualBase6int9 : public pybind11_weaver::DisabledEntity {
-  explicit Entity_VirtualBase6int9(EntityScope parent_h) {}
+  explicit Entity_VirtualBase6int9(EntityScope) {}
   static const char *Key() { return "VirtualBase6int9"; }
 };
 
 #endif // PB11_WEAVER_DISABLE_Entity_VirtualBase6int9
 
 template <class Pybind11T = pybind11::module_>
 struct Bind_disabled_member : public EntityBase {
@@ -792,15 +792,15 @@
 #ifndef PB11_WEAVER_DISABLE_Entity_disabled_member
 
 using Entity_disabled_member = Bind_disabled_member<>;
 
 #else
 
 struct Entity_disabled_member : public pybind11_weaver::DisabledEntity {
-  explicit Entity_disabled_member(EntityScope parent_h) {}
+  explicit Entity_disabled_member(EntityScope) {}
   static const char *Key() { return "disabled_member"; }
 };
 
 #endif // PB11_WEAVER_DISABLE_Entity_disabled_member
 
 template <class Pybind11T = pybind11::enum_<disabled_member::disabled_Foo>>
 struct Bind_disabled_member_disabled_Foo : public EntityBase {
@@ -829,15 +829,15 @@
 
 using Entity_disabled_member_disabled_Foo = Bind_disabled_member_disabled_Foo<>;
 
 #else
 
 struct Entity_disabled_member_disabled_Foo
     : public pybind11_weaver::DisabledEntity {
-  explicit Entity_disabled_member_disabled_Foo(EntityScope parent_h) {}
+  explicit Entity_disabled_member_disabled_Foo(EntityScope) {}
   static const char *Key() { return "disabled_member_disabled_Foo"; }
 };
 
 #endif // PB11_WEAVER_DISABLE_Entity_disabled_member_disabled_Foo
 
 template <class Pybind11T = pybind11::module_>
 struct Bind_disabled_space : public EntityBase {
@@ -862,15 +862,15 @@
 #ifndef PB11_WEAVER_DISABLE_Entity_disabled_space
 
 using Entity_disabled_space = Bind_disabled_space<>;
 
 #else
 
 struct Entity_disabled_space : public pybind11_weaver::DisabledEntity {
-  explicit Entity_disabled_space(EntityScope parent_h) {}
+  explicit Entity_disabled_space(EntityScope) {}
   static const char *Key() { return "disabled_space"; }
 };
 
 #endif // PB11_WEAVER_DISABLE_Entity_disabled_space
 
 template <class Pybind11T = pybind11::enum_<disabled_space::Foo>>
 struct Bind_disabled_space_Foo : public EntityBase {
@@ -897,15 +897,15 @@
 #ifndef PB11_WEAVER_DISABLE_Entity_disabled_space_Foo
 
 using Entity_disabled_space_Foo = Bind_disabled_space_Foo<>;
 
 #else
 
 struct Entity_disabled_space_Foo : public pybind11_weaver::DisabledEntity {
-  explicit Entity_disabled_space_Foo(EntityScope parent_h) {}
+  explicit Entity_disabled_space_Foo(EntityScope) {}
   static const char *Key() { return "disabled_space_Foo"; }
 };
 
 #endif // PB11_WEAVER_DISABLE_Entity_disabled_space_Foo
 
 template <class Pybind11T = pybind11::module_>
 struct Bind_earth : public EntityBase {
@@ -930,15 +930,15 @@
 #ifndef PB11_WEAVER_DISABLE_Entity_earth
 
 using Entity_earth = Bind_earth<>;
 
 #else
 
 struct Entity_earth : public pybind11_weaver::DisabledEntity {
-  explicit Entity_earth(EntityScope parent_h) {}
+  explicit Entity_earth(EntityScope) {}
   static const char *Key() { return "earth"; }
 };
 
 #endif // PB11_WEAVER_DISABLE_Entity_earth
 
 template <class Pybind11T = pybind11::module_>
 struct Bind_earth_creatures : public EntityBase {
@@ -963,15 +963,15 @@
 #ifndef PB11_WEAVER_DISABLE_Entity_earth_creatures
 
 using Entity_earth_creatures = Bind_earth_creatures<>;
 
 #else
 
 struct Entity_earth_creatures : public pybind11_weaver::DisabledEntity {
-  explicit Entity_earth_creatures(EntityScope parent_h) {}
+  explicit Entity_earth_creatures(EntityScope) {}
   static const char *Key() { return "earth_creatures"; }
 };
 
 #endif // PB11_WEAVER_DISABLE_Entity_earth_creatures
 
 template <class Pybind11T = pybind11::enum_<earth::creatures::Animal>>
 struct Bind_earth_creatures_Animal : public EntityBase {
@@ -1002,15 +1002,15 @@
 #ifndef PB11_WEAVER_DISABLE_Entity_earth_creatures_Animal
 
 using Entity_earth_creatures_Animal = Bind_earth_creatures_Animal<>;
 
 #else
 
 struct Entity_earth_creatures_Animal : public pybind11_weaver::DisabledEntity {
-  explicit Entity_earth_creatures_Animal(EntityScope parent_h) {}
+  explicit Entity_earth_creatures_Animal(EntityScope) {}
   static const char *Key() { return "earth_creatures_Animal"; }
 };
 
 #endif // PB11_WEAVER_DISABLE_Entity_earth_creatures_Animal
 
 template <class Pybind11T = pybind11::class_<earth::creatures::Home>>
 struct Bind_earth_creatures_Home : public EntityBase {
@@ -1053,15 +1053,15 @@
 #ifndef PB11_WEAVER_DISABLE_Entity_earth_creatures_Home
 
 using Entity_earth_creatures_Home = Bind_earth_creatures_Home<>;
 
 #else
 
 struct Entity_earth_creatures_Home : public pybind11_weaver::DisabledEntity {
-  explicit Entity_earth_creatures_Home(EntityScope parent_h) {}
+  explicit Entity_earth_creatures_Home(EntityScope) {}
   static const char *Key() { return "earth_creatures_Home"; }
 };
 
 #endif // PB11_WEAVER_DISABLE_Entity_earth_creatures_Home
 
 template <class Pybind11T = pybind11::enum_<earth::creatures::Home::Food>>
 struct Bind_earth_creatures_Home_Food : public EntityBase {
@@ -1090,15 +1090,15 @@
 
 using Entity_earth_creatures_Home_Food = Bind_earth_creatures_Home_Food<>;
 
 #else
 
 struct Entity_earth_creatures_Home_Food
     : public pybind11_weaver::DisabledEntity {
-  explicit Entity_earth_creatures_Home_Food(EntityScope parent_h) {}
+  explicit Entity_earth_creatures_Home_Food(EntityScope) {}
   static const char *Key() { return "earth_creatures_Home_Food"; }
 };
 
 #endif // PB11_WEAVER_DISABLE_Entity_earth_creatures_Home_Food
 
 template <class Pybind11T = pybind11::module_ &>
 struct Bind_NSFunction : public EntityBase {
@@ -1134,15 +1134,15 @@
 #ifndef PB11_WEAVER_DISABLE_Entity_NSFunction
 
 using Entity_NSFunction = Bind_NSFunction<>;
 
 #else
 
 struct Entity_NSFunction : public pybind11_weaver::DisabledEntity {
-  explicit Entity_NSFunction(EntityScope parent_h) {}
+  explicit Entity_NSFunction(EntityScope) {}
   static const char *Key() { return "NSFunction"; }
 };
 
 #endif // PB11_WEAVER_DISABLE_Entity_NSFunction
 
 template <class Pybind11T = pybind11::module_ &>
 struct Bind_NSFunctionDef : public EntityBase {
@@ -1177,15 +1177,15 @@
 #ifndef PB11_WEAVER_DISABLE_Entity_NSFunctionDef
 
 using Entity_NSFunctionDef = Bind_NSFunctionDef<>;
 
 #else
 
 struct Entity_NSFunctionDef : public pybind11_weaver::DisabledEntity {
-  explicit Entity_NSFunctionDef(EntityScope parent_h) {}
+  explicit Entity_NSFunctionDef(EntityScope) {}
   static const char *Key() { return "NSFunctionDef"; }
 };
 
 #endif // PB11_WEAVER_DISABLE_Entity_NSFunctionDef
 
 template <class = void>
 class PyTrampSweetHome : public earth::creatures::SweetHome {
@@ -1423,15 +1423,15 @@
 
 using Entity_earth_creatures_SweetHome = Bind_earth_creatures_SweetHome<>;
 
 #else
 
 struct Entity_earth_creatures_SweetHome
     : public pybind11_weaver::DisabledEntity {
-  explicit Entity_earth_creatures_SweetHome(EntityScope parent_h) {}
+  explicit Entity_earth_creatures_SweetHome(EntityScope) {}
   static const char *Key() { return "earth_creatures_SweetHome"; }
 };
 
 #endif // PB11_WEAVER_DISABLE_Entity_earth_creatures_SweetHome
 
 template <class Pybind11T = pybind11::enum_<earth::creatures::ValueSet>>
 struct Bind_earth_creatures_ValueSet : public EntityBase {
@@ -1461,15 +1461,15 @@
 
 using Entity_earth_creatures_ValueSet = Bind_earth_creatures_ValueSet<>;
 
 #else
 
 struct Entity_earth_creatures_ValueSet
     : public pybind11_weaver::DisabledEntity {
-  explicit Entity_earth_creatures_ValueSet(EntityScope parent_h) {}
+  explicit Entity_earth_creatures_ValueSet(EntityScope) {}
   static const char *Key() { return "earth_creatures_ValueSet"; }
 };
 
 #endif // PB11_WEAVER_DISABLE_Entity_earth_creatures_ValueSet
 
 template <class Pybind11T = pybind11::module_>
 struct Bind_template_ns : public EntityBase {
@@ -1494,15 +1494,15 @@
 #ifndef PB11_WEAVER_DISABLE_Entity_template_ns
 
 using Entity_template_ns = Bind_template_ns<>;
 
 #else
 
 struct Entity_template_ns : public pybind11_weaver::DisabledEntity {
-  explicit Entity_template_ns(EntityScope parent_h) {}
+  explicit Entity_template_ns(EntityScope) {}
   static const char *Key() { return "template_ns"; }
 };
 
 #endif // PB11_WEAVER_DISABLE_Entity_template_ns
 
 template <class Pybind11T = pybind11::class_<
               template_ns::DerivedClass, template_ns::TemplateClass<double>>>
@@ -1546,15 +1546,15 @@
 
 using Entity_template_ns_DerivedClass = Bind_template_ns_DerivedClass<>;
 
 #else
 
 struct Entity_template_ns_DerivedClass
     : public pybind11_weaver::DisabledEntity {
-  explicit Entity_template_ns_DerivedClass(EntityScope parent_h) {}
+  explicit Entity_template_ns_DerivedClass(EntityScope) {}
   static const char *Key() { return "template_ns_DerivedClass"; }
 };
 
 #endif // PB11_WEAVER_DISABLE_Entity_template_ns_DerivedClass
 
 template <class Pybind11T = pybind11::class_<template_ns::TemplateClass<float>>>
 struct Bind_template_ns_TemplateClass6float9 : public EntityBase {
@@ -1601,15 +1601,15 @@
 using Entity_template_ns_TemplateClass6float9 =
     Bind_template_ns_TemplateClass6float9<>;
 
 #else
 
 struct Entity_template_ns_TemplateClass6float9
     : public pybind11_weaver::DisabledEntity {
-  explicit Entity_template_ns_TemplateClass6float9(EntityScope parent_h) {}
+  explicit Entity_template_ns_TemplateClass6float9(EntityScope) {}
   static const char *Key() { return "template_ns_TemplateClass6float9"; }
 };
 
 #endif // PB11_WEAVER_DISABLE_Entity_template_ns_TemplateClass6float9
 
 template <class Pybind11T = pybind11::class_<template_ns::TemplateClass<int>>>
 struct Bind_template_ns_TemplateClass6int9 : public EntityBase {
@@ -1654,15 +1654,15 @@
 using Entity_template_ns_TemplateClass6int9 =
     Bind_template_ns_TemplateClass6int9<>;
 
 #else
 
 struct Entity_template_ns_TemplateClass6int9
     : public pybind11_weaver::DisabledEntity {
-  explicit Entity_template_ns_TemplateClass6int9(EntityScope parent_h) {}
+  explicit Entity_template_ns_TemplateClass6int9(EntityScope) {}
   static const char *Key() { return "template_ns_TemplateClass6int9"; }
 };
 
 #endif // PB11_WEAVER_DISABLE_Entity_template_ns_TemplateClass6int9
 
 template <class = void> class PyTrampDriveVirtual : public DriveVirtual {
 public:
@@ -1764,15 +1764,15 @@
 #ifndef PB11_WEAVER_DISABLE_Entity_DriveVirtual
 
 using Entity_DriveVirtual = Bind_DriveVirtual<>;
 
 #else
 
 struct Entity_DriveVirtual : public pybind11_weaver::DisabledEntity {
-  explicit Entity_DriveVirtual(EntityScope parent_h) {}
+  explicit Entity_DriveVirtual(EntityScope) {}
   static const char *Key() { return "DriveVirtual"; }
 };
 
 #endif // PB11_WEAVER_DISABLE_Entity_DriveVirtual
 
 /**
  * Create all entities, return a callable guard that can be called to update all
```

### Comparing `pybind11_weaver-0.1.2/sample/all_feature/template_pb11_weaver_helper.h` & `pybind11_weaver-0.1.3/sample/all_feature/template_pb11_weaver_helper.h`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 //
 
 /**
  * This file is manually crafted to help binding generation, it is not a part of
  * the public API.
  */
 
-#include "sample.h"
+#include "c_lib/c_lib.h"
 
 /**
  * Two things need to be done to bind a template function:
  * 1. Use syntax of "template specialization" to force generate the binding of
  * template function.
  * 2. Use syntax of extern template to avoid duplicate symbol.
  * Note that some instance must exist in the translation unit.
```

### Comparing `pybind11_weaver-0.1.2/test/sample_test/CMakeLists.txt` & `pybind11_weaver-0.1.3/test/sample/all_feature/CMakeLists.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 # may use`python3 -m pybind11 --cmakedir`
-if (NOT DEFINED pybind11_DIR)
-  return()
-endif ()
 
-find_package(pybind11 REQUIRED CONFIG)
-include_directories(${CMAKE_CURRENT_LIST_DIR}/../../pybind11_weaver/include)
-include_directories(${CMAKE_CURRENT_LIST_DIR}/../..)
-pybind11_add_module(all_feature_module ${PROJECT_SOURCE_DIR}/sample/all_feature/binding.cc)
-add_library(all_feature_lib ${PROJECT_SOURCE_DIR}/sample/all_feature/sample.cc)
-target_link_libraries(all_feature_module PRIVATE all_feature_lib)
+add_test(NAME generate_all_feature_binding
+    COMMAND ${Python3_EXECUTABLE} -m pybind11_weaver.main --config ${PROJECT_SOURCE_DIR}/sample/all_feature/cfg.yaml
+)
 
-add_test(build_extension
+add_test(build_all_feature_extension
     "${CMAKE_COMMAND}"
     --build "${CMAKE_BINARY_DIR}"
     --config "$<CONFIG>"
-    --target all_feature_module
+    --target all_feature
 )
+set_tests_properties(build_all_feature_extension PROPERTIES DEPENDS "generate_all_feature_binding")
 
-add_test(NAME launch_test_module
-    COMMAND ${Python3_EXECUTABLE} ${CMAKE_CURRENT_LIST_DIR}/launch_module.py
-)
-set_tests_properties(launch_test_module PROPERTIES DEPENDS "build_extension;update_sample_test")
 
-set_tests_properties(launch_test_module
-    PROPERTIES ENVIRONMENT "PYTHONPATH=${CMAKE_CURRENT_BINARY_DIR}:$ENV{PYTHONPATH}")
+add_test(NAME test_all_feature
+    COMMAND ${Python3_EXECUTABLE} ${CMAKE_CURRENT_LIST_DIR}/test_all_feature.py
+)
+set_tests_properties(test_all_feature PROPERTIES DEPENDS "build_all_feature_extension")
+set_tests_properties(test_all_feature PROPERTIES ENVIRONMENT "PYTHONPATH=${PROJECT_BINARY_DIR}")
```

### Comparing `pybind11_weaver-0.1.2/test/sample_test/launch_module.py` & `pybind11_weaver-0.1.3/test/sample/all_feature/test_all_feature.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 import random
 
-import all_feature_module as m
-from all_feature_module.earth import creatures
+import sample.all_feature.all_feature as m
+from sample.all_feature.all_feature.earth import creatures
 
 
 class TestAll(unittest.TestCase):
     def test_all_exported(self):
         m.TopFunction(0)
         m.TopFunction("str")
         m.TopFunctionDef()
```

