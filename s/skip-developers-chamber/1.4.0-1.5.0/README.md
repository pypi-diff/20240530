# Comparing `tmp/skip-developers-chamber-1.4.0.tar.gz` & `tmp/skip_developers_chamber-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skip-developers-chamber-1.4.0.tar", last modified: Thu Apr 11 09:36:00 2024, max compression
+gzip compressed data, was "skip_developers_chamber-1.5.0.tar", last modified: Thu May 30 14:17:35 2024, max compression
```

## Comparing `skip-developers-chamber-1.4.0.tar` & `skip_developers_chamber-1.5.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:36:00.276886 skip-developers-chamber-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-11 09:36:00.276886 skip-developers-chamber-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15303 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:36:00.268886 skip-developers-chamber-1.4.0/developers_chamber/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:36:00.268886 skip-developers-chamber-1.4.0/developers_chamber/bin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/bin/pydev.py
--rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/bitbucket_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:36:00.272886 skip-developers-chamber-1.4.0/developers_chamber/click/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/click/options.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/docker_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    27455 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/ecs_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/git_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/gitlab_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/jira_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10673 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/project_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:36:00.272886 skip-developers-chamber-1.4.0/developers_chamber/qa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/qa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/qa/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/qa/checks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:36:00.272886 skip-developers-chamber-1.4.0/developers_chamber/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/scripts/bitbucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/scripts/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)    15433 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/scripts/ecs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/scripts/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/scripts/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/scripts/init_aliasses.py
--rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/scripts/jira.py
--rw-r--r--   0 runner    (1001) docker     (127)    18907 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/scripts/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/scripts/qa.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/scripts/sh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/scripts/slack.py
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/scripts/toggle.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/scripts/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/slack_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/toggle_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/developers_chamber/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 09:36:00.276886 skip-developers-chamber-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-11 09:35:56.000000 skip-developers-chamber-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:36:00.276886 skip-developers-chamber-1.4.0/skip_developers_chamber.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-11 09:36:00.000000 skip-developers-chamber-1.4.0/skip_developers_chamber.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-11 09:36:00.000000 skip-developers-chamber-1.4.0/skip_developers_chamber.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 09:36:00.000000 skip-developers-chamber-1.4.0/skip_developers_chamber.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-11 09:36:00.000000 skip-developers-chamber-1.4.0/skip_developers_chamber.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 09:36:00.000000 skip-developers-chamber-1.4.0/skip_developers_chamber.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-11 09:36:00.000000 skip-developers-chamber-1.4.0/skip_developers_chamber.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-11 09:36:00.000000 skip-developers-chamber-1.4.0/skip_developers_chamber.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:17:35.285627 skip_developers_chamber-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-30 14:17:29.000000 skip_developers_chamber-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-30 14:17:35.285627 skip_developers_chamber-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15303 2024-05-30 14:17:29.000000 skip_developers_chamber-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:17:35.281627 skip_developers_chamber-1.5.0/developers_chamber/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:17:29.000000 skip_developers_chamber-1.5.0/developers_chamber/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:17:35.281627 skip_developers_chamber-1.5.0/developers_chamber/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:17:29.000000 skip_developers_chamber-1.5.0/developers_chamber/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-30 14:17:29.000000 skip_developers_chamber-1.5.0/developers_chamber/bin/pydev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-05-30 14:17:29.000000 skip_developers_chamber-1.5.0/developers_chamber/bitbucket_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:17:35.281627 skip_developers_chamber-1.5.0/developers_chamber/click/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:17:29.000000 skip_developers_chamber-1.5.0/developers_chamber/click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-30 14:17:29.000000 skip_developers_chamber-1.5.0/developers_chamber/click/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-30 14:17:29.000000 skip_developers_chamber-1.5.0/developers_chamber/docker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27455 2024-05-30 14:17:29.000000 skip_developers_chamber-1.5.0/developers_chamber/ecs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-05-30 14:17:29.000000 skip_developers_chamber-1.5.0/developers_chamber/git_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-30 14:17:29.000000 skip_developers_chamber-1.5.0/developers_chamber/gitlab_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-30 14:17:29.000000 skip_developers_chamber-1.5.0/developers_chamber/jira_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10673 2024-05-30 14:17:29.000000 skip_developers_chamber-1.5.0/developers_chamber/project_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:17:35.281627 skip_developers_chamber-1.5.0/developers_chamber/qa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:17:29.000000 skip_developers_chamber-1.5.0/developers_chamber/qa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-05-30 14:17:29.000000 skip_developers_chamber-1.5.0/developers_chamber/qa/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-05-30 14:17:29.000000 skip_developers_chamber-1.5.0/developers_chamber/qa/checks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:17:35.285627 skip_developers_chamber-1.5.0/developers_chamber/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-30 14:17:29.000000 skip_developers_chamber-1.5.0/developers_chamber/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-30 14:17:29.000000 skip_developers_chamber-1.5.0/developers_chamber/scripts/bitbucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-30 14:17:29.000000 skip_developers_chamber-1.5.0/developers_chamber/scripts/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15433 2024-05-30 14:17:29.000000 skip_developers_chamber-1.5.0/developers_chamber/scripts/ecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-05-30 14:17:29.000000 skip_developers_chamber-1.5.0/developers_chamber/scripts/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-30 14:17:29.000000 skip_developers_chamber-1.5.0/developers_chamber/scripts/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-05-30 14:17:29.000000 skip_developers_chamber-1.5.0/developers_chamber/scripts/init_aliasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-05-30 14:17:29.000000 skip_developers_chamber-1.5.0/developers_chamber/scripts/jira.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18907 2024-05-30 14:17:29.000000 skip_developers_chamber-1.5.0/developers_chamber/scripts/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-30 14:17:29.000000 skip_developers_chamber-1.5.0/developers_chamber/scripts/qa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-30 14:17:29.000000 skip_developers_chamber-1.5.0/developers_chamber/scripts/sh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-30 14:17:29.000000 skip_developers_chamber-1.5.0/developers_chamber/scripts/slack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-30 14:17:29.000000 skip_developers_chamber-1.5.0/developers_chamber/scripts/toggle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-30 14:17:29.000000 skip_developers_chamber-1.5.0/developers_chamber/scripts/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-30 14:17:29.000000 skip_developers_chamber-1.5.0/developers_chamber/slack_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-05-30 14:17:29.000000 skip_developers_chamber-1.5.0/developers_chamber/toggle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-30 14:17:29.000000 skip_developers_chamber-1.5.0/developers_chamber/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-05-30 14:17:29.000000 skip_developers_chamber-1.5.0/developers_chamber/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-05-30 14:17:29.000000 skip_developers_chamber-1.5.0/developers_chamber/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 14:17:35.285627 skip_developers_chamber-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-30 14:17:29.000000 skip_developers_chamber-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:17:35.285627 skip_developers_chamber-1.5.0/skip_developers_chamber.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-30 14:17:35.000000 skip_developers_chamber-1.5.0/skip_developers_chamber.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-30 14:17:35.000000 skip_developers_chamber-1.5.0/skip_developers_chamber.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 14:17:35.000000 skip_developers_chamber-1.5.0/skip_developers_chamber.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-30 14:17:35.000000 skip_developers_chamber-1.5.0/skip_developers_chamber.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 14:17:35.000000 skip_developers_chamber-1.5.0/skip_developers_chamber.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-30 14:17:35.000000 skip_developers_chamber-1.5.0/skip_developers_chamber.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-30 14:17:35.000000 skip_developers_chamber-1.5.0/skip_developers_chamber.egg-info/top_level.txt
```

### Comparing `skip-developers-chamber-1.4.0/LICENSE` & `skip_developers_chamber-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.4.0/PKG-INFO` & `skip_developers_chamber-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-developers-chamber
-Version: 1.4.0
+Version: 1.5.0
 Summary: A small plugin which help with development, deployment, git
 Home-page: https://github.com/skip-pay/developers-chamber
 Author: Druids team
 Author-email: matllubos@gmail.com
 License: MIT
 Keywords: django,skripts,easy live,git,bitbucket,Jira
 License-File: LICENSE
```

### Comparing `skip-developers-chamber-1.4.0/README.md` & `skip_developers_chamber-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.4.0/developers_chamber/bin/pydev.py` & `skip_developers_chamber-1.5.0/developers_chamber/bin/pydev.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.4.0/developers_chamber/bitbucket_utils.py` & `skip_developers_chamber-1.5.0/developers_chamber/bitbucket_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.4.0/developers_chamber/click/options.py` & `skip_developers_chamber-1.5.0/developers_chamber/click/options.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.4.0/developers_chamber/ecs_utils.py` & `skip_developers_chamber-1.5.0/developers_chamber/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.4.0/developers_chamber/git_utils.py` & `skip_developers_chamber-1.5.0/developers_chamber/git_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.4.0/developers_chamber/gitlab_utils.py` & `skip_developers_chamber-1.5.0/developers_chamber/gitlab_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.4.0/developers_chamber/jira_utils.py` & `skip_developers_chamber-1.5.0/developers_chamber/jira_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.4.0/developers_chamber/project_utils.py` & `skip_developers_chamber-1.5.0/developers_chamber/project_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.4.0/developers_chamber/qa/base.py` & `skip_developers_chamber-1.5.0/developers_chamber/qa/base.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.4.0/developers_chamber/qa/checks.py` & `skip_developers_chamber-1.5.0/developers_chamber/qa/checks.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.4.0/developers_chamber/scripts/bitbucket.py` & `skip_developers_chamber-1.5.0/developers_chamber/scripts/bitbucket.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.4.0/developers_chamber/scripts/docker.py` & `skip_developers_chamber-1.5.0/developers_chamber/scripts/docker.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.4.0/developers_chamber/scripts/ecs.py` & `skip_developers_chamber-1.5.0/developers_chamber/scripts/ecs.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.4.0/developers_chamber/scripts/git.py` & `skip_developers_chamber-1.5.0/developers_chamber/scripts/git.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.4.0/developers_chamber/scripts/gitlab.py` & `skip_developers_chamber-1.5.0/developers_chamber/scripts/gitlab.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.4.0/developers_chamber/scripts/init_aliasses.py` & `skip_developers_chamber-1.5.0/developers_chamber/scripts/init_aliasses.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.4.0/developers_chamber/scripts/jira.py` & `skip_developers_chamber-1.5.0/developers_chamber/scripts/jira.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.4.0/developers_chamber/scripts/project.py` & `skip_developers_chamber-1.5.0/developers_chamber/scripts/project.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.4.0/developers_chamber/scripts/qa.py` & `skip_developers_chamber-1.5.0/developers_chamber/scripts/qa.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.4.0/developers_chamber/scripts/slack.py` & `skip_developers_chamber-1.5.0/developers_chamber/scripts/slack.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.4.0/developers_chamber/scripts/toggle.py` & `skip_developers_chamber-1.5.0/developers_chamber/scripts/toggle.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.4.0/developers_chamber/scripts/version.py` & `skip_developers_chamber-1.5.0/developers_chamber/scripts/version.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.4.0/developers_chamber/slack_utils.py` & `skip_developers_chamber-1.5.0/developers_chamber/slack_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 
     def __init__(self, token, channel, target_branch, migrations_pattern):
         self.client = WebClient(token=token)
         self.channel = channel
         self.target_branch = target_branch
         self.migrations_pattern = r'{}'.format(migrations_pattern)
         self.active_branch = self._get_active_branch_name()
+        self.repo = self._get_repo()
 
     def _get_migration_files(self):
-        return [diff.b_path for diff in self._get_diffs(target_branch=self.target_branch)
+        return [diff.b_path for diff in self.repo.commit(self.target_branch).diff(self.active_branch, create_patch=True)
                 if diff.new_file and re.search(self.migrations_pattern, diff.b_path)]
 
     def send_message(self, msg):
         self.client.chat_postMessage(channel=self.channel, text=msg)
 
     def upload_file(self, file):
         self.client.files_upload(channels=self.channel, file=file, title=file)
```

### Comparing `skip-developers-chamber-1.4.0/developers_chamber/toggle_utils.py` & `skip_developers_chamber-1.5.0/developers_chamber/toggle_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.4.0/developers_chamber/types.py` & `skip_developers_chamber-1.5.0/developers_chamber/types.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.4.0/developers_chamber/utils.py` & `skip_developers_chamber-1.5.0/developers_chamber/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import subprocess
 import sys
 
 from click import ClickException
 from git import Repo
 
 LOGGER = logging.getLogger()
-MIGRATIONS_PATTERN = r'migrations\/([^\/]+)\.py$'
+MIGRATIONS_PATTERN = r'\d+_migration\.py$'
 
 
 def call_command(command, quiet=False, env=None):
     env = {} if env is None else env
     try:
         if not quiet:
             LOGGER.info(command if isinstance(command, str) else ' '.join(command))
```

### Comparing `skip-developers-chamber-1.4.0/developers_chamber/version_utils.py` & `skip_developers_chamber-1.5.0/developers_chamber/version_utils.py`

 * *Files identical despite different names*

### Comparing `skip-developers-chamber-1.4.0/setup.py` & `skip_developers_chamber-1.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='skip-developers-chamber',
-    version='1.4.0',
+    version='1.5.0',
     description='A small plugin which help with development, deployment, git',
     keywords='django, skripts, easy live, git, bitbucket, Jira',
     author='Druids team',
     author_email='matllubos@gmail.com',
     url='https://github.com/skip-pay/developers-chamber',
     license='MIT',
     package_dir={'developers_chamber': 'developers_chamber'},
```

### Comparing `skip-developers-chamber-1.4.0/skip_developers_chamber.egg-info/PKG-INFO` & `skip_developers_chamber-1.5.0/skip_developers_chamber.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-developers-chamber
-Version: 1.4.0
+Version: 1.5.0
 Summary: A small plugin which help with development, deployment, git
 Home-page: https://github.com/skip-pay/developers-chamber
 Author: Druids team
 Author-email: matllubos@gmail.com
 License: MIT
 Keywords: django,skripts,easy live,git,bitbucket,Jira
 License-File: LICENSE
```

### Comparing `skip-developers-chamber-1.4.0/skip_developers_chamber.egg-info/SOURCES.txt` & `skip_developers_chamber-1.5.0/skip_developers_chamber.egg-info/SOURCES.txt`

 * *Files identical despite different names*

