# Comparing `tmp/connect_four_tobiasocula-1.0.2.tar.gz` & `tmp/connect_four_tobiasocula-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connect_four_tobiasocula-1.0.2.tar", last modified: Thu May 30 10:36:30 2024, max compression
+gzip compressed data, was "connect_four_tobiasocula-1.0.3.tar", last modified: Thu May 30 10:40:06 2024, max compression
```

## Comparing `connect_four_tobiasocula-1.0.2.tar` & `connect_four_tobiasocula-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 10:36:30.038809 connect_four_tobiasocula-1.0.2/
--rw-rw-rw-   0        0        0      188 2024-05-30 10:36:30.036050 connect_four_tobiasocula-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       37 2024-05-28 15:09:21.000000 connect_four_tobiasocula-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 10:36:29.987631 connect_four_tobiasocula-1.0.2/connect_four_tobiasocula/
--rw-rw-rw-   0        0        0       22 2024-05-30 10:36:18.000000 connect_four_tobiasocula-1.0.2/connect_four_tobiasocula/__init__.py
--rw-rw-rw-   0        0        0       44 2024-05-30 10:29:51.000000 connect_four_tobiasocula-1.0.2/connect_four_tobiasocula/main.py
-drwxrwxrwx   0        0        0        0 2024-05-30 10:36:30.033723 connect_four_tobiasocula-1.0.2/connect_four_tobiasocula.egg-info/
--rw-rw-rw-   0        0        0      188 2024-05-30 10:36:29.000000 connect_four_tobiasocula-1.0.2/connect_four_tobiasocula.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2024-05-30 10:36:29.000000 connect_four_tobiasocula-1.0.2/connect_four_tobiasocula.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 10:36:29.000000 connect_four_tobiasocula-1.0.2/connect_four_tobiasocula.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-05-30 10:36:29.000000 connect_four_tobiasocula-1.0.2/connect_four_tobiasocula.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 10:36:30.038809 connect_four_tobiasocula-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      353 2024-05-30 10:34:12.000000 connect_four_tobiasocula-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 10:40:06.814154 connect_four_tobiasocula-1.0.3/
+-rw-rw-rw-   0        0        0      188 2024-05-30 10:40:06.812141 connect_four_tobiasocula-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       37 2024-05-28 15:09:21.000000 connect_four_tobiasocula-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 10:40:06.777411 connect_four_tobiasocula-1.0.3/connect_four_tobiasocula/
+-rw-rw-rw-   0        0        0       22 2024-05-30 10:36:18.000000 connect_four_tobiasocula-1.0.3/connect_four_tobiasocula/__init__.py
+-rw-rw-rw-   0        0        0     2858 2024-05-30 10:39:13.000000 connect_four_tobiasocula-1.0.3/connect_four_tobiasocula/main.py
+drwxrwxrwx   0        0        0        0 2024-05-30 10:40:06.809146 connect_four_tobiasocula-1.0.3/connect_four_tobiasocula.egg-info/
+-rw-rw-rw-   0        0        0      188 2024-05-30 10:40:06.000000 connect_four_tobiasocula-1.0.3/connect_four_tobiasocula.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2024-05-30 10:40:06.000000 connect_four_tobiasocula-1.0.3/connect_four_tobiasocula.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 10:40:06.000000 connect_four_tobiasocula-1.0.3/connect_four_tobiasocula.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-30 10:40:06.000000 connect_four_tobiasocula-1.0.3/connect_four_tobiasocula.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 10:40:06.815165 connect_four_tobiasocula-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      353 2024-05-30 10:39:34.000000 connect_four_tobiasocula-1.0.3/setup.py
```

