# Comparing `tmp/roxcrypter-1.0.0.tar.gz` & `tmp/roxcrypter-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roxcrypter-1.0.0.tar", last modified: Thu May 30 17:35:51 2024, max compression
+gzip compressed data, was "roxcrypter-1.0.1.tar", last modified: Thu May 30 19:50:50 2024, max compression
```

## Comparing `roxcrypter-1.0.0.tar` & `roxcrypter-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 17:35:51.658278 roxcrypter-1.0.0/
--rw-rw-rw-   0        0        0     7651 2016-12-23 23:26:00.000000 roxcrypter-1.0.0/LICENSE.md
--rw-rw-rw-   0        0        0      231 2024-05-30 17:35:51.656276 roxcrypter-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      492 2016-12-23 23:26:00.000000 roxcrypter-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 17:35:51.645885 roxcrypter-1.0.0/roxCrypter/
--rw-rw-rw-   0        0        0      960 2024-05-30 17:29:08.000000 roxcrypter-1.0.0/roxCrypter/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 17:35:51.655276 roxcrypter-1.0.0/roxCrypter.egg-info/
--rw-rw-rw-   0        0        0      231 2024-05-30 17:35:51.000000 roxcrypter-1.0.0/roxCrypter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2024-05-30 17:35:51.000000 roxcrypter-1.0.0/roxCrypter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 17:35:51.000000 roxcrypter-1.0.0/roxCrypter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-30 17:35:51.000000 roxcrypter-1.0.0/roxCrypter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 17:35:51.658278 roxcrypter-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      300 2024-05-30 17:30:03.000000 roxcrypter-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 19:50:50.948517 roxcrypter-1.0.1/
+-rw-rw-rw-   0        0        0     7651 2016-12-23 23:26:00.000000 roxcrypter-1.0.1/LICENSE.md
+-rw-rw-rw-   0        0        0     2589 2024-05-30 19:50:50.944514 roxcrypter-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2132 2024-05-30 17:54:31.000000 roxcrypter-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 19:50:50.924494 roxcrypter-1.0.1/roxCrypter/
+-rw-rw-rw-   0        0        0      960 2024-05-30 17:29:08.000000 roxcrypter-1.0.1/roxCrypter/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 19:50:50.942512 roxcrypter-1.0.1/roxCrypter.egg-info/
+-rw-rw-rw-   0        0        0     2589 2024-05-30 19:50:50.000000 roxcrypter-1.0.1/roxCrypter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2024-05-30 19:50:50.000000 roxcrypter-1.0.1/roxCrypter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 19:50:50.000000 roxcrypter-1.0.1/roxCrypter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-30 19:50:50.000000 roxcrypter-1.0.1/roxCrypter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 19:50:50.950520 roxcrypter-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      623 2024-05-30 19:48:10.000000 roxcrypter-1.0.1/setup.py
```

### Comparing `roxcrypter-1.0.0/LICENSE.md` & `roxcrypter-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `roxcrypter-1.0.0/roxCrypter/__init__.py` & `roxcrypter-1.0.1/roxCrypter/__init__.py`

 * *Files identical despite different names*

