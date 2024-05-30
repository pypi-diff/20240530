# Comparing `tmp/connect_four_tobiasocula-1.0.tar.gz` & `tmp/connect_four_tobiasocula-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connect_four_tobiasocula-1.0.tar", last modified: Tue May 28 15:40:44 2024, max compression
+gzip compressed data, was "connect_four_tobiasocula-1.0.1.tar", last modified: Thu May 30 10:27:44 2024, max compression
```

## Comparing `connect_four_tobiasocula-1.0.tar` & `connect_four_tobiasocula-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 15:40:44.806148 connect_four_tobiasocula-1.0/
--rw-rw-rw-   0        0        0       69 2024-05-28 15:40:44.803941 connect_four_tobiasocula-1.0/PKG-INFO
--rw-rw-rw-   0        0        0       37 2024-05-28 15:09:21.000000 connect_four_tobiasocula-1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 15:40:44.755945 connect_four_tobiasocula-1.0/connect_four_tobiasocula/
--rw-rw-rw-   0        0        0       44 2024-05-28 15:11:28.000000 connect_four_tobiasocula-1.0/connect_four_tobiasocula/__init__.py
--rw-rw-rw-   0        0        0       29 2024-05-28 15:10:37.000000 connect_four_tobiasocula-1.0/connect_four_tobiasocula/main.py
-drwxrwxrwx   0        0        0        0 2024-05-28 15:40:44.801195 connect_four_tobiasocula-1.0/connect_four_tobiasocula.egg-info/
--rw-rw-rw-   0        0        0       69 2024-05-28 15:40:44.000000 connect_four_tobiasocula-1.0/connect_four_tobiasocula.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2024-05-28 15:40:44.000000 connect_four_tobiasocula-1.0/connect_four_tobiasocula.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 15:40:44.000000 connect_four_tobiasocula-1.0/connect_four_tobiasocula.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-05-28 15:40:44.000000 connect_four_tobiasocula-1.0/connect_four_tobiasocula.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 15:40:44.806148 connect_four_tobiasocula-1.0/setup.cfg
--rw-rw-rw-   0        0        0      166 2024-05-28 15:40:21.000000 connect_four_tobiasocula-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 10:27:44.652440 connect_four_tobiasocula-1.0.1/
+-rw-rw-rw-   0        0        0      188 2024-05-30 10:27:44.650441 connect_four_tobiasocula-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       37 2024-05-28 15:09:21.000000 connect_four_tobiasocula-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 10:27:44.609778 connect_four_tobiasocula-1.0.1/connect_four_tobiasocula/
+-rw-rw-rw-   0        0        0       29 2024-05-28 15:44:20.000000 connect_four_tobiasocula-1.0.1/connect_four_tobiasocula/__init__.py
+-rw-rw-rw-   0        0        0       44 2024-05-28 15:44:24.000000 connect_four_tobiasocula-1.0.1/connect_four_tobiasocula/main.py
+drwxrwxrwx   0        0        0        0 2024-05-30 10:27:44.647444 connect_four_tobiasocula-1.0.1/connect_four_tobiasocula.egg-info/
+-rw-rw-rw-   0        0        0      188 2024-05-30 10:27:44.000000 connect_four_tobiasocula-1.0.1/connect_four_tobiasocula.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2024-05-30 10:27:44.000000 connect_four_tobiasocula-1.0.1/connect_four_tobiasocula.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 10:27:44.000000 connect_four_tobiasocula-1.0.1/connect_four_tobiasocula.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-30 10:27:44.000000 connect_four_tobiasocula-1.0.1/connect_four_tobiasocula.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 10:27:44.653440 connect_four_tobiasocula-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      353 2024-05-30 10:25:57.000000 connect_four_tobiasocula-1.0.1/setup.py
```

