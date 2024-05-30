# Comparing `tmp/ludic-0.4.7.tar.gz` & `tmp/ludic-0.4.8.tar.gz`

## Comparing `ludic-0.4.7.tar` & `ludic-0.4.8.tar`

### file list

```diff
@@ -1,84 +1,84 @@
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 ludic-0.4.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 ludic-0.4.7/.readthedocs.yaml
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 ludic-0.4.7/CONTRIBUTING.md
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ludic-0.4.7/_version.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 ludic-0.4.7/mkdocs.yaml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ludic-0.4.7/.github/dependabot.yml
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 ludic-0.4.7/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 ludic-0.4.7/.github/workflows/test.yaml
--rw-r--r--   0        0        0     9401 2020-02-02 00:00:00.000000 ludic-0.4.7/docs/catalog.md
--rw-r--r--   0        0        0    11706 2020-02-02 00:00:00.000000 ludic-0.4.7/docs/components.md
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ludic-0.4.7/docs/examples.md
--rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 ludic-0.4.7/docs/getting-started.md
--rw-r--r--   0        0        0     3665 2020-02-02 00:00:00.000000 ludic-0.4.7/docs/htmx.md
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 ludic-0.4.7/docs/index.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 ludic-0.4.7/docs/requirements.txt
--rw-r--r--   0        0        0     9658 2020-02-02 00:00:00.000000 ludic-0.4.7/docs/styles.md
--rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 ludic-0.4.7/docs/web-framework.md
--rw-r--r--   0        0        0   127587 2020-02-02 00:00:00.000000 ludic-0.4.7/docs/assets/ludic.png
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 ludic-0.4.7/examples/README.md
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 ludic-0.4.7/examples/__init__.py
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 ludic-0.4.7/examples/bulk_update.py
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 ludic-0.4.7/examples/click_to_edit.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 ludic-0.4.7/examples/click_to_load.py
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 ludic-0.4.7/examples/delete_row.py
--rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 ludic-0.4.7/examples/edit_row.py
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 ludic-0.4.7/examples/infinite_scroll.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 ludic-0.4.7/examples/lazy_loading.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/__init__.py
--rw-r--r--   0        0        0    16536 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/attrs.py
--rw-r--r--   0        0        0    10039 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/base.py
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/components.py
--rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/format.py
--rw-r--r--   0        0        0    12137 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/html.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/py.typed
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/types.py
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/utils.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/catalog/__init__.py
--rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/catalog/buttons.py
--rw-r--r--   0        0        0     8599 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/catalog/forms.py
--rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/catalog/headers.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/catalog/icons.py
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/catalog/items.py
--rw-r--r--   0        0        0     9271 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/catalog/layouts.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/catalog/lists.py
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/catalog/loaders.py
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/catalog/messages.py
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/catalog/navigation.py
--rw-r--r--   0        0        0     6982 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/catalog/pages.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/catalog/quotes.py
--rw-r--r--   0        0        0     7091 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/catalog/tables.py
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/catalog/typography.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/catalog/utils.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/styles/__init__.py
--rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/styles/collect.py
--rw-r--r--   0        0        0     6614 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/styles/themes.py
--rw-r--r--   0        0        0    27206 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/styles/types.py
--rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/styles/utils.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/web/__init__.py
--rw-r--r--   0        0        0     8202 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/web/app.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/web/datastructures.py
--rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/web/endpoints.py
--rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/web/exceptions.py
--rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/web/parsers.py
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/web/requests.py
--rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/web/responses.py
--rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 ludic-0.4.7/ludic/web/routing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.7/tests/__init__.py
--rw-r--r--   0        0        0     6868 2020-02-02 00:00:00.000000 ludic-0.4.7/tests/test_components.py
--rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 ludic-0.4.7/tests/test_elements.py
--rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 ludic-0.4.7/tests/test_examples.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 ludic-0.4.7/tests/test_exceptions.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 ludic-0.4.7/tests/test_formatting.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ludic-0.4.7/tests/test_types.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 ludic-0.4.7/tests/styles/__init__.py
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 ludic-0.4.7/tests/styles/test_styles.py
--rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 ludic-0.4.7/tests/styles/test_themes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.7/tests/web/__init__.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 ludic-0.4.7/tests/web/test_datastructures.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 ludic-0.4.7/tests/web/test_requests.py
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 ludic-0.4.7/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 ludic-0.4.7/LICENCE
--rw-r--r--   0        0        0     6269 2020-02-02 00:00:00.000000 ludic-0.4.7/README.md
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 ludic-0.4.7/pyproject.toml
--rw-r--r--   0        0        0     7574 2020-02-02 00:00:00.000000 ludic-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 ludic-0.4.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 ludic-0.4.8/.readthedocs.yaml
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 ludic-0.4.8/CONTRIBUTING.md
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ludic-0.4.8/_version.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 ludic-0.4.8/mkdocs.yaml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ludic-0.4.8/.github/dependabot.yml
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 ludic-0.4.8/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 ludic-0.4.8/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     9401 2020-02-02 00:00:00.000000 ludic-0.4.8/docs/catalog.md
+-rw-r--r--   0        0        0    11706 2020-02-02 00:00:00.000000 ludic-0.4.8/docs/components.md
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ludic-0.4.8/docs/examples.md
+-rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 ludic-0.4.8/docs/getting-started.md
+-rw-r--r--   0        0        0     3665 2020-02-02 00:00:00.000000 ludic-0.4.8/docs/htmx.md
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 ludic-0.4.8/docs/index.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 ludic-0.4.8/docs/requirements.txt
+-rw-r--r--   0        0        0     9658 2020-02-02 00:00:00.000000 ludic-0.4.8/docs/styles.md
+-rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 ludic-0.4.8/docs/web-framework.md
+-rw-r--r--   0        0        0   127587 2020-02-02 00:00:00.000000 ludic-0.4.8/docs/assets/ludic.png
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 ludic-0.4.8/examples/README.md
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 ludic-0.4.8/examples/__init__.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 ludic-0.4.8/examples/bulk_update.py
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 ludic-0.4.8/examples/click_to_edit.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 ludic-0.4.8/examples/click_to_load.py
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 ludic-0.4.8/examples/delete_row.py
+-rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 ludic-0.4.8/examples/edit_row.py
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 ludic-0.4.8/examples/infinite_scroll.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 ludic-0.4.8/examples/lazy_loading.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/__init__.py
+-rw-r--r--   0        0        0    16536 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/attrs.py
+-rw-r--r--   0        0        0    10039 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/base.py
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/components.py
+-rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/format.py
+-rw-r--r--   0        0        0    12137 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/html.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/py.typed
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/types.py
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/utils.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/catalog/__init__.py
+-rw-r--r--   0        0        0     4515 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/catalog/buttons.py
+-rw-r--r--   0        0        0     8600 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/catalog/forms.py
+-rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/catalog/headers.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/catalog/icons.py
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/catalog/items.py
+-rw-r--r--   0        0        0     9261 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/catalog/layouts.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/catalog/lists.py
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/catalog/loaders.py
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/catalog/messages.py
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/catalog/navigation.py
+-rw-r--r--   0        0        0     7378 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/catalog/pages.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/catalog/quotes.py
+-rw-r--r--   0        0        0     7216 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/catalog/tables.py
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/catalog/typography.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/catalog/utils.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/styles/__init__.py
+-rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/styles/collect.py
+-rw-r--r--   0        0        0     6611 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/styles/themes.py
+-rw-r--r--   0        0        0    27206 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/styles/types.py
+-rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/styles/utils.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/web/__init__.py
+-rw-r--r--   0        0        0     8202 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/web/app.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/web/datastructures.py
+-rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/web/endpoints.py
+-rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/web/exceptions.py
+-rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/web/parsers.py
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/web/requests.py
+-rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/web/responses.py
+-rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 ludic-0.4.8/ludic/web/routing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.8/tests/__init__.py
+-rw-r--r--   0        0        0     6937 2020-02-02 00:00:00.000000 ludic-0.4.8/tests/test_components.py
+-rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 ludic-0.4.8/tests/test_elements.py
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 ludic-0.4.8/tests/test_examples.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 ludic-0.4.8/tests/test_exceptions.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 ludic-0.4.8/tests/test_formatting.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ludic-0.4.8/tests/test_types.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 ludic-0.4.8/tests/styles/__init__.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 ludic-0.4.8/tests/styles/test_styles.py
+-rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 ludic-0.4.8/tests/styles/test_themes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.8/tests/web/__init__.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 ludic-0.4.8/tests/web/test_datastructures.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 ludic-0.4.8/tests/web/test_requests.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 ludic-0.4.8/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 ludic-0.4.8/LICENCE
+-rw-r--r--   0        0        0     6269 2020-02-02 00:00:00.000000 ludic-0.4.8/README.md
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 ludic-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0     7574 2020-02-02 00:00:00.000000 ludic-0.4.8/PKG-INFO
```

### Comparing `ludic-0.4.7/.pre-commit-config.yaml` & `ludic-0.4.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/CONTRIBUTING.md` & `ludic-0.4.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/mkdocs.yaml` & `ludic-0.4.8/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/.github/workflows/publish.yaml` & `ludic-0.4.8/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/.github/workflows/test.yaml` & `ludic-0.4.8/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/docs/catalog.md` & `ludic-0.4.8/docs/catalog.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/docs/components.md` & `ludic-0.4.8/docs/components.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/docs/getting-started.md` & `ludic-0.4.8/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/docs/htmx.md` & `ludic-0.4.8/docs/htmx.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/docs/index.md` & `ludic-0.4.8/docs/index.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/docs/styles.md` & `ludic-0.4.8/docs/styles.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/docs/web-framework.md` & `ludic-0.4.8/docs/web-framework.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/docs/assets/ludic.png` & `ludic-0.4.8/docs/assets/ludic.png`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/examples/README.md` & `ludic-0.4.8/examples/README.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/examples/__init__.py` & `ludic-0.4.8/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/examples/bulk_update.py` & `ludic-0.4.8/examples/bulk_update.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/examples/click_to_edit.py` & `ludic-0.4.8/examples/click_to_edit.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/examples/click_to_load.py` & `ludic-0.4.8/examples/click_to_load.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/examples/delete_row.py` & `ludic-0.4.8/examples/delete_row.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/examples/edit_row.py` & `ludic-0.4.8/examples/edit_row.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/examples/infinite_scroll.py` & `ludic-0.4.8/examples/infinite_scroll.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/examples/lazy_loading.py` & `ludic-0.4.8/examples/lazy_loading.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/ludic/attrs.py` & `ludic-0.4.8/ludic/attrs.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/ludic/base.py` & `ludic-0.4.8/ludic/base.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/ludic/components.py` & `ludic-0.4.8/ludic/components.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/ludic/format.py` & `ludic-0.4.8/ludic/format.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/ludic/html.py` & `ludic-0.4.8/ludic/html.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/ludic/types.py` & `ludic-0.4.8/ludic/types.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/ludic/utils.py` & `ludic-0.4.8/ludic/utils.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/ludic/catalog/buttons.py` & `ludic-0.4.8/ludic/catalog/buttons.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     styles = style.use(
         lambda theme: {
             ".btn": {
                 "display": "inline-block",
                 "text-decoration": "none",
                 "background-color": theme.colors.light,
                 "color": theme.colors.black,
-                "padding": f"{theme.sizes.xxxxs * 0.8} {theme.sizes.s}",
+                "padding": f"{theme.sizes.xxxxs * 0.8} {theme.sizes.xs}",
                 "border": "none",
                 "border-radius": theme.rounding.normal,
                 "cursor": "pointer",
                 "font-size": theme.fonts.size,
                 "transition": "0.1s filter linear, 0.1s -webkit-filter linear",
             },
             ":not(a).btn": {
```

### Comparing `ludic-0.4.7/ludic/catalog/forms.py` & `ludic-0.4.8/ludic/catalog/forms.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
             ".form-field label": {
                 "display": "block",
                 "font-weight": "bold",
                 "margin-block-end": theme.sizes.xxs,
             },
             (".form-field input", ".form-field textarea", ".form-field select"): {
                 "inline-size": "100%",
-                "padding": f"{theme.sizes.xxxs} {theme.sizes.xs}",
+                "padding": f"{theme.sizes.xxxxs} {theme.sizes.xs}",
                 "border": (
                     f"{theme.borders.thin} solid {theme.colors.light.darken(2)}"
                 ),
                 "border-radius": theme.rounding.normal,
                 "box-sizing": "border-box",
                 "font-size": theme.fonts.size * 0.9,
                 "transition": "all 0.3s ease-in-out",
```

### Comparing `ludic-0.4.7/ludic/catalog/headers.py` & `ludic-0.4.8/ludic/catalog/headers.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,26 +50,30 @@
                 "display": "flex",
                 "flex-wrap": "wrap",
                 "justify-content": "flex-start",
             },
             ".with-anchor > h1 + a": {
                 "margin-inline-start": theme.sizes.m,
                 "font-size": theme.headers.h1.size,
+                "line-height": round(theme.line_height * 0.9, 2),
             },
             ".with-anchor > h2 + a": {
                 "margin-inline-start": theme.sizes.s,
                 "font-size": theme.headers.h2.size,
+                "line-height": round(theme.line_height * 0.9, 2),
             },
             ".with-anchor > h3 + a": {
                 "margin-inline-start": theme.sizes.xs,
                 "font-size": theme.headers.h3.size,
+                "line-height": round(theme.line_height * 0.9, 2),
             },
             ".with-anchor > h4 + a": {
                 "margin-inline-start": theme.sizes.xxs,
                 "font-size": theme.headers.h4.size,
+                "line-height": round(theme.line_height * 0.9, 2),
             },
         }
     )
 
     @override
     def render(self) -> div:
         element: h1 | h2 | h3 | h4
```

### Comparing `ludic-0.4.7/ludic/catalog/icons.py` & `ludic-0.4.8/ludic/catalog/icons.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/ludic/catalog/items.py` & `ludic-0.4.8/ludic/catalog/items.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/ludic/catalog/layouts.py` & `ludic-0.4.8/ludic/catalog/layouts.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,21 +37,21 @@
             ".stack.recursive *": {
                 "margin-block": "0",
             },
             ".stack.recursive * + *": {
                 "margin-block-start": theme.sizes.xl,
             },
             ".stack.tiny > * + *": {
-                "margin-block-start": theme.sizes.xxxxs,
+                "margin-block-start": theme.sizes.xxxs,
             },
             ".stack.small > * + *": {
                 "margin-block-start": theme.sizes.s,
             },
             ".stack.large > * + *": {
-                "margin-block-start": theme.sizes.xxxxl,
+                "margin-block-start": theme.sizes.xxxl,
             },
         }
     )
 
 
 class Box(div):
     """A component which applies padding from all sides.
@@ -69,22 +69,22 @@
         )
     """
 
     classes = ["box"]
     styles = style.use(
         lambda theme: {
             ".box": {
-                "padding": theme.sizes.l,
+                "padding": theme.sizes.m,
                 "color": theme.colors.dark,
             },
             ".box.small": {
-                "padding": theme.sizes.s,
+                "padding": theme.sizes.xs,
             },
             ".box.large": {
-                "padding": theme.sizes.xxl,
+                "padding": theme.sizes.xl,
             },
             ".box:not(.transparent)": {
                 "border": (
                     f"{theme.borders.thin} solid {theme.colors.light.darken(1)}"
                 ),
                 "border-radius": theme.rounding.more,
                 "background-color": theme.colors.light,
@@ -116,16 +116,16 @@
     classes = ["center"]
     styles = style.use(
         lambda theme: {
             ".center": {
                 "box-sizing": "content-box",
                 "margin-inline": "auto",
                 "max-inline-size": theme.measure,
-                "padding-inline-start": theme.sizes.xxxl,
-                "padding-inline-end": theme.sizes.xxxl,
+                "padding-inline-start": theme.sizes.xxl,
+                "padding-inline-end": theme.sizes.xxl,
             }
         }
     )
 
 
 class Cluster(div):
     """A component for inline children to be rendered in a row.
@@ -192,15 +192,15 @@
 
     classes = ["with-sidebar"]
     styles = style.use(
         lambda theme: {
             ".with-sidebar": {
                 "display": "flex",
                 "flex-wrap": "wrap",
-                "gap": theme.sizes.xxxxl,
+                "gap": theme.sizes.xxl,
             },
             ".with-sidebar > .sidebar": (
                 {
                     "flex-basis": theme.layouts.sidebar.side_width,
                     "flex-grow": 1,
                 }
                 if theme.layouts.sidebar.side_width
@@ -238,15 +238,15 @@
 
     classes = ["switcher"]
     styles = style.use(
         lambda theme: {
             ".switcher": {
                 "display": "flex",
                 "flex-wrap": "wrap",
-                "gap": theme.sizes.xxl,
+                "gap": theme.sizes.xl,
             },
             ".switcher > *": {
                 "flex-grow": 1,
                 "flex-basis": (
                     f"calc(({theme.layouts.switcher.threshold} - 100%) * 999)"
                 ),
             },
@@ -273,18 +273,18 @@
     classes = ["cover"]
     styles = style.use(
         lambda theme: {
             ".cover": {
                 "display": "flex",
                 "flex-direction": "column",
                 "min-block-size": theme.layouts.cover.min_height,
-                "padding": theme.sizes.xxl,
+                "padding": theme.sizes.xl,
             },
             ".cover > *": {
-                "margin-block": theme.sizes.xxl,
+                "margin-block": theme.sizes.xl,
             },
             f".cover > :first-child:not({theme.layouts.cover.element})": {
                 "margin-block-start": "0",
             },
             f".cover > :last-child:not({theme.layouts.cover.element})": {
                 "margin-block-end": "0",
             },
@@ -307,15 +307,15 @@
     """
 
     classes = ["grid"]
     styles = style.use(
         lambda theme: {
             ".grid": {
                 "display": "grid",
-                "grid-gap": theme.sizes.xxl,
+                "grid-gap": theme.sizes.xl,
             },
             f"@supports (width: min({theme.layouts.grid.cell_size}, 100%))": {
                 ".grid": {
                     "grid-template-columns": (
                         "repeat("
                         "auto-fit,"
                         f"minmax(min({theme.layouts.grid.cell_size},"
```

### Comparing `ludic-0.4.7/ludic/catalog/lists.py` & `ludic-0.4.8/ludic/catalog/lists.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/ludic/catalog/loaders.py` & `ludic-0.4.8/ludic/catalog/loaders.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/ludic/catalog/messages.py` & `ludic-0.4.8/ludic/catalog/messages.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/ludic/catalog/navigation.py` & `ludic-0.4.8/ludic/catalog/navigation.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/ludic/catalog/pages.py` & `ludic-0.4.8/ludic/catalog/pages.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,34 +64,40 @@
             ("html", "body", "div", "header", "nav", "main", "footer"): {
                 "max-inline-size": "none",
             },
             # elements styling
             "h1": {
                 "font-size": theme.headers.h1.size,
                 "font-family": theme.fonts.serif,
+                "line-height": round(theme.line_height * 0.9, 2),
             },
             "h2": {
                 "font-size": theme.headers.h2.size,
                 "font-family": theme.fonts.serif,
+                "line-height": round(theme.line_height * 0.9, 2),
             },
             "h3": {
                 "font-size": theme.headers.h3.size,
                 "font-family": theme.fonts.serif,
+                "line-height": round(theme.line_height * 0.9, 2),
             },
             "h4": {
                 "font-size": theme.headers.h4.size,
                 "font-family": theme.fonts.serif,
+                "line-height": round(theme.line_height * 0.9, 2),
             },
             "h5": {
                 "font-size": theme.headers.h5.size,
                 "font-family": theme.fonts.serif,
+                "line-height": round(theme.line_height * 0.9, 2),
             },
             "h6": {
                 "font-size": theme.headers.h6.size,
                 "font-family": theme.fonts.serif,
+                "line-height": round(theme.line_height * 0.9, 2),
             },
             "a": {
                 "color": theme.colors.primary.darken(2),
                 "text-decoration": "none",
             },
             "a:hover": {
                 "text-decoration": "underline",
@@ -114,18 +120,18 @@
             "dt": {
                 "font-weight": "bold",
             },
             "dd": {
                 "margin-left": "0",
             },
             ("ul", "ol"): {
-                "padding-inline-start": theme.sizes.xxl,
+                "padding-inline-start": theme.sizes.xl,
             },
             ("ul > li + li", "ol > li + li", "li > * + *"): {
-                "margin-block-start": theme.sizes.xs,
+                "margin-block-start": theme.sizes.xxs,
             },
             "ul > li::marker": {
                 "font-size": theme.fonts.size * 1.2,
             },
             ("img", "svg"): {
                 "width": "100%",
             },
```

### Comparing `ludic-0.4.7/ludic/catalog/quotes.py` & `ludic-0.4.8/ludic/catalog/quotes.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/ludic/catalog/tables.py` & `ludic-0.4.8/ludic/catalog/tables.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from collections.abc import Callable
 from dataclasses import dataclass
 from typing import Any, Literal, cast, get_type_hints, override
 
 from typing_extensions import TypeVar
 
 from ludic.attrs import GlobalAttrs
-from ludic.html import style, table, tbody, td, th, thead, tr
+from ludic.html import div, style, table, tbody, td, th, thead, tr
 from ludic.types import (
     AnyChildren,
     BaseElement,
     Component,
     ComponentStrict,
     PrimitiveChildren,
     TAttrs,
@@ -124,15 +124,18 @@
             PersonRow("John", 42),
         )
     """
 
     classes = ["table"]
     styles = style.use(
         lambda theme: {
-            "table.table": {
+            ".table": {
+                "overflow": "auto",
+            },
+            ".table > table": {
                 "inline-size": "100%",  # type: ignore
                 "border-collapse": "collapse",  # type: ignore
                 "thead": {
                     "background-color": theme.colors.light,
                 },
                 "tr th": {
                     "border": (
@@ -167,19 +170,21 @@
             for row in rows:
                 if value := row.get_value(idx):
                     result.append(value)
 
         return result
 
     @override
-    def render(self) -> table:
-        return table(
-            thead(self.children[0], **self.attrs.get("head_attrs", {})),
-            tbody(*self.children[1:], **self.attrs.get("body_attrs", {})),
-            **self.attrs_for(table),
+    def render(self) -> div:
+        return div(
+            table(
+                thead(self.children[0], **self.attrs.get("head_attrs", {})),
+                tbody(*self.children[1:], **self.attrs.get("body_attrs", {})),
+                **self.attrs_for(table),
+            ),
         )
 
 
 def create_rows(
     attrs_list: list[TAttrs], spec: type[TAttrs], include_id_column: bool = True
 ) -> tuple[TableHead, *tuple[TableRow, ...]]:
     """Create table rows from the given attributes.
```

### Comparing `ludic-0.4.7/ludic/catalog/typography.py` & `ludic-0.4.8/ludic/catalog/typography.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/ludic/catalog/utils.py` & `ludic-0.4.8/ludic/catalog/utils.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/ludic/styles/collect.py` & `ludic-0.4.8/ludic/styles/collect.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/ludic/styles/themes.py` & `ludic-0.4.8/ludic/styles/themes.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,25 +71,25 @@
     size: BaseSize = Size(1, "em")
 
 
 @dataclass
 class Sizes:
     """Size for a theme."""
 
-    xxxxs: BaseSize = SizeClamp(0.39, -0.5, 0.57)
-    xxxs: BaseSize = SizeClamp(0.47, -0.4, 0.84)
-    xxs: BaseSize = SizeClamp(0.57, -0.3, 1)
-    xs: BaseSize = SizeClamp(0.69, -0.2, 1.16)
-    s: BaseSize = SizeClamp(0.84, -0.1, 1.4)
-    m: BaseSize = SizeClamp(1, 0.01, 1.68)
-    l: BaseSize = SizeClamp(1.16, 0.1, 2.01)  # noqa
-    xl: BaseSize = SizeClamp(1.4, 0.2, 2.41)
-    xxl: BaseSize = SizeClamp(1.68, 0.3, 2.81)
-    xxxl: BaseSize = SizeClamp(2.01, 0.4, 3.41)
-    xxxxl: BaseSize = SizeClamp(2.41, 0.5, 4.01)
+    xxxxs: BaseSize = SizeClamp(0.39, 0, 0.47)
+    xxxs: BaseSize = SizeClamp(0.47, 0.1, 0.69)
+    xxs: BaseSize = SizeClamp(0.57, 0.15, 0.69)
+    xs: BaseSize = SizeClamp(0.69, 0.2, 0.84)
+    s: BaseSize = SizeClamp(0.84, 0.25, 1)
+    m: BaseSize = SizeClamp(1, 0.3, 1.16)
+    l: BaseSize = SizeClamp(1.16, 0.35, 1.4)  # noqa
+    xl: BaseSize = SizeClamp(1.4, 0.4, 1.68)
+    xxl: BaseSize = SizeClamp(1.68, 0.45, 2.01)
+    xxxl: BaseSize = SizeClamp(2.01, 0.5, 2.41)
+    xxxxl: BaseSize = SizeClamp(2.41, 0.55, 2.88)
 
 
 @dataclass
 class Borders:
     """Border sizes for a theme."""
 
     thin: BaseSize = Size(0.1)
```

### Comparing `ludic-0.4.7/ludic/styles/types.py` & `ludic-0.4.8/ludic/styles/types.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/ludic/styles/utils.py` & `ludic-0.4.8/ludic/styles/utils.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/ludic/web/app.py` & `ludic-0.4.8/ludic/web/app.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/ludic/web/datastructures.py` & `ludic-0.4.8/ludic/web/datastructures.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/ludic/web/endpoints.py` & `ludic-0.4.8/ludic/web/endpoints.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/ludic/web/exceptions.py` & `ludic-0.4.8/ludic/web/exceptions.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/ludic/web/parsers.py` & `ludic-0.4.8/ludic/web/parsers.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/ludic/web/requests.py` & `ludic-0.4.8/ludic/web/requests.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/ludic/web/responses.py` & `ludic-0.4.8/ludic/web/responses.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/ludic/web/routing.py` & `ludic-0.4.8/ludic/web/routing.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/tests/test_components.py` & `ludic-0.4.8/tests/test_components.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,23 +93,25 @@
     assert table.getlist("Age") == [42, 43]
     assert table.getlist("NOT_FOUND") == []
 
     assert len(table.children) > 2
     assert table.children[2].get_value(123) is None
 
     assert table.to_html() == (
-        '<table class="table">'
-            "<thead>"
-                '<tr><th>Name</th><th>Age</th></tr>'
-            "</thead>"
-            "<tbody>"
-                '<tr><td>John</td><td>42</td></tr>'
-                '<tr><td>Jane</td><td>43</td></tr>'
-            "</tbody>"
-        "</table>"
+        '<div class="table">'
+            "<table>"
+                "<thead>"
+                    '<tr><th>Name</th><th>Age</th></tr>'
+                "</thead>"
+                "<tbody>"
+                    '<tr><td>John</td><td>42</td></tr>'
+                    '<tr><td>Jane</td><td>43</td></tr>'
+                "</tbody>"
+            "</table>"
+        "</div>"
     )  # fmt: skip
 
 
 def test_form_fields() -> None:
     form = Form(
         InputField(value="Name", name="name"),
         TextAreaField("Description", name="description"),
```

#### html2text {}

```diff
@@ -27,17 +27,19 @@
 ' '
 " ) # fmt: skip def test_tables() -> None: table = Table( TableHead("Name",
 "Age"), TableRow("John", 42), TableRow("Jane", 43), ) assert table.header ==
 ("Name", "Age") assert table.getlist("Name") == ["John", "Jane"] assert
 table.getlist("Age") == [42, 43] assert table.getlist("NOT_FOUND") == [] assert
 len(table.children) > 2 assert table.children[2].get_value(123) is None assert
 table.to_html() == ( '
+' "
 NNaammee AAggee
 John 42
 Jane 43
+" "
 " ) # fmt: skip def test_form_fields() -> None: form = Form( InputField
 (value="Name", name="name"), TextAreaField("Description", name="description"),
 ) assert form.to_html() == ( '
 ' '
 ' '[Name                ]' "
 " '
 ' '
```

### Comparing `ludic-0.4.7/tests/test_elements.py` & `ludic-0.4.8/tests/test_elements.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/tests/test_examples.py` & `ludic-0.4.8/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/tests/test_exceptions.py` & `ludic-0.4.8/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/tests/test_formatting.py` & `ludic-0.4.8/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/tests/test_types.py` & `ludic-0.4.8/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/tests/styles/__init__.py` & `ludic-0.4.8/tests/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/tests/styles/test_styles.py` & `ludic-0.4.8/tests/styles/test_styles.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/tests/styles/test_themes.py` & `ludic-0.4.8/tests/styles/test_themes.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/.gitignore` & `ludic-0.4.8/.gitignore`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/LICENCE` & `ludic-0.4.8/LICENCE`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/README.md` & `ludic-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/pyproject.toml` & `ludic-0.4.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ludic-0.4.7/PKG-INFO` & `ludic-0.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ludic
-Version: 0.4.7
+Version: 0.4.8
 Summary: Lightweight framework for building dynamic HTML pages in pure Python.
 Author-email: Pavel Dedík <dedikx@gmail.com>
 Maintainer-email: Pavel Dedík <dedikx@gmail.com>
 License-Expression: MIT
 License-File: LICENCE
 Keywords: async,html,htmx,templating,web
 Classifier: Development Status :: 4 - Beta
```

