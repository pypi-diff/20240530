# Comparing `tmp/pyeconomics-0.1.0.tar.gz` & `tmp/pyeconomics-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyeconomics-0.1.0.tar", last modified: Mon May  6 02:28:57 2024, max compression
+gzip compressed data, was "pyeconomics-0.2.0.tar", last modified: Thu May 30 01:41:25 2024, max compression
```

## Comparing `pyeconomics-0.1.0.tar` & `pyeconomics-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,111 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 02:28:57.416331 pyeconomics-0.1.0/
--rw-rw-rw-   0        0        0     1096 2024-05-06 02:25:23.000000 pyeconomics-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      499 2024-05-06 02:28:57.413334 pyeconomics-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-03 23:57:54.000000 pyeconomics-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 02:28:57.393716 pyeconomics-0.1.0/pyeconomics/
--rw-rw-rw-   0        0        0        0 2024-05-03 23:58:19.000000 pyeconomics-0.1.0/pyeconomics/__init__.py
--rw-rw-rw-   0        0        0     4213 2024-05-05 08:24:21.000000 pyeconomics-0.1.0/pyeconomics/api.py
--rw-rw-rw-   0        0        0        0 2024-05-06 01:35:49.000000 pyeconomics-0.1.0/pyeconomics/balanced_approach_rule.py
--rw-rw-rw-   0        0        0        0 2024-05-06 01:36:09.000000 pyeconomics-0.1.0/pyeconomics/balanced_approach_shortfalls_rule.py
--rw-rw-rw-   0        0        0        0 2024-05-06 01:36:22.000000 pyeconomics-0.1.0/pyeconomics/first_difference_rule.py
--rw-rw-rw-   0        0        0      909 2024-05-06 01:43:38.000000 pyeconomics-0.1.0/pyeconomics/fred_data.py
--rw-rw-rw-   0        0        0        0 2024-05-03 23:58:53.000000 pyeconomics-0.1.0/pyeconomics/quantity_of_money.py
--rw-rw-rw-   0        0        0        0 2024-05-03 23:59:03.000000 pyeconomics-0.1.0/pyeconomics/stock_to_flow.py
--rw-rw-rw-   0        0        0    10272 2024-05-06 01:46:57.000000 pyeconomics-0.1.0/pyeconomics/taylor_rule.py
-drwxrwxrwx   0        0        0        0 2024-05-06 02:28:57.408334 pyeconomics-0.1.0/pyeconomics.egg-info/
--rw-rw-rw-   0        0        0      499 2024-05-06 02:28:57.000000 pyeconomics-0.1.0/pyeconomics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      465 2024-05-06 02:28:57.000000 pyeconomics-0.1.0/pyeconomics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 02:28:57.000000 pyeconomics-0.1.0/pyeconomics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-05-06 02:28:57.000000 pyeconomics-0.1.0/pyeconomics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 02:28:57.417332 pyeconomics-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      737 2024-05-06 01:58:50.000000 pyeconomics-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 02:28:57.411334 pyeconomics-0.1.0/tests/
--rw-rw-rw-   0        0        0        0 2024-05-06 01:51:07.000000 pyeconomics-0.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:41:25.947462 pyeconomics-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:41:25.931462 pyeconomics-0.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:41:25.931462 pyeconomics-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    23724 2024-05-30 01:41:25.947462 pyeconomics-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22439 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:41:25.935462 pyeconomics-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:41:25.935462 pyeconomics-0.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    69539 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:41:25.935462 pyeconomics-0.2.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/_templates/.keep
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/api_key.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/contact.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/create_roadmap_files.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/docker.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/features.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    19195 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/roadmap.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/roadmap_discounted_cash_flow_models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/roadmap_exchange_rate_models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/roadmap_financial_models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/roadmap_fiscal_policy_models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/roadmap_macroeconomic_models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/roadmap_microeconomic_models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/roadmap_monetary_policy_models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/roadmap_other_economic_models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/roadmap_quantity_of_money_theory.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10580 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:41:25.927462 pyeconomics-0.2.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:41:25.939462 pyeconomics-0.2.0/examples/api_configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/examples/api_configuration/fred_api_configuration.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:41:25.939462 pyeconomics-0.2.0/examples/monetary_policy_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)   214512 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/examples/monetary_policy_rules/balanced_approach_rule.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   125883 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/examples/monetary_policy_rules/first_difference_rule.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   286474 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/examples/monetary_policy_rules/monetary_policy_rules.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   118525 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/examples/monetary_policy_rules/taylor_rule.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:41:25.939462 pyeconomics-0.2.0/markdown/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/markdown/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/markdown/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/markdown/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/markdown/FRED_API_CONFIGURATION.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:41:25.939462 pyeconomics-0.2.0/media/
+-rw-r--r--   0 runner    (1001) docker     (127)   181489 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/media/plot_adj_historical_rates.png
+-rw-r--r--   0 runner    (1001) docker     (127)   181531 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/media/plot_historical_policy_rates.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:41:25.939462 pyeconomics-0.2.0/pyeconomics/
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyeconomics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyeconomics/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:41:25.943462 pyeconomics-0.2.0/pyeconomics/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyeconomics/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyeconomics/api/cache_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7668 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyeconomics/api/fred_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyeconomics/api/fred_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:41:25.943462 pyeconomics-0.2.0/pyeconomics/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyeconomics/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyeconomics/data/economic_indicators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyeconomics/data/model_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:41:25.943462 pyeconomics-0.2.0/pyeconomics/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyeconomics/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:41:25.943462 pyeconomics-0.2.0/pyeconomics/models/monetary_policy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyeconomics/models/monetary_policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9556 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyeconomics/models/monetary_policy/balanced_approach_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyeconomics/models/monetary_policy/first_difference_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12879 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyeconomics/models/monetary_policy/monetary_policy_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8327 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyeconomics/models/monetary_policy/taylor_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:41:25.943462 pyeconomics-0.2.0/pyeconomics/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyeconomics/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6728 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyeconomics/utils/bar_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyeconomics/utils/fdr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyeconomics/utils/tr_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:41:25.939462 pyeconomics-0.2.0/pyeconomics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23724 2024-05-30 01:41:25.000000 pyeconomics-0.2.0/pyeconomics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-30 01:41:25.000000 pyeconomics-0.2.0/pyeconomics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 01:41:25.000000 pyeconomics-0.2.0/pyeconomics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-30 01:41:25.000000 pyeconomics-0.2.0/pyeconomics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 01:41:25.000000 pyeconomics-0.2.0/pyeconomics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 01:41:25.947462 pyeconomics-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:41:25.947462 pyeconomics-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/tests/test_balanced_approach_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14924 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/tests/test_bar_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/tests/test_cache_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/tests/test_fdr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11865 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/tests/test_first_difference_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9744 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/tests/test_fred_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/tests/test_fred_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10175 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/tests/test_monetary_policy_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/tests/test_taylor_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11867 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/tests/test_tr_utils.py
```

### Comparing `pyeconomics-0.1.0/LICENSE` & `pyeconomics-0.2.0/LICENSE`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 Nathan Ramos, CFA®
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2024 Nathan Ramos, CFA®
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `pyeconomics-0.1.0/pyeconomics/fred_data.py` & `pyeconomics-0.2.0/pyeconomics/api/fred_data.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,32 @@
-import pandas as pd
-
-from .api import fred_client
-
-
-def fetch_historical_fed_funds_rate() -> pd.DataFrame:
-    """
-    Fetches and combines Federal Funds Target Rate historical data.
-
-    Returns:
-        pandas.DataFrame: DataFrame containing the Federal Funds Target Rate
-            historical data.
-
-    Notes:
-        - Prior to 2008-12-15, the Federal Funds Target Rate was a single value.
-        - Post 2008-12-15, the Federal Funds Target Rate is a range.
-        - This function uses the single value up to 2008-12-15, and the upper
-          limit of the range post 2008-12-15.
-    """
-    dfedtar = fred_client.fetch_data('DFEDTAR')
-    dfedtaru = fred_client.fetch_data('DFEDTARU')
-
-    # Use only the upper limit post 2008-12-15
-    df = pd.concat([
-        dfedtar[dfedtar.index <= '2008-12-15'],
-        dfedtaru[dfedtaru.index > '2008-12-15']
-    ])
-    return df
+# pyeconomics/api/fred_data.py
+
+import pandas as pd
+
+from pyeconomics.api.fred_api import fred_client
+
+
+def fetch_historical_fed_funds_rate() -> pd.DataFrame:
+    """
+    Fetches and combines Federal Funds Target Rate historical data.
+
+    Returns:
+        pandas.DataFrame: DataFrame containing the Federal Funds Target Rate
+            historical data.
+
+    Notes:
+        - Prior to 2008-12-15, the Federal Funds Target Rate was a single value.
+        - Post 2008-12-15, the Federal Funds Target Rate is a range.
+        - This function uses the single value up to 2008-12-15, and the upper
+          limit of the range post 2008-12-15.
+    """
+    dfedtar = fred_client.fetch_data('DFEDTAR')
+    dfedtaru = fred_client.fetch_data('DFEDTARU')
+
+    # Use only the upper limit post 2008-12-15
+    df = pd.concat([
+        dfedtar[dfedtar.index <= '2008-12-15'],
+        dfedtaru[dfedtaru.index > '2008-12-15']
+    ])
+    df.index.name = 'FedRate'
+    df.name = 'FedRate'
+    return df
```

### Comparing `pyeconomics-0.1.0/pyeconomics/taylor_rule.py` & `pyeconomics-0.2.0/pyeconomics/models/monetary_policy/balanced_approach_rule.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,228 +1,259 @@
-import pandas as pd
-
-from .api import fred_client
-from .fred_data import fetch_historical_fed_funds_rate
-
-
-def taylor_rule(
-        inflation_series_id: str = 'PCETRIM12M159SFRBDAL',
-        unemployment_rate_series_id: str = 'UNRATE',
-        natural_unemployment_series_id: str = 'NROU',
-        real_interest_rate_series_id: str = 'DFII10',
-        fed_rate_series: pd.Series = None,
-        current_inflation: float = None,
-        current_unemployment_rate: float = None,
-        natural_unemployment_rate: float = None,
-        long_term_real_interest_rate: float = None,
-        fed_rate: float = None,
-        inflation_target: float = 2.0,
-        alpha: float = 0.5,
-        beta: float = 0.5,
-        okun_factor: float = 2.0,
-        rho: float = 0.0,
-        elb: float = 0.125,
-        apply_elb: bool = False,
-        verbose: bool = False
-) -> float:
-    """
-    Computes the Taylor Rule interest rate based on economic indicators.
-
-    Args:
-        inflation_series_id (str): Series ID for inflation data.
-        unemployment_rate_series_id (str): Series ID for unemployment rate.
-        natural_unemployment_series_id (str): Series ID for natural
-            unemployment rate.
-        real_interest_rate_series_id (str): Series ID for long-term real
-            interest rate.
-        fed_rate_series (pd.Series): Series of Federal Funds Target Rate.
-        current_inflation (float): Current inflation rate.
-        current_unemployment_rate (float): Current unemployment rate.
-        natural_unemployment_rate (float): Natural unemployment rate.
-        long_term_real_interest_rate (float): Long-term real interest rate.
-        fed_rate (float): Current Federal Funds Target Rate.
-        inflation_target (float): Target inflation rate.
-        alpha (float): Weight for inflation gap.
-        beta (float): Weight for unemployment gap.
-        okun_factor (float): Multiplier for the unemployment gap.
-        rho (float): Policy inertia coefficient. Defaults to 0.0 which means
-            no inertia and no adjustment is made to Taylor Rule estimate. A
-            value of 1.0 would mean full inertia and immediate central bank
-            adjustment to the Taylor Rule estimate.
-        elb (float): Effective lower bound for interest rates.
-        apply_elb (bool): Whether to apply the effective lower bound
-            constraint to the Taylor Rule estimate.
-        verbose (bool): Whether to print verbose output.
-
-    Returns:
-        float: Taylor Rule interest rate estimate.
-    """
-    # Fetch data if not provided
-    current_inflation = fred_client.get_data_or_fetch(
-        current_inflation, inflation_series_id)
-    current_unemployment_rate = fred_client.get_data_or_fetch(
-        current_unemployment_rate, unemployment_rate_series_id)
-    natural_unemployment_rate = fred_client.get_data_or_fetch(
-        natural_unemployment_rate, natural_unemployment_series_id)
-    long_term_real_interest_rate = fred_client.get_data_or_fetch(
-        long_term_real_interest_rate, real_interest_rate_series_id)
-
-    if fed_rate is None:
-        fed_rate = (fed_rate_series.iloc[-1] if fed_rate_series is not None
-                    else fred_client.get_latest_value('DFEDTARU'))
-
-    if None in (current_inflation, current_unemployment_rate,
-                natural_unemployment_rate, long_term_real_interest_rate,
-                fed_rate):
-        raise ValueError("Required economic data is missing.")
-
-    # Calculate gaps and Taylor Rule estimate
-    inflation_gap = current_inflation - inflation_target
-    unemployment_gap = natural_unemployment_rate - current_unemployment_rate
-
-    taylor_est = (long_term_real_interest_rate +
-                  current_inflation +
-                  alpha * inflation_gap +
-                  beta * okun_factor * unemployment_gap)
-
-    if apply_elb:
-        taylor_est = max(taylor_est, elb)
-
-    adjusted_taylor_rule_interest_rate = (
-        rho * fed_rate + (1 - rho) * taylor_est
-    )
-
-    # Verbose output
-    if verbose:
-        print(f"\n==== Economic Indicators ===================================="
-              f"==")
-        print(f"Current Inflation:                        "
-              f"  {current_inflation:.2f}%")
-        print(f"Current Unemployment Rate:                "
-              f"  {current_unemployment_rate:.2f}%")
-        print(f"Natural Unemployment Rate:                "
-              f"  {natural_unemployment_rate:.2f}%")
-        print(f"Long-Term Real Interest Rate:             "
-              f"  {long_term_real_interest_rate:.2f}%")
-        print(f"Current Fed Rate:                         "
-              f"  {fed_rate:.2f}%")
-        print(f"\n==== Gaps ==================================================="
-              f"==")
-        print(f"Inflation Gap:                            "
-              f"  {inflation_gap:.2f}%")
-        print(f"Unemployment Gap:                         "
-              f"  {unemployment_gap:.2f}%")
-        print(f"\n==== Taylor Rule ============================================"
-              f"==")
-        print(f"  Long-Term Real Interest Rate:           "
-              f"  {long_term_real_interest_rate:.2f}%")
-        print(f"  Current Inflation:                      "
-              f"+ {current_inflation:.2f}%")
-        print(f"  Alpha * Inflation Gap:                  "
-              f"+ {alpha:.2f} * {inflation_gap:.2f}%")
-        print(f"  Beta * Okun Factor * Unemployment Gap:  "
-              f"+ {beta:.2f} * {okun_factor:.2f} * {unemployment_gap:.2f}%")
-        print("---------------------------------------------------------------")
-        print(f"  Taylor Rule:                            "
-              f"  {taylor_est:.2f}%")
-        print(f"\n==== Adjusted Taylor Rule ==================================="
-              f"==")
-        print("  Adjustment Computation:")
-        print(f"  Policy Inertia Coefficient (rho):       "
-              f"  {rho:.2f}")
-        print(f"  Current Fed Rate:                       "
-              f"* {fed_rate:.2f}%")
-        print(f"  Adjustment Coefficient (1 - rho):       "
-              f"+ (1 - {rho:.2f})")
-        print(f"  Taylor Rule Estimate:                   "
-              f"* {taylor_est:.2f}%")
-        print("---------------------------------------------------------------")
-        print(f"  Adjusted Taylor Rule Estimate:          "
-              f"  {adjusted_taylor_rule_interest_rate:.2f}%")
-
-    return round(adjusted_taylor_rule_interest_rate, 2)
-
-
-def historical_taylor_rule(
-        inflation_series_id: str = 'PCETRIM12M159SFRBDAL',
-        unemployment_rate_series_id: str = 'UNRATE',
-        natural_unemployment_series_id: str = 'NROU',
-        real_interest_rate_series_id: str = 'DFII10',
-        inflation_target: float = 2.0,
-        alpha: float = 0.5,
-        beta: float = 0.5,
-        okun_factor: float = 2.0,
-        rho: float = 0.0,
-        elb: float = 0.125,
-        apply_elb: bool = False
-) -> pd.DataFrame:
-    """
-    Computes historical Taylor Rule interest rates using
-    economic indicators up to the last date with available
-    real interest rate data.
-
-    Args:
-        inflation_series_id (str): Series ID for inflation data.
-        unemployment_rate_series_id (str): Series ID for unemployment rate.
-        natural_unemployment_series_id (str): Series ID for natural
-            unemployment rate.
-        real_interest_rate_series_id (str): Series ID for long-term real
-            interest rate.
-        inflation_target (float): Target inflation rate.
-        alpha (float): Weight for inflation gap.
-        beta (float): Weight for unemployment gap.
-        okun_factor (float): Multiplier for the unemployment gap.
-        rho (float): Policy inertia coefficient. Defaults to 0.0 which means
-            no inertia and no adjustment is made to Taylor Rule estimate. A
-            value of 1.0 would mean full inertia and immediate central bank
-            adjustment to the Taylor Rule estimate.
-        elb (float): Effective lower bound for interest rates.
-        apply_elb (bool): Whether to apply the effective lower bound
-            constraint to the Taylor Rule estimate.
-
-    Returns:
-        pd.DataFrame: DataFrame with computed Taylor Rule rates.
-    """
-    # Fetch historical data for all series
-    inflation = fred_client.fetch_data(inflation_series_id)
-    unemployment_rate = fred_client.fetch_data(unemployment_rate_series_id)
-    natural_unemployment = fred_client.fetch_data(
-        natural_unemployment_series_id)
-    real_interest_rate = fred_client.fetch_data(real_interest_rate_series_id)
-    fed_rate = fetch_historical_fed_funds_rate()
-
-    # Combine into a DataFrame and ensure data alignment
-    data = pd.DataFrame({
-        'Inflation': inflation,
-        'UnemploymentRate': unemployment_rate,
-        'NaturalUnemploymentRate': natural_unemployment,
-        'RealInterestRate': real_interest_rate,
-        'FedRate': fed_rate
-    })
-
-    # Determine the cutoff date based on RealInterestRate data
-    last_real_interest_date = data['RealInterestRate'].last_valid_index()
-    data = data.loc[:last_real_interest_date]
-
-    # Handle missing data
-    data.ffill(inplace=True)
-    data.dropna(inplace=True)
-
-    # Calculate gaps and Taylor Rule estimation
-    data['InflationGap'] = data['Inflation'] - inflation_target
-    data['UnemploymentGap'] = (data['NaturalUnemploymentRate'] -
-                               data['UnemploymentRate'])
-    data['TaylorEst'] = (data['RealInterestRate'] +
-                         data['Inflation'] +
-                         alpha * data['InflationGap'] +
-                         beta * okun_factor * data['UnemploymentGap'])
-
-    # Apply effective lower bound constraint
-    if apply_elb:
-        data['AdjustedTaylorRule'] = data['TaylorEst'].apply(
-            lambda x: max(x, elb))
-
-    # Apply policy inertia
-    data['AdjustedTaylorRule'] = (rho * data['FedRate'] +
-                                  (1 - rho) * data['AdjustedTaylorRule'])
-
-    return round(data, 2)
+# pyeconomics/models/monetary_policy/balanced_approach_rule.py
+
+import matplotlib.pyplot as plt
+import pandas as pd
+from typing import Optional
+
+from pyeconomics.api import fetch_historical_fed_funds_rate, fred_client
+from pyeconomics.data.economic_indicators import EconomicIndicators
+from pyeconomics.data.model_parameters import BalancedApproachRuleParameters
+from pyeconomics.utils import verbose_balanced_approach_rule
+
+
+def balanced_approach_rule(
+        indicators: EconomicIndicators = EconomicIndicators(),
+        params: BalancedApproachRuleParameters =
+        BalancedApproachRuleParameters(),
+        verbose: Optional[bool] = None
+) -> float:
+    """
+    Computes the Balanced Approach Rule interest rate based on economic
+    indicators.
+
+    Args:
+        indicators (EconomicIndicators): Economic indicators data class.
+        params (BalancedApproachRuleParameters): Balanced Approach Rule
+            parameters data class.
+        verbose (bool, optional): Whether to print verbose output. If not
+            provided, defaults to the value in params. Defaults to None.
+
+    Returns:
+        float: Balanced Approach Rule interest rate estimate.
+    """
+    # Override params.verbose if verbose is explicitly provided
+    verbose = verbose if verbose is not None else params.verbose
+
+    # Fetch data if not provided
+    indicators.current_inflation_rate = fred_client.get_data_or_fetch(
+        indicators.current_inflation_rate,
+        indicators.inflation_series_id)
+    indicators.current_unemployment_rate = fred_client.get_data_or_fetch(
+        indicators.current_unemployment_rate,
+        indicators.unemployment_rate_series_id)
+    indicators.natural_unemployment_rate = fred_client.get_data_or_fetch(
+        indicators.natural_unemployment_rate,
+        indicators.natural_unemployment_series_id)
+    indicators.long_term_real_interest_rate = fred_client.get_data_or_fetch(
+        indicators.long_term_real_interest_rate,
+        indicators.real_interest_rate_series_id)
+
+    if indicators.current_fed_rate is None:
+        indicators.current_fed_rate = fred_client.get_latest_value('DFEDTARU')
+
+    if None in (indicators.current_inflation_rate,
+                indicators.current_unemployment_rate,
+                indicators.natural_unemployment_rate,
+                indicators.long_term_real_interest_rate,
+                indicators.current_fed_rate):
+        raise ValueError("Required economic data is missing.")
+
+    # Calculate gaps and Balanced Approach Rule estimate
+    inflation_gap = indicators.current_inflation_rate - params.inflation_target
+    unemployment_gap = (indicators.natural_unemployment_rate -
+                        indicators.current_unemployment_rate)
+
+    # Apply shortfalls rule
+    if params.use_shortfalls_rule:
+        unemployment_gap = min(0.0, unemployment_gap)
+
+    unadjusted_rate = (indicators.long_term_real_interest_rate +
+                       indicators.current_inflation_rate +
+                       params.alpha * inflation_gap +
+                       params.beta * unemployment_gap)
+
+    # Apply effective lower bound constraint
+    if params.apply_elb:
+        adjusted_rate_after_elb = max(unadjusted_rate, params.elb)
+    else:
+        adjusted_rate_after_elb = unadjusted_rate
+
+    # Apply policy inertia
+    adjusted_rate_after_inertia = (
+        params.rho * indicators.current_fed_rate +
+        (1 - params.rho) * adjusted_rate_after_elb
+    )
+
+    # Verbose output
+    if verbose:
+        data = {
+            'current_inflation_rate': indicators.current_inflation_rate,
+            'inflation_target': params.inflation_target,
+            'current_unemployment_rate': indicators.current_unemployment_rate,
+            'natural_unemployment_rate': indicators.natural_unemployment_rate,
+            'long_term_real_interest_rate':
+                indicators.long_term_real_interest_rate,
+            'current_fed_rate': indicators.current_fed_rate,
+            'inflation_gap': inflation_gap,
+            'unemployment_gap': unemployment_gap,
+            'unadjusted_rate': unadjusted_rate,
+            'adjusted_rate_after_elb': adjusted_rate_after_elb,
+            'adjusted_rate_after_inertia': adjusted_rate_after_inertia,
+            'rho': params.rho,
+            'alpha': params.alpha,
+            'beta': params.beta,
+            'elb': params.elb,
+            'apply_elb': params.apply_elb,
+            'use_shortfalls_rule': params.use_shortfalls_rule
+        }
+        verbose_balanced_approach_rule(data)
+
+    return round(adjusted_rate_after_inertia, 2)
+
+
+def historical_balanced_approach_rule(
+        indicators: EconomicIndicators,
+        params: BalancedApproachRuleParameters
+) -> pd.DataFrame:
+    """
+    Computes historical Balanced Approach Rule interest rates using economic
+    indicators up to the last date with available real interest rate data.
+
+    Args:
+        indicators (EconomicIndicators): Economic indicators data class.
+        params (BalancedApproachRuleParameters): Balanced Approach Rule
+            parameters data class.
+
+    Returns:
+        pd.DataFrame: DataFrame with computed Balanced Approach Rule rates.
+    """
+    # Fetch historical data for all series
+    inflation = fred_client.fetch_data(indicators.inflation_series_id)
+    unemployment_rate = fred_client.fetch_data(
+        indicators.unemployment_rate_series_id)
+    natural_unemployment = fred_client.fetch_data(
+        indicators.natural_unemployment_series_id)
+    real_interest_rate = fred_client.fetch_data(
+        indicators.real_interest_rate_series_id)
+    fed_rate = fetch_historical_fed_funds_rate()
+
+    # Combine into a DataFrame
+    data = pd.DataFrame({
+        'Inflation': inflation,
+        'UnemploymentRate': unemployment_rate,
+        'NaturalUnemploymentRate': natural_unemployment,
+        'RealInterestRate': real_interest_rate,
+        'FedRate': fed_rate
+    })
+
+    # Determine the cutoff date based on RealInterestRate data
+    last_real_interest_date = data['RealInterestRate'].last_valid_index()
+    data = data.loc[:last_real_interest_date]
+
+    # Handle missing data
+    data.ffill(inplace=True)
+    data.dropna(inplace=True)
+
+    # Calculate gaps and Balanced Approach Rule estimation
+    data['InflationGap'] = data['Inflation'] - params.inflation_target
+    data['UnemploymentGap'] = (data['NaturalUnemploymentRate'] -
+                               data['UnemploymentRate'])
+
+    # Apply shortfalls rule
+    if params.use_shortfalls_rule:
+        data['UnemploymentGap'] = data['UnemploymentGap'].apply(
+            lambda x: min(0, x))
+        rule_name = 'BalancedApproachShortfallsRule'
+    else:
+        rule_name = 'BalancedApproachRule'
+
+    data[rule_name] = (data['RealInterestRate'] +
+                       data['Inflation'] +
+                       params.alpha * data['InflationGap'] +
+                       params.beta * data['UnemploymentGap'])
+
+    adjusted_rule_name = 'Adjusted' + rule_name
+
+    # Apply effective lower bound
+    if params.apply_elb:
+        data[adjusted_rule_name] = data[rule_name].apply(
+            lambda x: max(x, params.elb))
+    else:
+        data[adjusted_rule_name] = data[rule_name]
+
+    # Apply policy inertia
+    data[adjusted_rule_name] = (
+            params.rho * data['FedRate'] +
+            (1 - params.rho) * data[adjusted_rule_name])
+
+    return data.round(2)
+
+
+def plot_historical_bar_basr_rule(
+    historical_rates: pd.DataFrame,
+    adjusted: bool = False
+) -> None:
+    """
+    Extract the time range from the data, plot either the Balanced Approach
+    Rule (BAR) and Balanced Approach Shortfalls Rule (BASR) estimates or their
+    adjusted versions along with the Federal Funds Rate, and display the date
+    range in the plot title.
+
+    Args:
+        historical_rates (pd.DataFrame): DataFrame containing the historical
+            rates including BAR, BASR estimates, and the Federal Funds Rate,
+            along with their adjusted versions if applicable.
+        adjusted (bool): A flag to determine whether to plot the adjusted or
+            unadjusted rates.
+
+    Returns:
+        None
+    """
+    if adjusted:
+        columns = [
+            'AdjustedBalancedApproachRule',
+            'AdjustedBalancedApproachShortfallsRule',
+            'FedRate'
+        ]
+        title_prefix = "Adjusted "
+    else:
+        columns = [
+            'BalancedApproachRule',
+            'BalancedApproachShortfallsRule',
+            'FedRate'
+        ]
+        title_prefix = ""
+
+    # Select relevant data
+    plot_data = historical_rates[columns].copy()
+
+    # Extracting the time range from the data
+    start_date = plot_data.dropna().index.min()
+    end_date = plot_data.dropna().index.max()
+    date_range = (f"{start_date.strftime('%B %d, %Y')} to "
+                  f"{end_date.strftime('%B %d, %Y')}")
+
+    # Plotting BAR and BASR Rule estimates and the Federal Funds Rate
+    plot_data.dropna().plot(
+        figsize=(10, 5),  # Specifies the figure size
+        grid=True  # Enables grid lines for better readability
+    )
+
+    plt.title(f'{title_prefix}BAR and BASR Rule Estimates and Federal Funds '
+              f'Rate\n{date_range}')
+    plt.xlabel('Year')
+    plt.ylabel('Interest Rate (%)')
+    plt.legend([
+        f'{title_prefix}BAR Rule',
+        f'{title_prefix}BASR Rule',
+        'Federal Funds Rate']
+    )
+
+    # Adding the citation as a footnote
+    plt.figtext(
+        x=0.25,
+        y=-0.01,
+        s="Data Source: Federal Reserve Economic Data (FRED)",
+        ha="center"
+    )
+
+    plt.show()  # Display the plot
```

