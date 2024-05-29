# Comparing `tmp/mktdata-0.0.2.tar.gz` & `tmp/mktdata-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mktdata-0.0.2.tar", last modified: Wed May 22 01:55:16 2024, max compression
+gzip compressed data, was "mktdata-0.0.3.tar", last modified: Wed May 29 23:18:01 2024, max compression
```

## Comparing `mktdata-0.0.2.tar` & `mktdata-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 01:55:16.286080 mktdata-0.0.2/
--rw-rw-rw-   0        0        0       54 2024-05-22 01:55:16.285081 mktdata-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-22 01:55:16.284080 mktdata-0.0.2/mktdata.egg-info/
--rw-rw-rw-   0        0        0       54 2024-05-22 01:55:16.000000 mktdata-0.0.2/mktdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      181 2024-05-22 01:55:16.000000 mktdata-0.0.2/mktdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 01:55:16.000000 mktdata-0.0.2/mktdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     4028 2024-05-22 01:55:16.000000 mktdata-0.0.2/mktdata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-22 01:55:16.000000 mktdata-0.0.2/mktdata.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-22 01:55:16.285081 mktdata-0.0.2/models/
--rw-rw-rw-   0        0        0        0 2024-05-18 03:54:40.000000 mktdata-0.0.2/models/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-22 01:55:16.286080 mktdata-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      375 2024-05-22 01:55:12.000000 mktdata-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 23:18:01.180329 mktdata-0.0.3/
+-rw-rw-rw-   0        0        0     7618 2024-05-29 23:18:01.179328 mktdata-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-29 23:18:01.138842 mktdata-0.0.3/embeddings/
+-rw-rw-rw-   0        0        0        0 2024-05-25 03:59:58.000000 mktdata-0.0.3/embeddings/__init__.py
+-rw-rw-rw-   0        0        0     8061 2024-05-29 21:36:23.000000 mktdata-0.0.3/embeddings/technical_embeds.py
+drwxrwxrwx   0        0        0        0 2024-05-29 23:18:01.156016 mktdata-0.0.3/feeds/
+-rw-rw-rw-   0        0        0        0 2024-05-26 03:57:33.000000 mktdata-0.0.3/feeds/__init__.py
+-rw-rw-rw-   0        0        0        8 2024-05-26 04:43:41.000000 mktdata-0.0.3/feeds/helpers.py
+-rw-rw-rw-   0        0        0    10011 2024-05-28 04:01:01.000000 mktdata-0.0.3/feeds/option_data.py
+-rw-rw-rw-   0        0        0     3474 2024-05-28 04:15:01.000000 mktdata-0.0.3/feeds/starter.py
+-rw-rw-rw-   0        0        0     6630 2024-05-29 13:22:09.000000 mktdata-0.0.3/feeds/stock_data.py
+-rw-rw-rw-   0        0        0    32551 2024-05-29 21:32:05.000000 mktdata-0.0.3/feeds/technicals.py
+drwxrwxrwx   0        0        0        0 2024-05-29 23:18:01.171130 mktdata-0.0.3/mktdata.egg-info/
+-rw-rw-rw-   0        0        0     7618 2024-05-29 23:18:00.000000 mktdata-0.0.3/mktdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2024-05-29 23:18:01.000000 mktdata-0.0.3/mktdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 23:18:00.000000 mktdata-0.0.3/mktdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     4028 2024-05-29 23:18:00.000000 mktdata-0.0.3/mktdata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-29 23:18:00.000000 mktdata-0.0.3/mktdata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 23:18:01.171130 mktdata-0.0.3/models/
+-rw-rw-rw-   0        0        0        0 2024-05-18 03:54:40.000000 mktdata-0.0.3/models/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-29 23:18:01.180329 mktdata-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      375 2024-05-29 23:17:48.000000 mktdata-0.0.3/setup.py
```

### Comparing `mktdata-0.0.2/mktdata.egg-info/requires.txt` & `mktdata-0.0.3/mktdata.egg-info/requires.txt`

 * *Files identical despite different names*

