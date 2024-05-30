# Comparing `tmp/deepsights-api-1.0.2.tar.gz` & `tmp/deepsights-api-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepsights-api-1.0.2.tar", last modified: Fri May 17 08:27:39 2024, max compression
+gzip compressed data, was "deepsights-api-1.0.3.tar", last modified: Thu May 30 09:54:11 2024, max compression
```

## Comparing `deepsights-api-1.0.2.tar` & `deepsights-api-1.0.3.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-17 08:27:39.662975 deepsights-api-1.0.2/
--rw-r--r--   0 0x1af      (501) staff       (20)    11356 2024-03-12 21:03:07.000000 deepsights-api-1.0.2/LICENSE
--rw-r--r--   0 0x1af      (501) staff       (20)     4754 2024-05-17 08:27:39.662765 deepsights-api-1.0.2/PKG-INFO
--rw-r--r--   0 0x1af      (501) staff       (20)     3839 2024-03-26 10:34:35.000000 deepsights-api-1.0.2/README.md
-drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-17 08:27:39.655139 deepsights-api-1.0.2/deepsights/
--rw-r--r--   0 0x1af      (501) staff       (20)      851 2024-03-25 16:53:44.000000 deepsights-api-1.0.2/deepsights/__init__.py
-drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-17 08:27:39.655601 deepsights-api-1.0.2/deepsights/api/
--rw-r--r--   0 0x1af      (501) staff       (20)      786 2024-03-25 15:56:22.000000 deepsights-api-1.0.2/deepsights/api/__init__.py
--rw-r--r--   0 0x1af      (501) staff       (20)     7798 2024-03-25 17:49:54.000000 deepsights-api-1.0.2/deepsights/api/api.py
--rw-r--r--   0 0x1af      (501) staff       (20)     1161 2024-03-24 07:09:55.000000 deepsights-api-1.0.2/deepsights/api/resource.py
-drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-17 08:27:39.655880 deepsights-api-1.0.2/deepsights/contentstore/
--rw-r--r--   0 0x1af      (501) staff       (20)      741 2024-03-24 07:36:24.000000 deepsights-api-1.0.2/deepsights/contentstore/__init__.py
--rw-r--r--   0 0x1af      (501) staff       (20)     1672 2024-03-25 17:23:37.000000 deepsights-api-1.0.2/deepsights/contentstore/contentstore.py
-drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-17 08:27:39.656712 deepsights-api-1.0.2/deepsights/contentstore/resources/
--rw-r--r--   0 0x1af      (501) staff       (20)      851 2024-03-25 17:24:10.000000 deepsights-api-1.0.2/deepsights/contentstore/resources/__init__.py
--rw-r--r--   0 0x1af      (501) staff       (20)     2374 2024-05-17 08:07:26.000000 deepsights-api-1.0.2/deepsights/contentstore/resources/_model.py
--rw-r--r--   0 0x1af      (501) staff       (20)     8358 2024-05-17 08:14:49.000000 deepsights-api-1.0.2/deepsights/contentstore/resources/_search.py
--rw-r--r--   0 0x1af      (501) staff       (20)     6684 2024-05-17 08:00:42.000000 deepsights-api-1.0.2/deepsights/contentstore/resources/news.py
--rw-r--r--   0 0x1af      (501) staff       (20)     6740 2024-05-17 08:16:59.000000 deepsights-api-1.0.2/deepsights/contentstore/resources/secondary.py
-drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-17 08:27:39.657130 deepsights-api-1.0.2/deepsights/deepsights/
--rw-r--r--   0 0x1af      (501) staff       (20)      735 2024-03-25 16:48:54.000000 deepsights-api-1.0.2/deepsights/deepsights/__init__.py
--rw-r--r--   0 0x1af      (501) staff       (20)     2861 2024-03-25 17:30:36.000000 deepsights-api-1.0.2/deepsights/deepsights/_mip_identity.py
--rw-r--r--   0 0x1af      (501) staff       (20)     3327 2024-03-25 17:51:00.000000 deepsights-api-1.0.2/deepsights/deepsights/deepsights.py
-drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-17 08:27:39.657247 deepsights-api-1.0.2/deepsights/deepsights/resources/
--rw-r--r--   0 0x1af      (501) staff       (20)      766 2024-03-25 16:48:34.000000 deepsights-api-1.0.2/deepsights/deepsights/resources/__init__.py
-drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-17 08:27:39.657595 deepsights-api-1.0.2/deepsights/deepsights/resources/quota/
--rw-r--r--   0 0x1af      (501) staff       (20)      847 2024-03-25 16:44:48.000000 deepsights-api-1.0.2/deepsights/deepsights/resources/quota/__init__.py
--rw-r--r--   0 0x1af      (501) staff       (20)     3311 2024-03-12 21:03:07.000000 deepsights-api-1.0.2/deepsights/deepsights/resources/quota/_model.py
--rw-r--r--   0 0x1af      (501) staff       (20)     1893 2024-03-25 16:44:57.000000 deepsights-api-1.0.2/deepsights/deepsights/resources/quota/quota.py
-drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-17 08:27:39.657863 deepsights-api-1.0.2/deepsights/documentstore/
--rw-r--r--   0 0x1af      (501) staff       (20)      847 2024-03-25 17:24:56.000000 deepsights-api-1.0.2/deepsights/documentstore/__init__.py
--rw-r--r--   0 0x1af      (501) staff       (20)     1607 2024-03-25 17:25:25.000000 deepsights-api-1.0.2/deepsights/documentstore/documentstore.py
-drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-17 08:27:39.657989 deepsights-api-1.0.2/deepsights/documentstore/resources/
--rw-r--r--   0 0x1af      (501) staff       (20)      828 2024-03-25 17:25:49.000000 deepsights-api-1.0.2/deepsights/documentstore/resources/__init__.py
-drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-17 08:27:39.659621 deepsights-api-1.0.2/deepsights/documentstore/resources/documents/
--rw-r--r--   0 0x1af      (501) staff       (20)      880 2024-03-25 16:42:51.000000 deepsights-api-1.0.2/deepsights/documentstore/resources/documents/__init__.py
--rw-r--r--   0 0x1af      (501) staff       (20)     1232 2024-03-24 08:05:24.000000 deepsights-api-1.0.2/deepsights/documentstore/resources/documents/_cache.py
--rw-r--r--   0 0x1af      (501) staff       (20)     2841 2024-03-25 16:42:51.000000 deepsights-api-1.0.2/deepsights/documentstore/resources/documents/_delete.py
--rw-r--r--   0 0x1af      (501) staff       (20)     2510 2024-03-25 16:42:51.000000 deepsights-api-1.0.2/deepsights/documentstore/resources/documents/_download.py
--rw-r--r--   0 0x1af      (501) staff       (20)     3269 2024-03-25 16:42:51.000000 deepsights-api-1.0.2/deepsights/documentstore/resources/documents/_list.py
--rw-r--r--   0 0x1af      (501) staff       (20)     5406 2024-03-25 16:42:51.000000 deepsights-api-1.0.2/deepsights/documentstore/resources/documents/_load.py
--rw-r--r--   0 0x1af      (501) staff       (20)     5582 2024-03-25 16:42:51.000000 deepsights-api-1.0.2/deepsights/documentstore/resources/documents/_model.py
--rw-r--r--   0 0x1af      (501) staff       (20)     6823 2024-03-25 16:42:51.000000 deepsights-api-1.0.2/deepsights/documentstore/resources/documents/_search.py
--rw-r--r--   0 0x1af      (501) staff       (20)     3378 2024-03-12 21:03:07.000000 deepsights-api-1.0.2/deepsights/documentstore/resources/documents/_segmenter.py
--rw-r--r--   0 0x1af      (501) staff       (20)     4560 2024-03-25 16:42:51.000000 deepsights-api-1.0.2/deepsights/documentstore/resources/documents/_upload.py
--rw-r--r--   0 0x1af      (501) staff       (20)     1923 2024-03-25 16:42:51.000000 deepsights-api-1.0.2/deepsights/documentstore/resources/documents/documents.py
-drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-17 08:27:39.659882 deepsights-api-1.0.2/deepsights/userclient/
--rw-r--r--   0 0x1af      (501) staff       (20)      756 2024-03-25 17:33:09.000000 deepsights-api-1.0.2/deepsights/userclient/__init__.py
-drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-17 08:27:39.660107 deepsights-api-1.0.2/deepsights/userclient/minions/
--rw-r--r--   0 0x1af      (501) staff       (20)        0 2024-03-12 21:03:07.000000 deepsights-api-1.0.2/deepsights/userclient/minions/__init__.py
--rw-r--r--   0 0x1af      (501) staff       (20)     1900 2024-03-24 08:06:13.000000 deepsights-api-1.0.2/deepsights/userclient/minions/_minions.py
-drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-17 08:27:39.660234 deepsights-api-1.0.2/deepsights/userclient/resources/
--rw-r--r--   0 0x1af      (501) staff       (20)      833 2024-03-25 17:32:47.000000 deepsights-api-1.0.2/deepsights/userclient/resources/__init__.py
-drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-17 08:27:39.660609 deepsights-api-1.0.2/deepsights/userclient/resources/answers/
--rw-r--r--   0 0x1af      (501) staff       (20)      774 2024-03-25 17:31:44.000000 deepsights-api-1.0.2/deepsights/userclient/resources/answers/__init__.py
--rw-r--r--   0 0x1af      (501) staff       (20)     4057 2024-03-25 18:15:10.000000 deepsights-api-1.0.2/deepsights/userclient/resources/answers/_model.py
--rw-r--r--   0 0x1af      (501) staff       (20)     4365 2024-03-25 18:12:47.000000 deepsights-api-1.0.2/deepsights/userclient/resources/answers/answer.py
-drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-17 08:27:39.661057 deepsights-api-1.0.2/deepsights/userclient/resources/reports/
--rw-r--r--   0 0x1af      (501) staff       (20)      775 2024-03-25 17:33:28.000000 deepsights-api-1.0.2/deepsights/userclient/resources/reports/__init__.py
--rw-r--r--   0 0x1af      (501) staff       (20)     5004 2024-03-25 18:22:13.000000 deepsights-api-1.0.2/deepsights/userclient/resources/reports/_model.py
--rw-r--r--   0 0x1af      (501) staff       (20)     4739 2024-03-26 10:43:01.000000 deepsights-api-1.0.2/deepsights/userclient/resources/reports/report.py
--rw-r--r--   0 0x1af      (501) staff       (20)     1547 2024-03-25 17:32:59.000000 deepsights-api-1.0.2/deepsights/userclient/userclient.py
-drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-17 08:27:39.661750 deepsights-api-1.0.2/deepsights/utils/
--rw-r--r--   0 0x1af      (501) staff       (20)     1062 2024-03-12 21:03:07.000000 deepsights-api-1.0.2/deepsights/utils/__init__.py
--rw-r--r--   0 0x1af      (501) staff       (20)     1995 2024-03-12 21:03:07.000000 deepsights-api-1.0.2/deepsights/utils/_cache.py
--rw-r--r--   0 0x1af      (501) staff       (20)     5901 2024-03-23 10:16:37.000000 deepsights-api-1.0.2/deepsights/utils/_ranking.py
--rw-r--r--   0 0x1af      (501) staff       (20)     1543 2024-03-12 21:03:07.000000 deepsights-api-1.0.2/deepsights/utils/_utils.py
--rw-r--r--   0 0x1af      (501) staff       (20)     2750 2024-03-12 21:03:07.000000 deepsights-api-1.0.2/deepsights/utils/model.py
-drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-17 08:27:39.662495 deepsights-api-1.0.2/deepsights_api.egg-info/
--rw-r--r--   0 0x1af      (501) staff       (20)     4754 2024-05-17 08:27:39.000000 deepsights-api-1.0.2/deepsights_api.egg-info/PKG-INFO
--rw-r--r--   0 0x1af      (501) staff       (20)     2296 2024-05-17 08:27:39.000000 deepsights-api-1.0.2/deepsights_api.egg-info/SOURCES.txt
--rw-r--r--   0 0x1af      (501) staff       (20)        1 2024-05-17 08:27:39.000000 deepsights-api-1.0.2/deepsights_api.egg-info/dependency_links.txt
--rw-r--r--   0 0x1af      (501) staff       (20)      117 2024-05-17 08:27:39.000000 deepsights-api-1.0.2/deepsights_api.egg-info/requires.txt
--rw-r--r--   0 0x1af      (501) staff       (20)       11 2024-05-17 08:27:39.000000 deepsights-api-1.0.2/deepsights_api.egg-info/top_level.txt
--rw-r--r--   0 0x1af      (501) staff       (20)       38 2024-05-17 08:27:39.663012 deepsights-api-1.0.2/setup.cfg
--rw-r--r--   0 0x1af      (501) staff       (20)     2023 2024-05-17 08:18:00.000000 deepsights-api-1.0.2/setup.py
+drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-30 09:54:11.339858 deepsights-api-1.0.3/
+-rw-r--r--   0 0x1af      (501) staff       (20)    11356 2024-03-12 21:03:07.000000 deepsights-api-1.0.3/LICENSE
+-rw-r--r--   0 0x1af      (501) staff       (20)     4754 2024-05-30 09:54:11.339631 deepsights-api-1.0.3/PKG-INFO
+-rw-r--r--   0 0x1af      (501) staff       (20)     3839 2024-03-26 10:34:35.000000 deepsights-api-1.0.3/README.md
+drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-30 09:54:11.331757 deepsights-api-1.0.3/deepsights/
+-rw-r--r--   0 0x1af      (501) staff       (20)      851 2024-03-25 16:53:44.000000 deepsights-api-1.0.3/deepsights/__init__.py
+drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-30 09:54:11.332162 deepsights-api-1.0.3/deepsights/api/
+-rw-r--r--   0 0x1af      (501) staff       (20)      786 2024-03-25 15:56:22.000000 deepsights-api-1.0.3/deepsights/api/__init__.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     7798 2024-03-25 17:49:54.000000 deepsights-api-1.0.3/deepsights/api/api.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     1161 2024-03-24 07:09:55.000000 deepsights-api-1.0.3/deepsights/api/resource.py
+drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-30 09:54:11.332394 deepsights-api-1.0.3/deepsights/contentstore/
+-rw-r--r--   0 0x1af      (501) staff       (20)      741 2024-03-24 07:36:24.000000 deepsights-api-1.0.3/deepsights/contentstore/__init__.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     1672 2024-03-25 17:23:37.000000 deepsights-api-1.0.3/deepsights/contentstore/contentstore.py
+drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-30 09:54:11.333058 deepsights-api-1.0.3/deepsights/contentstore/resources/
+-rw-r--r--   0 0x1af      (501) staff       (20)      851 2024-03-25 17:24:10.000000 deepsights-api-1.0.3/deepsights/contentstore/resources/__init__.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     2374 2024-05-17 08:07:26.000000 deepsights-api-1.0.3/deepsights/contentstore/resources/_model.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     9826 2024-05-30 09:38:38.000000 deepsights-api-1.0.3/deepsights/contentstore/resources/_search.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     7524 2024-05-30 09:46:55.000000 deepsights-api-1.0.3/deepsights/contentstore/resources/news.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     7580 2024-05-30 09:44:52.000000 deepsights-api-1.0.3/deepsights/contentstore/resources/secondary.py
+drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-30 09:54:11.333467 deepsights-api-1.0.3/deepsights/deepsights/
+-rw-r--r--   0 0x1af      (501) staff       (20)      735 2024-03-25 16:48:54.000000 deepsights-api-1.0.3/deepsights/deepsights/__init__.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     2861 2024-03-25 17:30:36.000000 deepsights-api-1.0.3/deepsights/deepsights/_mip_identity.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     3327 2024-03-25 17:51:00.000000 deepsights-api-1.0.3/deepsights/deepsights/deepsights.py
+drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-30 09:54:11.333592 deepsights-api-1.0.3/deepsights/deepsights/resources/
+-rw-r--r--   0 0x1af      (501) staff       (20)      766 2024-03-25 16:48:34.000000 deepsights-api-1.0.3/deepsights/deepsights/resources/__init__.py
+drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-30 09:54:11.333962 deepsights-api-1.0.3/deepsights/deepsights/resources/quota/
+-rw-r--r--   0 0x1af      (501) staff       (20)      847 2024-03-25 16:44:48.000000 deepsights-api-1.0.3/deepsights/deepsights/resources/quota/__init__.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     3311 2024-03-12 21:03:07.000000 deepsights-api-1.0.3/deepsights/deepsights/resources/quota/_model.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     1893 2024-03-25 16:44:57.000000 deepsights-api-1.0.3/deepsights/deepsights/resources/quota/quota.py
+drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-30 09:54:11.334206 deepsights-api-1.0.3/deepsights/documentstore/
+-rw-r--r--   0 0x1af      (501) staff       (20)      847 2024-03-25 17:24:56.000000 deepsights-api-1.0.3/deepsights/documentstore/__init__.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     1607 2024-03-25 17:25:25.000000 deepsights-api-1.0.3/deepsights/documentstore/documentstore.py
+drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-30 09:54:11.334346 deepsights-api-1.0.3/deepsights/documentstore/resources/
+-rw-r--r--   0 0x1af      (501) staff       (20)      828 2024-03-25 17:25:49.000000 deepsights-api-1.0.3/deepsights/documentstore/resources/__init__.py
+drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-30 09:54:11.335967 deepsights-api-1.0.3/deepsights/documentstore/resources/documents/
+-rw-r--r--   0 0x1af      (501) staff       (20)      880 2024-03-25 16:42:51.000000 deepsights-api-1.0.3/deepsights/documentstore/resources/documents/__init__.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     1232 2024-03-24 08:05:24.000000 deepsights-api-1.0.3/deepsights/documentstore/resources/documents/_cache.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     2841 2024-03-25 16:42:51.000000 deepsights-api-1.0.3/deepsights/documentstore/resources/documents/_delete.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     2510 2024-03-25 16:42:51.000000 deepsights-api-1.0.3/deepsights/documentstore/resources/documents/_download.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     3269 2024-03-25 16:42:51.000000 deepsights-api-1.0.3/deepsights/documentstore/resources/documents/_list.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     5406 2024-03-25 16:42:51.000000 deepsights-api-1.0.3/deepsights/documentstore/resources/documents/_load.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     5582 2024-03-25 16:42:51.000000 deepsights-api-1.0.3/deepsights/documentstore/resources/documents/_model.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     6823 2024-03-25 16:42:51.000000 deepsights-api-1.0.3/deepsights/documentstore/resources/documents/_search.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     3378 2024-03-12 21:03:07.000000 deepsights-api-1.0.3/deepsights/documentstore/resources/documents/_segmenter.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     4560 2024-03-25 16:42:51.000000 deepsights-api-1.0.3/deepsights/documentstore/resources/documents/_upload.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     1923 2024-03-25 16:42:51.000000 deepsights-api-1.0.3/deepsights/documentstore/resources/documents/documents.py
+drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-30 09:54:11.336410 deepsights-api-1.0.3/deepsights/userclient/
+-rw-r--r--   0 0x1af      (501) staff       (20)      756 2024-03-25 17:33:09.000000 deepsights-api-1.0.3/deepsights/userclient/__init__.py
+drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-30 09:54:11.336824 deepsights-api-1.0.3/deepsights/userclient/minions/
+-rw-r--r--   0 0x1af      (501) staff       (20)        0 2024-03-12 21:03:07.000000 deepsights-api-1.0.3/deepsights/userclient/minions/__init__.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     1900 2024-03-24 08:06:13.000000 deepsights-api-1.0.3/deepsights/userclient/minions/_minions.py
+drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-30 09:54:11.337107 deepsights-api-1.0.3/deepsights/userclient/resources/
+-rw-r--r--   0 0x1af      (501) staff       (20)      833 2024-03-25 17:32:47.000000 deepsights-api-1.0.3/deepsights/userclient/resources/__init__.py
+drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-30 09:54:11.337536 deepsights-api-1.0.3/deepsights/userclient/resources/answers/
+-rw-r--r--   0 0x1af      (501) staff       (20)      774 2024-03-25 17:31:44.000000 deepsights-api-1.0.3/deepsights/userclient/resources/answers/__init__.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     4057 2024-03-25 18:15:10.000000 deepsights-api-1.0.3/deepsights/userclient/resources/answers/_model.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     4365 2024-03-25 18:12:47.000000 deepsights-api-1.0.3/deepsights/userclient/resources/answers/answer.py
+drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-30 09:54:11.337968 deepsights-api-1.0.3/deepsights/userclient/resources/reports/
+-rw-r--r--   0 0x1af      (501) staff       (20)      775 2024-03-25 17:33:28.000000 deepsights-api-1.0.3/deepsights/userclient/resources/reports/__init__.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     5004 2024-03-25 18:22:13.000000 deepsights-api-1.0.3/deepsights/userclient/resources/reports/_model.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     4739 2024-03-26 10:43:01.000000 deepsights-api-1.0.3/deepsights/userclient/resources/reports/report.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     1547 2024-03-25 17:32:59.000000 deepsights-api-1.0.3/deepsights/userclient/userclient.py
+drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-30 09:54:11.338615 deepsights-api-1.0.3/deepsights/utils/
+-rw-r--r--   0 0x1af      (501) staff       (20)     1062 2024-03-12 21:03:07.000000 deepsights-api-1.0.3/deepsights/utils/__init__.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     1995 2024-03-12 21:03:07.000000 deepsights-api-1.0.3/deepsights/utils/_cache.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     5901 2024-03-23 10:16:37.000000 deepsights-api-1.0.3/deepsights/utils/_ranking.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     1543 2024-03-12 21:03:07.000000 deepsights-api-1.0.3/deepsights/utils/_utils.py
+-rw-r--r--   0 0x1af      (501) staff       (20)     2750 2024-03-12 21:03:07.000000 deepsights-api-1.0.3/deepsights/utils/model.py
+drwxr-xr-x   0 0x1af      (501) staff       (20)        0 2024-05-30 09:54:11.339350 deepsights-api-1.0.3/deepsights_api.egg-info/
+-rw-r--r--   0 0x1af      (501) staff       (20)     4754 2024-05-30 09:54:11.000000 deepsights-api-1.0.3/deepsights_api.egg-info/PKG-INFO
+-rw-r--r--   0 0x1af      (501) staff       (20)     2296 2024-05-30 09:54:11.000000 deepsights-api-1.0.3/deepsights_api.egg-info/SOURCES.txt
+-rw-r--r--   0 0x1af      (501) staff       (20)        1 2024-05-30 09:54:11.000000 deepsights-api-1.0.3/deepsights_api.egg-info/dependency_links.txt
+-rw-r--r--   0 0x1af      (501) staff       (20)      117 2024-05-30 09:54:11.000000 deepsights-api-1.0.3/deepsights_api.egg-info/requires.txt
+-rw-r--r--   0 0x1af      (501) staff       (20)       11 2024-05-30 09:54:11.000000 deepsights-api-1.0.3/deepsights_api.egg-info/top_level.txt
+-rw-r--r--   0 0x1af      (501) staff       (20)       38 2024-05-30 09:54:11.339901 deepsights-api-1.0.3/setup.cfg
+-rw-r--r--   0 0x1af      (501) staff       (20)     2023 2024-05-30 09:36:22.000000 deepsights-api-1.0.3/setup.py
```

### Comparing `deepsights-api-1.0.2/LICENSE` & `deepsights-api-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/PKG-INFO` & `deepsights-api-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepsights-api
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python library for the DeepSights APIs
 Home-page: https://github.com/marketlogicsoftware/deepsights-api
 Author: Market Logic Software
 Author-email: info@marketlogicsoftware.com
 License: Apache 2.0
 Project-URL: Documentation, https://marketlogicsoftware.github.io/deepsights-api/
 Classifier: Intended Audience :: Developers
```

### Comparing `deepsights-api-1.0.2/README.md` & `deepsights-api-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/__init__.py` & `deepsights-api-1.0.3/deepsights/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/api/__init__.py` & `deepsights-api-1.0.3/deepsights/api/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/api/api.py` & `deepsights-api-1.0.3/deepsights/api/api.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/api/resource.py` & `deepsights-api-1.0.3/deepsights/api/resource.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/contentstore/__init__.py` & `deepsights-api-1.0.3/deepsights/contentstore/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/contentstore/contentstore.py` & `deepsights-api-1.0.3/deepsights/contentstore/contentstore.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/contentstore/resources/__init__.py` & `deepsights-api-1.0.3/deepsights/contentstore/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/contentstore/resources/_model.py` & `deepsights-api-1.0.3/deepsights/contentstore/resources/_model.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/contentstore/resources/_search.py` & `deepsights-api-1.0.3/deepsights/contentstore/resources/_search.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,14 +23,38 @@
 from deepsights.utils import (
     promote_exact_matches,
     rerank_by_recency,
 )
 
 
 #################################################
+def _get_time_filter(search_from_timestamp: datetime, search_to_timestamp: datetime):
+    """
+    Returns a time filter dictionary based on the provided search_from_timestamp and search_to_timestamp.
+
+    Args:
+        search_from_timestamp (datetime): The starting timestamp for the search.
+        search_to_timestamp (datetime): The ending timestamp for the search.
+
+    Returns:
+        dict: A time filter dictionary with "from" and "to" keys representing the search range.
+              The values are ISO-formatted timestamps or None if the corresponding input is None.
+    """
+    time_filter = None
+    if search_from_timestamp or search_to_timestamp:
+        time_filter = {
+            "from": (
+                search_from_timestamp.isoformat() if search_from_timestamp else None
+            ),
+            "to": search_to_timestamp.isoformat() if search_to_timestamp else None,
+        }
+    return time_filter
+
+
+#################################################
 def contentstore_hybrid_search(
     api: API,
     query: str,
     item_type: str,
     search_result: BaseModel,
     max_results: int = 100,
     languages: List[str] = None,
@@ -70,34 +94,25 @@
     assert 0 <= vector_fraction <= 1, "Vector fraction must be between 0 and 1"
     assert 0 <= vector_weight <= 1, "Vector weught must be between 0 and 1"
     assert 0 < max_results <= 250, "Maximum results must be between 1 and 250."
     assert (
         recency_weight is None or 0 <= recency_weight <= 1
     ), "Recency weight must be between 0 and 1."
 
-    time_filter = None
-    if search_from_timestamp or search_to_timestamp:
-        time_filter = {
-            "from": (
-                search_from_timestamp.isoformat() if search_from_timestamp else None
-            ),
-            "to": search_to_timestamp.isoformat() if search_to_timestamp else None,
-        }
-
     body = {
         "query": query,
         "source_items_type": item_type,
         "content_restrictions": "NONE",
         "limit": max_results,
         "vector_search_cut_off_score": min_vector_score,
         "alfa": vector_weight,
         "beta": 1.0 - recency_weight,
         "text_search_fraction": 1.0 - vector_fraction,
         "k": 60,
-        "published_at": time_filter,
+        "published_at": _get_time_filter(search_from_timestamp, search_to_timestamp),
         "languages": languages,
     }
     response = api.post("item-service/items/_hybrid-search", body=body)
 
     # parse
     results = [search_result(i) for i in response["items"]]
 
@@ -118,28 +133,32 @@
     query_embedding: List,
     item_type: str,
     search_result: BaseModel,
     min_score: float = 0.7,
     max_results: int = 50,
     languages: List[str] = None,
     recency_weight: float = None,
+    search_from_timestamp: datetime = None,
+    search_to_timestamp: datetime = None,
 ):
     """
     Perform a contentstore vector search using the provided query embedding.
 
     Args:
 
         api (API): The DeepSights API instance.
         query_embedding (List): The query embedding vector.
         item_type (str): The type of items to search for.
         search_result (BaseModel): The model to use for parsing search results.
         min_score (float, optional): The minimum score threshold for search results. Defaults to 0.7.
         max_results (int, optional): The maximum number of search results to return. Defaults to 50.
         languages (List[str], optional): The languages to search for. Defaults to None.
         recency_weight (float, optional): The weight to apply to recency in result ranking. Defaults to None.
+        search_from_timestamp (datetime, optional): The start timestamp for the search. Defaults to None.
+        search_to_timestamp (datetime, optional): The end timestamp for the search. Defaults to None.
 
     Returns:
 
         List[BaseModel]: The re-ranked search results.
     """
     assert query_embedding, "The 'query_embedding' argument is required."
     assert len(query_embedding) == 1536, "The 'query_embedding' must be of length 1536."
@@ -153,14 +172,15 @@
         "vector": query_embedding,
         "source_items_type": item_type,
         "content_restrictions": "NONE",
         "limit": max_results,
         "score_lower_bound": min_score,
         "sort": "RELEVANCY_DESC",
         "languages": languages,
+        "published_at": _get_time_filter(search_from_timestamp, search_to_timestamp),
     }
     response = api.post("item-service/items/_vector-search", body=body)
 
     # parse
     results = [search_result(i) for i in response["items"]]
 
     # re-rank
@@ -173,28 +193,32 @@
     query: str,
     item_type: str,
     search_result: BaseModel,
     max_results: int = 50,
     offset: int = 0,
     languages: List[str] = None,
     recency_weight: float = None,
+    search_from_timestamp: datetime = None,
+    search_to_timestamp: datetime = None,
 ):
     """
     Perform a contentstore text search using the specified query and item type. If the query is None, the search will be sorted by publication date.
 
     Args:
 
         api (API): The DeepSights API instance.
         query (str): The search query.
         item_type (str): The type of items to search for.
         search_result (BaseModel): The model used to parse the search results.
         max_results (int, optional): The maximum number of results to return. Defaults to 50.
         offset (int, optional): The offset to start the search from. Defaults to 0.
         languages (List[str], optional): The languages to search for. Defaults to None.
         recency_weight (float, optional): The weight assigned to recency in result ranking. Defaults to None.
+        search_from_timestamp (datetime, optional): The start timestamp for the search. Defaults to None.
+        search_to_timestamp (datetime, optional): The end timestamp for the search. Defaults to None.
 
     Returns:
 
         List[BaseModel]: The re-ranked search results.
     """
     assert 0 < max_results <= 100, "Maximum results must be between 1 and 100."
     assert (
@@ -209,14 +233,15 @@
         "query": query,
         "source_items_type": item_type,
         "content_restrictions": "NONE",
         "limit": max_results,
         "offset": offset,
         "sort": "RELEVANCY_DESC" if query is not None else "PUBLISHED_AT_DESC",
         "languages": languages,
+        "published_at": _get_time_filter(search_from_timestamp, search_to_timestamp),
     }
     response = api.post("item-service/items/_text-search", body=body)
 
     # parse
     results = [search_result(i) for i in response["items"]]
 
     # re-rank
```

### Comparing `deepsights-api-1.0.2/deepsights/contentstore/resources/news.py` & `deepsights-api-1.0.3/deepsights/contentstore/resources/secondary.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,123 +9,134 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
-This module defines the resource to retrieve news content from the DeepSights API.
+This module contains the resource to retrieve secondary reports from the DeepSights content store.
 """
 
 from typing import List
 from datetime import datetime
 
 from deepsights.api import APIResource
 from deepsights.contentstore.resources._model import ContentStoreSearchResult
 from deepsights.contentstore.resources._search import (
     contentstore_text_search,
     contentstore_vector_search,
     contentstore_hybrid_search,
 )
 
 
-
 #################################################
-class NewsSearchResult(ContentStoreSearchResult):
+class SecondarySearchResult(ContentStoreSearchResult):
     """
-    Represents a search result of a news article in the content store.
+    Represents a search result of a secondary report in the DeepSights API.
     """
 
 
 #################################################
-class NewsResource(APIResource):
+class SecondaryResource(APIResource):
     """
-    Represents a resource for retrieving news articles from the DeepSights content store.
+    Represents a resource for retrieving secondary reports from the DeepSights content store.
     """
 
     #################################################
     def vector_search(
         self,
         query_embedding: List,
         min_score: float = 0.7,
-        max_results: int = 30,
+        max_results: int = 50,
         languages: List[str] = None,
         recency_weight: float = None,
+        search_from_timestamp: datetime = None,
+        search_to_timestamp: datetime = None,
     ):
         """
-        Perform a vector-based search for news articles.
+        Perform a vector-based search for secondary reports.
 
         Args:
 
             query_embedding (List): The embedding vector representing the query.
             min_score (float, optional): The minimum score threshold for search results. Defaults to 0.7.
-            max_results (int, optional): The maximum number of search results to return. Defaults to 30.
-            languages (List[str], optional): The list of languages to search for. Defaults to None.
+            max_results (int, optional): The maximum number of search results to return. Defaults to 50.
+            languages (List[str], optional): The languages to search for. Defaults to None.
             recency_weight (float, optional): The weight to apply to recency in the search ranking. Defaults to None.
+            search_from_timestamp (datetime, optional): The start timestamp for the search. Defaults to None.
+            search_to_timestamp (datetime, optional): The end timestamp for the search. Defaults to None.
 
         Returns:
 
-            List[NewsArticleSearchResult]: A list of search results as NewsArticleSearchResult objects.
+            List[SecondaryReportSearchResult]: A list of search results as SecondaryReportSearchResult objects.
         """
 
         return contentstore_vector_search(
             self.api,
-            item_type="NEWS",
-            search_result=lambda i: NewsSearchResult(
+            item_type="REPORTS",
+            search_result=lambda i: SecondarySearchResult(
                 **dict(source_name=i["source"]["display_name"], **i)
             ),
             query_embedding=query_embedding,
             min_score=min_score,
             max_results=max_results,
             recency_weight=recency_weight,
             languages=languages,
+            search_from_timestamp=search_from_timestamp,
+            search_to_timestamp=search_to_timestamp,
         )
 
     #################################################
     def text_search(
         self,
         query: str,
-        max_results: int = 30,
+        max_results: int = 50,
         offset: int = 0,
         languages: List[str] = None,
         recency_weight: float = None,
+        search_from_timestamp: datetime = None,
+        search_to_timestamp: datetime = None,
     ):
         """
-        Perform a text search for news articles in the DeepSights content store.
+        Perform a text search for secondary reports in the DeepSights content store.
 
         Args:
 
             query (str): The search query.
-            max_results (int, optional): The maximum number of search results to return. Defaults to 30.
+            max_results (int, optional): The maximum number of search results to return. Defaults to 50.
             offset (int, optional): The offset to start the search from. Defaults to 0.
-            languages (List[str], optional): The list of languages to search for. Defaults to None.
+            languages (List[str], optional): The languages to search for. Defaults to None.
             recency_weight (float, optional): The weight to assign to recency in the search ranking. Defaults to None.
+            search_from_timestamp (datetime, optional): The start timestamp for the search. Defaults to None.
+            search_to_timestamp (datetime, optional): The end timestamp for the search. Defaults to None.
 
         Returns:
 
-            List[NewsArticleSearchResult]: A list of news article search results.
+            List[SecondaryReportSearchResult]: A list of news article search results.
         """
         return contentstore_text_search(
             self.api,
-            item_type="NEWS",
-            search_result=lambda i: NewsSearchResult(
+            item_type="REPORTS",
+            search_result=lambda i: SecondarySearchResult(
                 **dict(source_name=i["source"]["display_name"], **i)
             ),
             query=query,
             max_results=max_results,
-            recency_weight=recency_weight,
-            languages=languages,
             offset=offset,
+            languages=languages,
+            recency_weight=recency_weight,
+            search_from_timestamp=search_from_timestamp,
+            search_to_timestamp=search_to_timestamp,
         )
 
     #################################################
     def search(
         self,
         query: str,
-        max_results: int = 30,
+        max_results: int = 100,
         languages: List[str] = None,
         min_vector_score: float = 0.7,
         vector_fraction: float = 0.9,
         vector_weight: float = 0.9,
         recency_weight: float = 0.4,
         promote_exact_match: bool = False,
         search_from_timestamp: datetime = None,
@@ -134,32 +145,32 @@
         """
         Perform a contentstore hybrid search using the provided query.
 
         Args:
 
             query (str): The query.
             search_result (BaseModel): The model to use for parsing search results.
-            max_results (int, optional): The maximum number of search results to return. Defaults to 30.
-            languages (List[str], optional): The list of languages to search for. Defaults to None.
+            max_results (int, optional): The maximum number of search results to return. Defaults to 100.
+            languages (List[str], optional): The languages to search for. Defaults to None.
             min_vector_score (float, optional): The minimum score threshold for search results. Defaults to 0.7.
             vector_fraction (float, optional): The fraction of the search results to be vector-based. Defaults to 0.9.
             vector_weight (float, optional): The weight to apply to vector search in result ranking. Defaults to 0.9.
             recency_weight (float, optional): The weight to apply to recency in result ranking. Defaults to 0.4.
             promote_exact_match (bool, optional): Whether to promote exact matches in the search ranking. Defaults to False.
             search_from_timestamp (datetime, optional): The start timestamp for the search. Defaults to None.
             search_to_timestamp (datetime, optional): The end timestamp for the search. Defaults to None.
 
         Returns:
 
             List[NewsArticleSearchResult]: The search results as a list of NewsArticleSearchResult objects.
         """
         return contentstore_hybrid_search(
             self.api,
-            item_type="NEWS",
-            search_result=lambda i: NewsSearchResult(
+            item_type="REPORTS",
+            search_result=lambda i: SecondarySearchResult(
                 **dict(source_name=i["source"]["display_name"], **i)
             ),
             query=query,
             max_results=max_results,
             vector_weight=vector_weight,
             vector_fraction=vector_fraction,
             min_vector_score=min_vector_score,
```

### Comparing `deepsights-api-1.0.2/deepsights/deepsights/__init__.py` & `deepsights-api-1.0.3/deepsights/deepsights/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/deepsights/_mip_identity.py` & `deepsights-api-1.0.3/deepsights/deepsights/_mip_identity.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/deepsights/deepsights.py` & `deepsights-api-1.0.3/deepsights/deepsights/deepsights.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/deepsights/resources/__init__.py` & `deepsights-api-1.0.3/deepsights/deepsights/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/deepsights/resources/quota/__init__.py` & `deepsights-api-1.0.3/deepsights/deepsights/resources/quota/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/deepsights/resources/quota/_model.py` & `deepsights-api-1.0.3/deepsights/deepsights/resources/quota/_model.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/deepsights/resources/quota/quota.py` & `deepsights-api-1.0.3/deepsights/deepsights/resources/quota/quota.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/documentstore/__init__.py` & `deepsights-api-1.0.3/deepsights/documentstore/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/documentstore/documentstore.py` & `deepsights-api-1.0.3/deepsights/documentstore/documentstore.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/documentstore/resources/__init__.py` & `deepsights-api-1.0.3/deepsights/documentstore/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/documentstore/resources/documents/__init__.py` & `deepsights-api-1.0.3/deepsights/documentstore/resources/documents/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/documentstore/resources/documents/_cache.py` & `deepsights-api-1.0.3/deepsights/documentstore/resources/documents/_cache.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/documentstore/resources/documents/_delete.py` & `deepsights-api-1.0.3/deepsights/documentstore/resources/documents/_delete.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/documentstore/resources/documents/_download.py` & `deepsights-api-1.0.3/deepsights/documentstore/resources/documents/_download.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/documentstore/resources/documents/_list.py` & `deepsights-api-1.0.3/deepsights/documentstore/resources/documents/_list.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/documentstore/resources/documents/_load.py` & `deepsights-api-1.0.3/deepsights/documentstore/resources/documents/_load.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/documentstore/resources/documents/_model.py` & `deepsights-api-1.0.3/deepsights/documentstore/resources/documents/_model.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/documentstore/resources/documents/_search.py` & `deepsights-api-1.0.3/deepsights/documentstore/resources/documents/_search.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/documentstore/resources/documents/_segmenter.py` & `deepsights-api-1.0.3/deepsights/documentstore/resources/documents/_segmenter.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/documentstore/resources/documents/_upload.py` & `deepsights-api-1.0.3/deepsights/documentstore/resources/documents/_upload.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/documentstore/resources/documents/documents.py` & `deepsights-api-1.0.3/deepsights/documentstore/resources/documents/documents.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/userclient/__init__.py` & `deepsights-api-1.0.3/deepsights/userclient/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/userclient/minions/_minions.py` & `deepsights-api-1.0.3/deepsights/userclient/minions/_minions.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/userclient/resources/__init__.py` & `deepsights-api-1.0.3/deepsights/userclient/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/userclient/resources/answers/__init__.py` & `deepsights-api-1.0.3/deepsights/userclient/resources/answers/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/userclient/resources/answers/_model.py` & `deepsights-api-1.0.3/deepsights/userclient/resources/answers/_model.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/userclient/resources/answers/answer.py` & `deepsights-api-1.0.3/deepsights/userclient/resources/answers/answer.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/userclient/resources/reports/__init__.py` & `deepsights-api-1.0.3/deepsights/userclient/resources/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/userclient/resources/reports/_model.py` & `deepsights-api-1.0.3/deepsights/userclient/resources/reports/_model.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/userclient/resources/reports/report.py` & `deepsights-api-1.0.3/deepsights/userclient/resources/reports/report.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/userclient/userclient.py` & `deepsights-api-1.0.3/deepsights/userclient/userclient.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/utils/__init__.py` & `deepsights-api-1.0.3/deepsights/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/utils/_cache.py` & `deepsights-api-1.0.3/deepsights/utils/_cache.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/utils/_ranking.py` & `deepsights-api-1.0.3/deepsights/utils/_ranking.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/utils/_utils.py` & `deepsights-api-1.0.3/deepsights/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights/utils/model.py` & `deepsights-api-1.0.3/deepsights/utils/model.py`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/deepsights_api.egg-info/PKG-INFO` & `deepsights-api-1.0.3/deepsights_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepsights-api
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python library for the DeepSights APIs
 Home-page: https://github.com/marketlogicsoftware/deepsights-api
 Author: Market Logic Software
 Author-email: info@marketlogicsoftware.com
 License: Apache 2.0
 Project-URL: Documentation, https://marketlogicsoftware.github.io/deepsights-api/
 Classifier: Intended Audience :: Developers
```

### Comparing `deepsights-api-1.0.2/deepsights_api.egg-info/SOURCES.txt` & `deepsights-api-1.0.3/deepsights_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepsights-api-1.0.2/setup.py` & `deepsights-api-1.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 reqs_filename = os.path.join(package_root, "requirements.txt")
 with io.open(reqs_filename, encoding="utf-8") as reqs_file:
     reqs = reqs_file.read().splitlines()
 
 setup(
     name="deepsights-api",
-    version="1.0.2",
+    version="1.0.3",
     author="Market Logic Software",
     author_email="info@marketlogicsoftware.com",
     description="Python library for the DeepSights APIs",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/marketlogicsoftware/deepsights-api",
     packages=find_packages(exclude=["tests", "tests.*"]),
```

