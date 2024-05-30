# Comparing `tmp/python-gerrit-api-3.0.7.tar.gz` & `tmp/python_gerrit_api-3.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-gerrit-api-3.0.7.tar", last modified: Tue Apr  2 06:01:25 2024, max compression
+gzip compressed data, was "python_gerrit_api-3.0.8.tar", last modified: Thu May 30 03:38:31 2024, max compression
```

## Comparing `python-gerrit-api-3.0.7.tar` & `python_gerrit_api-3.0.8.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:01:25.883339 python-gerrit-api-3.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12073 2024-04-02 06:01:25.883339 python-gerrit-api-3.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11119 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:01:25.875339 python-gerrit-api-3.0.7/gerrit/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:01:25.875339 python-gerrit-api-3.0.7/gerrit/accounts/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18444 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/accounts/account.py
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/accounts/accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/accounts/emails.py
--rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/accounts/gpg_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/accounts/ssh_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:01:25.875339 python-gerrit-api-3.0.7/gerrit/changes/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/changes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27591 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/changes/change.py
--rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/changes/changes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/changes/comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/changes/drafts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/changes/edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6997 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/changes/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/changes/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/changes/reviewers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12881 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/changes/revision.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:01:25.879339 python-gerrit-api-3.0.7/gerrit/config/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/config/caches.py
--rw-r--r--   0 runner    (1001) docker     (127)     7303 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/config/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:01:25.879339 python-gerrit-api-3.0.7/gerrit/groups/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/groups/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/groups/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/groups/members.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/groups/subgroups.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:01:25.879339 python-gerrit-api-3.0.7/gerrit/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/plugins/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:01:25.879339 python-gerrit-api-3.0.7/gerrit/projects/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/projects/branches.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/projects/commit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/projects/dashboards.py
--rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/projects/labels.py
--rw-r--r--   0 runner    (1001) docker     (127)    14123 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/projects/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/projects/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/projects/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/projects/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:01:25.883339 python-gerrit-api-3.0.7/gerrit/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/utils/gerritbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     8703 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gerrit/utils/requester.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:01:25.883339 python-gerrit-api-3.0.7/gitiles/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gitiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/gitiles/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:01:25.883339 python-gerrit-api-3.0.7/python_gerrit_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12073 2024-04-02 06:01:25.000000 python-gerrit-api-3.0.7/python_gerrit_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-02 06:01:25.000000 python-gerrit-api-3.0.7/python_gerrit_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 06:01:25.000000 python-gerrit-api-3.0.7/python_gerrit_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 06:01:25.000000 python-gerrit-api-3.0.7/python_gerrit_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-02 06:01:25.000000 python-gerrit-api-3.0.7/python_gerrit_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 06:01:25.887339 python-gerrit-api-3.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:01:25.883339 python-gerrit-api-3.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7679 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/tests/test_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/tests/test_changes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/tests/test_gitiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/tests/test_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    11540 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/tests/test_projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-04-02 06:01:21.000000 python-gerrit-api-3.0.7/tests/test_revision.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:38:31.315355 python_gerrit_api-3.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12073 2024-05-30 03:38:31.315355 python_gerrit_api-3.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11119 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:38:31.303355 python_gerrit_api-3.0.8/gerrit/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:38:31.307355 python_gerrit_api-3.0.8/gerrit/accounts/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18444 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/accounts/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/accounts/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/accounts/emails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/accounts/gpg_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/accounts/ssh_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:38:31.307355 python_gerrit_api-3.0.8/gerrit/changes/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/changes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27591 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/changes/change.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/changes/changes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/changes/comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/changes/drafts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/changes/edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6997 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/changes/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/changes/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/changes/reviewers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12881 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/changes/revision.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:38:31.307355 python_gerrit_api-3.0.8/gerrit/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/config/caches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7303 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/config/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:38:31.307355 python_gerrit_api-3.0.8/gerrit/groups/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/groups/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/groups/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/groups/members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/groups/subgroups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:38:31.307355 python_gerrit_api-3.0.8/gerrit/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/plugins/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:38:31.311355 python_gerrit_api-3.0.8/gerrit/projects/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/projects/branches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/projects/commit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/projects/dashboards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/projects/labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14123 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/projects/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/projects/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/projects/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/projects/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:38:31.311355 python_gerrit_api-3.0.8/gerrit/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/utils/gerritbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7973 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gerrit/utils/requester.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:38:31.311355 python_gerrit_api-3.0.8/gitiles/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gitiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/gitiles/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:38:31.315355 python_gerrit_api-3.0.8/python_gerrit_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12073 2024-05-30 03:38:31.000000 python_gerrit_api-3.0.8/python_gerrit_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-30 03:38:31.000000 python_gerrit_api-3.0.8/python_gerrit_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 03:38:31.000000 python_gerrit_api-3.0.8/python_gerrit_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-30 03:38:31.000000 python_gerrit_api-3.0.8/python_gerrit_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-30 03:38:31.000000 python_gerrit_api-3.0.8/python_gerrit_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 03:38:31.315355 python_gerrit_api-3.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:38:31.315355 python_gerrit_api-3.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7679 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/tests/test_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/tests/test_changes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/tests/test_gitiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/tests/test_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11540 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/tests/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-05-30 03:38:27.000000 python_gerrit_api-3.0.8/tests/test_revision.py
```

### Comparing `python-gerrit-api-3.0.7/LICENSE` & `python_gerrit_api-3.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/PKG-INFO` & `python_gerrit_api-3.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-gerrit-api
-Version: 3.0.7
+Version: 3.0.8
 Summary: Python wrapper for the Gerrit REST API.
 Home-page: https://github.com/shijl0925/python-gerrit-api
 Author: Jialiang Shi
 Author-email: kevin09254930sjl@gmail.com
 License: MIT
 Keywords: api gerrit client wrapper
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `python-gerrit-api-3.0.7/README.rst` & `python_gerrit_api-3.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/gerrit/accounts/account.py` & `python_gerrit_api-3.0.8/gerrit/accounts/account.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/gerrit/accounts/accounts.py` & `python_gerrit_api-3.0.8/gerrit/accounts/accounts.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/gerrit/accounts/emails.py` & `python_gerrit_api-3.0.8/gerrit/accounts/emails.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/gerrit/accounts/gpg_keys.py` & `python_gerrit_api-3.0.8/gerrit/accounts/gpg_keys.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/gerrit/accounts/ssh_keys.py` & `python_gerrit_api-3.0.8/gerrit/accounts/ssh_keys.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/gerrit/base.py` & `python_gerrit_api-3.0.8/gerrit/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
 import netrc
+import requests
+from requests.adapters import HTTPAdapter
 from gerrit.utils.requester import Requester
 from gerrit.utils.common import decode_response, strip_trailing_slash
 from gerrit.config.config import GerritConfig
 from gerrit.projects.projects import GerritProjects
 from gerrit.accounts.accounts import GerritAccounts
 from gerrit.groups.groups import GerritGroups
 from gerrit.plugins.plugins import GerritPlugins
@@ -33,22 +35,36 @@
         auth_suffix="/a",
     ):
         self._base_url = strip_trailing_slash(base_url)
 
         if use_netrc:
             password = self.get_password_from_netrc_file()
 
+        # make request session
+        _session = requests.Session()
+        if username and password:
+            _session.auth = (username, password)
+
+        if ssl_verify:
+            _session.verify = ssl_verify
+
+        if cert is not None:
+            _session.cert = cert
+
+        if max_retries is not None:
+            retry_adapter = HTTPAdapter(max_retries=max_retries)
+            _session.mount("http://", retry_adapter)
+            _session.mount("https://", retry_adapter)
+
+        self.session = _session
+
         self.requester = Requester(
             base_url=base_url,
-            username=username,
-            password=password,
-            ssl_verify=ssl_verify,
-            cert=cert,
+            session=self.session,
             timeout=timeout,
-            max_retries=max_retries,
         )
         if username and password:
             self.auth_suffix = auth_suffix
         else:
             self.auth_suffix = ""
 
     def get_password_from_netrc_file(self):
```

### Comparing `python-gerrit-api-3.0.7/gerrit/changes/change.py` & `python_gerrit_api-3.0.8/gerrit/changes/change.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/gerrit/changes/changes.py` & `python_gerrit_api-3.0.8/gerrit/changes/changes.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
             result = self.gerrit.get(endpoint)
 
             id = result.get("id")
             return GerritChange(id=id, gerrit=self.gerrit)
         except requests.exceptions.HTTPError as error:
             if error.response.status_code == 404:
                 message = f"Change {id_} does not exist"
-                if id_.startswith("I"):
+                if isinstance(id_, str) and id_.startswith("I"):
                     res = self.search(query=f"change: {id_}")
                     if len(res) > 0:
                         change_ids = [item.get("id") for item in res]
                         message = f"Change {id_} query multiple changes: {', '.join(change_ids)}, which one do you want?"
 
                 logger.error(message)
                 raise ChangeNotFoundError(message)
```

### Comparing `python-gerrit-api-3.0.7/gerrit/changes/comments.py` & `python_gerrit_api-3.0.8/gerrit/changes/comments.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/gerrit/changes/drafts.py` & `python_gerrit_api-3.0.8/gerrit/changes/drafts.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/gerrit/changes/edit.py` & `python_gerrit_api-3.0.8/gerrit/changes/edit.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/gerrit/changes/files.py` & `python_gerrit_api-3.0.8/gerrit/changes/files.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/gerrit/changes/messages.py` & `python_gerrit_api-3.0.8/gerrit/changes/messages.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/gerrit/changes/reviewers.py` & `python_gerrit_api-3.0.8/gerrit/changes/reviewers.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/gerrit/changes/revision.py` & `python_gerrit_api-3.0.8/gerrit/changes/revision.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/gerrit/config/caches.py` & `python_gerrit_api-3.0.8/gerrit/config/caches.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/gerrit/config/config.py` & `python_gerrit_api-3.0.8/gerrit/config/config.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/gerrit/config/tasks.py` & `python_gerrit_api-3.0.8/gerrit/config/tasks.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/gerrit/groups/group.py` & `python_gerrit_api-3.0.8/gerrit/groups/group.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/gerrit/groups/groups.py` & `python_gerrit_api-3.0.8/gerrit/groups/groups.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/gerrit/groups/members.py` & `python_gerrit_api-3.0.8/gerrit/groups/members.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/gerrit/groups/subgroups.py` & `python_gerrit_api-3.0.8/gerrit/groups/subgroups.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/gerrit/plugins/plugins.py` & `python_gerrit_api-3.0.8/gerrit/plugins/plugins.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/gerrit/projects/branches.py` & `python_gerrit_api-3.0.8/gerrit/projects/branches.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/gerrit/projects/commit.py` & `python_gerrit_api-3.0.8/gerrit/projects/commit.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/gerrit/projects/dashboards.py` & `python_gerrit_api-3.0.8/gerrit/projects/dashboards.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/gerrit/projects/labels.py` & `python_gerrit_api-3.0.8/gerrit/projects/labels.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/gerrit/projects/project.py` & `python_gerrit_api-3.0.8/gerrit/projects/project.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/gerrit/projects/projects.py` & `python_gerrit_api-3.0.8/gerrit/projects/projects.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/gerrit/projects/tags.py` & `python_gerrit_api-3.0.8/gerrit/projects/tags.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/gerrit/projects/webhooks.py` & `python_gerrit_api-3.0.8/gerrit/projects/webhooks.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/gerrit/utils/common.py` & `python_gerrit_api-3.0.8/gerrit/utils/common.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/gerrit/utils/exceptions.py` & `python_gerrit_api-3.0.8/gerrit/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/gerrit/utils/gerritbase.py` & `python_gerrit_api-3.0.8/gerrit/utils/gerritbase.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/gerrit/utils/requester.py` & `python_gerrit_api-3.0.8/gerrit/utils/requester.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
 import urllib.parse as urlparse
-from requests import Session
-from requests.adapters import HTTPAdapter
 from gerrit.utils.exceptions import (
     NotAllowedError,
     ValidationError,
     AuthError,
     UnauthorizedError,
     ConflictError,
     ClientError,
@@ -32,26 +30,16 @@
     def __init__(self, **kwargs):
         """
         :param kwargs:
         """
         timeout = 10
         base_url = kwargs.get("base_url")
         self.base_scheme = urlparse.urlsplit(base_url).scheme if base_url else None
-        self.username = kwargs.get("username")
-        self.password = kwargs.get("password")
-        self.ssl_verify = kwargs.get("ssl_verify")
-        self.cert = kwargs.get("cert")
+        self.session = kwargs.get("session")
         self.timeout = kwargs.get("timeout", timeout)
-        self.session = Session()
-
-        self.max_retries = kwargs.get("max_retries")
-        if self.max_retries is not None:
-            retry_adapter = HTTPAdapter(max_retries=self.max_retries)
-            self.session.mount("http://", retry_adapter)
-            self.session.mount("https://", retry_adapter)
 
     def _update_url_scheme(self, url):
         """
         Updates scheme of given url to the one used in Gerrit base_url.
         """
         if self.base_scheme and not url.startswith(f"{self.base_scheme}://"):
             url_split = urlparse.urlsplit(url)
@@ -74,16 +62,14 @@
         :param data:
         :param json:
         :param headers:
         :param kwargs:
         :return:
         """
         request_kwargs = kwargs
-        if self.username and self.password:
-            request_kwargs["auth"] = (self.username, self.password)
 
         if params:
             if not isinstance(params, dict):
                 raise ValueError(f"Params must be a dict, got {repr(params)}")
 
             request_kwargs["params"] = params
 
@@ -94,17 +80,14 @@
             request_kwargs["headers"] = headers
 
         if self.AUTH_COOKIE:
             currentheaders = request_kwargs.get("headers", {})
             currentheaders.update({"Cookie": self.AUTH_COOKIE})
             request_kwargs["headers"] = currentheaders
 
-        request_kwargs["verify"] = self.ssl_verify
-        request_kwargs["cert"] = self.cert
-
         if data and json:
             raise ValueError("Cannot use data and json together")
 
         if data:
             request_kwargs["data"] = data
 
         if json:
```

### Comparing `python-gerrit-api-3.0.7/gitiles/base.py` & `python_gerrit_api-3.0.8/gitiles/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # @Author: Jialiang Shi
 from typing import Optional
 from base64 import b64decode
+import requests
+from requests.adapters import HTTPAdapter
 from gerrit.utils.requester import Requester
 from gerrit.utils.common import decode_response, strip_trailing_slash
 
 
 class GitilesClient:
     def __init__(
         self,
@@ -16,22 +18,36 @@
         ssl_verify=True,
         cert=None,
         timeout=60,
         max_retries=None,
     ):
         self._base_url = strip_trailing_slash(base_url)
 
+        # make request session
+        _session = requests.Session()
+        if username and password:
+            _session.auth = (username, password)
+
+        if ssl_verify:
+            _session.verify = ssl_verify
+
+        if cert is not None:
+            _session.cert = cert
+
+        if max_retries is not None:
+            retry_adapter = HTTPAdapter(max_retries=max_retries)
+            _session.mount("http://", retry_adapter)
+            _session.mount("https://", retry_adapter)
+
+        self.session = _session
+
         self.requester = Requester(
             base_url=base_url,
-            username=username,
-            password=password,
-            ssl_verify=ssl_verify,
-            cert=cert,
+            session=self.session,
             timeout=timeout,
-            max_retries=max_retries,
         )
 
     def get_endpoint_url(self, endpoint):
         """
         Return the complete url including host and port for a given endpoint.
         :param endpoint: service endpoint as str
         :return: complete url (including host and port) as str
```

### Comparing `python-gerrit-api-3.0.7/python_gerrit_api.egg-info/PKG-INFO` & `python_gerrit_api-3.0.8/python_gerrit_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-gerrit-api
-Version: 3.0.7
+Version: 3.0.8
 Summary: Python wrapper for the Gerrit REST API.
 Home-page: https://github.com/shijl0925/python-gerrit-api
 Author: Jialiang Shi
 Author-email: kevin09254930sjl@gmail.com
 License: MIT
 Keywords: api gerrit client wrapper
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `python-gerrit-api-3.0.7/python_gerrit_api.egg-info/SOURCES.txt` & `python_gerrit_api-3.0.8/python_gerrit_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/setup.py` & `python_gerrit_api-3.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/tests/test_accounts.py` & `python_gerrit_api-3.0.8/tests/test_accounts.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/tests/test_changes.py` & `python_gerrit_api-3.0.8/tests/test_changes.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/tests/test_gitiles.py` & `python_gerrit_api-3.0.8/tests/test_gitiles.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/tests/test_groups.py` & `python_gerrit_api-3.0.8/tests/test_groups.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/tests/test_projects.py` & `python_gerrit_api-3.0.8/tests/test_projects.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.7/tests/test_revision.py` & `python_gerrit_api-3.0.8/tests/test_revision.py`

 * *Files identical despite different names*

