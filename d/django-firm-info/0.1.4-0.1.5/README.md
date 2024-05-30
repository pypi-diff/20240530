# Comparing `tmp/django-firm-info-0.1.4.tar.gz` & `tmp/django_firm_info-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-firm-info-0.1.4.tar", last modified: Thu Sep 21 18:16:09 2023, max compression
+gzip compressed data, was "django_firm_info-0.1.5.tar", last modified: Thu May 30 14:54:13 2024, max compression
```

## Comparing `django-firm-info-0.1.4.tar` & `django_firm_info-0.1.5.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 18:16:08.998433 django-firm-info-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/LICENCE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      316 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2023-09-21 18:16:08.998433 django-firm-info-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      815 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 18:16:08.990433 django-firm-info-0.1.4/django_firm_info.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2023-09-21 18:16:08.000000 django-firm-info-0.1.4/django_firm_info.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2023-09-21 18:16:08.000000 django-firm-info-0.1.4/django_firm_info.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-21 18:16:08.000000 django-firm-info-0.1.4/django_firm_info.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      222 2023-09-21 18:16:08.000000 django-firm-info-0.1.4/django_firm_info.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-09-21 18:16:08.000000 django-firm-info-0.1.4/django_firm_info.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-21 18:16:08.000000 django-firm-info-0.1.4/django_firm_info.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 18:16:08.990433 django-firm-info-0.1.4/firm_info/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 18:16:08.990433 django-firm-info-0.1.4/firm_info/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/contrib/django_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 18:16:08.994433 django-firm-info-0.1.4/firm_info/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/migrations/0002_alter_firmcontact_options_alter_firmcontact_address_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/migrations/0003_firmcontact_baseline_firmcontact_short_description_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/migrations/0004_firmcontact_logo_firmcontact_logo_invert.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/migrations/0005_firmcontact_favicon.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/migrations/0006_alter_firmcontact_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/migrations/0007_socialsharing_tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/migrations/0008_alter_tracking_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/migrations/0009_alter_socialsharing_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/migrations/0010_appsbanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/migrations/0011_alter_firmcontact_favicon_alter_firmcontact_logo_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/migrations/0012_alter_appsbanner_application_type.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7865 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 18:16:08.994433 django-firm-info-0.1.4/firm_info/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/templates/baseline.html
--rw-r--r--   0 runner    (1001) docker     (127)      232 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/templates/favicon.html
--rw-r--r--   0 runner    (1001) docker     (127)      431 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/templates/footer_adress.html
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/templates/footer_network.html
--rw-r--r--   0 runner    (1001) docker     (127)      428 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/templates/footer_social_sharing.html
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/templates/header_network.html
--rw-r--r--   0 runner    (1001) docker     (127)      212 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/templates/header_phone.html
--rw-r--r--   0 runner    (1001) docker     (127)      245 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/templates/logo.html
--rw-r--r--   0 runner    (1001) docker     (127)      171 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/templates/logo_i.html
--rw-r--r--   0 runner    (1001) docker     (127)      168 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/templates/og-description.html
--rw-r--r--   0 runner    (1001) docker     (127)      143 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/templates/og-image.html
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/templates/og-twitter-site.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 18:16:08.986433 django-firm-info-0.1.4/firm_info/templates/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 18:16:08.986433 django-firm-info-0.1.4/firm_info/templates/tests/templatetags/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 18:16:08.994433 django-firm-info-0.1.4/firm_info/templates/tests/templatetags/firm_info/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/templates/tests/templatetags/firm_info/test_firm_contact.html
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/templates/tests/templatetags/firm_info/test_firm_description.html
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/templates/tests/templatetags/firm_info/test_links.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 18:16:08.994433 django-firm-info-0.1.4/firm_info/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5758 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/firm_info/templatetags/firm_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2023-09-21 18:16:08.998433 django-firm-info-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-09-21 18:15:59.000000 django-firm-info-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:54:13.586113 django_firm_info-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-30 14:54:13.586113 django_firm_info-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:54:13.586113 django_firm_info-0.1.5/django_firm_info.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-30 14:54:13.000000 django_firm_info-0.1.5/django_firm_info.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-30 14:54:13.000000 django_firm_info-0.1.5/django_firm_info.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 14:54:13.000000 django_firm_info-0.1.5/django_firm_info.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-30 14:54:13.000000 django_firm_info-0.1.5/django_firm_info.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 14:54:13.000000 django_firm_info-0.1.5/django_firm_info.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 14:54:13.000000 django_firm_info-0.1.5/django_firm_info.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:54:13.578113 django_firm_info-0.1.5/firm_info/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:54:13.582113 django_firm_info-0.1.5/firm_info/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/contrib/django_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:54:13.582113 django_firm_info-0.1.5/firm_info/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/migrations/0002_alter_firmcontact_options_alter_firmcontact_address_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/migrations/0003_firmcontact_baseline_firmcontact_short_description_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/migrations/0004_firmcontact_logo_firmcontact_logo_invert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/migrations/0005_firmcontact_favicon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/migrations/0006_alter_firmcontact_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/migrations/0007_socialsharing_tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/migrations/0008_alter_tracking_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/migrations/0009_alter_socialsharing_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/migrations/0010_appsbanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/migrations/0011_alter_firmcontact_favicon_alter_firmcontact_logo_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/migrations/0012_alter_appsbanner_application_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7865 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:54:13.586113 django_firm_info-0.1.5/firm_info/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/templates/baseline.html
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/templates/favicon.html
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/templates/footer_adress.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/templates/footer_network.html
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/templates/footer_social_sharing.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/templates/header_network.html
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/templates/header_phone.html
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/templates/logo.html
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/templates/logo_i.html
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/templates/og-description.html
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/templates/og-image.html
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/templates/og-twitter-site.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:54:13.578113 django_firm_info-0.1.5/firm_info/templates/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:54:13.578113 django_firm_info-0.1.5/firm_info/templates/tests/templatetags/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:54:13.586113 django_firm_info-0.1.5/firm_info/templates/tests/templatetags/firm_info/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/templates/tests/templatetags/firm_info/test_firm_contact.html
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/templates/tests/templatetags/firm_info/test_firm_description.html
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/templates/tests/templatetags/firm_info/test_links.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:54:13.586113 django_firm_info-0.1.5/firm_info/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/firm_info/templatetags/firm_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-30 14:54:13.586113 django_firm_info-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-30 14:54:10.000000 django_firm_info-0.1.5/setup.py
```

### Comparing `django-firm-info-0.1.4/LICENCE.txt` & `django_firm_info-0.1.5/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `django-firm-info-0.1.4/PKG-INFO` & `django_firm_info-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-firm-info
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Django application package for storage firm info
 Home-page: https://github.com/emencia/django-firm-info
 Author: Philippe Lafaye
 Author-email: lafaye@emencia.com
 License: MIT
 Project-URL: Source Code, https://github.com/emencia/django-firm-info
 Project-URL: Issue Tracker, https://github.com/emencia/django-firm-info/issues
@@ -18,16 +18,14 @@
 Classifier: Environment :: Web Environment
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
-Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/x-rst
 License-File: LICENCE.txt
 Requires-Dist: Django>=3.2
```

### Comparing `django-firm-info-0.1.4/README.rst` & `django_firm_info-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `django-firm-info-0.1.4/django_firm_info.egg-info/PKG-INFO` & `django_firm_info-0.1.5/django_firm_info.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-firm-info
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Django application package for storage firm info
 Home-page: https://github.com/emencia/django-firm-info
 Author: Philippe Lafaye
 Author-email: lafaye@emencia.com
 License: MIT
 Project-URL: Source Code, https://github.com/emencia/django-firm-info
 Project-URL: Issue Tracker, https://github.com/emencia/django-firm-info/issues
@@ -18,16 +18,14 @@
 Classifier: Environment :: Web Environment
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
-Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/x-rst
 License-File: LICENCE.txt
 Requires-Dist: Django>=3.2
```

### Comparing `django-firm-info-0.1.4/django_firm_info.egg-info/SOURCES.txt` & `django_firm_info-0.1.5/django_firm_info.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-firm-info-0.1.4/firm_info/admin.py` & `django_firm_info-0.1.5/firm_info/admin.py`

 * *Files identical despite different names*

### Comparing `django-firm-info-0.1.4/firm_info/contrib/django_configuration.py` & `django_firm_info-0.1.5/firm_info/contrib/django_configuration.py`

 * *Files identical despite different names*

### Comparing `django-firm-info-0.1.4/firm_info/factories.py` & `django_firm_info-0.1.5/firm_info/factories.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from PIL import Image as PILimage
 
 from django.core.files import File
 
 import factory
 from firm_info.models import Tracking
 
-from .models import AppsBanner
+from .models import AppsBanner, FirmContact
 
 
 def create_image_file(filename=None, size=(100, 100), color="blue",
                       format_name="PNG"):
     """
     Return a File object with a dummy generated image on the fly by PIL or
     possibly a SVG file.
@@ -100,7 +100,37 @@
         Fill file field with generated image.
 
         Returns:
             django.core.files.File: File object.
         """
 
         return create_image_file()
+
+
+class FirmContactFactory(factory.django.DjangoModelFactory):
+    """
+    Factory to create instance of a FirmContact.
+    """
+
+    phone_number = factory.Faker("phone_number")
+    email = factory.Faker("email")
+    address = factory.Faker("address")
+    postal_code = factory.Faker("postcode")
+    city = factory.Faker("city")
+    country = factory.Faker("country")
+    baseline = factory.Faker("text", max_nb_chars=255)
+    short_description = factory.Faker("text")
+
+    class Meta:
+        model = FirmContact
+
+    @factory.lazy_attribute
+    def logo(self):
+        return create_image_file()
+
+    @factory.lazy_attribute
+    def logo_invert(self):
+        return create_image_file()
+
+    @factory.lazy_attribute
+    def favicon(self):
+        return create_image_file()
```

### Comparing `django-firm-info-0.1.4/firm_info/migrations/0001_initial.py` & `django_firm_info-0.1.5/firm_info/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-firm-info-0.1.4/firm_info/migrations/0002_alter_firmcontact_options_alter_firmcontact_address_and_more.py` & `django_firm_info-0.1.5/firm_info/migrations/0002_alter_firmcontact_options_alter_firmcontact_address_and_more.py`

 * *Files identical despite different names*

### Comparing `django-firm-info-0.1.4/firm_info/migrations/0003_firmcontact_baseline_firmcontact_short_description_and_more.py` & `django_firm_info-0.1.5/firm_info/migrations/0003_firmcontact_baseline_firmcontact_short_description_and_more.py`

 * *Files identical despite different names*

### Comparing `django-firm-info-0.1.4/firm_info/migrations/0004_firmcontact_logo_firmcontact_logo_invert.py` & `django_firm_info-0.1.5/firm_info/migrations/0004_firmcontact_logo_firmcontact_logo_invert.py`

 * *Files identical despite different names*

### Comparing `django-firm-info-0.1.4/firm_info/migrations/0007_socialsharing_tracking.py` & `django_firm_info-0.1.5/firm_info/migrations/0007_socialsharing_tracking.py`

 * *Files identical despite different names*

### Comparing `django-firm-info-0.1.4/firm_info/migrations/0010_appsbanner.py` & `django_firm_info-0.1.5/firm_info/migrations/0010_appsbanner.py`

 * *Files identical despite different names*

### Comparing `django-firm-info-0.1.4/firm_info/migrations/0011_alter_firmcontact_favicon_alter_firmcontact_logo_and_more.py` & `django_firm_info-0.1.5/firm_info/migrations/0011_alter_firmcontact_favicon_alter_firmcontact_logo_and_more.py`

 * *Files identical despite different names*

### Comparing `django-firm-info-0.1.4/firm_info/migrations/0012_alter_appsbanner_application_type.py` & `django_firm_info-0.1.5/firm_info/migrations/0012_alter_appsbanner_application_type.py`

 * *Files identical despite different names*

### Comparing `django-firm-info-0.1.4/firm_info/models.py` & `django_firm_info-0.1.5/firm_info/models.py`

 * *Files identical despite different names*

### Comparing `django-firm-info-0.1.4/firm_info/serializers.py` & `django_firm_info-0.1.5/firm_info/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-class SerializeFirmError(Exception):
-    pass
+from firm_info.exceptions import SerializeFirmError
 
 
 def _format_address(firm_info: dict) -> str:
     """
     Formats the address using the firm information.
 
     Args:
```

### Comparing `django-firm-info-0.1.4/firm_info/templates/footer_network.html` & `django_firm_info-0.1.5/firm_info/templates/footer_network.html`

 * *Files identical despite different names*

### Comparing `django-firm-info-0.1.4/firm_info/templates/header_network.html` & `django_firm_info-0.1.5/firm_info/templates/header_network.html`

 * *Files identical despite different names*

### Comparing `django-firm-info-0.1.4/firm_info/templatetags/firm_info.py` & `django_firm_info-0.1.5/firm_info/templatetags/firm_info.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,16 +9,16 @@
     serialize_firm_social,
     serialize_firm_social_sharing,
 )
 
 register = Library()
 
 
-@register.simple_tag(name="firm_contact")
-def firm_contact(template_path):
+@register.simple_tag(takes_context=True, name="firm_contact")
+def firm_contact(context, template_path):
     """
     Renders the template which path is provided as param
     using FirmContact only instance serialized contact data.
 
     Args:
         template_path (str): The path to the template file.
 
@@ -32,23 +32,24 @@
         {% load firm_info %}
         {% firm_contact "path/to/template.html" %}
 
     """
     qs_firm_info = FirmContact.objects.all()
     if qs_firm_info.exists():
         template = loader.get_template(template_path)
-        context = serialize_firm_info(qs_firm_info)
-        rendered = template.render(context)
+        specific_context = serialize_firm_info(qs_firm_info)
+        combined_context = {**context.flatten(), **specific_context}
+        rendered = template.render(combined_context)
         return rendered
     else:
         return ''
 
 
-@register.simple_tag(name="firm_social_links")
-def firm_social_links(template_path):
+@register.simple_tag(takes_context=True, name="firm_social_links")
+def firm_social_links(context, template_path):
     """
     Renders the template which path is provided as param
     using all social network link objects serialized data
     related the only FirmContact instance.
 
     Args:
         template_path (str): The path to the template file.
@@ -63,23 +64,24 @@
         {% load firm_info %}
         {% firm_social_links "path/to/template.html" %}
 
     """
     links = Link.objects.all()
     if links.exists():
         template = loader.get_template(template_path)
-        context = serialize_firm_social(links)
-        rendered = template.render(context)
+        specific_context = serialize_firm_social(links)
+        combined_context = {**context.flatten(), **specific_context}
+        rendered = template.render(combined_context)
         return rendered
     else:
         return ''
 
 
-@register.simple_tag(name="firm_description")
-def firm_description(template_path):
+@register.simple_tag(takes_context=True, name="firm_description")
+def firm_description(context, template_path):
     """
     Renders the template which path is provided as param
     using FirmContact only instance serialized description data.
 
     Args:
         template_path (str): The path to the template file.
 
@@ -93,23 +95,24 @@
         {% load firm_info %}
         {% firm_description "path/to/template.html" %}
 
     """
     qs_firm_info = FirmContact.objects.all()
     if qs_firm_info.exists():
         template = loader.get_template(template_path)
-        context = serialize_firm_description(qs_firm_info)
-        rendered = template.render(context)
+        specific_context = serialize_firm_description(qs_firm_info)
+        combined_context = {**context.flatten(), **specific_context}
+        rendered = template.render(combined_context)
         return rendered
     else:
         return ''
 
 
-@register.simple_tag(name="firm_logos")
-def firm_logos(template_path):
+@register.simple_tag(takes_context=True, name="firm_logos")
+def firm_logos(context, template_path):
     """
     Renders the firm logos using the specified template.
 
     Args:
         template_path (str): The path to the template file.
 
     Returns:
@@ -122,27 +125,28 @@
         {% load firm_info %}
         {% firm_logos "path/to/template.html" %}
 
     """
     firm_instance = FirmContact.objects.first()
     if firm_instance:
         template = loader.get_template(template_path)
-        context = {
+        specific_context = {
             "logo": getattr(firm_instance, "logo", None),
             "logo_invert": getattr(firm_instance, "logo_invert", None),
             "favicon": getattr(firm_instance, "favicon", None),
         }
-        rendered = template.render(context)
+        combined_context = {**context.flatten(), **specific_context}
+        rendered = template.render(combined_context)
         return rendered
     else:
         return ''
 
 
-@register.simple_tag(name="firm_social_shares")
-def firm_social_shares(template_path):
+@register.simple_tag(takes_context=True, name="firm_social_shares")
+def firm_social_shares(context, template_path):
     """
     Renders the template which path is provided as param
     using all social network shares link objects serialized data
     related the only SocialSharing instance.
 
     Args:
         template_path (str): The path to the template file.
@@ -158,16 +162,17 @@
         {% firm_social_shares "path/to/template.html" %}
 
     """
     social_shares = SocialSharing.objects.first()
 
     if social_shares:
         template = loader.get_template(template_path)
-        context = serialize_firm_social_sharing(social_shares)
-        rendered = template.render(context)
+        specific_context = serialize_firm_social_sharing(social_shares)
+        combined_context = {**context.flatten(), **specific_context}
+        rendered = template.render(combined_context)
 
         return rendered
     else:
         return ''
 
 
 @register.filter("firm_tag_analytic")
@@ -189,16 +194,16 @@
         {% load firm_info %}
         {% firm_tag_analytic "path/to/template.html" %}
 
     """
     return Tracking.objects.first().tag_analytic if Tracking.objects.exists() else ""
 
 
-@register.simple_tag(name="app_banner")
-def app_banner(app_type, template_path):
+@register.simple_tag(takes_context=True, name="app_banner")
+def app_banner(context, app_type, template_path):
     """
     Renders the app banner using the specified template and application type.
 
     Args:
         app_type (str): The application type.
         template_path (str): The path to the template file.
 
@@ -214,11 +219,12 @@
 
     """
     context = {}
     template = loader.get_template(template_path)
 
     with contextlib.suppress(ObjectDoesNotExist):
         app_banner = AppsBanner.objects.get(application_type=app_type)
-        context = serialize_firm_apps_banner(app_banner)
-    rendered = template.render(context)
+        specific_context = serialize_firm_apps_banner(app_banner)
+        combined_context = {**context.flatten(), **specific_context}
+    rendered = template.render(combined_context)
 
     return rendered
```

### Comparing `django-firm-info-0.1.4/setup.cfg` & `django_firm_info-0.1.5/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-firm-info
-version = 0.1.4
+version = 0.1.5
 description = A Django application package for storage firm info
 long_description = file:README.rst
 long_description_content_type = text/x-rst
 author = Philippe Lafaye
 author_email = lafaye@emencia.com
 url = https://github.com/emencia/django-firm-info
 project_urls = 
@@ -22,16 +22,14 @@
 	Environment :: Web Environment
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Framework :: Django
 	Framework :: Django :: 3.2
-	Framework :: Django :: 4.0
-	Framework :: Django :: 4.1
 	Framework :: Django :: 4.2
 	Intended Audience :: Developers
 	Topic :: Internet :: WWW/HTTP
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 include_package_data = True
@@ -85,27 +83,25 @@
 python_files = 
 	*.py
 testpaths = 
 	tests
 
 [tox:tox]
 minversion = 3.4.0
-envlist = py{38,39,310}-django{32,40,41,42}
+envlist = py{38,39,310}-django{32,42}
 
 [gh-actions]
 python = 
 	3.8: py38
 	3.9: py39
 	3.10: py310
 
 [testenv]
 deps = 
 	django32: Django>=3.2,<4.0
-	django40: Django>=4.0,<4.1
-	django41: Django>=4.1,<4.2
 	django42: Django>=4.2,<5.0
 	py38-django32: backports.zoneinfo
 commands = 
 	pip install -e .[dev]
 	pytest -vv tests
 
 [egg_info]
```

