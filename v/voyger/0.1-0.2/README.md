# Comparing `tmp/voyger-0.1.tar.gz` & `tmp/voyger-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voyger-0.1.tar", last modified: Thu May 30 14:22:09 2024, max compression
+gzip compressed data, was "voyger-0.2.tar", last modified: Thu May 30 15:00:35 2024, max compression
```

## Comparing `voyger-0.1.tar` & `voyger-0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 14:22:09.302175 voyger-0.1/
--rw-rw-rw-   0        0        0      170 2024-05-30 14:22:09.292963 voyger-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-30 14:22:09.302954 voyger-0.1/setup.cfg
--rw-rw-rw-   0        0        0      301 2024-05-30 14:21:20.000000 voyger-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:22:09.292963 voyger-0.1/voyger.egg-info/
--rw-rw-rw-   0        0        0      170 2024-05-30 14:22:08.000000 voyger-0.1/voyger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      138 2024-05-30 14:22:09.000000 voyger-0.1/voyger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 14:22:08.000000 voyger-0.1/voyger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-30 14:22:08.000000 voyger-0.1/voyger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      278 2024-05-30 14:11:55.000000 voyger-0.1/voyger.py
+drwxrwxrwx   0        0        0        0 2024-05-30 15:00:35.754701 voyger-0.2/
+-rw-rw-rw-   0        0        0      170 2024-05-30 15:00:35.750385 voyger-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-30 15:00:35.754701 voyger-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      327 2024-05-30 14:43:30.000000 voyger-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 15:00:35.748384 voyger-0.2/voyger.egg-info/
+-rw-rw-rw-   0        0        0      170 2024-05-30 15:00:35.000000 voyger-0.2/voyger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      138 2024-05-30 15:00:35.000000 voyger-0.2/voyger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 15:00:35.000000 voyger-0.2/voyger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-30 15:00:35.000000 voyger-0.2/voyger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      565 2024-05-30 14:59:34.000000 voyger-0.2/voyger.py
```

