# Comparing `tmp/ludic-0.4.6.tar.gz` & `tmp/ludic-0.4.7.tar.gz`

## Comparing `ludic-0.4.6.tar` & `ludic-0.4.7.tar`

### file list

```diff
@@ -1,84 +1,84 @@
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 ludic-0.4.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 ludic-0.4.6/.readthedocs.yaml
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 ludic-0.4.6/CONTRIBUTING.md
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ludic-0.4.6/_version.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 ludic-0.4.6/mkdocs.yaml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ludic-0.4.6/.github/dependabot.yml
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 ludic-0.4.6/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 ludic-0.4.6/.github/workflows/test.yaml
--rw-r--r--   0        0        0     9401 2020-02-02 00:00:00.000000 ludic-0.4.6/docs/catalog.md
--rw-r--r--   0        0        0    11706 2020-02-02 00:00:00.000000 ludic-0.4.6/docs/components.md
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ludic-0.4.6/docs/examples.md
--rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 ludic-0.4.6/docs/getting-started.md
--rw-r--r--   0        0        0     3665 2020-02-02 00:00:00.000000 ludic-0.4.6/docs/htmx.md
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 ludic-0.4.6/docs/index.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 ludic-0.4.6/docs/requirements.txt
--rw-r--r--   0        0        0     9658 2020-02-02 00:00:00.000000 ludic-0.4.6/docs/styles.md
--rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 ludic-0.4.6/docs/web-framework.md
--rw-r--r--   0        0        0   127587 2020-02-02 00:00:00.000000 ludic-0.4.6/docs/assets/ludic.png
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 ludic-0.4.6/examples/README.md
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 ludic-0.4.6/examples/__init__.py
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 ludic-0.4.6/examples/bulk_update.py
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 ludic-0.4.6/examples/click_to_edit.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 ludic-0.4.6/examples/click_to_load.py
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 ludic-0.4.6/examples/delete_row.py
--rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 ludic-0.4.6/examples/edit_row.py
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 ludic-0.4.6/examples/infinite_scroll.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 ludic-0.4.6/examples/lazy_loading.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/__init__.py
--rw-r--r--   0        0        0    16536 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/attrs.py
--rw-r--r--   0        0        0    10039 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/base.py
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/components.py
--rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/format.py
--rw-r--r--   0        0        0    12137 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/html.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/py.typed
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/types.py
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/utils.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/catalog/__init__.py
--rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/catalog/buttons.py
--rw-r--r--   0        0        0     8599 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/catalog/forms.py
--rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/catalog/headers.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/catalog/icons.py
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/catalog/items.py
--rw-r--r--   0        0        0     9271 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/catalog/layouts.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/catalog/lists.py
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/catalog/loaders.py
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/catalog/messages.py
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/catalog/navigation.py
--rw-r--r--   0        0        0     6982 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/catalog/pages.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/catalog/quotes.py
--rw-r--r--   0        0        0     7091 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/catalog/tables.py
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/catalog/typography.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/catalog/utils.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/styles/__init__.py
--rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/styles/collect.py
--rw-r--r--   0        0        0     6220 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/styles/themes.py
--rw-r--r--   0        0        0    24379 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/styles/types.py
--rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/styles/utils.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/web/__init__.py
--rw-r--r--   0        0        0     8202 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/web/app.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/web/datastructures.py
--rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/web/endpoints.py
--rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/web/exceptions.py
--rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/web/parsers.py
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/web/requests.py
--rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/web/responses.py
--rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 ludic-0.4.6/ludic/web/routing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.6/tests/__init__.py
--rw-r--r--   0        0        0     6868 2020-02-02 00:00:00.000000 ludic-0.4.6/tests/test_components.py
--rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 ludic-0.4.6/tests/test_elements.py
--rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 ludic-0.4.6/tests/test_examples.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 ludic-0.4.6/tests/test_exceptions.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 ludic-0.4.6/tests/test_formatting.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ludic-0.4.6/tests/test_types.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 ludic-0.4.6/tests/styles/__init__.py
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 ludic-0.4.6/tests/styles/test_styles.py
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 ludic-0.4.6/tests/styles/test_themes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.6/tests/web/__init__.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 ludic-0.4.6/tests/web/test_datastructures.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 ludic-0.4.6/tests/web/test_requests.py
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 ludic-0.4.6/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 ludic-0.4.6/LICENCE
--rw-r--r--   0        0        0     6269 2020-02-02 00:00:00.000000 ludic-0.4.6/README.md
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 ludic-0.4.6/pyproject.toml
--rw-r--r--   0        0        0     7574 2020-02-02 00:00:00.000000 ludic-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 ludic-0.4.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 ludic-0.4.7/.readthedocs.yaml
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 ludic-0.4.7/CONTRIBUTING.md
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ludic-0.4.7/_version.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 ludic-0.4.7/mkdocs.yaml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ludic-0.4.7/.github/dependabot.yml
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 ludic-0.4.7/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 ludic-0.4.7/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     9401 2020-02-02 00:00:00.000000 ludic-0.4.7/docs/catalog.md
+-rw-r--r--   0        0        0    11706 2020-02-02 00:00:00.000000 ludic-0.4.7/docs/components.md
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ludic-0.4.7/docs/examples.md
+-rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 ludic-0.4.7/docs/getting-started.md
+-rw-r--r--   0        0        0     3665 2020-02-02 00:00:00.000000 ludic-0.4.7/docs/htmx.md
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 ludic-0.4.7/docs/index.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 ludic-0.4.7/docs/requirements.txt
+-rw-r--r--   0        0        0     9658 2020-02-02 00:00:00.000000 ludic-0.4.7/docs/styles.md
+-rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 ludic-0.4.7/docs/web-framework.md
+-rw-r--r--   0        0        0   127587 2020-02-02 00:00:00.000000 ludic-0.4.7/docs/assets/ludic.png
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 ludic-0.4.7/examples/README.md
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 ludic-0.4.7/examples/__init__.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 ludic-0.4.7/examples/bulk_update.py
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 ludic-0.4.7/examples/click_to_edit.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 ludic-0.4.7/examples/click_to_load.py
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 ludic-0.4.7/examples/delete_row.py
+-rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 ludic-0.4.7/examples/edit_row.py
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 ludic-0.4.7/examples/infinite_scroll.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 ludic-0.4.7/examples/lazy_loading.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/__init__.py
+-rw-r--r--   0        0        0    16536 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/attrs.py
+-rw-r--r--   0        0        0    10039 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/base.py
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/components.py
+-rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/format.py
+-rw-r--r--   0        0        0    12137 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/html.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/py.typed
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/types.py
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/utils.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/catalog/__init__.py
+-rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/catalog/buttons.py
+-rw-r--r--   0        0        0     8599 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/catalog/forms.py
+-rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/catalog/headers.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/catalog/icons.py
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/catalog/items.py
+-rw-r--r--   0        0        0     9271 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/catalog/layouts.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/catalog/lists.py
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/catalog/loaders.py
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/catalog/messages.py
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/catalog/navigation.py
+-rw-r--r--   0        0        0     6982 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/catalog/pages.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/catalog/quotes.py
+-rw-r--r--   0        0        0     7091 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/catalog/tables.py
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/catalog/typography.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/catalog/utils.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/styles/__init__.py
+-rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/styles/collect.py
+-rw-r--r--   0        0        0     6614 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/styles/themes.py
+-rw-r--r--   0        0        0    27206 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/styles/types.py
+-rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/styles/utils.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/web/__init__.py
+-rw-r--r--   0        0        0     8202 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/web/app.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/web/datastructures.py
+-rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/web/endpoints.py
+-rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/web/exceptions.py
+-rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/web/parsers.py
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/web/requests.py
+-rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/web/responses.py
+-rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/web/routing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.7/tests/__init__.py
+-rw-r--r--   0        0        0     6868 2020-02-02 00:00:00.000000 ludic-0.4.7/tests/test_components.py
+-rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 ludic-0.4.7/tests/test_elements.py
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 ludic-0.4.7/tests/test_examples.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 ludic-0.4.7/tests/test_exceptions.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 ludic-0.4.7/tests/test_formatting.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ludic-0.4.7/tests/test_types.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 ludic-0.4.7/tests/styles/__init__.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 ludic-0.4.7/tests/styles/test_styles.py
+-rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 ludic-0.4.7/tests/styles/test_themes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.7/tests/web/__init__.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 ludic-0.4.7/tests/web/test_datastructures.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 ludic-0.4.7/tests/web/test_requests.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 ludic-0.4.7/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 ludic-0.4.7/LICENCE
+-rw-r--r--   0        0        0     6269 2020-02-02 00:00:00.000000 ludic-0.4.7/README.md
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 ludic-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0     7574 2020-02-02 00:00:00.000000 ludic-0.4.7/PKG-INFO
```

### Comparing `ludic-0.4.6/.pre-commit-config.yaml` & `ludic-0.4.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/CONTRIBUTING.md` & `ludic-0.4.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/mkdocs.yaml` & `ludic-0.4.7/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/.github/workflows/publish.yaml` & `ludic-0.4.7/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/.github/workflows/test.yaml` & `ludic-0.4.7/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/docs/catalog.md` & `ludic-0.4.7/docs/catalog.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/docs/components.md` & `ludic-0.4.7/docs/components.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/docs/getting-started.md` & `ludic-0.4.7/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/docs/htmx.md` & `ludic-0.4.7/docs/htmx.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/docs/index.md` & `ludic-0.4.7/docs/index.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/docs/styles.md` & `ludic-0.4.7/docs/styles.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/docs/web-framework.md` & `ludic-0.4.7/docs/web-framework.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/docs/assets/ludic.png` & `ludic-0.4.7/docs/assets/ludic.png`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/examples/README.md` & `ludic-0.4.7/examples/README.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/examples/__init__.py` & `ludic-0.4.7/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/examples/bulk_update.py` & `ludic-0.4.7/examples/bulk_update.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/examples/click_to_edit.py` & `ludic-0.4.7/examples/click_to_edit.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/examples/click_to_load.py` & `ludic-0.4.7/examples/click_to_load.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/examples/delete_row.py` & `ludic-0.4.7/examples/delete_row.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/examples/edit_row.py` & `ludic-0.4.7/examples/edit_row.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/examples/infinite_scroll.py` & `ludic-0.4.7/examples/infinite_scroll.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/examples/lazy_loading.py` & `ludic-0.4.7/examples/lazy_loading.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/ludic/attrs.py` & `ludic-0.4.7/ludic/attrs.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/ludic/base.py` & `ludic-0.4.7/ludic/base.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/ludic/components.py` & `ludic-0.4.7/ludic/components.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/ludic/format.py` & `ludic-0.4.7/ludic/format.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/ludic/html.py` & `ludic-0.4.7/ludic/html.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/ludic/types.py` & `ludic-0.4.7/ludic/types.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/ludic/utils.py` & `ludic-0.4.7/ludic/utils.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/ludic/catalog/buttons.py` & `ludic-0.4.7/ludic/catalog/buttons.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/ludic/catalog/forms.py` & `ludic-0.4.7/ludic/catalog/forms.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/ludic/catalog/headers.py` & `ludic-0.4.7/ludic/catalog/headers.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/ludic/catalog/icons.py` & `ludic-0.4.7/ludic/catalog/icons.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/ludic/catalog/items.py` & `ludic-0.4.7/ludic/catalog/items.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/ludic/catalog/layouts.py` & `ludic-0.4.7/ludic/catalog/layouts.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/ludic/catalog/lists.py` & `ludic-0.4.7/ludic/catalog/lists.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/ludic/catalog/loaders.py` & `ludic-0.4.7/ludic/catalog/loaders.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/ludic/catalog/messages.py` & `ludic-0.4.7/ludic/catalog/messages.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/ludic/catalog/navigation.py` & `ludic-0.4.7/ludic/catalog/navigation.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/ludic/catalog/pages.py` & `ludic-0.4.7/ludic/catalog/pages.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/ludic/catalog/quotes.py` & `ludic-0.4.7/ludic/catalog/quotes.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/ludic/catalog/tables.py` & `ludic-0.4.7/ludic/catalog/tables.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/ludic/catalog/typography.py` & `ludic-0.4.7/ludic/catalog/typography.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/ludic/catalog/utils.py` & `ludic-0.4.7/ludic/catalog/utils.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/ludic/styles/collect.py` & `ludic-0.4.7/ludic/styles/collect.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/ludic/styles/themes.py` & `ludic-0.4.7/ludic/styles/themes.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import ABCMeta, abstractmethod
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, TypeVar
 
-from .types import Color, ColorRange, Size
+from .types import BaseSize, Color, ColorRange, Size, SizeClamp
 
 if TYPE_CHECKING:
     from ludic.types import BaseElement
 
 _T = TypeVar("_T", bound="BaseElement")
 
 
@@ -28,122 +28,128 @@
     black: Color = Color("#222")
 
 
 @dataclass
 class Header:
     """Header for a theme."""
 
-    size: Size = Size(1.5, "em")
+    size: BaseSize = SizeClamp(1.5, 2, 2.5)
     anchor: bool = True
 
 
 @dataclass
 class Headers:
     """Headers for a theme."""
 
-    h1: Header = field(default_factory=lambda: Header(size=Size(3, "em"), anchor=False))
+    h1: Header = field(
+        default_factory=lambda: Header(size=SizeClamp(2, 1.5, 3.3), anchor=False)
+    )
     h2: Header = field(
-        default_factory=lambda: Header(size=Size(2.5, "em"), anchor=False)
+        default_factory=lambda: Header(size=SizeClamp(1.5, 1.3, 2.8), anchor=False)
+    )
+    h3: Header = field(
+        default_factory=lambda: Header(size=SizeClamp(1.2, 0.8, 2.2), anchor=False)
     )
-    h3: Header = field(default_factory=lambda: Header(size=Size(2, "em"), anchor=False))
     h4: Header = field(
-        default_factory=lambda: Header(size=Size(1.5, "em"), anchor=False)
+        default_factory=lambda: Header(size=SizeClamp(1, 0.6, 1.8), anchor=False)
     )
     h5: Header = field(
-        default_factory=lambda: Header(size=Size(1.25, "em"), anchor=False)
+        default_factory=lambda: Header(size=SizeClamp(0.7, 0.5, 1.3), anchor=False)
+    )
+    h6: Header = field(
+        default_factory=lambda: Header(size=SizeClamp(0.5, 0.4, 1.1), anchor=False)
     )
-    h6: Header = field(default_factory=lambda: Header(size=Size(1, "em"), anchor=False))
 
 
 @dataclass
 class Fonts:
     """Font sizes for a theme."""
 
     plain: str = "Helvetica Neue, Helvetica, Arial, sans-serif"
     serif: str = "Georgia, serif"
     mono: str = "Space Mono, Roboto Mono, monospace"
 
-    size: Size = Size(1, "em")
+    size: BaseSize = Size(1, "em")
 
 
 @dataclass
 class Sizes:
     """Size for a theme."""
 
-    xxxxs: Size = Size(0.39)
-    xxxs: Size = Size(0.47)
-    xxs: Size = Size(0.57)
-    xs: Size = Size(0.69)
-    s: Size = Size(0.84)
-    m: Size = Size(1)
-    l: Size = Size(1.16)  # noqa
-    xl: Size = Size(1.4)
-    xxl: Size = Size(1.68)
-    xxxl: Size = Size(2.01)
-    xxxxl: Size = Size(2.41)
+    xxxxs: BaseSize = SizeClamp(0.39, -0.5, 0.57)
+    xxxs: BaseSize = SizeClamp(0.47, -0.4, 0.84)
+    xxs: BaseSize = SizeClamp(0.57, -0.3, 1)
+    xs: BaseSize = SizeClamp(0.69, -0.2, 1.16)
+    s: BaseSize = SizeClamp(0.84, -0.1, 1.4)
+    m: BaseSize = SizeClamp(1, 0.01, 1.68)
+    l: BaseSize = SizeClamp(1.16, 0.1, 2.01)  # noqa
+    xl: BaseSize = SizeClamp(1.4, 0.2, 2.41)
+    xxl: BaseSize = SizeClamp(1.68, 0.3, 2.81)
+    xxxl: BaseSize = SizeClamp(2.01, 0.4, 3.41)
+    xxxxl: BaseSize = SizeClamp(2.41, 0.5, 4.01)
 
 
 @dataclass
 class Borders:
     """Border sizes for a theme."""
 
-    thin: Size = Size(0.1)
-    normal: Size = Size(0.23)
-    thick: Size = Size(0.42)
+    thin: BaseSize = Size(0.1)
+    normal: BaseSize = Size(0.23)
+    thick: BaseSize = Size(0.42)
 
 
 @dataclass
 class Rounding:
     """Border rounding for a theme."""
 
-    less: Size = Size(0.20)
-    normal: Size = Size(0.25)
-    more: Size = Size(0.35)
+    less: BaseSize = Size(0.20)
+    normal: BaseSize = Size(0.25)
+    more: BaseSize = Size(0.35)
 
 
 @dataclass
 class Sidebar:
     """Sidebar layout config for a theme."""
 
     # The width of the sidebar (empty means not set; defaults to the content width)
-    side_width: Size | None = None
+    side_width: str | None = None
 
     # The narrowest the content element can be before wrapping. Should be a percentage.
     content_min_width: str = "60%"
 
 
 @dataclass
 class Switcher:
     """Switcher layout config for a theme."""
 
     # The container width at which the component switches between a horizontal and
     # vertical layout
-    threshold: Size = Size(40, "rem")
+    threshold: BaseSize = Size(40, "rem")
 
     # The maximum number of elements allowed to appear in the horizontal configuration
     limit: int = 4
 
 
 @dataclass
 class Cover:
     """Cover layout config for a theme."""
 
     # The minimum height of the cover
-    min_height: Size = Size(100, "vh")
+    min_height: BaseSize = Size(100, "vh")
 
     # The minimum space between and around the child elements
     element: str = "h1"
 
 
 @dataclass
 class Grid:
     """Grid layout config for a theme."""
 
     # The size of the grid cells
-    cell_size: Size = Size(250, "px")
+    cell_size: BaseSize = Size(250, "px")
 
 
 @dataclass
 class Frame:
     """Frame layout config for a theme."""
 
     # The width of the frame
@@ -172,15 +178,15 @@
     style: str | type = "default"
 
 
 @dataclass
 class Theme(metaclass=ABCMeta):
     """An abstract base class for theme configuration."""
 
-    measure: Size = Size(70, "ch")
+    measure: BaseSize = Size(70, "ch")
     line_height: float = 1.5
 
     fonts: Fonts = field(default_factory=Fonts)
     colors: Colors = field(default_factory=Colors)
     sizes: Sizes = field(default_factory=Sizes)
 
     borders: Borders = field(default_factory=Borders)
```

### Comparing `ludic-0.4.6/ludic/styles/types.py` & `ludic-0.4.7/ludic/styles/types.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,35 @@
+from abc import ABCMeta, abstractmethod
 from collections.abc import Mapping
 from typing import Literal, LiteralString, Self, SupportsIndex, TypedDict
 
 from .utils import (
+    clamp,
     darken_color,
     hex_to_rgb,
     lighten_color,
     pick_readable_color_for,
 )
 
 SizeUnit = Literal["px", "ex", "em", "ch", "rem", "vw", "vh", "vmin", "vmax", "%"]
 
 
+def format_unit(value: float, unit: SizeUnit = "rem") -> str:
+    match unit:
+        case "px" | "ch":
+            formatted = f"{value:.0f}{unit}"
+        case _:
+            formatted = f"{value:.2f}".rstrip("0").rstrip(".")
+            if not formatted or formatted == "0":
+                formatted = f"0{unit}"
+            else:
+                formatted = f"{formatted}{unit}"
+    return formatted
+
+
 class Color(str):
     """Color class."""
 
     @property
     def rgb(self) -> tuple[int, int, int]:
         """RGB color."""
         return hex_to_rgb(self)
@@ -97,32 +112,38 @@
         """
         if 0 <= self.position + shift < len(self.variants):
             return type(self)(self.variants, self.position + shift)
         else:
             return type(self)(self.variants, len(self.variants) - 1)
 
 
-class Size(str):
+class BaseSize(str, metaclass=ABCMeta):
+    """Base size class."""
+
+    @abstractmethod
+    def __mul__(self, factor: float | int | LiteralString | SupportsIndex) -> Self:
+        pass
+
+    @abstractmethod
+    def __add__(self, value: float | int | LiteralString | SupportsIndex) -> Self:
+        pass
+
+    @abstractmethod
+    def __sub__(self, value: float | int | LiteralString | SupportsIndex) -> Self:
+        pass
+
+
+class Size(BaseSize):
     """Size class."""
 
     value: float
     unit: SizeUnit = "rem"
 
     def __new__(cls, value: float, unit: SizeUnit = "rem") -> "Size":
-        match unit:
-            case "px" | "ch":
-                self = super().__new__(cls, f"{value:.0f}{unit}")
-            case _:
-                formatted = f"{value:.2f}".rstrip("0").rstrip(".")
-                if not formatted or formatted == "0":
-                    formatted = "0"
-                else:
-                    formatted = f"{formatted}{unit}"
-                self = super().__new__(cls, formatted)
-
+        self = super().__new__(cls, format_unit(value, unit))
         self.value = value
         self.unit = unit
         return self
 
     def __mul__(self, factor: float | int | LiteralString | SupportsIndex) -> Self:
         """Scale size by a given factor.
 
@@ -162,14 +183,99 @@
         """
         if isinstance(value, float | int):
             return type(self)(self.value - value, self.unit)
         else:
             return self
 
 
+class SizeClamp(BaseSize):
+    """Size clamp class."""
+
+    minimum: float
+    value: float
+    maximum: float
+    base_unit: SizeUnit = "rem"
+    viewport_unit: SizeUnit = "vw"
+
+    def __new__(
+        cls,
+        minimum: float,
+        value: float,
+        maximum: float,
+        base_unit: SizeUnit = "rem",
+        viewport_unit: SizeUnit = "vw",
+    ) -> "SizeClamp":
+        self = super().__new__(
+            cls,
+            clamp(
+                format_unit(minimum, base_unit),
+                (
+                    f"{format_unit(minimum, base_unit)} + "
+                    f"{format_unit(value, viewport_unit)}"
+                ),
+                format_unit(maximum, base_unit),
+            ),
+        )
+
+        self.minimum = minimum
+        self.value = value
+        self.maximum = maximum
+        self.base_unit = base_unit
+        self.viewport_unit = viewport_unit
+        return self
+
+    def __mul__(self, factor: float | int | LiteralString | SupportsIndex) -> Self:
+        """Scale size by a given factor.
+
+        Args:
+            factor (float): Scaling factor.
+
+        Returns:
+            str: Scaled size.
+        """
+        if isinstance(factor, float | int):
+            return type(self)(
+                self.minimum * factor, self.value * factor, self.maximum * factor
+            )
+        else:
+            return self
+
+    def __add__(self, value: float | int | LiteralString | SupportsIndex) -> Self:
+        """Increment size by a given factor.
+
+        Args:
+            value (float, optional): Increment value.
+
+        Returns:
+            str: Incremented size.
+        """
+        if isinstance(value, float | int):
+            return type(self)(
+                self.minimum + value, self.value + value, self.maximum + value
+            )
+        else:
+            return self
+
+    def __sub__(self, value: float | int | LiteralString | SupportsIndex) -> Self:
+        """Decrement size by a given factor.
+
+        Args:
+            value (float, optional): Decrement value.
+
+        Returns:
+            str: Decremented size.
+        """
+        if isinstance(value, float | int):
+            return type(self)(
+                self.minimum - value, self.value - value, self.maximum - value
+            )
+        else:
+            return self
+
+
 CSSProperties = TypedDict(
     "CSSProperties",
     {
         # A
         "align-content": Literal[
             "center",
             "flex-start",
```

### Comparing `ludic-0.4.6/ludic/styles/utils.py` & `ludic-0.4.7/ludic/styles/utils.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/ludic/web/app.py` & `ludic-0.4.7/ludic/web/app.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/ludic/web/datastructures.py` & `ludic-0.4.7/ludic/web/datastructures.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/ludic/web/endpoints.py` & `ludic-0.4.7/ludic/web/endpoints.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/ludic/web/exceptions.py` & `ludic-0.4.7/ludic/web/exceptions.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/ludic/web/parsers.py` & `ludic-0.4.7/ludic/web/parsers.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/ludic/web/requests.py` & `ludic-0.4.7/ludic/web/requests.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/ludic/web/responses.py` & `ludic-0.4.7/ludic/web/responses.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/ludic/web/routing.py` & `ludic-0.4.7/ludic/web/routing.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/tests/test_components.py` & `ludic-0.4.7/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/tests/test_elements.py` & `ludic-0.4.7/tests/test_elements.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/tests/test_examples.py` & `ludic-0.4.7/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/tests/test_exceptions.py` & `ludic-0.4.7/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/tests/test_formatting.py` & `ludic-0.4.7/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/tests/test_types.py` & `ludic-0.4.7/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/tests/styles/__init__.py` & `ludic-0.4.7/tests/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/tests/styles/test_styles.py` & `ludic-0.4.7/tests/styles/test_styles.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/tests/styles/test_themes.py` & `ludic-0.4.7/tests/styles/test_themes.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from typing import override
 
 from ludic.attrs import GlobalAttrs
 from ludic.html import a, b, div, style
 from ludic.styles.themes import (
     Colors,
     Fonts,
+    Sizes,
     get_default_theme,
     set_default_theme,
 )
-from ludic.styles.types import Color, Size
+from ludic.styles.types import Color, Size, SizeClamp
 from ludic.types import Component
 
 from . import BarTheme, FooTheme
 
 
 def test_theme_colors() -> None:
     theme = FooTheme(
@@ -52,14 +53,27 @@
     assert theme.fonts.size + 5 == "15px"
     assert theme.fonts.size * 2 == "20px"
 
     assert theme.fonts.size + "2" == "10px"
     assert theme.fonts.size - "ab" == "10px"
 
 
+def test_theme_sizes() -> None:
+    theme = FooTheme(sizes=Sizes(m=SizeClamp(1, 1.2, 3)))
+
+    assert theme.sizes.m == "clamp(1rem, 1rem + 1.2vw, 3rem)"
+
+    assert theme.sizes.m - 0.1 == "clamp(0.9rem, 0.9rem + 1.1vw, 2.9rem)"
+    assert theme.sizes.m + 0.5 == "clamp(1.5rem, 1.5rem + 1.7vw, 3.5rem)"
+    assert theme.sizes.m * 0.2 == "clamp(0.2rem, 0.2rem + 0.24vw, 0.6rem)"
+
+    assert theme.sizes.m + "2" == "clamp(1rem, 1rem + 1.2vw, 3rem)"
+    assert theme.sizes.m - "ab" == "clamp(1rem, 1rem + 1.2vw, 3rem)"
+
+
 def test_themes_switching() -> None:
     foo, bar = FooTheme(), BarTheme()
 
     set_default_theme(foo)
     assert get_default_theme() == foo
     set_default_theme(bar)
     assert get_default_theme() == bar
```

#### html2text {}

```diff
@@ -1,40 +1,48 @@
 from typing import override from ludic.attrs import GlobalAttrs from ludic.html
-import a, b, div, style from ludic.styles.themes import ( Colors, Fonts,
+import a, b, div, style from ludic.styles.themes import ( Colors, Fonts, Sizes,
 get_default_theme, set_default_theme, ) from ludic.styles.types import Color,
-Size from ludic.types import Component from . import BarTheme, FooTheme def
-test_theme_colors() -> None: theme = FooTheme( colors=Colors( primary=Color
-("#c2e7fd"), white=Color("#fff"), light=Color("#eee"), dark=Color("#333"),
-black=Color("#000"), ) ) assert theme.colors.primary.rgb == (194, 231, 253)
-assert theme.colors.white.rgb == (255, 255, 255) assert theme.colors.light.rgb
-== (238, 238, 238) assert theme.colors.dark.rgb == (51, 51, 51) assert
-theme.colors.black.rgb == (0, 0, 0) assert theme.colors.white.darken(10).rgb ==
-(127, 127, 127) assert theme.colors.white.darken(20).rgb == (1, 1, 1) assert
+Size, SizeClamp from ludic.types import Component from . import BarTheme,
+FooTheme def test_theme_colors() -> None: theme = FooTheme( colors=Colors
+( primary=Color("#c2e7fd"), white=Color("#fff"), light=Color("#eee"),
+dark=Color("#333"), black=Color("#000"), ) ) assert theme.colors.primary.rgb ==
+(194, 231, 253) assert theme.colors.white.rgb == (255, 255, 255) assert
+theme.colors.light.rgb == (238, 238, 238) assert theme.colors.dark.rgb == (51,
+51, 51) assert theme.colors.black.rgb == (0, 0, 0) assert
+theme.colors.white.darken(10).rgb == (127, 127, 127) assert
+theme.colors.white.darken(20).rgb == (1, 1, 1) assert
 theme.colors.black.lighten(10).rgb == (127, 127, 127) assert
 theme.colors.black.lighten(20).rgb == (255, 255, 255) assert
 theme.colors.light.darken(10).rgb == (119, 119, 119) assert
 theme.colors.dark.lighten(10).rgb == (153, 153, 153) assert
 theme.colors.primary.darken(10).rgb == (97, 115, 126) def test_theme_font_sizes
 () -> None: theme = FooTheme(fonts=Fonts(size=Size(10, "px"))) assert
 theme.fonts.size == "10px" assert theme.fonts.plain == "Helvetica Neue,
 Helvetica, Arial, sans-serif" assert theme.fonts.size - 1 == "9px" assert
 theme.fonts.size + 5 == "15px" assert theme.fonts.size * 2 == "20px" assert
 theme.fonts.size + "2" == "10px" assert theme.fonts.size - "ab" == "10px" def
-test_themes_switching() -> None: foo, bar = FooTheme(), BarTheme()
-set_default_theme(foo) assert get_default_theme() == foo set_default_theme(bar)
-assert get_default_theme() == bar def test_element_theme_switching() -> None:
-foo = FooTheme() bar = BarTheme() set_default_theme(bar) class C1(Component
-[str, GlobalAttrs]): styles = style.use( lambda theme: { "#c1 a": {"color":
-theme.colors.warning}, } ) @override def render(self) -> div: return div( b
-("Hello, ", style={"color": self.theme.colors.secondary}), a(*self.children,
-href="https://example.com"), id="c1", ) class C2(Component[str, GlobalAttrs]):
-styles = style.use( lambda theme: { "#c2 a": {"color": theme.colors.danger}, }
-) @override def render(self) -> div: return div( foo.use(C1(*self.children)),
-id="c2", style={"background-color": self.theme.colors.primary}, ) assert C2
-("World").to_html() == ( f'
+test_theme_sizes() -> None: theme = FooTheme(sizes=Sizes(m=SizeClamp(1, 1.2,
+3))) assert theme.sizes.m == "clamp(1rem, 1rem + 1.2vw, 3rem)" assert
+theme.sizes.m - 0.1 == "clamp(0.9rem, 0.9rem + 1.1vw, 2.9rem)" assert
+theme.sizes.m + 0.5 == "clamp(1.5rem, 1.5rem + 1.7vw, 3.5rem)" assert
+theme.sizes.m * 0.2 == "clamp(0.2rem, 0.2rem + 0.24vw, 0.6rem)" assert
+theme.sizes.m + "2" == "clamp(1rem, 1rem + 1.2vw, 3rem)" assert theme.sizes.m -
+"ab" == "clamp(1rem, 1rem + 1.2vw, 3rem)" def test_themes_switching() -> None:
+foo, bar = FooTheme(), BarTheme() set_default_theme(foo) assert
+get_default_theme() == foo set_default_theme(bar) assert get_default_theme() ==
+bar def test_element_theme_switching() -> None: foo = FooTheme() bar = BarTheme
+() set_default_theme(bar) class C1(Component[str, GlobalAttrs]): styles =
+style.use( lambda theme: { "#c1 a": {"color": theme.colors.warning}, } )
+@override def render(self) -> div: return div( b("Hello, ", style={"color":
+self.theme.colors.secondary}), a(*self.children, href="https://example.com"),
+id="c1", ) class C2(Component[str, GlobalAttrs]): styles = style.use( lambda
+theme: { "#c2 a": {"color": theme.colors.danger}, } ) @override def render
+(self) -> div: return div( foo.use(C1(*self.children)), id="c2", style=
+{"background-color": self.theme.colors.primary}, ) assert C2("World").to_html()
+== ( f'
 ' '
 ' f'HHeelllloo,, ' '_W_o_r_l_d' "
 " "
 " ) # fmt: skip assert style.from_components(C1, C2).to_html() == ( '
 " ) # fmt: skip set_default_theme(foo) assert style.from_components(C1,
 C2).to_html() == ( '
 " ) # fmt: skip
```

### Comparing `ludic-0.4.6/.gitignore` & `ludic-0.4.7/.gitignore`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/LICENCE` & `ludic-0.4.7/LICENCE`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/README.md` & `ludic-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/pyproject.toml` & `ludic-0.4.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ludic-0.4.6/PKG-INFO` & `ludic-0.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ludic
-Version: 0.4.6
+Version: 0.4.7
 Summary: Lightweight framework for building dynamic HTML pages in pure Python.
 Author-email: Pavel Dedík <dedikx@gmail.com>
 Maintainer-email: Pavel Dedík <dedikx@gmail.com>
 License-Expression: MIT
 License-File: LICENCE
 Keywords: async,html,htmx,templating,web
 Classifier: Development Status :: 4 - Beta
```

