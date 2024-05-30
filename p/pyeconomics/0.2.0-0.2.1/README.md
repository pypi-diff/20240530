# Comparing `tmp/pyeconomics-0.2.0.tar.gz` & `tmp/pyeconomics-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyeconomics-0.2.0.tar", last modified: Thu May 30 01:41:25 2024, max compression
+gzip compressed data, was "pyeconomics-0.2.1.tar", last modified: Thu May 30 03:51:01 2024, max compression
```

## Comparing `pyeconomics-0.2.0.tar` & `pyeconomics-0.2.1.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:41:25.947462 pyeconomics-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:41:25.931462 pyeconomics-0.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:41:25.931462 pyeconomics-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    23724 2024-05-30 01:41:25.947462 pyeconomics-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22439 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:41:25.935462 pyeconomics-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:41:25.935462 pyeconomics-0.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    69539 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:41:25.935462 pyeconomics-0.2.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/_templates/.keep
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/api_key.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/contact.rst
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/create_roadmap_files.bat
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/docker.rst
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/features.rst
--rw-r--r--   0 runner    (1001) docker     (127)    19195 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/roadmap.rst
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/roadmap_discounted_cash_flow_models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/roadmap_exchange_rate_models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/roadmap_financial_models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/roadmap_fiscal_policy_models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/roadmap_macroeconomic_models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/roadmap_microeconomic_models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/roadmap_monetary_policy_models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/roadmap_other_economic_models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/roadmap_quantity_of_money_theory.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10580 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:41:25.927462 pyeconomics-0.2.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:41:25.939462 pyeconomics-0.2.0/examples/api_configuration/
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/examples/api_configuration/fred_api_configuration.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:41:25.939462 pyeconomics-0.2.0/examples/monetary_policy_rules/
--rw-r--r--   0 runner    (1001) docker     (127)   214512 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/examples/monetary_policy_rules/balanced_approach_rule.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   125883 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/examples/monetary_policy_rules/first_difference_rule.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   286474 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/examples/monetary_policy_rules/monetary_policy_rules.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   118525 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/examples/monetary_policy_rules/taylor_rule.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:41:25.939462 pyeconomics-0.2.0/markdown/
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/markdown/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/markdown/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/markdown/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/markdown/FRED_API_CONFIGURATION.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:41:25.939462 pyeconomics-0.2.0/media/
--rw-r--r--   0 runner    (1001) docker     (127)   181489 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/media/plot_adj_historical_rates.png
--rw-r--r--   0 runner    (1001) docker     (127)   181531 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/media/plot_historical_policy_rates.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:41:25.939462 pyeconomics-0.2.0/pyeconomics/
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyeconomics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyeconomics/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:41:25.943462 pyeconomics-0.2.0/pyeconomics/api/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyeconomics/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyeconomics/api/cache_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     7668 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyeconomics/api/fred_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyeconomics/api/fred_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:41:25.943462 pyeconomics-0.2.0/pyeconomics/data/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyeconomics/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyeconomics/data/economic_indicators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyeconomics/data/model_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:41:25.943462 pyeconomics-0.2.0/pyeconomics/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyeconomics/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:41:25.943462 pyeconomics-0.2.0/pyeconomics/models/monetary_policy/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyeconomics/models/monetary_policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9556 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyeconomics/models/monetary_policy/balanced_approach_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyeconomics/models/monetary_policy/first_difference_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    12879 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyeconomics/models/monetary_policy/monetary_policy_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     8327 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyeconomics/models/monetary_policy/taylor_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:41:25.943462 pyeconomics-0.2.0/pyeconomics/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyeconomics/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6728 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyeconomics/utils/bar_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyeconomics/utils/fdr_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyeconomics/utils/tr_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:41:25.939462 pyeconomics-0.2.0/pyeconomics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23724 2024-05-30 01:41:25.000000 pyeconomics-0.2.0/pyeconomics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-30 01:41:25.000000 pyeconomics-0.2.0/pyeconomics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 01:41:25.000000 pyeconomics-0.2.0/pyeconomics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-30 01:41:25.000000 pyeconomics-0.2.0/pyeconomics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 01:41:25.000000 pyeconomics-0.2.0/pyeconomics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 01:41:25.947462 pyeconomics-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:41:25.947462 pyeconomics-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/tests/test_balanced_approach_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    14924 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/tests/test_bar_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/tests/test_cache_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/tests/test_fdr_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11865 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/tests/test_first_difference_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9744 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/tests/test_fred_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/tests/test_fred_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10175 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/tests/test_monetary_policy_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/tests/test_taylor_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    11867 2024-05-30 01:40:47.000000 pyeconomics-0.2.0/tests/test_tr_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:51:01.609774 pyeconomics-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:51:01.593774 pyeconomics-0.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:51:01.593774 pyeconomics-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    23724 2024-05-30 03:51:01.609774 pyeconomics-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22439 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:51:01.597774 pyeconomics-0.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:51:01.597774 pyeconomics-0.2.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    69539 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:51:01.597774 pyeconomics-0.2.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/docs/_templates/.keep
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/docs/api_key.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/docs/contact.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/docs/create_roadmap_files.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/docs/docker.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/docs/features.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    19195 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/docs/roadmap.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/docs/roadmap_discounted_cash_flow_models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/docs/roadmap_exchange_rate_models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/docs/roadmap_financial_models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/docs/roadmap_fiscal_policy_models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/docs/roadmap_macroeconomic_models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/docs/roadmap_microeconomic_models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/docs/roadmap_monetary_policy_models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/docs/roadmap_other_economic_models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/docs/roadmap_quantity_of_money_theory.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10580 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:51:01.589774 pyeconomics-0.2.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:51:01.597774 pyeconomics-0.2.1/examples/api_configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/examples/api_configuration/fred_api_configuration.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:51:01.601774 pyeconomics-0.2.1/examples/monetary_policy_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)   214512 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/examples/monetary_policy_rules/balanced_approach_rule.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   125883 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/examples/monetary_policy_rules/first_difference_rule.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   286474 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/examples/monetary_policy_rules/monetary_policy_rules.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   118525 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/examples/monetary_policy_rules/taylor_rule.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:51:01.601774 pyeconomics-0.2.1/markdown/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/markdown/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/markdown/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/markdown/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/markdown/FRED_API_CONFIGURATION.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:51:01.601774 pyeconomics-0.2.1/media/
+-rw-r--r--   0 runner    (1001) docker     (127)   181489 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/media/plot_adj_historical_rates.png
+-rw-r--r--   0 runner    (1001) docker     (127)   181531 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/media/plot_historical_policy_rates.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:51:01.601774 pyeconomics-0.2.1/pyeconomics/
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/pyeconomics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/pyeconomics/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:51:01.605774 pyeconomics-0.2.1/pyeconomics/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/pyeconomics/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/pyeconomics/api/cache_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7668 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/pyeconomics/api/fred_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/pyeconomics/api/fred_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:51:01.605774 pyeconomics-0.2.1/pyeconomics/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/pyeconomics/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/pyeconomics/data/economic_indicators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/pyeconomics/data/model_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:51:01.605774 pyeconomics-0.2.1/pyeconomics/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/pyeconomics/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:51:01.605774 pyeconomics-0.2.1/pyeconomics/models/monetary_policy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/pyeconomics/models/monetary_policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9556 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/pyeconomics/models/monetary_policy/balanced_approach_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/pyeconomics/models/monetary_policy/first_difference_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12879 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/pyeconomics/models/monetary_policy/monetary_policy_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8327 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/pyeconomics/models/monetary_policy/taylor_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:51:01.605774 pyeconomics-0.2.1/pyeconomics/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/pyeconomics/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6728 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/pyeconomics/utils/bar_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/pyeconomics/utils/fdr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/pyeconomics/utils/tr_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:51:01.601774 pyeconomics-0.2.1/pyeconomics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23724 2024-05-30 03:51:01.000000 pyeconomics-0.2.1/pyeconomics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-30 03:51:01.000000 pyeconomics-0.2.1/pyeconomics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 03:51:01.000000 pyeconomics-0.2.1/pyeconomics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-30 03:51:01.000000 pyeconomics-0.2.1/pyeconomics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 03:51:01.000000 pyeconomics-0.2.1/pyeconomics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 03:51:01.609774 pyeconomics-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:51:01.609774 pyeconomics-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/tests/test_balanced_approach_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14924 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/tests/test_bar_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/tests/test_cache_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/tests/test_fdr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11865 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/tests/test_first_difference_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9744 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/tests/test_fred_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/tests/test_fred_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10175 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/tests/test_monetary_policy_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/tests/test_taylor_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11867 2024-05-30 03:50:25.000000 pyeconomics-0.2.1/tests/test_tr_utils.py
```

### Comparing `pyeconomics-0.2.0/.dockerignore` & `pyeconomics-0.2.1/.dockerignore`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/.editorconfig` & `pyeconomics-0.2.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/.github/workflows/docs.yml` & `pyeconomics-0.2.1/.github/workflows/docs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 jobs:
   build-docs:
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v4  # Ensure to use the latest version for Node.js 20 support
     - name: Set up Python
-      uses: actions/setup-python@v4  # Ensure to use the latest version for Node.js 20 support
+      uses: actions/setup-python@v5  # Ensure to use the latest version for Node.js 20 support
       with:
         python-version: '3.12'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -r requirements.txt
         pip install sphinx
```

### Comparing `pyeconomics-0.2.0/.github/workflows/release.yml` & `pyeconomics-0.2.1/.github/workflows/release.yml`

 * *Files 18% similar despite different names*

```diff
@@ -11,18 +11,18 @@
     strategy:
       fail-fast: false
       matrix:
         python-version: ['3.11', '3.12']
 
     steps:
     - name: Check out code
-      uses: actions/checkout@v4  # Ensure to use the latest version for Node.js 20 support
+      uses: actions/checkout@v4
 
     - name: Set up Python
-      uses: actions/setup-python@v4  # Ensure to use the latest version for Node.js 20 support
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Extract version from tag
       run: echo "VERSION=${GITHUB_REF#refs/tags/v}" >> $GITHUB_ENV
 
     - name: Update version number
@@ -35,11 +35,12 @@
     - name: Install dependencies
       run: pip install -r requirements.txt
 
     - name: Build package
       run: python setup.py sdist bdist_wheel
 
     - name: Publish to PyPI
-      uses: pypa/gh-action-pypi-publish@v1.4.2  # Already uses Node.js 20
+      uses: pypa/gh-action-pypi-publish@v1.4.2
       with:
         user: __token__
         password: ${{ secrets.PYPI_API_TOKEN }}
+        skip_existing: true  # Add this line to skip existing files
```

### Comparing `pyeconomics-0.2.0/.github/workflows/tests.yml` & `pyeconomics-0.2.1/.github/workflows/tests.yml`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         python-version: ['3.11', '3.12']
 
     steps:
     - uses: actions/checkout@v4  # Ensure to use the latest version for Node.js 20 support
 
     # Set up Python
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4  # Ensure to use the latest version for Node.js 20 support
+      uses: actions/setup-python@v5  # Ensure to use the latest version for Node.js 20 support
       with:
         python-version: ${{ matrix.python-version }}
 
     # Install dependencies
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
```

### Comparing `pyeconomics-0.2.0/.gitignore` & `pyeconomics-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/Dockerfile` & `pyeconomics-0.2.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/LICENSE` & `pyeconomics-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/MANIFEST.in` & `pyeconomics-0.2.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/PKG-INFO` & `pyeconomics-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyeconomics
-Version: 0.2.0
+Version: 0.2.1
 Summary: A library for economic and financial analysis
 Home-page: https://github.com/nathanramoscfa/pyeconomics
 Author: Nathan Ramos, CFA
 Author-email: nathan.ramos.github@gmail.com
 Project-URL: Bug Reports, https://github.com/nathanramoscfa/pyeconomics/issues
 Project-URL: Source, https://github.com/nathanramoscfa/pyeconomics
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyeconomics-0.2.0/README.md` & `pyeconomics-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/docs/Makefile` & `pyeconomics-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/docs/_static/logo.png` & `pyeconomics-0.2.1/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/docs/conf.py` & `pyeconomics-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/docs/contact.rst` & `pyeconomics-0.2.1/docs/contact.rst`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/docs/create_roadmap_files.bat` & `pyeconomics-0.2.1/docs/create_roadmap_files.bat`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/docs/docker.rst` & `pyeconomics-0.2.1/docs/docker.rst`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,16 @@
    content:
 
    .. code-block:: text
 
       FRED_API_KEY=your_fred_api_key_here
 
 2. **Build the Docker Image**:
-   Navigate to your project directory and run the following command to build the
-   Docker image:
+   Navigate to your pyeconomics root directory and run the following command to
+   build the Docker image:
 
    .. code-block:: shell
 
       docker build -t pyeconomics .
 
 3. **Run the Docker Container**:
    Run a container from your custom Docker image:
```

### Comparing `pyeconomics-0.2.0/docs/features.rst` & `pyeconomics-0.2.1/docs/features.rst`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/docs/index.rst` & `pyeconomics-0.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/docs/introduction.rst` & `pyeconomics-0.2.1/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/docs/make.bat` & `pyeconomics-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/docs/usage.rst` & `pyeconomics-0.2.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/examples/api_configuration/fred_api_configuration.ipynb` & `pyeconomics-0.2.1/examples/api_configuration/fred_api_configuration.ipynb`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/examples/monetary_policy_rules/balanced_approach_rule.ipynb` & `pyeconomics-0.2.1/examples/monetary_policy_rules/balanced_approach_rule.ipynb`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/examples/monetary_policy_rules/first_difference_rule.ipynb` & `pyeconomics-0.2.1/examples/monetary_policy_rules/first_difference_rule.ipynb`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/examples/monetary_policy_rules/monetary_policy_rules.ipynb` & `pyeconomics-0.2.1/examples/monetary_policy_rules/monetary_policy_rules.ipynb`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/examples/monetary_policy_rules/taylor_rule.ipynb` & `pyeconomics-0.2.1/examples/monetary_policy_rules/taylor_rule.ipynb`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/markdown/CHANGELOG.md` & `pyeconomics-0.2.1/markdown/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/markdown/CODE_OF_CONDUCT.md` & `pyeconomics-0.2.1/markdown/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/markdown/CONTRIBUTING.md` & `pyeconomics-0.2.1/markdown/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/markdown/FRED_API_CONFIGURATION.md` & `pyeconomics-0.2.1/markdown/FRED_API_CONFIGURATION.md`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/media/plot_adj_historical_rates.png` & `pyeconomics-0.2.1/media/plot_adj_historical_rates.png`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/media/plot_historical_policy_rates.png` & `pyeconomics-0.2.1/media/plot_historical_policy_rates.png`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/pyeconomics/__init__.py` & `pyeconomics-0.2.1/pyeconomics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/pyeconomics/api/cache_manager.py` & `pyeconomics-0.2.1/pyeconomics/api/cache_manager.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/pyeconomics/api/fred_api.py` & `pyeconomics-0.2.1/pyeconomics/api/fred_api.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/pyeconomics/api/fred_data.py` & `pyeconomics-0.2.1/pyeconomics/api/fred_data.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/pyeconomics/data/economic_indicators.py` & `pyeconomics-0.2.1/pyeconomics/data/economic_indicators.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/pyeconomics/data/model_parameters.py` & `pyeconomics-0.2.1/pyeconomics/data/model_parameters.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/pyeconomics/models/monetary_policy/__init__.py` & `pyeconomics-0.2.1/pyeconomics/models/monetary_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/pyeconomics/models/monetary_policy/balanced_approach_rule.py` & `pyeconomics-0.2.1/pyeconomics/models/monetary_policy/balanced_approach_rule.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/pyeconomics/models/monetary_policy/first_difference_rule.py` & `pyeconomics-0.2.1/pyeconomics/models/monetary_policy/first_difference_rule.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/pyeconomics/models/monetary_policy/monetary_policy_rules.py` & `pyeconomics-0.2.1/pyeconomics/models/monetary_policy/monetary_policy_rules.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/pyeconomics/models/monetary_policy/taylor_rule.py` & `pyeconomics-0.2.1/pyeconomics/models/monetary_policy/taylor_rule.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/pyeconomics/utils/bar_utils.py` & `pyeconomics-0.2.1/pyeconomics/utils/bar_utils.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/pyeconomics/utils/fdr_utils.py` & `pyeconomics-0.2.1/pyeconomics/utils/fdr_utils.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/pyeconomics/utils/tr_utils.py` & `pyeconomics-0.2.1/pyeconomics/utils/tr_utils.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/pyeconomics.egg-info/PKG-INFO` & `pyeconomics-0.2.1/pyeconomics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyeconomics
-Version: 0.2.0
+Version: 0.2.1
 Summary: A library for economic and financial analysis
 Home-page: https://github.com/nathanramoscfa/pyeconomics
 Author: Nathan Ramos, CFA
 Author-email: nathan.ramos.github@gmail.com
 Project-URL: Bug Reports, https://github.com/nathanramoscfa/pyeconomics/issues
 Project-URL: Source, https://github.com/nathanramoscfa/pyeconomics
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyeconomics-0.2.0/pyeconomics.egg-info/SOURCES.txt` & `pyeconomics-0.2.1/pyeconomics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/setup.py` & `pyeconomics-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/tests/conftest.py` & `pyeconomics-0.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/tests/test_balanced_approach_rule.py` & `pyeconomics-0.2.1/tests/test_balanced_approach_rule.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/tests/test_bar_utils.py` & `pyeconomics-0.2.1/tests/test_bar_utils.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/tests/test_cache_manager.py` & `pyeconomics-0.2.1/tests/test_cache_manager.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/tests/test_fdr_utils.py` & `pyeconomics-0.2.1/tests/test_fdr_utils.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/tests/test_first_difference_rule.py` & `pyeconomics-0.2.1/tests/test_first_difference_rule.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/tests/test_fred_api.py` & `pyeconomics-0.2.1/tests/test_fred_api.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/tests/test_fred_data.py` & `pyeconomics-0.2.1/tests/test_fred_data.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/tests/test_monetary_policy_rules.py` & `pyeconomics-0.2.1/tests/test_monetary_policy_rules.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/tests/test_taylor_rule.py` & `pyeconomics-0.2.1/tests/test_taylor_rule.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.0/tests/test_tr_utils.py` & `pyeconomics-0.2.1/tests/test_tr_utils.py`

 * *Files identical despite different names*

