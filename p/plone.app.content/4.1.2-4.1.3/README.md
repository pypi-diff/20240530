# Comparing `tmp/plone.app.content-4.1.2.tar.gz` & `tmp/plone_app_content-4.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.content-4.1.2.tar", last modified: Mon Feb 12 15:07:16 2024, max compression
+gzip compressed data, was "plone_app_content-4.1.3.tar", last modified: Thu May 30 18:29:27 2024, max compression
```

## Comparing `plone.app.content-4.1.2.tar` & `plone_app_content-4.1.3.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-12 15:07:16.278555 plone.app.content-4.1.2/
--rw-r--r--   0 maurits    (501) staff       (20)    38229 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      148 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    40684 2024-02-12 15:07:16.278094 plone.app.content-4.1.2/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      461 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-12 15:07:16.246689 plone.app.content-4.1.2/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      679 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-12 15:07:16.246972 plone.app.content-4.1.2/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-12 15:07:16.249727 plone.app.content-4.1.2/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-12 15:07:16.252194 plone.app.content-4.1.2/plone/app/content/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-12 15:07:16.260219 plone.app.content-4.1.2/plone/app/content/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)    12509 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/actions.py
--rw-r--r--   0 maurits    (501) staff       (20)      724 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/adding.py
--rw-r--r--   0 maurits    (501) staff       (20)     5053 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2599 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/constraintypes.pt
--rw-r--r--   0 maurits    (501) staff       (20)     6267 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/constraintypes.py
--rw-r--r--   0 maurits    (501) staff       (20)     5401 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/content_status_history.py
--rw-r--r--   0 maurits    (501) staff       (20)     6511 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/content_status_modify.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-12 15:07:16.264854 plone.app.content-4.1.2/plone/app/content/browser/contents/
--rw-r--r--   0 maurits    (501) staff       (20)    13480 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/contents/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3925 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/contents/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1693 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/contents/copy.py
--rw-r--r--   0 maurits    (501) staff       (20)     2419 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/contents/cut.py
--rw-r--r--   0 maurits    (501) staff       (20)      712 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/contents/defaultpage.py
--rw-r--r--   0 maurits    (501) staff       (20)     3441 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/contents/delete.py
--rw-r--r--   0 maurits    (501) staff       (20)     2168 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/contents/paste.py
--rw-r--r--   0 maurits    (501) staff       (20)     4893 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/contents/properties.py
--rw-r--r--   0 maurits    (501) staff       (20)     3143 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/contents/rearrange.py
--rw-r--r--   0 maurits    (501) staff       (20)     4229 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/contents/rename.py
--rw-r--r--   0 maurits    (501) staff       (20)     1882 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/contents/tags.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-12 15:07:16.266833 plone.app.content-4.1.2/plone/app/content/browser/contents/templates/
--rw-r--r--   0 maurits    (501) staff       (20)      202 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/contents/templates/delete.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1065 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/contents/templates/folder_contents.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2738 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/contents/templates/properties.pt
--rw-r--r--   0 maurits    (501) staff       (20)      799 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/contents/templates/rename.pt
--rw-r--r--   0 maurits    (501) staff       (20)      809 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/contents/templates/tags.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1229 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/contents/templates/workflow.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3879 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/contents/workflow.py
--rw-r--r--   0 maurits    (501) staff       (20)     6662 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/file.py
--rw-r--r--   0 maurits    (501) staff       (20)     3916 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/folder_publish.py
--rw-r--r--   0 maurits    (501) staff       (20)     3382 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/folderfactories.pt
--rw-r--r--   0 maurits    (501) staff       (20)     5360 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/folderfactories.py
--rw-r--r--   0 maurits    (501) staff       (20)     1198 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/full_review_list.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1489 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/i18n.py
--rw-r--r--   0 maurits    (501) staff       (20)      363 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      523 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/query.py
--rw-r--r--   0 maurits    (501) staff       (20)     6481 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/reviewlist.py
--rw-r--r--   0 maurits    (501) staff       (20)     4926 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/selection.py
--rw-r--r--   0 maurits    (501) staff       (20)    12110 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/table.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4810 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/table.txt
--rw-r--r--   0 maurits    (501) staff       (20)     5661 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/tableview.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-12 15:07:16.268866 plone.app.content-4.1.2/plone/app/content/browser/templates/
--rw-r--r--   0 maurits    (501) staff       (20)    22405 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/templates/content_status_history.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2413 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/templates/delete_confirmation.pt
--rw-r--r--   0 maurits    (501) staff       (20)      845 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/templates/object_rename.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4686 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/templates/select_default_page.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4607 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/templates/select_default_view.pt
--rw-r--r--   0 maurits    (501) staff       (20)    13746 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/browser/vocabulary.py
--rw-r--r--   0 maurits    (501) staff       (20)      220 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/catalog.py
--rw-r--r--   0 maurits    (501) staff       (20)      729 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1683 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     3447 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/namechooser.py
--rw-r--r--   0 maurits    (501) staff       (20)     4853 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/namechooser.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4664 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-12 15:07:16.275537 plone.app.content-4.1.2/plone/app/content/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1185 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/tests/image.png
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-12 15:07:16.275873 plone.app.content-4.1.2/plone/app/content/tests/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-12 15:07:16.276272 plone.app.content-4.1.2/plone/app/content/tests/profiles/non-ascii-workflow-profile/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-12 15:07:16.244107 plone.app.content-4.1.2/plone/app/content/tests/profiles/non-ascii-workflow-profile/workflows/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-12 15:07:16.276551 plone.app.content-4.1.2/plone/app/content/tests/profiles/non-ascii-workflow-profile/workflows/non-ascii-workflow/
--rw-r--r--   0 maurits    (501) staff       (20)     2153 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/tests/profiles/non-ascii-workflow-profile/workflows/non-ascii-workflow/definition.xml
--rw-r--r--   0 maurits    (501) staff       (20)      196 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/tests/profiles/non-ascii-workflow-profile/workflows.xml
--rw-r--r--   0 maurits    (501) staff       (20)      440 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/tests/profiles/non-ascii-workflow.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    17320 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/tests/test_actions.py
--rw-r--r--   0 maurits    (501) staff       (20)      785 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/tests/test_adding.py
--rw-r--r--   0 maurits    (501) staff       (20)      636 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/tests/test_constrains.py
--rw-r--r--   0 maurits    (501) staff       (20)     7024 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/tests/test_content_status_modify.py
--rw-r--r--   0 maurits    (501) staff       (20)    26693 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/tests/test_contents.py
--rw-r--r--   0 maurits    (501) staff       (20)    20506 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/tests/test_folder.py
--rw-r--r--   0 maurits    (501) staff       (20)     5289 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/tests/test_folder_publish.py
--rw-r--r--   0 maurits    (501) staff       (20)      457 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/tests/test_namechooser.py
--rw-r--r--   0 maurits    (501) staff       (20)     1795 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/tests/test_namechooser_unit.py
--rw-r--r--   0 maurits    (501) staff       (20)     2121 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/tests/test_non_ascii_characters_in_workflow_state.py
--rw-r--r--   0 maurits    (501) staff       (20)     9189 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/tests/test_permissions.py
--rw-r--r--   0 maurits    (501) staff       (20)     2911 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/tests/test_reviewlist.py
--rw-r--r--   0 maurits    (501) staff       (20)     4883 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/tests/test_selectdefaultpage.py
--rw-r--r--   0 maurits    (501) staff       (20)      386 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/tests/test_table.py
--rw-r--r--   0 maurits    (501) staff       (20)    26063 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/tests/test_widgets.py
--rw-r--r--   0 maurits    (501) staff       (20)     1050 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/plone/app/content/utils.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-12 15:07:16.276898 plone.app.content-4.1.2/plone.app.content.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    40684 2024-02-12 15:07:16.000000 plone.app.content-4.1.2/plone.app.content.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     3760 2024-02-12 15:07:16.000000 plone.app.content-4.1.2/plone.app.content.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-02-12 15:07:16.000000 plone.app.content-4.1.2/plone.app.content.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2024-02-12 15:07:16.000000 plone.app.content-4.1.2/plone.app.content.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-02-12 15:07:16.000000 plone.app.content-4.1.2/plone.app.content.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      503 2024-02-12 15:07:16.000000 plone.app.content-4.1.2/plone.app.content.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2024-02-12 15:07:16.000000 plone.app.content-4.1.2/plone.app.content.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4212 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)       38 2024-02-12 15:07:16.278629 plone.app.content-4.1.2/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2256 2024-02-12 15:07:15.000000 plone.app.content-4.1.2/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:29:27.665254 plone_app_content-4.1.3/
+-rw-r--r--   0 maurits    (501) staff       (20)    38341 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      148 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    40796 2024-05-30 18:29:27.664514 plone_app_content-4.1.3/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      461 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:29:27.621964 plone_app_content-4.1.3/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      679 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:29:27.622429 plone_app_content-4.1.3/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:29:27.626298 plone_app_content-4.1.3/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:29:27.630085 plone_app_content-4.1.3/plone/app/content/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:29:27.640812 plone_app_content-4.1.3/plone/app/content/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)    12509 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/actions.py
+-rw-r--r--   0 maurits    (501) staff       (20)      724 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/adding.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5053 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2599 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/constraintypes.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     6267 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/constraintypes.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5401 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/content_status_history.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6511 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/content_status_modify.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:29:27.646758 plone_app_content-4.1.3/plone/app/content/browser/contents/
+-rw-r--r--   0 maurits    (501) staff       (20)    13480 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/contents/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3925 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/contents/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1693 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/contents/copy.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2419 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/contents/cut.py
+-rw-r--r--   0 maurits    (501) staff       (20)      712 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/contents/defaultpage.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3441 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/contents/delete.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2168 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/contents/paste.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4893 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/contents/properties.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3143 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/contents/rearrange.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4229 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/contents/rename.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1882 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/contents/tags.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:29:27.649558 plone_app_content-4.1.3/plone/app/content/browser/contents/templates/
+-rw-r--r--   0 maurits    (501) staff       (20)      202 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/contents/templates/delete.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1065 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/contents/templates/folder_contents.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2738 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/contents/templates/properties.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      799 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/contents/templates/rename.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      809 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/contents/templates/tags.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1229 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/contents/templates/workflow.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3879 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/contents/workflow.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6662 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/file.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3916 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/folder_publish.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3382 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/folderfactories.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     5360 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/folderfactories.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1198 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/full_review_list.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1489 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/i18n.py
+-rw-r--r--   0 maurits    (501) staff       (20)      363 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      523 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/query.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6481 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/reviewlist.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5110 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/selection.py
+-rw-r--r--   0 maurits    (501) staff       (20)    12110 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/table.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4810 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/table.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     5661 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/tableview.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:29:27.652109 plone_app_content-4.1.3/plone/app/content/browser/templates/
+-rw-r--r--   0 maurits    (501) staff       (20)    22405 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/templates/content_status_history.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2413 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/templates/delete_confirmation.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      845 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/templates/object_rename.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4686 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/templates/select_default_page.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4607 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/templates/select_default_view.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    13746 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/browser/vocabulary.py
+-rw-r--r--   0 maurits    (501) staff       (20)      220 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/catalog.py
+-rw-r--r--   0 maurits    (501) staff       (20)      729 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1683 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3447 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/namechooser.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4853 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/namechooser.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4664 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:29:27.660373 plone_app_content-4.1.3/plone/app/content/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1185 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/tests/image.png
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:29:27.660925 plone_app_content-4.1.3/plone/app/content/tests/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:29:27.661400 plone_app_content-4.1.3/plone/app/content/tests/profiles/non-ascii-workflow-profile/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:29:27.617841 plone_app_content-4.1.3/plone/app/content/tests/profiles/non-ascii-workflow-profile/workflows/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:29:27.661874 plone_app_content-4.1.3/plone/app/content/tests/profiles/non-ascii-workflow-profile/workflows/non-ascii-workflow/
+-rw-r--r--   0 maurits    (501) staff       (20)     2153 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/tests/profiles/non-ascii-workflow-profile/workflows/non-ascii-workflow/definition.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      196 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/tests/profiles/non-ascii-workflow-profile/workflows.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      440 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/tests/profiles/non-ascii-workflow.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    17310 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/tests/test_actions.py
+-rw-r--r--   0 maurits    (501) staff       (20)      785 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/tests/test_adding.py
+-rw-r--r--   0 maurits    (501) staff       (20)      636 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/tests/test_constrains.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7024 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/tests/test_content_status_modify.py
+-rw-r--r--   0 maurits    (501) staff       (20)    26693 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/tests/test_contents.py
+-rw-r--r--   0 maurits    (501) staff       (20)    20506 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/tests/test_folder.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5289 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/tests/test_folder_publish.py
+-rw-r--r--   0 maurits    (501) staff       (20)      457 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/tests/test_namechooser.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1795 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/tests/test_namechooser_unit.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2121 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/tests/test_non_ascii_characters_in_workflow_state.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9189 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/tests/test_permissions.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2911 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/tests/test_reviewlist.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4883 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/tests/test_selectdefaultpage.py
+-rw-r--r--   0 maurits    (501) staff       (20)      386 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/tests/test_table.py
+-rw-r--r--   0 maurits    (501) staff       (20)    26063 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/tests/test_widgets.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1050 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/plone/app/content/utils.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:29:27.662481 plone_app_content-4.1.3/plone.app.content.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    40796 2024-05-30 18:29:27.000000 plone_app_content-4.1.3/plone.app.content.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     3760 2024-05-30 18:29:27.000000 plone_app_content-4.1.3/plone.app.content.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-05-30 18:29:27.000000 plone_app_content-4.1.3/plone.app.content.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2024-05-30 18:29:27.000000 plone_app_content-4.1.3/plone.app.content.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-05-30 18:29:27.000000 plone_app_content-4.1.3/plone.app.content.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      503 2024-05-30 18:29:27.000000 plone_app_content-4.1.3/plone.app.content.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-05-30 18:29:27.000000 plone_app_content-4.1.3/plone.app.content.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4212 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2024-05-30 18:29:27.665402 plone_app_content-4.1.3/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2256 2024-05-30 18:29:26.000000 plone_app_content-4.1.3/setup.py
```

### Comparing `plone.app.content-4.1.2/CHANGES.rst` & `plone_app_content-4.1.3/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,23 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.1.3 (2024-05-30)
+------------------
+
+Bug fixes:
+
+
+- Remove usage of CMFPlone skins script [@jensens] (#281)
+
+
 4.1.2 (2024-02-12)
 ------------------
 
 Bug fixes:
 
 
 - Fix escaping HTML in ``tags`` popover.
```

### Comparing `plone.app.content-4.1.2/PKG-INFO` & `plone_app_content-4.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.content
-Version: 4.1.2
+Version: 4.1.3
 Summary: Content Views for Plone
 Home-page: https://pypi.org/project/plone.app.content
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone content views viewlet
 Classifier: Development Status :: 5 - Production/Stable
@@ -75,14 +75,23 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.1.3 (2024-05-30)
+------------------
+
+Bug fixes:
+
+
+- Remove usage of CMFPlone skins script [@jensens] (#281)
+
+
 4.1.2 (2024-02-12)
 ------------------
 
 Bug fixes:
 
 
 - Fix escaping HTML in ``tags`` popover.
```

### Comparing `plone.app.content-4.1.2/docs/LICENSE.GPL` & `plone_app_content-4.1.3/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/docs/LICENSE.txt` & `plone_app_content-4.1.3/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/actions.py` & `plone_app_content-4.1.3/plone/app/content/browser/actions.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/adding.py` & `plone_app_content-4.1.3/plone/app/content/browser/adding.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/configure.zcml` & `plone_app_content-4.1.3/plone/app/content/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/constraintypes.pt` & `plone_app_content-4.1.3/plone/app/content/browser/constraintypes.pt`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/constraintypes.py` & `plone_app_content-4.1.3/plone/app/content/browser/constraintypes.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/content_status_history.py` & `plone_app_content-4.1.3/plone/app/content/browser/content_status_history.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/content_status_modify.py` & `plone_app_content-4.1.3/plone/app/content/browser/content_status_modify.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/contents/__init__.py` & `plone_app_content-4.1.3/plone/app/content/browser/contents/__init__.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/contents/configure.zcml` & `plone_app_content-4.1.3/plone/app/content/browser/contents/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/contents/copy.py` & `plone_app_content-4.1.3/plone/app/content/browser/contents/copy.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/contents/cut.py` & `plone_app_content-4.1.3/plone/app/content/browser/contents/cut.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/contents/defaultpage.py` & `plone_app_content-4.1.3/plone/app/content/browser/contents/defaultpage.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/contents/delete.py` & `plone_app_content-4.1.3/plone/app/content/browser/contents/delete.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/contents/paste.py` & `plone_app_content-4.1.3/plone/app/content/browser/contents/paste.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/contents/properties.py` & `plone_app_content-4.1.3/plone/app/content/browser/contents/properties.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/contents/rearrange.py` & `plone_app_content-4.1.3/plone/app/content/browser/contents/rearrange.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/contents/rename.py` & `plone_app_content-4.1.3/plone/app/content/browser/contents/rename.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/contents/tags.py` & `plone_app_content-4.1.3/plone/app/content/browser/contents/tags.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/contents/templates/folder_contents.pt` & `plone_app_content-4.1.3/plone/app/content/browser/contents/templates/folder_contents.pt`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/contents/templates/properties.pt` & `plone_app_content-4.1.3/plone/app/content/browser/contents/templates/properties.pt`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/contents/templates/rename.pt` & `plone_app_content-4.1.3/plone/app/content/browser/contents/templates/rename.pt`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/contents/templates/tags.pt` & `plone_app_content-4.1.3/plone/app/content/browser/contents/templates/tags.pt`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/contents/templates/workflow.pt` & `plone_app_content-4.1.3/plone/app/content/browser/contents/templates/workflow.pt`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/contents/workflow.py` & `plone_app_content-4.1.3/plone/app/content/browser/contents/workflow.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/file.py` & `plone_app_content-4.1.3/plone/app/content/browser/file.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/folder_publish.py` & `plone_app_content-4.1.3/plone/app/content/browser/folder_publish.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/folderfactories.pt` & `plone_app_content-4.1.3/plone/app/content/browser/folderfactories.pt`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/folderfactories.py` & `plone_app_content-4.1.3/plone/app/content/browser/folderfactories.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/full_review_list.pt` & `plone_app_content-4.1.3/plone/app/content/browser/full_review_list.pt`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/i18n.py` & `plone_app_content-4.1.3/plone/app/content/browser/i18n.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/query.py` & `plone_app_content-4.1.3/plone/app/content/browser/query.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/reviewlist.py` & `plone_app_content-4.1.3/plone/app/content/browser/reviewlist.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/selection.py` & `plone_app_content-4.1.3/plone/app/content/browser/selection.py`

 * *Files 13% similar despite different names*

```diff
@@ -96,17 +96,21 @@
     def get_selectable_items(self):
         """Return brains in this container that can be used as default_pages"""
         context = aq_inner(self.context)
         registry = getUtility(IRegistry)
         view_types = registry.get("plone.types_use_view_action_in_listings", [])
         default_page_types = registry.get("plone.default_page_types", [])
         portal_types = getToolByName(self.context, "portal_types")
+        portal_catalog = getToolByName(self.context, "portal_catalog")
 
         results = []
-        for brain in context.getFolderContents():
+        for brain in portal_catalog(
+            path={"query": context.absolute_url_path(), "depth": 1},
+            sort_on="getObjPositionInParent",
+        ):
             portal_type = brain.portal_type
             if portal_type in view_types:
                 # Skip files and images
                 continue
 
             if portal_type in default_page_types:
                 # Allow types that are explicitly in default_page_types
```

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/table.pt` & `plone_app_content-4.1.3/plone/app/content/browser/table.pt`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/table.txt` & `plone_app_content-4.1.3/plone/app/content/browser/table.txt`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/tableview.py` & `plone_app_content-4.1.3/plone/app/content/browser/tableview.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/templates/content_status_history.pt` & `plone_app_content-4.1.3/plone/app/content/browser/templates/content_status_history.pt`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/templates/delete_confirmation.pt` & `plone_app_content-4.1.3/plone/app/content/browser/templates/delete_confirmation.pt`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/templates/object_rename.pt` & `plone_app_content-4.1.3/plone/app/content/browser/templates/object_rename.pt`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/templates/select_default_page.pt` & `plone_app_content-4.1.3/plone/app/content/browser/templates/select_default_page.pt`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/templates/select_default_view.pt` & `plone_app_content-4.1.3/plone/app/content/browser/templates/select_default_view.pt`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/browser/vocabulary.py` & `plone_app_content-4.1.3/plone/app/content/browser/vocabulary.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/configure.zcml` & `plone_app_content-4.1.3/plone/app/content/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/interfaces.py` & `plone_app_content-4.1.3/plone/app/content/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/namechooser.py` & `plone_app_content-4.1.3/plone/app/content/namechooser.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/namechooser.txt` & `plone_app_content-4.1.3/plone/app/content/namechooser.txt`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/testing.py` & `plone_app_content-4.1.3/plone/app/content/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/tests/image.png` & `plone_app_content-4.1.3/plone/app/content/tests/image.png`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/tests/profiles/non-ascii-workflow-profile/workflows/non-ascii-workflow/definition.xml` & `plone_app_content-4.1.3/plone/app/content/tests/profiles/non-ascii-workflow-profile/workflows/non-ascii-workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/tests/test_actions.py` & `plone_app_content-4.1.3/plone/app/content/tests/test_actions.py`

 * *Files identical despite different names*

```diff
@@ -230,15 +230,15 @@
         self.assertEqual(folder.getDefaultPage(), "d1")
 
         # We need zope2.CopyOrMove permission to rename content
         self.browser.open(doc.absolute_url() + "/object_rename")
         self.browser.getControl(name="form.widgets.new_id").value = " ?renamed"
         self.browser.getControl(name="form.widgets.new_title").value = "Doc"
         self.browser.getControl(name="form.buttons.Rename").click()
-        self.assertEqual(folder.getFolderContents()[0].id, "renamed")
+        self.assertEqual(folder.contentIds()[0], "renamed")
         self.assertEqual(folder.getDefaultPage(), "renamed")
 
     def test_rename_form_cancel(self):
         folder = self.portal["f1"]
 
         _id = folder.getId()
         _title = folder.Title()
```

### Comparing `plone.app.content-4.1.2/plone/app/content/tests/test_adding.py` & `plone_app_content-4.1.3/plone/app/content/tests/test_adding.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/tests/test_constrains.py` & `plone_app_content-4.1.3/plone/app/content/tests/test_constrains.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/tests/test_content_status_modify.py` & `plone_app_content-4.1.3/plone/app/content/tests/test_content_status_modify.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/tests/test_contents.py` & `plone_app_content-4.1.3/plone/app/content/tests/test_contents.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/tests/test_folder.py` & `plone_app_content-4.1.3/plone/app/content/tests/test_folder.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/tests/test_folder_publish.py` & `plone_app_content-4.1.3/plone/app/content/tests/test_folder_publish.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/tests/test_namechooser_unit.py` & `plone_app_content-4.1.3/plone/app/content/tests/test_namechooser_unit.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/tests/test_non_ascii_characters_in_workflow_state.py` & `plone_app_content-4.1.3/plone/app/content/tests/test_non_ascii_characters_in_workflow_state.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/tests/test_permissions.py` & `plone_app_content-4.1.3/plone/app/content/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/tests/test_reviewlist.py` & `plone_app_content-4.1.3/plone/app/content/tests/test_reviewlist.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/tests/test_selectdefaultpage.py` & `plone_app_content-4.1.3/plone/app/content/tests/test_selectdefaultpage.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/tests/test_widgets.py` & `plone_app_content-4.1.3/plone/app/content/tests/test_widgets.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone/app/content/utils.py` & `plone_app_content-4.1.3/plone/app/content/utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/plone.app.content.egg-info/PKG-INFO` & `plone_app_content-4.1.3/plone.app.content.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.content
-Version: 4.1.2
+Version: 4.1.3
 Summary: Content Views for Plone
 Home-page: https://pypi.org/project/plone.app.content
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone content views viewlet
 Classifier: Development Status :: 5 - Production/Stable
@@ -75,14 +75,23 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.1.3 (2024-05-30)
+------------------
+
+Bug fixes:
+
+
+- Remove usage of CMFPlone skins script [@jensens] (#281)
+
+
 4.1.2 (2024-02-12)
 ------------------
 
 Bug fixes:
 
 
 - Fix escaping HTML in ``tags`` popover.
```

### Comparing `plone.app.content-4.1.2/plone.app.content.egg-info/SOURCES.txt` & `plone_app_content-4.1.3/plone.app.content.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/pyproject.toml` & `plone_app_content-4.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.1.2/setup.py` & `plone_app_content-4.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "4.1.2"
+version = "4.1.3"
 
 setup(
     name="plone.app.content",
     version=version,
     description="Content Views for Plone",
     long_description="\n\n".join(
         [
```

