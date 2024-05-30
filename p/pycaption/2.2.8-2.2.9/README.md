# Comparing `tmp/pycaption-2.2.8.tar.gz` & `tmp/pycaption-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycaption-2.2.8.tar", last modified: Thu May 23 08:44:32 2024, max compression
+gzip compressed data, was "pycaption-2.2.9.tar", last modified: Fri May 24 07:15:17 2024, max compression
```

## Comparing `pycaption-2.2.8.tar` & `pycaption-2.2.9.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:44:32.771030 pycaption-2.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-05-23 08:44:19.000000 pycaption-2.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-23 08:44:19.000000 pycaption-2.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-23 08:44:32.771030 pycaption-2.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-23 08:44:19.000000 pycaption-2.2.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:44:32.759030 pycaption-2.2.8/pycaption/
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-23 08:44:19.000000 pycaption-2.2.8/pycaption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13730 2024-05-23 08:44:19.000000 pycaption-2.2.8/pycaption/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:44:32.763030 pycaption-2.2.8/pycaption/dfxp/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-23 08:44:19.000000 pycaption-2.2.8/pycaption/dfxp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50759 2024-05-23 08:44:19.000000 pycaption-2.2.8/pycaption/dfxp/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8587 2024-05-23 08:44:19.000000 pycaption-2.2.8/pycaption/dfxp/extras.py
--rw-r--r--   0 runner    (1001) docker     (127)   433305 2024-05-23 08:44:19.000000 pycaption-2.2.8/pycaption/english.pickle
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-23 08:44:19.000000 pycaption-2.2.8/pycaption/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    30173 2024-05-23 08:44:19.000000 pycaption-2.2.8/pycaption/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-23 08:44:19.000000 pycaption-2.2.8/pycaption/microdvd.py
--rw-r--r--   0 runner    (1001) docker     (127)    28247 2024-05-23 08:44:19.000000 pycaption-2.2.8/pycaption/sami.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:44:32.763030 pycaption-2.2.8/pycaption/scc/
--rw-r--r--   0 runner    (1001) docker     (127)    26057 2024-05-23 08:44:19.000000 pycaption-2.2.8/pycaption/scc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28154 2024-05-23 08:44:19.000000 pycaption-2.2.8/pycaption/scc/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    28866 2024-05-23 08:44:19.000000 pycaption-2.2.8/pycaption/scc/specialized_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-05-23 08:44:19.000000 pycaption-2.2.8/pycaption/scc/state_machines.py
--rw-r--r--   0 runner    (1001) docker     (127)    32255 2024-05-23 08:44:19.000000 pycaption-2.2.8/pycaption/scc/translator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-23 08:44:19.000000 pycaption-2.2.8/pycaption/srt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-23 08:44:19.000000 pycaption-2.2.8/pycaption/transcript.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-23 08:44:19.000000 pycaption-2.2.8/pycaption/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17052 2024-05-23 08:44:19.000000 pycaption-2.2.8/pycaption/webvtt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:44:32.767030 pycaption-2.2.8/pycaption.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-23 08:44:32.000000 pycaption-2.2.8/pycaption.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-23 08:44:32.000000 pycaption-2.2.8/pycaption.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 08:44:32.000000 pycaption-2.2.8/pycaption.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-23 08:44:32.000000 pycaption-2.2.8/pycaption.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-23 08:44:32.000000 pycaption-2.2.8/pycaption.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 08:44:32.771030 pycaption-2.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-23 08:44:19.000000 pycaption-2.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:44:32.767030 pycaption-2.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:44:32.767030 pycaption-2.2.8/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49641 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/fixtures/dfxp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/fixtures/microdvd.py
--rw-r--r--   0 runner    (1001) docker     (127)    17112 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/fixtures/sami.py
--rw-r--r--   0 runner    (1001) docker     (127)    15380 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/fixtures/scc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/fixtures/srt.py
--rw-r--r--   0 runner    (1001) docker     (127)    11018 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/fixtures/translated_scc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7224 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/fixtures/webvtt.py
--rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8400 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/test_dfxp.py
--rw-r--r--   0 runner    (1001) docker     (127)    14453 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/test_dfxp_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/test_dfxp_extras.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/test_microdvd.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/test_microdvd_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/test_sami.py
--rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/test_sami_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)    23573 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/test_scc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/test_scc_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/test_scc_translator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/test_srt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/test_srt_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/test_webvtt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/test_webvtt_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:15:17.885135 pycaption-2.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-05-24 07:15:07.000000 pycaption-2.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-24 07:15:07.000000 pycaption-2.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-24 07:15:17.885135 pycaption-2.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-24 07:15:07.000000 pycaption-2.2.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:15:17.877135 pycaption-2.2.9/pycaption/
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-24 07:15:07.000000 pycaption-2.2.9/pycaption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13730 2024-05-24 07:15:07.000000 pycaption-2.2.9/pycaption/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:15:17.877135 pycaption-2.2.9/pycaption/dfxp/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-24 07:15:07.000000 pycaption-2.2.9/pycaption/dfxp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50759 2024-05-24 07:15:07.000000 pycaption-2.2.9/pycaption/dfxp/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8587 2024-05-24 07:15:07.000000 pycaption-2.2.9/pycaption/dfxp/extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)   433305 2024-05-24 07:15:07.000000 pycaption-2.2.9/pycaption/english.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-24 07:15:07.000000 pycaption-2.2.9/pycaption/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30173 2024-05-24 07:15:07.000000 pycaption-2.2.9/pycaption/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-24 07:15:07.000000 pycaption-2.2.9/pycaption/microdvd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28247 2024-05-24 07:15:07.000000 pycaption-2.2.9/pycaption/sami.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:15:17.877135 pycaption-2.2.9/pycaption/scc/
+-rw-r--r--   0 runner    (1001) docker     (127)    26004 2024-05-24 07:15:07.000000 pycaption-2.2.9/pycaption/scc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28154 2024-05-24 07:15:07.000000 pycaption-2.2.9/pycaption/scc/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28825 2024-05-24 07:15:07.000000 pycaption-2.2.9/pycaption/scc/specialized_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-05-24 07:15:07.000000 pycaption-2.2.9/pycaption/scc/state_machines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32255 2024-05-24 07:15:07.000000 pycaption-2.2.9/pycaption/scc/translator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-24 07:15:07.000000 pycaption-2.2.9/pycaption/srt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-24 07:15:07.000000 pycaption-2.2.9/pycaption/transcript.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-24 07:15:07.000000 pycaption-2.2.9/pycaption/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17052 2024-05-24 07:15:07.000000 pycaption-2.2.9/pycaption/webvtt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:15:17.885135 pycaption-2.2.9/pycaption.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-24 07:15:17.000000 pycaption-2.2.9/pycaption.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-24 07:15:17.000000 pycaption-2.2.9/pycaption.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 07:15:17.000000 pycaption-2.2.9/pycaption.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-24 07:15:17.000000 pycaption-2.2.9/pycaption.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-24 07:15:17.000000 pycaption-2.2.9/pycaption.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 07:15:17.885135 pycaption-2.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-24 07:15:07.000000 pycaption-2.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:15:17.881135 pycaption-2.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 07:15:07.000000 pycaption-2.2.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-05-24 07:15:07.000000 pycaption-2.2.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:15:17.881135 pycaption-2.2.9/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 07:15:07.000000 pycaption-2.2.9/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49641 2024-05-24 07:15:07.000000 pycaption-2.2.9/tests/fixtures/dfxp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-24 07:15:07.000000 pycaption-2.2.9/tests/fixtures/microdvd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17112 2024-05-24 07:15:07.000000 pycaption-2.2.9/tests/fixtures/sami.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15380 2024-05-24 07:15:07.000000 pycaption-2.2.9/tests/fixtures/scc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-24 07:15:07.000000 pycaption-2.2.9/tests/fixtures/srt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11018 2024-05-24 07:15:07.000000 pycaption-2.2.9/tests/fixtures/translated_scc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7224 2024-05-24 07:15:07.000000 pycaption-2.2.9/tests/fixtures/webvtt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-05-24 07:15:07.000000 pycaption-2.2.9/tests/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-05-24 07:15:07.000000 pycaption-2.2.9/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8400 2024-05-24 07:15:07.000000 pycaption-2.2.9/tests/test_dfxp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14453 2024-05-24 07:15:07.000000 pycaption-2.2.9/tests/test_dfxp_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-05-24 07:15:07.000000 pycaption-2.2.9/tests/test_dfxp_extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-24 07:15:07.000000 pycaption-2.2.9/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-05-24 07:15:07.000000 pycaption-2.2.9/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-24 07:15:07.000000 pycaption-2.2.9/tests/test_microdvd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-24 07:15:07.000000 pycaption-2.2.9/tests/test_microdvd_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-05-24 07:15:07.000000 pycaption-2.2.9/tests/test_sami.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-05-24 07:15:07.000000 pycaption-2.2.9/tests/test_sami_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23413 2024-05-24 07:15:07.000000 pycaption-2.2.9/tests/test_scc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-24 07:15:07.000000 pycaption-2.2.9/tests/test_scc_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-24 07:15:07.000000 pycaption-2.2.9/tests/test_scc_translator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-24 07:15:07.000000 pycaption-2.2.9/tests/test_srt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-24 07:15:07.000000 pycaption-2.2.9/tests/test_srt_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-05-24 07:15:07.000000 pycaption-2.2.9/tests/test_webvtt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-24 07:15:07.000000 pycaption-2.2.9/tests/test_webvtt_conversion.py
```

### Comparing `pycaption-2.2.8/LICENSE` & `pycaption-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/PKG-INFO` & `pycaption-2.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycaption
-Version: 2.2.8
+Version: 2.2.9
 Summary: Closed caption converter
 Author: Joe Norton
 Author-email: joey@nortoncrew.com
 Project-URL: Source, https://github.com/pbs/pycaption
 Project-URL: Documentation, https://pycaption.readthedocs.io/
 Project-URL: Release notes, https://pycaption.readthedocs.io/en/stable/changelog.html
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pycaption-2.2.8/README.rst` & `pycaption-2.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/pycaption/__init__.py` & `pycaption-2.2.9/pycaption/__init__.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/pycaption/base.py` & `pycaption-2.2.9/pycaption/base.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/pycaption/dfxp/base.py` & `pycaption-2.2.9/pycaption/dfxp/base.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/pycaption/dfxp/extras.py` & `pycaption-2.2.9/pycaption/dfxp/extras.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/pycaption/english.pickle` & `pycaption-2.2.9/pycaption/english.pickle`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/pycaption/exceptions.py` & `pycaption-2.2.9/pycaption/exceptions.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/pycaption/geometry.py` & `pycaption-2.2.9/pycaption/geometry.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/pycaption/microdvd.py` & `pycaption-2.2.9/pycaption/microdvd.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/pycaption/sami.py` & `pycaption-2.2.9/pycaption/sami.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/pycaption/scc/__init__.py` & `pycaption-2.2.9/pycaption/scc/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -309,32 +309,34 @@
         self.time_translator.start_at(parts[0][0])
 
         word_list = parts[0][2].split(' ')
         pacs_are_doubled = len(word_list) > 1 and word_list[0] == word_list[1]
         for idx, word in enumerate(word_list):
             # ignore empty results or invalid commands
             word = word.strip()
-            previous_is_pac = idx > 0 and _is_pac_command(word_list[idx-1])
+            previous_is_pac_or_tab = idx > 0 and (
+                _is_pac_command(word_list[idx-1]) or word_list[idx-1] in PAC_TAB_OFFSET_COMMANDS
+            )
             if len(word) == 4:
                 self._translate_word(
                     word=word,
-                    previous_is_pac=previous_is_pac,
+                    previous_is_pac_or_tab=previous_is_pac_or_tab,
                     pacs_are_doubled=pacs_are_doubled
                 )
 
-    def _translate_word(self, word, previous_is_pac, pacs_are_doubled):
+    def _translate_word(self, word, previous_is_pac_or_tab, pacs_are_doubled):
         if self._handle_double_command(word, pacs_are_doubled):
             # count frames for timing
             self.time_translator.increment_frames()
             return
         # first check if word is a command
         # TODO - check that all the positioning commands are here, or use
         # some other strategy to determine if the word is a command.
         if word in COMMANDS or _is_pac_command(word):
-            self._translate_command(word=word, previous_is_pac=previous_is_pac)
+            self._translate_command(word=word, previous_is_pac_or_tab=previous_is_pac_or_tab)
 
         # second, check if word is a special character
         elif word in SPECIAL_CHARS:
             self._translate_special_char(word)
 
         elif word in EXTENDED_CHARS:
             self._translate_extended_char(word)
@@ -350,18 +352,15 @@
         # If the caption is to be broadcast, each of the commands are doubled
         # up for redundancy in case the signal is garbled in transmission.
         # The decoder is programmed to ignore a second command when it is the
         # same as the first.
         # If we have doubled commands we're skipping also
         # doubled special characters and doubled extended characters
         # with only one member of each pair being displayed.
-        actionable_commands = {
-            key: COMMANDS[key] for key in COMMANDS.keys() if key != "94a1"
-        }
-        doubled_types = word in actionable_commands or _is_pac_command(word)
+        doubled_types = word in COMMANDS or _is_pac_command(word)
         if pacs_are_doubled:
             doubled_types = doubled_types or word in SPECIAL_CHARS or word in EXTENDED_CHARS
 
         if doubled_types and word == self.last_command:
             return True
             # Fix for the <position> <tab offset> <position> <tab offset>
             # repetition
@@ -375,31 +374,29 @@
             else:
                 return True
 
         self.last_command = word
         return False
 
     def _translate_special_char(self, word):
-        self.buffer.handle_backspace(word)
-        # add to buffer
         self.buffer.add_chars(SPECIAL_CHARS[word])
 
     def _translate_extended_char(self, word):
         """
         Each of the 64 Extended Characters incorporates an automatic BS.
         When an Extended Character is received, the cursor moves to the
         left one column position (unless the Extended Character is the first
         character on a row), erasing any character which may be in that location,
         then displays the Extended Character.
         """
         self.buffer.handle_backspace(word)
         # add to buffer
         self.buffer.add_chars(EXTENDED_CHARS[word])
 
-    def _translate_command(self, word, previous_is_pac):
+    def _translate_command(self, word, previous_is_pac_or_tab):
         # if command is pop_up
         if word == '9420':
             self.buffer_dict.set_active('pop')
 
         # command is paint_on [Resume Direct Captioning]
         elif word == '9429':
             self.buffer_dict.set_active('paint')
@@ -462,15 +459,15 @@
         elif word == '942c' and self.pop_ons_queue:
             self._pop_on(end=self.time_translator.get_time())
 
         # If command is not one of the aforementioned, add it to buffer
         else:
             self.buffer.interpret_command(
                 command=word,
-                previous_is_pac=previous_is_pac
+                previous_is_pac_or_tab=previous_is_pac_or_tab
             )
 
     def _translate_characters(self, word):
         # split word into the 2 bytes
         byte1 = word[:2]
         byte2 = word[2:]
```

### Comparing `pycaption-2.2.8/pycaption/scc/constants.py` & `pycaption-2.2.9/pycaption/scc/constants.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/pycaption/scc/specialized_collections.py` & `pycaption-2.2.9/pycaption/scc/specialized_collections.py`

 * *Files 2% similar despite different names*

```diff
@@ -333,22 +333,23 @@
             )
             node = _InstructionNode.create_text(current_position)
             self._collection.append(node)
             self._position_tracer.acknowledge_position_changed()
 
         node.add_chars(*chars)
 
-    def interpret_command(self, command, previous_is_pac=None):
+    def interpret_command(self, command, previous_is_pac_or_tab=False):
         """Given a command determines whether to turn italics on or off,
         or to set the positioning
 
         This is mostly used to convert from the legacy-style commands
 
         :type command: str
-        :type mode: pop or roll or paint
+        :type previous_is_pac_or_tab: previous command code is for a PAC command
+        or a PAC_TAB_OFFSET_COMMANDS
         """
         self._update_positioning(command)
 
         text = COMMANDS.get(command, '')
 
         if command == "94a1":
             self.handle_backspace("94a1")
@@ -378,16 +379,15 @@
                         turn_on=False
                     )
                 )
                 self.last_style = "italics off"
 
         # mid row code that is not first code on the line
         # (previous node is not a break node)
-        # fixes OCTO-11022
-        if command in MID_ROW_CODES and not previous_is_pac:
+        if command in MID_ROW_CODES and not previous_is_pac_or_tab:
             if self.last_style == "italics off":
                 self.add_chars(' ')
             else:
                 for node in self._collection[::-1]:
                     if node.is_text_node() and node.text:
                         node.text += ' '
                         break
@@ -452,20 +452,19 @@
         # in case of no previous text nodes or
         # if the backspace is required while no character
         # do nothing
         if node is None:
             return
         last_char = node.text[-1]
         delete_previous_condition = (
-            (word in SPECIAL_CHARS and last_char not in SPECIAL_CHARS.values()) or
             (word in EXTENDED_CHARS and last_char not in EXTENDED_CHARS.values()) or
             word == "94a1"
         )
-        # in case of special / extended char, perform backspace
-        # only if the previous character in not also special / extended
+        # in case extended char, perform backspace
+        # only if the previous character in not also extended
         if delete_previous_condition:
             node.text = node.text[:-1]
 
     def get_previous_text_node(self):
         for node in self._collection[::-1]:
             if node.is_text_node() and node.text:
                 return node
```

### Comparing `pycaption-2.2.8/pycaption/scc/state_machines.py` & `pycaption-2.2.9/pycaption/scc/state_machines.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/pycaption/scc/translator.py` & `pycaption-2.2.9/pycaption/scc/translator.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/pycaption/srt.py` & `pycaption-2.2.9/pycaption/srt.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/pycaption/transcript.py` & `pycaption-2.2.9/pycaption/transcript.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/pycaption/webvtt.py` & `pycaption-2.2.9/pycaption/webvtt.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/pycaption.egg-info/PKG-INFO` & `pycaption-2.2.9/pycaption.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycaption
-Version: 2.2.8
+Version: 2.2.9
 Summary: Closed caption converter
 Author: Joe Norton
 Author-email: joey@nortoncrew.com
 Project-URL: Source, https://github.com/pbs/pycaption
 Project-URL: Documentation, https://pycaption.readthedocs.io/
 Project-URL: Release notes, https://pycaption.readthedocs.io/en/stable/changelog.html
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pycaption-2.2.8/pycaption.egg-info/SOURCES.txt` & `pycaption-2.2.9/pycaption.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/setup.py` & `pycaption-2.2.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 transcript_dependencies = [
     'nltk'
 ]
 
 setup(
     name='pycaption',
-    version='2.2.8',
+    version='2.2.9',
     description='Closed caption converter',
     long_description=open(README_PATH).read(),
     author='Joe Norton',
     author_email='joey@nortoncrew.com',
     project_urls={
         'Source': 'https://github.com/pbs/pycaption',
         'Documentation': 'https://pycaption.readthedocs.io/',
```

### Comparing `pycaption-2.2.8/tests/conftest.py` & `pycaption-2.2.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/tests/fixtures/dfxp.py` & `pycaption-2.2.9/tests/fixtures/dfxp.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/tests/fixtures/microdvd.py` & `pycaption-2.2.9/tests/fixtures/microdvd.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/tests/fixtures/sami.py` & `pycaption-2.2.9/tests/fixtures/sami.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/tests/fixtures/scc.py` & `pycaption-2.2.9/tests/fixtures/scc.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/tests/fixtures/srt.py` & `pycaption-2.2.9/tests/fixtures/srt.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/tests/fixtures/translated_scc.py` & `pycaption-2.2.9/tests/fixtures/translated_scc.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/tests/fixtures/webvtt.py` & `pycaption-2.2.9/tests/fixtures/webvtt.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/tests/mixins.py` & `pycaption-2.2.9/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/tests/test_base.py` & `pycaption-2.2.9/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/tests/test_dfxp.py` & `pycaption-2.2.9/tests/test_dfxp.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/tests/test_dfxp_conversion.py` & `pycaption-2.2.9/tests/test_dfxp_conversion.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/tests/test_dfxp_extras.py` & `pycaption-2.2.9/tests/test_dfxp_extras.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/tests/test_functions.py` & `pycaption-2.2.9/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/tests/test_geometry.py` & `pycaption-2.2.9/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/tests/test_microdvd.py` & `pycaption-2.2.9/tests/test_microdvd.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/tests/test_microdvd_conversion.py` & `pycaption-2.2.9/tests/test_microdvd_conversion.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/tests/test_sami.py` & `pycaption-2.2.9/tests/test_sami.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/tests/test_sami_conversion.py` & `pycaption-2.2.9/tests/test_sami_conversion.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/tests/test_scc.py` & `pycaption-2.2.9/tests/test_scc.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,37 +200,36 @@
         assert captions[0].nodes[0].content == 'MÄRTHA:'
         expected_result = ['JUNIOR: ¡Yum!', None, 'Ya me siento mucho mejor.']
         content = [node.content for node in captions[1].nodes]
         assert all(result in expected_result for result in content)
 
     def test_skip_duplicate_tab_offset(self, sample_scc_duplicate_tab_offset):
         expected_lines = [
-            '[Radio reporter] ',
-            'The I-10 Santa Monica Freeway ',
+            '[Radio reporter]',
+            'The I-10 Santa Monica Freeway',
             'westbound is jammed,',
-            'due to a three-car accident ',
+            'due to a three-car accident',
             'blocking lanes 1 and 2'
         ]
 
         caption_set = SCCReader().read(sample_scc_duplicate_tab_offset)
         actual_lines = [
             node.content
             for cap_ in caption_set.get_captions('en-US')
             for node in cap_.nodes
             if node.type_ == CaptionNode.TEXT
         ]
-
         assert expected_lines == actual_lines
 
     def test_skip_duplicate_special_characters(
             self, sample_scc_duplicate_special_characters):
         expected_lines = [
-            '®°½¿™¢£♪à èâêîôû',   # double commands so we skip one
-            '®°½¿™¢£♪à èâêîôû',   # no double command, nothing skipped equal with above
-            '®°A½¿™¢£♪à èâêAîôû'  # no skips but a couple of normal chars "c1c1" = AA
+            '®°½¿™¢£♪à èâêîôû',
+            '®°½¿™¢£♪à èâêîôû',
+            '®°AA½¿™¢£♪à èâêAAîôû'
         ]
 
         caption_set = SCCReader().read(sample_scc_duplicate_special_characters)
         actual_lines = [
             node.content
             for cap_ in caption_set.get_captions('en-US')
             for node in cap_.nodes
@@ -270,29 +269,29 @@
         # There were no tests for ROLL-UP captions, but the library processed
         # Roll-Up captions. Make sure nothing changes during the refactoring
         scc1 = SCCReader().read(sample_scc_roll_up_ru2)
         captions = scc1.get_captions('en-US')
         actual_texts = [cap_.nodes[0].content for cap_ in captions]
         expected_texts = [
             '>>> HI.',
-             "I'M KEVIN CUNNING AND AT",
-             "INVESTOR'S BANK WE BELIEVE IN",
-             'HELPING THE LOCAL NEIGHBORHOODS',
-             'AND IMPROVING THE LIVES OF ALL',
-             'WE SERVE.',
-             '®°½',
-             'Aû',
-             'ÁÉÓ¡',
-             "WHERE YOU'RE STANDING NOW,",
-             "LOOKING OUT THERE, THAT'S AL",
-             'THE CROWD.',
-             '>> IT WAS GOOD TO BE IN TH',
-             "And restore Iowa's land, water",
-             'And wildlife.',
-             '>> Bike Iowa, your source for'
+            "I'M KEVIN CUNNING AND AT",
+            "INVESTOR'S BANK WE BELIEVE IN",
+            'HELPING THE LOCAL NEIGHBORHOODS',
+            'AND IMPROVING THE LIVES OF ALL',
+            'WE SERVE.',
+            '®°½',
+            'ABû',
+            'ÁÉÓ¡',
+            "WHERE YOU'RE STANDING NOW,",
+            "LOOKING OUT THERE, THAT'S AL",
+            'THE CROWD.',
+            '>> IT WAS GOOD TO BE IN TH',
+            "And restore Iowa's land, water",
+            'And wildlife.',
+            '>> Bike Iowa, your source for'
         ]
         assert expected_texts == actual_texts
 
     def test_multiple_formats(self, sample_scc_multiple_formats):
         # Test for captions that contain both pop on and paint on formats to
         # ensure the paint on lines are not repeated
         expected_text_lines = [
```

### Comparing `pycaption-2.2.8/tests/test_scc_conversion.py` & `pycaption-2.2.9/tests/test_scc_conversion.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/tests/test_scc_translator.py` & `pycaption-2.2.9/tests/test_scc_translator.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/tests/test_srt.py` & `pycaption-2.2.9/tests/test_srt.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/tests/test_srt_conversion.py` & `pycaption-2.2.9/tests/test_srt_conversion.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/tests/test_webvtt.py` & `pycaption-2.2.9/tests/test_webvtt.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.8/tests/test_webvtt_conversion.py` & `pycaption-2.2.9/tests/test_webvtt_conversion.py`

 * *Files identical despite different names*

