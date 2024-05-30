# Comparing `tmp/plone.app.contentrules-5.0.3.tar.gz` & `tmp/plone_app_contentrules-5.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.contentrules-5.0.3.tar", last modified: Fri Oct  6 22:47:56 2023, max compression
+gzip compressed data, was "plone_app_contentrules-5.0.4.tar", last modified: Thu May 30 18:28:34 2024, max compression
```

## Comparing `plone.app.contentrules-5.0.3.tar` & `plone_app_contentrules-5.0.4.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:47:56.027495 plone.app.contentrules-5.0.3/
--rw-r--r--   0 maurits    (501) staff       (20)    20350 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      148 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    22669 2023-10-06 22:47:56.026853 plone.app.contentrules-5.0.3/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      527 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:47:55.982345 plone.app.contentrules-5.0.3/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      684 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:47:55.982784 plone.app.contentrules-5.0.3/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:47:55.986526 plone.app.contentrules-5.0.3/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:47:55.989700 plone.app.contentrules-5.0.3/plone/app/contentrules/
--rw-r--r--   0 maurits    (501) staff       (20)      162 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:47:55.994461 plone.app.contentrules-5.0.3/plone/app/contentrules/actions/
--rw-r--r--   0 maurits    (501) staff       (20)     1923 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/actions/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     6880 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/actions/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     4835 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/actions/copy.py
--rw-r--r--   0 maurits    (501) staff       (20)     2197 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/actions/delete.py
--rw-r--r--   0 maurits    (501) staff       (20)     4143 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/actions/logger.py
--rw-r--r--   0 maurits    (501) staff       (20)     7188 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/actions/mail.py
--rw-r--r--   0 maurits    (501) staff       (20)     5694 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/actions/move.py
--rw-r--r--   0 maurits    (501) staff       (20)     2887 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/actions/notify.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:47:55.994918 plone.app.contentrules-5.0.3/plone/app/contentrules/actions/templates/
--rw-r--r--   0 maurits    (501) staff       (20)     1172 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/actions/templates/mail.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2850 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/actions/versioning.py
--rw-r--r--   0 maurits    (501) staff       (20)     3558 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/actions/workflow.py
--rw-r--r--   0 maurits    (501) staff       (20)     2391 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/api.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:47:56.000372 plone.app.contentrules-5.0.3/plone/app/contentrules/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        2 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3799 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/browser/adding.py
--rw-r--r--   0 maurits    (501) staff       (20)     7174 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/browser/assignments.py
--rw-r--r--   0 maurits    (501) staff       (20)     5827 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     5294 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/browser/controlpanel.py
--rw-r--r--   0 maurits    (501) staff       (20)     8506 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/browser/elements.py
--rw-r--r--   0 maurits    (501) staff       (20)     5139 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/browser/formhelper.py
--rw-r--r--   0 maurits    (501) staff       (20)      842 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/browser/info.py
--rw-r--r--   0 maurits    (501) staff       (20)      990 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/browser/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      827 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/browser/navigation.py
--rw-r--r--   0 maurits    (501) staff       (20)     1895 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/browser/rule.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:47:56.002212 plone.app.contentrules-5.0.3/plone/app/contentrules/browser/templates/
--rw-r--r--   0 maurits    (501) staff       (20)      968 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/browser/templates/contentrules-pageform.pt
--rw-r--r--   0 maurits    (501) staff       (20)    14016 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/browser/templates/controlpanel.pt
--rw-r--r--   0 maurits    (501) staff       (20)    14486 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/browser/templates/manage-assignments.pt
--rw-r--r--   0 maurits    (501) staff       (20)    15756 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/browser/templates/manage-elements.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2166 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/browser/traversal.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:47:56.006238 plone.app.contentrules-5.0.3/plone/app/contentrules/conditions/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/conditions/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     7283 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/conditions/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     3435 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/conditions/fileextension.py
--rw-r--r--   0 maurits    (501) staff       (20)     3313 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/conditions/group.py
--rw-r--r--   0 maurits    (501) staff       (20)     3773 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/conditions/portaltype.py
--rw-r--r--   0 maurits    (501) staff       (20)     3170 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/conditions/role.py
--rw-r--r--   0 maurits    (501) staff       (20)     3439 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/conditions/talesexpression.py
--rw-r--r--   0 maurits    (501) staff       (20)     3201 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/conditions/wfstate.py
--rw-r--r--   0 maurits    (501) staff       (20)     3148 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/conditions/wftransition.py
--rw-r--r--   0 maurits    (501) staff       (20)     5009 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:47:56.008024 plone.app.contentrules-5.0.3/plone/app/contentrules/exportimport/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/exportimport/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      891 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/exportimport/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      745 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/exportimport/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)    13594 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/exportimport/rules.py
--rw-r--r--   0 maurits    (501) staff       (20)     6057 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/handlers.py
--rw-r--r--   0 maurits    (501) staff       (20)      704 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/namechooser.py
--rw-r--r--   0 maurits    (501) staff       (20)     3137 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/rule.py
--rw-r--r--   0 maurits    (501) staff       (20)      962 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:47:56.023888 plone.app.contentrules-5.0.3/plone/app/contentrules/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     4025 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/tests/assignment.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1403 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/tests/base.py
--rw-r--r--   0 maurits    (501) staff       (20)      761 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/tests/dummy.py
--rw-r--r--   0 maurits    (501) staff       (20)     4021 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/tests/multipublish.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:47:55.978313 plone.app.contentrules-5.0.3/plone/app/contentrules/tests/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:47:56.025342 plone.app.contentrules-5.0.3/plone/app/contentrules/tests/profiles/testing/
--rw-r--r--   0 maurits    (501) staff       (20)     3556 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/tests/profiles/testing/contentrules.xml
--rw-r--r--   0 maurits    (501) staff       (20)      264 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/tests/profiles/testing/export_steps.xml
--rw-r--r--   0 maurits    (501) staff       (20)      346 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/tests/profiles/testing/import_steps.xml
--rw-r--r--   0 maurits    (501) staff       (20)     3447 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/tests/simplepublish.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4683 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_action_copy.py
--rw-r--r--   0 maurits    (501) staff       (20)     1821 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_action_delete.py
--rw-r--r--   0 maurits    (501) staff       (20)     3481 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_action_logger.py
--rw-r--r--   0 maurits    (501) staff       (20)     9521 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_action_mail.py
--rw-r--r--   0 maurits    (501) staff       (20)     1079 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_action_modify.py
--rw-r--r--   0 maurits    (501) staff       (20)     5419 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_action_move.py
--rw-r--r--   0 maurits    (501) staff       (20)     2686 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_action_notify.py
--rw-r--r--   0 maurits    (501) staff       (20)     2757 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_action_versioning.py
--rw-r--r--   0 maurits    (501) staff       (20)     3068 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_action_workflow.py
--rw-r--r--   0 maurits    (501) staff       (20)      663 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_browser.py
--rw-r--r--   0 maurits    (501) staff       (20)     1653 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_cascading_rule.py
--rw-r--r--   0 maurits    (501) staff       (20)     2588 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_condition_group.py
--rw-r--r--   0 maurits    (501) staff       (20)     2809 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_condition_portal_type.py
--rw-r--r--   0 maurits    (501) staff       (20)     2479 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_condition_role.py
--rw-r--r--   0 maurits    (501) staff       (20)     3086 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_condition_tales_expression.py
--rw-r--r--   0 maurits    (501) staff       (20)     2749 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_condition_wfstate.py
--rw-r--r--   0 maurits    (501) staff       (20)     3441 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_condition_wftransition.py
--rw-r--r--   0 maurits    (501) staff       (20)     8131 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_configuration.py
--rw-r--r--   0 maurits    (501) staff       (20)      288 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_events.py
--rw-r--r--   0 maurits    (501) staff       (20)     1652 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_handlers.py
--rw-r--r--   0 maurits    (501) staff       (20)     5713 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_rule_assignment_mapping.py
--rw-r--r--   0 maurits    (501) staff       (20)     6123 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_rule_management_views.py
--rw-r--r--   0 maurits    (501) staff       (20)      857 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_setup.py
--rw-r--r--   0 maurits    (501) staff       (20)     1926 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_traversal.py
--rw-r--r--   0 maurits    (501) staff       (20)     2743 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_ui.txt
--rw-r--r--   0 maurits    (501) staff       (20)      482 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/tests/testing.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      155 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/plone/app/contentrules/tests/utils.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:47:55.986074 plone.app.contentrules-5.0.3/plone.app.contentrules.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    22669 2023-10-06 22:47:55.000000 plone.app.contentrules-5.0.3/plone.app.contentrules.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     4388 2023-10-06 22:47:55.000000 plone.app.contentrules-5.0.3/plone.app.contentrules.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-10-06 22:47:55.000000 plone.app.contentrules-5.0.3/plone.app.contentrules.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2023-10-06 22:47:55.000000 plone.app.contentrules-5.0.3/plone.app.contentrules.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-10-06 22:47:55.000000 plone.app.contentrules-5.0.3/plone.app.contentrules.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      392 2023-10-06 22:47:55.000000 plone.app.contentrules-5.0.3/plone.app.contentrules.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-10-06 22:47:55.000000 plone.app.contentrules-5.0.3/plone.app.contentrules.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4232 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)       38 2023-10-06 22:47:56.027612 plone.app.contentrules-5.0.3/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2219 2023-10-06 22:47:54.000000 plone.app.contentrules-5.0.3/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:28:34.691802 plone_app_contentrules-5.0.4/
+-rw-r--r--   0 maurits    (501) staff       (20)    20495 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      148 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    22778 2024-05-30 18:28:34.691087 plone_app_contentrules-5.0.4/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      527 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:28:34.644330 plone_app_contentrules-5.0.4/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      684 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:28:34.644792 plone_app_contentrules-5.0.4/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:28:34.648625 plone_app_contentrules-5.0.4/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:28:34.651938 plone_app_contentrules-5.0.4/plone/app/contentrules/
+-rw-r--r--   0 maurits    (501) staff       (20)      162 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:28:34.656770 plone_app_contentrules-5.0.4/plone/app/contentrules/actions/
+-rw-r--r--   0 maurits    (501) staff       (20)     1923 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/actions/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6880 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/actions/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     4835 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/actions/copy.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2197 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/actions/delete.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4143 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/actions/logger.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7188 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/actions/mail.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5694 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/actions/move.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2887 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/actions/notify.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:28:34.657239 plone_app_contentrules-5.0.4/plone/app/contentrules/actions/templates/
+-rw-r--r--   0 maurits    (501) staff       (20)     1172 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/actions/templates/mail.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2850 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/actions/versioning.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3558 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/actions/workflow.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2391 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/api.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:28:34.663297 plone_app_contentrules-5.0.4/plone/app/contentrules/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        2 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3799 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/browser/adding.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7174 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/browser/assignments.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5827 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     5294 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/browser/controlpanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8506 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/browser/elements.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5139 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/browser/formhelper.py
+-rw-r--r--   0 maurits    (501) staff       (20)      842 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/browser/info.py
+-rw-r--r--   0 maurits    (501) staff       (20)      990 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/browser/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      827 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/browser/navigation.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1895 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/browser/rule.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:28:34.665417 plone_app_contentrules-5.0.4/plone/app/contentrules/browser/templates/
+-rw-r--r--   0 maurits    (501) staff       (20)      968 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/browser/templates/contentrules-pageform.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    14016 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/browser/templates/controlpanel.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    14486 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/browser/templates/manage-assignments.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    15756 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/browser/templates/manage-elements.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2166 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/browser/traversal.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:28:34.669777 plone_app_contentrules-5.0.4/plone/app/contentrules/conditions/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/conditions/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7283 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/conditions/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     3435 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/conditions/fileextension.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3313 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/conditions/group.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3773 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/conditions/portaltype.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3170 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/conditions/role.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3439 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/conditions/talesexpression.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3201 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/conditions/wfstate.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3148 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/conditions/wftransition.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5009 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:28:34.671507 plone_app_contentrules-5.0.4/plone/app/contentrules/exportimport/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/exportimport/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      891 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/exportimport/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      745 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/exportimport/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)    13594 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/exportimport/rules.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6209 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/handlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)      704 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/namechooser.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3137 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/rule.py
+-rw-r--r--   0 maurits    (501) staff       (20)      962 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:28:34.687312 plone_app_contentrules-5.0.4/plone/app/contentrules/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4025 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/tests/assignment.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1404 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/tests/base.py
+-rw-r--r--   0 maurits    (501) staff       (20)      761 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/tests/dummy.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4021 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/tests/multipublish.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:28:34.640432 plone_app_contentrules-5.0.4/plone/app/contentrules/tests/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:28:34.688769 plone_app_contentrules-5.0.4/plone/app/contentrules/tests/profiles/testing/
+-rw-r--r--   0 maurits    (501) staff       (20)     3556 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/tests/profiles/testing/contentrules.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      264 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/tests/profiles/testing/export_steps.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      346 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/tests/profiles/testing/import_steps.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     3447 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/tests/simplepublish.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4683 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_action_copy.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1821 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_action_delete.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3481 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_action_logger.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9521 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_action_mail.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1079 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_action_modify.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5419 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_action_move.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2686 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_action_notify.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2757 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_action_versioning.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3068 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_action_workflow.py
+-rw-r--r--   0 maurits    (501) staff       (20)      663 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_browser.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1653 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_cascading_rule.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2588 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_condition_group.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2809 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_condition_portal_type.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2479 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_condition_role.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3086 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_condition_tales_expression.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2749 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_condition_wfstate.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3441 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_condition_wftransition.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8131 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_configuration.py
+-rw-r--r--   0 maurits    (501) staff       (20)      288 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_events.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1652 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_handlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5713 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_rule_assignment_mapping.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6123 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_rule_management_views.py
+-rw-r--r--   0 maurits    (501) staff       (20)      857 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_setup.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1926 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_traversal.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2743 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_ui.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      482 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/tests/testing.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      155 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/plone/app/contentrules/tests/utils.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:28:34.689378 plone_app_contentrules-5.0.4/plone.app.contentrules.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    22778 2024-05-30 18:28:34.000000 plone_app_contentrules-5.0.4/plone.app.contentrules.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     4388 2024-05-30 18:28:34.000000 plone_app_contentrules-5.0.4/plone.app.contentrules.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-05-30 18:28:34.000000 plone_app_contentrules-5.0.4/plone.app.contentrules.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2024-05-30 18:28:34.000000 plone_app_contentrules-5.0.4/plone.app.contentrules.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-05-30 18:28:34.000000 plone_app_contentrules-5.0.4/plone.app.contentrules.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      371 2024-05-30 18:28:34.000000 plone_app_contentrules-5.0.4/plone.app.contentrules.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-05-30 18:28:34.000000 plone_app_contentrules-5.0.4/plone.app.contentrules.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4254 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2024-05-30 18:28:34.691933 plone_app_contentrules-5.0.4/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2187 2024-05-30 18:28:33.000000 plone_app_contentrules-5.0.4/setup.py
```

### Comparing `plone.app.contentrules-5.0.3/CHANGES.rst` & `plone_app_contentrules-5.0.4/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,23 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.0.4 (2024-05-30)
+------------------
+
+Bug fixes:
+
+
+- Remove hard dependency on plone.app.discussion. [@jensens] (rm-pa-discussion-dependency)
+
+
 5.0.3 (2023-10-07)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.app.contentrules-5.0.3/PKG-INFO` & `plone_app_contentrules-5.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.contentrules
-Version: 5.0.3
+Version: 5.0.4
 Summary: Plone integration for plone.contentrules
 Home-page: https://pypi.org/project/plone.app.contentrules
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone automatic content rules
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,15 +20,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Requires-Dist: lxml
 Requires-Dist: plone.app.contenttypes
-Requires-Dist: plone.app.discussion
 Requires-Dist: plone.app.uuid
 Requires-Dist: plone.app.vocabularies
 Requires-Dist: plone.autoform
 Requires-Dist: plone.base
 Requires-Dist: plone.contentrules
 Requires-Dist: plone.memoize
 Requires-Dist: plone.stringinterp
@@ -68,14 +67,23 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.0.4 (2024-05-30)
+------------------
+
+Bug fixes:
+
+
+- Remove hard dependency on plone.app.discussion. [@jensens] (rm-pa-discussion-dependency)
+
+
 5.0.3 (2023-10-07)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.app.contentrules-5.0.3/README.rst` & `plone_app_contentrules-5.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/docs/LICENSE.GPL` & `plone_app_contentrules-5.0.4/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/docs/LICENSE.txt` & `plone_app_contentrules-5.0.4/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/actions/__init__.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/actions/configure.zcml` & `plone_app_contentrules-5.0.4/plone/app/contentrules/actions/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/actions/copy.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/actions/copy.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/actions/delete.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/actions/delete.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/actions/logger.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/actions/logger.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/actions/mail.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/actions/mail.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/actions/move.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/actions/move.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/actions/notify.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/actions/notify.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/actions/templates/mail.pt` & `plone_app_contentrules-5.0.4/plone/app/contentrules/actions/templates/mail.pt`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/actions/versioning.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/actions/versioning.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/actions/workflow.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/actions/workflow.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/api.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/api.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/browser/adding.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/browser/adding.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/browser/assignments.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/browser/assignments.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/browser/configure.zcml` & `plone_app_contentrules-5.0.4/plone/app/contentrules/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/browser/controlpanel.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/browser/elements.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/browser/elements.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/browser/formhelper.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/browser/formhelper.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/browser/info.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/browser/info.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/browser/interfaces.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/browser/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/browser/navigation.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/browser/navigation.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/browser/rule.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/browser/rule.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/browser/templates/contentrules-pageform.pt` & `plone_app_contentrules-5.0.4/plone/app/contentrules/browser/templates/contentrules-pageform.pt`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/browser/templates/controlpanel.pt` & `plone_app_contentrules-5.0.4/plone/app/contentrules/browser/templates/controlpanel.pt`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/browser/templates/manage-assignments.pt` & `plone_app_contentrules-5.0.4/plone/app/contentrules/browser/templates/manage-assignments.pt`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/browser/templates/manage-elements.pt` & `plone_app_contentrules-5.0.4/plone/app/contentrules/browser/templates/manage-elements.pt`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/browser/traversal.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/browser/traversal.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/conditions/configure.zcml` & `plone_app_contentrules-5.0.4/plone/app/contentrules/conditions/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/conditions/fileextension.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/conditions/fileextension.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/conditions/group.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/conditions/group.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/conditions/portaltype.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/conditions/portaltype.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/conditions/role.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/conditions/role.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/conditions/talesexpression.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/conditions/talesexpression.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/conditions/wfstate.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/conditions/wfstate.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/conditions/wftransition.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/conditions/wftransition.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/configure.zcml` & `plone_app_contentrules-5.0.4/plone/app/contentrules/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/exportimport/configure.zcml` & `plone_app_contentrules-5.0.4/plone/app/contentrules/exportimport/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/exportimport/interfaces.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/exportimport/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/exportimport/rules.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/exportimport/rules.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/handlers.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 from Acquisition import aq_inner
 from Acquisition import aq_parent
-from plone.app.discussion.interfaces import IComment
 from plone.contentrules.engine.interfaces import IRuleExecutor
 from plone.contentrules.engine.interfaces import IRuleStorage
 from plone.contentrules.engine.interfaces import StopRule
 from plone.uuid.interfaces import IUUID
 from Products.CMFCore.interfaces import IContentish
 from Products.CMFCore.interfaces import ISiteRoot
 from zope.component import queryUtility
 from zope.component.hooks import getSite
 from zope.container.interfaces import IContainerModifiedEvent
 from zope.container.interfaces import IObjectAddedEvent
 from zope.container.interfaces import IObjectRemovedEvent
+from zope.interface import Interface
 from zope.lifecycleevent.interfaces import IObjectCopiedEvent
 
 import threading
 
 
+try:
+    from plone.app.discussion.interfaces import IComment
+except ImportError:
+
+    class IComment(Interface):
+        """Dummy interface if there is no plone.app.discussion available."""
+
+
 def _get_uid(context):
     uid = IUUID(context, None)
     if uid is not None:
         return uid
 
     try:
         return "/".join(context.getPhysicalPath())
@@ -138,16 +146,14 @@
 
 def added(event):
     """When an object is added, execute rules assigned to its new parent."""
     obj = event.object
 
     if IContentish.providedBy(obj) or IComment.providedBy(obj):
         execute(event.newParent, event)
-    else:
-        return
 
 
 def removed(event):
     """When an IObjectRemovedEvent was received, execute rules assigned to its
     previous parent.
     """
     obj = event.object
```

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/namechooser.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/namechooser.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/rule.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/rule.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/testing.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/tests/assignment.txt` & `plone_app_contentrules-5.0.4/plone/app/contentrules/tests/assignment.txt`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/tests/base.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/tests/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Base class for integration tests, based on plone.app.testing
 """
+
 from plone.app.contentrules.testing import (  # noqa: E501
     PLONE_APP_CONTENTRULES_INTEGRATION_TESTING,
 )
 from plone.app.testing import login
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from plone.app.testing import TEST_USER_NAME
```

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/tests/dummy.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/tests/dummy.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/tests/multipublish.txt` & `plone_app_contentrules-5.0.4/plone/app/contentrules/tests/multipublish.txt`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/tests/profiles/testing/contentrules.xml` & `plone_app_contentrules-5.0.4/plone/app/contentrules/tests/profiles/testing/contentrules.xml`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/tests/simplepublish.txt` & `plone_app_contentrules-5.0.4/plone/app/contentrules/tests/simplepublish.txt`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_action_copy.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_action_copy.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_action_delete.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_action_delete.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_action_logger.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_action_logger.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_action_mail.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_action_mail.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_action_modify.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_action_modify.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_action_move.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_action_move.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_action_notify.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_action_notify.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_action_versioning.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_action_versioning.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_action_workflow.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_action_workflow.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_browser.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_browser.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_cascading_rule.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_cascading_rule.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_condition_group.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_condition_group.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_condition_portal_type.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_condition_portal_type.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_condition_role.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_condition_role.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_condition_tales_expression.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_condition_tales_expression.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_condition_wfstate.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_condition_wfstate.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_condition_wftransition.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_condition_wftransition.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_configuration.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_handlers.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_rule_assignment_mapping.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_rule_assignment_mapping.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_rule_management_views.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_rule_management_views.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_setup.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_traversal.py` & `plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_traversal.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone/app/contentrules/tests/test_ui.txt` & `plone_app_contentrules-5.0.4/plone/app/contentrules/tests/test_ui.txt`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/plone.app.contentrules.egg-info/PKG-INFO` & `plone_app_contentrules-5.0.4/plone.app.contentrules.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.contentrules
-Version: 5.0.3
+Version: 5.0.4
 Summary: Plone integration for plone.contentrules
 Home-page: https://pypi.org/project/plone.app.contentrules
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone automatic content rules
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,15 +20,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Requires-Dist: lxml
 Requires-Dist: plone.app.contenttypes
-Requires-Dist: plone.app.discussion
 Requires-Dist: plone.app.uuid
 Requires-Dist: plone.app.vocabularies
 Requires-Dist: plone.autoform
 Requires-Dist: plone.base
 Requires-Dist: plone.contentrules
 Requires-Dist: plone.memoize
 Requires-Dist: plone.stringinterp
@@ -68,14 +67,23 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.0.4 (2024-05-30)
+------------------
+
+Bug fixes:
+
+
+- Remove hard dependency on plone.app.discussion. [@jensens] (rm-pa-discussion-dependency)
+
+
 5.0.3 (2023-10-07)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.app.contentrules-5.0.3/plone.app.contentrules.egg-info/SOURCES.txt` & `plone_app_contentrules-5.0.4/plone.app.contentrules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.3/pyproject.toml` & `plone_app_contentrules-5.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
   'zope.sendmail', 'Zope'
 ]
 'plone.base' = [
   'plone.batching', 'plone.registry', 'plone.schema','plone.z3cform',
   'Products.CMFCore', 'Products.CMFDynamicViewFTI',
 ]
 python-dateutil = ['dateutil']
-ignore-packages = ['Products.CMFPlone',]
+ignore-packages = ['Products.CMFPlone','plone.app.discussion']
 
 ##
 # Add extra configuration options in .meta.toml:
 #  [pyproject]
 #  dependencies_ignores = "['zestreleaser.towncrier']"
 #  dependencies_mappings = [
 #    "gitpython = ['git']",
```

### Comparing `plone.app.contentrules-5.0.3/setup.py` & `plone_app_contentrules-5.0.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "5.0.3"
+version = "5.0.4"
 
 long_description = (
     f"{Path('README.rst').read_text()}\n{Path('CHANGES.rst').read_text()}"
 )
 
 setup(
     name="plone.app.contentrules",
@@ -49,15 +49,14 @@
             "plone.dexterity",
             "plone.testing",
         ]
     },
     install_requires=[
         "lxml",
         "plone.app.contenttypes",
-        "plone.app.discussion",
         "plone.app.uuid",
         "plone.app.vocabularies",
         "plone.autoform",
         "plone.base",
         "plone.contentrules",
         "plone.memoize",
         "plone.stringinterp",
```

