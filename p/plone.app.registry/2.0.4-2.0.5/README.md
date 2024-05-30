# Comparing `tmp/plone.app.registry-2.0.4.tar.gz` & `tmp/plone_app_registry-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.registry-2.0.4.tar", last modified: Thu Dec 14 09:57:05 2023, max compression
+gzip compressed data, was "plone_app_registry-2.0.5.tar", last modified: Thu May 30 18:32:06 2024, max compression
```

## Comparing `plone.app.registry-2.0.4.tar` & `plone_app_registry-2.0.5.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-14 09:57:05.678094 plone.app.registry-2.0.4/
--rw-r--r--   0 maurits    (501) staff       (20)    11258 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      149 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    40679 2023-12-14 09:57:05.677591 plone.app.registry-2.0.4/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)    27968 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-14 09:57:05.659536 plone.app.registry-2.0.4/docs/
--rw-r--r--   0 maurits    (501) staff       (20)     1112 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/docs/INSTALL.txt
--rw-r--r--   0 maurits    (501) staff       (20)    12282 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      747 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)    78923 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/docs/configuration_registry_add_record_screenshot.jpg
--rw-r--r--   0 maurits    (501) staff       (20)    55440 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/docs/configuration_registry_edit_record_screenshot.jpg
--rw-r--r--   0 maurits    (501) staff       (20)    52471 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/docs/configuration_registry_export_screenshot.jpg
--rw-r--r--   0 maurits    (501) staff       (20)    55001 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/docs/configuration_registry_import_screenshot.jpg
--rw-r--r--   0 maurits    (501) staff       (20)   152613 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/docs/configuration_registry_screenshot.jpg
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-14 09:57:05.659963 plone.app.registry-2.0.4/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-14 09:57:05.662542 plone.app.registry-2.0.4/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-14 09:57:05.664449 plone.app.registry-2.0.4/plone/app/registry/
--rw-r--r--   0 maurits    (501) staff       (20)     1791 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/plone/app/registry/README.txt
--rw-r--r--   0 maurits    (501) staff       (20)       63 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/plone/app/registry/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-14 09:57:05.666905 plone.app.registry-2.0.4/plone/app/registry/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/plone/app/registry/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1284 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/plone/app/registry/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2935 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/plone/app/registry/browser/controlpanel.py
--rw-r--r--   0 maurits    (501) staff       (20)      972 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/plone/app/registry/browser/delete.py
--rw-r--r--   0 maurits    (501) staff       (20)     2380 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/plone/app/registry/browser/edit.py
--rw-r--r--   0 maurits    (501) staff       (20)     4958 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/plone/app/registry/browser/exportxml.py
--rw-r--r--   0 maurits    (501) staff       (20)     7845 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/plone/app/registry/browser/records.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-14 09:57:05.667518 plone.app.registry-2.0.4/plone/app/registry/browser/resources/
--rw-r--r--   0 maurits    (501) staff       (20)      267 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/plone/app/registry/browser/resources/icon.png
--rw-r--r--   0 maurits    (501) staff       (20)      490 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/plone/app/registry/browser/resources/style.css
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-14 09:57:05.669223 plone.app.registry-2.0.4/plone/app/registry/browser/templates/
--rw-r--r--   0 maurits    (501) staff       (20)      965 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/plone/app/registry/browser/templates/controlpanel_layout.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1854 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/plone/app/registry/browser/templates/delete_layout.pt
--rw-r--r--   0 maurits    (501) staff       (20)      993 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/plone/app/registry/browser/templates/edit_layout.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1200 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/plone/app/registry/browser/templates/exportxml.pt
--rw-r--r--   0 maurits    (501) staff       (20)    10030 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/plone/app/registry/browser/templates/records.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1029 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/plone/app/registry/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-14 09:57:05.671668 plone.app.registry-2.0.4/plone/app/registry/exportimport/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/plone/app/registry/exportimport/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      931 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/plone/app/registry/exportimport/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2008 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/plone/app/registry/exportimport/fields.py
--rw-r--r--   0 maurits    (501) staff       (20)    16153 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/plone/app/registry/exportimport/handler.py
--rw-r--r--   0 maurits    (501) staff       (20)     2503 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/plone/app/registry/exportimport/handlers.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-14 09:57:05.654873 plone.app.registry-2.0.4/plone/app/registry/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-14 09:57:05.673450 plone.app.registry-2.0.4/plone/app/registry/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      230 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/plone/app/registry/profiles/default/componentregistry.xml
--rw-r--r--   0 maurits    (501) staff       (20)      594 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/plone/app/registry/profiles/default/controlpanel.xml
--rw-r--r--   0 maurits    (501) staff       (20)      187 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/plone/app/registry/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)      166 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/plone/app/registry/profiles/default/toolset.xml
--rw-r--r--   0 maurits    (501) staff       (20)      274 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/plone/app/registry/registry.py
--rw-r--r--   0 maurits    (501) staff       (20)      818 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/plone/app/registry/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-14 09:57:05.676012 plone.app.registry-2.0.4/plone/app/registry/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/plone/app/registry/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      408 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/plone/app/registry/tests/data.py
--rw-r--r--   0 maurits    (501) staff       (20)     3546 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/plone/app/registry/tests/test_controlpanel.py
--rw-r--r--   0 maurits    (501) staff       (20)    46848 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/plone/app/registry/tests/test_exportimport.py
--rw-r--r--   0 maurits    (501) staff       (20)      711 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/plone/app/registry/tests/test_setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-14 09:57:05.676620 plone.app.registry-2.0.4/plone.app.registry.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    40679 2023-12-14 09:57:05.000000 plone.app.registry-2.0.4/plone.app.registry.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     2137 2023-12-14 09:57:05.000000 plone.app.registry-2.0.4/plone.app.registry.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-12-14 09:57:05.000000 plone.app.registry-2.0.4/plone.app.registry.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2023-12-14 09:57:05.000000 plone.app.registry-2.0.4/plone.app.registry.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-12-14 09:57:05.000000 plone.app.registry-2.0.4/plone.app.registry.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      232 2023-12-14 09:57:05.000000 plone.app.registry-2.0.4/plone.app.registry.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-12-14 09:57:05.000000 plone.app.registry-2.0.4/plone.app.registry.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4232 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)       38 2023-12-14 09:57:05.678164 plone.app.registry-2.0.4/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1996 2023-12-14 09:57:04.000000 plone.app.registry-2.0.4/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:32:06.125087 plone_app_registry-2.0.5/
+-rw-r--r--   0 maurits    (501) staff       (20)    11446 2024-05-30 18:32:04.000000 plone_app_registry-2.0.5/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2024-05-30 18:32:04.000000 plone_app_registry-2.0.5/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      149 2024-05-30 18:32:04.000000 plone_app_registry-2.0.5/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    40867 2024-05-30 18:32:06.124356 plone_app_registry-2.0.5/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)    27968 2024-05-30 18:32:04.000000 plone_app_registry-2.0.5/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:32:06.101653 plone_app_registry-2.0.5/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)     1112 2024-05-30 18:32:04.000000 plone_app_registry-2.0.5/docs/INSTALL.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    12282 2024-05-30 18:32:04.000000 plone_app_registry-2.0.5/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      747 2024-05-30 18:32:04.000000 plone_app_registry-2.0.5/docs/LICENSE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    78923 2024-05-30 18:32:04.000000 plone_app_registry-2.0.5/docs/configuration_registry_add_record_screenshot.jpg
+-rw-r--r--   0 maurits    (501) staff       (20)    55440 2024-05-30 18:32:04.000000 plone_app_registry-2.0.5/docs/configuration_registry_edit_record_screenshot.jpg
+-rw-r--r--   0 maurits    (501) staff       (20)    52471 2024-05-30 18:32:04.000000 plone_app_registry-2.0.5/docs/configuration_registry_export_screenshot.jpg
+-rw-r--r--   0 maurits    (501) staff       (20)    55001 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/docs/configuration_registry_import_screenshot.jpg
+-rw-r--r--   0 maurits    (501) staff       (20)   152613 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/docs/configuration_registry_screenshot.jpg
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:32:06.102431 plone_app_registry-2.0.5/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:32:06.106281 plone_app_registry-2.0.5/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:32:06.108632 plone_app_registry-2.0.5/plone/app/registry/
+-rw-r--r--   0 maurits    (501) staff       (20)     1791 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone/app/registry/README.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       63 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone/app/registry/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:32:06.111834 plone_app_registry-2.0.5/plone/app/registry/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone/app/registry/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1284 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone/app/registry/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2935 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone/app/registry/browser/controlpanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)      967 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone/app/registry/browser/delete.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2380 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone/app/registry/browser/edit.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4958 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone/app/registry/browser/exportxml.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7845 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone/app/registry/browser/records.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:32:06.112830 plone_app_registry-2.0.5/plone/app/registry/browser/resources/
+-rw-r--r--   0 maurits    (501) staff       (20)      267 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone/app/registry/browser/resources/icon.png
+-rw-r--r--   0 maurits    (501) staff       (20)      490 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone/app/registry/browser/resources/style.css
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:32:06.115145 plone_app_registry-2.0.5/plone/app/registry/browser/templates/
+-rw-r--r--   0 maurits    (501) staff       (20)      965 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone/app/registry/browser/templates/controlpanel_layout.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1854 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone/app/registry/browser/templates/delete_layout.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      993 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone/app/registry/browser/templates/edit_layout.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1200 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone/app/registry/browser/templates/exportxml.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    10019 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone/app/registry/browser/templates/records.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1029 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone/app/registry/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:32:06.117801 plone_app_registry-2.0.5/plone/app/registry/exportimport/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone/app/registry/exportimport/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      931 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone/app/registry/exportimport/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2008 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone/app/registry/exportimport/fields.py
+-rw-r--r--   0 maurits    (501) staff       (20)    16153 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone/app/registry/exportimport/handler.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2503 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone/app/registry/exportimport/handlers.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:32:06.093897 plone_app_registry-2.0.5/plone/app/registry/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:32:06.119781 plone_app_registry-2.0.5/plone/app/registry/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      230 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone/app/registry/profiles/default/componentregistry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      594 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone/app/registry/profiles/default/controlpanel.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      187 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone/app/registry/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      166 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone/app/registry/profiles/default/toolset.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      274 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone/app/registry/registry.py
+-rw-r--r--   0 maurits    (501) staff       (20)      818 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone/app/registry/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:32:06.122317 plone_app_registry-2.0.5/plone/app/registry/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone/app/registry/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      408 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone/app/registry/tests/data.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3546 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone/app/registry/tests/test_controlpanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)    46850 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone/app/registry/tests/test_exportimport.py
+-rw-r--r--   0 maurits    (501) staff       (20)      711 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone/app/registry/tests/test_setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:32:06.123004 plone_app_registry-2.0.5/plone.app.registry.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    40867 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone.app.registry.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     2137 2024-05-30 18:32:06.000000 plone_app_registry-2.0.5/plone.app.registry.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone.app.registry.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone.app.registry.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone.app.registry.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      232 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone.app.registry.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/plone.app.registry.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4232 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2024-05-30 18:32:06.125217 plone_app_registry-2.0.5/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1996 2024-05-30 18:32:05.000000 plone_app_registry-2.0.5/setup.py
```

### Comparing `plone.app.registry-2.0.4/CHANGES.rst` & `plone_app_registry-2.0.5/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,25 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.5 (2024-05-30)
+------------------
+
+Bug fixes:
+
+
+- Removes duplicate `<article id="content">`
+  [@szakitibi] (#84)
+- Fix misleading portal message when NOT deleting records @gforcada
+
+
 2.0.4 (2023-12-14)
 ------------------
 
 Bug fixes:
 
 
 - disable visibility of the right column in records template
```

### Comparing `plone.app.registry-2.0.4/PKG-INFO` & `plone_app_registry-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.registry
-Version: 2.0.4
+Version: 2.0.5
 Summary: Zope 2 and Plone  integration for plone.registry
 Home-page: https://pypi.org/project/plone.app.registry
 Author: Martin Aspeli
 Author-email: optilude@gmail.com
 License: GPL
 Keywords: plone registry settings configuration
 Classifier: Development Status :: 5 - Production/Stable
@@ -768,14 +768,25 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.5 (2024-05-30)
+------------------
+
+Bug fixes:
+
+
+- Removes duplicate `<article id="content">`
+  [@szakitibi] (#84)
+- Fix misleading portal message when NOT deleting records @gforcada
+
+
 2.0.4 (2023-12-14)
 ------------------
 
 Bug fixes:
 
 
 - disable visibility of the right column in records template
```

### Comparing `plone.app.registry-2.0.4/README.rst` & `plone_app_registry-2.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.4/docs/INSTALL.txt` & `plone_app_registry-2.0.5/docs/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.4/docs/LICENSE.GPL` & `plone_app_registry-2.0.5/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.4/docs/LICENSE.txt` & `plone_app_registry-2.0.5/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.4/docs/configuration_registry_add_record_screenshot.jpg` & `plone_app_registry-2.0.5/docs/configuration_registry_add_record_screenshot.jpg`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.4/docs/configuration_registry_edit_record_screenshot.jpg` & `plone_app_registry-2.0.5/docs/configuration_registry_edit_record_screenshot.jpg`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.4/docs/configuration_registry_export_screenshot.jpg` & `plone_app_registry-2.0.5/docs/configuration_registry_export_screenshot.jpg`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.4/docs/configuration_registry_import_screenshot.jpg` & `plone_app_registry-2.0.5/docs/configuration_registry_import_screenshot.jpg`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.4/docs/configuration_registry_screenshot.jpg` & `plone_app_registry-2.0.5/docs/configuration_registry_screenshot.jpg`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.4/plone/app/registry/README.txt` & `plone_app_registry-2.0.5/plone/app/registry/README.txt`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.4/plone/app/registry/browser/configure.zcml` & `plone_app_registry-2.0.5/plone/app/registry/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.4/plone/app/registry/browser/controlpanel.py` & `plone_app_registry-2.0.5/plone/app/registry/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.4/plone/app/registry/browser/delete.py` & `plone_app_registry-2.0.5/plone/app/registry/browser/delete.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,10 +11,10 @@
             if self.request.form.get("form.buttons.delete"):
                 if name in self.context:
                     del self.context.records[name]
                     messages = IStatusMessage(self.request)
                     messages.add("Successfully deleted field %s" % name, type="info")
             elif self.request.form.get("form.buttons.cancel") and name:
                 messages = IStatusMessage(self.request)
-                messages.add("Successfully deleted field %s" % name, type="info")
+                messages.add("Field %s was not deleted" % name, type="info")
             return self.request.response.redirect(self.context.absolute_url())
         return super().__call__()
```

### Comparing `plone.app.registry-2.0.4/plone/app/registry/browser/edit.py` & `plone_app_registry-2.0.5/plone/app/registry/browser/edit.py`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.4/plone/app/registry/browser/exportxml.py` & `plone_app_registry-2.0.5/plone/app/registry/browser/exportxml.py`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.4/plone/app/registry/browser/records.py` & `plone_app_registry-2.0.5/plone/app/registry/browser/records.py`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.4/plone/app/registry/browser/templates/controlpanel_layout.pt` & `plone_app_registry-2.0.5/plone/app/registry/browser/templates/controlpanel_layout.pt`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.4/plone/app/registry/browser/templates/delete_layout.pt` & `plone_app_registry-2.0.5/plone/app/registry/browser/templates/delete_layout.pt`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.4/plone/app/registry/browser/templates/edit_layout.pt` & `plone_app_registry-2.0.5/plone/app/registry/browser/templates/edit_layout.pt`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.4/plone/app/registry/browser/templates/exportxml.pt` & `plone_app_registry-2.0.5/plone/app/registry/browser/templates/exportxml.pt`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.4/plone/app/registry/browser/templates/records.pt` & `plone_app_registry-2.0.5/plone/app/registry/browser/templates/records.pt`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,18 @@
                    dummy python:request.set('disable_border', 1);
                    disable_column_one python:request.set('disable_plone.leftcolumn', 1);
                    disable_column_two python:request.set('disable_plone.rightcolumn', 1);
                  " />
   </metal:block>
 
   <body>
-    <article id="content"
-             metal:fill-slot="prefs_configlet_main"
-             tal:define="
-               records view/records;
-             "
+    <metal:main metal:fill-slot="prefs_configlet_main"
+                tal:define="
+                  records view/records;
+                "
     >
 
       <header>
         <h1 class="documentFirstHeading"
             i18n:translate="heading_registry"
         >Configuration Registry</h1>
 
@@ -247,10 +246,10 @@
             <h2 i18n:translate="registry_add_record_label">Add new record</h2>
             <p i18n:translate="registry_add_record_text"></p>
             <metal:block use-macro="context/@@ploneform-macros/titlelessform">
             </metal:block>
           </div>
         </div>
       </div>
-    </article>
+    </metal:main>
   </body>
 </html>
```

### Comparing `plone.app.registry-2.0.4/plone/app/registry/configure.zcml` & `plone_app_registry-2.0.5/plone/app/registry/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.4/plone/app/registry/exportimport/configure.zcml` & `plone_app_registry-2.0.5/plone/app/registry/exportimport/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.4/plone/app/registry/exportimport/fields.py` & `plone_app_registry-2.0.5/plone/app/registry/exportimport/fields.py`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.4/plone/app/registry/exportimport/handler.py` & `plone_app_registry-2.0.5/plone/app/registry/exportimport/handler.py`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.4/plone/app/registry/exportimport/handlers.zcml` & `plone_app_registry-2.0.5/plone/app/registry/exportimport/handlers.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.4/plone/app/registry/profiles/default/controlpanel.xml` & `plone_app_registry-2.0.5/plone/app/registry/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.4/plone/app/registry/testing.py` & `plone_app_registry-2.0.5/plone/app/registry/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.4/plone/app/registry/tests/test_controlpanel.py` & `plone_app_registry-2.0.5/plone/app/registry/tests/test_controlpanel.py`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.4/plone/app/registry/tests/test_exportimport.py` & `plone_app_registry-2.0.5/plone/app/registry/tests/test_exportimport.py`

 * *Files 0% similar despite different names*

```diff
@@ -1446,17 +1446,17 @@
 
         self.registry.records["test.export.simple"] = Record(
             field.TextLine(title="Simple record", default="N/A"),
             value="Sample value",
         )
 
         # Note: These are nominally read-only!
-        self.registry.records[
-            "test.export.simple"
-        ].field.interfaceName = "non.existent.ISchema"
+        self.registry.records["test.export.simple"].field.interfaceName = (
+            "non.existent.ISchema"
+        )
         self.registry.records["test.export.simple"].field.fieldName = "blah"
 
         alsoProvides(self.registry.records["test.export.simple"], IInterfaceAwareRecord)
 
         context = DummyExportContext(self.site)
         exportRegistry(context)
```

### Comparing `plone.app.registry-2.0.4/plone/app/registry/tests/test_setup.py` & `plone_app_registry-2.0.5/plone/app/registry/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.4/plone.app.registry.egg-info/PKG-INFO` & `plone_app_registry-2.0.5/plone.app.registry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.registry
-Version: 2.0.4
+Version: 2.0.5
 Summary: Zope 2 and Plone  integration for plone.registry
 Home-page: https://pypi.org/project/plone.app.registry
 Author: Martin Aspeli
 Author-email: optilude@gmail.com
 License: GPL
 Keywords: plone registry settings configuration
 Classifier: Development Status :: 5 - Production/Stable
@@ -768,14 +768,25 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.5 (2024-05-30)
+------------------
+
+Bug fixes:
+
+
+- Removes duplicate `<article id="content">`
+  [@szakitibi] (#84)
+- Fix misleading portal message when NOT deleting records @gforcada
+
+
 2.0.4 (2023-12-14)
 ------------------
 
 Bug fixes:
 
 
 - disable visibility of the right column in records template
```

### Comparing `plone.app.registry-2.0.4/plone.app.registry.egg-info/SOURCES.txt` & `plone_app_registry-2.0.5/plone.app.registry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.4/pyproject.toml` & `plone_app_registry-2.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.app.registry-2.0.4/setup.py` & `plone_app_registry-2.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "2.0.4"
+version = "2.0.5"
 
 long_description = (
     f"{Path('README.rst').read_text()}\n{Path('CHANGES.rst').read_text()}"
 )
 
 setup(
     name="plone.app.registry",
```

