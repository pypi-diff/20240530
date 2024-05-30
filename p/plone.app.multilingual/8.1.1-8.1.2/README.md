# Comparing `tmp/plone.app.multilingual-8.1.1.tar.gz` & `tmp/plone_app_multilingual-8.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.multilingual-8.1.1.tar", last modified: Tue Feb 27 16:10:54 2024, max compression
+gzip compressed data, was "plone_app_multilingual-8.1.2.tar", last modified: Thu May 30 18:21:46 2024, max compression
```

## Comparing `plone.app.multilingual-8.1.1.tar` & `plone_app_multilingual-8.1.2.tar`

### file list

```diff
@@ -1,176 +1,176 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:10:54.670945 plone.app.multilingual-8.1.1/
--rw-r--r--   0 maurits    (501) staff       (20)    28947 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      536 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/CREDITS.rst
--rw-r--r--   0 maurits    (501) staff       (20)      123 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    46232 2024-02-27 16:10:54.670765 plone.app.multilingual-8.1.1/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)    14047 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:10:54.611829 plone.app.multilingual-8.1.1/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/docs/LICENSE.gpl
--rw-r--r--   0 maurits    (501) staff       (20)      678 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)     5620 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/docs/Makefile
--rw-r--r--   0 maurits    (501) staff       (20)     8041 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/docs/conf.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:10:54.614081 plone.app.multilingual-8.1.1/docs/images/
--rwxr-xr-x   0 maurits    (501) staff       (20)   135534 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/docs/images/image00.png
--rwxr-xr-x   0 maurits    (501) staff       (20)   136010 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/docs/images/image01.png
--rwxr-xr-x   0 maurits    (501) staff       (20)   136026 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/docs/images/image02.png
--rwxr-xr-x   0 maurits    (501) staff       (20)    99720 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/docs/images/image03.png
--rwxr-xr-x   0 maurits    (501) staff       (20)    36518 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/docs/images/image04.png
--rw-r--r--   0 maurits    (501) staff       (20)     4301 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)     1048 2024-02-27 16:10:54.671459 plone.app.multilingual-8.1.1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1786 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:10:54.603719 plone.app.multilingual-8.1.1/src/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:10:54.614415 plone.app.multilingual-8.1.1/src/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:10:54.619110 plone.app.multilingual-8.1.1/src/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:10:54.626701 plone.app.multilingual-8.1.1/src/plone/app/multilingual/
--rw-r--r--   0 maurits    (501) staff       (20)      331 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1683 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/api.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:10:54.634439 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     7170 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/add.py
--rw-r--r--   0 maurits    (501) staff       (20)    11381 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    10300 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/controlpanel.py
--rw-r--r--   0 maurits    (501) staff       (20)     3821 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/edit.py
--rw-r--r--   0 maurits    (501) staff       (20)    10414 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/helper_views.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:10:54.634874 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/images/
--rw-r--r--   0 maurits    (501) staff       (20)     6926 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/images/gtranslate.png
--rw-r--r--   0 maurits    (501) staff       (20)     3610 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/interfaces.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:10:54.636317 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/javascript/
--rw-r--r--   0 maurits    (501) staff       (20)     9278 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/javascript/babel_helper.js
--rw-r--r--   0 maurits    (501) staff       (20)   162462 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/javascript/jit-yc.js
--rw-r--r--   0 maurits    (501) staff       (20)     9667 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/javascript/mmap_helper.js
--rw-r--r--   0 maurits    (501) staff       (20)    22919 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/menu.py
--rw-r--r--   0 maurits    (501) staff       (20)    14381 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/migrator.py
--rw-r--r--   0 maurits    (501) staff       (20)     3352 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/modify.py
--rw-r--r--   0 maurits    (501) staff       (20)     4024 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/selector.py
--rw-r--r--   0 maurits    (501) staff       (20)    10594 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:10:54.636670 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/stylesheet/
--rw-r--r--   0 maurits    (501) staff       (20)     2297 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/stylesheet/multilingual.css
--rw-r--r--   0 maurits    (501) staff       (20)     1554 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/switcher.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:10:54.643644 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/templates/
--rw-r--r--   0 maurits    (501) staff       (20)     1330 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/templates/add-form-is-translation.pt
--rw-r--r--   0 maurits    (501) staff       (20)      157 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/templates/alternate-languages.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3843 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/templates/cleanup.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1237 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/templates/cleanup_results.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1938 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/templates/controlpanel.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2877 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/templates/dexterity_edit.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1732 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/templates/disconnect_translation.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1563 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/templates/dx_babel_view.pt
--rw-r--r--   0 maurits    (501) staff       (20)      767 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/templates/languages-notice.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1347 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/templates/languageselector.pt
--rw-r--r--   0 maurits    (501) staff       (20)    11015 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/templates/migration.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1208 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/templates/migrator-results.pt
--rw-r--r--   0 maurits    (501) staff       (20)     5387 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/templates/mmap.pt
--rw-r--r--   0 maurits    (501) staff       (20)     6894 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/templates/modify_translations.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3307 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/templates/not_translated_yet.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1152 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/templates/reindex-results.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1218 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/templates/relocate-results.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3295 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/translate.py
--rw-r--r--   0 maurits    (501) staff       (20)     1084 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/update.py
--rw-r--r--   0 maurits    (501) staff       (20)     6724 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)      470 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/view.py
--rw-r--r--   0 maurits    (501) staff       (20)     5012 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/viewlets.py
--rw-r--r--   0 maurits    (501) staff       (20)     5962 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/vocabularies.py
--rw-r--r--   0 maurits    (501) staff       (20)     6674 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:10:54.645818 plone.app.multilingual-8.1.1/src/plone/app/multilingual/content/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/content/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      602 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/content/lif.py
--rw-r--r--   0 maurits    (501) staff       (20)      131 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/content/lif.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1273 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/content/lrf.py
--rw-r--r--   0 maurits    (501) staff       (20)      131 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/content/lrf.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:10:54.651105 plone.app.multilingual-8.1.1/src/plone/app/multilingual/dx/
--rw-r--r--   0 maurits    (501) staff       (20)       48 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/dx/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     4430 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/dx/cloner.py
--rw-r--r--   0 maurits    (501) staff       (20)     2725 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/dx/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1640 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/dx/directives.py
--rw-r--r--   0 maurits    (501) staff       (20)     3157 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/dx/form.py
--rw-r--r--   0 maurits    (501) staff       (20)      770 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/dx/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      652 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/dx/language.py
--rw-r--r--   0 maurits    (501) staff       (20)      456 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/dx/languageindependent.py
--rw-r--r--   0 maurits    (501) staff       (20)      139 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/dx/meta.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2521 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/dx/schemaeditor.py
--rw-r--r--   0 maurits    (501) staff       (20)     4955 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/dx/subscriber.py
--rw-r--r--   0 maurits    (501) staff       (20)     1100 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/dx/supermodel.py
--rw-r--r--   0 maurits    (501) staff       (20)     2994 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/events.py
--rw-r--r--   0 maurits    (501) staff       (20)     3338 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/factory.py
--rw-r--r--   0 maurits    (501) staff       (20)      366 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/indexer.py
--rw-r--r--   0 maurits    (501) staff       (20)     8436 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     1571 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/itg.py
--rw-r--r--   0 maurits    (501) staff       (20)     8506 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/manager.py
--rw-r--r--   0 maurits    (501) staff       (20)      151 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/overrides.zcml
--rw-r--r--   0 maurits    (501) staff       (20)       67 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/permissions.py
--rw-r--r--   0 maurits    (501) staff       (20)      234 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/permissions.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:10:54.606368 plone.app.multilingual-8.1.1/src/plone/app/multilingual/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:10:54.655273 plone.app.multilingual-8.1.1/src/plone/app/multilingual/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      188 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/profiles/default/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)      427 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/profiles/default/catalog.xml
--rw-r--r--   0 maurits    (501) staff       (20)      188 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)       51 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/profiles/default/plone.app.multilingual_default.txt
--rw-r--r--   0 maurits    (501) staff       (20)      113 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/profiles/default/reference_catalog.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1344 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/profiles/default/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)      343 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/profiles/default/rolemap.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:10:54.655909 plone.app.multilingual-8.1.1/src/plone/app/multilingual/profiles/default/types/
--rw-r--r--   0 maurits    (501) staff       (20)     2680 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/profiles/default/types/LIF.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2711 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/profiles/default/types/LRF.xml
--rw-r--r--   0 maurits    (501) staff       (20)      240 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/profiles/default/types.xml
--rw-r--r--   0 maurits    (501) staff       (20)      412 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/profiles/default/viewlets.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:10:54.659239 plone.app.multilingual-8.1.1/src/plone/app/multilingual/profiles/uninstall/
--rw-r--r--   0 maurits    (501) staff       (20)      211 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)      418 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/profiles/uninstall/catalog.xml
--rw-r--r--   0 maurits    (501) staff       (20)      191 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/profiles/uninstall/cssregistry.xml
--rw-r--r--   0 maurits    (501) staff       (20)       85 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/profiles/uninstall/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)       51 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/profiles/uninstall/plone.app.multilingual_uninstall.txt
--rw-r--r--   0 maurits    (501) staff       (20)      139 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/profiles/uninstall/reference_catalog.xml
--rw-r--r--   0 maurits    (501) staff       (20)      202 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/profiles/uninstall/types.xml
--rw-r--r--   0 maurits    (501) staff       (20)      362 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/profiles/uninstall/viewlets.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:10:54.606933 plone.app.multilingual-8.1.1/src/plone/app/multilingual/profiles/upgrades/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:10:54.606595 plone.app.multilingual-8.1.1/src/plone/app/multilingual/profiles/upgrades/to_1000/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:10:54.660057 plone.app.multilingual-8.1.1/src/plone/app/multilingual/profiles/upgrades/to_1000/types/
--rw-r--r--   0 maurits    (501) staff       (20)     1032 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/profiles/upgrades/to_1000/types/LIF.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1025 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/profiles/upgrades/to_1000/types/LRF.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:10:54.660360 plone.app.multilingual-8.1.1/src/plone/app/multilingual/profiles/upgrades/to_3/
--rw-r--r--   0 maurits    (501) staff       (20)      276 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/profiles/upgrades/to_3/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:10:54.660759 plone.app.multilingual-8.1.1/src/plone/app/multilingual/profiles/upgrades/to_4/
--rw-r--r--   0 maurits    (501) staff       (20)      975 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/profiles/upgrades/to_4/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2988 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/setuphandlers.py
--rw-r--r--   0 maurits    (501) staff       (20)     1214 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/shared_uuid.py
--rw-r--r--   0 maurits    (501) staff       (20)     6530 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/subscriber.py
--rw-r--r--   0 maurits    (501) staff       (20)     9607 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/testing.py
--rw-r--r--   0 maurits    (501) staff       (20)      183 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/testing.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:10:54.667463 plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:10:54.668644 plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/robot/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/robot/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3534 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/robot/test_add_translation.robot
--rw-r--r--   0 maurits    (501) staff       (20)     3418 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/robot/test_schemaeditor.robot
--rw-r--r--   0 maurits    (501) staff       (20)     2205 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/robot/test_translate_content.robot
--rw-r--r--   0 maurits    (501) staff       (20)     1434 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/test_alternates.py
--rw-r--r--   0 maurits    (501) staff       (20)    11045 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/test_api.py
--rw-r--r--   0 maurits    (501) staff       (20)     2147 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/test_catalog.py
--rw-r--r--   0 maurits    (501) staff       (20)     1878 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/test_directives.py
--rw-r--r--   0 maurits    (501) staff       (20)     8756 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/test_form.py
--rw-r--r--   0 maurits    (501) staff       (20)     5819 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/test_helper_views.py
--rw-r--r--   0 maurits    (501) staff       (20)     9471 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/test_lif.py
--rw-r--r--   0 maurits    (501) staff       (20)     5354 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/test_lrf.py
--rw-r--r--   0 maurits    (501) staff       (20)     3299 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/test_menu.py
--rw-r--r--   0 maurits    (501) staff       (20)      532 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/test_robot.py
--rw-r--r--   0 maurits    (501) staff       (20)    39142 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/test_selector.py
--rw-r--r--   0 maurits    (501) staff       (20)     4727 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/test_setup.py
--rw-r--r--   0 maurits    (501) staff       (20)     3326 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/test_sitemap.py
--rw-r--r--   0 maurits    (501) staff       (20)     8330 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/test_subscribers.py
--rw-r--r--   0 maurits    (501) staff       (20)     2742 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/test_switcher.py
--rw-r--r--   0 maurits    (501) staff       (20)     1601 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/test_uninstall.py
--rw-r--r--   0 maurits    (501) staff       (20)     1288 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/test_vocabularies.py
--rw-r--r--   0 maurits    (501) staff       (20)     8055 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/upgrades.py
--rw-r--r--   0 maurits    (501) staff       (20)     2687 2024-02-27 16:10:53.000000 plone.app.multilingual-8.1.1/src/plone/app/multilingual/upgrades.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 16:10:54.669090 plone.app.multilingual-8.1.1/src/plone.app.multilingual.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    46232 2024-02-27 16:10:54.000000 plone.app.multilingual-8.1.1/src/plone.app.multilingual.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     7054 2024-02-27 16:10:54.000000 plone.app.multilingual-8.1.1/src/plone.app.multilingual.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-02-27 16:10:54.000000 plone.app.multilingual-8.1.1/src/plone.app.multilingual.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2024-02-27 16:10:54.000000 plone.app.multilingual-8.1.1/src/plone.app.multilingual.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2024-02-27 16:10:54.000000 plone.app.multilingual-8.1.1/src/plone.app.multilingual.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-02-27 16:10:54.000000 plone.app.multilingual-8.1.1/src/plone.app.multilingual.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      751 2024-02-27 16:10:54.000000 plone.app.multilingual-8.1.1/src/plone.app.multilingual.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2024-02-27 16:10:54.000000 plone.app.multilingual-8.1.1/src/plone.app.multilingual.egg-info/top_level.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:21:46.739871 plone_app_multilingual-8.1.2/
+-rw-r--r--   0 maurits    (501) staff       (20)    29145 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      536 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/CREDITS.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      123 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    46449 2024-05-30 18:21:46.739575 plone_app_multilingual-8.1.2/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)    14047 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:21:46.669233 plone_app_multilingual-8.1.2/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/docs/LICENSE.gpl
+-rw-r--r--   0 maurits    (501) staff       (20)      678 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/docs/LICENSE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     5620 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/docs/Makefile
+-rw-r--r--   0 maurits    (501) staff       (20)     8041 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/docs/conf.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:21:46.672656 plone_app_multilingual-8.1.2/docs/images/
+-rwxr-xr-x   0 maurits    (501) staff       (20)   135534 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/docs/images/image00.png
+-rwxr-xr-x   0 maurits    (501) staff       (20)   136010 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/docs/images/image01.png
+-rwxr-xr-x   0 maurits    (501) staff       (20)   136026 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/docs/images/image02.png
+-rwxr-xr-x   0 maurits    (501) staff       (20)    99720 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/docs/images/image03.png
+-rwxr-xr-x   0 maurits    (501) staff       (20)    36518 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/docs/images/image04.png
+-rw-r--r--   0 maurits    (501) staff       (20)     4430 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)     1048 2024-05-30 18:21:46.740645 plone_app_multilingual-8.1.2/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1801 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:21:46.658190 plone_app_multilingual-8.1.2/src/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:21:46.673241 plone_app_multilingual-8.1.2/src/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:21:46.677662 plone_app_multilingual-8.1.2/src/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:21:46.686704 plone_app_multilingual-8.1.2/src/plone/app/multilingual/
+-rw-r--r--   0 maurits    (501) staff       (20)      331 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1683 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/api.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:21:46.695881 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7170 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/add.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11381 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    10300 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/controlpanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3821 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/edit.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10414 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/helper_views.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:21:46.696383 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/images/
+-rw-r--r--   0 maurits    (501) staff       (20)     6926 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/images/gtranslate.png
+-rw-r--r--   0 maurits    (501) staff       (20)     3610 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/interfaces.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:21:46.698137 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/javascript/
+-rw-r--r--   0 maurits    (501) staff       (20)     9278 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/javascript/babel_helper.js
+-rw-r--r--   0 maurits    (501) staff       (20)   162462 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/javascript/jit-yc.js
+-rw-r--r--   0 maurits    (501) staff       (20)     9667 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/javascript/mmap_helper.js
+-rw-r--r--   0 maurits    (501) staff       (20)    22919 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/menu.py
+-rw-r--r--   0 maurits    (501) staff       (20)    14381 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/migrator.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3352 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/modify.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4024 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/selector.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10594 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:21:46.698621 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/stylesheet/
+-rw-r--r--   0 maurits    (501) staff       (20)     2297 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/stylesheet/multilingual.css
+-rw-r--r--   0 maurits    (501) staff       (20)     1554 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/switcher.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:21:46.706741 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/templates/
+-rw-r--r--   0 maurits    (501) staff       (20)     1330 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/templates/add-form-is-translation.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      157 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/templates/alternate-languages.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3843 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/templates/cleanup.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1237 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/templates/cleanup_results.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1938 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/templates/controlpanel.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2877 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/templates/dexterity_edit.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1732 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/templates/disconnect_translation.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1563 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/templates/dx_babel_view.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      767 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/templates/languages-notice.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1347 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/templates/languageselector.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    11015 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/templates/migration.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1208 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/templates/migrator-results.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     5387 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/templates/mmap.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     6894 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/templates/modify_translations.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3307 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/templates/not_translated_yet.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1152 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/templates/reindex-results.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1218 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/templates/relocate-results.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3295 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/translate.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1084 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/update.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6724 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)      470 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/view.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5012 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/viewlets.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5966 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/vocabularies.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6674 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:21:46.708980 plone_app_multilingual-8.1.2/src/plone/app/multilingual/content/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/content/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      602 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/content/lif.py
+-rw-r--r--   0 maurits    (501) staff       (20)      131 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/content/lif.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1273 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/content/lrf.py
+-rw-r--r--   0 maurits    (501) staff       (20)      131 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/content/lrf.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:21:46.714698 plone_app_multilingual-8.1.2/src/plone/app/multilingual/dx/
+-rw-r--r--   0 maurits    (501) staff       (20)       48 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/dx/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4430 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/dx/cloner.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2725 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/dx/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1640 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/dx/directives.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3157 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/dx/form.py
+-rw-r--r--   0 maurits    (501) staff       (20)      770 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/dx/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      652 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/dx/language.py
+-rw-r--r--   0 maurits    (501) staff       (20)      456 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/dx/languageindependent.py
+-rw-r--r--   0 maurits    (501) staff       (20)      139 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/dx/meta.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2521 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/dx/schemaeditor.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4955 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/dx/subscriber.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1100 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/dx/supermodel.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2994 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/events.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3338 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/factory.py
+-rw-r--r--   0 maurits    (501) staff       (20)      366 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/indexer.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8436 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1571 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/itg.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8506 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/manager.py
+-rw-r--r--   0 maurits    (501) staff       (20)      151 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/overrides.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)       67 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/permissions.py
+-rw-r--r--   0 maurits    (501) staff       (20)      234 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/permissions.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:21:46.661828 plone_app_multilingual-8.1.2/src/plone/app/multilingual/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:21:46.719024 plone_app_multilingual-8.1.2/src/plone/app/multilingual/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      188 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/profiles/default/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      427 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/profiles/default/catalog.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      188 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)       51 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/profiles/default/plone.app.multilingual_default.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      113 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/profiles/default/reference_catalog.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1344 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/profiles/default/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      343 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/profiles/default/rolemap.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:21:46.720000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/profiles/default/types/
+-rw-r--r--   0 maurits    (501) staff       (20)     2680 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/profiles/default/types/LIF.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2711 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/profiles/default/types/LRF.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      240 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/profiles/default/types.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      412 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/profiles/default/viewlets.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:21:46.723773 plone_app_multilingual-8.1.2/src/plone/app/multilingual/profiles/uninstall/
+-rw-r--r--   0 maurits    (501) staff       (20)      211 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      418 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/profiles/uninstall/catalog.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      191 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/profiles/uninstall/cssregistry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)       85 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/profiles/uninstall/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)       51 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/profiles/uninstall/plone.app.multilingual_uninstall.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      139 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/profiles/uninstall/reference_catalog.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      202 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/profiles/uninstall/types.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      362 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/profiles/uninstall/viewlets.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:21:46.662763 plone_app_multilingual-8.1.2/src/plone/app/multilingual/profiles/upgrades/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:21:46.662230 plone_app_multilingual-8.1.2/src/plone/app/multilingual/profiles/upgrades/to_1000/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:21:46.724763 plone_app_multilingual-8.1.2/src/plone/app/multilingual/profiles/upgrades/to_1000/types/
+-rw-r--r--   0 maurits    (501) staff       (20)     1032 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/profiles/upgrades/to_1000/types/LIF.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1025 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/profiles/upgrades/to_1000/types/LRF.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:21:46.725247 plone_app_multilingual-8.1.2/src/plone/app/multilingual/profiles/upgrades/to_3/
+-rw-r--r--   0 maurits    (501) staff       (20)      276 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/profiles/upgrades/to_3/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:21:46.725738 plone_app_multilingual-8.1.2/src/plone/app/multilingual/profiles/upgrades/to_4/
+-rw-r--r--   0 maurits    (501) staff       (20)      975 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/profiles/upgrades/to_4/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2988 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/setuphandlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1214 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/shared_uuid.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6530 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/subscriber.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9607 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/testing.py
+-rw-r--r--   0 maurits    (501) staff       (20)      183 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/testing.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:21:46.734460 plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:21:46.736284 plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/robot/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/robot/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3534 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/robot/test_add_translation.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     3418 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/robot/test_schemaeditor.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     2205 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/robot/test_translate_content.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     1434 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/test_alternates.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11045 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/test_api.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2147 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/test_catalog.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1878 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/test_directives.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8756 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/test_form.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5819 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/test_helper_views.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9471 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/test_lif.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5354 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/test_lrf.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3299 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/test_menu.py
+-rw-r--r--   0 maurits    (501) staff       (20)      532 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/test_robot.py
+-rw-r--r--   0 maurits    (501) staff       (20)    39142 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/test_selector.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4727 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/test_setup.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3326 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/test_sitemap.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8330 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/test_subscribers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2742 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/test_switcher.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1601 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/test_uninstall.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1288 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/test_vocabularies.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8055 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/upgrades.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2687 2024-05-30 18:21:45.000000 plone_app_multilingual-8.1.2/src/plone/app/multilingual/upgrades.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:21:46.736963 plone_app_multilingual-8.1.2/src/plone.app.multilingual.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    46449 2024-05-30 18:21:46.000000 plone_app_multilingual-8.1.2/src/plone.app.multilingual.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     7054 2024-05-30 18:21:46.000000 plone_app_multilingual-8.1.2/src/plone.app.multilingual.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-05-30 18:21:46.000000 plone_app_multilingual-8.1.2/src/plone.app.multilingual.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2024-05-30 18:21:46.000000 plone_app_multilingual-8.1.2/src/plone.app.multilingual.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2024-05-30 18:21:46.000000 plone_app_multilingual-8.1.2/src/plone.app.multilingual.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-05-30 18:21:46.000000 plone_app_multilingual-8.1.2/src/plone.app.multilingual.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      755 2024-05-30 18:21:46.000000 plone_app_multilingual-8.1.2/src/plone.app.multilingual.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-05-30 18:21:46.000000 plone_app_multilingual-8.1.2/src/plone.app.multilingual.egg-info/top_level.txt
```

### Comparing `plone.app.multilingual-8.1.1/CHANGES.rst` & `plone_app_multilingual-8.1.2/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,30 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+8.1.2 (2024-05-30)
+------------------
+
+Bug fixes:
+
+
+- Removed DeprecationWarning from CatalogVocabularyFactory import. [@jensens] (#454)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs]
+
+
 8.1.1 (2024-02-27)
 ------------------
 
 Bug fixes:
 
 
 - Add missing translate icon for the menu. [szakitibi] (#447)
```

### Comparing `plone.app.multilingual-8.1.1/CREDITS.rst` & `plone_app_multilingual-8.1.2/CREDITS.rst`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/PKG-INFO` & `plone_app_multilingual-8.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.multilingual
-Version: 8.1.1
+Version: 8.1.2
 Summary: Multilingual Plone Content package
 Home-page: https://github.com/plone/plone.app.multilingual
 Author: Ramon Navarro, Victor Fernandez de Alba, awello et al
 Author-email: r.navarro@iskra.cat
 Maintainer: Plone Foundation
 Maintainer-email: releasemanager@plone.org
 License: GPL
@@ -20,50 +20,51 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
-Requires-Dist: plone.i18n>=4.0.4
-Requires-Dist: setuptools
 Requires-Dist: BTrees
-Requires-Dist: Products.CMFCore
-Requires-Dist: Products.CMFPlone
-Requires-Dist: Products.GenericSetup
-Requires-Dist: Products.statusmessages
 Requires-Dist: plone.app.content
 Requires-Dist: plone.app.contentmenu
 Requires-Dist: plone.app.dexterity
 Requires-Dist: plone.app.event
 Requires-Dist: plone.app.i18n
 Requires-Dist: plone.app.layout
+Requires-Dist: plone.app.querystring
 Requires-Dist: plone.app.registry
 Requires-Dist: plone.app.uuid
-Requires-Dist: plone.app.vocabularies
 Requires-Dist: plone.app.z3cform
 Requires-Dist: plone.autoform
 Requires-Dist: plone.base
 Requires-Dist: plone.behavior
 Requires-Dist: plone.dexterity
+Requires-Dist: plone.i18n>=4.0.4
 Requires-Dist: plone.indexer
 Requires-Dist: plone.locking
 Requires-Dist: plone.memoize
 Requires-Dist: plone.protect
 Requires-Dist: plone.registry
 Requires-Dist: plone.schemaeditor
 Requires-Dist: plone.supermodel
 Requires-Dist: plone.uuid
 Requires-Dist: plone.z3cform
+Requires-Dist: Products.CMFCore
+Requires-Dist: Products.CMFPlone
+Requires-Dist: Products.GenericSetup
+Requires-Dist: Products.statusmessages
+Requires-Dist: setuptools
 Requires-Dist: z3c.form
 Requires-Dist: z3c.relationfield
 Requires-Dist: zc.relation
 Requires-Dist: zope.browsermenu
 Requires-Dist: zope.intid
 Requires-Dist: zope.pagetemplate
+Requires-Dist: Zope
 Provides-Extra: test
 Requires-Dist: plone.app.testing[robot]; extra == "test"
 Requires-Dist: plone.app.robotframework; extra == "test"
 Requires-Dist: lxml; extra == "test"
 Requires-Dist: plone.api; extra == "test"
 Requires-Dist: plone.app.contenttypes; extra == "test"
 Requires-Dist: plone.app.relationfield; extra == "test"
@@ -427,14 +428,30 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+8.1.2 (2024-05-30)
+------------------
+
+Bug fixes:
+
+
+- Removed DeprecationWarning from CatalogVocabularyFactory import. [@jensens] (#454)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs]
+
+
 8.1.1 (2024-02-27)
 ------------------
 
 Bug fixes:
 
 
 - Add missing translate icon for the menu. [szakitibi] (#447)
```

### Comparing `plone.app.multilingual-8.1.1/README.rst` & `plone_app_multilingual-8.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/docs/LICENSE.gpl` & `plone_app_multilingual-8.1.2/docs/LICENSE.gpl`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/docs/LICENSE.txt` & `plone_app_multilingual-8.1.2/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/docs/Makefile` & `plone_app_multilingual-8.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/docs/conf.py` & `plone_app_multilingual-8.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/docs/images/image00.png` & `plone_app_multilingual-8.1.2/docs/images/image00.png`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/docs/images/image01.png` & `plone_app_multilingual-8.1.2/docs/images/image01.png`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/docs/images/image02.png` & `plone_app_multilingual-8.1.2/docs/images/image02.png`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/docs/images/image03.png` & `plone_app_multilingual-8.1.2/docs/images/image03.png`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/docs/images/image04.png` & `plone_app_multilingual-8.1.2/docs/images/image04.png`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/pyproject.toml` & `plone_app_multilingual-8.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -130,29 +130,36 @@
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
     "requirements.txt",
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

### Comparing `plone.app.multilingual-8.1.1/setup.cfg` & `plone_app_multilingual-8.1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 8.1.1
+version = 8.1.2
 name = plone.app.multilingual
 description = Multilingual Plone Content package
 long_description = file: README.rst, CREDITS.rst, CHANGES.rst
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Environment :: Web Environment
 	Framework :: Plone
```

### Comparing `plone.app.multilingual-8.1.1/setup.py` & `plone_app_multilingual-8.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,50 +8,51 @@
     # metadata in setup.cfg
     packages=find_packages("src"),
     package_dir={"": "src"},
     namespace_packages=["plone", "plone.app"],
     include_package_data=True,
     zip_safe=False,
     install_requires=[
-        "plone.i18n>=4.0.4",
-        "setuptools",
         "BTrees",
-        "Products.CMFCore",
-        "Products.CMFPlone",
-        "Products.GenericSetup",
-        "Products.statusmessages",
         "plone.app.content",
         "plone.app.contentmenu",
         "plone.app.dexterity",
         "plone.app.event",
         "plone.app.i18n",
         "plone.app.layout",
+        "plone.app.querystring",
         "plone.app.registry",
         "plone.app.uuid",
-        "plone.app.vocabularies",
         "plone.app.z3cform",
         "plone.autoform",
         "plone.base",
         "plone.behavior",
         "plone.dexterity",
+        "plone.i18n>=4.0.4",
         "plone.indexer",
         "plone.locking",
         "plone.memoize",
         "plone.protect",
         "plone.registry",
         "plone.schemaeditor",
         "plone.supermodel",
         "plone.uuid",
         "plone.z3cform",
+        "Products.CMFCore",
+        "Products.CMFPlone",
+        "Products.GenericSetup",
+        "Products.statusmessages",
+        "setuptools",
         "z3c.form",
         "z3c.relationfield",
         "zc.relation",
         "zope.browsermenu",
         "zope.intid",
         "zope.pagetemplate",
+        "Zope",
     ],
     extras_require={
         "test": [
             "plone.app.testing[robot]",
             "plone.app.robotframework",
             "lxml",
             "plone.api",
```

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/api.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/api.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/add.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/add.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/configure.zcml` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/controlpanel.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/edit.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/edit.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/helper_views.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/helper_views.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/images/gtranslate.png` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/images/gtranslate.png`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/interfaces.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/javascript/babel_helper.js` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/javascript/babel_helper.js`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/javascript/jit-yc.js` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/javascript/jit-yc.js`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/javascript/mmap_helper.js` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/javascript/mmap_helper.js`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/menu.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/menu.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/migrator.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/migrator.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/modify.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/modify.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/selector.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/selector.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/setup.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/setup.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/stylesheet/multilingual.css` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/stylesheet/multilingual.css`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/switcher.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/switcher.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/templates/add-form-is-translation.pt` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/templates/add-form-is-translation.pt`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/templates/cleanup.pt` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/templates/cleanup.pt`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/templates/cleanup_results.pt` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/templates/cleanup_results.pt`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/templates/controlpanel.pt` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/templates/controlpanel.pt`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/templates/dexterity_edit.pt` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/templates/dexterity_edit.pt`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/templates/disconnect_translation.pt` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/templates/disconnect_translation.pt`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/templates/dx_babel_view.pt` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/templates/dx_babel_view.pt`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/templates/languages-notice.pt` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/templates/languages-notice.pt`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/templates/languageselector.pt` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/templates/languageselector.pt`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/templates/migration.pt` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/templates/migration.pt`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/templates/migrator-results.pt` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/templates/migrator-results.pt`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/templates/mmap.pt` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/templates/mmap.pt`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/templates/modify_translations.pt` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/templates/modify_translations.pt`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/templates/not_translated_yet.pt` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/templates/not_translated_yet.pt`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/templates/reindex-results.pt` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/templates/reindex-results.pt`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/templates/relocate-results.pt` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/templates/relocate-results.pt`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/translate.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/translate.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/update.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/update.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/utils.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/viewlets.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/viewlets.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/browser/vocabularies.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/browser/vocabularies.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from plone.app.multilingual.browser.utils import is_language_independent
 from plone.app.multilingual.interfaces import ITranslationManager
-from plone.app.vocabularies.catalog import CatalogVocabularyFactory
+from plone.app.querystring.vocabularies import CatalogVocabularyFactory
 from plone.base.interfaces import ILanguage
 from plone.i18n.locales.interfaces import ILanguageAvailability
 from Products.CMFCore.utils import getToolByName
 from zope.component import getGlobalSiteManager
 from zope.interface import implementer
 from zope.interface import provider
 from zope.schema.interfaces import IContextSourceBinder
```

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/configure.zcml` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/content/lif.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/content/lif.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/content/lrf.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/content/lrf.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/dx/cloner.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/dx/cloner.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/dx/configure.zcml` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/dx/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/dx/directives.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/dx/directives.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/dx/form.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/dx/form.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/dx/interfaces.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/dx/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/dx/language.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/dx/language.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/dx/schemaeditor.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/dx/schemaeditor.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/dx/subscriber.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/dx/subscriber.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/dx/supermodel.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/dx/supermodel.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/events.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/events.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/factory.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/factory.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/interfaces.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/itg.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/itg.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/manager.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/manager.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/profiles/default/registry.xml` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/profiles/default/types/LIF.xml` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/profiles/default/types/LIF.xml`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/profiles/default/types/LRF.xml` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/profiles/default/types/LRF.xml`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/profiles/upgrades/to_1000/types/LIF.xml` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/profiles/upgrades/to_1000/types/LIF.xml`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/profiles/upgrades/to_1000/types/LRF.xml` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/profiles/upgrades/to_1000/types/LRF.xml`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/profiles/upgrades/to_4/registry.xml` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/profiles/upgrades/to_4/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/setuphandlers.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/shared_uuid.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/shared_uuid.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/subscriber.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/subscriber.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/testing.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/robot/test_add_translation.robot` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/robot/test_add_translation.robot`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/robot/test_schemaeditor.robot` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/robot/test_schemaeditor.robot`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/robot/test_translate_content.robot` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/robot/test_translate_content.robot`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/test_alternates.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/test_alternates.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/test_api.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/test_catalog.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/test_directives.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/test_directives.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/test_form.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/test_helper_views.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/test_helper_views.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/test_lif.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/test_lif.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/test_lrf.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/test_lrf.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/test_menu.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/test_menu.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/test_robot.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/test_selector.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/test_selector.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/test_setup.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/test_sitemap.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/test_sitemap.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/test_subscribers.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/test_subscribers.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/test_switcher.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/test_switcher.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/test_uninstall.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/test_uninstall.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/tests/test_vocabularies.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/tests/test_vocabularies.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/upgrades.py` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/upgrades.py`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone/app/multilingual/upgrades.zcml` & `plone_app_multilingual-8.1.2/src/plone/app/multilingual/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone.app.multilingual.egg-info/PKG-INFO` & `plone_app_multilingual-8.1.2/src/plone.app.multilingual.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.multilingual
-Version: 8.1.1
+Version: 8.1.2
 Summary: Multilingual Plone Content package
 Home-page: https://github.com/plone/plone.app.multilingual
 Author: Ramon Navarro, Victor Fernandez de Alba, awello et al
 Author-email: r.navarro@iskra.cat
 Maintainer: Plone Foundation
 Maintainer-email: releasemanager@plone.org
 License: GPL
@@ -20,50 +20,51 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
-Requires-Dist: plone.i18n>=4.0.4
-Requires-Dist: setuptools
 Requires-Dist: BTrees
-Requires-Dist: Products.CMFCore
-Requires-Dist: Products.CMFPlone
-Requires-Dist: Products.GenericSetup
-Requires-Dist: Products.statusmessages
 Requires-Dist: plone.app.content
 Requires-Dist: plone.app.contentmenu
 Requires-Dist: plone.app.dexterity
 Requires-Dist: plone.app.event
 Requires-Dist: plone.app.i18n
 Requires-Dist: plone.app.layout
+Requires-Dist: plone.app.querystring
 Requires-Dist: plone.app.registry
 Requires-Dist: plone.app.uuid
-Requires-Dist: plone.app.vocabularies
 Requires-Dist: plone.app.z3cform
 Requires-Dist: plone.autoform
 Requires-Dist: plone.base
 Requires-Dist: plone.behavior
 Requires-Dist: plone.dexterity
+Requires-Dist: plone.i18n>=4.0.4
 Requires-Dist: plone.indexer
 Requires-Dist: plone.locking
 Requires-Dist: plone.memoize
 Requires-Dist: plone.protect
 Requires-Dist: plone.registry
 Requires-Dist: plone.schemaeditor
 Requires-Dist: plone.supermodel
 Requires-Dist: plone.uuid
 Requires-Dist: plone.z3cform
+Requires-Dist: Products.CMFCore
+Requires-Dist: Products.CMFPlone
+Requires-Dist: Products.GenericSetup
+Requires-Dist: Products.statusmessages
+Requires-Dist: setuptools
 Requires-Dist: z3c.form
 Requires-Dist: z3c.relationfield
 Requires-Dist: zc.relation
 Requires-Dist: zope.browsermenu
 Requires-Dist: zope.intid
 Requires-Dist: zope.pagetemplate
+Requires-Dist: Zope
 Provides-Extra: test
 Requires-Dist: plone.app.testing[robot]; extra == "test"
 Requires-Dist: plone.app.robotframework; extra == "test"
 Requires-Dist: lxml; extra == "test"
 Requires-Dist: plone.api; extra == "test"
 Requires-Dist: plone.app.contenttypes; extra == "test"
 Requires-Dist: plone.app.relationfield; extra == "test"
@@ -427,14 +428,30 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+8.1.2 (2024-05-30)
+------------------
+
+Bug fixes:
+
+
+- Removed DeprecationWarning from CatalogVocabularyFactory import. [@jensens] (#454)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs]
+
+
 8.1.1 (2024-02-27)
 ------------------
 
 Bug fixes:
 
 
 - Add missing translate icon for the menu. [szakitibi] (#447)
```

### Comparing `plone.app.multilingual-8.1.1/src/plone.app.multilingual.egg-info/SOURCES.txt` & `plone_app_multilingual-8.1.2/src/plone.app.multilingual.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.multilingual-8.1.1/src/plone.app.multilingual.egg-info/requires.txt` & `plone_app_multilingual-8.1.2/src/plone.app.multilingual.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,44 @@
-plone.i18n>=4.0.4
-setuptools
 BTrees
-Products.CMFCore
-Products.CMFPlone
-Products.GenericSetup
-Products.statusmessages
 plone.app.content
 plone.app.contentmenu
 plone.app.dexterity
 plone.app.event
 plone.app.i18n
 plone.app.layout
+plone.app.querystring
 plone.app.registry
 plone.app.uuid
-plone.app.vocabularies
 plone.app.z3cform
 plone.autoform
 plone.base
 plone.behavior
 plone.dexterity
+plone.i18n>=4.0.4
 plone.indexer
 plone.locking
 plone.memoize
 plone.protect
 plone.registry
 plone.schemaeditor
 plone.supermodel
 plone.uuid
 plone.z3cform
+Products.CMFCore
+Products.CMFPlone
+Products.GenericSetup
+Products.statusmessages
+setuptools
 z3c.form
 z3c.relationfield
 zc.relation
 zope.browsermenu
 zope.intid
 zope.pagetemplate
+Zope
 
 [test]
 plone.app.testing[robot]
 plone.app.robotframework
 lxml
 plone.api
 plone.app.contenttypes
```

