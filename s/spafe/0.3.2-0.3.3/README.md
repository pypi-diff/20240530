# Comparing `tmp/spafe-0.3.2.tar.gz` & `tmp/spafe-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spafe-0.3.2.tar", last modified: Tue Feb 28 22:43:59 2023, max compression
+gzip compressed data, was "spafe-0.3.3.tar", last modified: Thu May 30 18:07:21 2024, max compression
```

## Comparing `spafe-0.3.2.tar` & `spafe-0.3.3.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-02-28 22:43:59.680813 spafe-0.3.2/
--rw-rw-r--   0 am        (1000) am        (1000)     1519 2023-02-28 00:21:17.000000 spafe-0.3.2/LICENSE
--rw-rw-r--   0 am        (1000) am        (1000)     7933 2023-02-28 22:43:59.680813 spafe-0.3.2/PKG-INFO
--rw-rw-r--   0 am        (1000) am        (1000)     6880 2023-02-28 00:21:17.000000 spafe-0.3.2/README.md
--rw-rw-r--   0 am        (1000) am        (1000)       38 2023-02-28 22:43:59.680813 spafe-0.3.2/setup.cfg
--rw-rw-r--   0 am        (1000) am        (1000)     2031 2023-02-28 22:43:28.000000 spafe-0.3.2/setup.py
-drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-02-28 22:43:59.676813 spafe-0.3.2/spafe/
--rw-rw-r--   0 am        (1000) am        (1000)      291 2023-02-28 00:21:17.000000 spafe-0.3.2/spafe/__init__.py
-drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-02-28 22:43:59.676813 spafe-0.3.2/spafe/fbanks/
--rw-rw-r--   0 am        (1000) am        (1000)       54 2023-02-28 00:21:17.000000 spafe-0.3.2/spafe/fbanks/__init__.py
--rw-rw-r--   0 am        (1000) am        (1000)     6229 2023-02-28 00:21:17.000000 spafe-0.3.2/spafe/fbanks/bark_fbanks.py
--rw-rw-r--   0 am        (1000) am        (1000)     8460 2023-02-28 00:21:17.000000 spafe-0.3.2/spafe/fbanks/gammatone_fbanks.py
--rw-rw-r--   0 am        (1000) am        (1000)     3658 2023-02-28 00:21:17.000000 spafe-0.3.2/spafe/fbanks/linear_fbanks.py
--rw-rw-r--   0 am        (1000) am        (1000)    12750 2023-02-28 00:21:17.000000 spafe-0.3.2/spafe/fbanks/mel_fbanks.py
-drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-02-28 22:43:59.676813 spafe-0.3.2/spafe/features/
--rw-rw-r--   0 am        (1000) am        (1000)       54 2023-02-28 00:21:17.000000 spafe-0.3.2/spafe/features/__init__.py
--rw-rw-r--   0 am        (1000) am        (1000)    12967 2023-02-28 00:21:17.000000 spafe-0.3.2/spafe/features/bfcc.py
--rw-rw-r--   0 am        (1000) am        (1000)    11792 2023-02-28 00:21:17.000000 spafe-0.3.2/spafe/features/cqcc.py
--rw-rw-r--   0 am        (1000) am        (1000)    12763 2023-02-28 00:21:17.000000 spafe-0.3.2/spafe/features/gfcc.py
--rw-rw-r--   0 am        (1000) am        (1000)    11014 2023-02-28 00:21:17.000000 spafe-0.3.2/spafe/features/lfcc.py
--rw-rw-r--   0 am        (1000) am        (1000)    11834 2023-02-28 00:21:17.000000 spafe-0.3.2/spafe/features/lpc.py
--rw-rw-r--   0 am        (1000) am        (1000)    17758 2023-02-28 00:21:17.000000 spafe-0.3.2/spafe/features/mfcc.py
--rw-rw-r--   0 am        (1000) am        (1000)     7127 2023-02-28 00:21:17.000000 spafe-0.3.2/spafe/features/msrcc.py
--rw-rw-r--   0 am        (1000) am        (1000)     7476 2023-02-28 00:21:17.000000 spafe-0.3.2/spafe/features/ngcc.py
--rw-rw-r--   0 am        (1000) am        (1000)    16249 2023-02-28 00:21:17.000000 spafe-0.3.2/spafe/features/pncc.py
--rw-rw-r--   0 am        (1000) am        (1000)     7673 2023-02-28 00:21:17.000000 spafe-0.3.2/spafe/features/psrcc.py
--rw-rw-r--   0 am        (1000) am        (1000)    15741 2023-02-28 00:21:17.000000 spafe-0.3.2/spafe/features/rplp.py
--rw-rw-r--   0 am        (1000) am        (1000)    10948 2023-02-28 00:21:17.000000 spafe-0.3.2/spafe/features/spfeats.py
-drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-02-28 22:43:59.676813 spafe-0.3.2/spafe/frequencies/
--rw-rw-r--   0 am        (1000) am        (1000)       54 2023-02-28 00:21:17.000000 spafe-0.3.2/spafe/frequencies/__init__.py
--rw-rw-r--   0 am        (1000) am        (1000)     6378 2023-02-28 00:21:17.000000 spafe-0.3.2/spafe/frequencies/dominant_frequencies.py
--rw-rw-r--   0 am        (1000) am        (1000)    10511 2023-02-28 00:21:17.000000 spafe-0.3.2/spafe/frequencies/fundamental_frequencies.py
-drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-02-28 22:43:59.676813 spafe-0.3.2/spafe/utils/
--rw-rw-r--   0 am        (1000) am        (1000)       54 2023-02-28 00:21:17.000000 spafe-0.3.2/spafe/utils/__init__.py
--rw-rw-r--   0 am        (1000) am        (1000)     4119 2023-02-28 00:21:17.000000 spafe-0.3.2/spafe/utils/cepstral.py
--rw-rw-r--   0 am        (1000) am        (1000)    12809 2023-02-28 00:21:17.000000 spafe-0.3.2/spafe/utils/converters.py
--rw-rw-r--   0 am        (1000) am        (1000)      988 2023-02-28 00:21:17.000000 spafe-0.3.2/spafe/utils/exceptions.py
--rw-rw-r--   0 am        (1000) am        (1000)     2000 2023-02-28 00:21:17.000000 spafe-0.3.2/spafe/utils/filters.py
--rw-rw-r--   0 am        (1000) am        (1000)     5369 2023-02-28 00:21:17.000000 spafe-0.3.2/spafe/utils/preprocessing.py
--rw-rw-r--   0 am        (1000) am        (1000)     4950 2023-02-28 00:21:17.000000 spafe-0.3.2/spafe/utils/spectral.py
--rw-rw-r--   0 am        (1000) am        (1000)     6024 2023-02-28 00:21:17.000000 spafe-0.3.2/spafe/utils/vis.py
--rw-rw-r--   0 am        (1000) am        (1000)      255 2023-02-28 21:45:24.000000 spafe-0.3.2/spafe/version.py
-drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-02-28 22:43:59.676813 spafe-0.3.2/spafe.egg-info/
--rw-rw-r--   0 am        (1000) am        (1000)     7933 2023-02-28 22:43:59.000000 spafe-0.3.2/spafe.egg-info/PKG-INFO
--rw-rw-r--   0 am        (1000) am        (1000)     1645 2023-02-28 22:43:59.000000 spafe-0.3.2/spafe.egg-info/SOURCES.txt
--rw-rw-r--   0 am        (1000) am        (1000)        1 2023-02-28 22:43:59.000000 spafe-0.3.2/spafe.egg-info/dependency_links.txt
--rw-rw-r--   0 am        (1000) am        (1000)        1 2023-02-28 21:46:32.000000 spafe-0.3.2/spafe.egg-info/not-zip-safe
--rw-rw-r--   0 am        (1000) am        (1000)      259 2023-02-28 22:43:59.000000 spafe-0.3.2/spafe.egg-info/requires.txt
--rw-rw-r--   0 am        (1000) am        (1000)       12 2023-02-28 22:43:59.000000 spafe-0.3.2/spafe.egg-info/top_level.txt
-drwxrwxr-x   0 am        (1000) am        (1000)        0 2023-02-28 22:43:59.680813 spafe-0.3.2/tests/
--rw-rw-r--   0 am        (1000) am        (1000)      162 2023-02-28 00:21:17.000000 spafe-0.3.2/tests/__init__.py
--rw-rw-r--   0 am        (1000) am        (1000)      376 2023-02-28 00:21:17.000000 spafe-0.3.2/tests/conftest.py
--rw-rw-r--   0 am        (1000) am        (1000)     1629 2023-02-28 00:21:17.000000 spafe-0.3.2/tests/test_fbanks_bark.py
--rw-rw-r--   0 am        (1000) am        (1000)     1674 2023-02-28 00:21:17.000000 spafe-0.3.2/tests/test_fbanks_gamma.py
--rw-rw-r--   0 am        (1000) am        (1000)     1642 2023-02-28 00:21:17.000000 spafe-0.3.2/tests/test_fbanks_lin.py
--rw-rw-r--   0 am        (1000) am        (1000)     3147 2023-02-28 00:21:17.000000 spafe-0.3.2/tests/test_fbanks_mel.py
--rw-rw-r--   0 am        (1000) am        (1000)     4827 2023-02-28 00:21:17.000000 spafe-0.3.2/tests/test_features_bfcc.py
--rw-rw-r--   0 am        (1000) am        (1000)     3199 2023-02-28 00:21:17.000000 spafe-0.3.2/tests/test_features_cqcc.py
--rw-rw-r--   0 am        (1000) am        (1000)     4870 2023-02-28 00:21:17.000000 spafe-0.3.2/tests/test_features_gfcc.py
--rw-rw-r--   0 am        (1000) am        (1000)     4860 2023-02-28 00:21:17.000000 spafe-0.3.2/tests/test_features_lfcc.py
--rw-rw-r--   0 am        (1000) am        (1000)     2522 2023-02-28 00:21:17.000000 spafe-0.3.2/tests/test_features_lpcc.py
--rw-rw-r--   0 am        (1000) am        (1000)     9492 2023-02-28 00:21:17.000000 spafe-0.3.2/tests/test_features_mfcc.py
--rw-rw-r--   0 am        (1000) am        (1000)     4871 2023-02-28 00:21:17.000000 spafe-0.3.2/tests/test_features_msrcc.py
--rw-rw-r--   0 am        (1000) am        (1000)     4870 2023-02-28 00:21:17.000000 spafe-0.3.2/tests/test_features_ngcc.py
--rw-rw-r--   0 am        (1000) am        (1000)     4123 2023-02-28 00:21:17.000000 spafe-0.3.2/tests/test_features_pncc.py
--rw-rw-r--   0 am        (1000) am        (1000)     4871 2023-02-28 00:21:17.000000 spafe-0.3.2/tests/test_features_psrcc.py
--rw-rw-r--   0 am        (1000) am        (1000)     2868 2023-02-28 00:21:17.000000 spafe-0.3.2/tests/test_features_rplp.py
--rw-rw-r--   0 am        (1000) am        (1000)     1956 2023-02-28 00:21:17.000000 spafe-0.3.2/tests/test_frequencies.py
--rw-rw-r--   0 am        (1000) am        (1000)     2510 2023-02-28 00:21:17.000000 spafe-0.3.2/tests/test_utils_cepstral.py
--rw-rw-r--   0 am        (1000) am        (1000)     3040 2023-02-28 00:21:17.000000 spafe-0.3.2/tests/test_utils_converters.py
--rw-rw-r--   0 am        (1000) am        (1000)      405 2023-02-28 00:21:17.000000 spafe-0.3.2/tests/test_utils_filters.py
--rw-rw-r--   0 am        (1000) am        (1000)     2902 2023-02-28 00:21:17.000000 spafe-0.3.2/tests/test_utils_preprocessing.py
--rw-rw-r--   0 am        (1000) am        (1000)      416 2023-02-28 00:21:17.000000 spafe-0.3.2/tests/test_utils_spectral.py
--rw-rw-r--   0 am        (1000) am        (1000)     2205 2023-02-28 00:21:17.000000 spafe-0.3.2/tests/test_utils_vis.py
+drwxrwxr-x   0 am        (1000) am        (1000)        0 2024-05-30 18:07:21.309527 spafe-0.3.3/
+-rw-rw-r--   0 am        (1000) am        (1000)     1519 2024-05-30 13:19:50.000000 spafe-0.3.3/LICENSE
+-rw-r--r--   0 am        (1000) am        (1000)     8994 2024-05-30 18:07:21.309527 spafe-0.3.3/PKG-INFO
+-rw-rw-r--   0 am        (1000) am        (1000)     7238 2024-05-30 18:06:20.000000 spafe-0.3.3/README.md
+-rw-rw-r--   0 am        (1000) am        (1000)       38 2024-05-30 18:07:21.309527 spafe-0.3.3/setup.cfg
+-rw-rw-r--   0 am        (1000) am        (1000)     2031 2024-05-30 13:19:50.000000 spafe-0.3.3/setup.py
+drwxrwxr-x   0 am        (1000) am        (1000)        0 2024-05-30 18:07:21.301527 spafe-0.3.3/spafe/
+-rw-rw-r--   0 am        (1000) am        (1000)      291 2024-05-30 13:19:50.000000 spafe-0.3.3/spafe/__init__.py
+drwxrwxr-x   0 am        (1000) am        (1000)        0 2024-05-30 18:07:21.301527 spafe-0.3.3/spafe/fbanks/
+-rw-rw-r--   0 am        (1000) am        (1000)       54 2024-05-30 13:19:50.000000 spafe-0.3.3/spafe/fbanks/__init__.py
+-rw-rw-r--   0 am        (1000) am        (1000)     6230 2024-05-30 13:19:50.000000 spafe-0.3.3/spafe/fbanks/bark_fbanks.py
+-rw-rw-r--   0 am        (1000) am        (1000)     8461 2024-05-30 13:19:50.000000 spafe-0.3.3/spafe/fbanks/gammatone_fbanks.py
+-rw-rw-r--   0 am        (1000) am        (1000)     3659 2024-05-30 13:19:50.000000 spafe-0.3.3/spafe/fbanks/linear_fbanks.py
+-rw-rw-r--   0 am        (1000) am        (1000)    12751 2024-05-30 13:19:50.000000 spafe-0.3.3/spafe/fbanks/mel_fbanks.py
+drwxrwxr-x   0 am        (1000) am        (1000)        0 2024-05-30 18:07:21.305527 spafe-0.3.3/spafe/features/
+-rw-rw-r--   0 am        (1000) am        (1000)       54 2024-05-30 13:19:50.000000 spafe-0.3.3/spafe/features/__init__.py
+-rw-rw-r--   0 am        (1000) am        (1000)    12968 2024-05-30 13:19:50.000000 spafe-0.3.3/spafe/features/bfcc.py
+-rw-rw-r--   0 am        (1000) am        (1000)    11812 2024-05-30 13:19:50.000000 spafe-0.3.3/spafe/features/cqcc.py
+-rw-rw-r--   0 am        (1000) am        (1000)    12764 2024-05-30 13:19:50.000000 spafe-0.3.3/spafe/features/gfcc.py
+-rw-rw-r--   0 am        (1000) am        (1000)    11015 2024-05-30 13:19:50.000000 spafe-0.3.3/spafe/features/lfcc.py
+-rw-rw-r--   0 am        (1000) am        (1000)    12892 2024-05-30 13:19:54.000000 spafe-0.3.3/spafe/features/lpc.py
+-rw-rw-r--   0 am        (1000) am        (1000)    17759 2024-05-30 13:19:50.000000 spafe-0.3.3/spafe/features/mfcc.py
+-rw-rw-r--   0 am        (1000) am        (1000)     7128 2024-05-30 13:19:50.000000 spafe-0.3.3/spafe/features/msrcc.py
+-rw-rw-r--   0 am        (1000) am        (1000)     7477 2024-05-30 13:19:50.000000 spafe-0.3.3/spafe/features/ngcc.py
+-rw-rw-r--   0 am        (1000) am        (1000)    16250 2024-05-30 13:19:50.000000 spafe-0.3.3/spafe/features/pncc.py
+-rw-rw-r--   0 am        (1000) am        (1000)     7674 2024-05-30 13:19:50.000000 spafe-0.3.3/spafe/features/psrcc.py
+-rw-rw-r--   0 am        (1000) am        (1000)    15726 2024-05-30 13:19:50.000000 spafe-0.3.3/spafe/features/rplp.py
+-rw-rw-r--   0 am        (1000) am        (1000)    10948 2024-05-30 13:19:50.000000 spafe-0.3.3/spafe/features/spfeats.py
+drwxrwxr-x   0 am        (1000) am        (1000)        0 2024-05-30 18:07:21.305527 spafe-0.3.3/spafe/frequencies/
+-rw-rw-r--   0 am        (1000) am        (1000)       54 2024-05-30 13:19:50.000000 spafe-0.3.3/spafe/frequencies/__init__.py
+-rw-rw-r--   0 am        (1000) am        (1000)     6378 2024-05-30 13:19:50.000000 spafe-0.3.3/spafe/frequencies/dominant_frequencies.py
+-rw-rw-r--   0 am        (1000) am        (1000)    10511 2024-05-30 13:19:50.000000 spafe-0.3.3/spafe/frequencies/fundamental_frequencies.py
+drwxrwxr-x   0 am        (1000) am        (1000)        0 2024-05-30 18:07:21.305527 spafe-0.3.3/spafe/utils/
+-rw-rw-r--   0 am        (1000) am        (1000)       54 2024-05-30 13:19:50.000000 spafe-0.3.3/spafe/utils/__init__.py
+-rw-rw-r--   0 am        (1000) am        (1000)     4120 2024-05-30 13:19:50.000000 spafe-0.3.3/spafe/utils/cepstral.py
+-rw-rw-r--   0 am        (1000) am        (1000)    12810 2024-05-30 13:19:50.000000 spafe-0.3.3/spafe/utils/converters.py
+-rw-rw-r--   0 am        (1000) am        (1000)      988 2024-05-30 13:19:50.000000 spafe-0.3.3/spafe/utils/exceptions.py
+-rw-rw-r--   0 am        (1000) am        (1000)     2001 2024-05-30 13:19:50.000000 spafe-0.3.3/spafe/utils/filters.py
+-rw-rw-r--   0 am        (1000) am        (1000)     5388 2024-05-30 13:19:50.000000 spafe-0.3.3/spafe/utils/preprocessing.py
+-rw-rw-r--   0 am        (1000) am        (1000)     4951 2024-05-30 13:19:50.000000 spafe-0.3.3/spafe/utils/spectral.py
+-rw-rw-r--   0 am        (1000) am        (1000)     6025 2024-05-30 13:19:50.000000 spafe-0.3.3/spafe/utils/vis.py
+-rw-rw-r--   0 am        (1000) am        (1000)      256 2024-05-30 13:19:50.000000 spafe-0.3.3/spafe/version.py
+drwxrwxr-x   0 am        (1000) am        (1000)        0 2024-05-30 18:07:21.309527 spafe-0.3.3/spafe.egg-info/
+-rw-r--r--   0 am        (1000) am        (1000)     8994 2024-05-30 18:07:21.000000 spafe-0.3.3/spafe.egg-info/PKG-INFO
+-rw-rw-r--   0 am        (1000) am        (1000)     1645 2024-05-30 18:07:21.000000 spafe-0.3.3/spafe.egg-info/SOURCES.txt
+-rw-rw-r--   0 am        (1000) am        (1000)        1 2024-05-30 18:07:21.000000 spafe-0.3.3/spafe.egg-info/dependency_links.txt
+-rw-rw-r--   0 am        (1000) am        (1000)        1 2024-05-30 18:07:13.000000 spafe-0.3.3/spafe.egg-info/not-zip-safe
+-rw-rw-r--   0 am        (1000) am        (1000)      259 2024-05-30 18:07:21.000000 spafe-0.3.3/spafe.egg-info/requires.txt
+-rw-rw-r--   0 am        (1000) am        (1000)       12 2024-05-30 18:07:21.000000 spafe-0.3.3/spafe.egg-info/top_level.txt
+drwxrwxr-x   0 am        (1000) am        (1000)        0 2024-05-30 18:07:21.309527 spafe-0.3.3/tests/
+-rw-rw-r--   0 am        (1000) am        (1000)      162 2024-05-30 13:19:50.000000 spafe-0.3.3/tests/__init__.py
+-rw-rw-r--   0 am        (1000) am        (1000)      376 2024-05-30 13:19:50.000000 spafe-0.3.3/tests/conftest.py
+-rw-rw-r--   0 am        (1000) am        (1000)     1629 2024-05-30 13:19:50.000000 spafe-0.3.3/tests/test_fbanks_bark.py
+-rw-rw-r--   0 am        (1000) am        (1000)     1674 2024-05-30 13:19:50.000000 spafe-0.3.3/tests/test_fbanks_gamma.py
+-rw-rw-r--   0 am        (1000) am        (1000)     1642 2024-05-30 13:19:50.000000 spafe-0.3.3/tests/test_fbanks_lin.py
+-rw-rw-r--   0 am        (1000) am        (1000)     3147 2024-05-30 13:19:50.000000 spafe-0.3.3/tests/test_fbanks_mel.py
+-rw-rw-r--   0 am        (1000) am        (1000)     4827 2024-05-30 13:19:50.000000 spafe-0.3.3/tests/test_features_bfcc.py
+-rw-rw-r--   0 am        (1000) am        (1000)     3818 2024-05-30 13:19:50.000000 spafe-0.3.3/tests/test_features_cqcc.py
+-rw-rw-r--   0 am        (1000) am        (1000)     4870 2024-05-30 13:19:50.000000 spafe-0.3.3/tests/test_features_gfcc.py
+-rw-rw-r--   0 am        (1000) am        (1000)     4860 2024-05-30 13:19:50.000000 spafe-0.3.3/tests/test_features_lfcc.py
+-rw-rw-r--   0 am        (1000) am        (1000)     2522 2024-05-30 13:19:50.000000 spafe-0.3.3/tests/test_features_lpcc.py
+-rw-rw-r--   0 am        (1000) am        (1000)     9492 2024-05-30 13:19:50.000000 spafe-0.3.3/tests/test_features_mfcc.py
+-rw-rw-r--   0 am        (1000) am        (1000)     4871 2024-05-30 13:19:50.000000 spafe-0.3.3/tests/test_features_msrcc.py
+-rw-rw-r--   0 am        (1000) am        (1000)     4870 2024-05-30 13:19:50.000000 spafe-0.3.3/tests/test_features_ngcc.py
+-rw-rw-r--   0 am        (1000) am        (1000)     4123 2024-05-30 13:19:50.000000 spafe-0.3.3/tests/test_features_pncc.py
+-rw-rw-r--   0 am        (1000) am        (1000)     4871 2024-05-30 13:19:50.000000 spafe-0.3.3/tests/test_features_psrcc.py
+-rw-rw-r--   0 am        (1000) am        (1000)     2868 2024-05-30 13:19:50.000000 spafe-0.3.3/tests/test_features_rplp.py
+-rw-rw-r--   0 am        (1000) am        (1000)     1956 2024-05-30 13:19:50.000000 spafe-0.3.3/tests/test_frequencies.py
+-rw-rw-r--   0 am        (1000) am        (1000)     2510 2024-05-30 13:19:50.000000 spafe-0.3.3/tests/test_utils_cepstral.py
+-rw-rw-r--   0 am        (1000) am        (1000)     3040 2024-05-30 13:19:50.000000 spafe-0.3.3/tests/test_utils_converters.py
+-rw-rw-r--   0 am        (1000) am        (1000)      405 2024-05-30 13:19:50.000000 spafe-0.3.3/tests/test_utils_filters.py
+-rw-rw-r--   0 am        (1000) am        (1000)     2902 2024-05-30 13:19:50.000000 spafe-0.3.3/tests/test_utils_preprocessing.py
+-rw-rw-r--   0 am        (1000) am        (1000)      416 2024-05-30 13:19:50.000000 spafe-0.3.3/tests/test_utils_spectral.py
+-rw-rw-r--   0 am        (1000) am        (1000)     2205 2024-05-30 13:19:50.000000 spafe-0.3.3/tests/test_utils_vis.py
```

### Comparing `spafe-0.3.2/LICENSE` & `spafe-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spafe-0.3.2/PKG-INFO` & `spafe-0.3.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spafe
-Version: 0.3.2
+Version: 0.3.3
 Summary: Simplified Python Audio-Features Extraction.
 Home-page: https://github.com/SuperKogito/spafe
 Author: Ayoub Malek
 Author-email: superkogito@gmail.com
 Maintainer: Ayoub Malek
 Maintainer-email: superkogito@gmail.com
 License: BSD
@@ -18,18 +18,34 @@
 Classifier: Programming Language :: Python
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Classifier: Topic :: Multimedia :: Sound/Audio :: Editors
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy>=1.21
+Requires-Dist: scipy>=1.7.3
+Requires-Dist: typing_extensions
 Provides-Extra: tests
+Requires-Dist: pytest>=6.2.4; extra == "tests"
+Requires-Dist: pytest-cov; extra == "tests"
+Requires-Dist: codecov; extra == "tests"
+Requires-Dist: coveralls; extra == "tests"
+Requires-Dist: pytest-xdist; extra == "tests"
+Requires-Dist: codacy-coverage; extra == "tests"
+Requires-Dist: matplotlib; extra == "tests"
+Requires-Dist: mock==4.0.3; extra == "tests"
 Provides-Extra: docs
+Requires-Dist: sphinxcontrib-napoleon==0.7; extra == "docs"
+Requires-Dist: nbsphinx==0.8.9; extra == "docs"
+Requires-Dist: pydata-sphinx-theme==0.8.1; extra == "docs"
+Requires-Dist: matplotlib; extra == "docs"
 Provides-Extra: plotting
-License-File: LICENSE
+Requires-Dist: maplotlib; extra == "plotting"
 
 ![](https://github.com/SuperKogito/spafe/blob/master/media/logo.png?raw=true)
 
 # Spafe
 
 Simplified Python Audio Features Extraction
 
@@ -38,30 +54,36 @@
 [![License](https://img.shields.io/badge/license-BSD%203--Clause%20License%20(Revised)%20-blue)](https://github.com/SuperKogito/spafe/blob/master/LICENSE)
 [![Python](https://img.shields.io/badge/python-3.5%20%7C%203.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue)](https://www.python.org/doc/versions/)
 [![codecov](https://codecov.io/gh/SuperKogito/spafe/branch/master/graph/badge.svg)](https://codecov.io/gh/SuperKogito/spafe)
 [![codebeat badge](https://codebeat.co/badges/97f81ec3-b8a3-42ff-a9f5-f6cf165f4448)](https://codebeat.co/projects/github-com-superkogito-spafe-master)
 [![PyPI version](https://badge.fury.io/py/spafe.svg)](https://badge.fury.io/py/spafe)
 [![anaconda](https://anaconda.org/superkogito/spafe/badges/version.svg)](https://anaconda.org/SuperKogito/spafe)
 [![Downloads](https://pepy.tech/badge/spafe)](https://pepy.tech/project/spafe)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6824667.svg)](https://doi.org/10.5281/zenodo.6824667)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7686438.svg)](https://doi.org/10.5281/zenodo.7686438)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.04739/status.svg)](https://doi.org/10.21105/joss.04739)
 
 #  Table of Contents
 
-- [Structure](#Structure)
-  - [Filter banks](#Filter-banks)
-  - [Spectrograms](#Spectrograms)
-  - [Features](#Features)
-  - [Frequencies](#Frequencies)
-- [Installation](#Installation)
-  - [Dependencies](#Dependencies)
-  - [Installation guide](#Installation-guide)
-- [How to use](#How-to-use)
-- [Contributing](#Contributing)
-- [Citing](#Citing)
+- [Spafe](#spafe)
+- [Table of Contents](#table-of-contents)
+- [Structure](#structure)
+  - [Filter banks](#filter-banks)
+  - [Spectrograms](#spectrograms)
+  - [Features](#features)
+  - [Frequencies](#frequencies)
+  - [Installation](#installation)
+    - [Dependencies](#dependencies)
+    - [Installation guide](#installation-guide)
+      - [Install from PyPI](#install-from-pypi)
+      - [Install from Anaconda](#install-from-anaconda)
+    - [Install from source](#install-from-source)
+  - [Why use Spafe?](#why-use-spafe)
+  - [How to use](#how-to-use)
+  - [Contributing](#contributing)
+  - [Citing](#citing)
 
 # Structure
 spafe aims to simplify feature extractions from **mono audio** files.
 Spafe includes various computations related to filter banks, spectrograms, frequencies and cepstral features .
 The library has the following structure:
 ![](https://github.com/SuperKogito/spafe/raw/master/media/spafe-structure.png)
 
@@ -156,26 +178,27 @@
 Most existing libraries and to their credits provide great implementations for features extraction but are unfortunately limited to the Mel Frequency Features (MFCC) and at best have Bark frequency and linear predictive coefficients additionally. [Librosa](https://github.com/librosa/librosa) for example includes great implementation of various algorithms (only MFCC and LPC are included), based on the **Short Time Fourrier Transform (STFT)**, which is theoretically more accurate but slower than the **Discret Fourrier Transform used in Spafe**'s implementation.
 
 
 ## How to use
 
 Various examples on how to use spafe are present in the documentation [https://superkogito.github.io/spafe](https://superkogito.github.io/spafe).
 
-**<!>** Please make sure you are referring to the correct documentation version.
+> !Please make sure you are referring to the correct documentation version.
 
 ## Contributing
 
 Contributions are welcome and encouraged. To learn more about how to contribute to spafe please refer to the [Contributing guidelines](https://github.com/SuperKogito/spafe/blob/master/CONTRIBUTING.md)
 
 ## Citing
 
 -  **If you want to cite spafe as a software, please cite the version used as indexed in** [Zenodo](https://zenodo.org/):
 
-   *Ayoub Malek. (2023). SuperKogito/spafe: Spafe: Simplified python audio features extraction (v0.3.1). Zenodo.* https://doi.org/10.5281/zenodo.7533946
-
-   [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6824667.svg)](https://doi.org/10.5281/zenodo.6824667)
+   *Ayoub Malek, Hadrien Titeux, Stefano Borzì, Christian Heider Nielsen, Fabian-Robert Stöter, Hervé Bredin, Eryk Urbański & Kevin Mattheus Moerman. (2023). SuperKogito/spafe: v0.3.3 (v0.3.3). Zenodo.* https://doi.org/10.5281/zenodo.11396240
+  
+   [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.11396240.svg)](https://doi.org/10.5281/zenodo.11396240)
+ 
 
 - **You can also site spafe's paper as follows:**
 
   *Malek, A., (2023). Spafe: Simplified python audio features extraction. Journal of Open Source Software, 8(81), 4739,* https://doi.org/10.21105/joss.04739
 
   [![DOI](https://joss.theoj.org/papers/10.21105/joss.04739/status.svg)](https://doi.org/10.21105/joss.04739)
```

### Comparing `spafe-0.3.2/README.md` & `spafe-0.3.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,30 +9,36 @@
 [![License](https://img.shields.io/badge/license-BSD%203--Clause%20License%20(Revised)%20-blue)](https://github.com/SuperKogito/spafe/blob/master/LICENSE)
 [![Python](https://img.shields.io/badge/python-3.5%20%7C%203.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue)](https://www.python.org/doc/versions/)
 [![codecov](https://codecov.io/gh/SuperKogito/spafe/branch/master/graph/badge.svg)](https://codecov.io/gh/SuperKogito/spafe)
 [![codebeat badge](https://codebeat.co/badges/97f81ec3-b8a3-42ff-a9f5-f6cf165f4448)](https://codebeat.co/projects/github-com-superkogito-spafe-master)
 [![PyPI version](https://badge.fury.io/py/spafe.svg)](https://badge.fury.io/py/spafe)
 [![anaconda](https://anaconda.org/superkogito/spafe/badges/version.svg)](https://anaconda.org/SuperKogito/spafe)
 [![Downloads](https://pepy.tech/badge/spafe)](https://pepy.tech/project/spafe)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6824667.svg)](https://doi.org/10.5281/zenodo.6824667)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7686438.svg)](https://doi.org/10.5281/zenodo.7686438)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.04739/status.svg)](https://doi.org/10.21105/joss.04739)
 
 #  Table of Contents
 
-- [Structure](#Structure)
-  - [Filter banks](#Filter-banks)
-  - [Spectrograms](#Spectrograms)
-  - [Features](#Features)
-  - [Frequencies](#Frequencies)
-- [Installation](#Installation)
-  - [Dependencies](#Dependencies)
-  - [Installation guide](#Installation-guide)
-- [How to use](#How-to-use)
-- [Contributing](#Contributing)
-- [Citing](#Citing)
+- [Spafe](#spafe)
+- [Table of Contents](#table-of-contents)
+- [Structure](#structure)
+  - [Filter banks](#filter-banks)
+  - [Spectrograms](#spectrograms)
+  - [Features](#features)
+  - [Frequencies](#frequencies)
+  - [Installation](#installation)
+    - [Dependencies](#dependencies)
+    - [Installation guide](#installation-guide)
+      - [Install from PyPI](#install-from-pypi)
+      - [Install from Anaconda](#install-from-anaconda)
+    - [Install from source](#install-from-source)
+  - [Why use Spafe?](#why-use-spafe)
+  - [How to use](#how-to-use)
+  - [Contributing](#contributing)
+  - [Citing](#citing)
 
 # Structure
 spafe aims to simplify feature extractions from **mono audio** files.
 Spafe includes various computations related to filter banks, spectrograms, frequencies and cepstral features .
 The library has the following structure:
 ![](https://github.com/SuperKogito/spafe/raw/master/media/spafe-structure.png)
 
@@ -127,26 +133,27 @@
 Most existing libraries and to their credits provide great implementations for features extraction but are unfortunately limited to the Mel Frequency Features (MFCC) and at best have Bark frequency and linear predictive coefficients additionally. [Librosa](https://github.com/librosa/librosa) for example includes great implementation of various algorithms (only MFCC and LPC are included), based on the **Short Time Fourrier Transform (STFT)**, which is theoretically more accurate but slower than the **Discret Fourrier Transform used in Spafe**'s implementation.
 
 
 ## How to use
 
 Various examples on how to use spafe are present in the documentation [https://superkogito.github.io/spafe](https://superkogito.github.io/spafe).
 
-**<!>** Please make sure you are referring to the correct documentation version.
+> !Please make sure you are referring to the correct documentation version.
 
 ## Contributing
 
 Contributions are welcome and encouraged. To learn more about how to contribute to spafe please refer to the [Contributing guidelines](https://github.com/SuperKogito/spafe/blob/master/CONTRIBUTING.md)
 
 ## Citing
 
 -  **If you want to cite spafe as a software, please cite the version used as indexed in** [Zenodo](https://zenodo.org/):
 
-   *Ayoub Malek. (2023). SuperKogito/spafe: Spafe: Simplified python audio features extraction (v0.3.1). Zenodo.* https://doi.org/10.5281/zenodo.7533946
-
-   [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6824667.svg)](https://doi.org/10.5281/zenodo.6824667)
+   *Ayoub Malek, Hadrien Titeux, Stefano Borzì, Christian Heider Nielsen, Fabian-Robert Stöter, Hervé Bredin, Eryk Urbański & Kevin Mattheus Moerman. (2023). SuperKogito/spafe: v0.3.3 (v0.3.3). Zenodo.* https://doi.org/10.5281/zenodo.11396240
+  
+   [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.11396240.svg)](https://doi.org/10.5281/zenodo.11396240)
+ 
 
 - **You can also site spafe's paper as follows:**
 
   *Malek, A., (2023). Spafe: Simplified python audio features extraction. Journal of Open Source Software, 8(81), 4739,* https://doi.org/10.21105/joss.04739
 
   [![DOI](https://joss.theoj.org/papers/10.21105/joss.04739/status.svg)](https://doi.org/10.21105/joss.04739)
```

### Comparing `spafe-0.3.2/setup.py` & `spafe-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `spafe-0.3.2/spafe/fbanks/bark_fbanks.py` & `spafe-0.3.3/spafe/fbanks/bark_fbanks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 
 - Description : Bark filter banks implementation.
-- Copyright (c) 2019-2023 Ayoub Malek.
+- Copyright (c) 2019-2024 Ayoub Malek.
   This source code is licensed under the terms of the BSD 3-Clause License.
   For a copy, see <https://github.com/SuperKogito/spafe/blob/master/LICENSE>.
 
 """
+
 from typing import Optional
 
 import numpy as np
 
 from ..utils.converters import hz2bark, bark2hz, BarkConversionApproach
 from ..utils.exceptions import ParameterError, ErrorMsgs
 from ..utils.filters import scale_fbank, ScaleType
```

### Comparing `spafe-0.3.2/spafe/fbanks/gammatone_fbanks.py` & `spafe-0.3.3/spafe/fbanks/gammatone_fbanks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 
 - Description : Gammatone filter banks implementation.
-- Copyright (c) 2019-2023 Ayoub Malek.
+- Copyright (c) 2019-2024 Ayoub Malek.
   This source code is licensed under the terms of the BSD 3-Clause License.
   For a copy, see <https://github.com/SuperKogito/spafe/blob/master/LICENSE>.
 
 """
+
 from typing import Optional, Tuple
 
 import numpy as np
 
 from ..utils.converters import hz2erb, ErbConversionApproach
 from ..utils.exceptions import ParameterError, ErrorMsgs
 from ..utils.filters import scale_fbank, ScaleType
```

### Comparing `spafe-0.3.2/spafe/fbanks/linear_fbanks.py` & `spafe-0.3.3/spafe/fbanks/linear_fbanks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 
 - Description : Linear filter banks implementation.
-- Copyright (c) 2019-2023 Ayoub Malek.
+- Copyright (c) 2019-2024 Ayoub Malek.
   This source code is licensed under the terms of the BSD 3-Clause License.
   For a copy, see <https://github.com/SuperKogito/spafe/blob/master/LICENSE>.
 
 """
+
 from typing import Optional
 
 import numpy as np
 
 from .mel_fbanks import mel_filter_banks_helper
 from ..utils.filters import ScaleType
```

### Comparing `spafe-0.3.2/spafe/fbanks/mel_fbanks.py` & `spafe-0.3.3/spafe/fbanks/mel_fbanks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 
 - Description : Mel filter banks implementation.
-- Copyright (c) 2019-2023 Ayoub Malek.
+- Copyright (c) 2019-2024 Ayoub Malek.
   This source code is licensed under the terms of the BSD 3-Clause License.
   For a copy, see <https://github.com/SuperKogito/spafe/blob/master/LICENSE>.
 
 """
+
 from typing import Optional
 
 import numpy as np
 
 from ..utils.converters import hz2mel, mel2hz, MelConversionApproach
 from ..utils.exceptions import ParameterError, ErrorMsgs
 from ..utils.filters import scale_fbank, ScaleType
```

### Comparing `spafe-0.3.2/spafe/features/bfcc.py` & `spafe-0.3.3/spafe/features/bfcc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 
 - Description : Bark Frequency Cepstral Coefﬁcients (BFCCs) extraction algorithm implementation.
-- Copyright (c) 2019-2023 Ayoub Malek.
+- Copyright (c) 2019-2024 Ayoub Malek.
   This source code is licensed under the terms of the BSD 3-Clause License.
   For a copy, see <https://github.com/SuperKogito/spafe/blob/master/LICENSE>.
 
 """
+
 from typing import Optional
 
 import numpy as np
 from scipy.fftpack import dct
 
 from ..fbanks.bark_fbanks import bark_filter_banks
 from ..utils.cepstral import normalize_ceps, lifter_ceps, NormalizationType
```

### Comparing `spafe-0.3.2/spafe/features/cqcc.py` & `spafe-0.3.3/spafe/features/cqcc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 
 - Description : Constant Q-transform Cepstral Coeﬃcients (CQCCs) extraction algorithm implementation.
-- Copyright (c) 2019-2023 Ayoub Malek.
+- Copyright (c) 2019-2024 Ayoub Malek.
   This source code is licensed under the terms of the BSD 3-Clause License.
   For a copy, see <https://github.com/SuperKogito/spafe/blob/master/LICENSE>.
 
 """
+
 from typing import Optional
 
 import numpy as np
 from scipy.fftpack import dct
 from scipy.signal import resample
 
 from ..utils.cepstral import normalize_ceps, lifter_ceps, NormalizationType
@@ -162,15 +163,15 @@
     low_freq: float = 0,
     high_freq: Optional[float] = None,
     dct_type: int = 2,
     lifter: Optional[int] = None,
     normalize: Optional[NormalizationType] = None,
     number_of_octaves: int = 7,
     number_of_bins_per_octave: int = 24,
-    resampling_ratio: float = 0.95,
+    resampling_ratio: float = 1.0,
     spectral_threshold: float = 0.005,
     f0: float = 120,
     q_rate: float = 1.0,
 ):
     """
     Compute the Constant-Q Cepstral Coeﬃcients (CQCC features) from an audio signal
     as described in [Todisco]_.
@@ -204,24 +205,24 @@
         normalize                   (str) : normalization approach.
                                             (Default is None).
         number_of_octaves           (int) : number of occtaves.
                                             (Default is 7).
         number_of_bins_per_octave   (int) : numbers of bins oer occtave.
                                             (Default is 24).
         resampling_ratio          (float) : ratio to use for the uniform resampling.
-                                            (Default is 0.95).
+                                            (Default is 1.00).
         spectral_threshold        (float) : spectral threshold.
                                             (Default is 0.005).
         f0                        (float) : fundamental frequency.
                                             (Default is 28).
         q_rate                    (float) : number of FFT points.
                                             (Default is 1.0).
 
     Returns:
-        (numpy.ndarray) : 2d array of BFCC features (num_frames x num_ceps).
+        (numpy.ndarray) : 2d array of BFCC features (num_frames*resampling_ratio x num_ceps).
 
     Tip:
         - :code:`dct` : can take the following options [1, 2, 3, 4].
         - :code:`normalize` : can take the following options ["mvn", "ms", "vn", "mn"].
 
     References:
         .. [Todisco] : Todisco M., Héctor Delgado H., Evans N., Constant Q cepstral
@@ -279,15 +280,15 @@
 
     # |Xcq|**2
     power_spectrum = np.absolute(constant_qtransform) ** 2
 
     # -> log(.)
     # handle zeros: if feat is zero, we get problems with log
     features_no_zero = zero_handling(x=power_spectrum)
-    log_features = np.log(features_no_zero)
+    log_features = np.log(features_no_zero.T)
 
     # uniform resampling
     resampled_features = resample(
         log_features, int(len(log_features) * resampling_ratio)
     )
 
     #  -> DCT(.)
@@ -296,8 +297,9 @@
     # apply filter
     if lifter:
         cqccs = lifter_ceps(cqccs, lifter)
 
     # normalization
     if normalize:
         cqccs = normalize_ceps(cqccs, normalize)
+
     return cqccs
```

### Comparing `spafe-0.3.2/spafe/features/gfcc.py` & `spafe-0.3.3/spafe/features/gfcc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 
 - Description : Gammatone Frequency Cepstral Coefﬁcients (GFCCs) extraction algorithm implementation.
-- Copyright (c) 2019-2023 Ayoub Malek.
+- Copyright (c) 2019-2024 Ayoub Malek.
   This source code is licensed under the terms of the BSD 3-Clause License.
   For a copy, see <https://github.com/SuperKogito/spafe/blob/master/LICENSE>.
 
 """
+
 from typing import Optional, Tuple
 
 import numpy as np
 from scipy.fftpack import dct
 
 from ..fbanks.gammatone_fbanks import gammatone_filter_banks
 from ..utils.cepstral import normalize_ceps, lifter_ceps, NormalizationType
```

### Comparing `spafe-0.3.2/spafe/features/lfcc.py` & `spafe-0.3.3/spafe/features/lfcc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 
 - Description : Linear Frequency Cepstral Coefﬁcients (LFCCs) extraction algorithm implementation.
-- Copyright (c) 2019-2023 Ayoub Malek.
+- Copyright (c) 2019-2024 Ayoub Malek.
   This source code is licensed under the terms of the BSD 3-Clause License.
   For a copy, see <https://github.com/SuperKogito/spafe/blob/master/LICENSE>.
 
 """
+
 from typing import Optional
 
 import numpy as np
 from scipy.fftpack import dct
 
 from ..fbanks.linear_fbanks import linear_filter_banks
 from ..utils.cepstral import normalize_ceps, lifter_ceps, NormalizationType
```

### Comparing `spafe-0.3.2/spafe/features/lpc.py` & `spafe-0.3.3/spafe/features/lpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 
 - Description : Linear Prediction Components and Cepstral Coefﬁcients (LPCs and LPCCs) extraction algorithm implementation.
-- Copyright (c) 2019-2023 Ayoub Malek.
+- Copyright (c) 2019-2024 Ayoub Malek.
   This source code is licensed under the terms of the BSD 3-Clause License.
   For a copy, see <https://github.com/SuperKogito/spafe/blob/master/LICENSE>.
 
 """
+
 from typing import Optional
 
 import numpy as np
 from scipy import linalg
 
 from ..utils.cepstral import normalize_ceps, lifter_ceps, NormalizationType
 from ..utils.preprocessing import (
@@ -28,24 +29,21 @@
 
     Args:
         sig    (numpy.ndarray) : input mono audio signal (Nx1).
         order            (int) : Size of the cepstral components/ model order. If None is given,
                                  we use len(seq) as default, otherwise order+1.
                                  (Default is 13).
 
-    Returns:
-        - (numpy.ndarray) : linear prediction coefficents (lpc coefficents: a).
-        - (numpy.ndarray) : the error term is the square root of the squared prediction error (e**2).
-
     Note:
+
         The premis of linear predictive analysis is that the nth sample can be estimated by a
         linear combination of the previous p samples:
 
         .. math::
-            xp[n] = -a[1] * x[n-1] - ... -a[k] * x[n-k] ... - a[p] * x[n-p] = - \\sum_{k=1}^{p+1} a_{k} . x[n-k]
+            xp[n] = -a[1] * x[n-1] - ... -a[k] * x[n-k] - ... -a[p] * x[n-p] = - \\sum_{k=1}^{p+1} a_{k} . x[n-k]
 
         where xp is the predicted signal. a_{1},.., a_{p} are known as the predictor
         coefficents and p is called the model order and n is the sample index.
         Based on the previous equation, we can estimate the prediction error as follows [Ucl-brain]_:
 
         .. math::
             e[n] = x[n] - xp[n] \\implies  x[n] = e[n] - \\sum_{k=1}^{p+1} a_{k} . x[n-k]
@@ -54,34 +52,28 @@
         We can further rewrite the previous equations for all samples [Collomb]_:
 
         .. math::
             E = \\sum_{i=1}^{N} (x[i] - (-\\sum_{k=1}^{p+1} a_{k} . x[i-k])) \\text{for x\\in[1,p]}
 
 
         All the previous steps can be presented in a matrix, which is a toeplitz matrix: R.A = 0
-                           _          _
+                            _          _
             -r[1] = r[0]   r[1]   ... r[p-1]    a[1]
-             :      :      :          :         :
-             :      :      :          _      *  :
+                :      :      :          :         :
+                :      :      :          :   *     :
             -r[p] = r[p-1] r[p-2] ... r[0]      a[p]
 
         To solve this, one can use the Levinson-Durbin, which is a well-known
         algorithm to solve the Hermitian toeplitz with respect to a. Using the
         special symmetry in the matrix, the inversion can be done in O(p^2)
         instead of O(p^3).
 
-    References:
-        .. [Darconis] : Draconi, Replacing Levinson implementation in scikits.talkbox,
-                        Stackoverflow, https://stackoverflow.com/a/43457190/6939324
-        .. [Cournapeau] : David Cournapeau D. talkbox, https://github.com/cournape/talkbox
-        .. [Menares] : Menares E. F. M., ML-experiments, https://github.com/erickfmm/ML-experiments
-        .. [Collomb] : Collomb C. Linear Prediction and Levinson-Durbin Algorithm, 03.02.2009,
-                       <https://www.academia.edu/8479430/Linear_Prediction_and_Levinson-Durbin_Algorithm_Contents>
-        .. [Ucl-brain] : Ucl psychology and language sciences, Faculty of brain Sciences, Unit 8 linear prediction
-                         <https://www.phon.ucl.ac.uk/courses/spsci/dsp/lpc.html>
+    Returns:
+        - (numpy.ndarray) : linear prediction coefficents (lpc coefficents: a).
+        - (numpy.ndarray) : the error term is the square root of the squared prediction error (e**2).
     """
     p = order + 1
     r = np.zeros(p, frame.dtype)
 
     # Number of non zero values in autocorrelation one needs for p LPC coefficients
     nx = np.min([p, frame.size])
     auto_corr = np.correlate(frame, frame, "full")
@@ -103,33 +95,65 @@
 ):
     """
     Compute the Linear prediction coefficents (LPC) from an audio signal.
 
     Args:
         sig    (numpy.ndarray) : a mono audio signal (Nx1) from which to compute features.
         fs               (int) : the sampling frequency of the signal we are working with.
-                                 (Default is 16000).
+                                    (Default is 16000).
         order            (int) : order of the LP model and number of cepstral components.
-                                 (Default is 13).
+                                    (Default is 13).
         pre_emph        (bool) : apply pre-emphasis if 1.
-                                 (Default is 1).
+                                    (Default is 1).
         pre_emph_coeff (float) : pre-emphasis filter coefficient.
-                                 (Default is 0.97).
+                                    (Default is 0.97).
         window (SlidingWindow) : sliding window object.
-                                 (Default is None).
+                                    (Default is None).
 
     Returns:
         (tuple) :
             - (numpy.ndarray) : 2d array of LPC features (num_frames x num_ceps).
             - (numpy.ndarray) : The error term is the sqare root of the squared prediction error.
 
     Note:
         .. figure:: ../_static/architectures/lpcs.png
 
-           Architecture of linear prediction components extraction algorithm.
+            Architecture of linear prediction components extraction algorithm.
+
+
+        The premis of linear predictive analysis is that the nth sample can be estimated by a
+        linear combination of the previous p samples:
+
+        .. math::
+            xp[n] = -a[1] * x[n-1] - \dots - a[k] * x[n-k] - \dots - a[p] * x[n-p] = - \\sum_{k=1}^{p} a_{k} x[n-k]
+
+        where :math:`xp` is the predicted signal, :math:`a_{1}, \dots, a_{p}` are the predictor
+        coefficients, :math:`p` is the model order, and :math:`n` is the sample index.
+        Based on the previous equation, we can estimate the prediction error as follows [Ucl-brain]_:
+
+        .. math::
+            e[n] = x[n] - xp[n] \\implies x[n] = e[n] + \\sum_{k=1}^{p} a_{k} x[n-k]
+
+        The unknown here are the LP coefficients :math:`a`, hence we need to minimize e to find those.
+        We can further rewrite the previous equations for all samples [Collomb]_:
+
+        .. math::
+            E = \\sum_{i=1}^{N} \\left( x[i] - \\sum_{k=1}^{p} a_{k} x[i-k] \\right)^2
+
+        All the previous steps can be presented in a matrix, which is a Toeplitz matrix :math:`R.A = 0`
+
+    References:
+        .. [Darconis] : Draconi, Replacing Levinson implementation in scikits.talkbox,
+                        Stackoverflow, https://stackoverflow.com/a/43457190/6939324
+        .. [Cournapeau] : David Cournapeau D. talkbox, https://github.com/cournape/talkbox
+        .. [Menares] : Menares E. F. M., ML-experiments, https://github.com/erickfmm/ML-experiments
+        .. [Collomb] : Collomb C. Linear Prediction and Levinson-Durbin Algorithm, 03.02.2009,
+                        <https://www.academia.edu/8479430/Linear_Prediction_and_Levinson-Durbin_Algorithm_Contents>
+        .. [Ucl-brain] : Ucl psychology and language sciences, Faculty of brain Sciences, Unit 8 linear prediction
+                            <https://www.phon.ucl.ac.uk/courses/spsci/dsp/lpc.html>
 
     Examples
         .. plot::
 
             from scipy.io.wavfile import read
             from spafe.features.lpc import lpc
             from spafe.utils.preprocessing import SlidingWindow
@@ -137,18 +161,18 @@
 
             # read audio
             fpath = "../../../tests/data/test.wav"
             fs, sig = read(fpath)
 
             # compute lpcs
             lpcs, _ = lpc(sig,
-                          fs=fs,
-                          pre_emph=0,
-                          pre_emph_coeff=0.97,
-                          window=SlidingWindow(0.030, 0.015, "hamming"))
+                            fs=fs,
+                            pre_emph=0,
+                            pre_emph_coeff=0.97,
+                            window=SlidingWindow(0.030, 0.015, "hamming"))
 
             # visualize features
             show_features(lpcs, "Linear prediction coefficents", "LPCs Index", "Frame Index")
     """
     order = order - 1
     # pre-emphasis
     if pre_emph:
@@ -170,15 +194,15 @@
     e_vec = np.zeros((len(windows), 1))
 
     for i, windowed_frame in enumerate(frames):
         a, e = __lpc_helper(windowed_frame, order)
         a_mat[i, :] = a
         e_vec[i] = e
 
-    return np.array(a_mat), np.sqrt(e_vec)
+    return np.array(a_mat), np.array(e_vec)
 
 
 def lpc2lpcc(a, e, nceps):
     """
     Convert linear prediction coefficents (LPC) to linear prediction cepstral coefﬁcients (LPCC)
     as described in [Rao]_ and [Makhoul]_.
 
@@ -191,38 +215,35 @@
         (numpy.ndarray) : linear prediction cepstrum coefficents (LPCC).
 
     Note:
         .. math::
 
             C_{m}=\\left\\{\\begin{array}{l}
             log_{e}(p), & \\text{if } m = 0 \\\\
-            a_{m} + \\sum_{k=1}^{m-1} \\frac{k}{m} C_{m} a_{m-k} , & \\text{if } 1 < m < p \\\\
+            a_{m} + \\sum_{k=1}^{m-1} \\frac{k}{m} C_{m} a_{m-k} , & \\text{if } 1 <= m <= p \\\\
             \\sum_{k=m-p}^{m-1} \\frac{k}{m} C_{m} a_{m-k} , & \\text{if } m > p \\end{array}\\right.
 
     References:
         .. [Makhoul] : Makhoul, J. (1975). Linear prediction: A tutorial review.
                        Proceedings of the IEEE, 63(4), 561–580. doi:10.1109/proc.1975.9792
         .. [Rao] : Rao, K. S., Reddy, V. R., & Maity, S. (2015). 
                    Language Identification Using Spectral and Prosodic Features. 
                    SpringerBriefs in Electrical and Computer Engineering. doi:10.1007/978-3-319-17163-0
     """
     p = len(a)
-    c = [0 for i in range(nceps)]
+    c = [1] * nceps
 
     c[0] = np.log(zero_handling(e))
-    c[1:p] = [
-        a[m] + sum([(k / m) * c[k] * a[m - k] for k in range(1, m)])
-        for m in range(1, p)
-    ]
+
+    for m in range(1, p):
+        c[m] = a[m] + sum([(k / m) * c[m] * a[m - k] for k in range(1, m)])
 
     if nceps > p:
-        c[p:nceps] = [
-            sum([(k / m) * c[k] * a[m - k] for k in range(m - p, m)])
-            for m in range(p, nceps)
-        ]
+        for m in range(p + 1, nceps):
+            c[m] = sum([(k / m) * c[m] * a[m - k] for k in range(m - p, m)])
 
     return c
 
 
 def lpcc(
     sig: np.ndarray,
     fs: int = 16000,
```

### Comparing `spafe-0.3.2/spafe/features/mfcc.py` & `spafe-0.3.3/spafe/features/mfcc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 
 - Description : Mel and inverse Mel Features Cepstral Coefﬁcients (MFCCs and IMFCCs) extraction algorithm implementation.
-- Copyright (c) 2019-2023 Ayoub Malek.
+- Copyright (c) 2019-2024 Ayoub Malek.
   This source code is licensed under the terms of the BSD 3-Clause License.
   For a copy, see <https://github.com/SuperKogito/spafe/blob/master/LICENSE>.
 
 """
+
 from typing import Optional
 
 import numpy as np
 from scipy.fftpack import dct
 
 from ..fbanks.mel_fbanks import inverse_mel_filter_banks, mel_filter_banks
 from ..utils.cepstral import normalize_ceps, lifter_ceps, NormalizationType
```

### Comparing `spafe-0.3.2/spafe/features/msrcc.py` & `spafe-0.3.3/spafe/features/msrcc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 
 - Description : Magnitude based Spectral Root Cepstral Coefficients (MSRCCs) extraction algorithm implementation.
-- Copyright (c) 2019-2023 Ayoub Malek.
+- Copyright (c) 2019-2024 Ayoub Malek.
   This source code is licensed under the terms of the BSD 3-Clause License.
   For a copy, see <https://github.com/SuperKogito/spafe/blob/master/LICENSE>.
 
 """
+
 from typing import Optional
 
 import numpy as np
 from scipy.fftpack import dct
 
 from ..features.mfcc import mel_spectrogram
 from ..utils.cepstral import normalize_ceps, lifter_ceps, NormalizationType
```

### Comparing `spafe-0.3.2/spafe/features/ngcc.py` & `spafe-0.3.3/spafe/features/ngcc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 
 - Description : Normalized Gammachirp Cepstral Coefficients (NGCCs) extraction algorithm implementation.
-- Copyright (c) 2019-2023 Ayoub Malek.
+- Copyright (c) 2019-2024 Ayoub Malek.
   This source code is licensed under the terms of the BSD 3-Clause License.
   For a copy, see <https://github.com/SuperKogito/spafe/blob/master/LICENSE>.
 
 """
+
 from typing import Optional
 
 import numpy as np
 from scipy.fftpack import dct
 
 from ..fbanks.gammatone_fbanks import gammatone_filter_banks
 from ..utils.cepstral import normalize_ceps, lifter_ceps, NormalizationType
```

### Comparing `spafe-0.3.2/spafe/features/pncc.py` & `spafe-0.3.3/spafe/features/pncc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 
 - Description : Power-Normalized Cepstral Coefficients (PNCCs) extraction algorithm implementation.
-- Copyright (c) 2019-2023 Ayoub Malek.
+- Copyright (c) 2019-2024 Ayoub Malek.
   This source code is licensed under the terms of the BSD 3-Clause License.
   For a copy, see <https://github.com/SuperKogito/spafe/blob/master/LICENSE>.
 
 """
+
 from typing import Optional
 
 import numpy as np
 from scipy.fftpack import dct
 
 from ..fbanks.gammatone_fbanks import gammatone_filter_banks
 from ..utils.cepstral import normalize_ceps, lifter_ceps, NormalizationType
```

### Comparing `spafe-0.3.2/spafe/features/psrcc.py` & `spafe-0.3.3/spafe/features/psrcc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 
 - Description : Phase based Spectral Root Cepstral Coefficients (PSRCCs) extraction algorithm implementation.
-- Copyright (c) 2019-2023 Ayoub Malek.
+- Copyright (c) 2019-2024 Ayoub Malek.
   This source code is licensed under the terms of the BSD 3-Clause License.
   For a copy, see <https://github.com/SuperKogito/spafe/blob/master/LICENSE>.
 
 """
+
 from typing import Optional
 
 import numpy as np
 from scipy.fftpack import dct
 
 from ..fbanks.mel_fbanks import mel_filter_banks
 from ..utils.cepstral import normalize_ceps, lifter_ceps
```

### Comparing `spafe-0.3.2/spafe/features/rplp.py` & `spafe-0.3.3/spafe/features/rplp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 
 - Description : (Rasta) Perceptual linear prediction coefficents (RPLPs/PLPs) extraction algorithm implementation.
-- Copyright (c) 2019-2023 Ayoub Malek.
+- Copyright (c) 2019-2024 Ayoub Malek.
   This source code is licensed under the terms of the BSD 3-Clause License.
   For a copy, see <https://github.com/SuperKogito/spafe/blob/master/LICENSE>.
 
 """
+
 from typing import Optional
 
 import numpy as np
 
 from ..fbanks.bark_fbanks import bark_filter_banks
 from ..features.lpc import __lpc_helper, lpc2lpcc
 from ..utils.cepstral import normalize_ceps, lifter_ceps, NormalizationType
@@ -144,17 +145,15 @@
         ras_nl_aspectrum = rasta_filter(nl_aspectrum)
 
         # do inverse log
         auditory_spectrum = np.exp(ras_nl_aspectrum)
 
     # equal loudness pre_emphasis
     E = lambda w: ((w**2 + 56.8 * 10**6) * w**4) / (
-        (w**2 + 6.3 * 10**6)
-        * (w**2 + 0.38 * 10**9)
-        * (w**6 + 9.58 * 10**26)
+        (w**2 + 6.3 * 10**6) * (w**2 + 0.38 * 10**9) * (w**6 + 9.58 * 10**26)
     )
     Y = [E(w) for w in auditory_spectrum]
 
     # intensity loudness compression
     L = np.abs(Y) ** (1 / 3)
 
     # ifft
```

### Comparing `spafe-0.3.2/spafe/features/spfeats.py` & `spafe-0.3.3/spafe/features/spfeats.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 
 - Description : Spectral and frequency stats and features extraction algorithms implementation.
-- Copyright (c) 2019-2023 Ayoub Malek.
+- Copyright (c) 2019-2024 Ayoub Malek.
   This source code is licensed under the terms of the BSD 3-Clause License.
   For a copy, see <https://github.com/SuperKogito/spafe/blob/master/LICENSE>.
 
 """
 
 import numpy as np
 from scipy import stats
```

### Comparing `spafe-0.3.2/spafe/frequencies/dominant_frequencies.py` & `spafe-0.3.3/spafe/frequencies/dominant_frequencies.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 
 - Description : Implementation Dominant Frequency Extraction Using the YIN-Algorithm.
-- Copyright (c) 2019-2023 Ayoub Malek.
+- Copyright (c) 2019-2024 Ayoub Malek.
   This source code is licensed under the terms of the BSD 3-Clause License.
   For a copy, see <https://github.com/SuperKogito/spafe/blob/master/LICENSE>.
 
 """
 import numpy as np
 from scipy import signal
```

### Comparing `spafe-0.3.2/spafe/frequencies/fundamental_frequencies.py` & `spafe-0.3.3/spafe/frequencies/fundamental_frequencies.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 
 - Description : Implementation Fundamental Frequency Extraction Using the YIN-Algorithm.
-- Copyright (c) 2019-2023 Ayoub Malek.
+- Copyright (c) 2019-2024 Ayoub Malek.
   This source code is licensed under the terms of the BSD 3-Clause License.
   For a copy, see <https://github.com/SuperKogito/spafe/blob/master/LICENSE>.
 
 """
 from typing import Tuple
 
 import numpy as np
```

### Comparing `spafe-0.3.2/spafe/utils/cepstral.py` & `spafe-0.3.3/spafe/utils/cepstral.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 
 - Description : Power-Normalized Cepstral Coefficients (PNCCs) extraction algorithm implementation.
-- Copyright (c) 2019-2023 Ayoub Malek.
+- Copyright (c) 2019-2024 Ayoub Malek.
   This source code is licensed under the terms of the BSD 3-Clause License.
   For a copy, see <https://github.com/SuperKogito/spafe/blob/master/LICENSE>.
 
 """
+
 import numpy as np
 from scipy.signal import lfilter
 from typing_extensions import Literal
 
 NormalizationType = Literal["mvn", "ms", "vn", "mn"]
```

### Comparing `spafe-0.3.2/spafe/utils/converters.py` & `spafe-0.3.3/spafe/utils/converters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 
 - Description : Frequency converters implementation.
-- Copyright (c) 2019-2023 Ayoub Malek.
+- Copyright (c) 2019-2024 Ayoub Malek.
   This source code is licensed under the terms of the BSD 3-Clause License.
   For a copy, see <https://github.com/SuperKogito/spafe/blob/master/LICENSE>.
 
 """
+
 import numpy as np
 from typing_extensions import Literal
 
 # init vars
 F0 = 0
 FSP = 200 / 3
 BARK_FREQ = 1000
```

### Comparing `spafe-0.3.2/spafe/utils/exceptions.py` & `spafe-0.3.3/spafe/utils/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 
 - Description : Exception classes for Spafe implementation.
-- Copyright (c) 2019-2023 Ayoub Malek.
+- Copyright (c) 2019-2024 Ayoub Malek.
   This source code is licensed under the terms of the BSD 3-Clause License.
   For a copy, see <https://github.com/SuperKogito/spafe/blob/master/LICENSE>.
 
 """
 
 ErrorMsgs = {
     "low_freq": "minimal frequency cannot be less than zero.",
```

### Comparing `spafe-0.3.2/spafe/utils/filters.py` & `spafe-0.3.3/spafe/utils/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 
 - Description : Filter utils implementation.
-- Copyright (c) 2019-2023 Ayoub Malek.
+- Copyright (c) 2019-2024 Ayoub Malek.
   This source code is licensed under the terms of the BSD 3-Clause License.
   For a copy, see <https://github.com/SuperKogito/spafe/blob/master/LICENSE>.
 
 """
+
 import numpy as np
 from scipy import signal
 from typing_extensions import Literal
 
 ScaleType = Literal["ascendant", "descendant", "constant"]
```

### Comparing `spafe-0.3.2/spafe/utils/preprocessing.py` & `spafe-0.3.3/spafe/utils/preprocessing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """
 
 - Description : Preprocessing utils implementation.
-- Copyright (c) 2019-2023 Ayoub Malek.
+- Copyright (c) 2019-2024 Ayoub Malek.
   This source code is licensed under the terms of the BSD 3-Clause License.
   For a copy, see <https://github.com/SuperKogito/spafe/blob/master/LICENSE>.
 
 """
+
 from typing import Tuple
 
 import numpy as np
+from scipy.signal import lfilter
 from dataclasses import dataclass
 from typing_extensions import Literal
 
 from .exceptions import ParameterError, ErrorMsgs
 
 WindowType = Literal["hanning", "bartlet", "kaiser", "blackman", "hamming"]
 
@@ -63,15 +65,15 @@
         (numpy.ndarray) : pre-empahsised signal.
 
     Note:
         .. math::
 
             y[t] = x[t] - \\alpha \\times x[t-1]
     """
-    return np.append(sig[0], sig[1:] - pre_emph_coeff * sig[:-1])
+    return lfilter([1, -pre_emph_coeff], [1], sig)
 
 
 def stride_trick(a: np.ndarray, stride_length: int, stride_step: int) -> np.ndarray:
     """
     apply framing using the stride trick from numpy.
 
     Args:
```

### Comparing `spafe-0.3.2/spafe/utils/spectral.py` & `spafe-0.3.3/spafe/utils/spectral.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 
 - Description : Spectral utils implementation.
-- Copyright (c) 2019-2023 Ayoub Malek.
+- Copyright (c) 2019-2024 Ayoub Malek.
   This source code is licensed under the terms of the BSD 3-Clause License.
   For a copy, see <https://github.com/SuperKogito/spafe/blob/master/LICENSE>.
 
 """
+
 from typing import List
 
 import numpy as np
 from scipy.sparse import csr_matrix
 
 from .preprocessing import WindowType
 from ..utils.preprocessing import windowing
```

### Comparing `spafe-0.3.2/spafe/utils/vis.py` & `spafe-0.3.3/spafe/utils/vis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 
 - Description : Visualization implementation.
-- Copyright (c) 2019-2023 Ayoub Malek.
+- Copyright (c) 2019-2024 Ayoub Malek.
   This source code is licensed under the terms of the BSD 3-Clause License.
   For a copy, see <https://github.com/SuperKogito/spafe/blob/master/LICENSE>.
 
 """
+
 import numpy as np
 
 from spafe.utils.converters import hz2mel, hz2bark, hz2erb
 
 
 def tick_function(X, fb_type):
     """
```

### Comparing `spafe-0.3.2/spafe.egg-info/PKG-INFO` & `spafe-0.3.3/spafe.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spafe
-Version: 0.3.2
+Version: 0.3.3
 Summary: Simplified Python Audio-Features Extraction.
 Home-page: https://github.com/SuperKogito/spafe
 Author: Ayoub Malek
 Author-email: superkogito@gmail.com
 Maintainer: Ayoub Malek
 Maintainer-email: superkogito@gmail.com
 License: BSD
@@ -18,18 +18,34 @@
 Classifier: Programming Language :: Python
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Classifier: Topic :: Multimedia :: Sound/Audio :: Editors
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy>=1.21
+Requires-Dist: scipy>=1.7.3
+Requires-Dist: typing_extensions
 Provides-Extra: tests
+Requires-Dist: pytest>=6.2.4; extra == "tests"
+Requires-Dist: pytest-cov; extra == "tests"
+Requires-Dist: codecov; extra == "tests"
+Requires-Dist: coveralls; extra == "tests"
+Requires-Dist: pytest-xdist; extra == "tests"
+Requires-Dist: codacy-coverage; extra == "tests"
+Requires-Dist: matplotlib; extra == "tests"
+Requires-Dist: mock==4.0.3; extra == "tests"
 Provides-Extra: docs
+Requires-Dist: sphinxcontrib-napoleon==0.7; extra == "docs"
+Requires-Dist: nbsphinx==0.8.9; extra == "docs"
+Requires-Dist: pydata-sphinx-theme==0.8.1; extra == "docs"
+Requires-Dist: matplotlib; extra == "docs"
 Provides-Extra: plotting
-License-File: LICENSE
+Requires-Dist: maplotlib; extra == "plotting"
 
 ![](https://github.com/SuperKogito/spafe/blob/master/media/logo.png?raw=true)
 
 # Spafe
 
 Simplified Python Audio Features Extraction
 
@@ -38,30 +54,36 @@
 [![License](https://img.shields.io/badge/license-BSD%203--Clause%20License%20(Revised)%20-blue)](https://github.com/SuperKogito/spafe/blob/master/LICENSE)
 [![Python](https://img.shields.io/badge/python-3.5%20%7C%203.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue)](https://www.python.org/doc/versions/)
 [![codecov](https://codecov.io/gh/SuperKogito/spafe/branch/master/graph/badge.svg)](https://codecov.io/gh/SuperKogito/spafe)
 [![codebeat badge](https://codebeat.co/badges/97f81ec3-b8a3-42ff-a9f5-f6cf165f4448)](https://codebeat.co/projects/github-com-superkogito-spafe-master)
 [![PyPI version](https://badge.fury.io/py/spafe.svg)](https://badge.fury.io/py/spafe)
 [![anaconda](https://anaconda.org/superkogito/spafe/badges/version.svg)](https://anaconda.org/SuperKogito/spafe)
 [![Downloads](https://pepy.tech/badge/spafe)](https://pepy.tech/project/spafe)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6824667.svg)](https://doi.org/10.5281/zenodo.6824667)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7686438.svg)](https://doi.org/10.5281/zenodo.7686438)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.04739/status.svg)](https://doi.org/10.21105/joss.04739)
 
 #  Table of Contents
 
-- [Structure](#Structure)
-  - [Filter banks](#Filter-banks)
-  - [Spectrograms](#Spectrograms)
-  - [Features](#Features)
-  - [Frequencies](#Frequencies)
-- [Installation](#Installation)
-  - [Dependencies](#Dependencies)
-  - [Installation guide](#Installation-guide)
-- [How to use](#How-to-use)
-- [Contributing](#Contributing)
-- [Citing](#Citing)
+- [Spafe](#spafe)
+- [Table of Contents](#table-of-contents)
+- [Structure](#structure)
+  - [Filter banks](#filter-banks)
+  - [Spectrograms](#spectrograms)
+  - [Features](#features)
+  - [Frequencies](#frequencies)
+  - [Installation](#installation)
+    - [Dependencies](#dependencies)
+    - [Installation guide](#installation-guide)
+      - [Install from PyPI](#install-from-pypi)
+      - [Install from Anaconda](#install-from-anaconda)
+    - [Install from source](#install-from-source)
+  - [Why use Spafe?](#why-use-spafe)
+  - [How to use](#how-to-use)
+  - [Contributing](#contributing)
+  - [Citing](#citing)
 
 # Structure
 spafe aims to simplify feature extractions from **mono audio** files.
 Spafe includes various computations related to filter banks, spectrograms, frequencies and cepstral features .
 The library has the following structure:
 ![](https://github.com/SuperKogito/spafe/raw/master/media/spafe-structure.png)
 
@@ -156,26 +178,27 @@
 Most existing libraries and to their credits provide great implementations for features extraction but are unfortunately limited to the Mel Frequency Features (MFCC) and at best have Bark frequency and linear predictive coefficients additionally. [Librosa](https://github.com/librosa/librosa) for example includes great implementation of various algorithms (only MFCC and LPC are included), based on the **Short Time Fourrier Transform (STFT)**, which is theoretically more accurate but slower than the **Discret Fourrier Transform used in Spafe**'s implementation.
 
 
 ## How to use
 
 Various examples on how to use spafe are present in the documentation [https://superkogito.github.io/spafe](https://superkogito.github.io/spafe).
 
-**<!>** Please make sure you are referring to the correct documentation version.
+> !Please make sure you are referring to the correct documentation version.
 
 ## Contributing
 
 Contributions are welcome and encouraged. To learn more about how to contribute to spafe please refer to the [Contributing guidelines](https://github.com/SuperKogito/spafe/blob/master/CONTRIBUTING.md)
 
 ## Citing
 
 -  **If you want to cite spafe as a software, please cite the version used as indexed in** [Zenodo](https://zenodo.org/):
 
-   *Ayoub Malek. (2023). SuperKogito/spafe: Spafe: Simplified python audio features extraction (v0.3.1). Zenodo.* https://doi.org/10.5281/zenodo.7533946
-
-   [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6824667.svg)](https://doi.org/10.5281/zenodo.6824667)
+   *Ayoub Malek, Hadrien Titeux, Stefano Borzì, Christian Heider Nielsen, Fabian-Robert Stöter, Hervé Bredin, Eryk Urbański & Kevin Mattheus Moerman. (2023). SuperKogito/spafe: v0.3.3 (v0.3.3). Zenodo.* https://doi.org/10.5281/zenodo.11396240
+  
+   [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.11396240.svg)](https://doi.org/10.5281/zenodo.11396240)
+ 
 
 - **You can also site spafe's paper as follows:**
 
   *Malek, A., (2023). Spafe: Simplified python audio features extraction. Journal of Open Source Software, 8(81), 4739,* https://doi.org/10.21105/joss.04739
 
   [![DOI](https://joss.theoj.org/papers/10.21105/joss.04739/status.svg)](https://doi.org/10.21105/joss.04739)
```

### Comparing `spafe-0.3.2/spafe.egg-info/SOURCES.txt` & `spafe-0.3.3/spafe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spafe-0.3.2/tests/test_fbanks_bark.py` & `spafe-0.3.3/tests/test_fbanks_bark.py`

 * *Files identical despite different names*

### Comparing `spafe-0.3.2/tests/test_fbanks_gamma.py` & `spafe-0.3.3/tests/test_fbanks_gamma.py`

 * *Files identical despite different names*

### Comparing `spafe-0.3.2/tests/test_fbanks_lin.py` & `spafe-0.3.3/tests/test_fbanks_lin.py`

 * *Files identical despite different names*

### Comparing `spafe-0.3.2/tests/test_fbanks_mel.py` & `spafe-0.3.3/tests/test_fbanks_mel.py`

 * *Files identical despite different names*

### Comparing `spafe-0.3.2/tests/test_features_bfcc.py` & `spafe-0.3.3/tests/test_features_bfcc.py`

 * *Files identical despite different names*

### Comparing `spafe-0.3.2/tests/test_features_cqcc.py` & `spafe-0.3.3/tests/test_features_cqcc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pytest
 import numpy as np
 import scipy.io.wavfile
 from spafe.utils import vis
 from spafe.features.cqcc import cqcc
+from spafe.utils.preprocessing import framing
 from spafe.utils.exceptions import ParameterError
 from spafe.utils.cepstral import normalize_ceps, lifter_ceps
 
 
 @pytest.mark.test_id(202)
 @pytest.mark.usefixtures("sig")
 @pytest.mark.usefixtures("fs")
@@ -14,66 +15,77 @@
 @pytest.mark.parametrize("pre_emph", [False, True])
 @pytest.mark.parametrize("nfft", [1024])
 @pytest.mark.parametrize("low_freq", [50])
 @pytest.mark.parametrize("high_freq", [4000])
 @pytest.mark.parametrize("dct_type", [1, 2, 4])
 @pytest.mark.parametrize("lifter", [None, 0.7, -7])
 @pytest.mark.parametrize("normalize", [None, "mvn", "ms"])
+@pytest.mark.parametrize("resampling_ratio", [1.0, 0.9, 0.3])
 def test_cqcc(
     sig,
     fs,
     num_ceps,
     pre_emph,
     nfft,
     low_freq,
     high_freq,
     dct_type,
     lifter,
     normalize,
+    resampling_ratio,
 ):
     """
     test cqcc features module for the following:
         - check if ParameterErrors are raised for:
                 - nfilts < num_ceps
                 - negative low_freq value
                 - high_freq > fs / 2
         - check that the returned number of cepstrums is correct.
         - check normalization.
         - check liftering.
     """
+    # get number of frames
+    frames, frame_length = framing(sig=sig, fs=fs, win_len=0.025, win_hop=0.01)
+    num_frames = len(frames)
 
     # check error for number of filters is smaller than number of cepstrums
     with pytest.raises(ParameterError):
         cqccs = cqcc(
             sig=sig,
             fs=fs,
             num_ceps=num_ceps,
             nfft=nfft,
             low_freq=low_freq,
             high_freq=fs,
+            resampling_ratio=resampling_ratio,
         )
 
     # compute features
     cqccs = cqcc(
         sig=sig,
         fs=fs,
         num_ceps=num_ceps,
         pre_emph=pre_emph,
         nfft=nfft,
         low_freq=low_freq,
         high_freq=high_freq,
         dct_type=dct_type,
         lifter=lifter,
         normalize=normalize,
+        resampling_ratio=resampling_ratio,
     )
 
     # assert number of returned cepstrum coefficients
     if not cqccs.shape[1] == num_ceps:
         raise AssertionError
 
+    # assert number of returned cepstrum coefficients
+    if not cqccs.shape[0] == int(num_frames * resampling_ratio):
+        raise AssertionError
+
     # check normalize
     if normalize:
         np.testing.assert_array_almost_equal(
             cqccs,
             normalize_ceps(
                 cqcc(
                     sig=sig,
@@ -82,14 +94,15 @@
                     pre_emph=pre_emph,
                     nfft=nfft,
                     low_freq=low_freq,
                     high_freq=high_freq,
                     dct_type=dct_type,
                     lifter=lifter,
                     normalize=None,
+                    resampling_ratio=resampling_ratio,
                 ),
                 normalize,
             ),
             3,
         )
     else:
         # check lifter
@@ -104,12 +117,13 @@
                         pre_emph=pre_emph,
                         nfft=nfft,
                         low_freq=low_freq,
                         high_freq=high_freq,
                         dct_type=dct_type,
                         lifter=None,
                         normalize=normalize,
+                        resampling_ratio=resampling_ratio,
                     ),
                     lifter,
                 ),
                 3,
             )
```

### Comparing `spafe-0.3.2/tests/test_features_gfcc.py` & `spafe-0.3.3/tests/test_features_gfcc.py`

 * *Files identical despite different names*

### Comparing `spafe-0.3.2/tests/test_features_lfcc.py` & `spafe-0.3.3/tests/test_features_lfcc.py`

 * *Files identical despite different names*

### Comparing `spafe-0.3.2/tests/test_features_lpcc.py` & `spafe-0.3.3/tests/test_features_lpcc.py`

 * *Files identical despite different names*

### Comparing `spafe-0.3.2/tests/test_features_mfcc.py` & `spafe-0.3.3/tests/test_features_mfcc.py`

 * *Files identical despite different names*

### Comparing `spafe-0.3.2/tests/test_features_msrcc.py` & `spafe-0.3.3/tests/test_features_msrcc.py`

 * *Files identical despite different names*

### Comparing `spafe-0.3.2/tests/test_features_ngcc.py` & `spafe-0.3.3/tests/test_features_ngcc.py`

 * *Files identical despite different names*

### Comparing `spafe-0.3.2/tests/test_features_pncc.py` & `spafe-0.3.3/tests/test_features_pncc.py`

 * *Files identical despite different names*

### Comparing `spafe-0.3.2/tests/test_features_psrcc.py` & `spafe-0.3.3/tests/test_features_psrcc.py`

 * *Files identical despite different names*

### Comparing `spafe-0.3.2/tests/test_features_rplp.py` & `spafe-0.3.3/tests/test_features_rplp.py`

 * *Files identical despite different names*

### Comparing `spafe-0.3.2/tests/test_frequencies.py` & `spafe-0.3.3/tests/test_frequencies.py`

 * *Files identical despite different names*

### Comparing `spafe-0.3.2/tests/test_utils_cepstral.py` & `spafe-0.3.3/tests/test_utils_cepstral.py`

 * *Files identical despite different names*

### Comparing `spafe-0.3.2/tests/test_utils_converters.py` & `spafe-0.3.3/tests/test_utils_converters.py`

 * *Files identical despite different names*

### Comparing `spafe-0.3.2/tests/test_utils_preprocessing.py` & `spafe-0.3.3/tests/test_utils_preprocessing.py`

 * *Files identical despite different names*

### Comparing `spafe-0.3.2/tests/test_utils_vis.py` & `spafe-0.3.3/tests/test_utils_vis.py`

 * *Files identical despite different names*

