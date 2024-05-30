# Comparing `tmp/voyger-0.4.tar.gz` & `tmp/voyger-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voyger-0.4.tar", last modified: Thu May 30 18:47:07 2024, max compression
+gzip compressed data, was "voyger-0.7.tar", last modified: Thu May 30 18:59:03 2024, max compression
```

## Comparing `voyger-0.4.tar` & `voyger-0.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 18:47:07.831904 voyger-0.4/
--rw-rw-rw-   0        0        0      170 2024-05-30 18:47:07.829870 voyger-0.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-30 18:47:07.831904 voyger-0.4/setup.cfg
--rw-rw-rw-   0        0        0      327 2024-05-30 18:41:02.000000 voyger-0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-30 18:47:07.823337 voyger-0.4/voyger.egg-info/
--rw-rw-rw-   0        0        0      170 2024-05-30 18:47:07.000000 voyger-0.4/voyger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      138 2024-05-30 18:47:07.000000 voyger-0.4/voyger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 18:47:07.000000 voyger-0.4/voyger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-30 18:47:07.000000 voyger-0.4/voyger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      645 2024-05-30 18:25:49.000000 voyger-0.4/voyger.py
+drwxrwxrwx   0        0        0        0 2024-05-30 18:59:03.909486 voyger-0.7/
+-rw-rw-rw-   0        0        0      170 2024-05-30 18:59:03.905945 voyger-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-30 18:59:03.910569 voyger-0.7/setup.cfg
+-rw-rw-rw-   0        0        0      327 2024-05-30 18:58:28.000000 voyger-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 18:59:03.903949 voyger-0.7/voyger.egg-info/
+-rw-rw-rw-   0        0        0      170 2024-05-30 18:59:03.000000 voyger-0.7/voyger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      138 2024-05-30 18:59:03.000000 voyger-0.7/voyger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 18:59:03.000000 voyger-0.7/voyger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-30 18:59:03.000000 voyger-0.7/voyger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2564 2024-05-30 18:58:09.000000 voyger-0.7/voyger.py
```

