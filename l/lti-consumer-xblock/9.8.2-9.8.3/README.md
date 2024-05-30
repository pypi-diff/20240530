# Comparing `tmp/lti-consumer-xblock-9.8.2.tar.gz` & `tmp/lti-consumer-xblock-9.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lti-consumer-xblock-9.8.2.tar", last modified: Mon Jan 22 15:20:06 2024, max compression
+gzip compressed data, was "lti-consumer-xblock-9.8.3.tar", last modified: Tue Jan 23 16:47:55 2024, max compression
```

## Comparing `lti-consumer-xblock-9.8.2.tar` & `lti-consumer-xblock-9.8.3.tar`

### file list

```diff
@@ -1,246 +1,246 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.165914 lti-consumer-xblock-9.8.2/
--rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)    16103 2024-01-22 15:20:06.165914 lti-consumer-xblock-9.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14840 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.145915 lti-consumer-xblock-9.8.2/lti_consumer/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)    12233 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.145915 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15317 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p1/consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.145915 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p1/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p1/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p1/contrib/django.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.145915 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p1/contrib/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p1/contrib/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6923 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p1/contrib/tests/test_django.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p1/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p1/oauth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.145915 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14154 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p1/tests/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p1/tests/test_oauth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.145915 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/ags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    35458 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/deep_linking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.145915 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.149915 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/extensions/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/extensions/rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/extensions/rest_framework/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py
--rw-r--r--   0 runner    (1001) docker     (127)    14353 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/extensions/rest_framework/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10557 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/key_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/nprs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.149915 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.149915 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/tests/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/tests/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.149915 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/tests/extensions/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/tests/extensions/rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     9875 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/tests/test_ags.py
--rw-r--r--   0 runner    (1001) docker     (127)    45009 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/tests/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/tests/test_deep_linking.py
--rw-r--r--   0 runner    (1001) docker     (127)    10270 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/tests/test_key_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/tests/test_nrps.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    75714 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/lti_xblock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.153915 lti-consumer-xblock-9.8.2/lti_consumer/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/migrations/0002_ltiagslineitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/migrations/0003_ltiagsscore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/migrations/0004_keyset_mgmt_to_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/migrations/0005_migrate_keyset_to_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/migrations/0007_ltidlcontentitem.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/migrations/0008_fix_uuid_backfill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/migrations/0009_backfill-empty-string-config-id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/migrations/0012_rename_courseeditltifieldsenabledflag_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/migrations/0013_auto_20210712_1352.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/migrations/0014_adds_external_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/migrations/0015_add_additional_1p3_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35477 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     8232 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/outcomes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.153915 lti-consumer-xblock-9.8.2/lti_consumer/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11574 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/plugin/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/plugin/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    39612 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/plugin/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.137915 lti-consumer-xblock-9.8.2/lti_consumer/public/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.137915 lti-consumer-xblock-9.8.2/lti_consumer/public/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.137915 lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.153915 lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/ar/
--rw-r--r--   0 runner    (1001) docker     (127)    22730 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/ar/text.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.153915 lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/en/
--rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/en/text.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.153915 lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/es_419/
--rw-r--r--   0 runner    (1001) docker     (127)    23422 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/es_419/text.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.153915 lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/fr/
--rw-r--r--   0 runner    (1001) docker     (127)    21751 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/fr/text.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.153915 lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/he/
--rw-r--r--   0 runner    (1001) docker     (127)    20445 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/he/text.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.153915 lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/hi/
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/hi/text.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.153915 lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/it/
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/it/text.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.153915 lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/ja/
--rw-r--r--   0 runner    (1001) docker     (127)    16711 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/ja/text.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.153915 lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/ko/
--rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/ko/text.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.153915 lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/pt_BR/
--rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/pt_BR/text.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.153915 lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/pt_PT/
--rw-r--r--   0 runner    (1001) docker     (127)    27017 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/pt_PT/text.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.153915 lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/ru/
--rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/ru/text.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.153915 lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/zh_CN/
--rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/zh_CN/text.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.153915 lti-consumer-xblock-9.8.2/lti_consumer/signals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/signals/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.137915 lti-consumer-xblock-9.8.2/lti_consumer/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.153915 lti-consumer-xblock-9.8.2/lti_consumer/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/static/css/student.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.153915 lti-consumer-xblock-9.8.2/lti_consumer/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    12186 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/static/js/xblock_lti_consumer.js
--rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/static/js/xblock_studio_view.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.153915 lti-consumer-xblock-9.8.2/lti_consumer/static/sass/
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/static/sass/student.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.137915 lti-consumer-xblock-9.8.2/lti_consumer/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.157914 lti-consumer-xblock-9.8.2/lti_consumer/templates/html/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.157914 lti-consumer-xblock-9.8.2/lti_consumer/templates/html/lti-dl/
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/templates/html/lti-dl/dl_response_error.html
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/templates/html/lti-dl/dl_response_saved.html
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/templates/html/lti-dl/render_dl_content.html
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/templates/html/lti-dl/render_html.html
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/templates/html/lti-dl/render_image.html
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/templates/html/lti-dl/render_link.html
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/templates/html/lti-dl/render_lti_resource_link.html
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/templates/html/lti_1p3_launch.html
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/templates/html/lti_1p3_permission_error.html
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/templates/html/lti_1p3_studio.html
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/templates/html/lti_iframe.html
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/templates/html/lti_launch.html
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/templates/html/lti_launch_error.html
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/templates/html/lti_proctoring_start_error.html
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/templates/html/lti_start_assessment.html
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/templates/html/student.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.157914 lti-consumer-xblock-9.8.2/lti_consumer/templates/xml/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/templates/xml/outcome_service_response.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.157914 lti-consumer-xblock-9.8.2/lti_consumer/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/templatetags/get_dl_lti_launch_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/templatetags/lti_sanitize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.157914 lti-consumer-xblock-9.8.2/lti_consumer/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.157914 lti-consumer-xblock-9.8.2/lti_consumer/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.161914 lti-consumer-xblock-9.8.2/lti_consumer/tests/unit/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/tests/unit/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11960 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/tests/unit/plugin/test_proctoring.py
--rw-r--r--   0 runner    (1001) docker     (127)    33526 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/tests/unit/plugin/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)    38579 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/tests/unit/plugin/test_views_lti_ags.py
--rw-r--r--   0 runner    (1001) docker     (127)    26203 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py
--rw-r--r--   0 runner    (1001) docker     (127)    10559 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py
--rw-r--r--   0 runner    (1001) docker     (127)    28029 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/tests/unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/tests/unit/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    91837 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/tests/unit/test_lti_xblock.py
--rw-r--r--   0 runner    (1001) docker     (127)    29276 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/tests/unit/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    16718 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/tests/unit/test_outcomes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/tests/unit/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     6028 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/track.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.161914 lti-consumer-xblock-9.8.2/lti_consumer/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.141915 lti-consumer-xblock-9.8.2/lti_consumer/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.161914 lti-consumer-xblock-9.8.2/lti_consumer/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    10252 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/translations/ar/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (127)    22143 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/translations/ar/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/translations/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.141915 lti-consumer-xblock-9.8.2/lti_consumer/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.161914 lti-consumer-xblock-9.8.2/lti_consumer/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/translations/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    16396 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/translations/en/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/translations/en/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (127)    16396 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/translations/en/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.141915 lti-consumer-xblock-9.8.2/lti_consumer/translations/es_419/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.161914 lti-consumer-xblock-9.8.2/lti_consumer/translations/es_419/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    20799 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/translations/es_419/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (127)    26467 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/translations/es_419/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.141915 lti-consumer-xblock-9.8.2/lti_consumer/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.161914 lti-consumer-xblock-9.8.2/lti_consumer/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18761 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/translations/fr/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (127)    25340 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/translations/fr/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.141915 lti-consumer-xblock-9.8.2/lti_consumer/translations/fr_CA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.161914 lti-consumer-xblock-9.8.2/lti_consumer/translations/fr_CA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     9166 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10186 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/translations/fr_CA/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.141915 lti-consumer-xblock-9.8.2/lti_consumer/translations/he/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.161914 lti-consumer-xblock-9.8.2/lti_consumer/translations/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     9608 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/translations/he/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (127)    21499 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/translations/he/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.141915 lti-consumer-xblock-9.8.2/lti_consumer/translations/hi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.161914 lti-consumer-xblock-9.8.2/lti_consumer/translations/hi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/translations/hi/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (127)    16407 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/translations/hi/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.141915 lti-consumer-xblock-9.8.2/lti_consumer/translations/ja_JP/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.165914 lti-consumer-xblock-9.8.2/lti_consumer/translations/ja_JP/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (127)    21266 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.141915 lti-consumer-xblock-9.8.2/lti_consumer/translations/ko_KR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.165914 lti-consumer-xblock-9.8.2/lti_consumer/translations/ko_KR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/translations/ko_KR/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (127)    16477 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/translations/ko_KR/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.141915 lti-consumer-xblock-9.8.2/lti_consumer/translations/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.165914 lti-consumer-xblock-9.8.2/lti_consumer/translations/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (127)    16884 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/translations/pt_BR/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.141915 lti-consumer-xblock-9.8.2/lti_consumer/translations/pt_PT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.165914 lti-consumer-xblock-9.8.2/lti_consumer/translations/pt_PT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    23772 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (127)    27799 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.141915 lti-consumer-xblock-9.8.2/lti_consumer/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.165914 lti-consumer-xblock-9.8.2/lti_consumer/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/translations/ru/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (127)    16547 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/translations/ru/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/translations/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.141915 lti-consumer-xblock-9.8.2/lti_consumer/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.165914 lti-consumer-xblock-9.8.2/lti_consumer/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/translations/zh_CN/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (127)    16458 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/translations/zh_CN/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (127)    11729 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/lti_consumer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.165914 lti-consumer-xblock-9.8.2/lti_consumer_xblock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16103 2024-01-22 15:20:06.000000 lti-consumer-xblock-9.8.2/lti_consumer_xblock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7644 2024-01-22 15:20:06.000000 lti-consumer-xblock-9.8.2/lti_consumer_xblock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-01-22 15:20:06.000000 lti-consumer-xblock-9.8.2/lti_consumer_xblock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-01-22 15:20:06.000000 lti-consumer-xblock-9.8.2/lti_consumer_xblock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-01-22 15:20:06.000000 lti-consumer-xblock-9.8.2/lti_consumer_xblock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-22 15:20:06.000000 lti-consumer-xblock-9.8.2/lti_consumer_xblock.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:20:06.165914 lti-consumer-xblock-9.8.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-01-22 15:20:06.169914 lti-consumer-xblock-9.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-01-22 15:20:02.000000 lti-consumer-xblock-9.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.780395 lti-consumer-xblock-9.8.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)    16103 2024-01-23 16:47:55.780395 lti-consumer-xblock-9.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14840 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.752395 lti-consumer-xblock-9.8.3/lti_consumer/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12233 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.752395 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15317 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p1/consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.756395 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p1/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p1/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p1/contrib/django.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.756395 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p1/contrib/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p1/contrib/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6923 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p1/contrib/tests/test_django.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p1/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p1/oauth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.756395 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14154 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p1/tests/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p1/tests/test_oauth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.756395 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/ags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35535 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/deep_linking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.756395 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.756395 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/extensions/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/extensions/rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/extensions/rest_framework/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14353 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/extensions/rest_framework/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10762 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/key_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/nprs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.760395 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.760395 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/tests/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/tests/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.760395 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/tests/extensions/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/tests/extensions/rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9875 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/tests/test_ags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45009 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/tests/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/tests/test_deep_linking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10270 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/tests/test_key_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/tests/test_nrps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75714 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/lti_xblock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.764395 lti-consumer-xblock-9.8.3/lti_consumer/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/migrations/0002_ltiagslineitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/migrations/0003_ltiagsscore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/migrations/0004_keyset_mgmt_to_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/migrations/0005_migrate_keyset_to_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/migrations/0007_ltidlcontentitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/migrations/0008_fix_uuid_backfill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/migrations/0009_backfill-empty-string-config-id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/migrations/0012_rename_courseeditltifieldsenabledflag_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/migrations/0013_auto_20210712_1352.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/migrations/0014_adds_external_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/migrations/0015_add_additional_1p3_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35477 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8232 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/outcomes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.764395 lti-consumer-xblock-9.8.3/lti_consumer/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11574 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/plugin/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/plugin/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39612 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/plugin/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.744395 lti-consumer-xblock-9.8.3/lti_consumer/public/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.744395 lti-consumer-xblock-9.8.3/lti_consumer/public/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.744395 lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.764395 lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/ar/
+-rw-r--r--   0 runner    (1001) docker     (127)    22730 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/ar/text.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.764395 lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/en/
+-rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/en/text.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.764395 lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/es_419/
+-rw-r--r--   0 runner    (1001) docker     (127)    23422 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/es_419/text.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.764395 lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)    21751 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/fr/text.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.764395 lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/he/
+-rw-r--r--   0 runner    (1001) docker     (127)    20445 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/he/text.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.764395 lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/hi/
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/hi/text.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.764395 lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/it/
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/it/text.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.764395 lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/ja/
+-rw-r--r--   0 runner    (1001) docker     (127)    16711 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/ja/text.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.764395 lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/ko/
+-rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/ko/text.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.764395 lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/pt_BR/
+-rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/pt_BR/text.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.764395 lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/pt_PT/
+-rw-r--r--   0 runner    (1001) docker     (127)    27017 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/pt_PT/text.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.764395 lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/ru/
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/ru/text.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.764395 lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/zh_CN/
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/zh_CN/text.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.764395 lti-consumer-xblock-9.8.3/lti_consumer/signals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/signals/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.744395 lti-consumer-xblock-9.8.3/lti_consumer/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.764395 lti-consumer-xblock-9.8.3/lti_consumer/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/static/css/student.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.764395 lti-consumer-xblock-9.8.3/lti_consumer/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    12186 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/static/js/xblock_lti_consumer.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/static/js/xblock_studio_view.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.768395 lti-consumer-xblock-9.8.3/lti_consumer/static/sass/
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/static/sass/student.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.748395 lti-consumer-xblock-9.8.3/lti_consumer/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.768395 lti-consumer-xblock-9.8.3/lti_consumer/templates/html/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.768395 lti-consumer-xblock-9.8.3/lti_consumer/templates/html/lti-dl/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/templates/html/lti-dl/dl_response_error.html
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/templates/html/lti-dl/dl_response_saved.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/templates/html/lti-dl/render_dl_content.html
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/templates/html/lti-dl/render_html.html
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/templates/html/lti-dl/render_image.html
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/templates/html/lti-dl/render_link.html
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/templates/html/lti-dl/render_lti_resource_link.html
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/templates/html/lti_1p3_launch.html
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/templates/html/lti_1p3_permission_error.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/templates/html/lti_1p3_studio.html
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/templates/html/lti_iframe.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/templates/html/lti_launch.html
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/templates/html/lti_launch_error.html
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/templates/html/lti_proctoring_start_error.html
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/templates/html/lti_start_assessment.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/templates/html/student.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.768395 lti-consumer-xblock-9.8.3/lti_consumer/templates/xml/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/templates/xml/outcome_service_response.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.768395 lti-consumer-xblock-9.8.3/lti_consumer/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/templatetags/get_dl_lti_launch_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/templatetags/lti_sanitize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.768395 lti-consumer-xblock-9.8.3/lti_consumer/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.772395 lti-consumer-xblock-9.8.3/lti_consumer/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.772395 lti-consumer-xblock-9.8.3/lti_consumer/tests/unit/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/tests/unit/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11960 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/tests/unit/plugin/test_proctoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33526 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/tests/unit/plugin/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38579 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/tests/unit/plugin/test_views_lti_ags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26203 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10559 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28029 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/tests/unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/tests/unit/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91837 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/tests/unit/test_lti_xblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29276 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/tests/unit/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16718 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/tests/unit/test_outcomes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/tests/unit/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6028 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/track.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.772395 lti-consumer-xblock-9.8.3/lti_consumer/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.748395 lti-consumer-xblock-9.8.3/lti_consumer/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.772395 lti-consumer-xblock-9.8.3/lti_consumer/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    10252 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/translations/ar/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    22143 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/translations/ar/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/translations/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.748395 lti-consumer-xblock-9.8.3/lti_consumer/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.772395 lti-consumer-xblock-9.8.3/lti_consumer/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/translations/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    16396 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/translations/en/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/translations/en/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    16396 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/translations/en/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.748395 lti-consumer-xblock-9.8.3/lti_consumer/translations/es_419/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.772395 lti-consumer-xblock-9.8.3/lti_consumer/translations/es_419/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    20799 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/translations/es_419/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    26467 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/translations/es_419/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.748395 lti-consumer-xblock-9.8.3/lti_consumer/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.776395 lti-consumer-xblock-9.8.3/lti_consumer/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18761 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/translations/fr/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    25340 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/translations/fr/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.748395 lti-consumer-xblock-9.8.3/lti_consumer/translations/fr_CA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.776395 lti-consumer-xblock-9.8.3/lti_consumer/translations/fr_CA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     9166 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10186 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/translations/fr_CA/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.748395 lti-consumer-xblock-9.8.3/lti_consumer/translations/he/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.776395 lti-consumer-xblock-9.8.3/lti_consumer/translations/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     9608 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/translations/he/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    21499 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/translations/he/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.748395 lti-consumer-xblock-9.8.3/lti_consumer/translations/hi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.776395 lti-consumer-xblock-9.8.3/lti_consumer/translations/hi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/translations/hi/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    16407 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/translations/hi/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.748395 lti-consumer-xblock-9.8.3/lti_consumer/translations/ja_JP/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.776395 lti-consumer-xblock-9.8.3/lti_consumer/translations/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    21266 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.748395 lti-consumer-xblock-9.8.3/lti_consumer/translations/ko_KR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.776395 lti-consumer-xblock-9.8.3/lti_consumer/translations/ko_KR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/translations/ko_KR/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    16477 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/translations/ko_KR/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.748395 lti-consumer-xblock-9.8.3/lti_consumer/translations/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.776395 lti-consumer-xblock-9.8.3/lti_consumer/translations/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    16884 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/translations/pt_BR/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.748395 lti-consumer-xblock-9.8.3/lti_consumer/translations/pt_PT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.776395 lti-consumer-xblock-9.8.3/lti_consumer/translations/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    23772 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    27799 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.748395 lti-consumer-xblock-9.8.3/lti_consumer/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.776395 lti-consumer-xblock-9.8.3/lti_consumer/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/translations/ru/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    16547 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/translations/ru/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/translations/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.748395 lti-consumer-xblock-9.8.3/lti_consumer/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.776395 lti-consumer-xblock-9.8.3/lti_consumer/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/translations/zh_CN/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    16458 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/translations/zh_CN/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (127)    11729 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/lti_consumer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.780395 lti-consumer-xblock-9.8.3/lti_consumer_xblock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16103 2024-01-23 16:47:55.000000 lti-consumer-xblock-9.8.3/lti_consumer_xblock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7644 2024-01-23 16:47:55.000000 lti-consumer-xblock-9.8.3/lti_consumer_xblock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-01-23 16:47:55.000000 lti-consumer-xblock-9.8.3/lti_consumer_xblock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-01-23 16:47:55.000000 lti-consumer-xblock-9.8.3/lti_consumer_xblock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-01-23 16:47:55.000000 lti-consumer-xblock-9.8.3/lti_consumer_xblock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-23 16:47:55.000000 lti-consumer-xblock-9.8.3/lti_consumer_xblock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 16:47:55.780395 lti-consumer-xblock-9.8.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-01-23 16:47:55.780395 lti-consumer-xblock-9.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-01-23 16:47:49.000000 lti-consumer-xblock-9.8.3/setup.py
```

### Comparing `lti-consumer-xblock-9.8.2/LICENSE` & `lti-consumer-xblock-9.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/NOTICE` & `lti-consumer-xblock-9.8.3/NOTICE`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/PKG-INFO` & `lti-consumer-xblock-9.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lti-consumer-xblock
-Version: 9.8.2
+Version: 9.8.3
 Summary: This XBlock implements the consumer side of the LTI specification.
 Home-page: https://github.com/openedx/xblock-lti-consumer
 Author: Open edX project
 Author-email: oscm@edx.org
 Keywords: lti consumer xblock
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
```

### Comparing `lti-consumer-xblock-9.8.2/README.rst` & `lti-consumer-xblock-9.8.3/README.rst`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/admin.py` & `lti-consumer-xblock-9.8.3/lti_consumer/admin.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/api.py` & `lti-consumer-xblock-9.8.3/lti_consumer/api.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/apps.py` & `lti-consumer-xblock-9.8.3/lti_consumer/apps.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/data.py` & `lti-consumer-xblock-9.8.3/lti_consumer/data.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/filters.py` & `lti-consumer-xblock-9.8.3/lti_consumer/filters.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/forms.py` & `lti-consumer-xblock-9.8.3/lti_consumer/forms.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/lti_1p1/consumer.py` & `lti-consumer-xblock-9.8.3/lti_consumer/lti_1p1/consumer.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/lti_1p1/contrib/django.py` & `lti-consumer-xblock-9.8.3/lti_consumer/lti_1p1/contrib/django.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/lti_1p1/contrib/tests/test_django.py` & `lti-consumer-xblock-9.8.3/lti_consumer/lti_1p1/contrib/tests/test_django.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/lti_1p1/oauth.py` & `lti-consumer-xblock-9.8.3/lti_consumer/lti_1p1/oauth.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/lti_1p1/tests/test_consumer.py` & `lti-consumer-xblock-9.8.3/lti_consumer/lti_1p1/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/lti_1p1/tests/test_oauth.py` & `lti-consumer-xblock-9.8.3/lti_consumer/lti_1p1/tests/test_oauth.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/ags.py` & `lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/ags.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/constants.py` & `lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/constants.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/consumer.py` & `lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/consumer.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
 
 class LtiConsumer1p3:
     """
     LTI 1.3 Consumer Implementation
     """
 
+    @function_trace('lti_consumer.lti_1p3.consumer.LtiConsumer1p3.__init__')
     def __init__(
             self,
             iss,
             lti_oidc_url,
             lti_launch_url,
             client_id,
             deployment_id,
```

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/deep_linking.py` & `lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/deep_linking.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/exceptions.py` & `lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/exceptions.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py` & `lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py` & `lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py` & `lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py` & `lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py` & `lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/extensions/rest_framework/utils.py` & `lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/extensions/rest_framework/utils.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/key_handlers.py` & `lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/key_handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import codecs
 import copy
 import time
 import json
 import logging
 
 from Cryptodome.PublicKey import RSA
+from edx_django_utils.monitoring import function_trace
 from jwkest import BadSignature, BadSyntax, WrongNumberOfParts, jwk
 from jwkest.jwk import RSAKey, load_jwks_from_url
 from jwkest.jws import JWS, NoSuitableSigningKeys, UnknownAlgorithm
 from jwkest.jwt import JWT
 
 from . import exceptions
 
@@ -28,14 +29,15 @@
     Uses a tool public keys or keysets URL to retrieve
     a key and validate a message sent by the tool.
 
     This is primarily used by the Access Token endpoint
     in order to validate the JWT Signature of messages
     signed with the tools signature.
     """
+    @function_trace('lti_consumer.key_handlers.ToolKeyHandler.__init__')
     def __init__(self, public_key=None, keyset_url=None):
         """
         Instance message validator
 
         Import a public key from the tool by either using a keyset url
         or a combination of public key + key id.
 
@@ -158,14 +160,15 @@
 class PlatformKeyHandler:
     """
     Platform RSA Key handler.
 
     This class loads the platform key and is responsible for
     encoding JWT messages and exporting public keys.
     """
+    @function_trace('lti_consumer.key_handlers.PlatformKeyHandler.__init__')
     def __init__(self, key_pem, kid=None):
         """
         Import Key when instancing class if a key is present.
         """
         self.key = None
 
         if key_pem:
```

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/nprs.py` & `lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/nprs.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py` & `lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py` & `lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/tests/test_ags.py` & `lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/tests/test_ags.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/tests/test_consumer.py` & `lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/tests/test_deep_linking.py` & `lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/tests/test_deep_linking.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/tests/test_key_handlers.py` & `lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/tests/test_key_handlers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/lti_1p3/tests/test_nrps.py` & `lti-consumer-xblock-9.8.3/lti_consumer/lti_1p3/tests/test_nrps.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/lti_xblock.py` & `lti-consumer-xblock-9.8.3/lti_consumer/lti_xblock.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/migrations/0001_initial.py` & `lti-consumer-xblock-9.8.3/lti_consumer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/migrations/0002_ltiagslineitem.py` & `lti-consumer-xblock-9.8.3/lti_consumer/migrations/0002_ltiagslineitem.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/migrations/0003_ltiagsscore.py` & `lti-consumer-xblock-9.8.3/lti_consumer/migrations/0003_ltiagsscore.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/migrations/0004_keyset_mgmt_to_model.py` & `lti-consumer-xblock-9.8.3/lti_consumer/migrations/0004_keyset_mgmt_to_model.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/migrations/0005_migrate_keyset_to_model.py` & `lti-consumer-xblock-9.8.3/lti_consumer/migrations/0005_migrate_keyset_to_model.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py` & `lti-consumer-xblock-9.8.3/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/migrations/0007_ltidlcontentitem.py` & `lti-consumer-xblock-9.8.3/lti_consumer/migrations/0007_ltidlcontentitem.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/migrations/0008_fix_uuid_backfill.py` & `lti-consumer-xblock-9.8.3/lti_consumer/migrations/0008_fix_uuid_backfill.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/migrations/0009_backfill-empty-string-config-id.py` & `lti-consumer-xblock-9.8.3/lti_consumer/migrations/0009_backfill-empty-string-config-id.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py` & `lti-consumer-xblock-9.8.3/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py` & `lti-consumer-xblock-9.8.3/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/migrations/0013_auto_20210712_1352.py` & `lti-consumer-xblock-9.8.3/lti_consumer/migrations/0013_auto_20210712_1352.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/migrations/0014_adds_external_id.py` & `lti-consumer-xblock-9.8.3/lti_consumer/migrations/0014_adds_external_id.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/migrations/0015_add_additional_1p3_fields.py` & `lti-consumer-xblock-9.8.3/lti_consumer/migrations/0015_add_additional_1p3_fields.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py` & `lti-consumer-xblock-9.8.3/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py` & `lti-consumer-xblock-9.8.3/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/models.py` & `lti-consumer-xblock-9.8.3/lti_consumer/models.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/outcomes.py` & `lti-consumer-xblock-9.8.3/lti_consumer/outcomes.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/plugin/compat.py` & `lti-consumer-xblock-9.8.3/lti_consumer/plugin/compat.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/plugin/urls.py` & `lti-consumer-xblock-9.8.3/lti_consumer/plugin/urls.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/plugin/views.py` & `lti-consumer-xblock-9.8.3/lti_consumer/plugin/views.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/ar/text.js` & `lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/ar/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/en/text.js` & `lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/en/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/es_419/text.js` & `lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/es_419/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/fr/text.js` & `lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/fr/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/he/text.js` & `lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/he/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/hi/text.js` & `lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/hi/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/it/text.js` & `lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/it/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/ja/text.js` & `lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/ja/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/ko/text.js` & `lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/ko/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/pt_BR/text.js` & `lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/pt_BR/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/pt_PT/text.js` & `lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/pt_PT/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/ru/text.js` & `lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/ru/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/public/js/translations/zh_CN/text.js` & `lti-consumer-xblock-9.8.3/lti_consumer/public/js/translations/zh_CN/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/signals/signals.py` & `lti-consumer-xblock-9.8.3/lti_consumer/signals/signals.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/static/css/student.css` & `lti-consumer-xblock-9.8.3/lti_consumer/static/css/student.css`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/static/js/xblock_lti_consumer.js` & `lti-consumer-xblock-9.8.3/lti_consumer/static/js/xblock_lti_consumer.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/static/js/xblock_studio_view.js` & `lti-consumer-xblock-9.8.3/lti_consumer/static/js/xblock_studio_view.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/static/sass/student.scss` & `lti-consumer-xblock-9.8.3/lti_consumer/static/sass/student.scss`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/templates/html/lti-dl/render_dl_content.html` & `lti-consumer-xblock-9.8.3/lti_consumer/templates/html/lti-dl/render_dl_content.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/templates/html/lti-dl/render_image.html` & `lti-consumer-xblock-9.8.3/lti_consumer/templates/html/lti-dl/render_image.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/templates/html/lti-dl/render_link.html` & `lti-consumer-xblock-9.8.3/lti_consumer/templates/html/lti-dl/render_link.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/templates/html/lti_1p3_launch.html` & `lti-consumer-xblock-9.8.3/lti_consumer/templates/html/lti_1p3_launch.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/templates/html/lti_1p3_studio.html` & `lti-consumer-xblock-9.8.3/lti_consumer/templates/html/lti_1p3_studio.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/templates/html/lti_launch.html` & `lti-consumer-xblock-9.8.3/lti_consumer/templates/html/lti_launch.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/templates/html/student.html` & `lti-consumer-xblock-9.8.3/lti_consumer/templates/html/student.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/templates/xml/outcome_service_response.xml` & `lti-consumer-xblock-9.8.3/lti_consumer/templates/xml/outcome_service_response.xml`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/templatetags/get_dl_lti_launch_url.py` & `lti-consumer-xblock-9.8.3/lti_consumer/templatetags/get_dl_lti_launch_url.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/templatetags/lti_sanitize.py` & `lti-consumer-xblock-9.8.3/lti_consumer/templatetags/lti_sanitize.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/tests/test_utils.py` & `lti-consumer-xblock-9.8.3/lti_consumer/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/tests/unit/plugin/test_proctoring.py` & `lti-consumer-xblock-9.8.3/lti_consumer/tests/unit/plugin/test_proctoring.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/tests/unit/plugin/test_views.py` & `lti-consumer-xblock-9.8.3/lti_consumer/tests/unit/plugin/test_views.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/tests/unit/plugin/test_views_lti_ags.py` & `lti-consumer-xblock-9.8.3/lti_consumer/tests/unit/plugin/test_views_lti_ags.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py` & `lti-consumer-xblock-9.8.3/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py` & `lti-consumer-xblock-9.8.3/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/tests/unit/test_api.py` & `lti-consumer-xblock-9.8.3/lti_consumer/tests/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/tests/unit/test_filters.py` & `lti-consumer-xblock-9.8.3/lti_consumer/tests/unit/test_filters.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/tests/unit/test_lti_xblock.py` & `lti-consumer-xblock-9.8.3/lti_consumer/tests/unit/test_lti_xblock.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/tests/unit/test_models.py` & `lti-consumer-xblock-9.8.3/lti_consumer/tests/unit/test_models.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/tests/unit/test_outcomes.py` & `lti-consumer-xblock-9.8.3/lti_consumer/tests/unit/test_outcomes.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/tests/unit/test_signals.py` & `lti-consumer-xblock-9.8.3/lti_consumer/tests/unit/test_signals.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/tests/unit/test_utils.py` & `lti-consumer-xblock-9.8.3/lti_consumer/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/translations/ar/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.8.3/lti_consumer/translations/ar/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/translations/ar/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.8.3/lti_consumer/translations/ar/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/translations/config.yaml` & `lti-consumer-xblock-9.8.3/lti_consumer/translations/config.yaml`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/translations/en/LC_MESSAGES/django.po` & `lti-consumer-xblock-9.8.3/lti_consumer/translations/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/translations/en/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.8.3/lti_consumer/translations/en/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/translations/es_419/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.8.3/lti_consumer/translations/es_419/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/translations/es_419/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.8.3/lti_consumer/translations/es_419/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/translations/fr/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.8.3/lti_consumer/translations/fr/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/translations/fr/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.8.3/lti_consumer/translations/fr/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.8.3/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/translations/fr_CA/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.8.3/lti_consumer/translations/fr_CA/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/translations/he/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.8.3/lti_consumer/translations/he/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/translations/he/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.8.3/lti_consumer/translations/he/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/translations/hi/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.8.3/lti_consumer/translations/hi/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.8.3/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.8.3/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/translations/ko_KR/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.8.3/lti_consumer/translations/ko_KR/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.8.3/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/translations/pt_BR/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.8.3/lti_consumer/translations/pt_BR/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.8.3/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.8.3/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/translations/ru/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.8.3/lti_consumer/translations/ru/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/translations/ru/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.8.3/lti_consumer/translations/ru/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/translations/settings.py` & `lti-consumer-xblock-9.8.3/lti_consumer/translations/settings.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/translations/zh_CN/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.8.3/lti_consumer/translations/zh_CN/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer/utils.py` & `lti-consumer-xblock-9.8.3/lti_consumer/utils.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer_xblock.egg-info/PKG-INFO` & `lti-consumer-xblock-9.8.3/lti_consumer_xblock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lti-consumer-xblock
-Version: 9.8.2
+Version: 9.8.3
 Summary: This XBlock implements the consumer side of the LTI specification.
 Home-page: https://github.com/openedx/xblock-lti-consumer
 Author: Open edX project
 Author-email: oscm@edx.org
 Keywords: lti consumer xblock
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
```

### Comparing `lti-consumer-xblock-9.8.2/lti_consumer_xblock.egg-info/SOURCES.txt` & `lti-consumer-xblock-9.8.3/lti_consumer_xblock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/requirements/constraints.txt` & `lti-consumer-xblock-9.8.3/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.8.2/setup.py` & `lti-consumer-xblock-9.8.3/setup.py`

 * *Files identical despite different names*

