# Comparing `tmp/kitconcept.seo-2.0.1.dev0.tar.gz` & `tmp/kitconcept_seo-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kitconcept.seo-2.0.1.dev0.tar", last modified: Mon Nov  1 08:37:28 2021, max compression
+gzip compressed data, was "kitconcept_seo-2.1.0.tar", last modified: Thu May 30 18:13:28 2024, max compression
```

## Comparing `kitconcept.seo-2.0.1.dev0.tar` & `kitconcept_seo-2.1.0.tar`

### file list

```diff
@@ -1,61 +1,69 @@
-drwxrwxr-x   0 ericof    (1000) ericof    (1000)        0 2021-11-01 08:37:28.590889 kitconcept.seo-2.0.1.dev0/
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     1131 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/CHANGES.rst
--rw-rw-r--   0 ericof    (1000) ericof    (1000)       66 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/CONTRIBUTORS.rst
--rw-rw-r--   0 ericof    (1000) ericof    (1000)      123 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/MANIFEST.in
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     9608 2021-11-01 08:37:28.590889 kitconcept.seo-2.0.1.dev0/PKG-INFO
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     5499 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/README.rst
-drwxrwxr-x   0 ericof    (1000) ericof    (1000)        0 2021-11-01 08:37:28.586889 kitconcept.seo-2.0.1.dev0/docs/
--rw-rw-r--   0 ericof    (1000) ericof    (1000)    18092 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/docs/LICENSE.GPL
--rw-rw-r--   0 ericof    (1000) ericof    (1000)      660 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/docs/LICENSE.rst
--rw-rw-r--   0 ericof    (1000) ericof    (1000)       77 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/docs/index.rst
--rw-rw-r--   0 ericof    (1000) ericof    (1000)      270 2021-11-01 08:37:28.590889 kitconcept.seo-2.0.1.dev0/setup.cfg
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     1803 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/setup.py
-drwxrwxr-x   0 ericof    (1000) ericof    (1000)        0 2021-11-01 08:37:28.586889 kitconcept.seo-2.0.1.dev0/src/
-drwxrwxr-x   0 ericof    (1000) ericof    (1000)        0 2021-11-01 08:37:28.586889 kitconcept.seo-2.0.1.dev0/src/kitconcept/
--rw-rw-r--   0 ericof    (1000) ericof    (1000)       80 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/src/kitconcept/__init__.py
-drwxrwxr-x   0 ericof    (1000) ericof    (1000)        0 2021-11-01 08:37:28.586889 kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/
--rw-rw-r--   0 ericof    (1000) ericof    (1000)      131 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/__init__.py
-drwxrwxr-x   0 ericof    (1000) ericof    (1000)        0 2021-11-01 08:37:28.586889 kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/behaviors/
--rw-rw-r--   0 ericof    (1000) ericof    (1000)        0 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/behaviors/__init__.py
--rw-rw-r--   0 ericof    (1000) ericof    (1000)      549 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/behaviors/configure.zcml
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     3880 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/behaviors/seo.py
-drwxrwxr-x   0 ericof    (1000) ericof    (1000)        0 2021-11-01 08:37:28.586889 kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/browser/
--rw-rw-r--   0 ericof    (1000) ericof    (1000)        0 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/browser/__init__.py
--rw-rw-r--   0 ericof    (1000) ericof    (1000)      568 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/browser/configure.zcml
-drwxrwxr-x   0 ericof    (1000) ericof    (1000)        0 2021-11-01 08:37:28.586889 kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/browser/overrides/
--rw-rw-r--   0 ericof    (1000) ericof    (1000)        0 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/browser/overrides/.gitkeep
-drwxrwxr-x   0 ericof    (1000) ericof    (1000)        0 2021-11-01 08:37:28.586889 kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/browser/static/
--rw-rw-r--   0 ericof    (1000) ericof    (1000)        0 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/browser/static/.gitkeep
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     1083 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/configure.zcml
--rw-rw-r--   0 ericof    (1000) ericof    (1000)      225 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/dependencies.zcml
--rw-rw-r--   0 ericof    (1000) ericof    (1000)      263 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/interfaces.py
-drwxrwxr-x   0 ericof    (1000) ericof    (1000)        0 2021-11-01 08:37:28.590889 kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/locales/
-drwxrwxr-x   0 ericof    (1000) ericof    (1000)        0 2021-11-01 08:37:28.586889 kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/locales/de/
-drwxrwxr-x   0 ericof    (1000) ericof    (1000)        0 2021-11-01 08:37:28.590889 kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/locales/de/LC_MESSAGES/
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     3723 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/locales/de/LC_MESSAGES/kitconcept.seo.po
-drwxrwxr-x   0 ericof    (1000) ericof    (1000)        0 2021-11-01 08:37:28.586889 kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/locales/it/
-drwxrwxr-x   0 ericof    (1000) ericof    (1000)        0 2021-11-01 08:37:28.590889 kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/locales/it/LC_MESSAGES/
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     4193 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/locales/it/LC_MESSAGES/kitconcept.seo.po
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     2886 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/locales/kitconcept.seo.pot
--rwxrwxr-x   0 ericof    (1000) ericof    (1000)      479 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/locales/update.sh
-drwxrwxr-x   0 ericof    (1000) ericof    (1000)        0 2021-11-01 08:37:28.586889 kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/profiles/
-drwxrwxr-x   0 ericof    (1000) ericof    (1000)        0 2021-11-01 08:37:28.590889 kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/profiles/default/
--rw-rw-r--   0 ericof    (1000) ericof    (1000)      168 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/profiles/default/browserlayer.xml
--rw-rw-r--   0 ericof    (1000) ericof    (1000)      188 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/profiles/default/metadata.xml
-drwxrwxr-x   0 ericof    (1000) ericof    (1000)        0 2021-11-01 08:37:28.590889 kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/profiles/uninstall/
--rw-rw-r--   0 ericof    (1000) ericof    (1000)      124 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/profiles/uninstall/browserlayer.xml
--rw-rw-r--   0 ericof    (1000) ericof    (1000)      590 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/setuphandlers.py
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     1413 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/testing.py
-drwxrwxr-x   0 ericof    (1000) ericof    (1000)        0 2021-11-01 08:37:28.590889 kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/tests/
--rw-rw-r--   0 ericof    (1000) ericof    (1000)        0 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/tests/__init__.py
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     2309 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/tests/test_behaviors_seo.py
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     2105 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/tests/test_setup.py
-drwxrwxr-x   0 ericof    (1000) ericof    (1000)        0 2021-11-01 08:37:28.586889 kitconcept.seo-2.0.1.dev0/src/kitconcept.seo.egg-info/
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     9608 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/src/kitconcept.seo.egg-info/PKG-INFO
--rw-rw-r--   0 ericof    (1000) ericof    (1000)     1467 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/src/kitconcept.seo.egg-info/SOURCES.txt
--rw-rw-r--   0 ericof    (1000) ericof    (1000)        1 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/src/kitconcept.seo.egg-info/dependency_links.txt
--rw-rw-r--   0 ericof    (1000) ericof    (1000)       53 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/src/kitconcept.seo.egg-info/entry_points.txt
--rw-rw-r--   0 ericof    (1000) ericof    (1000)       11 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/src/kitconcept.seo.egg-info/namespace_packages.txt
--rw-rw-r--   0 ericof    (1000) ericof    (1000)        1 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/src/kitconcept.seo.egg-info/not-zip-safe
--rw-rw-r--   0 ericof    (1000) ericof    (1000)      162 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/src/kitconcept.seo.egg-info/requires.txt
--rw-rw-r--   0 ericof    (1000) ericof    (1000)       11 2021-11-01 08:37:28.000000 kitconcept.seo-2.0.1.dev0/src/kitconcept.seo.egg-info/top_level.txt
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-05-30 18:13:28.511453 kitconcept_seo-2.1.0/
+-rw-r--r--   0 davisagli   (501) staff       (20)     1363 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/.editorconfig
+-rw-r--r--   0 davisagli   (501) staff       (20)     1531 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/CHANGES.md
+-rw-r--r--   0 davisagli   (501) staff       (20)       56 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/CONTRIBUTORS.md
+-rw-r--r--   0 davisagli   (501) staff       (20)    18092 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/LICENSE.GPL
+-rw-r--r--   0 davisagli   (501) staff       (20)      660 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/LICENSE.md
+-rw-r--r--   0 davisagli   (501) staff       (20)      342 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/MANIFEST.in
+-rw-r--r--   0 davisagli   (501) staff       (20)     7910 2024-05-30 18:13:28.511188 kitconcept_seo-2.1.0/PKG-INFO
+-rw-r--r--   0 davisagli   (501) staff       (20)     4426 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/README.md
+-rw-r--r--   0 davisagli   (501) staff       (20)       61 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/constraints.txt
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-05-30 18:13:28.505432 kitconcept_seo-2.1.0/docs/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/docs/.gitkeep
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-05-30 18:13:28.505545 kitconcept_seo-2.1.0/news/
+-rw-r--r--   0 davisagli   (501) staff       (20)        1 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/news/.gitkeep
+-rw-r--r--   0 davisagli   (501) staff       (20)     4496 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/pyproject.toml
+-rw-r--r--   0 davisagli   (501) staff       (20)       32 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/requirements.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)       38 2024-05-30 18:13:28.511494 kitconcept_seo-2.1.0/setup.cfg
+-rw-r--r--   0 davisagli   (501) staff       (20)     2575 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/setup.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-05-30 18:13:28.502507 kitconcept_seo-2.1.0/src/
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-05-30 18:13:28.505692 kitconcept_seo-2.1.0/src/kitconcept/
+-rw-r--r--   0 davisagli   (501) staff       (20)       56 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/src/kitconcept/__init__.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-05-30 18:13:28.507779 kitconcept_seo-2.1.0/src/kitconcept/seo/
+-rw-r--r--   0 davisagli   (501) staff       (20)      194 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/src/kitconcept/seo/__init__.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-05-30 18:13:28.508171 kitconcept_seo-2.1.0/src/kitconcept/seo/behaviors/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/src/kitconcept/seo/behaviors/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      589 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/src/kitconcept/seo/behaviors/configure.zcml
+-rw-r--r--   0 davisagli   (501) staff       (20)     3829 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/src/kitconcept/seo/behaviors/seo.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      474 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/src/kitconcept/seo/configure.zcml
+-rw-r--r--   0 davisagli   (501) staff       (20)      252 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/src/kitconcept/seo/dependencies.zcml
+-rw-r--r--   0 davisagli   (501) staff       (20)      239 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/src/kitconcept/seo/interfaces.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-05-30 18:13:28.508576 kitconcept_seo-2.1.0/src/kitconcept/seo/locales/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/src/kitconcept/seo/locales/__init__.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-05-30 18:13:28.502911 kitconcept_seo-2.1.0/src/kitconcept/seo/locales/de/
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-05-30 18:13:28.508718 kitconcept_seo-2.1.0/src/kitconcept/seo/locales/de/LC_MESSAGES/
+-rw-r--r--   0 davisagli   (501) staff       (20)     3723 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/src/kitconcept/seo/locales/de/LC_MESSAGES/kitconcept.seo.po
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-05-30 18:13:28.503079 kitconcept_seo-2.1.0/src/kitconcept/seo/locales/it/
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-05-30 18:13:28.508858 kitconcept_seo-2.1.0/src/kitconcept/seo/locales/it/LC_MESSAGES/
+-rw-r--r--   0 davisagli   (501) staff       (20)     4193 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/src/kitconcept/seo/locales/it/LC_MESSAGES/kitconcept.seo.po
+-rw-r--r--   0 davisagli   (501) staff       (20)     2886 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/src/kitconcept/seo/locales/kitconcept.seo.pot
+-rwxr-xr-x   0 davisagli   (501) staff       (20)      479 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/src/kitconcept/seo/locales/update.sh
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-05-30 18:13:28.503310 kitconcept_seo-2.1.0/src/kitconcept/seo/profiles/
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-05-30 18:13:28.509151 kitconcept_seo-2.1.0/src/kitconcept/seo/profiles/default/
+-rw-r--r--   0 davisagli   (501) staff       (20)      161 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/src/kitconcept/seo/profiles/default/browserlayer.xml
+-rw-r--r--   0 davisagli   (501) staff       (20)      188 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/src/kitconcept/seo/profiles/default/metadata.xml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-05-30 18:13:28.509297 kitconcept_seo-2.1.0/src/kitconcept/seo/profiles/uninstall/
+-rw-r--r--   0 davisagli   (501) staff       (20)      117 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/src/kitconcept/seo/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 davisagli   (501) staff       (20)      849 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/src/kitconcept/seo/profiles.zcml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-05-30 18:13:28.509439 kitconcept_seo-2.1.0/src/kitconcept/seo/setuphandlers/
+-rw-r--r--   0 davisagli   (501) staff       (20)      334 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/src/kitconcept/seo/setuphandlers/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      657 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/src/kitconcept/seo/subscribers.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1183 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/src/kitconcept/seo/testing.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-05-30 18:13:28.509707 kitconcept_seo-2.1.0/src/kitconcept/seo/upgrades/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/src/kitconcept/seo/upgrades/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      451 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/src/kitconcept/seo/upgrades/configure.zcml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-05-30 18:13:28.510490 kitconcept_seo-2.1.0/src/kitconcept.seo.egg-info/
+-rw-r--r--   0 davisagli   (501) staff       (20)     7910 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/src/kitconcept.seo.egg-info/PKG-INFO
+-rw-r--r--   0 davisagli   (501) staff       (20)     1534 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/src/kitconcept.seo.egg-info/SOURCES.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)        1 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/src/kitconcept.seo.egg-info/dependency_links.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)      124 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/src/kitconcept.seo.egg-info/entry_points.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)       11 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/src/kitconcept.seo.egg-info/namespace_packages.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)        1 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/src/kitconcept.seo.egg-info/not-zip-safe
+-rw-r--r--   0 davisagli   (501) staff       (20)      309 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/src/kitconcept.seo.egg-info/requires.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)       11 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/src/kitconcept.seo.egg-info/top_level.txt
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-05-30 18:13:28.509983 kitconcept_seo-2.1.0/tests/
+-rw-r--r--   0 davisagli   (501) staff       (20)      753 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/tests/conftest.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-05-30 18:13:28.510261 kitconcept_seo-2.1.0/tests/setup/
+-rw-r--r--   0 davisagli   (501) staff       (20)      646 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/tests/setup/test_setup_install.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      629 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/tests/setup/test_setup_uninstall.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1523 2024-05-30 18:13:28.000000 kitconcept_seo-2.1.0/tests/test_behavior.py
```

### Comparing `kitconcept.seo-2.0.1.dev0/docs/LICENSE.GPL` & `kitconcept_seo-2.1.0/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `kitconcept.seo-2.0.1.dev0/docs/LICENSE.rst` & `kitconcept_seo-2.1.0/LICENSE.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-kitconcept.seo Copyright 2018, kitconcept GmbH
+kitconcept.seo Copyright 2023, Plone Community
 
 This program is free software; you can redistribute it and/or
 modify it under the terms of the GNU General Public License version 2
 as published by the Free Software Foundation.
 
 This program is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
```

### Comparing `kitconcept.seo-2.0.1.dev0/setup.py` & `kitconcept_seo-2.1.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,62 +1,82 @@
-# -*- coding: utf-8 -*-
 """Installer for the kitconcept.seo package."""
 
+from pathlib import Path
 from setuptools import find_packages
 from setuptools import setup
 
 
-long_description = '\n\n'.join([
-    open('README.rst').read(),
-    open('CONTRIBUTORS.rst').read(),
-    open('CHANGES.rst').read(),
-])
+long_description = f"""
+{Path("README.md").read_text()}\n
+{Path("CONTRIBUTORS.md").read_text()}\n
+{Path("CHANGES.md").read_text()}\n
+"""
 
 
 setup(
-    name='kitconcept.seo',
-    version='2.0.1.dev0',
+    name="kitconcept.seo",
+    version="2.1.0",
     description="SEO optimizations plugin for Plone",
     long_description=long_description,
-    # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
+    long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
-        "Framework :: Plone :: 5.2",
+        "Framework :: Plone :: Addon",
+        "Framework :: Plone :: 6.0",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     ],
-    keywords='Python Plone',
-    author='kitconcept GmbH',
-    author_email='info@kitconcept.com',
-    url='https://pypi.python.org/pypi/kitconcept.seo',
-    license='GPL version 2',
-    packages=find_packages('src', exclude=['ez_setup']),
-    namespace_packages=['kitconcept'],
-    package_dir={'': 'src'},
+    keywords="Python Plone CMS",
+    author="kitconcept GmbH",
+    author_email="info@kitconcept.com",
+    url="https://pypi.python.org/pypi/kitconcept.seo",
+    project_urls={
+        "PyPI": "https://pypi.python.org/pypi/kitconcept.seo",
+        "Source": "https://github.com/kitconcept/kitconcept.seo",
+        "Tracker": "https://github.com/kitconcept/kitconcept.seo/issues",
+    },
+    license="GPL version 2",
+    packages=find_packages("src", exclude=["ez_setup"]),
+    namespace_packages=["kitconcept"],
+    package_dir={"": "src"},
     include_package_data=True,
     zip_safe=False,
+    python_requires=">=3.8",
     install_requires=[
-        'plone.api',
-        'Products.GenericSetup',
-        'setuptools',
-        'z3c.jbot',
-        'plone.behavior',
+        "setuptools",
+        "Products.CMFPlone",
+        "plone.app.dexterity",
+        "plone.autoform",
+        "plone.behavior",
+        "plone.dexterity",
+        "plone.namedfile",
+        "plone.supermodel",
     ],
     extras_require={
-        'test': [
-            'plone.app.testing',
-            'plone.testing',
-            'plone.app.contenttypes',
-            'plone.app.robotframework[debug]',
+        "test": [
+            "zest.releaser[recommended]",
+            "zestreleaser.towncrier",
+            "plone.app.contenttypes[test]",
+            "plone.app.testing",
+            "plone.restapi[test]",
+            # Undeclared dependency of plone.restapi,
+            # can be removed after next release
+            "plone.app.iterate",
+            "pytest",
+            "pytest-cov",
+            "pytest-plone>=0.2.0",
         ],
     },
     entry_points="""
     [z3c.autoinclude.plugin]
     target = plone
+    [console_scripts]
+    update_dist_locale = kitconcept.seo.locales.update:update_locale
     """,
 )
```

### Comparing `kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/behaviors/seo.py` & `kitconcept_seo-2.1.0/src/kitconcept/seo/behaviors/seo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-# -*- coding: utf-8 -*-
 from kitconcept.seo import _
 from plone.autoform.interfaces import IFormFieldProvider
 from plone.dexterity.interfaces import IDexterityContent
 from plone.namedfile.field import NamedBlobImage
 from plone.supermodel import model
 from zope import schema
 from zope.component import adapter
 from zope.interface import implementer
 from zope.interface import provider
 
 
 @provider(IFormFieldProvider)
 class ISeo(model.Schema):
-
     model.fieldset(
         "seo",
-        label=_(u"SEO"),
+        label=_("SEO"),
         fields=[
             "seo_title",
             "seo_description",
             "seo_noindex",
             "seo_canonical_url",
             #            "seo_nofollow",
             #            "seo_noarchive",
@@ -29,41 +27,41 @@
             "opengraph_image",
         ],
     )
 
     seo_title = schema.TextLine(
         title=_("Title"),
         description=_(
-            u"Override the meta title. When empty the default title will "
-            + u"be used. Use maximum 50 characters."
+            "Override the meta title. When empty the default title will "
+            + "be used. Use maximum 50 characters."
         ),
         required=False,
     )
 
     seo_description = schema.TextLine(
-        title=_(u"Description"),
+        title=_("Description"),
         description=_(
-            u"Override the meta description. When empty the default "
-            + u"description will be used. Use maximum 150 characters."
+            "Override the meta description. When empty the default "
+            + "description will be used. Use maximum 150 characters."
         ),
         required=False,
     )
 
     # https://support.google.com/webmasters/answer/93710?hl=en
     seo_noindex = schema.Bool(
-        title=_(u"No Index"),
-        description=_(u"Prevents a page from appearing in search engines"),
+        title=_("No Index"),
+        description=_("Prevents a page from appearing in search engines"),
         required=False,
     )
 
     # https://support.google.com/webmasters/answer/139066?hl=en
     seo_canonical_url = schema.URI(
-        title=_(u"Canonical URL"),
+        title=_("Canonical URL"),
         description=_(
-            u"Tells the search engine to choose this URL as the canonical version and crawl that."
+            "Tells the search engine to choose this URL as the canonical version and crawl that."
         ),
         required=False,
     )
 
     # # https://support.google.com/webmasters/answer/96569?hl=en
     # seo_nofollow = schema.Bool(
     #     title=_(u"No Follow"),
@@ -87,37 +85,37 @@
     #     ),
     #     required=False,
     # )
 
     opengraph_title = schema.TextLine(
         title=_("Open Graph Title"),
         description=_(
-            u"Override the Open Graph title, that Facebook and Twitter use. When empty the default title will "
-            + u"be used. Use maximum 60 characters."
+            "Override the Open Graph title, that Facebook and Twitter use. When empty the default title will "
+            + "be used. Use maximum 60 characters."
         ),
         required=False,
     )
 
     opengraph_description = schema.TextLine(
-        title=_(u"Open Graph Description"),
+        title=_("Open Graph Description"),
         description=_(
-            u"Override the Open Graph description, that Facebook and Twitter use. When empty the default "
-            + u"description will be used. Use maximum 155 characters."
+            "Override the Open Graph description, that Facebook and Twitter use. When empty the default "
+            + "description will be used. Use maximum 155 characters."
         ),
         required=False,
     )
 
     opengraph_image = NamedBlobImage(
-        title=_(u"Open Graph Image"),
+        title=_("Open Graph Image"),
         description=_(
-            u"Override the Open Graph image, that Facebook and Twitter use. When empty the default "
-            + u"lead image will be used. Recommended image ratio is 1,91:1 and 1200 x 630px."
+            "Override the Open Graph image, that Facebook and Twitter use. When empty the default "
+            + "lead image will be used. Recommended image ratio is 1,91:1 and 1200 x 630px."
         ),
         required=False,
     )
 
 
 @implementer(ISeo)
 @adapter(IDexterityContent)
-class Seo(object):
+class Seo:
     def __init__(self, context):
         self.context = context
```

### Comparing `kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/browser/configure.zcml` & `kitconcept_seo-2.1.0/src/kitconcept/seo/behaviors/configure.zcml`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
-    xmlns:browser="http://namespaces.zope.org/browser"
     xmlns:plone="http://namespaces.plone.org/plone"
-    i18n_domain="kitconcept.seo">
+    xmlns:zcml="http://namespaces.zope.org/zcml"
+    i18n_domain="kitconcept.seo"
+    >
 
-  <!-- Set overrides folder for Just-a-Bunch-Of-Templates product -->
-  <include package="z3c.jbot" file="meta.zcml" />
-  <browser:jbot
-      directory="overrides"
-      layer="kitconcept.seo.interfaces.IKitconceptSeoLayer"
+  <include
+      package="plone.behavior"
+      file="meta.zcml"
       />
 
-  <!-- Publish static files -->
-  <browser:resourceDirectory
+  <plone:behavior
       name="kitconcept.seo"
-      directory="static"
+      title="SEO Behavior"
+      description="Enhances a content type with fields for Search Engine Optimizations"
+      factory=".seo.Seo"
+      provides=".seo.ISeo"
+      for="plone.dexterity.interfaces.IDexterityContent"
+      marker=".seo.ISeo"
       />
 
 </configure>
```

### Comparing `kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/configure.zcml` & `kitconcept_seo-2.1.0/src/kitconcept/seo/profiles.zcml`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,32 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
-    xmlns:i18n="http://namespaces.zope.org/i18n"
-    i18n_domain="kitconcept.seo">
-
-  <i18n:registerTranslations directory="locales" />
-
-  <include file="dependencies.zcml" />
-
-  <include package=".behaviors" />
-  <include package=".browser" />
-
+    i18n_domain="kitconcept.seo"
+    >
 
   <genericsetup:registerProfile
       name="default"
-      title="kitconcept.seo"
-      directory="profiles/default"
+      title="kitconcept seo: Install"
       description="Installs the kitconcept.seo add-on."
       provides="Products.GenericSetup.interfaces.EXTENSION"
-      post_handler=".setuphandlers.post_install"
+      directory="profiles/default"
       />
 
   <genericsetup:registerProfile
       name="uninstall"
-      title="kitconcept.seo (uninstall)"
-      directory="profiles/uninstall"
+      title="kitconcept seo: Uninstall"
       description="Uninstalls the kitconcept.seo add-on."
       provides="Products.GenericSetup.interfaces.EXTENSION"
-      post_handler=".setuphandlers.uninstall"
+      directory="profiles/uninstall"
       />
 
+  <!-- Hide Uninstall Profile-->
   <utility
       factory=".setuphandlers.HiddenProfiles"
-      name="kitconcept.seo-hiddenprofiles" />
+      name="kitconcept.seo"
+      />
+
+
+  <include package=".upgrades" />
 
 </configure>
```

### Comparing `kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/locales/de/LC_MESSAGES/kitconcept.seo.po` & `kitconcept_seo-2.1.0/src/kitconcept/seo/locales/de/LC_MESSAGES/kitconcept.seo.po`

 * *Files identical despite different names*

### Comparing `kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/locales/it/LC_MESSAGES/kitconcept.seo.po` & `kitconcept_seo-2.1.0/src/kitconcept/seo/locales/it/LC_MESSAGES/kitconcept.seo.po`

 * *Files identical despite different names*

### Comparing `kitconcept.seo-2.0.1.dev0/src/kitconcept/seo/locales/kitconcept.seo.pot` & `kitconcept_seo-2.1.0/src/kitconcept/seo/locales/kitconcept.seo.pot`

 * *Files identical despite different names*

### Comparing `kitconcept.seo-2.0.1.dev0/src/kitconcept.seo.egg-info/SOURCES.txt` & `kitconcept_seo-2.1.0/src/kitconcept.seo.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,47 @@
-CHANGES.rst
-CONTRIBUTORS.rst
+.editorconfig
+CHANGES.md
+CONTRIBUTORS.md
+LICENSE.GPL
+LICENSE.md
 MANIFEST.in
-README.rst
-setup.cfg
+README.md
+constraints.txt
+pyproject.toml
+requirements.txt
 setup.py
-docs/LICENSE.GPL
-docs/LICENSE.rst
-docs/index.rst
+docs/.gitkeep
+news/.gitkeep
 src/kitconcept/__init__.py
 src/kitconcept.seo.egg-info/PKG-INFO
 src/kitconcept.seo.egg-info/SOURCES.txt
 src/kitconcept.seo.egg-info/dependency_links.txt
 src/kitconcept.seo.egg-info/entry_points.txt
 src/kitconcept.seo.egg-info/namespace_packages.txt
 src/kitconcept.seo.egg-info/not-zip-safe
 src/kitconcept.seo.egg-info/requires.txt
 src/kitconcept.seo.egg-info/top_level.txt
 src/kitconcept/seo/__init__.py
 src/kitconcept/seo/configure.zcml
 src/kitconcept/seo/dependencies.zcml
 src/kitconcept/seo/interfaces.py
-src/kitconcept/seo/setuphandlers.py
+src/kitconcept/seo/profiles.zcml
+src/kitconcept/seo/subscribers.py
 src/kitconcept/seo/testing.py
 src/kitconcept/seo/behaviors/__init__.py
 src/kitconcept/seo/behaviors/configure.zcml
 src/kitconcept/seo/behaviors/seo.py
-src/kitconcept/seo/browser/__init__.py
-src/kitconcept/seo/browser/configure.zcml
-src/kitconcept/seo/browser/overrides/.gitkeep
-src/kitconcept/seo/browser/static/.gitkeep
+src/kitconcept/seo/locales/__init__.py
 src/kitconcept/seo/locales/kitconcept.seo.pot
 src/kitconcept/seo/locales/update.sh
 src/kitconcept/seo/locales/de/LC_MESSAGES/kitconcept.seo.po
 src/kitconcept/seo/locales/it/LC_MESSAGES/kitconcept.seo.po
 src/kitconcept/seo/profiles/default/browserlayer.xml
 src/kitconcept/seo/profiles/default/metadata.xml
 src/kitconcept/seo/profiles/uninstall/browserlayer.xml
-src/kitconcept/seo/tests/__init__.py
-src/kitconcept/seo/tests/test_behaviors_seo.py
-src/kitconcept/seo/tests/test_setup.py
+src/kitconcept/seo/setuphandlers/__init__.py
+src/kitconcept/seo/upgrades/__init__.py
+src/kitconcept/seo/upgrades/configure.zcml
+tests/conftest.py
+tests/test_behavior.py
+tests/setup/test_setup_install.py
+tests/setup/test_setup_uninstall.py
```

