# Comparing `tmp/imio.smartweb.policy-1.2.4.tar.gz` & `tmp/imio_smartweb_policy-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imio.smartweb.policy-1.2.4.tar", last modified: Fri Feb  2 08:39:39 2024, max compression
+gzip compressed data, was "imio_smartweb_policy-1.2.5.tar", last modified: Thu May 30 09:19:25 2024, max compression
```

## Comparing `imio.smartweb.policy-1.2.4.tar` & `imio_smartweb_policy-1.2.5.tar`

### file list

```diff
@@ -1,163 +1,166 @@
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.835832 imio.smartweb.policy-1.2.4/
--rw-r--r--   0 thom       (501) staff       (20)     8236 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/CHANGES.rst
--rw-r--r--   0 thom       (501) staff       (20)       80 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/CONTRIBUTORS.rst
--rw-r--r--   0 thom       (501) staff       (20)      520 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/DEVELOP.rst
--rw-r--r--   0 thom       (501) staff       (20)    18092 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/LICENSE.GPL
--rw-r--r--   0 thom       (501) staff       (20)      671 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/LICENSE.rst
--rw-r--r--   0 thom       (501) staff       (20)       61 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/MANIFEST.in
--rw-r--r--   0 thom       (501) staff       (20)    11460 2024-02-02 08:39:39.835963 imio.smartweb.policy-1.2.4/PKG-INFO
--rw-r--r--   0 thom       (501) staff       (20)     2090 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/README.rst
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.806542 imio.smartweb.policy-1.2.4/docs/
--rw-r--r--   0 thom       (501) staff       (20)     7998 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/docs/conf.py
--rw-r--r--   0 thom       (501) staff       (20)       83 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/docs/index.rst
--rw-r--r--   0 thom       (501) staff       (20)      518 2024-02-02 08:39:39.836666 imio.smartweb.policy-1.2.4/setup.cfg
--rw-r--r--   0 thom       (501) staff       (20)     2890 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/setup.py
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.792458 imio.smartweb.policy-1.2.4/src/
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.806868 imio.smartweb.policy-1.2.4/src/imio/
--rw-r--r--   0 thom       (501) staff       (20)       80 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/__init__.py
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.809594 imio.smartweb.policy-1.2.4/src/imio/smartweb/
--rw-r--r--   0 thom       (501) staff       (20)       80 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/__init__.py
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.814329 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/
--rw-r--r--   0 thom       (501) staff       (20)      341 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/__init__.py
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.814927 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/browser/
--rw-r--r--   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/browser/__init__.py
--rw-r--r--   0 thom       (501) staff       (20)     1326 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/browser/configure.zcml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.815905 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/browser/faceted/
--rw-r--r--   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/browser/faceted/__init__.py
--rw-r--r--   0 thom       (501) staff       (20)      944 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/browser/faceted/configure.zcml
--rw-r--r--   0 thom       (501) staff       (20)      707 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/browser/faceted/subtyper.py
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.816238 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/browser/overrides/
--rw-r--r--   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/browser/overrides/.gitkeep
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.816504 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/browser/static/
--rw-r--r--   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/browser/static/.gitkeep
--rw-r--r--   0 thom       (501) staff       (20)      533 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/caching.py
--rw-r--r--   0 thom       (501) staff       (20)      814 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/caching.zcml
--rw-r--r--   0 thom       (501) staff       (20)     1529 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/configure.zcml
--rw-r--r--   0 thom       (501) staff       (20)      268 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/interfaces.py
--rw-r--r--   0 thom       (501) staff       (20)     1769 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/monkey.py
--rw-r--r--   0 thom       (501) staff       (20)      549 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/permissions.zcml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.795304 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.818081 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/default/
--rw-r--r--   0 thom       (501) staff       (20)      185 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/default/browserlayer.xml
--rw-r--r--   0 thom       (501) staff       (20)     1177 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/default/controlpanel.xml
--rw-r--r--   0 thom       (501) staff       (20)      780 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/default/metadata.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.819727 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/default/registry/
--rw-r--r--   0 thom       (501) staff       (20)     8287 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/default/registry/autopublishing.xml
--rw-r--r--   0 thom       (501) staff       (20)     1307 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/default/registry/autoscaling.xml
--rw-r--r--   0 thom       (501) staff       (20)     4086 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/default/registry/caching.xml
--rw-r--r--   0 thom       (501) staff       (20)      296 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/default/registry/messagesviewlet.xml
--rw-r--r--   0 thom       (501) staff       (20)      961 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/default/registry/smartweb.xml
--rw-r--r--   0 thom       (501) staff       (20)     2026 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/default/rolemap.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.822700 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/default/types/
--rw-r--r--   0 thom       (501) staff       (20)      967 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/default/types/Collection.xml
--rw-r--r--   0 thom       (501) staff       (20)      215 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/default/types/Document.xml
--rw-r--r--   0 thom       (501) staff       (20)      212 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/default/types/Event.xml
--rw-r--r--   0 thom       (501) staff       (20)      591 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/default/types/File.xml
--rw-r--r--   0 thom       (501) staff       (20)      213 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/default/types/Folder.xml
--rw-r--r--   0 thom       (501) staff       (20)      355 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/default/types/Image.xml
--rw-r--r--   0 thom       (501) staff       (20)      354 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/default/types/Link.xml
--rw-r--r--   0 thom       (501) staff       (20)      216 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/default/types/News_Item.xml
--rw-r--r--   0 thom       (501) staff       (20)      186 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/default/types/Plone_Site.xml
--rw-r--r--   0 thom       (501) staff       (20)     2949 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/default/viewlets.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.823026 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/demo/
--rw-r--r--   0 thom       (501) staff       (20)      189 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/demo/metadata.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.823355 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/multilingual/
--rw-r--r--   0 thom       (501) staff       (20)     1432 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/multilingual/registry.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.826728 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/multilingual/types/
--rw-r--r--   0 thom       (501) staff       (20)      268 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/multilingual/types/Collection.xml
--rw-r--r--   0 thom       (501) staff       (20)      262 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/multilingual/types/Link.xml
--rw-r--r--   0 thom       (501) staff       (20)      290 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/multilingual/types/imio.smartweb.CirkwiView.xml
--rw-r--r--   0 thom       (501) staff       (20)      293 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/multilingual/types/imio.smartweb.DirectoryView.xml
--rw-r--r--   0 thom       (501) staff       (20)      290 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/multilingual/types/imio.smartweb.EventsView.xml
--rw-r--r--   0 thom       (501) staff       (20)      286 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/multilingual/types/imio.smartweb.Folder.xml
--rw-r--r--   0 thom       (501) staff       (20)      288 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/multilingual/types/imio.smartweb.NewsView.xml
--rw-r--r--   0 thom       (501) staff       (20)      284 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/multilingual/types/imio.smartweb.Page.xml
--rw-r--r--   0 thom       (501) staff       (20)      290 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/multilingual/types/imio.smartweb.PortalPage.xml
--rw-r--r--   0 thom       (501) staff       (20)      289 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/multilingual/types/imio.smartweb.Procedure.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.827048 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/uninstall/
--rw-r--r--   0 thom       (501) staff       (20)      205 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 thom       (501) staff       (20)     1585 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles.zcml
--rw-r--r--   0 thom       (501) staff       (20)     2250 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/setupdemo.py
--rw-r--r--   0 thom       (501) staff       (20)     4308 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/setuphandlers.py
--rw-r--r--   0 thom       (501) staff       (20)      234 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/subscribers.zcml
--rw-r--r--   0 thom       (501) staff       (20)     1749 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/testing.py
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.827904 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/tests/
--rw-r--r--   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/tests/__init__.py
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.828205 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/tests/robot/
--rw-r--r--   0 thom       (501) staff       (20)     2011 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/tests/robot/test_example.robot
--rw-r--r--   0 thom       (501) staff       (20)      955 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/tests/test_robot.py
--rw-r--r--   0 thom       (501) staff       (20)     2102 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/tests/test_setup.py
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.829071 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/
--rw-r--r--   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/__init__.py
--rw-r--r--   0 thom       (501) staff       (20)    17962 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/configure.zcml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.802856 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.796444 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1006_to_1007/
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.829369 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1006_to_1007/registry/
--rw-r--r--   0 thom       (501) staff       (20)     3749 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1006_to_1007/registry/caching.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.796818 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1008_to_1009/
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.829661 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1008_to_1009/registry/
--rw-r--r--   0 thom       (501) staff       (20)      136 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1008_to_1009/registry/caching.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.797176 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1010_to_1011/
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.829961 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1010_to_1011/registry/
--rw-r--r--   0 thom       (501) staff       (20)      148 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1010_to_1011/registry/caching.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.797531 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1011_to_1012/
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.830281 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1011_to_1012/registry/
--rw-r--r--   0 thom       (501) staff       (20)     1307 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1011_to_1012/registry/collective.autoscaling.values.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.797884 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1013_to_1014/
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.830587 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1013_to_1014/registry/
--rw-r--r--   0 thom       (501) staff       (20)      561 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1013_to_1014/registry/collective.autoscaling.values.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.798237 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1014_to_1015/
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.830891 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1014_to_1015/registry/
--rw-r--r--   0 thom       (501) staff       (20)      515 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1014_to_1015/registry/caching.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.798605 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1017_to_1018/
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.831184 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1017_to_1018/registry/
--rw-r--r--   0 thom       (501) staff       (20)      311 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1017_to_1018/registry/smartweb.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.798970 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1018_to_1019/
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.831477 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1018_to_1019/registry/
--rw-r--r--   0 thom       (501) staff       (20)      235 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1018_to_1019/registry/smartweb.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.799337 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1019_to_1020/
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.831783 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1019_to_1020/registry/
--rw-r--r--   0 thom       (501) staff       (20)      235 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1019_to_1020/registry/caching.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.832366 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1020_to_1021/
--rw-r--r--   0 thom       (501) staff       (20)     1177 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1020_to_1021/controlpanel.xml
--rw-r--r--   0 thom       (501) staff       (20)     1787 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1020_to_1021/rolemap.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.799925 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1021_to_1022/
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.832652 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1021_to_1022/registry/
--rw-r--r--   0 thom       (501) staff       (20)     3970 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1021_to_1022/registry/caching.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.800290 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1022_to_1023/
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.832959 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1022_to_1023/registry/
--rw-r--r--   0 thom       (501) staff       (20)     4086 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1022_to_1023/registry/caching.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.800661 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1023_to_1024/
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.833251 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1023_to_1024/registry/
--rw-r--r--   0 thom       (501) staff       (20)      332 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1023_to_1024/registry/bundles.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.801015 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1026_to_1027/
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.833545 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1026_to_1027/registry/
--rw-r--r--   0 thom       (501) staff       (20)     8287 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1026_to_1027/registry/autopublishing.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.801375 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1028_to_1029/
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.833842 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1028_to_1029/registry/
--rw-r--r--   0 thom       (501) staff       (20)      296 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1028_to_1029/registry/messagesviewlet.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.834422 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1029_to_1030/
--rw-r--r--   0 thom       (501) staff       (20)      457 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1029_to_1030/controlpanel.xml
--rw-r--r--   0 thom       (501) staff       (20)      233 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1029_to_1030/rolemap.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.801939 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1030_to_1031/
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.834709 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1030_to_1031/types/
--rw-r--r--   0 thom       (501) staff       (20)      358 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1030_to_1031/types/Collection.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.802289 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1031_to_1032/
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.835012 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1031_to_1032/types/
--rw-r--r--   0 thom       (501) staff       (20)      809 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1031_to_1032/types/Collection.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.802649 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1032_to_1033/
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.835312 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1032_to_1033/registry/
--rw-r--r--   0 thom       (501) staff       (20)     1307 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1032_to_1033/registry/collective.autoscaling.values.xml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.835604 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1033_to_1034/
--rw-r--r--   0 thom       (501) staff       (20)      304 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1033_to_1034/viewlets.xml
--rw-r--r--   0 thom       (501) staff       (20)     1586 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/upgrades.py
--rw-r--r--   0 thom       (501) staff       (20)     2954 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/utils.py
--rw-r--r--   0 thom       (501) staff       (20)     1200 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/viewlets.zcml
-drwxr-xr-x   0 thom       (501) staff       (20)        0 2024-02-02 08:39:39.809261 imio.smartweb.policy-1.2.4/src/imio.smartweb.policy.egg-info/
--rw-r--r--   0 thom       (501) staff       (20)    11460 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio.smartweb.policy.egg-info/PKG-INFO
--rw-r--r--   0 thom       (501) staff       (20)     5598 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio.smartweb.policy.egg-info/SOURCES.txt
--rw-r--r--   0 thom       (501) staff       (20)        1 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio.smartweb.policy.egg-info/dependency_links.txt
--rw-r--r--   0 thom       (501) staff       (20)       19 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio.smartweb.policy.egg-info/namespace_packages.txt
--rw-r--r--   0 thom       (501) staff       (20)        1 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio.smartweb.policy.egg-info/not-zip-safe
--rw-r--r--   0 thom       (501) staff       (20)      518 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio.smartweb.policy.egg-info/requires.txt
--rw-r--r--   0 thom       (501) staff       (20)        5 2024-02-02 08:39:39.000000 imio.smartweb.policy-1.2.4/src/imio.smartweb.policy.egg-info/top_level.txt
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.341762 imio_smartweb_policy-1.2.5/
+-rw-r--r--   0 laurent    (501) staff       (20)     8355 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/CHANGES.rst
+-rw-r--r--   0 laurent    (501) staff       (20)       80 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/CONTRIBUTORS.rst
+-rw-r--r--   0 laurent    (501) staff       (20)      520 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/DEVELOP.rst
+-rw-r--r--   0 laurent    (501) staff       (20)    18092 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/LICENSE.GPL
+-rw-r--r--   0 laurent    (501) staff       (20)      671 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/LICENSE.rst
+-rw-r--r--   0 laurent    (501) staff       (20)       61 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/MANIFEST.in
+-rw-r--r--   0 laurent    (501) staff       (20)    12532 2024-05-30 09:19:25.341686 imio_smartweb_policy-1.2.5/PKG-INFO
+-rw-r--r--   0 laurent    (501) staff       (20)     2090 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/README.rst
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.331004 imio_smartweb_policy-1.2.5/docs/
+-rw-r--r--   0 laurent    (501) staff       (20)     7998 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/docs/conf.py
+-rw-r--r--   0 laurent    (501) staff       (20)       83 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/docs/index.rst
+-rw-r--r--   0 laurent    (501) staff       (20)      518 2024-05-30 09:19:25.341974 imio_smartweb_policy-1.2.5/setup.cfg
+-rw-r--r--   0 laurent    (501) staff       (20)     2890 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/setup.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.326543 imio_smartweb_policy-1.2.5/src/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.331122 imio_smartweb_policy-1.2.5/src/imio/
+-rw-r--r--   0 laurent    (501) staff       (20)       80 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/__init__.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.332079 imio_smartweb_policy-1.2.5/src/imio/smartweb/
+-rw-r--r--   0 laurent    (501) staff       (20)       80 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/__init__.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.333577 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/
+-rw-r--r--   0 laurent    (501) staff       (20)      341 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/__init__.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.333741 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/browser/
+-rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/browser/__init__.py
+-rw-r--r--   0 laurent    (501) staff       (20)     1326 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/browser/configure.zcml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.334010 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/browser/faceted/
+-rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/browser/faceted/__init__.py
+-rw-r--r--   0 laurent    (501) staff       (20)      944 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/browser/faceted/configure.zcml
+-rw-r--r--   0 laurent    (501) staff       (20)      707 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/browser/faceted/subtyper.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.334104 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/browser/overrides/
+-rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/browser/overrides/.gitkeep
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.334187 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/browser/static/
+-rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/browser/static/.gitkeep
+-rw-r--r--   0 laurent    (501) staff       (20)      533 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/caching.py
+-rw-r--r--   0 laurent    (501) staff       (20)      814 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/caching.zcml
+-rw-r--r--   0 laurent    (501) staff       (20)     1529 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/configure.zcml
+-rw-r--r--   0 laurent    (501) staff       (20)      268 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/interfaces.py
+-rw-r--r--   0 laurent    (501) staff       (20)     1769 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/monkey.py
+-rw-r--r--   0 laurent    (501) staff       (20)      549 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/permissions.zcml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.327323 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.334642 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/default/
+-rw-r--r--   0 laurent    (501) staff       (20)      185 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/default/browserlayer.xml
+-rw-r--r--   0 laurent    (501) staff       (20)     1177 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/default/controlpanel.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      780 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/default/metadata.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.335159 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/default/registry/
+-rw-r--r--   0 laurent    (501) staff       (20)     8287 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/default/registry/autopublishing.xml
+-rw-r--r--   0 laurent    (501) staff       (20)     1307 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/default/registry/autoscaling.xml
+-rw-r--r--   0 laurent    (501) staff       (20)     4218 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/default/registry/caching.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      296 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/default/registry/messagesviewlet.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      961 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/default/registry/smartweb.xml
+-rw-r--r--   0 laurent    (501) staff       (20)     2026 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/default/rolemap.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.336267 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/default/types/
+-rw-r--r--   0 laurent    (501) staff       (20)      967 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/default/types/Collection.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      215 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/default/types/Document.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      212 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/default/types/Event.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      591 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/default/types/File.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      213 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/default/types/Folder.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      355 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/default/types/Image.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      354 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/default/types/Link.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      216 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/default/types/News_Item.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      186 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/default/types/Plone_Site.xml
+-rw-r--r--   0 laurent    (501) staff       (20)     2949 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/default/viewlets.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.336381 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/demo/
+-rw-r--r--   0 laurent    (501) staff       (20)      189 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/demo/metadata.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.336493 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/multilingual/
+-rw-r--r--   0 laurent    (501) staff       (20)     1432 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/multilingual/registry.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.337612 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/multilingual/types/
+-rw-r--r--   0 laurent    (501) staff       (20)      268 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/multilingual/types/Collection.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      262 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/multilingual/types/Link.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      290 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/multilingual/types/imio.smartweb.CirkwiView.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      293 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/multilingual/types/imio.smartweb.DirectoryView.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      290 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/multilingual/types/imio.smartweb.EventsView.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      286 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/multilingual/types/imio.smartweb.Folder.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      288 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/multilingual/types/imio.smartweb.NewsView.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      284 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/multilingual/types/imio.smartweb.Page.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      290 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/multilingual/types/imio.smartweb.PortalPage.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      289 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/multilingual/types/imio.smartweb.Procedure.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.337728 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/uninstall/
+-rw-r--r--   0 laurent    (501) staff       (20)      205 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 laurent    (501) staff       (20)     1585 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles.zcml
+-rw-r--r--   0 laurent    (501) staff       (20)     2250 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/setupdemo.py
+-rw-r--r--   0 laurent    (501) staff       (20)     4308 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/setuphandlers.py
+-rw-r--r--   0 laurent    (501) staff       (20)      234 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/subscribers.zcml
+-rw-r--r--   0 laurent    (501) staff       (20)     1749 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/testing.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.338029 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/tests/
+-rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/tests/__init__.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.338143 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/tests/robot/
+-rw-r--r--   0 laurent    (501) staff       (20)     2011 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/tests/robot/test_example.robot
+-rw-r--r--   0 laurent    (501) staff       (20)      955 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/tests/test_robot.py
+-rw-r--r--   0 laurent    (501) staff       (20)     2102 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/tests/test_setup.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.338477 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/
+-rw-r--r--   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/__init__.py
+-rw-r--r--   0 laurent    (501) staff       (20)    18594 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/configure.zcml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.329623 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.327634 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1006_to_1007/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.338590 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1006_to_1007/registry/
+-rw-r--r--   0 laurent    (501) staff       (20)     3749 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1006_to_1007/registry/caching.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.327734 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1008_to_1009/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.338701 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1008_to_1009/registry/
+-rw-r--r--   0 laurent    (501) staff       (20)      136 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1008_to_1009/registry/caching.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.327838 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1010_to_1011/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.338814 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1010_to_1011/registry/
+-rw-r--r--   0 laurent    (501) staff       (20)      148 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1010_to_1011/registry/caching.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.327942 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1011_to_1012/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.338945 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1011_to_1012/registry/
+-rw-r--r--   0 laurent    (501) staff       (20)     1307 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1011_to_1012/registry/collective.autoscaling.values.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.328044 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1013_to_1014/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.339067 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1013_to_1014/registry/
+-rw-r--r--   0 laurent    (501) staff       (20)      561 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1013_to_1014/registry/collective.autoscaling.values.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.328143 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1014_to_1015/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.339185 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1014_to_1015/registry/
+-rw-r--r--   0 laurent    (501) staff       (20)      515 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1014_to_1015/registry/caching.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.328242 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1017_to_1018/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.339304 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1017_to_1018/registry/
+-rw-r--r--   0 laurent    (501) staff       (20)      311 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1017_to_1018/registry/smartweb.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.328343 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1018_to_1019/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.339414 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1018_to_1019/registry/
+-rw-r--r--   0 laurent    (501) staff       (20)      235 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1018_to_1019/registry/smartweb.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.328447 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1019_to_1020/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.339526 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1019_to_1020/registry/
+-rw-r--r--   0 laurent    (501) staff       (20)      235 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1019_to_1020/registry/caching.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.339726 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1020_to_1021/
+-rw-r--r--   0 laurent    (501) staff       (20)     1177 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1020_to_1021/controlpanel.xml
+-rw-r--r--   0 laurent    (501) staff       (20)     1787 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1020_to_1021/rolemap.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.328599 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1021_to_1022/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.339823 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1021_to_1022/registry/
+-rw-r--r--   0 laurent    (501) staff       (20)     3970 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1021_to_1022/registry/caching.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.328698 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1022_to_1023/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.339925 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1022_to_1023/registry/
+-rw-r--r--   0 laurent    (501) staff       (20)     4086 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1022_to_1023/registry/caching.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.328804 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1023_to_1024/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.340023 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1023_to_1024/registry/
+-rw-r--r--   0 laurent    (501) staff       (20)      332 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1023_to_1024/registry/bundles.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.328916 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1026_to_1027/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.340128 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1026_to_1027/registry/
+-rw-r--r--   0 laurent    (501) staff       (20)     8287 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1026_to_1027/registry/autopublishing.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.329031 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1028_to_1029/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.340232 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1028_to_1029/registry/
+-rw-r--r--   0 laurent    (501) staff       (20)      296 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1028_to_1029/registry/messagesviewlet.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.340435 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1029_to_1030/
+-rw-r--r--   0 laurent    (501) staff       (20)      457 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1029_to_1030/controlpanel.xml
+-rw-r--r--   0 laurent    (501) staff       (20)      233 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1029_to_1030/rolemap.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.329222 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1030_to_1031/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.340534 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1030_to_1031/types/
+-rw-r--r--   0 laurent    (501) staff       (20)      358 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1030_to_1031/types/Collection.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.329353 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1031_to_1032/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.340634 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1031_to_1032/types/
+-rw-r--r--   0 laurent    (501) staff       (20)      809 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1031_to_1032/types/Collection.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.329477 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1032_to_1033/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.340754 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1032_to_1033/registry/
+-rw-r--r--   0 laurent    (501) staff       (20)     1307 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1032_to_1033/registry/collective.autoscaling.values.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.340850 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1033_to_1034/
+-rw-r--r--   0 laurent    (501) staff       (20)      304 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1033_to_1034/viewlets.xml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.329673 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1034_to_1035/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.340947 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1034_to_1035/registry/
+-rw-r--r--   0 laurent    (501) staff       (20)      801 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1034_to_1035/registry/caching.xml
+-rw-r--r--   0 laurent    (501) staff       (20)     1586 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/upgrades.py
+-rw-r--r--   0 laurent    (501) staff       (20)     2954 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/utils.py
+-rw-r--r--   0 laurent    (501) staff       (20)     1200 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/viewlets.zcml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2024-05-30 09:19:25.341279 imio_smartweb_policy-1.2.5/src/imio.smartweb.policy.egg-info/
+-rw-r--r--   0 laurent    (501) staff       (20)    12532 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio.smartweb.policy.egg-info/PKG-INFO
+-rw-r--r--   0 laurent    (501) staff       (20)     5675 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio.smartweb.policy.egg-info/SOURCES.txt
+-rw-r--r--   0 laurent    (501) staff       (20)        1 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio.smartweb.policy.egg-info/dependency_links.txt
+-rw-r--r--   0 laurent    (501) staff       (20)       19 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio.smartweb.policy.egg-info/namespace_packages.txt
+-rw-r--r--   0 laurent    (501) staff       (20)        1 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio.smartweb.policy.egg-info/not-zip-safe
+-rw-r--r--   0 laurent    (501) staff       (20)      518 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio.smartweb.policy.egg-info/requires.txt
+-rw-r--r--   0 laurent    (501) staff       (20)        5 2024-05-30 09:19:25.000000 imio_smartweb_policy-1.2.5/src/imio.smartweb.policy.egg-info/top_level.txt
```

### Comparing `imio.smartweb.policy-1.2.4/CHANGES.rst` & `imio_smartweb_policy-1.2.5/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 Changelog
 =========
 
 
+1.2.5 (2024-05-30)
+------------------
+
+- WEB-4107 : Use resourceRegistries ETag in caching configurations
+  [laulaz]
+
+
 1.2.4 (2024-02-02)
 ------------------
 
 - Make content types translatable (with `plone.translatable` behavior) in
   multilingual profile.
   [laulaz]
```

### Comparing `imio.smartweb.policy-1.2.4/DEVELOP.rst` & `imio_smartweb_policy-1.2.5/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/LICENSE.GPL` & `imio_smartweb_policy-1.2.5/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/LICENSE.rst` & `imio_smartweb_policy-1.2.5/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/PKG-INFO` & `imio_smartweb_policy-1.2.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.smartweb.policy
-Version: 1.2.4
+Version: 1.2.5
 Summary: Policies to setup imio.smartweb
 Home-page: https://github.com/imio/imio.smartweb.policy
 Author: Christophe Boulanger
 Author-email: christophe.boulanger@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/imio.smartweb.policy
 Project-URL: Source, https://github.com/imio/imio.smartweb.policy
@@ -17,17 +17,42 @@
 Classifier: Framework :: Plone :: 6.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Requires-Python: >=3.8
-Provides-Extra: test
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
+Requires-Dist: setuptools
+Requires-Dist: z3c.jbot
+Requires-Dist: plone.api>=1.8.4
+Requires-Dist: plone.app.dexterity
+Requires-Dist: plone.app.imagecropping
+Requires-Dist: collective.autopublishing
+Requires-Dist: collective.autoscaling
+Requires-Dist: collective.big.bang
+Requires-Dist: collective.geotransform
+Requires-Dist: collective.js.jqueryui
+Requires-Dist: collective.messagesviewlet
+Requires-Dist: collective.pivot
+Requires-Dist: collective.solr
+Requires-Dist: collective.themefragments
+Requires-Dist: collective.z3cform.select2
+Requires-Dist: eea.facetednavigation
+Requires-Dist: pas.plugins.imio
+Requires-Dist: imio.gdpr
+Requires-Dist: imio.smartweb.core
+Requires-Dist: imio.smartweb.locales
+Requires-Dist: imio.prometheus
+Provides-Extra: test
+Requires-Dist: plone.app.testing; extra == "test"
+Requires-Dist: plone.testing>=5.0.0; extra == "test"
+Requires-Dist: plone.app.contenttypes; extra == "test"
+Requires-Dist: plone.app.robotframework[debug]; extra == "test"
 
 .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
    If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide.html
    This text does not appear on pypi or github. It is a comment.
 
 .. image:: https://github.com/IMIO/imio.smartweb.policy/workflows/Tests/badge.svg
     :target: https://github.com/IMIO/imio.smartweb.policy/actions?query=workflow%3ATests
@@ -120,14 +145,21 @@
 - Christophe Boulanger, christophe.boulanger@imio.be
 
 
 Changelog
 =========
 
 
+1.2.5 (2024-05-30)
+------------------
+
+- WEB-4107 : Use resourceRegistries ETag in caching configurations
+  [laulaz]
+
+
 1.2.4 (2024-02-02)
 ------------------
 
 - Make content types translatable (with `plone.translatable` behavior) in
   multilingual profile.
   [laulaz]
```

### Comparing `imio.smartweb.policy-1.2.4/README.rst` & `imio_smartweb_policy-1.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/docs/conf.py` & `imio_smartweb_policy-1.2.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/setup.cfg` & `imio_smartweb_policy-1.2.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/setup.py` & `imio_smartweb_policy-1.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="imio.smartweb.policy",
-    version="1.2.4",
+    version="1.2.5",
     description="Policies to setup imio.smartweb",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/browser/configure.zcml` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/browser/faceted/configure.zcml` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/browser/faceted/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/browser/faceted/subtyper.py` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/browser/faceted/subtyper.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/caching.py` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/caching.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/caching.zcml` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/caching.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/configure.zcml` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/monkey.py` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/monkey.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/permissions.zcml` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/permissions.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/default/controlpanel.xml` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/default/metadata.xml` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/default/metadata.xml`

 * *Files 10% similar despite different names*

#### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/default/metadata.xml` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/default/metadata.xml`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
 <metadata>
-  <version>1034</version>
+  <version>1035</version>
   <dependencies>
     <dependency>profile-plone.app.contenttypes:plone-content</dependency>
     <dependency>profile-plone.app.caching:default</dependency>
     <dependency>profile-pas.plugins.imio:default</dependency>
     <dependency>profile-collective.autopublishing:default</dependency>
     <dependency>profile-collective.autoscaling:default</dependency>
     <dependency>profile-collective.messagesviewlet:default</dependency>
```

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/default/registry/autopublishing.xml` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/default/registry/autopublishing.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/default/registry/autoscaling.xml` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/default/registry/autoscaling.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/default/registry/caching.xml` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1022_to_1023/registry/caching.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/default/registry/smartweb.xml` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/default/registry/smartweb.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/default/rolemap.xml` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/default/types/Collection.xml` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/default/types/Collection.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/default/types/File.xml` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/default/types/File.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/default/viewlets.xml` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/default/viewlets.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles/multilingual/registry.xml` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/multilingual/registry.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/profiles.zcml` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/setupdemo.py` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/setupdemo.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/setuphandlers.py` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/testing.py` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/testing.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/tests/robot/test_example.robot` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/tests/test_robot.py` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/tests/test_setup.py` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/configure.zcml` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/configure.zcml`

 * *Files 3% similar despite different names*

```diff
@@ -159,14 +159,22 @@
       name="upgrade_1033_to_1034"
       title="Upgrade policy 1033 to 1034"
       directory="profiles/1033_to_1034"
       description="Add Skip to content viewlet in portal top"
       provides="Products.GenericSetup.interfaces.EXTENSION"
     />
 
+  <genericsetup:registerProfile
+      name="upgrade_1034_to_1035"
+      title="Upgrade policy 1034 to 1035"
+      directory="profiles/1034_to_1035"
+      description="Use resourceRegistries ETag in caching configurations"
+      provides="Products.GenericSetup.interfaces.EXTENSION"
+    />
+
   <genericsetup:upgradeStep
       title="Configure first official release"
       description="Install pas.plugins.imio and run needed profiles steps"
       source="1000"
       destination="1001"
       handler=".upgrades.configure_first_official_release"
       profile="imio.smartweb.policy:default"
@@ -527,8 +535,18 @@
       profile="imio.smartweb.policy:default">
     <genericsetup:upgradeDepends
         title="Add Skip to content viewlet in portal top"
         import_profile="imio.smartweb.policy.upgrades:upgrade_1033_to_1034"
         />
   </genericsetup:upgradeSteps>
 
+  <genericsetup:upgradeSteps
+      source="1034"
+      destination="1035"
+      profile="imio.smartweb.policy:default">
+    <genericsetup:upgradeDepends
+        title="Use resourceRegistries ETag in caching configurations"
+        import_profile="imio.smartweb.policy.upgrades:upgrade_1034_to_1035"
+        />
+  </genericsetup:upgradeSteps>
+
 </configure>
```

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1006_to_1007/registry/caching.xml` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1006_to_1007/registry/caching.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1011_to_1012/registry/collective.autoscaling.values.xml` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1011_to_1012/registry/collective.autoscaling.values.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1013_to_1014/registry/collective.autoscaling.values.xml` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1013_to_1014/registry/collective.autoscaling.values.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1014_to_1015/registry/caching.xml` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1014_to_1015/registry/caching.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1020_to_1021/controlpanel.xml` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1020_to_1021/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1020_to_1021/rolemap.xml` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1020_to_1021/rolemap.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1021_to_1022/registry/caching.xml` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1021_to_1022/registry/caching.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1022_to_1023/registry/caching.xml` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/default/registry/caching.xml`

 * *Files 6% similar despite different names*

#### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1022_to_1023/registry/caching.xml` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/profiles/default/registry/caching.xml`

```diff
@@ -30,14 +30,15 @@
     <value>False</value>
   </record>
   <record name="plone.app.caching.moderateCaching.etags">
     <value>
       <element>lastModified</element>
       <element>userid</element>
       <element>roles</element>
+      <element>resourceRegistries</element>
     </value>
   </record>
   <record name="plone.app.caching.moderateCaching.lastModified">
     <value>True</value>
   </record>
   <record name="plone.app.caching.moderateCaching.ramCache">
     <value>False</value>
@@ -52,14 +53,15 @@
     <value>False</value>
   </record>
   <record name="plone.app.caching.terseCaching.etags">
     <value>
       <element>lastModified</element>
       <element>userid</element>
       <element>roles</element>
+      <element>resourceRegistries</element>
     </value>
   </record>
   <record name="plone.app.caching.terseCaching.lastModified">
     <value>True</value>
   </record>
   <record name="plone.app.caching.terseCaching.maxage">
     <value>0</value>
@@ -98,14 +100,15 @@
     <value>False</value>
   </record>
   <record name="plone.app.caching.weakCaching.etags">
     <value>
       <element>lastModified</element>
       <element>userid</element>
       <element>roles</element>
+      <element>resourceRegistries</element>
     </value>
   </record>
   <record name="plone.app.caching.weakCaching.lastModified">
     <value>True</value>
   </record>
   <record name="plone.app.caching.weakCaching.ramCache">
     <value>False</value>
```

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1026_to_1027/registry/autopublishing.xml` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1026_to_1027/registry/autopublishing.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1031_to_1032/types/Collection.xml` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1031_to_1032/types/Collection.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/profiles/1032_to_1033/registry/collective.autoscaling.values.xml` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/profiles/1032_to_1033/registry/collective.autoscaling.values.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/upgrades/upgrades.py` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/upgrades/upgrades.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/utils.py` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/utils.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/src/imio/smartweb/policy/viewlets.zcml` & `imio_smartweb_policy-1.2.5/src/imio/smartweb/policy/viewlets.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.2.4/src/imio.smartweb.policy.egg-info/PKG-INFO` & `imio_smartweb_policy-1.2.5/src/imio.smartweb.policy.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.smartweb.policy
-Version: 1.2.4
+Version: 1.2.5
 Summary: Policies to setup imio.smartweb
 Home-page: https://github.com/imio/imio.smartweb.policy
 Author: Christophe Boulanger
 Author-email: christophe.boulanger@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/imio.smartweb.policy
 Project-URL: Source, https://github.com/imio/imio.smartweb.policy
@@ -17,17 +17,42 @@
 Classifier: Framework :: Plone :: 6.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Requires-Python: >=3.8
-Provides-Extra: test
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
+Requires-Dist: setuptools
+Requires-Dist: z3c.jbot
+Requires-Dist: plone.api>=1.8.4
+Requires-Dist: plone.app.dexterity
+Requires-Dist: plone.app.imagecropping
+Requires-Dist: collective.autopublishing
+Requires-Dist: collective.autoscaling
+Requires-Dist: collective.big.bang
+Requires-Dist: collective.geotransform
+Requires-Dist: collective.js.jqueryui
+Requires-Dist: collective.messagesviewlet
+Requires-Dist: collective.pivot
+Requires-Dist: collective.solr
+Requires-Dist: collective.themefragments
+Requires-Dist: collective.z3cform.select2
+Requires-Dist: eea.facetednavigation
+Requires-Dist: pas.plugins.imio
+Requires-Dist: imio.gdpr
+Requires-Dist: imio.smartweb.core
+Requires-Dist: imio.smartweb.locales
+Requires-Dist: imio.prometheus
+Provides-Extra: test
+Requires-Dist: plone.app.testing; extra == "test"
+Requires-Dist: plone.testing>=5.0.0; extra == "test"
+Requires-Dist: plone.app.contenttypes; extra == "test"
+Requires-Dist: plone.app.robotframework[debug]; extra == "test"
 
 .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
    If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide.html
    This text does not appear on pypi or github. It is a comment.
 
 .. image:: https://github.com/IMIO/imio.smartweb.policy/workflows/Tests/badge.svg
     :target: https://github.com/IMIO/imio.smartweb.policy/actions?query=workflow%3ATests
@@ -120,14 +145,21 @@
 - Christophe Boulanger, christophe.boulanger@imio.be
 
 
 Changelog
 =========
 
 
+1.2.5 (2024-05-30)
+------------------
+
+- WEB-4107 : Use resourceRegistries ETag in caching configurations
+  [laulaz]
+
+
 1.2.4 (2024-02-02)
 ------------------
 
 - Make content types translatable (with `plone.translatable` behavior) in
   multilingual profile.
   [laulaz]
```

### Comparing `imio.smartweb.policy-1.2.4/src/imio.smartweb.policy.egg-info/SOURCES.txt` & `imio_smartweb_policy-1.2.5/src/imio.smartweb.policy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -95,8 +95,9 @@
 src/imio/smartweb/policy/upgrades/profiles/1026_to_1027/registry/autopublishing.xml
 src/imio/smartweb/policy/upgrades/profiles/1028_to_1029/registry/messagesviewlet.xml
 src/imio/smartweb/policy/upgrades/profiles/1029_to_1030/controlpanel.xml
 src/imio/smartweb/policy/upgrades/profiles/1029_to_1030/rolemap.xml
 src/imio/smartweb/policy/upgrades/profiles/1030_to_1031/types/Collection.xml
 src/imio/smartweb/policy/upgrades/profiles/1031_to_1032/types/Collection.xml
 src/imio/smartweb/policy/upgrades/profiles/1032_to_1033/registry/collective.autoscaling.values.xml
-src/imio/smartweb/policy/upgrades/profiles/1033_to_1034/viewlets.xml
+src/imio/smartweb/policy/upgrades/profiles/1033_to_1034/viewlets.xml
+src/imio/smartweb/policy/upgrades/profiles/1034_to_1035/registry/caching.xml
```

### Comparing `imio.smartweb.policy-1.2.4/src/imio.smartweb.policy.egg-info/requires.txt` & `imio_smartweb_policy-1.2.5/src/imio.smartweb.policy.egg-info/requires.txt`

 * *Files identical despite different names*

