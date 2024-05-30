# Comparing `tmp/document_merge_service-6.4.5.tar.gz` & `tmp/document_merge_service-6.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "document_merge_service-6.4.5.tar", max compression
+gzip compressed data, was "document_merge_service-6.5.0.tar", max compression
```

## Comparing `document_merge_service-6.4.5.tar` & `document_merge_service-6.5.0.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0        0        0    13469 2024-04-25 13:27:33.149890 document_merge_service-6.4.5/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2024-04-25 13:27:33.149890 document_merge_service-6.4.5/LICENSE
--rw-r--r--   0        0        0     2522 2024-04-25 13:27:33.149890 document_merge_service-6.4.5/README.md
--rw-r--r--   0        0        0        0 2024-04-25 13:27:33.149890 document_merge_service-6.4.5/document_merge_service/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 13:27:33.149890 document_merge_service-6.4.5/document_merge_service/api/__init__.py
--rw-r--r--   0        0        0      405 2024-04-25 13:27:33.149890 document_merge_service-6.4.5/document_merge_service/api/apps.py
--rw-r--r--   0        0        0     3232 2024-04-25 13:27:33.149890 document_merge_service-6.4.5/document_merge_service/api/authentication.py
--rw-r--r--   0        0        0     5490 2024-04-25 13:27:33.149890 document_merge_service-6.4.5/document_merge_service/api/data/2023.test.test.docx-template.docx
--rw-r--r--   0        0        0      580 2024-04-25 13:27:33.149890 document_merge_service-6.4.5/document_merge_service/api/data/__init__.py
--rw-r--r--   0        0        0      559 2024-04-25 13:27:33.149890 document_merge_service-6.4.5/document_merge_service/api/data/black.png
--rw-r--r--   0        0        0     9125 2024-04-25 13:27:33.149890 document_merge_service-6.4.5/document_merge_service/api/data/docx-mailmerge-syntax.docx
--rw-r--r--   0        0        0    11489 2024-04-25 13:27:33.149890 document_merge_service-6.4.5/document_merge_service/api/data/docx-mailmerge.docx
--rw-r--r--   0        0        0     5735 2024-04-25 13:27:33.149890 document_merge_service-6.4.5/document_merge_service/api/data/docx-template-filters.docx
--rw-r--r--   0        0        0     7335 2024-04-25 13:27:33.149890 document_merge_service-6.4.5/document_merge_service/api/data/docx-template-image-placeholder-header-footer.docx
--rw-r--r--   0        0        0     6087 2024-04-25 13:27:33.149890 document_merge_service-6.4.5/document_merge_service/api/data/docx-template-loopcontrols.docx
--rw-r--r--   0        0        0     5952 2024-04-25 13:27:33.153890 document_merge_service-6.4.5/document_merge_service/api/data/docx-template-placeholdercheck.docx
--rw-r--r--   0        0        0     5091 2024-04-25 13:27:33.153890 document_merge_service-6.4.5/document_merge_service/api/data/docx-template-syntax.docx
--rw-r--r--   0        0        0     5490 2024-04-25 13:27:33.153890 document_merge_service-6.4.5/document_merge_service/api/data/docx-template.docx
--rw-r--r--   0        0        0     4750 2024-04-25 13:27:33.153890 document_merge_service-6.4.5/document_merge_service/api/data/invalid-template.xlsx
--rw-r--r--   0        0        0  1127936 2024-04-25 13:27:33.153890 document_merge_service-6.4.5/document_merge_service/api/data/loadtest/1.doc
--rw-r--r--   0        0        0   175922 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/data/loadtest/2.docx
--rw-r--r--   0        0        0   163307 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/data/loadtest/3.docx
--rw-r--r--   0        0        0   141498 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/data/loadtest/4.docx
--rw-r--r--   0        0        0    10589 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/data/odt-template.odt
--rw-r--r--   0        0        0       22 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/data/test.txt
--rw-r--r--   0        0        0        5 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/data/xlsx-not-valid.xlsx
--rw-r--r--   0        0        0     6467 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/data/xlsx-structure.xlsx
--rw-r--r--   0        0        0     6432 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/data/xlsx-syntax.xlsx
--rw-r--r--   0        0        0     4750 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/data/xlsx-template.xlsx
--rw-r--r--   0        0        0    10586 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/engines.py
--rw-r--r--   0        0        0      389 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/factories.py
--rw-r--r--   0        0        0      815 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/file_converter.py
--rw-r--r--   0        0        0     2841 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/filters.py
--rw-r--r--   0        0        0     2546 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/jinja.py
--rw-r--r--   0        0        0        0 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/management/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/management/commands/__init__.py
--rw-r--r--   0        0        0     1628 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/management/commands/clean_dangling_files.py
--rw-r--r--   0        0        0     2252 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/management/commands/upload_local_templates.py
--rw-r--r--   0        0        0     1248 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/migrations/0001_initial.py
--rw-r--r--   0        0        0      488 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/migrations/0002_template_group.py
--rw-r--r--   0        0        0      374 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/migrations/0003_template_meta.py
--rw-r--r--   0        0        0      145 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/migrations/0004_cleanup_files.py
--rw-r--r--   0        0        0     1004 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/migrations/0005_xlsx_template_engine.py
--rw-r--r--   0        0        0      932 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/migrations/0006_remove_template_group.py
--rw-r--r--   0        0        0        0 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/migrations/__init__.py
--rw-r--r--   0        0        0     1845 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/models.py
--rw-r--r--   0        0        0      231 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/pagination.py
--rw-r--r--   0        0        0      289 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/permissions.py
--rw-r--r--   0        0        0     4995 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/serializers.py
--rw-r--r--   0        0        0        0 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/tests/__init__.py
--rw-r--r--   0        0        0    30689 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/tests/__snapshots__/test_template.ambr
--rw-r--r--   0        0        0     2357 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/tests/test_authentication.py
--rw-r--r--   0        0        0      942 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/tests/test_clean_dangling_files.py
--rw-r--r--   0        0        0     1446 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/tests/test_convert.py
--rw-r--r--   0        0        0     1963 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/tests/test_excel.py
--rw-r--r--   0        0        0     1372 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/tests/test_filters.py
--rw-r--r--   0        0        0     1300 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/tests/test_jinja.py
--rw-r--r--   0        0        0      749 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/tests/test_pagination.py
--rw-r--r--   0        0        0    25891 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/tests/test_template.py
--rw-r--r--   0        0        0     3425 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/tests/test_unoconv.py
--rw-r--r--   0        0        0     1712 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/tests/test_upload_local_templates.py
--rw-r--r--   0        0        0     6947 2024-04-25 13:27:33.157890 document_merge_service-6.4.5/document_merge_service/api/unoconv.py
--rw-r--r--   0        0        0      460 2024-04-25 13:27:33.161890 document_merge_service-6.4.5/document_merge_service/api/urls.py
--rw-r--r--   0        0        0     3797 2024-04-25 13:27:33.161890 document_merge_service-6.4.5/document_merge_service/api/views.py
--rw-r--r--   0        0        0     2909 2024-04-25 13:27:33.161890 document_merge_service-6.4.5/document_merge_service/conftest.py
--rw-r--r--   0        0        0        0 2024-04-25 13:27:33.161890 document_merge_service-6.4.5/document_merge_service/extensions/__init__.py
--rw-r--r--   0        0        0       52 2024-04-25 13:27:33.161890 document_merge_service-6.4.5/document_merge_service/extensions/permissions.py
--rw-r--r--   0        0        0       52 2024-04-25 13:27:33.161890 document_merge_service-6.4.5/document_merge_service/extensions/visibilities.py
--rw-r--r--   0        0        0      789 2024-04-25 13:27:33.161890 document_merge_service-6.4.5/document_merge_service/sentry.py
--rw-r--r--   0        0        0     9052 2024-04-25 13:27:33.161890 document_merge_service-6.4.5/document_merge_service/settings.py
--rw-r--r--   0        0        0        0 2024-04-25 13:27:33.161890 document_merge_service-6.4.5/document_merge_service/tests/__init__.py
--rw-r--r--   0        0        0      434 2024-04-25 13:27:33.161890 document_merge_service-6.4.5/document_merge_service/tests/test_sentry.py
--rw-r--r--   0        0        0      615 2024-04-25 13:27:33.161890 document_merge_service-6.4.5/document_merge_service/tests/test_settings.py
--rw-r--r--   0        0        0      225 2024-04-25 13:27:33.161890 document_merge_service-6.4.5/document_merge_service/urls.py
--rw-r--r--   0        0        0      412 2024-04-25 13:27:33.161890 document_merge_service-6.4.5/document_merge_service/wsgi.py
--rw-r--r--   0        0        0     3594 2024-04-25 13:27:33.161890 document_merge_service-6.4.5/pyproject.toml
--rw-r--r--   0        0        0     4555 1970-01-01 00:00:00.000000 document_merge_service-6.4.5/PKG-INFO
+-rw-r--r--   0        0        0    14122 2024-05-30 12:01:47.360634 document_merge_service-6.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2024-05-30 12:01:47.360634 document_merge_service-6.5.0/LICENSE
+-rw-r--r--   0        0        0     2522 2024-05-30 12:01:47.360634 document_merge_service-6.5.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-30 12:01:47.360634 document_merge_service-6.5.0/document_merge_service/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 12:01:47.360634 document_merge_service-6.5.0/document_merge_service/api/__init__.py
+-rw-r--r--   0        0        0      405 2024-05-30 12:01:47.360634 document_merge_service-6.5.0/document_merge_service/api/apps.py
+-rw-r--r--   0        0        0     3232 2024-05-30 12:01:47.360634 document_merge_service-6.5.0/document_merge_service/api/authentication.py
+-rw-r--r--   0        0        0     5490 2024-05-30 12:01:47.360634 document_merge_service-6.5.0/document_merge_service/api/data/2023.test.test.docx-template.docx
+-rw-r--r--   0        0        0      580 2024-05-30 12:01:47.360634 document_merge_service-6.5.0/document_merge_service/api/data/__init__.py
+-rw-r--r--   0        0        0      559 2024-05-30 12:01:47.360634 document_merge_service-6.5.0/document_merge_service/api/data/black.png
+-rw-r--r--   0        0        0     9125 2024-05-30 12:01:47.360634 document_merge_service-6.5.0/document_merge_service/api/data/docx-mailmerge-syntax.docx
+-rw-r--r--   0        0        0    11489 2024-05-30 12:01:47.360634 document_merge_service-6.5.0/document_merge_service/api/data/docx-mailmerge.docx
+-rw-r--r--   0        0        0     5735 2024-05-30 12:01:47.360634 document_merge_service-6.5.0/document_merge_service/api/data/docx-template-filters.docx
+-rw-r--r--   0        0        0     7335 2024-05-30 12:01:47.360634 document_merge_service-6.5.0/document_merge_service/api/data/docx-template-image-placeholder-header-footer.docx
+-rw-r--r--   0        0        0     6087 2024-05-30 12:01:47.360634 document_merge_service-6.5.0/document_merge_service/api/data/docx-template-loopcontrols.docx
+-rw-r--r--   0        0        0     5952 2024-05-30 12:01:47.360634 document_merge_service-6.5.0/document_merge_service/api/data/docx-template-placeholdercheck.docx
+-rw-r--r--   0        0        0     5091 2024-05-30 12:01:47.360634 document_merge_service-6.5.0/document_merge_service/api/data/docx-template-syntax.docx
+-rw-r--r--   0        0        0     5490 2024-05-30 12:01:47.360634 document_merge_service-6.5.0/document_merge_service/api/data/docx-template.docx
+-rw-r--r--   0        0        0     4750 2024-05-30 12:01:47.360634 document_merge_service-6.5.0/document_merge_service/api/data/invalid-template.xlsx
+-rw-r--r--   0        0        0  1127936 2024-05-30 12:01:47.368634 document_merge_service-6.5.0/document_merge_service/api/data/loadtest/1.doc
+-rw-r--r--   0        0        0   175922 2024-05-30 12:01:47.368634 document_merge_service-6.5.0/document_merge_service/api/data/loadtest/2.docx
+-rw-r--r--   0        0        0   163307 2024-05-30 12:01:47.368634 document_merge_service-6.5.0/document_merge_service/api/data/loadtest/3.docx
+-rw-r--r--   0        0        0   141498 2024-05-30 12:01:47.368634 document_merge_service-6.5.0/document_merge_service/api/data/loadtest/4.docx
+-rw-r--r--   0        0        0    10589 2024-05-30 12:01:47.368634 document_merge_service-6.5.0/document_merge_service/api/data/odt-template.odt
+-rw-r--r--   0        0        0       22 2024-05-30 12:01:47.368634 document_merge_service-6.5.0/document_merge_service/api/data/test.txt
+-rw-r--r--   0        0        0        5 2024-05-30 12:01:47.368634 document_merge_service-6.5.0/document_merge_service/api/data/xlsx-not-valid.xlsx
+-rw-r--r--   0        0        0     6467 2024-05-30 12:01:47.368634 document_merge_service-6.5.0/document_merge_service/api/data/xlsx-structure.xlsx
+-rw-r--r--   0        0        0     6432 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/data/xlsx-syntax.xlsx
+-rw-r--r--   0        0        0     4750 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/data/xlsx-template.xlsx
+-rw-r--r--   0        0        0    10586 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/engines.py
+-rw-r--r--   0        0        0      389 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/factories.py
+-rw-r--r--   0        0        0      815 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/file_converter.py
+-rw-r--r--   0        0        0     3013 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/filters.py
+-rw-r--r--   0        0        0     2546 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/jinja.py
+-rw-r--r--   0        0        0        0 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/management/commands/__init__.py
+-rw-r--r--   0        0        0     1628 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/management/commands/clean_dangling_files.py
+-rw-r--r--   0        0        0     2252 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/management/commands/upload_local_templates.py
+-rw-r--r--   0        0        0     1248 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/migrations/0001_initial.py
+-rw-r--r--   0        0        0      488 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/migrations/0002_template_group.py
+-rw-r--r--   0        0        0      374 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/migrations/0003_template_meta.py
+-rw-r--r--   0        0        0      145 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/migrations/0004_cleanup_files.py
+-rw-r--r--   0        0        0     1004 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/migrations/0005_xlsx_template_engine.py
+-rw-r--r--   0        0        0      932 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/migrations/0006_remove_template_group.py
+-rw-r--r--   0        0        0        0 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/migrations/__init__.py
+-rw-r--r--   0        0        0     1845 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/models.py
+-rw-r--r--   0        0        0      231 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/pagination.py
+-rw-r--r--   0        0        0      289 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/permissions.py
+-rw-r--r--   0        0        0     4995 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/serializers.py
+-rw-r--r--   0        0        0        0 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/tests/__init__.py
+-rw-r--r--   0        0        0    30689 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/tests/__snapshots__/test_template.ambr
+-rw-r--r--   0        0        0     2357 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/tests/test_authentication.py
+-rw-r--r--   0        0        0      942 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/tests/test_clean_dangling_files.py
+-rw-r--r--   0        0        0     1446 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/tests/test_convert.py
+-rw-r--r--   0        0        0     1963 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/tests/test_excel.py
+-rw-r--r--   0        0        0     1372 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/tests/test_filters.py
+-rw-r--r--   0        0        0     1300 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/tests/test_jinja.py
+-rw-r--r--   0        0        0      749 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/tests/test_pagination.py
+-rw-r--r--   0        0        0    25891 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/tests/test_template.py
+-rw-r--r--   0        0        0     3425 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/tests/test_unoconv.py
+-rw-r--r--   0        0        0     1712 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/tests/test_upload_local_templates.py
+-rw-r--r--   0        0        0     6947 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/unoconv.py
+-rw-r--r--   0        0        0      460 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/urls.py
+-rw-r--r--   0        0        0     3797 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/api/views.py
+-rw-r--r--   0        0        0     2909 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/conftest.py
+-rw-r--r--   0        0        0        0 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/extensions/__init__.py
+-rw-r--r--   0        0        0       52 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/extensions/permissions.py
+-rw-r--r--   0        0        0       52 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/extensions/visibilities.py
+-rw-r--r--   0        0        0      789 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/sentry.py
+-rw-r--r--   0        0        0     9066 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/settings.py
+-rw-r--r--   0        0        0        0 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/tests/__init__.py
+-rw-r--r--   0        0        0      434 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/tests/test_sentry.py
+-rw-r--r--   0        0        0      615 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/tests/test_settings.py
+-rw-r--r--   0        0        0      197 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/urls.py
+-rw-r--r--   0        0        0      412 2024-05-30 12:01:47.372634 document_merge_service-6.5.0/document_merge_service/wsgi.py
+-rw-r--r--   0        0        0     4007 2024-05-30 12:01:47.376634 document_merge_service-6.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4628 1970-01-01 00:00:00.000000 document_merge_service-6.5.0/PKG-INFO
```

### Comparing `document_merge_service-6.4.5/CHANGELOG.md` & `document_merge_service-6.5.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,20 @@
 # Changelog
 
+## 6.5.0 (30 May 2024)
+### Feature
+
+* **docker:** Update python to v3.12 ([`14c4d7f`](https://github.com/adfinis/document-merge-service/commit/14c4d7f97005ce9651be6dc37eae904125614e29))
+* **deps:** Update dependencies ([`5773d5c`](https://github.com/adfinis/document-merge-service/commit/5773d5c5283543c843c4986daf8b71cc1cafa611))
+* **deps:** Update django to v4.2 LTS ([`5287a3e`](https://github.com/adfinis/document-merge-service/commit/5287a3e4a6b26c12e122026f789e80d2c70f892b))
+
+### Fix
+
+* **docker:** Install dependencies as dms user ([`6a17a8f`](https://github.com/adfinis/document-merge-service/commit/6a17a8f1cfce053440790e9b62a7d6c21405f580))
+
 ## 6.4.5 (25 April 2024)
 ### Fix
 * **image:** Fix template validation with images in headers / footers ([`eccbb34`](https://github.com/adfinis/document-merge-service/commit/eccbb34ce69cd26a998a8ef15db109e8faf2a1e3))
 
 ## 6.4.4 (24 January 2024)
 ### Fix
 * **settings:** Add s3 ssl settings ([#698](https://github.com/adfinis/document-merge-service/issues/698)) ([`c92b381`](https://github.com/adfinis/document-merge-service/commit/c92b381ce6ebc45c0b96eba828b471f2bd28a169))
```

### Comparing `document_merge_service-6.4.5/LICENSE` & `document_merge_service-6.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/README.md` & `document_merge_service-6.5.0/README.md`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/authentication.py` & `document_merge_service-6.5.0/document_merge_service/api/authentication.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/data/2023.test.test.docx-template.docx` & `document_merge_service-6.5.0/document_merge_service/api/data/2023.test.test.docx-template.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/data/__init__.py` & `document_merge_service-6.5.0/document_merge_service/api/data/__init__.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/data/black.png` & `document_merge_service-6.5.0/document_merge_service/api/data/black.png`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/data/docx-mailmerge-syntax.docx` & `document_merge_service-6.5.0/document_merge_service/api/data/docx-mailmerge-syntax.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/data/docx-mailmerge.docx` & `document_merge_service-6.5.0/document_merge_service/api/data/docx-mailmerge.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/data/docx-template-filters.docx` & `document_merge_service-6.5.0/document_merge_service/api/data/docx-template-filters.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/data/docx-template-image-placeholder-header-footer.docx` & `document_merge_service-6.5.0/document_merge_service/api/data/docx-template-image-placeholder-header-footer.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/data/docx-template-loopcontrols.docx` & `document_merge_service-6.5.0/document_merge_service/api/data/docx-template-loopcontrols.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/data/docx-template-placeholdercheck.docx` & `document_merge_service-6.5.0/document_merge_service/api/data/docx-template-placeholdercheck.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/data/docx-template-syntax.docx` & `document_merge_service-6.5.0/document_merge_service/api/data/docx-template-syntax.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/data/docx-template.docx` & `document_merge_service-6.5.0/document_merge_service/api/data/docx-template.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/data/invalid-template.xlsx` & `document_merge_service-6.5.0/document_merge_service/api/data/invalid-template.xlsx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/data/loadtest/1.doc` & `document_merge_service-6.5.0/document_merge_service/api/data/loadtest/1.doc`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/data/loadtest/2.docx` & `document_merge_service-6.5.0/document_merge_service/api/data/loadtest/2.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/data/loadtest/3.docx` & `document_merge_service-6.5.0/document_merge_service/api/data/loadtest/3.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/data/loadtest/4.docx` & `document_merge_service-6.5.0/document_merge_service/api/data/loadtest/4.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/data/odt-template.odt` & `document_merge_service-6.5.0/document_merge_service/api/data/odt-template.odt`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/data/xlsx-structure.xlsx` & `document_merge_service-6.5.0/document_merge_service/api/data/xlsx-structure.xlsx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/data/xlsx-syntax.xlsx` & `document_merge_service-6.5.0/document_merge_service/api/data/xlsx-syntax.xlsx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/data/xlsx-template.xlsx` & `document_merge_service-6.5.0/document_merge_service/api/data/xlsx-template.xlsx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/engines.py` & `document_merge_service-6.5.0/document_merge_service/api/engines.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/file_converter.py` & `document_merge_service-6.5.0/document_merge_service/api/file_converter.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/filters.py` & `document_merge_service-6.5.0/document_merge_service/api/filters.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import json
 
-from django.db.models.fields.json import KeyTextTransform
+from django.db.models.fields import TextField
+from django.db.models.fields.json import KT
+from django.db.models.functions import Cast
 from django_filters import Filter, FilterSet
 from django_filters.constants import EMPTY_VALUES
 from rest_framework.exceptions import ValidationError
 
 from . import models
 
 
@@ -43,15 +45,18 @@
                 )
             # "contains" behaves differently on JSONFields as it does on TextFields.
             # That's why we annotate the queryset with the value.
             # Some discussion about it can be found here:
             # https://code.djangoproject.com/ticket/26511
             if isinstance(expr["value"], str):
                 qs = qs.annotate(
-                    field_val=KeyTextTransform(expr["key"], self.field_name)
+                    field_val=Cast(
+                        KT(f"{self.field_name}__{expr['key']}"),
+                        output_field=TextField(),
+                    )
                 )
                 lookup = {f"field_val__{lookup_expr}": expr["value"]}
             else:
                 lookup = {
                     f"{self.field_name}__{expr['key']}__{lookup_expr}": expr["value"]
                 }
             qs = qs.filter(**lookup)
```

### Comparing `document_merge_service-6.4.5/document_merge_service/api/jinja.py` & `document_merge_service-6.5.0/document_merge_service/api/jinja.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/management/commands/clean_dangling_files.py` & `document_merge_service-6.5.0/document_merge_service/api/management/commands/clean_dangling_files.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/management/commands/upload_local_templates.py` & `document_merge_service-6.5.0/document_merge_service/api/management/commands/upload_local_templates.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/migrations/0001_initial.py` & `document_merge_service-6.5.0/document_merge_service/api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/migrations/0005_xlsx_template_engine.py` & `document_merge_service-6.5.0/document_merge_service/api/migrations/0005_xlsx_template_engine.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/migrations/0006_remove_template_group.py` & `document_merge_service-6.5.0/document_merge_service/api/migrations/0006_remove_template_group.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/models.py` & `document_merge_service-6.5.0/document_merge_service/api/models.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/serializers.py` & `document_merge_service-6.5.0/document_merge_service/api/serializers.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/tests/__snapshots__/test_template.ambr` & `document_merge_service-6.5.0/document_merge_service/api/tests/__snapshots__/test_template.ambr`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/tests/test_authentication.py` & `document_merge_service-6.5.0/document_merge_service/api/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/tests/test_clean_dangling_files.py` & `document_merge_service-6.5.0/document_merge_service/api/tests/test_clean_dangling_files.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/tests/test_convert.py` & `document_merge_service-6.5.0/document_merge_service/api/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/tests/test_excel.py` & `document_merge_service-6.5.0/document_merge_service/api/tests/test_excel.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/tests/test_filters.py` & `document_merge_service-6.5.0/document_merge_service/api/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/tests/test_jinja.py` & `document_merge_service-6.5.0/document_merge_service/api/tests/test_jinja.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/tests/test_pagination.py` & `document_merge_service-6.5.0/document_merge_service/api/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/tests/test_template.py` & `document_merge_service-6.5.0/document_merge_service/api/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/tests/test_unoconv.py` & `document_merge_service-6.5.0/document_merge_service/api/tests/test_unoconv.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/tests/test_upload_local_templates.py` & `document_merge_service-6.5.0/document_merge_service/api/tests/test_upload_local_templates.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/unoconv.py` & `document_merge_service-6.5.0/document_merge_service/api/unoconv.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/api/views.py` & `document_merge_service-6.5.0/document_merge_service/api/views.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/conftest.py` & `document_merge_service-6.5.0/document_merge_service/conftest.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/sentry.py` & `document_merge_service-6.5.0/document_merge_service/sentry.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/document_merge_service/settings.py` & `document_merge_service-6.5.0/document_merge_service/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,17 +54,14 @@
     "rest_framework",
     "django_filters",
     "document_merge_service.api.apps.DefaultConfig",
     "corsheaders",
     "generic_permissions.apps.GenericPermissionsConfig",
 ]
 
-if "postgresql" in DATABASES["default"]["ENGINE"]:  # pragma: no cover
-    INSTALLED_APPS.append("django.contrib.postgres")
-
 MIDDLEWARE = [
     "django.middleware.security.SecurityMiddleware",
     "corsheaders.middleware.CorsMiddleware",
     "django.middleware.common.CommonMiddleware",
     "django.middleware.locale.LocaleMiddleware",
 ]
 
@@ -110,15 +107,14 @@
 
 # Internationalization
 # https://docs.djangoproject.com/en/1.11/topics/i18n/
 
 LANGUAGE_CODE = env.str("LANGUAGE_CODE", "en-us")
 TIME_ZONE = env.str("TIME_ZONE", "UTC")
 USE_I18N = True
-USE_L10N = True
 USE_TZ = True
 
 
 def parse_admins(admins):
     """
     Parse env admins to django admins.
 
@@ -144,17 +140,24 @@
 # https://docs.djangoproject.com/en/1.11/howto/static-files/
 
 STATIC_URL = "/static/"
 STATIC_ROOT = env.str("STATIC_ROOT", None)
 
 # Media files
 
-DEFAULT_FILE_STORAGE = env.str(
-    "FILE_STORAGE", default="django.core.files.storage.FileSystemStorage"
-)
+STORAGES = {
+    "default": {
+        "BACKEND": env.str(
+            "FILE_STORAGE", default="django.core.files.storage.FileSystemStorage"
+        )
+    },
+    "staticfiles": {
+        "BACKEND": "django.contrib.staticfiles.storage.StaticFilesStorage",
+    },
+}
 MEDIA_ROOT = env.str("MEDIA_ROOT", "")
 # TODO: This should be removed in favor of storing the files in a bucket
 # https://code.djangoproject.com/ticket/32991
 MEDIA_URL = env.str("MEDIA_URL", "api/v1/template/")
 
 # django-storages S3 settings
 AWS_S3_ACCESS_KEY_ID = env.str("AWS_S3_ACCESS_KEY_ID", "")
```

### Comparing `document_merge_service-6.4.5/document_merge_service/tests/test_settings.py` & `document_merge_service-6.5.0/document_merge_service/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.4.5/pyproject.toml` & `document_merge_service-6.5.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,86 +1,93 @@
 [tool.poetry]
 name = "document-merge-service"
-version = "6.4.5"
+version = "6.5.0"
 description = "Merge Document Template Service"
 license = "GPL-3.0-or-later"
 authors = ["Adfinis AG <info@adfinis.com>"]
 homepage = "https://github.com/adfinis/document-merge-service"
 repository = "https://github.com/adfinis/document-merge-service"
 documentation = "https://github.com/adfinis/document-merge-service/blob/main/README.md"
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
+    "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Framework :: Django :: 4",
+    "Framework :: Django :: 4.2",
 ]
 include = ["CHANGELOG.md"]
 exclude = [
     "document-merge-service/**/tests",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8.1"
-Babel = "^2.11.0"
-Django = "^3.2.20"
-django-cors-headers = "^4.2.0"
-django-environ = ">=0.10,<0.12"
-django-filter = "^23.2"
-django-generic-api-permissions = "^0.2.0"
-django-storages = "^1.13.2"
-djangorestframework = "^3.14.0"
+python = ">=3.8.1,<3.13"
+Babel = "^2.15.0"
+Django = "~4.2.13"
+django-cors-headers = "^4.3.1"
+django-environ = "^0.11.2"
+django-filter = "^24.2"
+django-generic-api-permissions = "^0.4.6"
+django-storages = "^1.14.3"
+djangorestframework = "^3.15.1"
 docx-mailmerge = "^0.5.0"
-docxtpl = "^0.16.7"
-Jinja2 = "^3.1.2"
-mysqlclient = { version = "^2.2.0", optional = true }
-psycopg2-binary = { version = "^2.9.6", optional = true }
-python-dateutil = "^2.8.2"
+docxtpl = "^0.17.0"
+Jinja2 = "^3.1.4"
+mysqlclient = { version = "^2.2.4", optional = true }
+psycopg = { version = "^3.1.19", optional = true }
+python-dateutil = "^2.9.0"
 python-memcached = "^1.59"
-requests = "^2.31.0"
-sentry-sdk = "^1.28.1"
-urllib3 = ">=1.26.16 <2"
+requests = "^2.32.3"
+sentry-sdk = "^2.3.1"
+urllib3 = "^2.2.1"
 uWSGI = "^2.0.21"
-xltpl = ">=0.18,<0.20"
+xltpl = "~0.19"
 
 [tool.poetry.group.dev.dependencies]
-black = "23.7.0"
-django-stubs = "4.2.3"
+black = "24.4.2"
+django-stubs = "5.0.2"
 factory-boy = "3.3.0"
-flake8 = "6.1.0"
+flake8 = "7.0.0"
 flake8-debugger = "4.1.2"
 flake8-docstrings = "1.7.0"
 flake8-isort = "6.1.1"
 flake8-string-format = "0.3.0"
 flake8-tuple = "0.4.1"
 gitlint = "0.19.1"
-isort = "5.12.0"
-mypy = "1.7.1"
+isort = "5.13.2"
+mypy = "1.10.0"
 pdbpp = "0.10.3"
 psutil = "5.9.8"
 pydocstyle = "6.3.0"
-pytest = "7.4.4"
-pytest-cov = "4.1.0"
-pytest-django = "4.7.0"
+pytest = "8.2.1"
+pytest-cov = "5.0.0"
+pytest-django = "4.8.0"
 pytest-env = "1.1.3"
-pytest-factoryboy = "2.6.0"
-pytest-mock = "3.12.0"
+pytest-factoryboy = "2.7.0"
+pytest-mock = "3.14.0"
 pytest-randomly = "3.15.0"
 python-semantic-release = "7.34.6"
-requests-mock = "1.11.0"
-syrupy = "4.6.0"
-types-python-dateutil = "2.8.19.14"
-types-requests = "2.31.0.6"
-types-setuptools = "69.0.0.0"
-types-toml = "0.10.8.7"
+requests-mock = "1.12.1"
+syrupy = "4.6.1"
+types-python-dateutil = "2.9.0.20240316"
+types-requests = "2.32.0.20240523"
+types-setuptools = "70.0.0.20240524"
+types-toml = "0.10.8.20240310"
 
 [tool.poetry.extras]
 mysql = ["mysqlclient"]
-pgsql = ["psycopg2-binary"]
-databases = ["mysqlclient", "psycopg2-binary"]
+pgsql = ["psycopg"]
+databases = ["mysqlclient", "psycopg"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 skip = "migrations"
@@ -90,23 +97,27 @@
 force_grid_wrap = 0
 combine_as_imports = true
 line_length = 88
 
 [tool.pytest.ini_options]
 addopts = "--reuse-db --randomly-seed=1521188766 --randomly-dont-reorganize"
 DJANGO_SETTINGS_MODULE = "document_merge_service.settings"
-filterwarnings = """
-    error::DeprecationWarning
-    error::PendingDeprecationWarning
-    ignore:invalid escape sequence
-    ignore:pkg_resources is deprecated as an API:DeprecationWarning"""
-env = """
-    ADMINS=Test Example <test@example.com>,Test2 <test2@example.com>
-    OIDC_USERINFO_ENDPOINT=mock://document-merge-service.github.com/openid/userinfo
-    OIDC_BEARER_TOKEN_REVALIDATION_TIME=60"""
+filterwarnings = [
+    "error::DeprecationWarning",
+    "error::PendingDeprecationWarning",
+    "ignore:invalid escape sequence",
+    "ignore:pkg_resources is deprecated as an API:DeprecationWarning",
+    "ignore:'imghdr' is deprecated:DeprecationWarning",
+    "ignore:datetime.datetime.utcnow():DeprecationWarning"
+]
+env = [
+    "ADMINS=Test Example <test@example.com>,Test2 <test2@example.com>",
+    "OIDC_USERINFO_ENDPOINT=mock://document-merge-service.github.com/openid/userinfo",
+    "OIDC_BEARER_TOKEN_REVALIDATION_TIME=60"
+]
 
 [tool.coverage.run]
 source = ["."]
 
 [tool.coverage.report]
 fail_under = 100
```

### Comparing `document_merge_service-6.4.5/PKG-INFO` & `document_merge_service-6.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,50 @@
 Metadata-Version: 2.1
 Name: document-merge-service
-Version: 6.4.5
+Version: 6.5.0
 Summary: Merge Document Template Service
 Home-page: https://github.com/adfinis/document-merge-service
 License: GPL-3.0-or-later
 Author: Adfinis AG
 Author-email: info@adfinis.com
-Requires-Python: >=3.8.1,<4.0.0
+Requires-Python: >=3.8.1,<3.13
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: Django :: 4
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.8
 Provides-Extra: databases
 Provides-Extra: mysql
 Provides-Extra: pgsql
-Requires-Dist: Babel (>=2.11.0,<3.0.0)
-Requires-Dist: Django (>=3.2.20,<4.0.0)
-Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: django-cors-headers (>=4.2.0,<5.0.0)
-Requires-Dist: django-environ (>=0.10,<0.12)
-Requires-Dist: django-filter (>=23.2,<24.0)
-Requires-Dist: django-generic-api-permissions (>=0.2.0,<0.3.0)
-Requires-Dist: django-storages (>=1.13.2,<2.0.0)
-Requires-Dist: djangorestframework (>=3.14.0,<4.0.0)
+Requires-Dist: Babel (>=2.15.0,<3.0.0)
+Requires-Dist: Django (>=4.2.13,<4.3.0)
+Requires-Dist: Jinja2 (>=3.1.4,<4.0.0)
+Requires-Dist: django-cors-headers (>=4.3.1,<5.0.0)
+Requires-Dist: django-environ (>=0.11.2,<0.12.0)
+Requires-Dist: django-filter (>=24.2,<25.0)
+Requires-Dist: django-generic-api-permissions (>=0.4.6,<0.5.0)
+Requires-Dist: django-storages (>=1.14.3,<2.0.0)
+Requires-Dist: djangorestframework (>=3.15.1,<4.0.0)
 Requires-Dist: docx-mailmerge (>=0.5.0,<0.6.0)
-Requires-Dist: docxtpl (>=0.16.7,<0.17.0)
-Requires-Dist: mysqlclient (>=2.2.0,<3.0.0) ; extra == "mysql" or extra == "databases"
-Requires-Dist: psycopg2-binary (>=2.9.6,<3.0.0) ; extra == "pgsql" or extra == "databases"
-Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
+Requires-Dist: docxtpl (>=0.17.0,<0.18.0)
+Requires-Dist: mysqlclient (>=2.2.4,<3.0.0) ; extra == "mysql" or extra == "databases"
+Requires-Dist: psycopg (>=3.1.19,<4.0.0) ; extra == "pgsql" or extra == "databases"
+Requires-Dist: python-dateutil (>=2.9.0,<3.0.0)
 Requires-Dist: python-memcached (>=1.59,<2.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: sentry-sdk (>=1.28.1,<2.0.0)
+Requires-Dist: requests (>=2.32.3,<3.0.0)
+Requires-Dist: sentry-sdk (>=2.3.1,<3.0.0)
 Requires-Dist: uWSGI (>=2.0.21,<3.0.0)
-Requires-Dist: urllib3 (>=1.26.16,<2)
-Requires-Dist: xltpl (>=0.18,<0.20)
+Requires-Dist: urllib3 (>=2.2.1,<3.0.0)
+Requires-Dist: xltpl (>=0.19,<0.20)
 Project-URL: Documentation, https://github.com/adfinis/document-merge-service/blob/main/README.md
 Project-URL: Repository, https://github.com/adfinis/document-merge-service
 Description-Content-Type: text/markdown
 
 # Document Merge Service
 
 [![Build Status](https://github.com/adfinis/document-merge-service/actions/workflows/tests.yml/badge.svg)](https://github.com/adfinis/document-merge-service/actions/workflows/tests.yml)
```

