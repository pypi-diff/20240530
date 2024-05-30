# Comparing `tmp/feedsbot-0.5.0.tar.gz` & `tmp/feedsbot-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feedsbot-0.5.0.tar", last modified: Sat Apr 27 20:40:16 2024, max compression
+gzip compressed data, was "feedsbot-0.6.0.tar", last modified: Thu May 30 17:02:39 2024, max compression
```

## Comparing `feedsbot-0.5.0.tar` & `feedsbot-0.6.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:40:16.446969 feedsbot-0.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:40:16.442969 feedsbot-0.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-27 20:40:07.000000 feedsbot-0.5.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:40:16.442969 feedsbot-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-27 20:40:07.000000 feedsbot-0.5.0/.github/workflows/python-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-27 20:40:07.000000 feedsbot-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-27 20:40:07.000000 feedsbot-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-27 20:40:16.446969 feedsbot-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-27 20:40:07.000000 feedsbot-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-04-27 20:40:07.000000 feedsbot-0.5.0/avatar.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:40:16.442969 feedsbot-0.5.0/feedsbot/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-27 20:40:07.000000 feedsbot-0.5.0/feedsbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-27 20:40:16.000000 feedsbot-0.5.0/feedsbot/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    10830 2024-04-27 20:40:07.000000 feedsbot-0.5.0/feedsbot/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-27 20:40:07.000000 feedsbot-0.5.0/feedsbot/orm.py
--rw-r--r--   0 runner    (1001) docker     (127)     9831 2024-04-27 20:40:07.000000 feedsbot-0.5.0/feedsbot/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:40:16.446969 feedsbot-0.5.0/feedsbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-27 20:40:16.000000 feedsbot-0.5.0/feedsbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-27 20:40:16.000000 feedsbot-0.5.0/feedsbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 20:40:16.000000 feedsbot-0.5.0/feedsbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-27 20:40:16.000000 feedsbot-0.5.0/feedsbot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-27 20:40:16.000000 feedsbot-0.5.0/feedsbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-27 20:40:16.000000 feedsbot-0.5.0/feedsbot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-27 20:40:07.000000 feedsbot-0.5.0/pylama.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-27 20:40:07.000000 feedsbot-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 20:40:16.446969 feedsbot-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:02:39.105045 feedsbot-0.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:02:39.101045 feedsbot-0.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-30 17:02:29.000000 feedsbot-0.6.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:02:39.101045 feedsbot-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-30 17:02:29.000000 feedsbot-0.6.0/.github/workflows/python-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-30 17:02:29.000000 feedsbot-0.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-05-30 17:02:29.000000 feedsbot-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-30 17:02:39.105045 feedsbot-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-30 17:02:29.000000 feedsbot-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-05-30 17:02:29.000000 feedsbot-0.6.0/avatar.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:02:39.101045 feedsbot-0.6.0/feedsbot/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-30 17:02:29.000000 feedsbot-0.6.0/feedsbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-30 17:02:29.000000 feedsbot-0.6.0/feedsbot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-30 17:02:39.000000 feedsbot-0.6.0/feedsbot/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10830 2024-05-30 17:02:29.000000 feedsbot-0.6.0/feedsbot/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-30 17:02:29.000000 feedsbot-0.6.0/feedsbot/orm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9831 2024-05-30 17:02:29.000000 feedsbot-0.6.0/feedsbot/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:02:39.101045 feedsbot-0.6.0/feedsbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-30 17:02:39.000000 feedsbot-0.6.0/feedsbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-30 17:02:39.000000 feedsbot-0.6.0/feedsbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 17:02:39.000000 feedsbot-0.6.0/feedsbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-30 17:02:39.000000 feedsbot-0.6.0/feedsbot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-30 17:02:39.000000 feedsbot-0.6.0/feedsbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-30 17:02:39.000000 feedsbot-0.6.0/feedsbot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-30 17:02:29.000000 feedsbot-0.6.0/pylama.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-30 17:02:29.000000 feedsbot-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 17:02:39.105045 feedsbot-0.6.0/setup.cfg
```

### Comparing `feedsbot-0.5.0/.github/dependabot.yml` & `feedsbot-0.6.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `feedsbot-0.5.0/.github/workflows/python-ci.yml` & `feedsbot-0.6.0/.github/workflows/python-ci.yml`

 * *Files identical despite different names*

### Comparing `feedsbot-0.5.0/LICENSE` & `feedsbot-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `feedsbot-0.5.0/PKG-INFO` & `feedsbot-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feedsbot
-Version: 0.5.0
+Version: 0.6.0
 Summary: Subscribe to RSS/Atom feeds in Delta Chat
 Author-email: adbenitez <adb@merlinux.eu>
 Project-URL: Homepage, https://github.com/deltachat-bot/feedsbot
 Keywords: deltachat,bot,feeds,rss,atom
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `feedsbot-0.5.0/README.md` & `feedsbot-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `feedsbot-0.5.0/avatar.png` & `feedsbot-0.6.0/avatar.png`

 * *Files identical despite different names*

### Comparing `feedsbot-0.5.0/feedsbot/hooks.py` & `feedsbot-0.6.0/feedsbot/hooks.py`

 * *Files identical despite different names*

### Comparing `feedsbot-0.5.0/feedsbot/orm.py` & `feedsbot-0.6.0/feedsbot/orm.py`

 * *Files identical despite different names*

### Comparing `feedsbot-0.5.0/feedsbot/util.py` & `feedsbot-0.6.0/feedsbot/util.py`

 * *Files identical despite different names*

### Comparing `feedsbot-0.5.0/feedsbot.egg-info/PKG-INFO` & `feedsbot-0.6.0/feedsbot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feedsbot
-Version: 0.5.0
+Version: 0.6.0
 Summary: Subscribe to RSS/Atom feeds in Delta Chat
 Author-email: adbenitez <adb@merlinux.eu>
 Project-URL: Homepage, https://github.com/deltachat-bot/feedsbot
 Keywords: deltachat,bot,feeds,rss,atom
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `feedsbot-0.5.0/pyproject.toml` & `feedsbot-0.6.0/pyproject.toml`

 * *Files identical despite different names*

