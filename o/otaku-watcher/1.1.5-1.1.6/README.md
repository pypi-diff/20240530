# Comparing `tmp/otaku_watcher-1.1.5.tar.gz` & `tmp/otaku_watcher-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otaku_watcher-1.1.5.tar", last modified: Wed May 29 21:36:39 2024, max compression
+gzip compressed data, was "otaku_watcher-1.1.6.tar", last modified: Wed May 29 22:24:31 2024, max compression
```

## Comparing `otaku_watcher-1.1.5.tar` & `otaku_watcher-1.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-29 21:36:39.455577 otaku_watcher-1.1.5/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1063 2024-05-01 10:29:15.000000 otaku_watcher-1.1.5/LICENSE
--rw-r--r--   0 goldy     (1000) goldy     (1000)     3079 2024-05-29 21:36:39.455577 otaku_watcher-1.1.5/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)      846 2024-05-28 21:10:14.000000 otaku_watcher-1.1.5/README.md
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-29 21:36:39.452244 otaku_watcher-1.1.5/otaku_watcher/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      402 2024-05-29 21:36:30.000000 otaku_watcher-1.1.5/otaku_watcher/__init__.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-29 21:36:39.452244 otaku_watcher-1.1.5/otaku_watcher/anitaku/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       22 2024-05-01 10:29:15.000000 otaku_watcher-1.1.5/otaku_watcher/anitaku/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     5233 2024-05-29 21:35:54.000000 otaku_watcher-1.1.5/otaku_watcher/anitaku/scraper.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-29 21:36:39.452244 otaku_watcher-1.1.5/otaku_watcher.egg-info/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     3079 2024-05-29 21:36:39.000000 otaku_watcher-1.1.5/otaku_watcher.egg-info/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)      309 2024-05-29 21:36:39.000000 otaku_watcher-1.1.5/otaku_watcher.egg-info/SOURCES.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-05-29 21:36:39.000000 otaku_watcher-1.1.5/otaku_watcher.egg-info/dependency_links.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       86 2024-05-29 21:36:39.000000 otaku_watcher-1.1.5/otaku_watcher.egg-info/requires.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       14 2024-05-29 21:36:39.000000 otaku_watcher-1.1.5/otaku_watcher.egg-info/top_level.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1226 2024-05-01 10:29:15.000000 otaku_watcher-1.1.5/pyproject.toml
--rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-05-29 21:36:39.455577 otaku_watcher-1.1.5/setup.cfg
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-05-29 22:24:31.911163 otaku_watcher-1.1.6/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     1063 2024-05-29 21:32:04.000000 otaku_watcher-1.1.6/LICENSE
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     3079 2024-05-29 22:24:31.911163 otaku_watcher-1.1.6/PKG-INFO
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      846 2024-05-29 21:32:04.000000 otaku_watcher-1.1.6/README.md
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-05-29 22:24:31.907829 otaku_watcher-1.1.6/otaku_watcher/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      402 2024-05-29 22:22:34.000000 otaku_watcher-1.1.6/otaku_watcher/__init__.py
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-05-29 22:24:31.907829 otaku_watcher-1.1.6/otaku_watcher/anitaku/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)       22 2024-05-29 21:32:04.000000 otaku_watcher-1.1.6/otaku_watcher/anitaku/__init__.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     5233 2024-05-29 21:32:43.000000 otaku_watcher-1.1.6/otaku_watcher/anitaku/scraper.py
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-05-29 22:24:31.907829 otaku_watcher-1.1.6/otaku_watcher.egg-info/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     3079 2024-05-29 22:24:31.000000 otaku_watcher-1.1.6/otaku_watcher.egg-info/PKG-INFO
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      309 2024-05-29 22:24:31.000000 otaku_watcher-1.1.6/otaku_watcher.egg-info/SOURCES.txt
+-rw-r--r--   0 ananas    (1000) ananas    (1000)        1 2024-05-29 22:24:31.000000 otaku_watcher-1.1.6/otaku_watcher.egg-info/dependency_links.txt
+-rw-r--r--   0 ananas    (1000) ananas    (1000)       86 2024-05-29 22:24:31.000000 otaku_watcher-1.1.6/otaku_watcher.egg-info/requires.txt
+-rw-r--r--   0 ananas    (1000) ananas    (1000)       14 2024-05-29 22:24:31.000000 otaku_watcher-1.1.6/otaku_watcher.egg-info/top_level.txt
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     1209 2024-05-29 22:22:22.000000 otaku_watcher-1.1.6/pyproject.toml
+-rw-r--r--   0 ananas    (1000) ananas    (1000)       38 2024-05-29 22:24:31.911163 otaku_watcher-1.1.6/setup.cfg
```

### Comparing `otaku_watcher-1.1.5/LICENSE` & `otaku_watcher-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `otaku_watcher-1.1.5/PKG-INFO` & `otaku_watcher-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otaku-watcher
-Version: 1.1.5
+Version: 1.1.6
 Summary: A mov-cli plugin for watching anime.
 License: MIT License
         
         Copyright (c) 2024 JDALab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `otaku_watcher-1.1.5/README.md` & `otaku_watcher-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `otaku_watcher-1.1.5/otaku_watcher/anitaku/scraper.py` & `otaku_watcher-1.1.6/otaku_watcher/anitaku/scraper.py`

 * *Files identical despite different names*

### Comparing `otaku_watcher-1.1.5/otaku_watcher.egg-info/PKG-INFO` & `otaku_watcher-1.1.6/otaku_watcher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otaku-watcher
-Version: 1.1.5
+Version: 1.1.6
 Summary: A mov-cli plugin for watching anime.
 License: MIT License
         
         Copyright (c) 2024 JDALab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `otaku_watcher-1.1.5/pyproject.toml` & `otaku_watcher-1.1.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -41,8 +41,8 @@
 version = { attr = "otaku_watcher.__version__" }
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
-include = ["otaku_watcher*", "mov_cli_anime*"]
+include = ["otaku_watcher*"]
```

