# Comparing `tmp/plone_app_z3cform-4.6.0.tar.gz` & `tmp/plone_app_z3cform-4.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone_app_z3cform-4.6.0.tar", last modified: Mon Apr 22 10:05:04 2024, max compression
+gzip compressed data, was "plone_app_z3cform-4.6.1.tar", last modified: Thu May 30 18:22:37 2024, max compression
```

## Comparing `plone_app_z3cform-4.6.0.tar` & `plone_app_z3cform-4.6.1.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-22 10:05:04.705291 plone_app_z3cform-4.6.0/
--rw-r--r--   0 maurits    (501) staff       (20)    27374 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      146 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    51287 2024-04-22 10:05:04.704853 plone_app_z3cform-4.6.0/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)    13825 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-22 10:05:04.674882 plone_app_z3cform-4.6.0/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    12282 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      749 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-22 10:05:04.675199 plone_app_z3cform-4.6.0/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-22 10:05:04.677727 plone_app_z3cform-4.6.0/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-22 10:05:04.683005 plone_app_z3cform-4.6.0/plone/app/z3cform/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1965 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    18525 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/converters.py
--rw-r--r--   0 maurits    (501) staff       (20)     1312 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/converters.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      724 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/csrf.py
--rw-r--r--   0 maurits    (501) staff       (20)      110 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/factories.py
--rw-r--r--   0 maurits    (501) staff       (20)     2349 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/inline_validation.py
--rw-r--r--   0 maurits    (501) staff       (20)     7480 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/inline_validation.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3859 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      212 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/layout.py
--rw-r--r--   0 maurits    (501) staff       (20)      152 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/overrides.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-22 10:05:04.671592 plone_app_z3cform-4.6.0/plone/app/z3cform/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-22 10:05:04.683973 plone_app_z3cform-4.6.0/plone/app/z3cform/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      163 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/profiles/default/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)       85 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)      635 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/profiles.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-22 10:05:04.693179 plone_app_z3cform-4.6.0/plone/app/z3cform/templates/
--rw-r--r--   0 maurits    (501) staff       (20)      435 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/templates/ajaxselect_display.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1607 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/templates/checkbox_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      140 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/templates/contentprovider-widget.pt
--rw-r--r--   0 maurits    (501) staff       (20)      324 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/templates/date_time_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      280 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/templates/email_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      209 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/templates/error.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3712 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/templates/file_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      829 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/templates/form.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3820 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/templates/image_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      677 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/templates/layout.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3356 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/templates/link_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     9654 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/templates/macros.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4033 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/templates/multi_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1861 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/templates/object_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2703 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/templates/orderedselect_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      283 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/templates/password_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      630 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/templates/radio_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      937 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/templates/radio_input_single.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1534 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/templates/relateditems_display.pt
--rw-r--r--   0 maurits    (501) staff       (20)      295 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/templates/richtext_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1465 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/templates/select_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      976 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/templates/singlecheckbox.pt
--rw-r--r--   0 maurits    (501) staff       (20)      290 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/templates/singlecheckboxbool_display.pt
--rw-r--r--   0 maurits    (501) staff       (20)      371 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/templates/singlecheckboxbool_hidden.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1380 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/templates/singlecheckboxbool_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      334 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/templates/submit_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      279 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/templates/text_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      286 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/templates/textarea_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      296 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/templates/textlines_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1801 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/templates/widget.pt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-22 10:05:04.695917 plone_app_z3cform-4.6.0/plone/app/z3cform/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2421 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/tests/example.py
--rw-r--r--   0 maurits    (501) staff       (20)     1139 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/tests/layer.py
--rw-r--r--   0 maurits    (501) staff       (20)      907 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/tests/test_csrf.py
--rw-r--r--   0 maurits    (501) staff       (20)     7951 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/tests/test_patterns.py
--rw-r--r--   0 maurits    (501) staff       (20)     4921 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/tests/test_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)    69170 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/tests/test_widgets.py
--rw-r--r--   0 maurits    (501) staff       (20)      776 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/tests/testing.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1966 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/tests/tests.py
--rw-r--r--   0 maurits    (501) staff       (20)     6162 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     1657 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/views.py
--rw-r--r--   0 maurits    (501) staff       (20)     2961 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/widget.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-22 10:05:04.701553 plone_app_z3cform-4.6.0/plone/app/z3cform/widgets/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/widgets/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     5004 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/widgets/base.py
--rw-r--r--   0 maurits    (501) staff       (20)      728 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/widgets/checkbox.py
--rw-r--r--   0 maurits    (501) staff       (20)     3579 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/widgets/datetime.py
--rw-r--r--   0 maurits    (501) staff       (20)      535 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/widgets/email.py
--rw-r--r--   0 maurits    (501) staff       (20)     2018 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/widgets/link.py
--rw-r--r--   0 maurits    (501) staff       (20)      901 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/widgets/orderedselect.py
--rw-r--r--   0 maurits    (501) staff       (20)      598 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/widgets/password.py
--rw-r--r--   0 maurits    (501) staff       (20)     9722 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/widgets/patterns.py
--rw-r--r--   0 maurits    (501) staff       (20)     2051 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/widgets/querystring.py
--rw-r--r--   0 maurits    (501) staff       (20)      750 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/widgets/radio.py
--rw-r--r--   0 maurits    (501) staff       (20)     8104 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/widgets/relateditems.py
--rw-r--r--   0 maurits    (501) staff       (20)     5437 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/widgets/richtext.py
--rw-r--r--   0 maurits    (501) staff       (20)     8840 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/widgets/select.py
--rw-r--r--   0 maurits    (501) staff       (20)     3165 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/widgets/singlecheckbox.py
--rw-r--r--   0 maurits    (501) staff       (20)     1311 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/widgets/submit.py
--rw-r--r--   0 maurits    (501) staff       (20)     1449 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/widgets/text.py
--rw-r--r--   0 maurits    (501) staff       (20)    13282 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/widgets.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-22 10:05:04.702236 plone_app_z3cform-4.6.0/plone/app/z3cform/wysiwyg/
--rw-r--r--   0 maurits    (501) staff       (20)      273 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/wysiwyg/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      391 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/plone/app/z3cform/wysiwyg/widget.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-22 10:05:04.702609 plone_app_z3cform-4.6.0/plone.app.z3cform.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    51287 2024-04-22 10:05:04.000000 plone_app_z3cform-4.6.0/plone.app.z3cform.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     3461 2024-04-22 10:05:04.000000 plone_app_z3cform-4.6.0/plone.app.z3cform.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-22 10:05:04.000000 plone_app_z3cform-4.6.0/plone.app.z3cform.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2024-04-22 10:05:04.000000 plone_app_z3cform-4.6.0/plone.app.z3cform.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-22 10:05:04.000000 plone_app_z3cform-4.6.0/plone.app.z3cform.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      643 2024-04-22 10:05:04.000000 plone_app_z3cform-4.6.0/plone.app.z3cform.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2024-04-22 10:05:04.000000 plone_app_z3cform-4.6.0/plone.app.z3cform.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4448 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)       38 2024-04-22 10:05:04.705369 plone_app_z3cform-4.6.0/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2706 2024-04-22 10:05:03.000000 plone_app_z3cform-4.6.0/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:22:37.839109 plone_app_z3cform-4.6.1/
+-rw-r--r--   0 maurits    (501) staff       (20)    27735 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      146 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    51648 2024-05-30 18:22:37.838382 plone_app_z3cform-4.6.1/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)    13825 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:22:37.792161 plone_app_z3cform-4.6.1/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    12282 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      749 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:22:37.792613 plone_app_z3cform-4.6.1/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:22:37.796517 plone_app_z3cform-4.6.1/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:22:37.804122 plone_app_z3cform-4.6.1/plone/app/z3cform/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1965 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    18525 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/converters.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1312 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/converters.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      724 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/csrf.py
+-rw-r--r--   0 maurits    (501) staff       (20)      110 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/factories.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2349 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/inline_validation.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7480 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/inline_validation.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3859 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      212 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/layout.py
+-rw-r--r--   0 maurits    (501) staff       (20)      152 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/overrides.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:22:37.787129 plone_app_z3cform-4.6.1/plone/app/z3cform/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:22:37.805215 plone_app_z3cform-4.6.1/plone/app/z3cform/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      163 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/profiles/default/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)       85 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      635 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/profiles.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:22:37.819952 plone_app_z3cform-4.6.1/plone/app/z3cform/templates/
+-rw-r--r--   0 maurits    (501) staff       (20)      435 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/templates/ajaxselect_display.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1607 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/templates/checkbox_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      140 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/templates/contentprovider-widget.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      324 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/templates/date_time_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      280 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/templates/email_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      209 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/templates/error.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3712 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/templates/file_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      829 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/templates/form.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3820 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/templates/image_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      677 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/templates/layout.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3356 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/templates/link_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     9654 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/templates/macros.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4033 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/templates/multi_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1861 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/templates/object_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2703 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/templates/orderedselect_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      283 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/templates/password_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      630 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/templates/radio_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      937 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/templates/radio_input_single.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1534 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/templates/relateditems_display.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      295 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/templates/richtext_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1465 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/templates/select_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      976 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/templates/singlecheckbox.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      290 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/templates/singlecheckboxbool_display.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      371 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/templates/singlecheckboxbool_hidden.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1380 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/templates/singlecheckboxbool_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      334 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/templates/submit_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      279 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/templates/text_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      286 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/templates/textarea_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      296 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/templates/textlines_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1801 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/templates/widget.pt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:22:37.824469 plone_app_z3cform-4.6.1/plone/app/z3cform/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2421 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/tests/example.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1139 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/tests/layer.py
+-rw-r--r--   0 maurits    (501) staff       (20)      907 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/tests/test_csrf.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7951 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/tests/test_patterns.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4921 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/tests/test_utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)    69431 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/tests/test_widgets.py
+-rw-r--r--   0 maurits    (501) staff       (20)      776 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/tests/testing.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1966 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/tests/tests.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6162 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1657 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/views.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2961 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/widget.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:22:37.833041 plone_app_z3cform-4.6.1/plone/app/z3cform/widgets/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/widgets/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5004 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/widgets/base.py
+-rw-r--r--   0 maurits    (501) staff       (20)      728 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/widgets/checkbox.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3486 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/widgets/datetime.py
+-rw-r--r--   0 maurits    (501) staff       (20)      535 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/widgets/email.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2018 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/widgets/link.py
+-rw-r--r--   0 maurits    (501) staff       (20)      901 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/widgets/orderedselect.py
+-rw-r--r--   0 maurits    (501) staff       (20)      598 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/widgets/password.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9722 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/widgets/patterns.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2051 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/widgets/querystring.py
+-rw-r--r--   0 maurits    (501) staff       (20)      750 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/widgets/radio.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8104 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/widgets/relateditems.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5437 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/widgets/richtext.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8840 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/widgets/select.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3165 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/widgets/singlecheckbox.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1311 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/widgets/submit.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1449 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/widgets/text.py
+-rw-r--r--   0 maurits    (501) staff       (20)    13282 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/widgets.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:22:37.834004 plone_app_z3cform-4.6.1/plone/app/z3cform/wysiwyg/
+-rw-r--r--   0 maurits    (501) staff       (20)      273 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/wysiwyg/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      391 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/plone/app/z3cform/wysiwyg/widget.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:22:37.834633 plone_app_z3cform-4.6.1/plone.app.z3cform.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    51648 2024-05-30 18:22:37.000000 plone_app_z3cform-4.6.1/plone.app.z3cform.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     3461 2024-05-30 18:22:37.000000 plone_app_z3cform-4.6.1/plone.app.z3cform.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-05-30 18:22:37.000000 plone_app_z3cform-4.6.1/plone.app.z3cform.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2024-05-30 18:22:37.000000 plone_app_z3cform-4.6.1/plone.app.z3cform.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-05-30 18:22:37.000000 plone_app_z3cform-4.6.1/plone.app.z3cform.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      643 2024-05-30 18:22:37.000000 plone_app_z3cform-4.6.1/plone.app.z3cform.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-05-30 18:22:37.000000 plone_app_z3cform-4.6.1/plone.app.z3cform.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4448 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2024-05-30 18:22:37.839244 plone_app_z3cform-4.6.1/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2706 2024-05-30 18:22:36.000000 plone_app_z3cform-4.6.1/setup.py
```

### Comparing `plone_app_z3cform-4.6.0/CHANGES.rst` & `plone_app_z3cform-4.6.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,26 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.6.1 (2024-05-30)
+------------------
+
+Internal:
+
+
+- Date/time widget: Fix data converter adaption.
+  Get the data converter for the date and datetime widgets via adaption and remove the _converter attribute hack.
+  This aligns the code to z3c.form standards and allows to override the data converter which was previously not easily possible.
+  [thet] (#204)
+
+
 4.6.0 (2024-04-22)
 ------------------
 
 New features:
 
 
 - Use label_css_class attribute from widget if available in checkbox_input & radio_input
```

### Comparing `plone_app_z3cform-4.6.0/PKG-INFO` & `plone_app_z3cform-4.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.z3cform
-Version: 4.6.0
+Version: 4.6.1
 Summary: A collection of widgets, templates and other components for use with z3c.form and Plone
 Home-page: https://pypi.org/project/plone.app.z3cform
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL
 Keywords: zope plone form widget template
 Classifier: Development Status :: 5 - Production/Stable
@@ -690,14 +690,26 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.6.1 (2024-05-30)
+------------------
+
+Internal:
+
+
+- Date/time widget: Fix data converter adaption.
+  Get the data converter for the date and datetime widgets via adaption and remove the _converter attribute hack.
+  This aligns the code to z3c.form standards and allows to override the data converter which was previously not easily possible.
+  [thet] (#204)
+
+
 4.6.0 (2024-04-22)
 ------------------
 
 New features:
 
 
 - Use label_css_class attribute from widget if available in checkbox_input & radio_input
```

### Comparing `plone_app_z3cform-4.6.0/README.rst` & `plone_app_z3cform-4.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/docs/LICENSE.GPL` & `plone_app_z3cform-4.6.1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/docs/LICENSE.txt` & `plone_app_z3cform-4.6.1/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/configure.zcml` & `plone_app_z3cform-4.6.1/plone/app/z3cform/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/converters.py` & `plone_app_z3cform-4.6.1/plone/app/z3cform/converters.py`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/converters.zcml` & `plone_app_z3cform-4.6.1/plone/app/z3cform/converters.zcml`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/csrf.py` & `plone_app_z3cform-4.6.1/plone/app/z3cform/csrf.py`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/inline_validation.py` & `plone_app_z3cform-4.6.1/plone/app/z3cform/inline_validation.py`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/inline_validation.rst` & `plone_app_z3cform-4.6.1/plone/app/z3cform/inline_validation.rst`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/interfaces.py` & `plone_app_z3cform-4.6.1/plone/app/z3cform/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/profiles.zcml` & `plone_app_z3cform-4.6.1/plone/app/z3cform/profiles.zcml`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/templates/checkbox_input.pt` & `plone_app_z3cform-4.6.1/plone/app/z3cform/templates/checkbox_input.pt`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/templates/file_input.pt` & `plone_app_z3cform-4.6.1/plone/app/z3cform/templates/file_input.pt`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/templates/form.pt` & `plone_app_z3cform-4.6.1/plone/app/z3cform/templates/form.pt`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/templates/image_input.pt` & `plone_app_z3cform-4.6.1/plone/app/z3cform/templates/image_input.pt`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/templates/layout.pt` & `plone_app_z3cform-4.6.1/plone/app/z3cform/templates/layout.pt`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/templates/link_input.pt` & `plone_app_z3cform-4.6.1/plone/app/z3cform/templates/link_input.pt`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/templates/macros.pt` & `plone_app_z3cform-4.6.1/plone/app/z3cform/templates/macros.pt`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/templates/multi_input.pt` & `plone_app_z3cform-4.6.1/plone/app/z3cform/templates/multi_input.pt`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/templates/object_input.pt` & `plone_app_z3cform-4.6.1/plone/app/z3cform/templates/object_input.pt`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/templates/orderedselect_input.pt` & `plone_app_z3cform-4.6.1/plone/app/z3cform/templates/orderedselect_input.pt`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/templates/radio_input.pt` & `plone_app_z3cform-4.6.1/plone/app/z3cform/templates/radio_input.pt`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/templates/radio_input_single.pt` & `plone_app_z3cform-4.6.1/plone/app/z3cform/templates/radio_input_single.pt`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/templates/relateditems_display.pt` & `plone_app_z3cform-4.6.1/plone/app/z3cform/templates/relateditems_display.pt`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/templates/select_input.pt` & `plone_app_z3cform-4.6.1/plone/app/z3cform/templates/select_input.pt`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/templates/singlecheckbox.pt` & `plone_app_z3cform-4.6.1/plone/app/z3cform/templates/singlecheckbox.pt`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/templates/singlecheckboxbool_input.pt` & `plone_app_z3cform-4.6.1/plone/app/z3cform/templates/singlecheckboxbool_input.pt`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/templates/widget.pt` & `plone_app_z3cform-4.6.1/plone/app/z3cform/templates/widget.pt`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/tests/example.py` & `plone_app_z3cform-4.6.1/plone/app/z3cform/tests/example.py`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/tests/layer.py` & `plone_app_z3cform-4.6.1/plone/app/z3cform/tests/layer.py`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/tests/test_csrf.py` & `plone_app_z3cform-4.6.1/plone/app/z3cform/tests/test_csrf.py`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/tests/test_patterns.py` & `plone_app_z3cform-4.6.1/plone/app/z3cform/tests/test_patterns.py`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/tests/test_utils.py` & `plone_app_z3cform-4.6.1/plone/app/z3cform/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/tests/test_widgets.py` & `plone_app_z3cform-4.6.1/plone/app/z3cform/tests/test_widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from plone.registry.interfaces import IRegistry
 from plone.supermodel.model import Schema
 from plone.uuid.interfaces import IUUID
 from unittest import mock
 from unittest.mock import Mock
 from z3c.form.form import EditForm
 from z3c.form.form import Form
+from z3c.form.interfaces import IDataConverter
 from z3c.form.interfaces import IValue
 from z3c.form.interfaces import IWidget
 from z3c.form.widget import FieldWidget
 from z3c.form.widget import Widget
 from z3c.relationfield.relation import RelationValue
 from z3c.relationfield.schema import RelationChoice
 from z3c.relationfield.schema import RelationList
@@ -261,18 +262,22 @@
 
     def test_widget_required(self):
         """Required fields should not have a "Clear" button."""
         self.field.required = True
         pattern_options = self.widget.get_pattern_options()
         self.assertEqual(pattern_options["clear"], False)
 
-    def test_data_converter(self):
-        from plone.app.z3cform.widgets.datetime import DateWidgetConverter
+    def test_datewidget_data_converter_adaption(self):
+        from plone.app.z3cform.converters import DateWidgetConverter
+
+        converter = getMultiAdapter((self.field, self.widget), IDataConverter)
+        self.assertEqual(DateWidgetConverter, converter.__class__)
 
-        converter = DateWidgetConverter(self.field, self.widget)
+    def test_data_converter(self):
+        converter = getMultiAdapter((self.field, self.widget), IDataConverter)
 
         self.assertEqual(
             converter.field.missing_value,
             converter.toFieldValue(""),
         )
 
         self.assertEqual(
@@ -371,18 +376,22 @@
 
     def test_widget_required(self):
         """Required fields should not have a "Clear" button."""
         self.field.required = True
         pattern_options = self.widget.get_pattern_options()
         self.assertEqual(pattern_options["clear"], False)
 
-    def test_data_converter(self):
-        from plone.app.z3cform.widgets.datetime import DatetimeWidgetConverter
+    def test_datetimewidget_data_converter_adaption(self):
+        from plone.app.z3cform.converters import DatetimeWidgetConverter
 
-        converter = DatetimeWidgetConverter(self.field, self.widget)
+        converter = getMultiAdapter((self.field, self.widget), IDataConverter)
+        self.assertEqual(DatetimeWidgetConverter, converter.__class__)
+
+    def test_data_converter(self):
+        converter = getMultiAdapter((self.field, self.widget), IDataConverter)
 
         self.assertEqual(
             converter.toFieldValue(""),
             converter.field.missing_value,
         )
 
         self.assertEqual(
@@ -408,70 +417,64 @@
         self.assertEqual(
             converter.toWidgetValue(datetime(21, 10, 30, 15, 40)),
             "21-10-30T15:40",
         )
 
     def test_data_converter__no_timezone(self):
         """When no timezone is set, don't apply one."""
-        from plone.app.z3cform.widgets.datetime import DatetimeWidgetConverter
-
         context = Mock()
 
         dt = datetime(2013, 11, 13, 10, 20)
         setattr(context, self.field.getName(), dt)
         self.widget.context = context
         self.widget.default_timezone = None
 
-        converter = DatetimeWidgetConverter(self.field, self.widget)
+        converter = getMultiAdapter((self.field, self.widget), IDataConverter)
         self.assertEqual(
             converter.toFieldValue("2013-11-13T10:20"),
             datetime(2013, 11, 13, 10, 20),
         )
 
         # cleanup
         self.widget.context = None
         self.widget.default_timezone = None
 
     def test_data_converter__timezone_id(self):
         """When a (pytz) timezone id is set, use that."""
-        from plone.app.z3cform.widgets.datetime import DatetimeWidgetConverter
-
         context = Mock()
 
         dt = datetime(2013, 11, 13, 10, 20)
         setattr(context, self.field.getName(), dt)
         self.widget.context = context
         self.widget.default_timezone = "Europe/Amsterdam"
         tz = pytz.timezone("Europe/Amsterdam")
 
-        converter = DatetimeWidgetConverter(self.field, self.widget)
+        converter = getMultiAdapter((self.field, self.widget), IDataConverter)
         self.assertEqual(
             converter.toFieldValue("2013-11-13T10:20"),
             tz.localize(datetime(2013, 11, 13, 10, 20)),
         )
 
         # cleanup
         self.widget.context = None
         self.widget.default_timezone = None
 
     def test_data_converter__timezone_callback(self):
         """When a timezone callback is set, returning a (pytz) timezone id,
         use that.
         """
-        from plone.app.z3cform.widgets.datetime import DatetimeWidgetConverter
-
         context = Mock()
 
         dt = datetime(2013, 11, 13, 10, 20)
         setattr(context, self.field.getName(), dt)
         self.widget.context = context
         self.widget.default_timezone = lambda context: "Europe/Amsterdam"
         tz = pytz.timezone("Europe/Amsterdam")
 
-        converter = DatetimeWidgetConverter(self.field, self.widget)
+        converter = getMultiAdapter((self.field, self.widget), IDataConverter)
         self.assertEqual(
             converter.toFieldValue("2013-11-13T10:20"),
             tz.localize(datetime(2013, 11, 13, 10, 20)),
         )
 
         # cleanup
         self.widget.context = None
```

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/tests/testing.zcml` & `plone_app_z3cform-4.6.1/plone/app/z3cform/tests/testing.zcml`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/tests/tests.py` & `plone_app_z3cform-4.6.1/plone/app/z3cform/tests/tests.py`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/utils.py` & `plone_app_z3cform-4.6.1/plone/app/z3cform/utils.py`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/views.py` & `plone_app_z3cform-4.6.1/plone/app/z3cform/views.py`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/widget.py` & `plone_app_z3cform-4.6.1/plone/app/z3cform/widget.py`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/widgets/base.py` & `plone_app_z3cform-4.6.1/plone/app/z3cform/widgets/base.py`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/widgets/checkbox.py` & `plone_app_z3cform-4.6.1/plone/app/z3cform/widgets/checkbox.py`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/widgets/datetime.py` & `plone_app_z3cform-4.6.1/plone/app/z3cform/widgets/datetime.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from plone.app.z3cform.converters import DatetimeWidgetConverter
-from plone.app.z3cform.converters import DateWidgetConverter
 from plone.app.z3cform.interfaces import IDatetimeWidget
 from plone.app.z3cform.interfaces import IDateWidget
 from plone.app.z3cform.interfaces import ITimeWidget
 from plone.app.z3cform.utils import dict_merge
 from plone.app.z3cform.widgets.base import HTMLTextInputWidget
 from plone.base import PloneMessageFactory as _
+from z3c.form.interfaces import IDataConverter
 from z3c.form.interfaces import IFieldWidget
 from z3c.form.widget import FieldWidget
 from z3c.form.widget import Widget
+from zope.component import getMultiAdapter
 from zope.i18n import translate
 from zope.interface import implementer
 from zope.interface import implementer_only
 
 
 def get_date_options(request):
     calendar = request.locale.dates.calendars["gregorian"]
@@ -23,15 +23,14 @@
         "today": translate(_("Today"), context=request),
         "clear": translate(_("Clear"), context=request),
     }
 
 
 class DateTimeWidgetBase(HTMLTextInputWidget, Widget):
     _input_type = ""
-    _converter = None
     _formater = ""
     _formater_length = ""
 
     default_timezone = None
     default_time = "00:00:00"
 
     @property
@@ -59,18 +58,20 @@
         """
         if self.mode != "display":
             return super().render()
 
         if not self.value:
             return ""
 
-        if not self._converter:
+        converter = getMultiAdapter((self.field, self), IDataConverter)
+
+        if not converter:
             return self.value
 
-        field_value = self._converter(self.field, self).toFieldValue(self.value)
+        field_value = converter.toFieldValue(self.value)
         if field_value is self.field.missing_value:
             return ""
 
         formatter = self.request.locale.dates.getFormatter(
             self._formater,
             self._formater_length,
         )
@@ -78,15 +79,14 @@
 
 
 @implementer_only(IDateWidget)
 class DateWidget(DateTimeWidgetBase):
     """Date widget for z3c.form."""
 
     _input_type = "date"
-    _converter = DateWidgetConverter
     _formater = "date"
     _formater_length = "short"
 
     pattern = "date-picker"
     klass = "date-widget"
 
 
@@ -96,15 +96,14 @@
 
 
 @implementer_only(IDatetimeWidget)
 class DatetimeWidget(DateTimeWidgetBase):
     """Datetime widget for z3c.form."""
 
     _input_type = "datetime-local"
-    _converter = DatetimeWidgetConverter
     _formater = "dateTime"
     _formater_length = "short"
 
     pattern = "datetime-picker"
     klass = "datetime-widget"
```

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/widgets/email.py` & `plone_app_z3cform-4.6.1/plone/app/z3cform/widgets/email.py`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/widgets/link.py` & `plone_app_z3cform-4.6.1/plone/app/z3cform/widgets/link.py`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/widgets/orderedselect.py` & `plone_app_z3cform-4.6.1/plone/app/z3cform/widgets/orderedselect.py`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/widgets/password.py` & `plone_app_z3cform-4.6.1/plone/app/z3cform/widgets/password.py`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/widgets/patterns.py` & `plone_app_z3cform-4.6.1/plone/app/z3cform/widgets/patterns.py`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/widgets/querystring.py` & `plone_app_z3cform-4.6.1/plone/app/z3cform/widgets/querystring.py`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/widgets/radio.py` & `plone_app_z3cform-4.6.1/plone/app/z3cform/widgets/radio.py`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/widgets/relateditems.py` & `plone_app_z3cform-4.6.1/plone/app/z3cform/widgets/relateditems.py`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/widgets/richtext.py` & `plone_app_z3cform-4.6.1/plone/app/z3cform/widgets/richtext.py`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/widgets/select.py` & `plone_app_z3cform-4.6.1/plone/app/z3cform/widgets/select.py`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/widgets/singlecheckbox.py` & `plone_app_z3cform-4.6.1/plone/app/z3cform/widgets/singlecheckbox.py`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/widgets/submit.py` & `plone_app_z3cform-4.6.1/plone/app/z3cform/widgets/submit.py`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/widgets/text.py` & `plone_app_z3cform-4.6.1/plone/app/z3cform/widgets/text.py`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone/app/z3cform/widgets.zcml` & `plone_app_z3cform-4.6.1/plone/app/z3cform/widgets.zcml`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone.app.z3cform.egg-info/PKG-INFO` & `plone_app_z3cform-4.6.1/plone.app.z3cform.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.z3cform
-Version: 4.6.0
+Version: 4.6.1
 Summary: A collection of widgets, templates and other components for use with z3c.form and Plone
 Home-page: https://pypi.org/project/plone.app.z3cform
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL
 Keywords: zope plone form widget template
 Classifier: Development Status :: 5 - Production/Stable
@@ -690,14 +690,26 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.6.1 (2024-05-30)
+------------------
+
+Internal:
+
+
+- Date/time widget: Fix data converter adaption.
+  Get the data converter for the date and datetime widgets via adaption and remove the _converter attribute hack.
+  This aligns the code to z3c.form standards and allows to override the data converter which was previously not easily possible.
+  [thet] (#204)
+
+
 4.6.0 (2024-04-22)
 ------------------
 
 New features:
 
 
 - Use label_css_class attribute from widget if available in checkbox_input & radio_input
```

### Comparing `plone_app_z3cform-4.6.0/plone.app.z3cform.egg-info/SOURCES.txt` & `plone_app_z3cform-4.6.1/plone.app.z3cform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/plone.app.z3cform.egg-info/requires.txt` & `plone_app_z3cform-4.6.1/plone.app.z3cform.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/pyproject.toml` & `plone_app_z3cform-4.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone_app_z3cform-4.6.0/setup.py` & `plone_app_z3cform-4.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "4.6.0"
+version = "4.6.1"
 
 long_description = (
     f"{Path('README.rst').read_text()}\n"
     f"{(Path('plone') / 'app' / 'z3cform' / 'inline_validation.rst').read_text()}\n"
     f"{Path('CHANGES.rst').read_text()}"
 )
```

