# Comparing `tmp/django_import_export-4.0.6.tar.gz` & `tmp/django_import_export-4.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_import_export-4.0.6.tar", last modified: Mon May 27 09:34:50 2024, max compression
+gzip compressed data, was "django_import_export-4.0.7.tar", last modified: Thu May 30 16:58:01 2024, max compression
```

## Comparing `django_import_export-4.0.6.tar` & `django_import_export-4.0.7.tar`

### file list

```diff
@@ -1,346 +1,347 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.741959 django_import_export-4.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-27 09:34:46.000000 django_import_export-4.0.6/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-27 09:34:46.000000 django_import_export-4.0.6/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-27 09:34:46.000000 django_import_export-4.0.6/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-27 09:34:46.000000 django_import_export-4.0.6/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.697959 django_import_export-4.0.6/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-27 09:34:46.000000 django_import_export-4.0.6/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.697959 django_import_export-4.0.6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-27 09:34:46.000000 django_import_export-4.0.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-27 09:34:46.000000 django_import_export-4.0.6/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-27 09:34:46.000000 django_import_export-4.0.6/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-27 09:34:46.000000 django_import_export-4.0.6/.github/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-27 09:34:46.000000 django_import_export-4.0.6/.github/stale.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.697959 django_import_export-4.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-27 09:34:46.000000 django_import_export-4.0.6/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-27 09:34:46.000000 django_import_export-4.0.6/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-27 09:34:46.000000 django_import_export-4.0.6/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-27 09:34:46.000000 django_import_export-4.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-27 09:34:46.000000 django_import_export-4.0.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-27 09:34:46.000000 django_import_export-4.0.6/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-05-27 09:34:46.000000 django_import_export-4.0.6/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-05-27 09:34:46.000000 django_import_export-4.0.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-27 09:34:46.000000 django_import_export-4.0.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-27 09:34:46.000000 django_import_export-4.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-27 09:34:46.000000 django_import_export-4.0.6/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    11616 2024-05-27 09:34:50.741959 django_import_export-4.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8074 2024-05-27 09:34:46.000000 django_import_export-4.0.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-27 09:34:46.000000 django_import_export-4.0.6/RELEASE.md
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-27 09:34:46.000000 django_import_export-4.0.6/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.741959 django_import_export-4.0.6/django_import_export.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11616 2024-05-27 09:34:50.000000 django_import_export-4.0.6/django_import_export.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10608 2024-05-27 09:34:50.000000 django_import_export-4.0.6/django_import_export.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 09:34:50.000000 django_import_export-4.0.6/django_import_export.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-27 09:34:50.000000 django_import_export-4.0.6/django_import_export.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-27 09:34:50.000000 django_import_export-4.0.6/django_import_export.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.705959 django_import_export-4.0.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.685958 django_import_export-4.0.6/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.705959 django_import_export-4.0.6/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (127)    21509 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/_static/images/change-form-export.png
--rw-r--r--   0 runner    (1001) docker     (127)    28966 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/_static/images/custom-export-form.png
--rw-r--r--   0 runner    (1001) docker     (127)    90059 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/_static/images/custom-import-form.png
--rw-r--r--   0 runner    (1001) docker     (127)    33092 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/_static/images/date-widget-validation-error.png
--rw-r--r--   0 runner    (1001) docker     (127)    30818 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/_static/images/django-import-export-change.png
--rw-r--r--   0 runner    (1001) docker     (127)    29191 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/_static/images/django-import-export-export-confirm.png
--rw-r--r--   0 runner    (1001) docker     (127)    35696 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/_static/images/django-import-export-import-confirm.png
--rw-r--r--   0 runner    (1001) docker     (127)    32366 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/_static/images/django-import-export-import.png
--rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/_static/images/export-button.png
--rw-r--r--   0 runner    (1001) docker     (127)    33710 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/_static/images/export_workflow.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/_static/images/import-button.png
--rw-r--r--   0 runner    (1001) docker     (127)    56726 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/_static/images/import_workflow.svg
--rw-r--r--   0 runner    (1001) docker     (127)    29758 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/_static/images/non-field-specific-validation-error.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.709959 django_import_export-4.0.6/docs/_static/images/screenshots/
--rw-r--r--   0 runner    (1001) docker     (127)   445502 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/_static/images/screenshots/confirm-import.png
--rw-r--r--   0 runner    (1001) docker     (127)   311653 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/_static/images/screenshots/export-form.png
--rw-r--r--   0 runner    (1001) docker     (127)   469577 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/_static/images/screenshots/export-selected-action.png
--rw-r--r--   0 runner    (1001) docker     (127)   447473 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/_static/images/screenshots/import-complete.png
--rw-r--r--   0 runner    (1001) docker     (127)   308805 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/_static/images/screenshots/import-form.png
--rw-r--r--   0 runner    (1001) docker     (127)   313540 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/_static/images/screenshots/import-update-with-authors.png
--rw-r--r--   0 runner    (1001) docker     (127)    17197 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/_static/images/select-for-export.png
--rw-r--r--   0 runner    (1001) docker     (127)    22131 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/admin_integration.rst
--rw-r--r--   0 runner    (1001) docker     (127)    32484 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/advanced_usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/api_admin.rst
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/api_exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/api_fields.rst
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/api_forms.rst
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/api_instance_loaders.rst
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/api_mixins.rst
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/api_resources.rst
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/api_results.rst
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/api_tmp_storages.rst
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/api_widgets.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/bulk_import.rst
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/celery.rst
--rw-r--r--   0 runner    (1001) docker     (127)    60640 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/export_workflow.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)    10518 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/getting_started.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.709959 django_import_export-4.0.6/docs/image_src/
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/image_src/export_workflow.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/image_src/import_workflow.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/import_workflow.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)    15691 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/release_notes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/screenshots.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-27 09:34:46.000000 django_import_export-4.0.6/docs/testing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.713959 django_import_export-4.0.6/import_export/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-27 09:34:50.000000 django_import_export-4.0.6/import_export/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    35711 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/declarative.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.713959 django_import_export-4.0.6/import_export/formats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/formats/base_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     9649 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/instance_loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.689959 django_import_export-4.0.6/import_export/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.685958 django_import_export-4.0.6/import_export/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.713959 django_import_export-4.0.6/import_export/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.685958 django_import_export-4.0.6/import_export/locale/bg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.713959 django_import_export-4.0.6/import_export/locale/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/bg/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/bg/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.685958 django_import_export-4.0.6/import_export/locale/ca/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.713959 django_import_export-4.0.6/import_export/locale/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.685958 django_import_export-4.0.6/import_export/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.713959 django_import_export-4.0.6/import_export/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.685958 django_import_export-4.0.6/import_export/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.717959 django_import_export-4.0.6/import_export/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.685958 django_import_export-4.0.6/import_export/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.717959 django_import_export-4.0.6/import_export/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.685958 django_import_export-4.0.6/import_export/locale/es_AR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.717959 django_import_export-4.0.6/import_export/locale/es_AR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/es_AR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/es_AR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.685958 django_import_export-4.0.6/import_export/locale/fa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.717959 django_import_export-4.0.6/import_export/locale/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.685958 django_import_export-4.0.6/import_export/locale/fi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.717959 django_import_export-4.0.6/import_export/locale/fi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.689959 django_import_export-4.0.6/import_export/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.717959 django_import_export-4.0.6/import_export/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.689959 django_import_export-4.0.6/import_export/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.717959 django_import_export-4.0.6/import_export/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.689959 django_import_export-4.0.6/import_export/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.717959 django_import_export-4.0.6/import_export/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.689959 django_import_export-4.0.6/import_export/locale/ko/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.717959 django_import_export-4.0.6/import_export/locale/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/ko/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/ko/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.689959 django_import_export-4.0.6/import_export/locale/kz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.717959 django_import_export-4.0.6/import_export/locale/kz/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/kz/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/kz/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.689959 django_import_export-4.0.6/import_export/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.721959 django_import_export-4.0.6/import_export/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.689959 django_import_export-4.0.6/import_export/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.721959 django_import_export-4.0.6/import_export/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.689959 django_import_export-4.0.6/import_export/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.721959 django_import_export-4.0.6/import_export/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.689959 django_import_export-4.0.6/import_export/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.721959 django_import_export-4.0.6/import_export/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.689959 django_import_export-4.0.6/import_export/locale/sk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.721959 django_import_export-4.0.6/import_export/locale/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/sk/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/sk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.689959 django_import_export-4.0.6/import_export/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.721959 django_import_export-4.0.6/import_export/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.689959 django_import_export-4.0.6/import_export/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.721959 django_import_export-4.0.6/import_export/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (127)     9665 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    51180 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/results.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.689959 django_import_export-4.0.6/import_export/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.721959 django_import_export-4.0.6/import_export/static/import_export/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/static/import_export/export.css
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/static/import_export/export_selectable_fields.js
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/static/import_export/guess_format.js
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/static/import_export/import.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.689959 django_import_export-4.0.6/import_export/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.689959 django_import_export-4.0.6/import_export/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.725959 django_import_export-4.0.6/import_export/templates/admin/import_export/
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/templates/admin/import_export/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/templates/admin/import_export/change_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/templates/admin/import_export/change_list.html
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/templates/admin/import_export/change_list_export.html
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/templates/admin/import_export/change_list_export_item.html
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/templates/admin/import_export/change_list_import.html
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/templates/admin/import_export/change_list_import_export.html
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/templates/admin/import_export/change_list_import_item.html
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/templates/admin/import_export/export.html
--rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/templates/admin/import_export/import.html
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/templates/admin/import_export/resource_fields_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.725959 django_import_export-4.0.6/import_export/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/templatetags/import_export_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/tmp_storages.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21074 2024-05-27 09:34:46.000000 django_import_export-4.0.6/import_export/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-27 09:34:46.000000 django_import_export-4.0.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.725959 django_import_export-4.0.6/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-27 09:34:46.000000 django_import_export-4.0.6/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-27 09:34:46.000000 django_import_export-4.0.6/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-27 09:34:46.000000 django_import_export-4.0.6/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-27 09:34:46.000000 django_import_export-4.0.6/runtests.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      884 2024-05-27 09:34:46.000000 django_import_export-4.0.6/runtests.sh
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 09:34:50.741959 django_import_export-4.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 09:34:46.000000 django_import_export-4.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.725959 django_import_export-4.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/books-sample.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.725959 django_import_export-4.0.6/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.729959 django_import_export-4.0.6/tests/core/exports/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/exports/authors.csv
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/exports/books-ISO-8859-1.csv
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/exports/books-dos.csv
--rw-r--r--   0 runner    (1001) docker     (127)     9650 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/exports/books-empty-author-email.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/exports/books-for-delete.csv
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/exports/books-invalid-date.csv
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/exports/books-mac.csv
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/exports/books-mac.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/exports/books-no-headers.csv
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/exports/books-unicode.csv
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/exports/books-unicode.tsv
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/exports/books.csv
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/exports/books.json
--rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/exports/books.xls
--rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/exports/books.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/exports/child.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.729959 django_import_export-4.0.6/tests/core/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/fixtures/author.json
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/fixtures/book.json
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/fixtures/category.json
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.733959 django_import_export-4.0.6/tests/core/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/migrations/0002_book_published_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/migrations/0003_withfloatfield.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/migrations/0004_bookwithchapters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/migrations/0005_addparentchild.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/migrations/0006_auto_20171130_0147.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/migrations/0007_auto_20180628_0411.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/migrations/0008_auto_20190409_0846.py
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/migrations/0009_auto_20211111_0807.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/migrations/0010_uuidbook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/migrations/0011_uuidcategory_legacybook_alter_uuidbook_id_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/migrations/0012_delete_legacybook.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/migrations/0013_alter_author_birthday.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/migrations/0014_bookwithchapternumbers.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/migrations/0015_withpositiveintegerfields.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/migrations/0016_alter_category_options_alter_uuidcategory_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/migrations/0017_namedauthor_uuidbook_author.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.693959 django_import_export-4.0.6/tests/core/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.733959 django_import_export-4.0.6/tests/core/templates/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.733959 django_import_export-4.0.6/tests/core/templates/core/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/templates/core/admin/change_list.html
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/templates/core/category_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.733959 django_import_export-4.0.6/tests/core/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.737959 django_import_export-4.0.6/tests/core/tests/admin_integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/admin_integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/admin_integration/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     9133 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/admin_integration/test_action_export.py
--rw-r--r--   0 runner    (1001) docker     (127)    20354 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/admin_integration/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)    42497 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/admin_integration/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/admin_integration/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_base_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_declarative.py
--rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_import_export_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_instance_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_invalidrow.py
--rw-r--r--   0 runner    (1001) docker     (127)    14997 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_model_resource_fields_generate_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.737959 django_import_export-4.0.6/tests/core/tests/test_resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22130 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_resources/test_bulk_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_resources/test_diffs.py
--rw-r--r--   0 runner    (1001) docker     (127)    17974 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_resources/test_import_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_resources/test_misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.741959 django_import_export-4.0.6/tests/core/tests/test_resources/test_modelresource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_resources/test_modelresource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6300 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_resources/test_modelresource/test_data_deletion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_resources/test_modelresource/test_data_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_resources/test_modelresource/test_data_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_resources/test_modelresource/test_deprecated_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    13486 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_resources/test_modelresource/test_dynamic_customization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_resources/test_modelresource/test_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_resources/test_modelresource/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_resources/test_modelresource/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_resources/test_modelresource/test_m2m.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_resources/test_modelresource/test_queryset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_resources/test_modelresource/test_relationship.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_resources/test_modelresource/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_resources/test_modelresource/test_resource_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     6083 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_resources/test_modelresource/test_resource_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_resources/test_modelresource/test_resource_postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_resources/test_modelresource/test_resource_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_resources/test_modelresource/test_resource_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_resources/test_modelresource/test_string_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_resources/test_modelresource/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_resources/test_natural_foreign_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_resources/test_relationships.py
--rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_tmp_storages.py
--rw-r--r--   0 runner    (1001) docker     (127)    26670 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/test_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/tests/widget.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/core/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.693959 django_import_export-4.0.6/tests/docker/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.741959 django_import_export-4.0.6/tests/docker/db/
--rwxr-xr-x   0 runner    (1001) docker     (127)      146 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/docker/db/init-mysql-db.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      401 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/docker/db/init-postgres-db.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/docker-compose.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)      320 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:50.741959 django_import_export-4.0.6/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/scripts/bulk_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-27 09:34:46.000000 django_import_export-4.0.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.228353 django_import_export-4.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-30 16:57:56.000000 django_import_export-4.0.7/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-30 16:57:56.000000 django_import_export-4.0.7/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-30 16:57:56.000000 django_import_export-4.0.7/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-30 16:57:56.000000 django_import_export-4.0.7/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.184353 django_import_export-4.0.7/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-30 16:57:56.000000 django_import_export-4.0.7/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.184353 django_import_export-4.0.7/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-30 16:57:56.000000 django_import_export-4.0.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-30 16:57:56.000000 django_import_export-4.0.7/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-30 16:57:56.000000 django_import_export-4.0.7/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-30 16:57:56.000000 django_import_export-4.0.7/.github/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-30 16:57:56.000000 django_import_export-4.0.7/.github/stale.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.184353 django_import_export-4.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-30 16:57:56.000000 django_import_export-4.0.7/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-30 16:57:56.000000 django_import_export-4.0.7/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-30 16:57:56.000000 django_import_export-4.0.7/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-30 16:57:56.000000 django_import_export-4.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-30 16:57:56.000000 django_import_export-4.0.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-30 16:57:56.000000 django_import_export-4.0.7/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-05-30 16:57:56.000000 django_import_export-4.0.7/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-05-30 16:57:56.000000 django_import_export-4.0.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-30 16:57:56.000000 django_import_export-4.0.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-30 16:57:56.000000 django_import_export-4.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-30 16:57:56.000000 django_import_export-4.0.7/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    11616 2024-05-30 16:58:01.228353 django_import_export-4.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8074 2024-05-30 16:57:56.000000 django_import_export-4.0.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-30 16:57:56.000000 django_import_export-4.0.7/RELEASE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-30 16:57:56.000000 django_import_export-4.0.7/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.228353 django_import_export-4.0.7/django_import_export.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11616 2024-05-30 16:58:01.000000 django_import_export-4.0.7/django_import_export.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10638 2024-05-30 16:58:01.000000 django_import_export-4.0.7/django_import_export.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 16:58:01.000000 django_import_export-4.0.7/django_import_export.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-30 16:58:01.000000 django_import_export-4.0.7/django_import_export.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-30 16:58:01.000000 django_import_export-4.0.7/django_import_export.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.188353 django_import_export-4.0.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.172353 django_import_export-4.0.7/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.192353 django_import_export-4.0.7/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    21509 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/_static/images/change-form-export.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28966 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/_static/images/custom-export-form.png
+-rw-r--r--   0 runner    (1001) docker     (127)    90059 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/_static/images/custom-import-form.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33092 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/_static/images/date-widget-validation-error.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30818 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/_static/images/django-import-export-change.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29191 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/_static/images/django-import-export-export-confirm.png
+-rw-r--r--   0 runner    (1001) docker     (127)    35696 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/_static/images/django-import-export-import-confirm.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32366 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/_static/images/django-import-export-import.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/_static/images/export-button.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33710 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/_static/images/export_workflow.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/_static/images/import-button.png
+-rw-r--r--   0 runner    (1001) docker     (127)    56726 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/_static/images/import_workflow.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    29758 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/_static/images/non-field-specific-validation-error.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.196353 django_import_export-4.0.7/docs/_static/images/screenshots/
+-rw-r--r--   0 runner    (1001) docker     (127)   445502 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/_static/images/screenshots/confirm-import.png
+-rw-r--r--   0 runner    (1001) docker     (127)   311653 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/_static/images/screenshots/export-form.png
+-rw-r--r--   0 runner    (1001) docker     (127)   469577 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/_static/images/screenshots/export-selected-action.png
+-rw-r--r--   0 runner    (1001) docker     (127)   447473 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/_static/images/screenshots/import-complete.png
+-rw-r--r--   0 runner    (1001) docker     (127)   308805 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/_static/images/screenshots/import-form.png
+-rw-r--r--   0 runner    (1001) docker     (127)   313540 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/_static/images/screenshots/import-update-with-authors.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17197 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/_static/images/select-for-export.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22134 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/admin_integration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    32484 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/advanced_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/api_admin.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/api_exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/api_fields.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/api_forms.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/api_instance_loaders.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/api_mixins.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/api_resources.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/api_results.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/api_tmp_storages.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/api_widgets.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/bulk_import.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/celery.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    61565 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/export_workflow.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11286 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/getting_started.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.196353 django_import_export-4.0.7/docs/image_src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/image_src/export_workflow.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/image_src/import_workflow.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/import_workflow.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)    16052 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/release_notes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/screenshots.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-30 16:57:56.000000 django_import_export-4.0.7/docs/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.200353 django_import_export-4.0.7/import_export/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-30 16:58:01.000000 django_import_export-4.0.7/import_export/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35711 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/declarative.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.200353 django_import_export-4.0.7/import_export/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/formats/base_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/instance_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.176353 django_import_export-4.0.7/import_export/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.172353 django_import_export-4.0.7/import_export/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.200353 django_import_export-4.0.7/import_export/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.172353 django_import_export-4.0.7/import_export/locale/bg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.200353 django_import_export-4.0.7/import_export/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/bg/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/bg/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.172353 django_import_export-4.0.7/import_export/locale/ca/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.200353 django_import_export-4.0.7/import_export/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.176353 django_import_export-4.0.7/import_export/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.200353 django_import_export-4.0.7/import_export/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.176353 django_import_export-4.0.7/import_export/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.200353 django_import_export-4.0.7/import_export/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.176353 django_import_export-4.0.7/import_export/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.200353 django_import_export-4.0.7/import_export/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.176353 django_import_export-4.0.7/import_export/locale/es_AR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.200353 django_import_export-4.0.7/import_export/locale/es_AR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/es_AR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/es_AR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.176353 django_import_export-4.0.7/import_export/locale/fa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.200353 django_import_export-4.0.7/import_export/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.176353 django_import_export-4.0.7/import_export/locale/fi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.204353 django_import_export-4.0.7/import_export/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.176353 django_import_export-4.0.7/import_export/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.204353 django_import_export-4.0.7/import_export/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.176353 django_import_export-4.0.7/import_export/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.204353 django_import_export-4.0.7/import_export/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.176353 django_import_export-4.0.7/import_export/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.204353 django_import_export-4.0.7/import_export/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.176353 django_import_export-4.0.7/import_export/locale/ko/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.204353 django_import_export-4.0.7/import_export/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/ko/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/ko/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.176353 django_import_export-4.0.7/import_export/locale/kz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.204353 django_import_export-4.0.7/import_export/locale/kz/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/kz/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/kz/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.176353 django_import_export-4.0.7/import_export/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.204353 django_import_export-4.0.7/import_export/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.176353 django_import_export-4.0.7/import_export/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.204353 django_import_export-4.0.7/import_export/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.176353 django_import_export-4.0.7/import_export/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.204353 django_import_export-4.0.7/import_export/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.176353 django_import_export-4.0.7/import_export/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.204353 django_import_export-4.0.7/import_export/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.176353 django_import_export-4.0.7/import_export/locale/sk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.204353 django_import_export-4.0.7/import_export/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/sk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.176353 django_import_export-4.0.7/import_export/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.204353 django_import_export-4.0.7/import_export/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.176353 django_import_export-4.0.7/import_export/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.204353 django_import_export-4.0.7/import_export/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)     9665 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50956 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.176353 django_import_export-4.0.7/import_export/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.208353 django_import_export-4.0.7/import_export/static/import_export/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/static/import_export/export.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/static/import_export/export_selectable_fields.js
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/static/import_export/guess_format.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/static/import_export/import.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.176353 django_import_export-4.0.7/import_export/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.180353 django_import_export-4.0.7/import_export/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.208353 django_import_export-4.0.7/import_export/templates/admin/import_export/
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/templates/admin/import_export/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/templates/admin/import_export/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/templates/admin/import_export/change_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/templates/admin/import_export/change_list_export.html
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/templates/admin/import_export/change_list_export_item.html
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/templates/admin/import_export/change_list_import.html
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/templates/admin/import_export/change_list_import_export.html
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/templates/admin/import_export/change_list_import_item.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/templates/admin/import_export/export.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/templates/admin/import_export/import.html
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/templates/admin/import_export/resource_fields_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.208353 django_import_export-4.0.7/import_export/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/templatetags/import_export_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/tmp_storages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21074 2024-05-30 16:57:56.000000 django_import_export-4.0.7/import_export/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-30 16:57:56.000000 django_import_export-4.0.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.208353 django_import_export-4.0.7/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-30 16:57:56.000000 django_import_export-4.0.7/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-30 16:57:56.000000 django_import_export-4.0.7/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-30 16:57:56.000000 django_import_export-4.0.7/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-30 16:57:56.000000 django_import_export-4.0.7/runtests.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      884 2024-05-30 16:57:56.000000 django_import_export-4.0.7/runtests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 16:58:01.228353 django_import_export-4.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 16:57:56.000000 django_import_export-4.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.208353 django_import_export-4.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/books-sample.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.212353 django_import_export-4.0.7/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.212353 django_import_export-4.0.7/tests/core/exports/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/exports/authors.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/exports/books-ISO-8859-1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/exports/books-dos.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9650 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/exports/books-empty-author-email.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/exports/books-for-delete.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/exports/books-invalid-date.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/exports/books-mac.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/exports/books-mac.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/exports/books-no-headers.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/exports/books-unicode.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/exports/books-unicode.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/exports/books.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/exports/books.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/exports/books.xls
+-rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/exports/books.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/exports/child.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/exports/ebooks.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.212353 django_import_export-4.0.7/tests/core/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/fixtures/author.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/fixtures/book.json
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/fixtures/category.json
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.216353 django_import_export-4.0.7/tests/core/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/migrations/0002_book_published_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/migrations/0003_withfloatfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/migrations/0004_bookwithchapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/migrations/0005_addparentchild.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/migrations/0006_auto_20171130_0147.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/migrations/0007_auto_20180628_0411.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/migrations/0008_auto_20190409_0846.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/migrations/0009_auto_20211111_0807.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/migrations/0010_uuidbook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/migrations/0011_uuidcategory_legacybook_alter_uuidbook_id_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/migrations/0012_delete_legacybook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/migrations/0013_alter_author_birthday.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/migrations/0014_bookwithchapternumbers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/migrations/0015_withpositiveintegerfields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/migrations/0016_alter_category_options_alter_uuidcategory_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/migrations/0017_namedauthor_uuidbook_author.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.180353 django_import_export-4.0.7/tests/core/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.216353 django_import_export-4.0.7/tests/core/templates/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.216353 django_import_export-4.0.7/tests/core/templates/core/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/templates/core/admin/change_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/templates/core/category_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.220353 django_import_export-4.0.7/tests/core/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.220353 django_import_export-4.0.7/tests/core/tests/admin_integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/admin_integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/admin_integration/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9133 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/admin_integration/test_action_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22304 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/admin_integration/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42527 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/admin_integration/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/admin_integration/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_base_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_declarative.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_import_export_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_instance_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_invalidrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14997 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_model_resource_fields_generate_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.220353 django_import_export-4.0.7/tests/core/tests/test_resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22130 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_resources/test_bulk_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_resources/test_diffs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18254 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_resources/test_import_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_resources/test_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.224353 django_import_export-4.0.7/tests/core/tests/test_resources/test_modelresource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_resources/test_modelresource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6300 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_resources/test_modelresource/test_data_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_resources/test_modelresource/test_data_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_resources/test_modelresource/test_data_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_resources/test_modelresource/test_deprecated_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13438 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_resources/test_modelresource/test_dynamic_customization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_resources/test_modelresource/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_resources/test_modelresource/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_resources/test_modelresource/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_resources/test_modelresource/test_m2m.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_resources/test_modelresource/test_queryset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_resources/test_modelresource/test_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_resources/test_modelresource/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_resources/test_modelresource/test_resource_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6083 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_resources/test_modelresource/test_resource_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_resources/test_modelresource/test_resource_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_resources/test_modelresource/test_resource_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_resources/test_modelresource/test_resource_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_resources/test_modelresource/test_string_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_resources/test_modelresource/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_resources/test_natural_foreign_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_resources/test_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_tmp_storages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26670 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/test_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/tests/widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/core/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.180353 django_import_export-4.0.7/tests/docker/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.224353 django_import_export-4.0.7/tests/docker/db/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      146 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/docker/db/init-mysql-db.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      401 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/docker/db/init-postgres-db.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/docker-compose.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      320 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:58:01.224353 django_import_export-4.0.7/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/scripts/bulk_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-30 16:57:56.000000 django_import_export-4.0.7/tox.ini
```

### Comparing `django_import_export-4.0.6/.github/ISSUE_TEMPLATE/bug_report.md` & `django_import_export-4.0.7/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/.github/ISSUE_TEMPLATE/question.md` & `django_import_export-4.0.7/.github/ISSUE_TEMPLATE/question.md`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/.github/stale.yml` & `django_import_export-4.0.7/.github/stale.yml`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/.github/workflows/release.yml` & `django_import_export-4.0.7/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/.github/workflows/test.yml` & `django_import_export-4.0.7/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/AUTHORS` & `django_import_export-4.0.7/AUTHORS`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/CODE_OF_CONDUCT.md` & `django_import_export-4.0.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/LICENSE` & `django_import_export-4.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/Makefile` & `django_import_export-4.0.7/Makefile`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/PKG-INFO` & `django_import_export-4.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-import-export
-Version: 4.0.6
+Version: 4.0.7
 Summary: Django application and library for importing and exporting data with included admin integration.
 Author-email: Bojan Mihelač <djangoimportexport@gmail.com>
 Maintainer-email: Matthew Hegarty <djangoimportexport@gmail.com>
 License: Copyright (c) Bojan Mihelac and individual contributors.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
```

### Comparing `django_import_export-4.0.6/README.rst` & `django_import_export-4.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/RELEASE.md` & `django_import_export-4.0.7/RELEASE.md`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/django_import_export.egg-info/PKG-INFO` & `django_import_export-4.0.7/django_import_export.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-import-export
-Version: 4.0.6
+Version: 4.0.7
 Summary: Django application and library for importing and exporting data with included admin integration.
 Author-email: Bojan Mihelač <djangoimportexport@gmail.com>
 Maintainer-email: Matthew Hegarty <djangoimportexport@gmail.com>
 License: Copyright (c) Bojan Mihelac and individual contributors.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
```

### Comparing `django_import_export-4.0.6/django_import_export.egg-info/SOURCES.txt` & `django_import_export-4.0.7/django_import_export.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -184,14 +184,15 @@
 tests/core/exports/books-unicode.csv
 tests/core/exports/books-unicode.tsv
 tests/core/exports/books.csv
 tests/core/exports/books.json
 tests/core/exports/books.xls
 tests/core/exports/books.xlsx
 tests/core/exports/child.csv
+tests/core/exports/ebooks.csv
 tests/core/fixtures/author.json
 tests/core/fixtures/book.json
 tests/core/fixtures/category.json
 tests/core/migrations/0001_initial.py
 tests/core/migrations/0002_book_published_time.py
 tests/core/migrations/0003_withfloatfield.py
 tests/core/migrations/0004_bookwithchapters.py
```

### Comparing `django_import_export-4.0.6/docs/Makefile` & `django_import_export-4.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/docs/_static/images/change-form-export.png` & `django_import_export-4.0.7/docs/_static/images/change-form-export.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/docs/_static/images/custom-export-form.png` & `django_import_export-4.0.7/docs/_static/images/custom-export-form.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/docs/_static/images/custom-import-form.png` & `django_import_export-4.0.7/docs/_static/images/custom-import-form.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/docs/_static/images/date-widget-validation-error.png` & `django_import_export-4.0.7/docs/_static/images/date-widget-validation-error.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/docs/_static/images/django-import-export-change.png` & `django_import_export-4.0.7/docs/_static/images/django-import-export-change.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/docs/_static/images/django-import-export-export-confirm.png` & `django_import_export-4.0.7/docs/_static/images/django-import-export-export-confirm.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/docs/_static/images/django-import-export-import-confirm.png` & `django_import_export-4.0.7/docs/_static/images/django-import-export-import-confirm.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/docs/_static/images/django-import-export-import.png` & `django_import_export-4.0.7/docs/_static/images/django-import-export-import.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/docs/_static/images/export-button.png` & `django_import_export-4.0.7/docs/_static/images/export-button.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/docs/_static/images/export_workflow.svg` & `django_import_export-4.0.7/docs/_static/images/export_workflow.svg`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/docs/_static/images/import-button.png` & `django_import_export-4.0.7/docs/_static/images/import-button.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/docs/_static/images/import_workflow.svg` & `django_import_export-4.0.7/docs/_static/images/import_workflow.svg`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/docs/_static/images/non-field-specific-validation-error.png` & `django_import_export-4.0.7/docs/_static/images/non-field-specific-validation-error.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/docs/_static/images/screenshots/confirm-import.png` & `django_import_export-4.0.7/docs/_static/images/screenshots/confirm-import.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/docs/_static/images/screenshots/export-form.png` & `django_import_export-4.0.7/docs/_static/images/screenshots/export-form.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/docs/_static/images/screenshots/export-selected-action.png` & `django_import_export-4.0.7/docs/_static/images/screenshots/export-selected-action.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/docs/_static/images/screenshots/import-complete.png` & `django_import_export-4.0.7/docs/_static/images/screenshots/import-complete.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/docs/_static/images/screenshots/import-form.png` & `django_import_export-4.0.7/docs/_static/images/screenshots/import-form.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/docs/_static/images/screenshots/import-update-with-authors.png` & `django_import_export-4.0.7/docs/_static/images/screenshots/import-update-with-authors.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/docs/_static/images/select-for-export.png` & `django_import_export-4.0.7/docs/_static/images/select-for-export.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/docs/admin_integration.rst` & `django_import_export-4.0.7/docs/admin_integration.rst`

 * *Files 0% similar despite different names*

```diff
@@ -348,19 +348,19 @@
 
 Customize ``ModelAdmin`` (for example see ``tests/core/admin.py``)::
 
     class CustomBookAdmin(ImportMixin, ImportExportModelAdmin):
         resource_classes = [EBookResource]
         export_form_class = CustomExportForm
 
-        def get_export_resource_kwargs(self, request, *args, **kwargs):
-            export_form = kwargs["export_form"]
+        def get_export_resource_kwargs(self, request, **kwargs):
+            export_form = kwargs.get("export_form")
             if export_form:
-                return dict(author_id=export_form.cleaned_data["author"].id)
-            return {}
+                kwargs.update(author_id=export_form.cleaned_data["author"].id)
+            return kwargs
 
     admin.site.register(Book, CustomBookAdmin)
 
 Create a Resource subclass to apply the filter
 (for example see ``tests/core/admin.py``)::
 
     class EBookResource(ModelResource):
```

### Comparing `django_import_export-4.0.6/docs/advanced_usage.rst` & `django_import_export-4.0.7/docs/advanced_usage.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/docs/api_mixins.rst` & `django_import_export-4.0.7/docs/api_mixins.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/docs/api_widgets.rst` & `django_import_export-4.0.7/docs/api_widgets.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/docs/bulk_import.rst` & `django_import_export-4.0.7/docs/bulk_import.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/docs/changelog.rst` & `django_import_export-4.0.7/docs/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 Changelog
 =========
 
 .. warning::
 
     Version 4 introduces breaking changes.  Please refer to :doc:`release notes<release_notes>`.
 
+4.0.7 (2024-05-30)
+------------------
+
+- fix documentation to show correct method for reading form data on export (`1859 <https://github.com/django-import-export/django-import-export/pull/1859>`_)
+- Admin UI: display both field name and column name on export (`1857 <https://github.com/django-import-export/django-import-export/pull/1857>`_)
+- fix export declared field with custom column name (`1861 <https://github.com/django-import-export/django-import-export/pull/1861>`_)
+- fix declared fields do not have correct Widget class set (`1861 <https://github.com/django-import-export/django-import-export/pull/1861>`_)
+- docs: clarify changes to ``CharWidget`` in v4 (`1862 <https://github.com/django-import-export/django-import-export/pull/1862>`_)
+- refactor :class:`~import_export.resources.Resource` to remove code duplication in export (`1863 <https://github.com/django-import-export/django-import-export/pull/1863>`_)
+
 4.0.6 (2024-05-27)
 ------------------
 
 - Added additional test for export field order (`1848 <https://github.com/django-import-export/django-import-export/pull/1848>`_)
 - fix crash on import when relation has custom PK (`1853 <https://github.com/django-import-export/django-import-export/pull/1853>`_)
 - fix crash on export from action when instance has custom PK (`1854 <https://github.com/django-import-export/django-import-export/pull/1854>`_)
```

### Comparing `django_import_export-4.0.6/docs/conf.py` & `django_import_export-4.0.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/docs/contributing.rst` & `django_import_export-4.0.7/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/docs/export_workflow.rst` & `django_import_export-4.0.7/docs/export_workflow.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/docs/faq.rst` & `django_import_export-4.0.7/docs/faq.rst`

 * *Files 3% similar despite different names*

```diff
@@ -125,17 +125,35 @@
 back prior to the confirm step.  Database implementations mean that sequence numbers may not be reused.
 
 Consider enabling :ref:`import_export_skip_admin_confirm` as a workaround.
 
 See `this issue <https://github.com/django-import-export/django-import-export/issues/560>`_ for more detailed
 discussion.
 
-Not Null constraint fails when importing blank Charfield
+Not Null constraint fails when importing blank CharField
 --------------------------------------------------------
 
+This was an issue in v3 which is resolved in v4. The issue arises when importing from Excel because empty cells
+are converted to ``None`` during import.  If the import process attempted to save a null value then a 'NOT NULL'
+exception was raised.
+
+In v4, initialization checks to see if the Django ``CharField`` has
+`blank <https://docs.djangoproject.com/en/stable/ref/models/fields/#blank>`_ set to ``True``.
+If it does, then null values or empty strings are persisted as empty strings.
+
+If it is necessary to persist ``None`` instead of an empty string, then the ``allow_blank`` widget parameter can be
+set::
+
+    class BookResource(resources.ModelResource):
+
+        name = Field(widget=CharWidget(allow_blank=False))
+
+        class Meta:
+            model = Book
+
 See `this issue <https://github.com/django-import-export/django-import-export/issues/1485>`_.
 
 Foreign key is null when importing
 ----------------------------------
 
 It is possible to reference model relations by defining a field with the double underscore syntax. For example::
```

### Comparing `django_import_export-4.0.6/docs/getting_started.rst` & `django_import_export-4.0.7/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/docs/image_src/export_workflow.txt` & `django_import_export-4.0.7/docs/image_src/export_workflow.txt`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/docs/image_src/import_workflow.txt` & `django_import_export-4.0.7/docs/image_src/import_workflow.txt`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/docs/import_workflow.rst` & `django_import_export-4.0.7/docs/import_workflow.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/docs/index.rst` & `django_import_export-4.0.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/docs/installation.rst` & `django_import_export-4.0.7/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/docs/make.bat` & `django_import_export-4.0.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/docs/release_notes.rst` & `django_import_export-4.0.7/docs/release_notes.rst`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,19 @@
 
 Functional changes
 ==================
 
 CharWidget
 ----------
 
+Constructor arguments are dynamically set during instantiation based on the properties of the underlying Django
+db CharField.  If the db field has `blank <https://docs.djangoproject.com/en/stable/ref/models/fields/#blank>`_
+set to True, then incoming values of empty strings or null are stored as empty strings.
+See :class:`~import_export.widgets.CharWidget`.
+
 :meth:`~import_export.widgets.CharWidget.clean` will now return a string type as the default.
 The ``coerce_to_string`` option introduced in v3 is no longer used in this method.
 
 Validation error messages
 -------------------------
 
 The following widgets have had validation error messages updated:
```

### Comparing `django_import_export-4.0.6/docs/screenshots.rst` & `django_import_export-4.0.7/docs/screenshots.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/docs/testing.rst` & `django_import_export-4.0.7/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/admin.py` & `django_import_export-4.0.7/import_export/admin.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/declarative.py` & `django_import_export-4.0.7/import_export/declarative.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,14 +47,16 @@
 
         # Add direct fields
         for field_name, obj in attrs.copy().items():
             if isinstance(obj, Field):
                 field = attrs.pop(field_name)
                 if not field.column_name:
                     field.column_name = field_name
+                if not field.attribute:
+                    field.attribute = field_name
                 declared_fields.append((field_name, field))
 
         attrs["fields"] = OrderedDict(declared_fields)
         new_class = super().__new__(cls, name, bases, attrs)
         # add direct fields
         _load_meta_options(new_class, meta)
         new_class._meta = meta
```

### Comparing `django_import_export-4.0.6/import_export/exceptions.py` & `django_import_export-4.0.7/import_export/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/fields.py` & `django_import_export-4.0.7/import_export/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         return value
 
     def get_value(self, instance):
         """
         Returns the value of the instance's attribute.
         """
         if self.attribute is None:
-            return None
+            raise AttributeError("Field attribute cannot be null")
 
         attrs = self.attribute.split("__")
         value = instance
 
         for attr in attrs:
             try:
                 value = getattr(value, attr, None)
```

### Comparing `django_import_export-4.0.6/import_export/formats/base_formats.py` & `django_import_export-4.0.7/import_export/formats/base_formats.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/forms.py` & `django_import_export-4.0.7/import_export/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,24 +130,31 @@
         ordered_fields = [
             "resource",
             # flatten resource fields lists
             *chain(*[fields for fields in self.resource_fields.values()]),
         ]
         self.order_fields(ordered_fields)
 
+    def _get_field_label(self, resource: ModelResource, field_name: str) -> str:
+        title = field_name.replace("_", " ").title()
+        field = resource.fields.get(field_name)
+        if field and field.column_name != field_name:
+            title = f"{title} ({field.column_name})"
+        return title
+
     def _create_boolean_fields(self, resource: ModelResource, index: int) -> None:
         # Initiate resource to get ordered export fields
         fields = resource().get_export_order()
         boolean_fields = []  # will be used for ordering the fields
         is_initial_field = False
 
         for field in fields:
             field_name = self.create_boolean_field_name(resource, field)
             boolean_field = forms.BooleanField(
-                label=field.replace("_", " ").title(),
+                label=self._get_field_label(resource, field),
                 initial=True,
                 required=False,
             )
 
             # These attributes will be used for rendering in template
             boolean_field.is_selectable_field = True
             boolean_field.resource_name = resource.__name__
```

### Comparing `django_import_export-4.0.6/import_export/instance_loaders.py` & `django_import_export-4.0.7/import_export/instance_loaders.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/ar/LC_MESSAGES/django.mo` & `django_import_export-4.0.7/import_export/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/ar/LC_MESSAGES/django.po` & `django_import_export-4.0.7/import_export/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/bg/LC_MESSAGES/django.mo` & `django_import_export-4.0.7/import_export/locale/bg/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/bg/LC_MESSAGES/django.po` & `django_import_export-4.0.7/import_export/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/ca/LC_MESSAGES/django.mo` & `django_import_export-4.0.7/import_export/locale/ca/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/ca/LC_MESSAGES/django.po` & `django_import_export-4.0.7/import_export/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/cs/LC_MESSAGES/django.mo` & `django_import_export-4.0.7/import_export/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/cs/LC_MESSAGES/django.po` & `django_import_export-4.0.7/import_export/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/de/LC_MESSAGES/django.mo` & `django_import_export-4.0.7/import_export/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/de/LC_MESSAGES/django.po` & `django_import_export-4.0.7/import_export/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/es/LC_MESSAGES/django.mo` & `django_import_export-4.0.7/import_export/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/es/LC_MESSAGES/django.po` & `django_import_export-4.0.7/import_export/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/es_AR/LC_MESSAGES/django.mo` & `django_import_export-4.0.7/import_export/locale/es_AR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/es_AR/LC_MESSAGES/django.po` & `django_import_export-4.0.7/import_export/locale/es_AR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/fa/LC_MESSAGES/django.mo` & `django_import_export-4.0.7/import_export/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/fa/LC_MESSAGES/django.po` & `django_import_export-4.0.7/import_export/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/fi/LC_MESSAGES/django.mo` & `django_import_export-4.0.7/import_export/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/fi/LC_MESSAGES/django.po` & `django_import_export-4.0.7/import_export/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/fr/LC_MESSAGES/django.mo` & `django_import_export-4.0.7/import_export/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/fr/LC_MESSAGES/django.po` & `django_import_export-4.0.7/import_export/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/it/LC_MESSAGES/django.mo` & `django_import_export-4.0.7/import_export/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/it/LC_MESSAGES/django.po` & `django_import_export-4.0.7/import_export/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/ja/LC_MESSAGES/django.mo` & `django_import_export-4.0.7/import_export/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/ja/LC_MESSAGES/django.po` & `django_import_export-4.0.7/import_export/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/ko/LC_MESSAGES/django.mo` & `django_import_export-4.0.7/import_export/locale/ko/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/ko/LC_MESSAGES/django.po` & `django_import_export-4.0.7/import_export/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/kz/LC_MESSAGES/django.mo` & `django_import_export-4.0.7/import_export/locale/kz/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/kz/LC_MESSAGES/django.po` & `django_import_export-4.0.7/import_export/locale/kz/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/nl/LC_MESSAGES/django.mo` & `django_import_export-4.0.7/import_export/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/nl/LC_MESSAGES/django.po` & `django_import_export-4.0.7/import_export/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/pl/LC_MESSAGES/django.mo` & `django_import_export-4.0.7/import_export/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/pl/LC_MESSAGES/django.po` & `django_import_export-4.0.7/import_export/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/pt_BR/LC_MESSAGES/django.mo` & `django_import_export-4.0.7/import_export/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/pt_BR/LC_MESSAGES/django.po` & `django_import_export-4.0.7/import_export/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/ru/LC_MESSAGES/django.mo` & `django_import_export-4.0.7/import_export/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/ru/LC_MESSAGES/django.po` & `django_import_export-4.0.7/import_export/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/sk/LC_MESSAGES/django.mo` & `django_import_export-4.0.7/import_export/locale/sk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/sk/LC_MESSAGES/django.po` & `django_import_export-4.0.7/import_export/locale/sk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/tr/LC_MESSAGES/django.mo` & `django_import_export-4.0.7/import_export/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/tr/LC_MESSAGES/django.po` & `django_import_export-4.0.7/import_export/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/zh_Hans/LC_MESSAGES/django.mo` & `django_import_export-4.0.7/import_export/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/locale/zh_Hans/LC_MESSAGES/django.po` & `django_import_export-4.0.7/import_export/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/mixins.py` & `django_import_export-4.0.7/import_export/mixins.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/options.py` & `django_import_export-4.0.7/import_export/options.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/resources.py` & `django_import_export-4.0.7/import_export/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -415,17 +415,14 @@
 
         :param is_m2m: A boolean value indicating whether or not this is a
           many-to-many field.
 
         :param \**kwargs:
             See :meth:`import_row`
         """
-        if not field.attribute:
-            logger.debug(f"skipping field '{field}' - field attribute is not defined")
-            return
         if field.column_name not in row:
             logger.debug(
                 f"skipping field '{field}' "
                 f"- column name '{field.column_name}' is not present in row"
             )
             return
         field.save(instance, row, is_m2m, **kwargs)
@@ -1058,34 +1055,19 @@
             for field in self.fields.values():
                 if field.column_name == field_name:
                     export_fields.append(field)
                     continue
         return export_fields
 
     def export_resource(self, instance, fields=None):
-        export_fields = self.get_export_fields()
-
-        if isinstance(fields, list) and fields:
-            return [
-                self.export_field(field, instance)
-                for field in export_fields
-                if field.attribute in fields or field.column_name in fields
-            ]
-
+        export_fields = self._get_enabled_export_fields(fields)
         return [self.export_field(field, instance) for field in export_fields]
 
     def get_export_headers(self, fields=None):
-        export_fields = self.get_export_fields()
-        if isinstance(fields, list) and fields:
-            return [
-                f.column_name
-                for f in export_fields
-                if f.attribute in fields or f.column_name in fields
-            ]
-
+        export_fields = self._get_enabled_export_fields(fields)
         return [force_str(field.column_name) for field in export_fields]
 
     def get_user_visible_fields(self):
         return self.get_import_fields()
 
     def iter_queryset(self, queryset):
         if not isinstance(queryset, QuerySet):
@@ -1194,14 +1176,26 @@
                 _(
                     "The following fields are declared in 'import_id_fields' but "
                     "are not present in the file headers: %s"
                     % ", ".join(missing_headers)
                 )
             )
 
+    def _get_enabled_export_fields(self, fields_):
+        export_fields = self.get_export_fields()
+
+        if isinstance(fields_, list) and fields_:
+            return [
+                field
+                for field in export_fields
+                if field.attribute in fields_ or field.column_name in fields_
+            ]
+
+        return export_fields
+
 
 class ModelResource(Resource, metaclass=ModelDeclarativeMetaclass):
     """
     ModelResource is Resource subclass for handling Django models.
     """
 
     DEFAULT_RESOURCE_FIELD = Field
```

### Comparing `django_import_export-4.0.6/import_export/results.py` & `django_import_export-4.0.7/import_export/results.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/static/import_export/export_selectable_fields.js` & `django_import_export-4.0.7/import_export/static/import_export/export_selectable_fields.js`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/static/import_export/guess_format.js` & `django_import_export-4.0.7/import_export/static/import_export/guess_format.js`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/static/import_export/import.css` & `django_import_export-4.0.7/import_export/static/import_export/import.css`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/templates/admin/import_export/base.html` & `django_import_export-4.0.7/import_export/templates/admin/import_export/base.html`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/templates/admin/import_export/export.html` & `django_import_export-4.0.7/import_export/templates/admin/import_export/export.html`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/templates/admin/import_export/import.html` & `django_import_export-4.0.7/import_export/templates/admin/import_export/import.html`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/templates/admin/import_export/resource_fields_list.html` & `django_import_export-4.0.7/import_export/templates/admin/import_export/resource_fields_list.html`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/tmp_storages.py` & `django_import_export-4.0.7/import_export/tmp_storages.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/utils.py` & `django_import_export-4.0.7/import_export/utils.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/import_export/widgets.py` & `django_import_export-4.0.7/import_export/widgets.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/pyproject.toml` & `django_import_export-4.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/runtests.py` & `django_import_export-4.0.7/runtests.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/runtests.sh` & `django_import_export-4.0.7/runtests.sh`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/admin.py` & `django_import_export-4.0.7/tests/core/admin.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 class UUIDBookResource(ModelResource):
     class Meta:
         model = UUIDBook
 
 
 class EBookResource(ModelResource):
     published = Field(attribute="published", column_name="published_date")
+    author_email = Field(attribute="author_email", column_name="Email of the author")
 
     def __init__(self, **kwargs):
         super().__init__()
         self.author_id = kwargs.get("author_id")
 
     def filter_export(self, queryset, **kwargs):
         return queryset.filter(author_id=self.author_id)
```

### Comparing `django_import_export-4.0.6/tests/core/exports/books-empty-author-email.xlsx` & `django_import_export-4.0.7/tests/core/exports/books-empty-author-email.xlsx`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/exports/books.json` & `django_import_export-4.0.7/tests/core/exports/books.json`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/exports/books.xls` & `django_import_export-4.0.7/tests/core/exports/books.xls`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/exports/books.xlsx` & `django_import_export-4.0.7/tests/core/exports/books.xlsx`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/fixtures/book.json` & `django_import_export-4.0.7/tests/core/fixtures/book.json`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/forms.py` & `django_import_export-4.0.7/tests/core/forms.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,10 +22,10 @@
 class CustomConfirmImportForm(AuthorFormMixin, ConfirmImportForm):
     """Customized ConfirmImportForm, with author field required"""
 
     pass
 
 
 class CustomExportForm(AuthorFormMixin, SelectableFieldsExportForm):
-    """Customized ExportForm, with author field required"""
+    """Customized ExportForm, with author field required."""
 
-    pass
+    author = forms.ModelChoiceField(queryset=Author.objects.all(), required=True)
```

### Comparing `django_import_export-4.0.6/tests/core/migrations/0001_initial.py` & `django_import_export-4.0.7/tests/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/migrations/0003_withfloatfield.py` & `django_import_export-4.0.7/tests/core/migrations/0003_withfloatfield.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/migrations/0004_bookwithchapters.py` & `django_import_export-4.0.7/tests/core/migrations/0004_bookwithchapters.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/migrations/0005_addparentchild.py` & `django_import_export-4.0.7/tests/core/migrations/0005_addparentchild.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/migrations/0007_auto_20180628_0411.py` & `django_import_export-4.0.7/tests/core/migrations/0007_auto_20180628_0411.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/migrations/0008_auto_20190409_0846.py` & `django_import_export-4.0.7/tests/core/migrations/0008_auto_20190409_0846.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/migrations/0009_auto_20211111_0807.py` & `django_import_export-4.0.7/tests/core/migrations/0009_auto_20211111_0807.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/migrations/0010_uuidbook.py` & `django_import_export-4.0.7/tests/core/migrations/0010_uuidbook.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/migrations/0011_uuidcategory_legacybook_alter_uuidbook_id_and_more.py` & `django_import_export-4.0.7/tests/core/migrations/0011_uuidcategory_legacybook_alter_uuidbook_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/migrations/0014_bookwithchapternumbers.py` & `django_import_export-4.0.7/tests/core/migrations/0014_bookwithchapternumbers.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/migrations/0015_withpositiveintegerfields.py` & `django_import_export-4.0.7/tests/core/migrations/0015_withpositiveintegerfields.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/migrations/0017_namedauthor_uuidbook_author.py` & `django_import_export-4.0.7/tests/core/migrations/0017_namedauthor_uuidbook_author.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/models.py` & `django_import_export-4.0.7/tests/core/models.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/tests/admin_integration/mixins.py` & `django_import_export-4.0.7/tests/core/tests/admin_integration/mixins.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/tests/admin_integration/test_action_export.py` & `django_import_export-4.0.7/tests/core/tests/admin_integration/test_action_export.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/tests/admin_integration/test_export.py` & `django_import_export-4.0.7/tests/core/tests/admin_integration/test_export.py`

 * *Files 2% similar despite different names*

```diff
@@ -304,14 +304,33 @@
     def test_export_model_with_custom_PK(self):
         # issue 1800
         UUIDCategory.objects.create(name="UUIDCategory")
         response = self.client.get(self.uuid_category_export_url)
         self.assertEqual(response.status_code, 200)
         self.assertContains(response, "UUIDCategoryResource")
 
+    def test_export_get(self):
+        """
+        Test export view get method.
+        Test that field checkboxes are displayied with names as discussed under #1846
+        """
+        response = self.client.get(self.ebook_export_url)
+        self.assertContains(
+            response,
+            '<label for="id_ebookresource_published">'
+            "Published (published_date):</label>",
+            html=True,
+        )
+        self.assertContains(
+            response,
+            '<input type="checkbox" name="ebookresource_published" resource-id="0" '
+            'id="id_ebookresource_published" checked="">',
+            html=True,
+        )
+
     def test_export_with_custom_field(self):
         # issue 1808
         a = Author.objects.create(id=11, name="Ian Fleming")
         data = {
             "format": "0",
             "author": a.id,
             "resource": "",
@@ -325,15 +344,17 @@
         self.assertEqual(response.status_code, 200)
         self.assertTrue(response.has_header("Content-Disposition"))
         self.assertEqual(response["Content-Type"], "text/csv")
         self.assertEqual(
             response["Content-Disposition"],
             'attachment; filename="EBook-{}.csv"'.format(date_str),
         )
-        self.assertEqual(b"id,author_email,name,published_date\r\n", response.content)
+        self.assertEqual(
+            b"id,Email of the author,name,published_date\r\n", response.content
+        )
 
 
 class FilteredExportAdminIntegrationTest(AdminTestMixin, TestCase):
     fixtures = ["category", "book", "author"]
 
     def test_export_filters_by_form_param(self):
         # issue 1578
@@ -353,15 +374,15 @@
         self.assertTrue(response.has_header("Content-Disposition"))
         self.assertEqual(response["Content-Type"], "text/csv")
         self.assertEqual(
             response["Content-Disposition"],
             'attachment; filename="EBook-{}.csv"'.format(date_str),
         )
         self.assertEqual(
-            b"id,author_email,name,published_date\r\n"
+            b"id,Email of the author,name,published_date\r\n"
             b"5,ian@example.com,The Man with the Golden Gun,1965-04-01\r\n",
             response.content,
         )
 
 
 class TestExportEncoding(TestCase):
     mock_request = MagicMock(spec=HttpRequest)
@@ -498,11 +519,43 @@
         self.assertTrue(response.has_header("Content-Disposition"))
         self.assertEqual(response["Content-Type"], "text/csv")
         self.assertEqual(
             response["Content-Disposition"],
             'attachment; filename="EBook-{}.csv"'.format(date_str),
         )
         s = (
-            "id,author_email,name,published_date\r\n"
+            "id,Email of the author,name,published_date\r\n"
             f"{book.id},,Moonraker,1955-04-05\r\n"
         )
         self.assertEqual(str.encode(s), response.content)
+
+
+class FilteredExportTest(AdminTestMixin, TestCase):
+    """
+    Tests that exports can be filtered by a custom form field.
+    This process is demonstrated in the documentation.
+    """
+
+    def test_filtered_export(self):
+        a1 = Author.objects.create(id=11, name="Ian Fleming")
+        a2 = Author.objects.create(id=12, name="James Joyce")
+        b1 = Book.objects.create(name="Moonraker", author=a1)
+        b2 = Book.objects.create(name="Ulysses", author=a2)
+        response = self.client.get(self.ebook_export_url)
+        self.assertEqual(response.status_code, 200)
+        data = {
+            "format": "0",
+            "author": a1.id,
+            "resource": "",
+            "ebookresource_id": True,
+            "ebookresource_name": True,
+        }
+        response = self.client.post(self.ebook_export_url, data)
+        self.assertEqual(response.status_code, 200)
+        s = "id,name\r\n" f"{b1.id},Moonraker\r\n"
+        self.assertEqual(str.encode(s), response.content)
+
+        data["author"] = a2.id
+        response = self.client.post(self.ebook_export_url, data)
+        self.assertEqual(response.status_code, 200)
+        s = "id,name\r\n" f"{b2.id},Ulysses\r\n"
+        self.assertEqual(str.encode(s), response.content)
```

### Comparing `django_import_export-4.0.6/tests/core/tests/admin_integration/test_import.py` & `django_import_export-4.0.7/tests/core/tests/admin_integration/test_import.py`

 * *Files 1% similar despite different names*

```diff
@@ -928,25 +928,25 @@
 
     fixtures = ["author"]
 
     def test_import_preview_order(self):
         author_id = Author.objects.first().id
         response = self._do_import_post(
             self.ebook_import_url,
-            "books.csv",
+            "ebooks.csv",
             input_format="0",
             data={"author": author_id},
         )
         # test header rendered in correct order
         target_header_re = (
             r"<thead>[\\n\s]+"
             r"<tr>[\\n\s]+"
             r"<th></th>[\\n\s]+"
             r"<th>id</th>[\\n\s]+"
-            r"<th>author_email</th>[\\n\s]+"
+            r"<th>Email of the author</th>[\\n\s]+"
             r"<th>name</th>[\\n\s]+"
             r"<th>published_date</th>[\\n\s]+"
             r"</tr>[\\n\s]+"
             "</thead>"
         )
         self.assertRegex(str(response.content), target_header_re)
         # test row rendered in correct order
@@ -975,25 +975,25 @@
         super().tearDown()
         EBookResource._meta.fields = ("id", "author_email", "name", "published")
 
     def test_import_preview_order(self):
         author_id = Author.objects.first().id
         response = self._do_import_post(
             self.ebook_import_url,
-            "books.csv",
+            "ebooks.csv",
             input_format="0",
             data={"author": author_id},
         )
         # test header rendered in correct order
         target_header_re = (
             r"<thead>[\\n\s]+"
             r"<tr>[\\n\s]+"
             r"<th></th>[\\n\s]+"
             r"<th>id</th>[\\n\s]+"
-            r"<th>author_email</th>[\\n\s]+"
+            r"<th>Email of the author</th>[\\n\s]+"
             r"<th>name</th>[\\n\s]+"
             r"<th>published_date</th>[\\n\s]+"
             r"</tr>[\\n\s]+"
             "</thead>"
         )
         self.assertRegex(str(response.content), target_header_re)
         # test row rendered in correct order
@@ -1017,15 +1017,15 @@
     """
 
     def test_import_preview_order(self):
         response = self.client.get(self.ebook_import_url)
         # test display rendered in correct order
         target_re = (
             r"This importer will import the following fields:[\\n\s]+"
-            r"<code>id, author_email, name, published_date</code>[\\n\s]+"
+            r"<code>id, Email of the author, name, published_date</code>[\\n\s]+"
         )
         self.assertRegex(str(response.content), target_re)
 
 
 class DeclaredImportOrderTest(AdminTestMixin, TestCase):
     """
     Display correct import order when 'import_order' is declared (issue 1845).
@@ -1042,10 +1042,10 @@
         EBookResource._meta.import_order = ()
 
     def test_import_preview_order(self):
         response = self.client.get(self.ebook_import_url)
         # test display rendered in correct order
         target_re = (
             r"This importer will import the following fields:[\\n\s]+"
-            r"<code>id, name, published_date, author_email</code>[\\n\s]+"
+            r"<code>id, name, published_date, Email of the author</code>[\\n\s]+"
         )
         self.assertRegex(str(response.content), target_re)
```

### Comparing `django_import_export-4.0.6/tests/core/tests/admin_integration/test_views.py` & `django_import_export-4.0.7/tests/core/tests/admin_integration/test_views.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/tests/resources.py` & `django_import_export-4.0.7/tests/core/tests/resources.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/tests/test_base_formats.py` & `django_import_export-4.0.7/tests/core/tests/test_base_formats.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/tests/test_declarative.py` & `django_import_export-4.0.7/tests/core/tests/test_declarative.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/tests/test_fields.py` & `django_import_export-4.0.7/tests/core/tests/test_fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,7 +147,13 @@
         class CallableValue:
             def __call__(self):
                 return "some val"
 
         self.obj.name = CallableValue()
         val = self.field.get_value(self.obj)
         self.assertEqual("some val", val)
+
+    def test_get_value_with_no_attribute(self):
+        self.field.attribute = None
+        with self.assertRaises(AttributeError) as e:
+            self.field.get_value(self.obj)
+        self.assertEqual("Field attribute cannot be null", str(e.exception))
```

### Comparing `django_import_export-4.0.6/tests/core/tests/test_forms.py` & `django_import_export-4.0.7/tests/core/tests/test_forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,14 +176,28 @@
     def test_get_selected_resource_fields_without_validation_raises_validation_error(
         self,
     ) -> None:
         self.assertRaises(
             django.forms.ValidationError, self.form.get_selected_resource_export_fields
         )
 
+    def test_get_field_label(self):
+        """test SelectableFieldsExportForm._get_field_label"""
+        form = forms.SelectableFieldsExportForm(
+            formats=(CSV,), resources=(BookResource,)
+        )
+        resource = BookResource()
+        self.assertEqual(
+            form._get_field_label(resource, "bookresource_id"),
+            "Bookresource Id",
+        )
+        self.assertEqual(
+            form._get_field_label(resource, "published"), "Published (published_date)"
+        )
+
     def test_get_selected_resrource_fields(self) -> None:
         data = {"resource": "0", "format": "0"}
         form = forms.SelectableFieldsExportForm(
             formats=(CSV,), resources=self.resources, data=data
         )
         for resource in self.resources:
             for field in resource().get_export_order():
```

### Comparing `django_import_export-4.0.6/tests/core/tests/test_instance_loaders.py` & `django_import_export-4.0.7/tests/core/tests/test_instance_loaders.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/tests/test_invalidrow.py` & `django_import_export-4.0.7/tests/core/tests/test_invalidrow.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/tests/test_mixins.py` & `django_import_export-4.0.7/tests/core/tests/test_mixins.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/tests/test_model_resource_fields_generate_widgets.py` & `django_import_export-4.0.7/tests/core/tests/test_model_resource_fields_generate_widgets.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/tests/test_permissions.py` & `django_import_export-4.0.7/tests/core/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/tests/test_resources/test_bulk_operations.py` & `django_import_export-4.0.7/tests/core/tests/test_resources/test_bulk_operations.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/tests/test_resources/test_diffs.py` & `django_import_export-4.0.7/tests/core/tests/test_resources/test_diffs.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/tests/test_resources/test_import_export.py` & `django_import_export-4.0.7/tests/core/tests/test_resources/test_import_export.py`

 * *Files 3% similar despite different names*

```diff
@@ -251,15 +251,15 @@
 
                 return ""
 
         self.resource = DeclaredModelFieldBookResource()
         self.assertEqual(self.resource.get_export_order(), self.resource._meta.fields)
 
     def test_declared_field_export_order(self):
-        # issue 1846
+        # issue 1848
         class DeclaredModelFieldBookResource(
             ImportExportFieldOrderTest.BaseBookResource
         ):
             published = fields.Field(
                 attribute="published",
                 column_name="date published",
                 widget=widgets.DateWidget("%d.%m.%Y"),
@@ -279,14 +279,47 @@
                 )
 
         self.resource = DeclaredModelFieldBookResource()
         data = self.resource.export()
         target = f"date published,id,author\r\n,{self.pk},\r\n"
         self.assertEqual(target, data.csv)
 
+    def test_export_fields_column_name(self):
+        """Test export with declared export_fields and custom column_name"""
+
+        # issue 1846
+        class DeclaredModelFieldBookResource(resources.ModelResource):
+            published = fields.Field(
+                attribute="published",
+                column_name="datePublished",
+                widget=widgets.DateWidget("%d.%m.%Y"),
+            )
+            author = fields.Field(column_name="AuthorFooName")
+
+            class Meta:
+                model = Book
+                fields = (
+                    "id",
+                    "author",
+                    "published",
+                )
+                export_order = (
+                    "published",
+                    "id",
+                    "author",
+                )
+
+            def dehydrate_author(self, obj):
+                return obj.author
+
+        self.resource = DeclaredModelFieldBookResource()
+        data = self.resource.export()
+        target = f"datePublished,id,AuthorFooName\r\n,{self.pk},\r\n"
+        self.assertEqual(target, data.csv)
+
 
 class ImportIdFieldsTestCase(TestCase):
     class BookResource(resources.ModelResource):
         name = fields.Field(attribute="name", column_name="book_name")
 
         class Meta:
             model = Book
@@ -380,35 +413,14 @@
         )
         self.resource.import_data(dataset, raise_errors=True)
         self.assertEqual("Goldeneye", Book.objects.latest("id").name)
 
 
 class ImportWithMissingFields(TestCase):
     # issue 1517
-
-    @patch("import_export.resources.logger")
-    @patch("import_export.fields.Field.save")
-    def test_import_with_missing_instance_attribute(self, mock_field_save, mock_logger):
-        class _BookResource(resources.ModelResource):
-            name = fields.Field(column_name="name")
-
-            class Meta:
-                model = Book
-
-        dataset = tablib.Dataset(*[(1, "Some book")], headers=["id", "name"])
-        self.resource = _BookResource()
-        result = self.resource.import_data(dataset)
-        self.assertFalse(result.has_errors())
-        target = (
-            "skipping field '<import_export.fields.Field: name>' "
-            "- field attribute is not defined"
-        )
-        mock_logger.debug.assert_any_call(target)
-        self.assertEqual(1, mock_field_save.call_count)
-
     @patch("import_export.resources.logger")
     @patch("import_export.fields.Field.save")
     def test_import_with_missing_field_in_row(self, mock_field_save, mock_logger):
         dataset = tablib.Dataset(*[(1, "Some book")], headers=["id", "name"])
         self.resource = BookResource()
         result = self.resource.import_data(dataset)
         self.assertFalse(result.has_errors())
```

### Comparing `django_import_export-4.0.6/tests/core/tests/test_resources/test_misc.py` & `django_import_export-4.0.7/tests/core/tests/test_resources/test_misc.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/tests/test_resources/test_modelresource/test_data_deletion.py` & `django_import_export-4.0.7/tests/core/tests/test_resources/test_modelresource/test_data_deletion.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/tests/test_resources/test_modelresource/test_data_handling.py` & `django_import_export-4.0.7/tests/core/tests/test_resources/test_modelresource/test_data_handling.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/tests/test_resources/test_modelresource/test_data_import.py` & `django_import_export-4.0.7/tests/core/tests/test_resources/test_modelresource/test_data_import.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/tests/test_resources/test_modelresource/test_deprecated_fields.py` & `django_import_export-4.0.7/tests/core/tests/test_resources/test_modelresource/test_deprecated_fields.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/tests/test_resources/test_modelresource/test_dynamic_customization.py` & `django_import_export-4.0.7/tests/core/tests/test_resources/test_modelresource/test_dynamic_customization.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,17 +114,15 @@
         resource = B()
         with self.assertRaises(exceptions.ImportError) as cm:
             resource.import_data(self.dataset, raise_errors=True)
         self.assertEqual("This is an invalid dataset", cm.exception.error.args[0])
 
     def test_after_import_raises_error(self):
         class B(BookResource):
-            def after_import(
-                self, dataset, result, using_transactions, dry_run, **kwargs
-            ):
+            def after_import(self, dataset, result, **kwargs):
                 raise Exception("This is an invalid dataset")
 
         resource = B()
         with self.assertRaises(exceptions.ImportError) as cm:
             resource.import_data(self.dataset, raise_errors=True)
         self.assertEqual("This is an invalid dataset", cm.exception.error.args[0])
 
@@ -183,15 +181,15 @@
                 if field_name == "published":
                     return {"sound": "quack"}
 
         B()
         self.assertEqual({"sound": "quack"}, B.fields["published"])
 
     def test_readonly_annotated_field_import_and_export(self):
-        class B(BookResource):
+        class B(resources.ModelResource):
             total_categories = fields.Field("total_categories", readonly=True)
 
             class Meta:
                 model = Book
                 skip_unchanged = True
 
         cat1 = Category.objects.create(name="Cat 1")
```

### Comparing `django_import_export-4.0.6/tests/core/tests/test_resources/test_modelresource/test_error_handling.py` & `django_import_export-4.0.7/tests/core/tests/test_resources/test_modelresource/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/tests/test_resources/test_modelresource/test_export.py` & `django_import_export-4.0.7/tests/core/tests/test_resources/test_modelresource/test_export.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,17 @@
+from datetime import date
+
 import tablib
 from core.admin import BookResource
-from core.models import Author, Book
+from core.models import Author, Book, EBook
 from django.test import TestCase
 
+from import_export.fields import Field
+from import_export.resources import ModelResource
+
 
 class ExportFunctionalityTest(TestCase):
     def setUp(self):
         self.resource = BookResource()
         self.book = Book.objects.create(name="Some book")
         self.dataset = tablib.Dataset(headers=["id", "name", "author_email", "price"])
         row = [self.book.pk, "Some book", "test@example.com", "10.25"]
@@ -71,7 +76,24 @@
                 self.kwargs_ = kwargs
 
         self.resource = _BookResource()
         # when queryset is supplied, it should be passed to before_export()
         self.resource.export(queryset=Book.objects.all(), **{"a": 1})
         self.assertEqual(Book.objects.count(), len(self.resource.qs))
         self.assertEqual(dict(a=1), self.resource.kwargs_)
+
+    def test_export_declared_field(self):
+        # test that declared fields have the correct widget set
+        # #1860
+        class EBookResource(ModelResource):
+            published = Field(column_name="published")
+
+            class Meta:
+                model = EBook
+                fields = ("id", "published")
+
+        resource = EBookResource()
+
+        self.book.published = date(1955, 4, 5)
+        self.book.save()
+        dataset = resource.export()
+        self.assertEqual("1955-04-05", dataset.dict[0]["published"])
```

### Comparing `django_import_export-4.0.6/tests/core/tests/test_resources/test_modelresource/test_fields.py` & `django_import_export-4.0.7/tests/core/tests/test_resources/test_modelresource/test_fields.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/tests/test_resources/test_modelresource/test_m2m.py` & `django_import_export-4.0.7/tests/core/tests/test_resources/test_modelresource/test_m2m.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/tests/test_resources/test_modelresource/test_queryset.py` & `django_import_export-4.0.7/tests/core/tests/test_resources/test_modelresource/test_queryset.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/tests/test_resources/test_modelresource/test_relationship.py` & `django_import_export-4.0.7/tests/core/tests/test_resources/test_modelresource/test_relationship.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/tests/test_resources/test_modelresource/test_resource.py` & `django_import_export-4.0.7/tests/core/tests/test_resources/test_modelresource/test_resource.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/tests/test_resources/test_modelresource/test_resource_fields.py` & `django_import_export-4.0.7/tests/core/tests/test_resources/test_modelresource/test_resource_fields.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/tests/test_resources/test_modelresource/test_resource_postgres.py` & `django_import_export-4.0.7/tests/core/tests/test_resources/test_modelresource/test_resource_postgres.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/tests/test_resources/test_modelresource/test_resource_setup.py` & `django_import_export-4.0.7/tests/core/tests/test_resources/test_modelresource/test_resource_setup.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/tests/test_resources/test_modelresource/test_resource_transactions.py` & `django_import_export-4.0.7/tests/core/tests/test_resources/test_modelresource/test_resource_transactions.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/tests/test_resources/test_modelresource/test_widget.py` & `django_import_export-4.0.7/tests/core/tests/test_resources/test_modelresource/test_widget.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/tests/test_resources/test_natural_foreign_key.py` & `django_import_export-4.0.7/tests/core/tests/test_resources/test_natural_foreign_key.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/tests/test_resources/test_relationships.py` & `django_import_export-4.0.7/tests/core/tests/test_resources/test_relationships.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/tests/test_results.py` & `django_import_export-4.0.7/tests/core/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/tests/test_tmp_storages.py` & `django_import_export-4.0.7/tests/core/tests/test_tmp_storages.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/core/tests/test_widgets.py` & `django_import_export-4.0.7/tests/core/tests/test_widgets.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/docker-compose.yml` & `django_import_export-4.0.7/tests/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/scripts/bulk_import.py` & `django_import_export-4.0.7/tests/scripts/bulk_import.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tests/settings.py` & `django_import_export-4.0.7/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.6/tox.ini` & `django_import_export-4.0.7/tox.ini`

 * *Files identical despite different names*

