# Comparing `tmp/myfunctions_SashaKrav-0.0.10.tar.gz` & `tmp/myfunctions_SashaKrav-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/SashaKrav/Python-class/class5/dist/tmpawn51ngz/myfunctions_SashaKrav-0.0.10.tar", last modified: Thu May 30 01:14:14 2024, max compression
+gzip compressed data, was "/mnt/SashaKrav/Python-class/class5/dist/tmpt5w4b34m/myfunctions_SashaKrav-0.0.11.tar", last modified: Thu May 30 01:19:12 2024, max compression
```

## Comparing `myfunctions_SashaKrav-0.0.10.tar` & `myfunctions_SashaKrav-0.0.11.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 SashaKrav  (1628) SashaKrav  (1629)        0 2024-05-30 01:14:14.000000 myfunctions_SashaKrav-0.0.10/
--rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)      631 2024-05-30 01:13:53.000000 myfunctions_SashaKrav-0.0.10/setup.py
-drwxrwxr-x   0 SashaKrav  (1628) SashaKrav  (1629)        0 2024-05-30 01:14:14.000000 myfunctions_SashaKrav-0.0.10/myfunctions_SashaKrav.egg-info/
--rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)        1 2024-05-30 01:14:14.000000 myfunctions_SashaKrav-0.0.10/myfunctions_SashaKrav.egg-info/top_level.txt
--rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)      198 2024-05-30 01:14:14.000000 myfunctions_SashaKrav-0.0.10/myfunctions_SashaKrav.egg-info/SOURCES.txt
--rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)        1 2024-05-30 01:14:14.000000 myfunctions_SashaKrav-0.0.10/myfunctions_SashaKrav.egg-info/dependency_links.txt
--rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)      447 2024-05-30 01:14:14.000000 myfunctions_SashaKrav-0.0.10/myfunctions_SashaKrav.egg-info/PKG-INFO
--rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)        0 2024-05-30 00:48:28.000000 myfunctions_SashaKrav-0.0.10/README.md
--rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)      447 2024-05-30 01:14:14.000000 myfunctions_SashaKrav-0.0.10/PKG-INFO
--rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)       38 2024-05-30 01:14:14.000000 myfunctions_SashaKrav-0.0.10/setup.cfg
+drwxrwxr-x   0 SashaKrav  (1628) SashaKrav  (1629)        0 2024-05-30 01:19:12.000000 myfunctions_SashaKrav-0.0.11/
+-rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)      631 2024-05-30 01:18:51.000000 myfunctions_SashaKrav-0.0.11/setup.py
+drwxrwxr-x   0 SashaKrav  (1628) SashaKrav  (1629)        0 2024-05-30 01:19:12.000000 myfunctions_SashaKrav-0.0.11/myfunctions_SashaKrav.egg-info/
+-rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)        1 2024-05-30 01:19:12.000000 myfunctions_SashaKrav-0.0.11/myfunctions_SashaKrav.egg-info/top_level.txt
+-rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)      198 2024-05-30 01:19:12.000000 myfunctions_SashaKrav-0.0.11/myfunctions_SashaKrav.egg-info/SOURCES.txt
+-rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)        1 2024-05-30 01:19:12.000000 myfunctions_SashaKrav-0.0.11/myfunctions_SashaKrav.egg-info/dependency_links.txt
+-rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)     2243 2024-05-30 01:19:12.000000 myfunctions_SashaKrav-0.0.11/myfunctions_SashaKrav.egg-info/PKG-INFO
+-rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)     1803 2024-05-30 01:18:40.000000 myfunctions_SashaKrav-0.0.11/README.md
+-rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)     2243 2024-05-30 01:19:12.000000 myfunctions_SashaKrav-0.0.11/PKG-INFO
+-rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)       38 2024-05-30 01:19:12.000000 myfunctions_SashaKrav-0.0.11/setup.cfg
```

