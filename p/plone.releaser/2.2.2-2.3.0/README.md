# Comparing `tmp/plone.releaser-2.2.2.tar.gz` & `tmp/plone_releaser-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.releaser-2.2.2.tar", last modified: Tue Apr 16 19:35:35 2024, max compression
+gzip compressed data, was "plone_releaser-2.3.0.tar", last modified: Thu May 30 18:20:14 2024, max compression
```

## Comparing `plone.releaser-2.2.2.tar` & `plone_releaser-2.3.0.tar`

### file list

```diff
@@ -1,55 +1,60 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:35:35.333778 plone.releaser-2.2.2/
--rw-r--r--   0 maurits    (501) staff       (20)     3287 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/ADD-A-NEWS-ITEM.rst
--rw-r--r--   0 maurits    (501) staff       (20)     8279 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      142 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    10008 2024-04-16 19:35:35.333222 plone.releaser-2.2.2/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      713 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)      108 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/buildout.cfg
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:35:35.319175 plone.releaser-2.2.2/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:35:35.325382 plone.releaser-2.2.2/plone/releaser/
--rw-r--r--   0 maurits    (501) staff       (20)      940 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1752 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/base.py
--rw-r--r--   0 maurits    (501) staff       (20)    17582 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/buildout.py
--rw-r--r--   0 maurits    (501) staff       (20)    11798 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/changelog.py
--rw-r--r--   0 maurits    (501) staff       (20)      772 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/db.py
--rw-r--r--   0 maurits    (501) staff       (20)    11110 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/manage.py
--rw-r--r--   0 maurits    (501) staff       (20)    10899 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/package.py
--rw-r--r--   0 maurits    (501) staff       (20)    10703 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/pip.py
--rw-r--r--   0 maurits    (501) staff       (20)      701 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/pypi.py
--rw-r--r--   0 maurits    (501) staff       (20)    10440 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/release.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:35:35.327498 plone.releaser-2.2.2/plone/releaser/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/tests/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:35:35.332051 plone.releaser-2.2.2/plone/releaser/tests/input/
--rw-r--r--   0 maurits    (501) staff       (20)      465 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/tests/input/changes.md
--rw-r--r--   0 maurits    (501) staff       (20)      975 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/tests/input/changes.rst
--rw-r--r--   0 maurits    (501) staff       (20)      145 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/tests/input/checkouts.cfg
--rw-r--r--   0 maurits    (501) staff       (20)      313 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/tests/input/constraints.txt
--rw-r--r--   0 maurits    (501) staff       (20)       73 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/tests/input/constraints2.txt
--rw-r--r--   0 maurits    (501) staff       (20)       75 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/tests/input/constraints3.txt
--rw-r--r--   0 maurits    (501) staff       (20)       49 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/tests/input/constraints4.txt
--rw-r--r--   0 maurits    (501) staff       (20)      460 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/tests/input/mxdev.ini
--rw-r--r--   0 maurits    (501) staff       (20)      774 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/tests/input/sources.cfg
--rw-r--r--   0 maurits    (501) staff       (20)      408 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/tests/input/versions.cfg
--rw-r--r--   0 maurits    (501) staff       (20)      101 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/tests/input/versions2.cfg
--rw-r--r--   0 maurits    (501) staff       (20)      107 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/tests/input/versions3.cfg
--rw-r--r--   0 maurits    (501) staff       (20)       52 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/tests/input/versions4.cfg
--rw-r--r--   0 maurits    (501) staff       (20)    18176 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/tests/test_buildout.py
--rw-r--r--   0 maurits    (501) staff       (20)     1900 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/tests/test_changelog.py
--rw-r--r--   0 maurits    (501) staff       (20)    12684 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/tests/test_pip.py
--rw-r--r--   0 maurits    (501) staff       (20)     3008 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/tests/test_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     1137 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/tests/test_versions2constraints.py
--rw-r--r--   0 maurits    (501) staff       (20)     4812 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/utils.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:35:35.332482 plone.releaser-2.2.2/plone.releaser.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    10008 2024-04-16 19:35:35.000000 plone.releaser-2.2.2/plone.releaser.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1472 2024-04-16 19:35:35.000000 plone.releaser-2.2.2/plone.releaser.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-16 19:35:35.000000 plone.releaser-2.2.2/plone.releaser.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)      706 2024-04-16 19:35:35.000000 plone.releaser-2.2.2/plone.releaser.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2024-04-16 19:35:35.000000 plone.releaser-2.2.2/plone.releaser.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-16 19:35:35.000000 plone.releaser-2.2.2/plone.releaser.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      143 2024-04-16 19:35:35.000000 plone.releaser-2.2.2/plone.releaser.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2024-04-16 19:35:35.000000 plone.releaser-2.2.2/plone.releaser.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4271 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)       38 2024-04-16 19:35:35.333866 plone.releaser-2.2.2/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2573 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:20:14.258365 plone_releaser-2.3.0/
+-rw-r--r--   0 maurits    (501) staff       (20)     3287 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/ADD-A-NEWS-ITEM.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     8868 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      142 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    12306 2024-05-30 18:20:14.257680 plone_releaser-2.3.0/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     2422 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      108 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/buildout.cfg
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:20:14.235765 plone_releaser-2.3.0/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:20:14.244931 plone_releaser-2.3.0/plone/releaser/
+-rw-r--r--   0 maurits    (501) staff       (20)      940 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/plone/releaser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4953 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/plone/releaser/base.py
+-rw-r--r--   0 maurits    (501) staff       (20)    17620 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/plone/releaser/buildout.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11798 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/plone/releaser/changelog.py
+-rw-r--r--   0 maurits    (501) staff       (20)      772 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/plone/releaser/db.py
+-rw-r--r--   0 maurits    (501) staff       (20)    12483 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/plone/releaser/manage.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10899 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/plone/releaser/package.py
+-rw-r--r--   0 maurits    (501) staff       (20)    12721 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/plone/releaser/pip.py
+-rw-r--r--   0 maurits    (501) staff       (20)      701 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/plone/releaser/pypi.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10062 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/plone/releaser/release.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:20:14.249605 plone_releaser-2.3.0/plone/releaser/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/plone/releaser/tests/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:20:14.255972 plone_releaser-2.3.0/plone/releaser/tests/input/
+-rw-r--r--   0 maurits    (501) staff       (20)      465 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/plone/releaser/tests/input/changes.md
+-rw-r--r--   0 maurits    (501) staff       (20)      975 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/plone/releaser/tests/input/changes.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      145 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/plone/releaser/tests/input/checkouts.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)      313 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/plone/releaser/tests/input/constraints.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       73 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/plone/releaser/tests/input/constraints2.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       75 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/plone/releaser/tests/input/constraints3.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       49 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/plone/releaser/tests/input/constraints4.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       77 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/plone/releaser/tests/input/mxcheckouts.ini
+-rw-r--r--   0 maurits    (501) staff       (20)      477 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/plone/releaser/tests/input/mxsources.ini
+-rw-r--r--   0 maurits    (501) staff       (20)      774 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/plone/releaser/tests/input/sources.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)      408 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/plone/releaser/tests/input/versions.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)      101 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/plone/releaser/tests/input/versions2.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)      107 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/plone/releaser/tests/input/versions3.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)       52 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/plone/releaser/tests/input/versions4.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)    16643 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/plone/releaser/tests/test_buildout.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2992 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/plone/releaser/tests/test_buildout2pip.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1900 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/plone/releaser/tests/test_changelog.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3361 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/plone/releaser/tests/test_mxdev_checkouts.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2592 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/plone/releaser/tests/test_mxdev_sources.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9410 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/plone/releaser/tests/test_pip.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2598 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/plone/releaser/tests/test_source.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3008 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/plone/releaser/tests/test_utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4102 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/plone/releaser/tests/test_versions2constraints.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4812 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/plone/releaser/utils.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:20:14.256538 plone_releaser-2.3.0/plone.releaser.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    12306 2024-05-30 18:20:14.000000 plone_releaser-2.3.0/plone.releaser.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1685 2024-05-30 18:20:14.000000 plone_releaser-2.3.0/plone.releaser.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-05-30 18:20:14.000000 plone_releaser-2.3.0/plone.releaser.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      706 2024-05-30 18:20:14.000000 plone_releaser-2.3.0/plone.releaser.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-05-30 18:20:14.000000 plone_releaser-2.3.0/plone.releaser.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-05-30 18:20:14.000000 plone_releaser-2.3.0/plone.releaser.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      143 2024-05-30 18:20:14.000000 plone_releaser-2.3.0/plone.releaser.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-05-30 18:20:14.000000 plone_releaser-2.3.0/plone.releaser.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4446 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2024-05-30 18:20:14.258494 plone_releaser-2.3.0/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2573 2024-05-30 18:20:13.000000 plone_releaser-2.3.0/setup.py
```

### Comparing `plone.releaser-2.2.2/ADD-A-NEWS-ITEM.rst` & `plone_releaser-2.3.0/ADD-A-NEWS-ITEM.rst`

 * *Files identical despite different names*

### Comparing `plone.releaser-2.2.2/CHANGES.rst` & `plone_releaser-2.3.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,42 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.3.0 (2024-05-30)
+------------------
+
+New features:
+
+
+- Add buildout2pip manage command.
+  [maurits] (#72)
+
+
+Bug fixes:
+
+
+- Catch error when trying to change coredev branches.
+  Not everyone may have the branches available, or there may be some problem with it. (#67)
+- No longer offer to push changes to buildout.coredev.
+  This is no longer what we ever want: the newly uploaded package will not yet be available on all PyPI mirrors.
+  Fixes `issue 69 <https://github.com/plone/plone.releaser/issues/69>`_.
+  [maurits] (#69)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs]
+
+
 2.2.2 (2024-04-16)
 ------------------
 
 Bug fixes:
 
 
 - Preserve the case of package names in versions2constraints and friends.
```

### Comparing `plone.releaser-2.2.2/PKG-INFO` & `plone_releaser-2.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.releaser
-Version: 2.2.2
+Version: 2.3.0
 Summary: Plone release management utilities
 Home-page: https://github.com/plone/plone.releaser
 Author: Eric Steele
 Author-email: eric@esteele.net
 License: GPL
 Keywords: plone release
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,30 +28,67 @@
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
 Introduction
 ============
 
 Tools to make managing Plone core releases easier.
+It is a wrapper around ``zest.releaser``, plus it adds some commands.
+
+WARNING: this package is only meant for development of core Plone.
+It may have useful bits for others, but we may drop features and edge cases at any time if it is no longer useful for Plone.
+
 
 Installation
 ------------
 
-To install plone.releaser add it to your buildout::
+Do ``pip install plone.releaser`` or add it to your buildout::
 
   [release]
   recipe = zc.recipe.egg
-  eggs =  plone.releaser
+  eggs = plone.releaser
+
+
+Main usage: release a package
+-----------------------------
+
+In  the `Plone core development buildout <https://github.com/plone/buildout.coredev>`_ go to ``src/some.package`` and run ``../../bin/fullrelease``.
+This calls the ``fullrelease`` command from ``zest.releaser``, but with some extra hooks and packages available.
+
+One nice thing it does: look in the checkouts and sources of your ``buildout.coredev`` checkout and update them:
+remove the released package from the checkouts and update the version.
+
+If you are working on branch 6.1 of coredev, then we check if you also have branches 5.2 and 6.0 checked out.
+There we check if the branch of the released package is in the sources.
+If you make a release from package branch ``main`` and this is the branch used in the sources, then we update the checkouts and sources of this coredev branch as well.
+
+After releasing a package, you should wait a few minutes before you manually push the changes to all coredev branches.
+This gives the PyPI mirrors time to catch up so the new release is available, so Jenkins and GitHub Actions can find it.
+
 
-To make it available in buildout.coredev, run buildout with releaser.cfg::
+Main commands
+-------------
 
-  $ bin/buildout -c releaser.cfg
+Take several Buildout files and create pip/mxdev files out of them::
 
-Usage
------
+  $ bin/manage buildout2pip
+
+Take a Buildout versions file and create a pip constraints file out of it.
+
+  $ bin/manage versions2constraints
+
+Generate a changelog with changes from all packages since a certain Plone release::
+
+  $ bin/manage changelog --start=6.1.0a1
+
+
+Other commands
+--------------
+
+Some commands are not used much (by Maurits anyway) because they are less needed these days.
 
 Check PyPi access to all Plone packages for a certain user::
 
   $ bin/manage checkPypi timo
 
 Check a package for updates::
 
@@ -61,32 +98,56 @@
 
   $ bin/manage report --interactive
 
 Pulls::
 
   $ bin/manage pulls
 
-Changelog::
-
-  $ bin/manage changelog
-
 Check checkout::
 
   $ bin/manage check-checkout
 
 Changelog
 =========
 
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.3.0 (2024-05-30)
+------------------
+
+New features:
+
+
+- Add buildout2pip manage command.
+  [maurits] (#72)
+
+
+Bug fixes:
+
+
+- Catch error when trying to change coredev branches.
+  Not everyone may have the branches available, or there may be some problem with it. (#67)
+- No longer offer to push changes to buildout.coredev.
+  This is no longer what we ever want: the newly uploaded package will not yet be available on all PyPI mirrors.
+  Fixes `issue 69 <https://github.com/plone/plone.releaser/issues/69>`_.
+  [maurits] (#69)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs]
+
+
 2.2.2 (2024-04-16)
 ------------------
 
 Bug fixes:
 
 
 - Preserve the case of package names in versions2constraints and friends.
```

### Comparing `plone.releaser-2.2.2/plone/releaser/__init__.py` & `plone_releaser-2.3.0/plone/releaser/__init__.py`

 * *Files identical despite different names*

### Comparing `plone.releaser-2.2.2/plone/releaser/buildout.py` & `plone_releaser-2.3.0/plone/releaser/buildout.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,78 +1,23 @@
 from .base import BaseFile
+from .base import Source
 from .utils import buildout_marker_to_pip_marker
 from .utils import update_contents
 from collections import defaultdict
 from collections import OrderedDict
 from configparser import ConfigParser
 from configparser import ExtendedInterpolation
 from functools import cached_property
 from textwrap import indent
 
 import os
 import pathlib
 import re
 
 
-class Source:
-    """Source definition for mr.developer"""
-
-    def __init__(
-        self, protocol=None, url=None, pushurl=None, branch=None, path=None, egg=True
-    ):
-        # I think mxdev only supports git as protocol.
-        self.protocol = protocol
-        self.url = url
-        self.pushurl = pushurl
-        self.branch = branch
-        # mxdev has target (default: sources) instead of path (default: src).
-        self.path = path
-        # egg=True: mxdev install-mode="direct"
-        # egg=False: mxdev install-mode="skip"
-        self.egg = egg
-
-    @classmethod
-    def create_from_string(cls, source_string):
-        line_options = source_string.split()
-        protocol = line_options.pop(0)
-        url = line_options.pop(0)
-        # September 2023: mr.developer defaults to master, mxdev to main.
-        options = {"protocol": protocol, "url": url, "branch": "master"}
-
-        # The rest of the line options are key/value pairs.
-        for param in line_options:
-            if param is not None:
-                key, value = param.split("=")
-                if key == "egg":
-                    if value.lower() in ("true", "yes", "on"):
-                        value = True
-                    elif value.lower() in ("false", "no", "off"):
-                        value = False
-                options[key] = value
-        return cls(**options)
-
-    def __repr__(self):
-        return f"<Source {self.protocol} url={self.url} pushurl={self.pushurl} branch={self.branch} path={self.path} egg={self.egg}>"
-
-    def __str__(self):
-        line = f"{self.protocol} {self.url}"
-        if self.pushurl:
-            line += f" pushurl={self.pushurl}"
-        if self.branch:
-            line += f" branch={self.branch}"
-        if self.path:
-            line += f" path={self.path}"
-        if not self.egg:
-            line += " egg=false"
-        return line
-
-    def __eq__(self, other):
-        return repr(self) == repr(other)
-
-
 class BaseBuildoutFile(BaseFile):
     def __init__(self, file_location, with_markers=False, read_extends=False):
         self.file_location = file_location
         self.path = pathlib.Path(self.file_location).resolve()
         self.with_markers = with_markers
         self.markers = set()
         self.read_extends = read_extends
@@ -312,15 +257,15 @@
                     continue
                 # If this is a Buildout-specific marker, we need to translate it.
                 new_marker = buildout_marker_to_pip_marker(marker)
                 new_version[new_marker] = value
             new_data[package] = new_version
         return new_data
 
-    def to_constraints(self, constraints_path):
+    def to_pip(self, constraints_path):
         """Overwrite constraints file with our data.
 
         The strategy is:
 
         1. Translate our data to constraints data.
         2. Ask the constraints file to rewrite itself.
         """
@@ -347,24 +292,24 @@
 
 class SourcesFile(BaseBuildoutFile):
     @property
     def data(self):
         sources_dict = OrderedDict()
         # I don't think we need to support [sources:marker].
         for name, value in self.config["sources"].items():
-            source = Source.create_from_string(value)
+            source = Source.create_from_string(name, value)
             sources_dict[name] = source
         return sources_dict
 
     @property
     def raw_data(self):
         sources_dict = OrderedDict()
         # I don't think we need to support [sources:marker].
         for name, value in self.raw_config["sources"].items():
-            source = Source.create_from_string(value)
+            source = Source.create_from_string(name, value)
             sources_dict[name] = source
         return sources_dict
 
     def __setitem__(self, package_name, value):
         raise NotImplementedError
 
     def rewrite(self):
@@ -392,14 +337,46 @@
         for name, source in self.raw_data.items():
             contents.append(f"{name} = {str(source)}")
 
         contents.append("")
         new_contents = "\n".join(contents)
         self.path.write_text(new_contents)
 
+    def to_pip(self, pip_path):
+        """Overwrite mxdev/pip sources file with our data.
+
+        The strategy is:
+
+        1. Translate our data to mxdev sources data.
+        2. Ask the msdev sources file to rewrite itself.
+        """
+        # Import here to avoid circular imports.
+        from plone.releaser.pip import MxSourcesFile
+
+        sources = MxSourcesFile(pip_path)
+        # Create or empty the sources file.
+        sources.path.write_text("")
+
+        # Translate our data to pip.
+        sources.data = self.raw_data
+        sources.settings = {"docs-directory": "documentation"}
+        if "remotes" in self.config:
+            remotes = self.config["remotes"]
+            for key, value in remotes.items():
+                sources.settings[key] = value
+            for source in sources.data.values():
+                source.url = source.url.replace("{remotes:", "{settings:")
+                if source.pushurl:
+                    source.pushurl = source.pushurl.replace("{remotes:", "{settings:")
+                if source.path:
+                    source.path = source.path.replace("{buildout:", "{settings:")
+
+        # Rewrite the file.
+        sources.rewrite()
+
 
 class CheckoutsFile(BaseBuildoutFile):
     @property
     def always_checkout(self):
         return self.config.get("buildout", "always-checkout")
 
     @property
@@ -450,14 +427,38 @@
         contents.append("auto-checkout =")
         for package in self:
             contents.append(f"    {package}")
         contents.append("")
         new_contents = "\n".join(contents)
         self.path.write_text(new_contents)
 
+    def to_pip(self, pip_path):
+        """Overwrite mxdev/pip checkouts file with our data.
+
+        The strategy is:
+
+        1. Translate our data to mxdev checkouts data.
+        2. Ask the msdev checkouts file to rewrite itself.
+        """
+        # Import here to avoid circular imports.
+        from plone.releaser.pip import MxCheckoutsFile
+
+        checkouts = MxCheckoutsFile(pip_path)
+        # Create or empty the checkouts file.
+        checkouts.path.write_text("")
+
+        # Translate our data to pip.
+        # XXX does not do anything
+        checkouts.data = self.data
+        # This is the only setting that makes sense for Plone coredev:
+        checkouts.settings = {"default-use": "false"}
+
+        # Rewrite the file.
+        checkouts.rewrite()
+
 
 class Buildout:
     def __init__(
         self,
         sources_file="sources.cfg",
         checkouts_file="checkouts.cfg",
         versions_file="versions.cfg",
```

### Comparing `plone.releaser-2.2.2/plone/releaser/changelog.py` & `plone_releaser-2.3.0/plone/releaser/changelog.py`

 * *Files identical despite different names*

### Comparing `plone.releaser-2.2.2/plone/releaser/db.py` & `plone_releaser-2.3.0/plone/releaser/db.py`

 * *Files identical despite different names*

### Comparing `plone.releaser-2.2.2/plone/releaser/manage.py` & `plone_releaser-2.3.0/plone/releaser/manage.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from argh import arg
 from argh import ArghParser
 from argh.decorators import named
+from pathlib import Path
 from plone.releaser import ACTION_BATCH
 from plone.releaser import ACTION_INTERACTIVE
 from plone.releaser import ACTION_REPORT
 from plone.releaser import pypi
 from plone.releaser import THIRD_PARTY_PACKAGES
 from plone.releaser.buildout import Buildout
 from plone.releaser.buildout import CheckoutsFile
+from plone.releaser.buildout import SourcesFile
 from plone.releaser.buildout import VersionsFile
 from plone.releaser.package import Package
 from plone.releaser.pip import ConstraintsFile
-from plone.releaser.pip import IniFile
+from plone.releaser.pip import MxCheckoutsFile
 from progress.bar import Bar
 
 import glob
 import time
 
 
 # TODO
@@ -139,15 +141,15 @@
     """
     if path:
         paths = [path]
     else:
         paths = glob.glob("mxdev.ini") + glob.glob("checkouts.cfg")
     for path in paths:
         if path.endswith(".ini"):
-            checkouts = IniFile(path)
+            checkouts = MxCheckoutsFile(path)
         else:
             checkouts = CheckoutsFile(path)
         yield checkouts
 
 
 def check_checkout(package_name, *, path=None):
     """Check if package is in the checkouts.
@@ -264,49 +266,83 @@
             print(
                 f"{constraints.file_location}: {package_name} not pinned yet. "
                 f"Adding pin because you explicitly gave the path."
             )
         constraints.set(package_name, new_version)
 
 
+def _get_paths(path, patterns):
+    paths = []
+    if path:
+        if not isinstance(path, Path):
+            path = Path(path)
+        if path.is_dir():
+            for pat in patterns:
+                paths.extend(glob.glob(str(path / pat)))
+        else:
+            paths = [path]
+    else:
+        for pat in patterns:
+            paths.extend(glob.glob(pat))
+    all_paths = []
+    for path in paths:
+        if not isinstance(path, Path):
+            path = Path(path)
+        all_paths.append(path)
+    return all_paths
+
+
 def versions2constraints(*, path=None):
     """Take a Buildout versions file and create a pip constraints file out of it.
 
+    If a path is given, we handle only that file.
     If no path is given, we use versions*.cfg.
-
-    Notes:
-    * This does not handle 'extends' yet.
-    * This does not handle [versions:pythonX] yet.
-
-    We could parse the file with Buildout.  This incorporates the 'extends',
-    but you lose versions information for other Python versions.
-
-    We could pass an option simple/full.
-    Maybe if a path is passed, we handle only that file in simple mode.
-    Without path, we grab versions.cfg and check 'extends' and other versions.
-
-    'extends = versions-extra.cfg' could be transformed to '-c constraints-extra.txt'
-
-    I think I need some more options in VersionsFile first:
-    - what to do with extends
-    - what to do with [versions:*]
-    - whether to turn it into a single constraints file.
     """
-    if path:
-        paths = [path]
-    else:
-        paths = glob.glob("versions*.cfg")
+    paths = _get_paths(path, ["versions*.cfg"])
     for path in paths:
         versions = VersionsFile(path, with_markers=True)
         # Create path to constraints*.txt instead of versions*.cfg.
         filepath = versions.path
         filename = str(filepath)[len(str(filepath.parent)) + 1 :]
         filename = filename.replace("versions", "constraints").replace(".cfg", ".txt")
         constraints_path = filepath.parent / filename
-        versions.to_constraints(constraints_path)
+        versions.to_pip(constraints_path)
+
+
+def buildout2pip(*, path=None):
+    """Take a Buildout file and create a pip/mxdev file out of it.
+
+    If a path is given, we handle only that file, guessing whether it is a file
+    with versions or sources or checkouts.
+    If no path is given, we use versions*.cfg, sources*.cfg and checkouts*.cfg.
+    """
+    paths = _get_paths(path, ["versions*.cfg", "sources*.cfg", "checkouts*.cfg"])
+    for path in paths:
+        if path.name.startswith("versions"):
+            buildout_file = VersionsFile(path, with_markers=True)
+        elif path.name.startswith("sources"):
+            buildout_file = SourcesFile(path)
+        elif path.name.startswith("checkouts"):
+            buildout_file = CheckoutsFile(path)
+        # Create path to constraints*.txt instead of versions*.cfg, etc.
+        filepath = buildout_file.path
+        filename = str(filepath)[len(str(filepath.parent)) + 1 :]
+        filename = filename.replace("versions", "constraints")
+        if "checkouts" in filename or "sources" in filename:
+            filename = (
+                filename.replace("checkouts", "mxcheckouts")
+                .replace("sources", "mxsources")
+                .replace(".cfg", ".ini")
+            )
+        else:
+            filename = filename.replace(".cfg", ".txt")
+        pip_path = filepath.parent / filename
+        if not pip_path.exists():
+            pip_path.write_text("")
+        buildout_file.to_pip(pip_path)
 
 
 class Manage:
     def __call__(self, **kwargs):
         parser = ArghParser()
         parser.add_commands(
             [
@@ -318,13 +354,14 @@
                 remove_checkout,
                 add_checkout,
                 append_jenkins_build_number_to_package_version,
                 set_package_version,
                 get_package_version,
                 jenkins_report,
                 versions2constraints,
+                buildout2pip,
             ]
         )
         parser.dispatch()
 
 
 manage = Manage()
```

### Comparing `plone.releaser-2.2.2/plone/releaser/package.py` & `plone_releaser-2.3.0/plone/releaser/package.py`

 * *Files identical despite different names*

### Comparing `plone.releaser-2.2.2/plone/releaser/pip.py` & `plone_releaser-2.3.0/plone/releaser/pip.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from .base import BaseFile
+from .base import Source
 from .utils import update_contents
 from collections import defaultdict
+from collections import OrderedDict
 from configparser import ConfigParser
 from functools import cached_property
 
 import pathlib
 import re
 
 
@@ -131,18 +133,73 @@
                 contents.append(line)
 
         contents.append("")
         new_contents = "\n".join(contents)
         self.path.write_text(new_contents)
 
 
-class IniFile(BaseFile):
+class MxSourcesFile(BaseFile):
     """Ini file for mxdev.
 
     What we want to do here is similar to what we have in buildout.py
+    in the SourcesFile.
+    """
+
+    def __init__(self, file_location):
+        super().__init__(file_location)
+        self.config = ConfigParser(
+            default_section="settings",
+        )
+        # mxdev itself calls ConfigParser with extra option
+        # interpolation=ExtendedInterpolation().
+        # This turns a line like 'url = ${settings:plone}/package.git'
+        # into 'url = https://github.com/plone/package.git'.
+        # In our case we very much want the original line,
+        # especially when we do a rewrite of the file.
+        with self.path.open() as f:
+            self.config.read_file(f)
+
+    @cached_property
+    def data(self):
+        sources_dict = OrderedDict()
+        # I don't think we need to support [sources:marker].
+        for package in self.config.sections():
+            section = self.config[package]
+            sources_dict[package] = Source.create_from_section(section)
+        return sources_dict
+
+    @cached_property
+    def settings(self):
+        return self.config["settings"]
+
+    def __setitem__(self, package_name, enabled=True):
+        raise NotImplementedError
+
+    def rewrite(self):
+        """Rewrite the file based on the parsed data.
+
+        This will lose comments, and may change the order.
+        """
+        contents = ["[settings]"]
+        for key, value in self.settings.items():
+            contents.append(f"{key} = {value}")
+
+        for package in self:
+            contents.append("")
+            contents.append(self[package].to_section())
+
+        contents.append("")
+        new_contents = "\n".join(contents)
+        self.path.write_text(new_contents)
+
+
+class MxCheckoutsFile(BaseFile):
+    """Checkouts file for mxdev.
+
+    What we want to do here is similar to what we have in buildout.py
     in the CheckoutsFile: remove a package from auto-checkouts.
     For mxdev: set 'use = false'.
     The default is in 'settings': 'default-use'.
     """
 
     def __init__(self, file_location):
         super().__init__(file_location)
@@ -155,56 +212,71 @@
         # into 'url = https://github.com/plone/package.git'.
         # In our case we very much want the original line,
         # especially when we do a rewrite of the file.
         with self.path.open() as f:
             self.config.read_file(f)
         self.default_use = to_bool(self.config["settings"].get("default-use", True))
 
-    @property
+    @cached_property
     def data(self):
         checkouts = {}
         for package in self.config.sections():
             use = to_bool(self.config[package].get("use", self.default_use))
             if use:
                 checkouts[package] = True
         return checkouts
 
-    @property
+    @cached_property
     def sections(self):
         # If we want to use a package, we must first know that it exists.
         sections = {}
         for package in self.config.sections():
             sections[package] = True
         return sections
 
+    @cached_property
+    def settings(self):
+        return self.config["settings"]
+
     @property
     def lowerkeys_section(self):
         # Map from lower case key to actual key in the sections.
         return {key.lower(): key for key in self.sections}
 
+    def append_package(self, package_name, enabled=True):
+        """Append a package to the checkouts.
+
+        The caller should have made sure this package is currently
+        not in the file.
+        """
+        contents = self.path.read_text()
+        if not contents.endswith("\n"):
+            contents += "\n"
+        use = "true" if enabled else "false"
+        contents += f"\n[{package_name}]\nuse = {use}\n"
+        self.path.write_text(contents)
+
     def __setitem__(self, package_name, enabled=True):
         """Enable or disable a checkout.
 
         Mostly this will be called to disable a checkout.
         Expected is that default-use is false.
         This means we can remove 'use = true' from the package.
 
         But let's support the other way around as well:
         when default-use is true, we set 'use = false'.
-
-        Note that in our Buildout setup, we have sources.cfg separately.
-        In mxdev.ini the source definition and 'use = false/true' is combined.
-        So if the package we want to enable is not defined, meaning it has no
-        section, then we should fail loudly.
         """
         stored_package_name = self.lowerkeys_section.get(package_name.lower())
         if not stored_package_name:
-            raise KeyError(
-                f"{self.file_location}: There is no definition for {package_name}"
-            )
+            # Package is not known to us.
+            if self.default_use == enabled:
+                # The wanted state is the default state, so do nothing.
+                return
+            self.append_package(package_name, enabled=enabled)
+            return
         package_name = stored_package_name
         if package_name in self:
             use = to_bool(self.config[package_name].get("use", self.default_use))
         else:
             use = False
         if use and enabled:
             print(f"{self.file_location}: {package_name} already in checkouts.")
@@ -259,24 +331,20 @@
         contents = "\n".join(lines)
         self.path.write_text(contents)
 
     def rewrite(self):
         """Rewrite the file based on the parsed data.
 
         This will lose comments, and may change the order.
-        TODO Can we trust self.config? It won't get updated if we change any data
-        after reading.
         """
         contents = ["[settings]"]
-        for key, value in self.config["settings"].items():
+        for key, value in self.settings.items():
             contents.append(f"{key} = {value}")
 
-        for package in self.sections:
+        for package in self.data:
             contents.append("")
             contents.append(f"[{package}]")
-            for key, value in self.config[package].items():
-                if self.config["settings"].get(key) != value:
-                    contents.append(f"{key} = {value}")
+            contents.append("use = true")
 
         contents.append("")
         new_contents = "\n".join(contents)
         self.path.write_text(new_contents)
```

### Comparing `plone.releaser-2.2.2/plone/releaser/pypi.py` & `plone_releaser-2.3.0/plone/releaser/pypi.py`

 * *Files identical despite different names*

### Comparing `plone.releaser-2.2.2/plone/releaser/release.py` & `plone_releaser-2.3.0/plone/releaser/release.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from copy import copy
 from plone.releaser.buildout import CheckoutsFile
 from plone.releaser.buildout import SourcesFile
 from plone.releaser.buildout import VersionsFile
 from plone.releaser.pip import ConstraintsFile
-from plone.releaser.pip import IniFile
+from plone.releaser.pip import MxSourcesFile
 from plone.releaser.pypi import can_user_release_package_to_pypi
 from zest.releaser import pypi
 from zest.releaser.utils import ask
 from zest.releaser.utils import read_text_file
 from zest.releaser.utils import write_text_file
 
 import git
@@ -216,39 +216,23 @@
             remove_from_checkouts(package_name)
         # git commit
         message = f"{package_name} {new_version}"
         # add all changed files
         g.add("--all")
         print("Committing changes.")
         g.commit(message=message)
-        # When doing releases of several packages in a row,
-        # it is better to not push, because this means a needlessly high load on Jenkins.
-        # Also, if you create a release and immediately push,
-        # then Jenkins will not find the new release yet and fail:
-        # it takes a few minutes for the release to be propagated to all PyPI mirrors.
-        # Pushing still seems the best default, but let's have an easy way to not push.
-        print("Checking PLONE_RELEASER_MULTI_PACKAGES env variable.")
-        try:
-            multi = int(os.getenv("PLONE_RELEASER_MULTI_PACKAGES"))
-        except (TypeError, ValueError, AttributeError):
-            print(
-                "ERROR: could not parse PLONE_RELEASER_MULTI_PACKAGES env var. Ignoring it."
-            )
-            multi = False
-        if multi:
-            print(
-                "PLONE_RELEASER_MULTI_PACKAGES env variable set, so not pushing to coredev."
-            )
-            return
-        msg = "Ok to push coredev?"
-        if branch:
-            msg = f"Ok to push coredev {branch}?"
-        if ask(msg, default=True):
-            print("Pushing changes to server.")
-            g.push()
+        # We used to offer pushing the coredev change, but this is no longer a
+        # good idea.
+        print(
+            "WARNING: a change in one or more buildout.coredev branches was made. "
+            "Please wait a few minutes and then push this change. Otherwise the "
+            "newly uploaded package is not yet available on all PyPI mirrors. "
+            "This would cause Jenkins and GitHub Actions to fail."
+        )
+        return
 
 
 def update_other_core_branches(data):
     CORE_BRANCHES = ["5.2", "6.0", "6.1"]
     package_name = data["name"]
     root_path = os.path.join(os.getcwd(), "../../")
 
@@ -267,15 +251,23 @@
     current_core_branch = _get_current_core_branch()
     CORE_BRANCHES.remove(current_core_branch)
 
     reference_package_branch = _get_package_branch(package_name=package_name)
 
     g = git.Git(root_path)
     for branch_name in CORE_BRANCHES:
-        g.checkout(branch_name)
+        try:
+            g.checkout(branch_name)
+        except git.exc.GitCommandError:
+            print(
+                f"WARNING: There was an error checking out coredev branch "
+                f"{branch_name}. This means we cannot check if this branch needs an "
+                f"update for {package_name}. Please check manually."
+            )
+            continue
 
         package_branch = _get_package_branch(package_name=package_name)
         if package_branch == reference_package_branch:
             try:
                 update_core(data, branch=branch_name)
             except Exception:
                 print(
@@ -315,9 +307,9 @@
     coredev_dir = (cwd / os.pardir / os.pardir).resolve()
     checkouts_file = coredev_dir / "checkouts.cfg"
     if checkouts_file.exists():
         checkouts = CheckoutsFile(checkouts_file)
         checkouts.remove(package_name)
     checkouts_file = coredev_dir / "mxdev.ini"
     if checkouts_file.exists():
-        checkouts = IniFile(checkouts_file)
+        checkouts = MxSourcesFile(checkouts_file)
         checkouts.remove(package_name)
```

### Comparing `plone.releaser-2.2.2/plone/releaser/tests/input/changes.rst` & `plone_releaser-2.3.0/plone/releaser/tests/input/changes.rst`

 * *Files identical despite different names*

### Comparing `plone.releaser-2.2.2/plone/releaser/tests/input/sources.cfg` & `plone_releaser-2.3.0/plone/releaser/tests/input/sources.cfg`

 * *Files identical despite different names*

### Comparing `plone.releaser-2.2.2/plone/releaser/tests/test_buildout.py` & `plone_releaser-2.3.0/plone/releaser/tests/test_buildout.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from plone.releaser.buildout import CheckoutsFile
-from plone.releaser.buildout import Source
 from plone.releaser.buildout import SourcesFile
 from plone.releaser.buildout import VersionsFile
 
 import os
 import pathlib
 import pytest
 import shutil
@@ -97,57 +96,14 @@
 auto-checkout =
     CamelCase
     package
 """
     )
 
 
-def test_source_standard():
-    src = Source.create_from_string(
-        "git https://github.com/plone/Plone.git pushurl=git@github.com:plone/Plone.git branch=6.0.x"
-    )
-    assert src.protocol == "git"
-    assert src.url == "https://github.com/plone/Plone.git"
-    assert src.pushurl == "git@github.com:plone/Plone.git"
-    assert src.branch == "6.0.x"
-    assert src.egg is True
-    assert src.path is None
-
-
-def test_source_not_enough_parameters():
-    with pytest.raises(IndexError):
-        Source.create_from_string("")
-    with pytest.raises(IndexError):
-        Source.create_from_string("git")
-
-
-def test_source_just_enough_parameters():
-    # protocol and url are enough
-    src = Source.create_from_string("git https://github.com/plone/Plone.git")
-    assert src.protocol == "git"
-    assert src.url == "https://github.com/plone/Plone.git"
-    assert src.pushurl is None
-    assert src.branch == "master"
-    assert src.egg is True
-    assert src.path is None
-
-
-def test_source_docs():
-    # Plone has a docs source with some extra options.
-    src = Source.create_from_string(
-        "git https://github.com/plone/documentation.git pushurl=git@github.com:plone/documentation.git egg=false branch=6.0 path=docs"
-    )
-    assert src.protocol == "git"
-    assert src.url == "https://github.com/plone/documentation.git"
-    assert src.pushurl == "git@github.com:plone/documentation.git"
-    assert src.branch == "6.0"
-    assert src.egg is False
-    assert src.path == "docs"
-
-
 def test_sources_file_data():
     sf = SourcesFile(SOURCES_FILE)
     assert sorted(sf.data.keys()) == ["Plone", "docs", "plone.alterego", "plone.base"]
 
 
 def test_sources_file_contains():
     sf = SourcesFile(SOURCES_FILE)
```

### Comparing `plone.releaser-2.2.2/plone/releaser/tests/test_changelog.py` & `plone_releaser-2.3.0/plone/releaser/tests/test_changelog.py`

 * *Files identical despite different names*

### Comparing `plone.releaser-2.2.2/plone/releaser/tests/test_pip.py` & `plone_releaser-2.3.0/plone/releaser/tests/test_pip.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,139 +1,20 @@
 from plone.releaser.pip import ConstraintsFile
-from plone.releaser.pip import IniFile
 
 import pathlib
 import pytest
 import shutil
 
 
 TESTS_DIR = pathlib.Path(__file__).parent
 INPUT_DIR = TESTS_DIR / "input"
 CONSTRAINTS_FILE = INPUT_DIR / "constraints.txt"
 CONSTRAINTS_FILE2 = INPUT_DIR / "constraints2.txt"
 CONSTRAINTS_FILE3 = INPUT_DIR / "constraints3.txt"
 CONSTRAINTS_FILE4 = INPUT_DIR / "constraints4.txt"
-MXDEV_FILE = INPUT_DIR / "mxdev.ini"
-
-
-def test_mxdev_file_data():
-    mf = IniFile(MXDEV_FILE)
-    # The data used to map lower case to actual case,
-    # but now actual case to True.
-    assert mf.data == {
-        "CamelCase": True,
-        "package": True,
-    }
-
-
-def test_mxdev_file_contains():
-    mf = IniFile(MXDEV_FILE)
-    assert "package" in mf
-    assert "unused" not in mf
-    # We compare case insensitively.
-    assert "camelcase" in mf
-    assert "CamelCase" in mf
-    assert "CAMELCASE" in mf
-
-
-def test_mxdev_file_get():
-    mf = IniFile(MXDEV_FILE)
-    assert mf["package"] is True
-    assert mf.get("package") is True
-    assert mf["camelcase"] is True
-    assert mf["CAMELCASE"] is True
-    assert mf["CamelCase"] is True
-    with pytest.raises(KeyError):
-        mf["unused"]
-    assert mf.get("unused") is None
-
-
-def test_mxdev_file_add_known(tmp_path):
-    # When we add or remove a checkout, the file changes, so we work on a copy.
-    copy_path = tmp_path / "mxdev.ini"
-    shutil.copyfile(MXDEV_FILE, copy_path)
-    mf = IniFile(copy_path)
-    assert "unused" not in mf
-    mf.add("unused")
-    # Let's read it fresh, for good measure.
-    mf = IniFile(copy_path)
-    assert "unused" in mf
-    assert mf["unused"] is True
-
-
-def test_mxdev_file_add_unknown(tmp_path):
-    # We cannot edit mxdev.ini to use a package when it is not defined.
-    copy_path = tmp_path / "mxdev.ini"
-    shutil.copyfile(MXDEV_FILE, copy_path)
-    mf = IniFile(copy_path)
-    assert "unknown" not in mf
-    with pytest.raises(KeyError):
-        mf.add("unknown")
-
-
-def test_mxdev_file_remove(tmp_path):
-    copy_path = tmp_path / "mxdev.ini"
-    shutil.copyfile(MXDEV_FILE, copy_path)
-    mf = IniFile(copy_path)
-    assert "package" in mf
-    mf.remove("package")
-    # Let's read it fresh, for good measure.
-    mf = IniFile(copy_path)
-    assert "package" not in mf
-    assert "CAMELCASE" in mf
-    mf.remove("CAMELCASE")
-    mf = IniFile(copy_path)
-    assert "CAMELCASE" not in mf
-    assert "CamelCase" not in mf
-    assert "camelcase" not in mf
-    # Check that we can re-enable a package:
-    # editing should not remove the entire section.
-    mf.add("package")
-    mf = IniFile(copy_path)
-    assert "package" in mf
-    # This should work for the last section as well.
-    mf.add("CamelCase")
-    mf = IniFile(copy_path)
-    assert "CamelCase" in mf
-
-
-def test_mxdev_file_rewrite(tmp_path):
-    copy_path = tmp_path / "mxdev.ini"
-    shutil.copyfile(MXDEV_FILE, copy_path)
-    mf = IniFile(copy_path)
-    mf.rewrite()
-    # Read it fresh and compare
-    mf2 = IniFile(copy_path)
-    assert mf.data == mf2.data
-    # Check the entire text.  Note that packages are alphabetically sorted.
-    # Currently we get the original case, but we may change this to lowercase.
-    assert (
-        copy_path.read_text()
-        == """[settings]
-requirements-in = requirements.txt
-requirements-out = requirements-mxdev.txt
-contraints-out = constraints-mxdev.txt
-default-use = false
-plone = https://github.com/plone
-
-[package]
-url = ${settings:plone}/package.git
-branch = main
-use = true
-
-[unused]
-url = ${settings:plone}/package.git
-branch = main
-
-[CamelCase]
-url = ${settings:plone}/CamelCase.git
-branch = main
-use = true
-"""
-    )
 
 
 def test_constraints_file_constraints():
     cf = ConstraintsFile(CONSTRAINTS_FILE)
     # All constraints are reported lowercased.
     assert cf.data == {
         "annotated": "1.0",
```

### Comparing `plone.releaser-2.2.2/plone/releaser/tests/test_utils.py` & `plone_releaser-2.3.0/plone/releaser/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `plone.releaser-2.2.2/plone/releaser/utils.py` & `plone_releaser-2.3.0/plone/releaser/utils.py`

 * *Files identical despite different names*

### Comparing `plone.releaser-2.2.2/plone.releaser.egg-info/PKG-INFO` & `plone_releaser-2.3.0/plone.releaser.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.releaser
-Version: 2.2.2
+Version: 2.3.0
 Summary: Plone release management utilities
 Home-page: https://github.com/plone/plone.releaser
 Author: Eric Steele
 Author-email: eric@esteele.net
 License: GPL
 Keywords: plone release
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,30 +28,67 @@
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
 Introduction
 ============
 
 Tools to make managing Plone core releases easier.
+It is a wrapper around ``zest.releaser``, plus it adds some commands.
+
+WARNING: this package is only meant for development of core Plone.
+It may have useful bits for others, but we may drop features and edge cases at any time if it is no longer useful for Plone.
+
 
 Installation
 ------------
 
-To install plone.releaser add it to your buildout::
+Do ``pip install plone.releaser`` or add it to your buildout::
 
   [release]
   recipe = zc.recipe.egg
-  eggs =  plone.releaser
+  eggs = plone.releaser
+
+
+Main usage: release a package
+-----------------------------
+
+In  the `Plone core development buildout <https://github.com/plone/buildout.coredev>`_ go to ``src/some.package`` and run ``../../bin/fullrelease``.
+This calls the ``fullrelease`` command from ``zest.releaser``, but with some extra hooks and packages available.
+
+One nice thing it does: look in the checkouts and sources of your ``buildout.coredev`` checkout and update them:
+remove the released package from the checkouts and update the version.
+
+If you are working on branch 6.1 of coredev, then we check if you also have branches 5.2 and 6.0 checked out.
+There we check if the branch of the released package is in the sources.
+If you make a release from package branch ``main`` and this is the branch used in the sources, then we update the checkouts and sources of this coredev branch as well.
+
+After releasing a package, you should wait a few minutes before you manually push the changes to all coredev branches.
+This gives the PyPI mirrors time to catch up so the new release is available, so Jenkins and GitHub Actions can find it.
+
 
-To make it available in buildout.coredev, run buildout with releaser.cfg::
+Main commands
+-------------
 
-  $ bin/buildout -c releaser.cfg
+Take several Buildout files and create pip/mxdev files out of them::
 
-Usage
------
+  $ bin/manage buildout2pip
+
+Take a Buildout versions file and create a pip constraints file out of it.
+
+  $ bin/manage versions2constraints
+
+Generate a changelog with changes from all packages since a certain Plone release::
+
+  $ bin/manage changelog --start=6.1.0a1
+
+
+Other commands
+--------------
+
+Some commands are not used much (by Maurits anyway) because they are less needed these days.
 
 Check PyPi access to all Plone packages for a certain user::
 
   $ bin/manage checkPypi timo
 
 Check a package for updates::
 
@@ -61,32 +98,56 @@
 
   $ bin/manage report --interactive
 
 Pulls::
 
   $ bin/manage pulls
 
-Changelog::
-
-  $ bin/manage changelog
-
 Check checkout::
 
   $ bin/manage check-checkout
 
 Changelog
 =========
 
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.3.0 (2024-05-30)
+------------------
+
+New features:
+
+
+- Add buildout2pip manage command.
+  [maurits] (#72)
+
+
+Bug fixes:
+
+
+- Catch error when trying to change coredev branches.
+  Not everyone may have the branches available, or there may be some problem with it. (#67)
+- No longer offer to push changes to buildout.coredev.
+  This is no longer what we ever want: the newly uploaded package will not yet be available on all PyPI mirrors.
+  Fixes `issue 69 <https://github.com/plone/plone.releaser/issues/69>`_.
+  [maurits] (#69)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs]
+
+
 2.2.2 (2024-04-16)
 ------------------
 
 Bug fixes:
 
 
 - Preserve the case of package names in versions2constraints and friends.
```

### Comparing `plone.releaser-2.2.2/plone.releaser.egg-info/SOURCES.txt` & `plone_releaser-2.3.0/plone.releaser.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -24,24 +24,29 @@
 plone/releaser/package.py
 plone/releaser/pip.py
 plone/releaser/pypi.py
 plone/releaser/release.py
 plone/releaser/utils.py
 plone/releaser/tests/__init__.py
 plone/releaser/tests/test_buildout.py
+plone/releaser/tests/test_buildout2pip.py
 plone/releaser/tests/test_changelog.py
+plone/releaser/tests/test_mxdev_checkouts.py
+plone/releaser/tests/test_mxdev_sources.py
 plone/releaser/tests/test_pip.py
+plone/releaser/tests/test_source.py
 plone/releaser/tests/test_utils.py
 plone/releaser/tests/test_versions2constraints.py
 plone/releaser/tests/input/changes.md
 plone/releaser/tests/input/changes.rst
 plone/releaser/tests/input/checkouts.cfg
 plone/releaser/tests/input/constraints.txt
 plone/releaser/tests/input/constraints2.txt
 plone/releaser/tests/input/constraints3.txt
 plone/releaser/tests/input/constraints4.txt
-plone/releaser/tests/input/mxdev.ini
+plone/releaser/tests/input/mxcheckouts.ini
+plone/releaser/tests/input/mxsources.ini
 plone/releaser/tests/input/sources.cfg
 plone/releaser/tests/input/versions.cfg
 plone/releaser/tests/input/versions2.cfg
 plone/releaser/tests/input/versions3.cfg
 plone/releaser/tests/input/versions4.cfg
```

### Comparing `plone.releaser-2.2.2/plone.releaser.egg-info/entry_points.txt` & `plone_releaser-2.3.0/plone.releaser.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `plone.releaser-2.2.2/pyproject.toml` & `plone_releaser-2.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # Generated from:
-# https://github.com/plone/meta/tree/master/config/default
+# https://github.com/plone/meta/tree/main/config/default
 # See the inline comments on how to expand/tweak this configuration file
+[build-system]
+requires = ["setuptools>=68.2"]
+
 [tool.towncrier]
 directory = "news/"
 filename = "CHANGES.rst"
 title_format = "{version} ({project_date})"
 underlines = ["-", ""]
 
 [[tool.towncrier.type]]
@@ -129,28 +132,35 @@
 #    "pygithub = ['github']",
 #  ]
 ##
 
 [tool.check-manifest]
 ignore = [
     ".editorconfig",
+    ".flake8",
     ".meta.toml",
     ".pre-commit-config.yaml",
-    "tox.ini",
-    ".flake8",
+    "dependabot.yml",
     "mx.ini",
+    "tox.ini",
 
 ]
+
 ##
 # Add extra configuration options in .meta.toml:
 #  [pyproject]
 #  check_manifest_ignores = """
 #      "*.map.js",
 #      "*.pyc",
 #  """
+#  check_manifest_extra_lines = """
+#  ignore-bad-ideas = [
+#      "some/test/file/PKG-INFO",
+#  ]
+#  """
 ##
 
 
 ##
 # Add extra configuration options in .meta.toml:
 #  [pyproject]
 #  extra_lines = """
```

### Comparing `plone.releaser-2.2.2/setup.py` & `plone_releaser-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "2.2.2"
+version = "2.3.0"
 
 long_description = "{}\n{}".format(
     open("README.rst").read(), open("CHANGES.rst").read()
 )
 
 setup(
     name="plone.releaser",
```

