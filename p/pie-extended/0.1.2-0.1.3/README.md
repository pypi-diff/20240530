# Comparing `tmp/pie_extended-0.1.2.tar.gz` & `tmp/pie_extended-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pie_extended-0.1.2.tar", last modified: Fri Apr 28 10:39:19 2023, max compression
+gzip compressed data, was "pie_extended-0.1.3.tar", last modified: Thu May 30 08:57:39 2024, max compression
```

## Comparing `pie_extended-0.1.2.tar` & `pie_extended-0.1.3.tar`

### file list

```diff
@@ -1,89 +1,94 @@
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-28 10:39:19.927600 pie_extended-0.1.2/
--rw-r--r--   0 thibault  (1000) thibault  (1000)    16725 2019-12-19 07:41:47.000000 pie_extended-0.1.2/LICENSE
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     6606 2023-04-28 10:39:19.927600 pie_extended-0.1.2/PKG-INFO
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     5915 2023-04-27 10:01:39.000000 pie_extended-0.1.2/README.md
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-28 10:39:19.923600 pie_extended-0.1.2/pie_extended/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2019-12-19 07:58:23.000000 pie_extended-0.1.2/pie_extended/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       67 2019-12-19 08:02:18.000000 pie_extended-0.1.2/pie_extended/__main__.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-28 10:39:19.923600 pie_extended-0.1.2/pie_extended/cli/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2020-08-20 16:54:07.000000 pie_extended-0.1.2/pie_extended/cli/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     5212 2023-01-31 13:50:33.000000 pie_extended-0.1.2/pie_extended/cli/main.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     4530 2022-05-10 08:25:45.000000 pie_extended-0.1.2/pie_extended/cli/utils.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-28 10:39:19.923600 pie_extended-0.1.2/pie_extended/models/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       82 2020-12-04 18:21:14.000000 pie_extended-0.1.2/pie_extended/models/__init__.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-28 10:39:19.923600 pie_extended-0.1.2/pie_extended/models/dum/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      616 2020-12-04 18:21:14.000000 pie_extended-0.1.2/pie_extended/models/dum/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      463 2021-01-13 15:28:06.000000 pie_extended-0.1.2/pie_extended/models/dum/imports.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-28 10:39:19.923600 pie_extended-0.1.2/pie_extended/models/fr/
--rwxrwxr-x   0 thibault  (1000) thibault  (1000)     1795 2020-04-23 13:58:50.000000 pie_extended-0.1.2/pie_extended/models/fr/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     5383 2021-04-12 07:59:41.000000 pie_extended-0.1.2/pie_extended/models/fr/excluders.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      761 2021-01-13 15:27:50.000000 pie_extended-0.1.2/pie_extended/models/fr/imports.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1606 2020-04-23 13:58:50.000000 pie_extended-0.1.2/pie_extended/models/fr/processor.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     3637 2021-04-12 07:28:48.000000 pie_extended-0.1.2/pie_extended/models/fr/tokenizer.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-28 10:39:19.923600 pie_extended-0.1.2/pie_extended/models/freem/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      810 2022-12-05 19:37:10.000000 pie_extended-0.1.2/pie_extended/models/freem/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      941 2021-04-12 08:03:09.000000 pie_extended-0.1.2/pie_extended/models/freem/imports.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-28 10:39:19.923600 pie_extended-0.1.2/pie_extended/models/fro/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1995 2023-04-28 10:16:34.000000 pie_extended-0.1.2/pie_extended/models/fro/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1114 2021-05-20 08:42:31.000000 pie_extended-0.1.2/pie_extended/models/fro/imports.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     2157 2023-04-28 10:37:02.000000 pie_extended-0.1.2/pie_extended/models/fro/processor.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     3156 2023-04-28 10:34:37.000000 pie_extended-0.1.2/pie_extended/models/fro/tokenizer.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-28 10:39:19.923600 pie_extended-0.1.2/pie_extended/models/grc/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     2023 2021-02-11 09:35:40.000000 pie_extended-0.1.2/pie_extended/models/grc/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      749 2021-03-22 13:34:04.000000 pie_extended-0.1.2/pie_extended/models/grc/imports.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1641 2021-02-11 09:35:40.000000 pie_extended-0.1.2/pie_extended/models/grc/processor.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     2451 2021-03-22 13:31:46.000000 pie_extended-0.1.2/pie_extended/models/grc/tokenizer.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-28 10:39:19.923600 pie_extended-0.1.2/pie_extended/models/lasla/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     2495 2021-04-03 07:13:21.000000 pie_extended-0.1.2/pie_extended/models/lasla/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1375 2020-12-04 16:36:08.000000 pie_extended-0.1.2/pie_extended/models/lasla/_params.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     2639 2021-01-13 15:25:15.000000 pie_extended-0.1.2/pie_extended/models/lasla/imports.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     5596 2021-02-11 09:35:40.000000 pie_extended-0.1.2/pie_extended/models/lasla/processor.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     4090 2021-02-03 12:42:25.000000 pie_extended-0.1.2/pie_extended/models/lasla/tokenizer.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-28 10:39:19.923600 pie_extended-0.1.2/pie_extended/pipeline/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2019-12-20 08:07:13.000000 pie_extended-0.1.2/pie_extended/pipeline/__init__.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-28 10:39:19.923600 pie_extended-0.1.2/pie_extended/pipeline/disambiguators/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2019-12-19 17:07:25.000000 pie_extended-0.1.2/pie_extended/pipeline/disambiguators/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     2134 2020-09-23 09:14:05.000000 pie_extended-0.1.2/pie_extended/pipeline/disambiguators/autocat.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      283 2019-12-19 17:08:38.000000 pie_extended-0.1.2/pie_extended/pipeline/disambiguators/proto.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-28 10:39:19.927600 pie_extended-0.1.2/pie_extended/pipeline/formatters/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2019-12-19 15:11:48.000000 pie_extended-0.1.2/pie_extended/pipeline/formatters/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1420 2020-06-22 12:18:04.000000 pie_extended-0.1.2/pie_extended/pipeline/formatters/proto.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-28 10:39:19.927600 pie_extended-0.1.2/pie_extended/pipeline/iterators/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        3 2019-12-19 17:13:20.000000 pie_extended-0.1.2/pie_extended/pipeline/iterators/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     5461 2021-01-13 15:24:27.000000 pie_extended-0.1.2/pie_extended/pipeline/iterators/proto.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-28 10:39:19.927600 pie_extended-0.1.2/pie_extended/pipeline/postprocessor/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2020-02-25 14:02:45.000000 pie_extended-0.1.2/pie_extended/pipeline/postprocessor/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     4614 2021-02-11 09:35:40.000000 pie_extended-0.1.2/pie_extended/pipeline/postprocessor/glue.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     3723 2020-04-23 14:53:46.000000 pie_extended-0.1.2/pie_extended/pipeline/postprocessor/memory.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     5455 2021-02-11 09:26:29.000000 pie_extended-0.1.2/pie_extended/pipeline/postprocessor/proto.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1863 2020-04-23 14:53:46.000000 pie_extended-0.1.2/pie_extended/pipeline/postprocessor/rulebased.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     2887 2020-05-05 15:15:28.000000 pie_extended-0.1.2/pie_extended/pipeline/postprocessor/splitter.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-28 10:39:19.927600 pie_extended-0.1.2/pie_extended/pipeline/tokenizers/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2019-12-19 17:06:18.000000 pie_extended-0.1.2/pie_extended/pipeline/tokenizers/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     2000 2020-08-20 16:54:07.000000 pie_extended-0.1.2/pie_extended/pipeline/tokenizers/memorizing.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     2537 2020-12-04 18:21:14.000000 pie_extended-0.1.2/pie_extended/pipeline/tokenizers/simple_tokenizer.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-28 10:39:19.927600 pie_extended-0.1.2/pie_extended/pipeline/tokenizers/utils/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2020-08-20 16:54:07.000000 pie_extended-0.1.2/pie_extended/pipeline/tokenizers/utils/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       86 2020-09-08 15:47:36.000000 pie_extended-0.1.2/pie_extended/pipeline/tokenizers/utils/chars.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)    11438 2021-04-12 07:58:27.000000 pie_extended-0.1.2/pie_extended/pipeline/tokenizers/utils/excluder.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      601 2020-09-08 15:53:07.000000 pie_extended-0.1.2/pie_extended/pipeline/tokenizers/utils/regexps.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     4979 2022-05-10 08:17:38.000000 pie_extended-0.1.2/pie_extended/tagger.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-28 10:39:19.927600 pie_extended-0.1.2/pie_extended/testing_utils/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     3800 2020-08-20 16:54:07.000000 pie_extended-0.1.2/pie_extended/testing_utils/__init__.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-28 10:39:19.927600 pie_extended-0.1.2/pie_extended/utils/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1537 2020-05-05 15:15:28.000000 pie_extended-0.1.2/pie_extended/utils/__init__.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-28 10:39:19.923600 pie_extended-0.1.2/pie_extended.egg-info/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     6606 2023-04-28 10:39:19.000000 pie_extended-0.1.2/pie_extended.egg-info/PKG-INFO
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     2397 2023-04-28 10:39:19.000000 pie_extended-0.1.2/pie_extended.egg-info/SOURCES.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        1 2023-04-28 10:39:19.000000 pie_extended-0.1.2/pie_extended.egg-info/dependency_links.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       64 2023-04-28 10:39:19.000000 pie_extended-0.1.2/pie_extended.egg-info/entry_points.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      130 2023-04-28 10:39:19.000000 pie_extended-0.1.2/pie_extended.egg-info/requires.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       19 2023-04-28 10:39:19.000000 pie_extended-0.1.2/pie_extended.egg-info/top_level.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       38 2023-04-28 10:39:19.927600 pie_extended-0.1.2/setup.cfg
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     3799 2023-04-28 10:37:30.000000 pie_extended-0.1.2/setup.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-28 10:39:19.923600 pie_extended-0.1.2/tests/
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-04-28 10:39:19.927600 pie_extended-0.1.2/tests/test_models/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2019-12-20 08:44:57.000000 pie_extended-0.1.2/tests/test_models/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     4278 2020-04-28 14:13:57.000000 pie_extended-0.1.2/tests/test_models/test_fr.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1424 2020-08-20 16:54:07.000000 pie_extended-0.1.2/tests/test_models/test_fro.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     9770 2020-12-04 16:36:08.000000 pie_extended-0.1.2/tests/test_models/test_lasla.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2024-05-30 08:57:39.555856 pie_extended-0.1.3/
+-rw-r--r--   0 thibault  (1000) thibault  (1000)    16725 2019-12-19 07:41:47.000000 pie_extended-0.1.3/LICENSE
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     6606 2024-05-30 08:57:39.555856 pie_extended-0.1.3/PKG-INFO
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     5915 2023-04-27 10:01:39.000000 pie_extended-0.1.3/README.md
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2024-05-30 08:57:39.551856 pie_extended-0.1.3/pie_extended/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2019-12-19 07:58:23.000000 pie_extended-0.1.3/pie_extended/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)       67 2019-12-19 08:02:18.000000 pie_extended-0.1.3/pie_extended/__main__.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2024-05-30 08:57:39.551856 pie_extended-0.1.3/pie_extended/cli/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2020-08-20 16:54:07.000000 pie_extended-0.1.3/pie_extended/cli/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     5212 2023-01-31 13:50:33.000000 pie_extended-0.1.3/pie_extended/cli/main.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     4530 2024-05-30 06:31:55.000000 pie_extended-0.1.3/pie_extended/cli/utils.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2024-05-30 08:57:39.551856 pie_extended-0.1.3/pie_extended/models/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)       98 2024-05-30 08:54:32.000000 pie_extended-0.1.3/pie_extended/models/__init__.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2024-05-30 08:57:39.551856 pie_extended-0.1.3/pie_extended/models/dum/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      616 2020-12-04 18:21:14.000000 pie_extended-0.1.3/pie_extended/models/dum/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      463 2021-01-13 15:28:06.000000 pie_extended-0.1.3/pie_extended/models/dum/imports.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2024-05-30 08:57:39.551856 pie_extended-0.1.3/pie_extended/models/fr/
+-rwxrwxr-x   0 thibault  (1000) thibault  (1000)     1795 2020-04-23 13:58:50.000000 pie_extended-0.1.3/pie_extended/models/fr/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     5383 2021-04-12 07:59:41.000000 pie_extended-0.1.3/pie_extended/models/fr/excluders.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      761 2021-01-13 15:27:50.000000 pie_extended-0.1.3/pie_extended/models/fr/imports.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1606 2020-04-23 13:58:50.000000 pie_extended-0.1.3/pie_extended/models/fr/processor.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     3637 2021-04-12 07:28:48.000000 pie_extended-0.1.3/pie_extended/models/fr/tokenizer.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2024-05-30 08:57:39.551856 pie_extended-0.1.3/pie_extended/models/freem/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      810 2022-12-05 19:37:10.000000 pie_extended-0.1.3/pie_extended/models/freem/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      941 2021-04-12 08:03:09.000000 pie_extended-0.1.3/pie_extended/models/freem/imports.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2024-05-30 08:57:39.551856 pie_extended-0.1.3/pie_extended/models/fro/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1995 2023-04-28 10:16:34.000000 pie_extended-0.1.3/pie_extended/models/fro/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1114 2021-05-20 08:42:31.000000 pie_extended-0.1.3/pie_extended/models/fro/imports.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     2157 2023-04-28 10:37:02.000000 pie_extended-0.1.3/pie_extended/models/fro/processor.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     3156 2023-04-28 10:34:37.000000 pie_extended-0.1.3/pie_extended/models/fro/tokenizer.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2024-05-30 08:57:39.555856 pie_extended-0.1.3/pie_extended/models/grc/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     2023 2021-02-11 09:35:40.000000 pie_extended-0.1.3/pie_extended/models/grc/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      749 2021-03-22 13:34:04.000000 pie_extended-0.1.3/pie_extended/models/grc/imports.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1641 2021-02-11 09:35:40.000000 pie_extended-0.1.3/pie_extended/models/grc/processor.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     2451 2021-03-22 13:31:46.000000 pie_extended-0.1.3/pie_extended/models/grc/tokenizer.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2024-05-30 08:57:39.555856 pie_extended-0.1.3/pie_extended/models/lasla/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     2495 2021-04-03 07:13:21.000000 pie_extended-0.1.3/pie_extended/models/lasla/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1375 2020-12-04 16:36:08.000000 pie_extended-0.1.3/pie_extended/models/lasla/_params.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     2639 2021-01-13 15:25:15.000000 pie_extended-0.1.3/pie_extended/models/lasla/imports.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     5596 2021-02-11 09:35:40.000000 pie_extended-0.1.3/pie_extended/models/lasla/processor.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     4090 2024-05-30 07:28:14.000000 pie_extended-0.1.3/pie_extended/models/lasla/tokenizer.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2024-05-30 08:57:39.555856 pie_extended-0.1.3/pie_extended/models/occ_cont/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      716 2024-05-30 08:54:32.000000 pie_extended-0.1.3/pie_extended/models/occ_cont/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      800 2024-05-30 08:54:32.000000 pie_extended-0.1.3/pie_extended/models/occ_cont/imports.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2024-05-30 08:54:32.000000 pie_extended-0.1.3/pie_extended/models/occ_cont/processor.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     6103 2024-05-30 08:54:32.000000 pie_extended-0.1.3/pie_extended/models/occ_cont/tokenizer.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2024-05-30 08:57:39.555856 pie_extended-0.1.3/pie_extended/pipeline/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2019-12-20 08:07:13.000000 pie_extended-0.1.3/pie_extended/pipeline/__init__.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2024-05-30 08:57:39.555856 pie_extended-0.1.3/pie_extended/pipeline/disambiguators/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2019-12-19 17:07:25.000000 pie_extended-0.1.3/pie_extended/pipeline/disambiguators/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     2134 2020-09-23 09:14:05.000000 pie_extended-0.1.3/pie_extended/pipeline/disambiguators/autocat.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      283 2019-12-19 17:08:38.000000 pie_extended-0.1.3/pie_extended/pipeline/disambiguators/proto.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2024-05-30 08:57:39.555856 pie_extended-0.1.3/pie_extended/pipeline/formatters/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2019-12-19 15:11:48.000000 pie_extended-0.1.3/pie_extended/pipeline/formatters/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1420 2020-06-22 12:18:04.000000 pie_extended-0.1.3/pie_extended/pipeline/formatters/proto.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2024-05-30 08:57:39.555856 pie_extended-0.1.3/pie_extended/pipeline/iterators/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        3 2019-12-19 17:13:20.000000 pie_extended-0.1.3/pie_extended/pipeline/iterators/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     5461 2021-01-13 15:24:27.000000 pie_extended-0.1.3/pie_extended/pipeline/iterators/proto.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2024-05-30 08:57:39.555856 pie_extended-0.1.3/pie_extended/pipeline/postprocessor/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2020-02-25 14:02:45.000000 pie_extended-0.1.3/pie_extended/pipeline/postprocessor/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     4614 2021-02-11 09:35:40.000000 pie_extended-0.1.3/pie_extended/pipeline/postprocessor/glue.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     3723 2020-04-23 14:53:46.000000 pie_extended-0.1.3/pie_extended/pipeline/postprocessor/memory.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     5455 2021-02-11 09:26:29.000000 pie_extended-0.1.3/pie_extended/pipeline/postprocessor/proto.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1863 2020-04-23 14:53:46.000000 pie_extended-0.1.3/pie_extended/pipeline/postprocessor/rulebased.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     2887 2020-05-05 15:15:28.000000 pie_extended-0.1.3/pie_extended/pipeline/postprocessor/splitter.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2024-05-30 08:57:39.555856 pie_extended-0.1.3/pie_extended/pipeline/tokenizers/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2019-12-19 17:06:18.000000 pie_extended-0.1.3/pie_extended/pipeline/tokenizers/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     2000 2020-08-20 16:54:07.000000 pie_extended-0.1.3/pie_extended/pipeline/tokenizers/memorizing.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     2537 2020-12-04 18:21:14.000000 pie_extended-0.1.3/pie_extended/pipeline/tokenizers/simple_tokenizer.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2024-05-30 08:57:39.555856 pie_extended-0.1.3/pie_extended/pipeline/tokenizers/utils/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2020-08-20 16:54:07.000000 pie_extended-0.1.3/pie_extended/pipeline/tokenizers/utils/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)       86 2020-09-08 15:47:36.000000 pie_extended-0.1.3/pie_extended/pipeline/tokenizers/utils/chars.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)    11495 2024-05-30 08:54:32.000000 pie_extended-0.1.3/pie_extended/pipeline/tokenizers/utils/excluder.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      601 2020-09-08 15:53:07.000000 pie_extended-0.1.3/pie_extended/pipeline/tokenizers/utils/regexps.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     4979 2022-05-10 08:17:38.000000 pie_extended-0.1.3/pie_extended/tagger.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2024-05-30 08:57:39.555856 pie_extended-0.1.3/pie_extended/testing_utils/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     3800 2020-08-20 16:54:07.000000 pie_extended-0.1.3/pie_extended/testing_utils/__init__.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2024-05-30 08:57:39.555856 pie_extended-0.1.3/pie_extended/utils/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1537 2020-05-05 15:15:28.000000 pie_extended-0.1.3/pie_extended/utils/__init__.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2024-05-30 08:57:39.551856 pie_extended-0.1.3/pie_extended.egg-info/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     6606 2024-05-30 08:57:39.000000 pie_extended-0.1.3/pie_extended.egg-info/PKG-INFO
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     2562 2024-05-30 08:57:39.000000 pie_extended-0.1.3/pie_extended.egg-info/SOURCES.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        1 2024-05-30 08:57:39.000000 pie_extended-0.1.3/pie_extended.egg-info/dependency_links.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)       64 2024-05-30 08:57:39.000000 pie_extended-0.1.3/pie_extended.egg-info/entry_points.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      130 2024-05-30 08:57:39.000000 pie_extended-0.1.3/pie_extended.egg-info/requires.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)       19 2024-05-30 08:57:39.000000 pie_extended-0.1.3/pie_extended.egg-info/top_level.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)       38 2024-05-30 08:57:39.555856 pie_extended-0.1.3/setup.cfg
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     3799 2024-05-30 08:54:46.000000 pie_extended-0.1.3/setup.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2024-05-30 08:57:39.551856 pie_extended-0.1.3/tests/
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2024-05-30 08:57:39.555856 pie_extended-0.1.3/tests/test_models/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2019-12-20 08:44:57.000000 pie_extended-0.1.3/tests/test_models/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     4278 2020-04-28 14:13:57.000000 pie_extended-0.1.3/tests/test_models/test_fr.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1424 2020-08-20 16:54:07.000000 pie_extended-0.1.3/tests/test_models/test_fro.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     9770 2020-12-04 16:36:08.000000 pie_extended-0.1.3/tests/test_models/test_lasla.py
```

### Comparing `pie_extended-0.1.2/LICENSE` & `pie_extended-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/PKG-INFO` & `pie_extended-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pie_extended
-Version: 0.1.2
+Version: 0.1.3
 Summary: Extension for nlp-pie package
 Home-page: https://github.com/hipster-philology/nlp-pie-taggers
 Author: Thibault Clérice
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Text Processing :: Linguistic
-Requires-Python: >=3.6.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Pie Extended
 
 [![Build Status](https://travis-ci.org/hipster-philology/nlp-pie-taggers.svg?branch=master)](https://travis-ci.org/hipster-philology/nlp-pie-taggers)
```

### Comparing `pie_extended-0.1.2/README.md` & `pie_extended-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/pie_extended/cli/main.py` & `pie_extended-0.1.3/pie_extended/cli/main.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/pie_extended/cli/utils.py` & `pie_extended-0.1.3/pie_extended/cli/utils.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/pie_extended/models/dum/__init__.py` & `pie_extended-0.1.3/pie_extended/models/dum/__init__.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/pie_extended/models/fr/__init__.py` & `pie_extended-0.1.3/pie_extended/models/fr/__init__.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/pie_extended/models/fr/excluders.py` & `pie_extended-0.1.3/pie_extended/models/fr/excluders.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/pie_extended/models/fr/imports.py` & `pie_extended-0.1.3/pie_extended/models/fr/imports.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/pie_extended/models/fr/processor.py` & `pie_extended-0.1.3/pie_extended/models/fr/processor.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/pie_extended/models/fr/tokenizer.py` & `pie_extended-0.1.3/pie_extended/models/fr/tokenizer.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/pie_extended/models/freem/__init__.py` & `pie_extended-0.1.3/pie_extended/models/freem/__init__.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/pie_extended/models/freem/imports.py` & `pie_extended-0.1.3/pie_extended/models/freem/imports.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/pie_extended/models/fro/__init__.py` & `pie_extended-0.1.3/pie_extended/models/fro/__init__.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/pie_extended/models/fro/imports.py` & `pie_extended-0.1.3/pie_extended/models/fro/imports.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/pie_extended/models/fro/processor.py` & `pie_extended-0.1.3/pie_extended/models/fro/processor.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/pie_extended/models/fro/tokenizer.py` & `pie_extended-0.1.3/pie_extended/models/fro/tokenizer.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/pie_extended/models/grc/__init__.py` & `pie_extended-0.1.3/pie_extended/models/grc/__init__.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/pie_extended/models/grc/imports.py` & `pie_extended-0.1.3/pie_extended/models/grc/imports.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/pie_extended/models/grc/processor.py` & `pie_extended-0.1.3/pie_extended/models/grc/processor.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/pie_extended/models/grc/tokenizer.py` & `pie_extended-0.1.3/pie_extended/models/grc/tokenizer.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/pie_extended/models/lasla/__init__.py` & `pie_extended-0.1.3/pie_extended/models/lasla/__init__.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/pie_extended/models/lasla/_params.py` & `pie_extended-0.1.3/pie_extended/models/lasla/_params.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/pie_extended/models/lasla/imports.py` & `pie_extended-0.1.3/pie_extended/models/lasla/imports.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/pie_extended/models/lasla/processor.py` & `pie_extended-0.1.3/pie_extended/models/lasla/processor.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/pie_extended/models/lasla/tokenizer.py` & `pie_extended-0.1.3/pie_extended/models/lasla/tokenizer.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/pie_extended/pipeline/disambiguators/autocat.py` & `pie_extended-0.1.3/pie_extended/pipeline/disambiguators/autocat.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/pie_extended/pipeline/formatters/proto.py` & `pie_extended-0.1.3/pie_extended/pipeline/formatters/proto.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/pie_extended/pipeline/iterators/proto.py` & `pie_extended-0.1.3/pie_extended/pipeline/iterators/proto.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/pie_extended/pipeline/postprocessor/glue.py` & `pie_extended-0.1.3/pie_extended/pipeline/postprocessor/glue.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/pie_extended/pipeline/postprocessor/memory.py` & `pie_extended-0.1.3/pie_extended/pipeline/postprocessor/memory.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/pie_extended/pipeline/postprocessor/proto.py` & `pie_extended-0.1.3/pie_extended/pipeline/postprocessor/proto.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/pie_extended/pipeline/postprocessor/rulebased.py` & `pie_extended-0.1.3/pie_extended/pipeline/postprocessor/rulebased.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/pie_extended/pipeline/postprocessor/splitter.py` & `pie_extended-0.1.3/pie_extended/pipeline/postprocessor/splitter.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/pie_extended/pipeline/tokenizers/memorizing.py` & `pie_extended-0.1.3/pie_extended/pipeline/tokenizers/memorizing.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/pie_extended/pipeline/tokenizers/simple_tokenizer.py` & `pie_extended-0.1.3/pie_extended/pipeline/tokenizers/simple_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/pie_extended/pipeline/tokenizers/utils/excluder.py` & `pie_extended-0.1.3/pie_extended/pipeline/tokenizers/utils/excluder.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,17 +289,18 @@
     """Allows for keeping apostrophes that are the mark of an elision, mostly in French such as
     "l'abbé"
     """
     def __init__(self,
                  match_apostrophes=chars.APOSTROPHE,
                  char_registry: Optional[CharRegistry] = None,
                  add_space_after: bool = True,
-                 add_space_before: bool = False):
+                 add_space_before: bool = False,
+                 regex: Optional[str] = None):
         self.apostrophes = match_apostrophes
-        self.re: re.Regex = re.compile(r"(\w+)([" + self.apostrophes + r"])(\w+)")
+        self.re: re.Regex = re.compile(regex or (r"(\w+)([" + self.apostrophes + r"])(\w+)"))
         self.char_registry = char_registry or CharRegistry()
 
         # Space handling
         self.space_before: str = ""
         if add_space_before:
             self.space_before = " "
```

### Comparing `pie_extended-0.1.2/pie_extended/pipeline/tokenizers/utils/regexps.py` & `pie_extended-0.1.3/pie_extended/pipeline/tokenizers/utils/regexps.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/pie_extended/tagger.py` & `pie_extended-0.1.3/pie_extended/tagger.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/pie_extended/testing_utils/__init__.py` & `pie_extended-0.1.3/pie_extended/testing_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/pie_extended/utils/__init__.py` & `pie_extended-0.1.3/pie_extended/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/pie_extended.egg-info/PKG-INFO` & `pie_extended-0.1.3/pie_extended.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pie-extended
-Version: 0.1.2
+Version: 0.1.3
 Summary: Extension for nlp-pie package
 Home-page: https://github.com/hipster-philology/nlp-pie-taggers
 Author: Thibault Clérice
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Text Processing :: Linguistic
-Requires-Python: >=3.6.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Pie Extended
 
 [![Build Status](https://travis-ci.org/hipster-philology/nlp-pie-taggers.svg?branch=master)](https://travis-ci.org/hipster-philology/nlp-pie-taggers)
```

### Comparing `pie_extended-0.1.2/pie_extended.egg-info/SOURCES.txt` & `pie_extended-0.1.3/pie_extended.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,18 @@
 pie_extended/models/grc/processor.py
 pie_extended/models/grc/tokenizer.py
 pie_extended/models/lasla/__init__.py
 pie_extended/models/lasla/_params.py
 pie_extended/models/lasla/imports.py
 pie_extended/models/lasla/processor.py
 pie_extended/models/lasla/tokenizer.py
+pie_extended/models/occ_cont/__init__.py
+pie_extended/models/occ_cont/imports.py
+pie_extended/models/occ_cont/processor.py
+pie_extended/models/occ_cont/tokenizer.py
 pie_extended/pipeline/__init__.py
 pie_extended/pipeline/disambiguators/__init__.py
 pie_extended/pipeline/disambiguators/autocat.py
 pie_extended/pipeline/disambiguators/proto.py
 pie_extended/pipeline/formatters/__init__.py
 pie_extended/pipeline/formatters/proto.py
 pie_extended/pipeline/iterators/__init__.py
```

### Comparing `pie_extended-0.1.2/setup.py` & `pie_extended-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Package meta-data.
 NAME = 'pie_extended'
 DESCRIPTION = "Extension for nlp-pie package"
 URL = 'https://github.com/hipster-philology/nlp-pie-taggers'
 AUTHOR = 'Thibault Clérice'
-REQUIRES_PYTHON = '>=3.6.0'
-VERSION = "0.1.2"
+REQUIRES_PYTHON = '>=3.8.0'
+VERSION = "0.1.3"
 
 # What packages are required for this module to be executed?
 
 with open(os.path.join(here, 'requirements.txt')) as f:
     REQUIRED = f.read().splitlines()
 
 # What packages are optional?
```

### Comparing `pie_extended-0.1.2/tests/test_models/test_fr.py` & `pie_extended-0.1.3/tests/test_models/test_fr.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/tests/test_models/test_fro.py` & `pie_extended-0.1.3/tests/test_models/test_fro.py`

 * *Files identical despite different names*

### Comparing `pie_extended-0.1.2/tests/test_models/test_lasla.py` & `pie_extended-0.1.3/tests/test_models/test_lasla.py`

 * *Files identical despite different names*

