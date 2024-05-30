# Comparing `tmp/plone.app.dexterity-3.2.0.tar.gz` & `tmp/plone_app_dexterity-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.dexterity-3.2.0.tar", last modified: Fri Nov  3 22:34:10 2023, max compression
+gzip compressed data, was "plone_app_dexterity-4.0.0.tar", last modified: Thu May 30 18:27:12 2024, max compression
```

## Comparing `plone.app.dexterity-3.2.0.tar` & `plone_app_dexterity-4.0.0.tar`

### file list

```diff
@@ -1,195 +1,195 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-11-03 22:34:10.637560 plone.app.dexterity-3.2.0/
--rw-r--r--   0 maurits    (501) staff       (20)    32974 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      149 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    46989 2023-11-03 22:34:10.636921 plone.app.dexterity-3.2.0/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     6519 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)     4640 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/RELEASE_NOTES.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-11-03 22:34:10.564865 plone.app.dexterity-3.2.0/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    12282 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      760 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)     3310 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/Makefile
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-11-03 22:34:10.572354 plone.app.dexterity-3.2.0/docs/advanced/
--rw-r--r--   0 maurits    (501) staff       (20)     1950 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/advanced/behaviours.rst
--rw-r--r--   0 maurits    (501) staff       (20)    14910 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/advanced/catalog-indexing-strategies.rst
--rw-r--r--   0 maurits    (501) staff       (20)     9634 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/advanced/custom-add-and-edit-forms.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3181 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/advanced/custom-content-classes.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2145 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/advanced/defaults.rst
--rw-r--r--   0 maurits    (501) staff       (20)     5191 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/advanced/event-handlers.rst
--rw-r--r--   0 maurits    (501) staff       (20)     4599 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/advanced/files-and-images.rst
--rw-r--r--   0 maurits    (501) staff       (20)      492 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/advanced/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)     6971 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/advanced/permissions.rst
--rw-r--r--   0 maurits    (501) staff       (20)     7156 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/advanced/references.rst
--rw-r--r--   0 maurits    (501) staff       (20)     7451 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/advanced/rich-text-markup-transformations.rst
--rw-r--r--   0 maurits    (501) staff       (20)     5276 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/advanced/static-resources.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3814 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/advanced/validators.rst
--rw-r--r--   0 maurits    (501) staff       (20)    13225 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/advanced/vocabularies.rst
--rw-r--r--   0 maurits    (501) staff       (20)    21829 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/advanced/webdav-and-other-file-representations.rst
--rw-r--r--   0 maurits    (501) staff       (20)    16315 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/advanced/workflow.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-11-03 22:34:10.575613 plone.app.dexterity-3.2.0/docs/behaviors/
--rw-r--r--   0 maurits    (501) staff       (20)     1931 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/behaviors/behavior-basics.rst
--rw-r--r--   0 maurits    (501) staff       (20)     5438 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/behaviors/creating-and-registering-behaviors.rst
--rw-r--r--   0 maurits    (501) staff       (20)      277 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/behaviors/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2080 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/behaviors/intro.rst
--rw-r--r--   0 maurits    (501) staff       (20)    10189 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/behaviors/providing-marker-interfaces.rst
--rw-r--r--   0 maurits    (501) staff       (20)     5855 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/behaviors/schema-only-behaviors.rst
--rw-r--r--   0 maurits    (501) staff       (20)    11007 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/behaviors/testing-behaviors.rst
--rw-r--r--   0 maurits    (501) staff       (20)     7095 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/conf.py
--rw-r--r--   0 maurits    (501) staff       (20)    10738 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/custom-views.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2354 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/designing.rst
--rw-r--r--   0 maurits    (501) staff       (20)      460 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)      943 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/install.rst
--rw-r--r--   0 maurits    (501) staff       (20)     5689 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/intro.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3973 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/model-driven-types.rst
--rw-r--r--   0 maurits    (501) staff       (20)     6303 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/prerequisite.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-11-03 22:34:10.579408 plone.app.dexterity-3.2.0/docs/reference/
--rw-r--r--   0 maurits    (501) staff       (20)     9806 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/reference/dexterity-xml.rst
--rw-r--r--   0 maurits    (501) staff       (20)    14982 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/reference/fields.rst
--rw-r--r--   0 maurits    (501) staff       (20)     8261 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/reference/form-schema-hints.rst
--rw-r--r--   0 maurits    (501) staff       (20)      270 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/reference/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)    35076 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/reference/manipulating-content-objects.rst
--rw-r--r--   0 maurits    (501) staff       (20)      871 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/reference/misc.rst
--rw-r--r--   0 maurits    (501) staff       (20)     6133 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/reference/standard-behaviours.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3419 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/reference/widgets.rst
--rw-r--r--   0 maurits    (501) staff       (20)    16976 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/schema-driven-types.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-11-03 22:34:10.581248 plone.app.dexterity-3.2.0/docs/testing/
--rw-r--r--   0 maurits    (501) staff       (20)      186 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/testing/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)    14391 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/testing/integration-tests.rst
--rw-r--r--   0 maurits    (501) staff       (20)    10941 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/testing/mock-testing.rst
--rw-r--r--   0 maurits    (501) staff       (20)     5860 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/docs/testing/unit-tests.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-11-03 22:34:10.581719 plone.app.dexterity-3.2.0/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-11-03 22:34:10.585991 plone.app.dexterity-3.2.0/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-11-03 22:34:10.590968 plone.app.dexterity-3.2.0/plone/app/dexterity/
--rw-r--r--   0 maurits    (501) staff       (20)      672 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/TODO.txt
--rw-r--r--   0 maurits    (501) staff       (20)       76 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-11-03 22:34:10.595472 plone.app.dexterity-3.2.0/plone/app/dexterity/behaviors/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/behaviors/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     5584 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/behaviors/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     6908 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/behaviors/constrains.py
--rw-r--r--   0 maurits    (501) staff       (20)     1102 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/behaviors/discussion.py
--rw-r--r--   0 maurits    (501) staff       (20)     1759 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/behaviors/exclfromnav.py
--rw-r--r--   0 maurits    (501) staff       (20)      963 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/behaviors/filename.py
--rw-r--r--   0 maurits    (501) staff       (20)     1808 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/behaviors/id.py
--rw-r--r--   0 maurits    (501) staff       (20)    12317 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/behaviors/metadata.py
--rw-r--r--   0 maurits    (501) staff       (20)     5255 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/behaviors/nextprevious.py
--rw-r--r--   0 maurits    (501) staff       (20)      441 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/behaviors/related.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-11-03 22:34:10.597224 plone.app.dexterity-3.2.0/plone/app/dexterity/behaviors/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/behaviors/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2827 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/behaviors/tests/test_contrains.py
--rw-r--r--   0 maurits    (501) staff       (20)     5128 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/behaviors/tests/test_id.py
--rw-r--r--   0 maurits    (501) staff       (20)     4370 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/behaviors/tests/test_metadata.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-11-03 22:34:10.608691 plone.app.dexterity-3.2.0/plone/app/dexterity/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1751 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/browser/add_type.py
--rw-r--r--   0 maurits    (501) staff       (20)     2884 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/browser/behaviors.pt
--rw-r--r--   0 maurits    (501) staff       (20)     5024 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/browser/behaviors.py
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/browser/blank.css
--rw-r--r--   0 maurits    (501) staff       (20)     1223 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/browser/clone_type.py
--rw-r--r--   0 maurits    (501) staff       (20)     3833 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1740 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/browser/container.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4539 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/browser/export.py
--rw-r--r--   0 maurits    (501) staff       (20)     1185 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/browser/fields.py
--rw-r--r--   0 maurits    (501) staff       (20)     6792 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/browser/folder_listing.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3408 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/browser/folder_listing.py
--rw-r--r--   0 maurits    (501) staff       (20)     6391 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/browser/import_types.py
--rw-r--r--   0 maurits    (501) staff       (20)     1307 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/browser/item.pt
--rw-r--r--   0 maurits    (501) staff       (20)      429 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/browser/layout.py
--rw-r--r--   0 maurits    (501) staff       (20)     2493 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/browser/modeleditor.pt
--rw-r--r--   0 maurits    (501) staff       (20)     5644 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/browser/modeleditor.py
--rw-r--r--   0 maurits    (501) staff       (20)     2264 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/browser/overview.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1177 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/browser/overview.py
--rw-r--r--   0 maurits    (501) staff       (20)     1297 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/browser/tabbed_forms.pt
--rw-r--r--   0 maurits    (501) staff       (20)    10142 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/browser/types.py
--rw-r--r--   0 maurits    (501) staff       (20)     1098 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/browser/types_listing.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1350 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/browser/types_listing_row.pt
--rw-r--r--   0 maurits    (501) staff       (20)      710 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/browser/typesformwrapper.pt
--rw-r--r--   0 maurits    (501) staff       (20)      249 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/browser/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     2770 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      547 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/events.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2219 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/factories.py
--rw-r--r--   0 maurits    (501) staff       (20)     3667 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      482 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/meta.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      271 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/overrides.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     4664 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/permissions.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-11-03 22:34:10.554380 plone.app.dexterity-3.2.0/plone/app/dexterity/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-11-03 22:34:10.609639 plone.app.dexterity-3.2.0/plone/app/dexterity/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      591 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/profiles/default/controlpanel.xml
--rw-r--r--   0 maurits    (501) staff       (20)      186 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/profiles/default/metadata.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-11-03 22:34:10.610568 plone.app.dexterity-3.2.0/plone/app/dexterity/profiles/testing/
--rw-r--r--   0 maurits    (501) staff       (20)      248 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/profiles/testing/metadata.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-11-03 22:34:10.611483 plone.app.dexterity-3.2.0/plone/app/dexterity/profiles/testing/types/
--rw-r--r--   0 maurits    (501) staff       (20)     2214 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/profiles/testing/types/Document.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2467 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/profiles/testing/types/Folder.xml
--rw-r--r--   0 maurits    (501) staff       (20)      356 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/profiles/testing/types.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1661 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/serialize.py
--rw-r--r--   0 maurits    (501) staff       (20)     1074 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-11-03 22:34:10.618357 plone.app.dexterity-3.2.0/plone/app/dexterity/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3656 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/tests/discussion.txt
--rw-r--r--   0 maurits    (501) staff       (20)    22722 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/tests/editing.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1851 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/tests/filename.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-11-03 22:34:10.618813 plone.app.dexterity-3.2.0/plone/app/dexterity/tests/import/
--rw-r--r--   0 maurits    (501) staff       (20)     5804 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/tests/import/dexterity_export.zip
--rw-r--r--   0 maurits    (501) staff       (20)     2498 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/tests/metadata.txt
--rw-r--r--   0 maurits    (501) staff       (20)     3592 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/tests/nextprevious.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-11-03 22:34:10.619272 plone.app.dexterity-3.2.0/plone/app/dexterity/tests/robot/
--rw-r--r--   0 maurits    (501) staff       (20)     1082 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/tests/robot/test_types.robot
--rw-r--r--   0 maurits    (501) staff       (20)     1458 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/tests/schema_events.txt
--rw-r--r--   0 maurits    (501) staff       (20)    18456 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/tests/test_constrains.py
--rw-r--r--   0 maurits    (501) staff       (20)      753 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/tests/test_doctests.py
--rw-r--r--   0 maurits    (501) staff       (20)     1857 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/tests/test_export.py
--rw-r--r--   0 maurits    (501) staff       (20)     2851 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/tests/test_import.py
--rw-r--r--   0 maurits    (501) staff       (20)     2952 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/tests/test_namefromtitle.py
--rw-r--r--   0 maurits    (501) staff       (20)     8186 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/tests/test_nextprevious.py
--rw-r--r--   0 maurits    (501) staff       (20)      826 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/tests/test_robot.py
--rw-r--r--   0 maurits    (501) staff       (20)     1586 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/tests/test_upgrades.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-11-03 22:34:10.624291 plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/
--rw-r--r--   0 maurits    (501) staff       (20)      555 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      293 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/behavior.py
--rw-r--r--   0 maurits    (501) staff       (20)     2066 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     5051 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/converters.py
--rw-r--r--   0 maurits    (501) staff       (20)      890 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/directives.py
--rw-r--r--   0 maurits    (501) staff       (20)     5290 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/indexer.py
--rw-r--r--   0 maurits    (501) staff       (20)     1046 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     2339 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/schemaeditor.py
--rw-r--r--   0 maurits    (501) staff       (20)     1340 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/supermodel.py
--rw-r--r--   0 maurits    (501) staff       (20)     2662 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-11-03 22:34:10.629866 plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/tests/
--rw-r--r--   0 maurits    (501) staff       (20)       80 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3249 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/tests/behaviors.py
--rw-r--r--   0 maurits    (501) staff       (20)    11423 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/tests/behaviors.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2524 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/tests/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    21311 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/tests/file.pdf
--rw-r--r--   0 maurits    (501) staff       (20)      376 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/tests/helpers.py
--rw-r--r--   0 maurits    (501) staff       (20)      434 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/tests/test_basic_behavior.py
--rw-r--r--   0 maurits    (501) staff       (20)      792 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/tests/test_behaviors.py
--rw-r--r--   0 maurits    (501) staff       (20)     1610 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/tests/test_directives.py
--rw-r--r--   0 maurits    (501) staff       (20)     3656 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/tests/test_schemaeditor.py
--rw-r--r--   0 maurits    (501) staff       (20)     3767 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/tests/test_supermodel_handler.py
--rw-r--r--   0 maurits    (501) staff       (20)     1793 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/tests/test_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     1170 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/utils.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-11-03 22:34:10.634353 plone.app.dexterity-3.2.0/plone/app/dexterity/upgrades/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/upgrades/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2416 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/upgrades/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      249 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/upgrades/to1.py
--rw-r--r--   0 maurits    (501) staff       (20)      195 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/upgrades/to2.py
--rw-r--r--   0 maurits    (501) staff       (20)      221 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/upgrades/to2000.py
--rw-r--r--   0 maurits    (501) staff       (20)      631 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/upgrades/to2001.py
--rw-r--r--   0 maurits    (501) staff       (20)      268 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/upgrades/to2002.py
--rw-r--r--   0 maurits    (501) staff       (20)      606 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/upgrades/to2003.py
--rw-r--r--   0 maurits    (501) staff       (20)      976 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/upgrades/to2004.py
--rw-r--r--   0 maurits    (501) staff       (20)     1444 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/plone/app/dexterity/upgrades/to2005.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-11-03 22:34:10.585521 plone.app.dexterity-3.2.0/plone.app.dexterity.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    46989 2023-11-03 22:34:10.000000 plone.app.dexterity-3.2.0/plone.app.dexterity.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     6528 2023-11-03 22:34:10.000000 plone.app.dexterity-3.2.0/plone.app.dexterity.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-11-03 22:34:10.000000 plone.app.dexterity-3.2.0/plone.app.dexterity.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2023-11-03 22:34:10.000000 plone.app.dexterity-3.2.0/plone.app.dexterity.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2023-11-03 22:34:10.000000 plone.app.dexterity-3.2.0/plone.app.dexterity.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-11-03 22:34:10.000000 plone.app.dexterity-3.2.0/plone.app.dexterity.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      804 2023-11-03 22:34:10.000000 plone.app.dexterity-3.2.0/plone.app.dexterity.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-11-03 22:34:10.000000 plone.app.dexterity-3.2.0/plone.app.dexterity.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4020 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)       38 2023-11-03 22:34:10.637676 plone.app.dexterity-3.2.0/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     3326 2023-11-03 22:34:09.000000 plone.app.dexterity-3.2.0/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:27:12.445595 plone_app_dexterity-4.0.0/
+-rw-r--r--   0 maurits    (501) staff       (20)    33187 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      149 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    47184 2024-05-30 18:27:12.444831 plone_app_dexterity-4.0.0/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     6519 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     4640 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/RELEASE_NOTES.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:27:12.341064 plone_app_dexterity-4.0.0/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    12282 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      760 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/LICENSE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     3310 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/Makefile
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:27:12.349292 plone_app_dexterity-4.0.0/docs/advanced/
+-rw-r--r--   0 maurits    (501) staff       (20)     1950 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/advanced/behaviours.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    14910 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/advanced/catalog-indexing-strategies.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     9634 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/advanced/custom-add-and-edit-forms.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3181 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/advanced/custom-content-classes.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2145 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/advanced/defaults.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     5191 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/advanced/event-handlers.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     4599 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/advanced/files-and-images.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      492 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/advanced/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     6971 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/advanced/permissions.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     7156 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/advanced/references.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     7451 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/advanced/rich-text-markup-transformations.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     5276 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/advanced/static-resources.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3814 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/advanced/validators.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    13225 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/advanced/vocabularies.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    21829 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/advanced/webdav-and-other-file-representations.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    16315 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/advanced/workflow.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:27:12.352723 plone_app_dexterity-4.0.0/docs/behaviors/
+-rw-r--r--   0 maurits    (501) staff       (20)     1931 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/behaviors/behavior-basics.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     5438 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/behaviors/creating-and-registering-behaviors.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      277 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/behaviors/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2080 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/behaviors/intro.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    10189 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/behaviors/providing-marker-interfaces.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     5855 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/behaviors/schema-only-behaviors.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    11007 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/behaviors/testing-behaviors.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     7095 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/conf.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10738 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/custom-views.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2354 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/designing.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      460 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      943 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/install.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     5689 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/intro.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3973 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/model-driven-types.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     6303 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/prerequisite.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:27:12.356583 plone_app_dexterity-4.0.0/docs/reference/
+-rw-r--r--   0 maurits    (501) staff       (20)     9806 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/reference/dexterity-xml.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    14982 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/reference/fields.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     8261 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/reference/form-schema-hints.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      270 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/reference/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    35076 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/reference/manipulating-content-objects.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      871 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/reference/misc.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     6133 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/reference/standard-behaviours.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3419 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/reference/widgets.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    16976 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/schema-driven-types.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:27:12.358528 plone_app_dexterity-4.0.0/docs/testing/
+-rw-r--r--   0 maurits    (501) staff       (20)      186 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/testing/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    14391 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/testing/integration-tests.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    10941 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/testing/mock-testing.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     5860 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/docs/testing/unit-tests.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:27:12.359033 plone_app_dexterity-4.0.0/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:27:12.363290 plone_app_dexterity-4.0.0/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:27:12.394589 plone_app_dexterity-4.0.0/plone/app/dexterity/
+-rw-r--r--   0 maurits    (501) staff       (20)      672 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/TODO.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       76 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:27:12.399474 plone_app_dexterity-4.0.0/plone/app/dexterity/behaviors/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/behaviors/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5584 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/behaviors/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     6908 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/behaviors/constrains.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1102 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/behaviors/discussion.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1759 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/behaviors/exclfromnav.py
+-rw-r--r--   0 maurits    (501) staff       (20)      963 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/behaviors/filename.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1808 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/behaviors/id.py
+-rw-r--r--   0 maurits    (501) staff       (20)    12345 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/behaviors/metadata.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5255 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/behaviors/nextprevious.py
+-rw-r--r--   0 maurits    (501) staff       (20)      442 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/behaviors/related.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:27:12.401294 plone_app_dexterity-4.0.0/plone/app/dexterity/behaviors/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/behaviors/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2827 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/behaviors/tests/test_contrains.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5128 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/behaviors/tests/test_id.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4370 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/behaviors/tests/test_metadata.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:27:12.413161 plone_app_dexterity-4.0.0/plone/app/dexterity/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1751 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/browser/add_type.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2884 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/browser/behaviors.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     5024 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/browser/behaviors.py
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/browser/blank.css
+-rw-r--r--   0 maurits    (501) staff       (20)     1223 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/browser/clone_type.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3833 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1740 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/browser/container.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4539 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/browser/export.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1185 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/browser/fields.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6792 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/browser/folder_listing.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3408 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/browser/folder_listing.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6392 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/browser/import_types.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1307 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/browser/item.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      429 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/browser/layout.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2493 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/browser/modeleditor.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     5644 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/browser/modeleditor.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2264 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/browser/overview.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1177 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/browser/overview.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1297 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/browser/tabbed_forms.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    10142 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/browser/types.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1098 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/browser/types_listing.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1350 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/browser/types_listing_row.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      710 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/browser/typesformwrapper.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      249 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/browser/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2770 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      547 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/events.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2219 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/factories.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3667 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      482 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/meta.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      271 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/overrides.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     4664 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/permissions.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:27:12.329916 plone_app_dexterity-4.0.0/plone/app/dexterity/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:27:12.414099 plone_app_dexterity-4.0.0/plone/app/dexterity/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      591 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/profiles/default/controlpanel.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      186 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/profiles/default/metadata.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:27:12.415043 plone_app_dexterity-4.0.0/plone/app/dexterity/profiles/testing/
+-rw-r--r--   0 maurits    (501) staff       (20)      248 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/profiles/testing/metadata.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:27:12.415968 plone_app_dexterity-4.0.0/plone/app/dexterity/profiles/testing/types/
+-rw-r--r--   0 maurits    (501) staff       (20)     2214 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/profiles/testing/types/Document.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2467 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/profiles/testing/types/Folder.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      356 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/profiles/testing/types.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1661 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/serialize.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1074 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:27:12.423047 plone_app_dexterity-4.0.0/plone/app/dexterity/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3656 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/tests/discussion.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    22722 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/tests/editing.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1851 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/tests/filename.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:27:12.423527 plone_app_dexterity-4.0.0/plone/app/dexterity/tests/import/
+-rw-r--r--   0 maurits    (501) staff       (20)     5804 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/tests/import/dexterity_export.zip
+-rw-r--r--   0 maurits    (501) staff       (20)     2498 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/tests/metadata.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     3592 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/tests/nextprevious.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:27:12.424038 plone_app_dexterity-4.0.0/plone/app/dexterity/tests/robot/
+-rw-r--r--   0 maurits    (501) staff       (20)     1082 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/tests/robot/test_types.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     1458 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/tests/schema_events.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    18456 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/tests/test_constrains.py
+-rw-r--r--   0 maurits    (501) staff       (20)      753 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/tests/test_doctests.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1858 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/tests/test_export.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2852 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/tests/test_import.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2952 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/tests/test_namefromtitle.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8186 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/tests/test_nextprevious.py
+-rw-r--r--   0 maurits    (501) staff       (20)      826 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/tests/test_robot.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1586 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/tests/test_upgrades.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:27:12.429292 plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/
+-rw-r--r--   0 maurits    (501) staff       (20)      555 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      294 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/behavior.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2066 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     5051 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/converters.py
+-rw-r--r--   0 maurits    (501) staff       (20)      890 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/directives.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5290 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/indexer.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1046 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2339 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/schemaeditor.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1340 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/supermodel.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2662 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:27:12.435219 plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)       80 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3250 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/tests/behaviors.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11423 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/tests/behaviors.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2524 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/tests/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    21311 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/tests/file.pdf
+-rw-r--r--   0 maurits    (501) staff       (20)      376 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/tests/helpers.py
+-rw-r--r--   0 maurits    (501) staff       (20)      434 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/tests/test_basic_behavior.py
+-rw-r--r--   0 maurits    (501) staff       (20)      792 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/tests/test_behaviors.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1610 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/tests/test_directives.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3656 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/tests/test_schemaeditor.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3767 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/tests/test_supermodel_handler.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1793 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/tests/test_utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1170 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/utils.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:27:12.439777 plone_app_dexterity-4.0.0/plone/app/dexterity/upgrades/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/upgrades/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2416 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/upgrades/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      249 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/upgrades/to1.py
+-rw-r--r--   0 maurits    (501) staff       (20)      195 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/upgrades/to2.py
+-rw-r--r--   0 maurits    (501) staff       (20)      221 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/upgrades/to2000.py
+-rw-r--r--   0 maurits    (501) staff       (20)      631 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/upgrades/to2001.py
+-rw-r--r--   0 maurits    (501) staff       (20)      268 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/upgrades/to2002.py
+-rw-r--r--   0 maurits    (501) staff       (20)      606 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/upgrades/to2003.py
+-rw-r--r--   0 maurits    (501) staff       (20)      976 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/upgrades/to2004.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1444 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/plone/app/dexterity/upgrades/to2005.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:27:12.440404 plone_app_dexterity-4.0.0/plone.app.dexterity.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    47184 2024-05-30 18:27:12.000000 plone_app_dexterity-4.0.0/plone.app.dexterity.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     6528 2024-05-30 18:27:12.000000 plone_app_dexterity-4.0.0/plone.app.dexterity.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-05-30 18:27:12.000000 plone_app_dexterity-4.0.0/plone.app.dexterity.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2024-05-30 18:27:12.000000 plone_app_dexterity-4.0.0/plone.app.dexterity.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2024-05-30 18:27:12.000000 plone_app_dexterity-4.0.0/plone.app.dexterity.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-05-30 18:27:12.000000 plone_app_dexterity-4.0.0/plone.app.dexterity.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      819 2024-05-30 18:27:12.000000 plone_app_dexterity-4.0.0/plone.app.dexterity.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-05-30 18:27:12.000000 plone_app_dexterity-4.0.0/plone.app.dexterity.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4576 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2024-05-30 18:27:12.445727 plone_app_dexterity-4.0.0/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     3304 2024-05-30 18:27:11.000000 plone_app_dexterity-4.0.0/setup.py
```

### Comparing `plone.app.dexterity-3.2.0/CHANGES.rst` & `plone_app_dexterity-4.0.0/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,30 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.0 (2024-05-30)
+------------------
+
+Bug fixes:
+
+
+- Remove a DeprecationWarning from a moved p.a.z3cform.widgets import. [@jensens] (#387)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (6e36bcc4)
+
+
 3.2.0 (2023-11-03)
 ------------------
 
 Internal:
 
 
 - Make the dependency on ``plone.app.content`` conditional.
```

### Comparing `plone.app.dexterity-3.2.0/PKG-INFO` & `plone_app_dexterity-4.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: plone.app.dexterity
-Version: 3.2.0
+Version: 4.0.0
 Summary: Dexterity is a content type framework for CMF  applications, with particular emphasis on Plone. It can be viewed as an alternative to Archetypes that is more light-weight and modular.
 Home-page: http://plone.org/products/dexterity
 Author: Martin Aspeli, David Glick, et al
 Author-email: dexterity-development@googlegroups.com
 License: GPL
 Keywords: plone ttw dexterity schema interface
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
-Classifier: Framework :: Plone :: 6.0
+Classifier: Framework :: Plone :: 6.1
 Classifier: Framework :: Plone :: Core
 Classifier: Framework :: Zope :: 5
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 Requires-Dist: plone.app.textfield
 Requires-Dist: plone.behavior>=1.0
 Requires-Dist: plone.dexterity>=2.2.2
 Requires-Dist: plone.formwidget.namedfile
 Requires-Dist: plone.namedfile>=1.0.0
 Requires-Dist: plone.rfc822
 Requires-Dist: plone.schemaeditor>1.3.3
 Requires-Dist: lxml
 Requires-Dist: plone.base
 Requires-Dist: plone.app.uuid
-Requires-Dist: plone.app.z3cform>=1.1.0
+Requires-Dist: plone.app.z3cform>=4.6.0
 Requires-Dist: plone.autoform>=1.1
 Requires-Dist: plone.contentrules
+Requires-Dist: plone.portlets
 Requires-Dist: plone.schema>=1.1.0
 Requires-Dist: plone.supermodel>=1.1
 Requires-Dist: plone.z3cform>=0.6.0
 Requires-Dist: Products.GenericSetup
 Requires-Dist: setuptools
 Requires-Dist: Zope
 Requires-Dist: zope.browserpage
@@ -371,14 +371,30 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.0 (2024-05-30)
+------------------
+
+Bug fixes:
+
+
+- Remove a DeprecationWarning from a moved p.a.z3cform.widgets import. [@jensens] (#387)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (6e36bcc4)
+
+
 3.2.0 (2023-11-03)
 ------------------
 
 Internal:
 
 
 - Make the dependency on ``plone.app.content`` conditional.
```

### Comparing `plone.app.dexterity-3.2.0/README.rst` & `plone_app_dexterity-4.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/RELEASE_NOTES.rst` & `plone_app_dexterity-4.0.0/RELEASE_NOTES.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/LICENSE.GPL` & `plone_app_dexterity-4.0.0/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/LICENSE.txt` & `plone_app_dexterity-4.0.0/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/Makefile` & `plone_app_dexterity-4.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/advanced/behaviours.rst` & `plone_app_dexterity-4.0.0/docs/advanced/behaviours.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/advanced/catalog-indexing-strategies.rst` & `plone_app_dexterity-4.0.0/docs/advanced/catalog-indexing-strategies.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/advanced/custom-add-and-edit-forms.rst` & `plone_app_dexterity-4.0.0/docs/advanced/custom-add-and-edit-forms.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/advanced/custom-content-classes.rst` & `plone_app_dexterity-4.0.0/docs/advanced/custom-content-classes.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/advanced/defaults.rst` & `plone_app_dexterity-4.0.0/docs/advanced/defaults.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/advanced/event-handlers.rst` & `plone_app_dexterity-4.0.0/docs/advanced/event-handlers.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/advanced/files-and-images.rst` & `plone_app_dexterity-4.0.0/docs/advanced/files-and-images.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/advanced/permissions.rst` & `plone_app_dexterity-4.0.0/docs/advanced/permissions.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/advanced/references.rst` & `plone_app_dexterity-4.0.0/docs/advanced/references.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/advanced/rich-text-markup-transformations.rst` & `plone_app_dexterity-4.0.0/docs/advanced/rich-text-markup-transformations.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/advanced/static-resources.rst` & `plone_app_dexterity-4.0.0/docs/advanced/static-resources.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/advanced/validators.rst` & `plone_app_dexterity-4.0.0/docs/advanced/validators.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/advanced/vocabularies.rst` & `plone_app_dexterity-4.0.0/docs/advanced/vocabularies.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/advanced/webdav-and-other-file-representations.rst` & `plone_app_dexterity-4.0.0/docs/advanced/webdav-and-other-file-representations.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/advanced/workflow.rst` & `plone_app_dexterity-4.0.0/docs/advanced/workflow.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/behaviors/behavior-basics.rst` & `plone_app_dexterity-4.0.0/docs/behaviors/behavior-basics.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/behaviors/creating-and-registering-behaviors.rst` & `plone_app_dexterity-4.0.0/docs/behaviors/creating-and-registering-behaviors.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/behaviors/intro.rst` & `plone_app_dexterity-4.0.0/docs/behaviors/intro.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/behaviors/providing-marker-interfaces.rst` & `plone_app_dexterity-4.0.0/docs/behaviors/providing-marker-interfaces.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/behaviors/schema-only-behaviors.rst` & `plone_app_dexterity-4.0.0/docs/behaviors/schema-only-behaviors.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/behaviors/testing-behaviors.rst` & `plone_app_dexterity-4.0.0/docs/behaviors/testing-behaviors.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/conf.py` & `plone_app_dexterity-4.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/custom-views.rst` & `plone_app_dexterity-4.0.0/docs/custom-views.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/designing.rst` & `plone_app_dexterity-4.0.0/docs/designing.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/install.rst` & `plone_app_dexterity-4.0.0/docs/install.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/intro.rst` & `plone_app_dexterity-4.0.0/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/model-driven-types.rst` & `plone_app_dexterity-4.0.0/docs/model-driven-types.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/prerequisite.rst` & `plone_app_dexterity-4.0.0/docs/prerequisite.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/reference/dexterity-xml.rst` & `plone_app_dexterity-4.0.0/docs/reference/dexterity-xml.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/reference/fields.rst` & `plone_app_dexterity-4.0.0/docs/reference/fields.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/reference/form-schema-hints.rst` & `plone_app_dexterity-4.0.0/docs/reference/form-schema-hints.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/reference/manipulating-content-objects.rst` & `plone_app_dexterity-4.0.0/docs/reference/manipulating-content-objects.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/reference/misc.rst` & `plone_app_dexterity-4.0.0/docs/reference/misc.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/reference/standard-behaviours.rst` & `plone_app_dexterity-4.0.0/docs/reference/standard-behaviours.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/reference/widgets.rst` & `plone_app_dexterity-4.0.0/docs/reference/widgets.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/schema-driven-types.rst` & `plone_app_dexterity-4.0.0/docs/schema-driven-types.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/testing/integration-tests.rst` & `plone_app_dexterity-4.0.0/docs/testing/integration-tests.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/testing/mock-testing.rst` & `plone_app_dexterity-4.0.0/docs/testing/mock-testing.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/docs/testing/unit-tests.rst` & `plone_app_dexterity-4.0.0/docs/testing/unit-tests.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/TODO.txt` & `plone_app_dexterity-4.0.0/plone/app/dexterity/TODO.txt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/behaviors/configure.zcml` & `plone_app_dexterity-4.0.0/plone/app/dexterity/behaviors/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/behaviors/constrains.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/behaviors/constrains.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/behaviors/discussion.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/behaviors/discussion.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/behaviors/exclfromnav.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/behaviors/exclfromnav.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/behaviors/filename.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/behaviors/filename.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/behaviors/id.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/behaviors/id.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/behaviors/metadata.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/behaviors/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from AccessControl.SecurityManagement import getSecurityManager
 from datetime import datetime
 from DateTime import DateTime
 from plone.app.dexterity import _
-from plone.app.z3cform.widget import AjaxSelectFieldWidget
-from plone.app.z3cform.widget import DatetimeFieldWidget
-from plone.app.z3cform.widget import SelectFieldWidget
+from plone.app.z3cform.widgets.datetime import DatetimeFieldWidget
+from plone.app.z3cform.widgets.select import AjaxSelectFieldWidget
+from plone.app.z3cform.widgets.select import Select2FieldWidget
 from plone.autoform import directives
 from plone.autoform.interfaces import IFormFieldProvider
 from plone.base.interfaces.siteroot import IPloneSiteRoot
 from plone.dexterity.interfaces import IDexterityContent
 from plone.dexterity.utils import safe_unicode
 from plone.supermodel import model
 from Products.CMFCore.utils import getToolByName
@@ -112,15 +112,15 @@
     language = schema.Choice(
         title=_("label_language", default="Language"),
         vocabulary="plone.app.vocabularies.SupportedContentLanguages",
         required=False,
         missing_value="",
         defaultFactory=default_language,
     )
-    directives.widget("language", SelectFieldWidget)
+    directives.widget("language", Select2FieldWidget)
 
     directives.omitted("subjects", "language")
     directives.no_omit(IEditForm, "subjects", "language")
     directives.no_omit(IAddForm, "subjects", "language")
 
 
 class EffectiveAfterExpires(Invalid):
```

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/behaviors/nextprevious.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/behaviors/nextprevious.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/behaviors/tests/test_contrains.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/behaviors/tests/test_contrains.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/behaviors/tests/test_id.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/behaviors/tests/test_id.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/behaviors/tests/test_metadata.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/behaviors/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/browser/add_type.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/browser/add_type.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/browser/behaviors.pt` & `plone_app_dexterity-4.0.0/plone/app/dexterity/browser/behaviors.pt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/browser/behaviors.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/browser/behaviors.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/browser/clone_type.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/browser/clone_type.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/browser/configure.zcml` & `plone_app_dexterity-4.0.0/plone/app/dexterity/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/browser/container.pt` & `plone_app_dexterity-4.0.0/plone/app/dexterity/browser/container.pt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/browser/export.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/browser/export.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/browser/fields.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/browser/fields.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/browser/folder_listing.pt` & `plone_app_dexterity-4.0.0/plone/app/dexterity/browser/folder_listing.pt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/browser/folder_listing.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/browser/folder_listing.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/browser/import_types.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/browser/import_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ Support for importing Dexterity types from GS zip file.
 """
+
 # XXX: need to make exceptions more specific, shorten messages
 from DateTime.DateTime import DateTime
 from io import BytesIO
 from lxml import etree
 from plone.app.dexterity import _
 from plone.namedfile.field import NamedFile
 from plone.z3cform.layout import wrap_form
```

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/browser/item.pt` & `plone_app_dexterity-4.0.0/plone/app/dexterity/browser/item.pt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/browser/modeleditor.pt` & `plone_app_dexterity-4.0.0/plone/app/dexterity/browser/modeleditor.pt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/browser/modeleditor.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/browser/modeleditor.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/browser/overview.pt` & `plone_app_dexterity-4.0.0/plone/app/dexterity/browser/overview.pt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/browser/overview.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/browser/overview.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/browser/tabbed_forms.pt` & `plone_app_dexterity-4.0.0/plone/app/dexterity/browser/tabbed_forms.pt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/browser/types.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/browser/types.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/browser/types_listing.pt` & `plone_app_dexterity-4.0.0/plone/app/dexterity/browser/types_listing.pt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/browser/types_listing_row.pt` & `plone_app_dexterity-4.0.0/plone/app/dexterity/browser/types_listing_row.pt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/browser/typesformwrapper.pt` & `plone_app_dexterity-4.0.0/plone/app/dexterity/browser/typesformwrapper.pt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/configure.zcml` & `plone_app_dexterity-4.0.0/plone/app/dexterity/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/events.zcml` & `plone_app_dexterity-4.0.0/plone/app/dexterity/events.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/factories.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/factories.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/interfaces.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/permissions.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/permissions.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/profiles/default/controlpanel.xml` & `plone_app_dexterity-4.0.0/plone/app/dexterity/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/profiles/testing/types/Document.xml` & `plone_app_dexterity-4.0.0/plone/app/dexterity/profiles/testing/types/Document.xml`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/profiles/testing/types/Folder.xml` & `plone_app_dexterity-4.0.0/plone/app/dexterity/profiles/testing/types/Folder.xml`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/serialize.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/serialize.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/testing.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/tests/discussion.txt` & `plone_app_dexterity-4.0.0/plone/app/dexterity/tests/discussion.txt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/tests/editing.rst` & `plone_app_dexterity-4.0.0/plone/app/dexterity/tests/editing.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/tests/filename.txt` & `plone_app_dexterity-4.0.0/plone/app/dexterity/tests/filename.txt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/tests/import/dexterity_export.zip` & `plone_app_dexterity-4.0.0/plone/app/dexterity/tests/import/dexterity_export.zip`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/tests/metadata.txt` & `plone_app_dexterity-4.0.0/plone/app/dexterity/tests/metadata.txt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/tests/nextprevious.txt` & `plone_app_dexterity-4.0.0/plone/app/dexterity/tests/nextprevious.txt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/tests/robot/test_types.robot` & `plone_app_dexterity-4.0.0/plone/app/dexterity/tests/robot/test_types.robot`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/tests/schema_events.txt` & `plone_app_dexterity-4.0.0/plone/app/dexterity/tests/schema_events.txt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/tests/test_constrains.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/tests/test_constrains.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/tests/test_doctests.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/tests/test_doctests.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/tests/test_export.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/tests/test_export.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test the @@types-export view."""
+
 from plone.app.dexterity.testing import DEXTERITY_INTEGRATION_TESTING
 from plone.app.dexterity.tests.test_constrains import add_item_type
 from xml.dom.minidom import parseString
 from xml.parsers.expat import ExpatError
 from zope.component import getMultiAdapter
 
 import io
```

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/tests/test_import.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/tests/test_import.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test the types import."""
+
 from DateTime.DateTime import DateTime
 from plone.app.dexterity.browser.import_types import ITypeProfileImport
 from plone.app.dexterity.browser.import_types import TypeProfileImport
 from plone.app.dexterity.browser.import_types import ZipFileImportContext
 from plone.app.dexterity.testing import DEXTERITY_INTEGRATION_TESTING
 from Products.CMFCore.utils import getToolByName
```

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/tests/test_namefromtitle.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/tests/test_namefromtitle.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/tests/test_nextprevious.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/tests/test_nextprevious.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/tests/test_robot.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/tests/test_upgrades.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/tests/test_upgrades.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/__init__.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/__init__.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/configure.zcml` & `plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/converters.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/converters.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/directives.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/directives.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/indexer.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/indexer.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/interfaces.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/schemaeditor.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/schemaeditor.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/supermodel.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/supermodel.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/testing.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/tests/behaviors.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/tests/behaviors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Contains different behaviors needed for testing.
 """
+
 from plone.app.dexterity import textindexer
 from plone.app.textfield import RichText
 from plone.autoform.interfaces import IFormFieldProvider
 from plone.namedfile.field import NamedFile
 from plone.supermodel import model
 from zope import schema
 from zope.interface import provider
```

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/tests/behaviors.rst` & `plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/tests/behaviors.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/tests/configure.zcml` & `plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/tests/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/tests/file.pdf` & `plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/tests/file.pdf`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/tests/test_behaviors.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/tests/test_behaviors.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/tests/test_directives.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/tests/test_directives.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/tests/test_schemaeditor.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/tests/test_schemaeditor.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/tests/test_supermodel_handler.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/tests/test_supermodel_handler.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/tests/test_utils.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/textindexer/utils.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/textindexer/utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/upgrades/configure.zcml` & `plone_app_dexterity-4.0.0/plone/app/dexterity/upgrades/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/upgrades/to2001.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/upgrades/to2001.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/upgrades/to2003.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/upgrades/to2003.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/upgrades/to2004.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/upgrades/to2004.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone/app/dexterity/upgrades/to2005.py` & `plone_app_dexterity-4.0.0/plone/app/dexterity/upgrades/to2005.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone.app.dexterity.egg-info/PKG-INFO` & `plone_app_dexterity-4.0.0/plone.app.dexterity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: plone.app.dexterity
-Version: 3.2.0
+Version: 4.0.0
 Summary: Dexterity is a content type framework for CMF  applications, with particular emphasis on Plone. It can be viewed as an alternative to Archetypes that is more light-weight and modular.
 Home-page: http://plone.org/products/dexterity
 Author: Martin Aspeli, David Glick, et al
 Author-email: dexterity-development@googlegroups.com
 License: GPL
 Keywords: plone ttw dexterity schema interface
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
-Classifier: Framework :: Plone :: 6.0
+Classifier: Framework :: Plone :: 6.1
 Classifier: Framework :: Plone :: Core
 Classifier: Framework :: Zope :: 5
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 Requires-Dist: plone.app.textfield
 Requires-Dist: plone.behavior>=1.0
 Requires-Dist: plone.dexterity>=2.2.2
 Requires-Dist: plone.formwidget.namedfile
 Requires-Dist: plone.namedfile>=1.0.0
 Requires-Dist: plone.rfc822
 Requires-Dist: plone.schemaeditor>1.3.3
 Requires-Dist: lxml
 Requires-Dist: plone.base
 Requires-Dist: plone.app.uuid
-Requires-Dist: plone.app.z3cform>=1.1.0
+Requires-Dist: plone.app.z3cform>=4.6.0
 Requires-Dist: plone.autoform>=1.1
 Requires-Dist: plone.contentrules
+Requires-Dist: plone.portlets
 Requires-Dist: plone.schema>=1.1.0
 Requires-Dist: plone.supermodel>=1.1
 Requires-Dist: plone.z3cform>=0.6.0
 Requires-Dist: Products.GenericSetup
 Requires-Dist: setuptools
 Requires-Dist: Zope
 Requires-Dist: zope.browserpage
@@ -371,14 +371,30 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.0 (2024-05-30)
+------------------
+
+Bug fixes:
+
+
+- Remove a DeprecationWarning from a moved p.a.z3cform.widgets import. [@jensens] (#387)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (6e36bcc4)
+
+
 3.2.0 (2023-11-03)
 ------------------
 
 Internal:
 
 
 - Make the dependency on ``plone.app.content`` conditional.
```

### Comparing `plone.app.dexterity-3.2.0/plone.app.dexterity.egg-info/SOURCES.txt` & `plone_app_dexterity-4.0.0/plone.app.dexterity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.2.0/plone.app.dexterity.egg-info/requires.txt` & `plone_app_dexterity-4.0.0/plone.app.dexterity.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 plone.formwidget.namedfile
 plone.namedfile>=1.0.0
 plone.rfc822
 plone.schemaeditor>1.3.3
 lxml
 plone.base
 plone.app.uuid
-plone.app.z3cform>=1.1.0
+plone.app.z3cform>=4.6.0
 plone.autoform>=1.1
 plone.contentrules
+plone.portlets
 plone.schema>=1.1.0
 plone.supermodel>=1.1
 plone.z3cform>=0.6.0
 Products.GenericSetup
 setuptools
 Zope
 zope.browserpage
```

### Comparing `plone.app.dexterity-3.2.0/pyproject.toml` & `plone_app_dexterity-4.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

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
@@ -33,20 +36,44 @@
 showcontent = true
 
 [[tool.towncrier.type]]
 directory = "tests"
 name = "Tests"
 showcontent = true
 
+##
+# Add extra configuration options in .meta.toml:
+#  [pyproject]
+#  towncrier_extra_lines = """
+#  extra_configuration
+#  """
+##
+
 [tool.isort]
 profile = "plone"
 
+##
+# Add extra configuration options in .meta.toml:
+#  [pyproject]
+#  isort_extra_lines = """
+#  extra_configuration
+#  """
+##
+
 [tool.black]
 target-version = ["py38"]
 
+##
+# Add extra configuration options in .meta.toml:
+#  [pyproject]
+#  black_extra_lines = """
+#  extra_configuration
+#  """
+##
+
 [tool.codespell]
 ignore-words-list = "discreet,hove"
 skip = "*.po,"
 ##
 # Add extra configuration options in .meta.toml:
 #  [pyproject]
 #  codespell_ignores = "foo,bar"
@@ -98,34 +125,40 @@
 # Add extra configuration options in .meta.toml:
 #  [pyproject]
 #  dependencies_ignores = "['zestreleaser.towncrier']"
 #  dependencies_mappings = [
 #    "gitpython = ['git']",
 #    "pygithub = ['github']",
 #  ]
-#  """
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

### Comparing `plone.app.dexterity-3.2.0/setup.py` & `plone_app_dexterity-4.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "3.2.0"
+version = "4.0.0"
 
 short_description = (
     "Dexterity is a content type framework for CMF  applications, "
     "with particular emphasis on Plone. It can be viewed as an "
     "alternative to Archetypes that is more light-weight and modular."
 )
 
@@ -25,51 +25,51 @@
     long_description_content_type="text/x-rst",
     # Get more strings from
     # https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
-        "Framework :: Plone :: 6.0",
+        "Framework :: Plone :: 6.1",
         "Framework :: Plone :: Core",
         "Framework :: Zope :: 5",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
     keywords="plone ttw dexterity schema interface",
     author="Martin Aspeli, David Glick, et al",
     author_email="dexterity-development@googlegroups.com",
     url="http://plone.org/products/dexterity",
     license="GPL",
     packages=find_packages(),
     namespace_packages=["plone", "plone.app"],
     include_package_data=True,
     zip_safe=False,
-    python_requires=">=3.8",
+    python_requires=">=3.10",
     install_requires=[
         # Dexterity
         "plone.app.textfield",
         "plone.behavior>=1.0",
         "plone.dexterity>=2.2.2",
         "plone.formwidget.namedfile",
         "plone.namedfile>=1.0.0",
         "plone.rfc822",
-        "plone.schemaeditor >1.3.3",
+        "plone.schemaeditor>1.3.3",
         # Plone/Zope core
         "lxml",
         "plone.base",
         "plone.app.uuid",
-        "plone.app.z3cform>=1.1.0",
+        "plone.app.z3cform>=4.6.0",
         "plone.autoform>=1.1",
         "plone.contentrules",
+        "plone.portlets",
         "plone.schema>=1.1.0",
         "plone.supermodel>=1.1",
         "plone.z3cform>=0.6.0",
         "Products.GenericSetup",
         "setuptools",
         "Zope",
         "zope.browserpage",
```

