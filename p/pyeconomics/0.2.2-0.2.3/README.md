# Comparing `tmp/pyeconomics-0.2.2.tar.gz` & `tmp/pyeconomics-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyeconomics-0.2.2.tar", last modified: Thu May 30 05:00:53 2024, max compression
+gzip compressed data, was "pyeconomics-0.2.3.tar", last modified: Thu May 30 16:17:28 2024, max compression
```

## Comparing `pyeconomics-0.2.2.tar` & `pyeconomics-0.2.3.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:00:53.573213 pyeconomics-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:00:53.557213 pyeconomics-0.2.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:00:53.557213 pyeconomics-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    23847 2024-05-30 05:00:53.573213 pyeconomics-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22562 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:00:53.561213 pyeconomics-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:00:53.561213 pyeconomics-0.2.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    69539 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/docs/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:00:53.561213 pyeconomics-0.2.2/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/docs/_templates/.keep
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/docs/api_key.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/docs/contact.rst
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/docs/create_roadmap_files.bat
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/docs/docker.rst
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/docs/features.rst
--rw-r--r--   0 runner    (1001) docker     (127)    19195 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/docs/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/docs/roadmap.rst
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/docs/roadmap_discounted_cash_flow_models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/docs/roadmap_exchange_rate_models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/docs/roadmap_financial_models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/docs/roadmap_fiscal_policy_models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/docs/roadmap_macroeconomic_models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/docs/roadmap_microeconomic_models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/docs/roadmap_monetary_policy_models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/docs/roadmap_other_economic_models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/docs/roadmap_quantity_of_money_theory.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10580 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:00:53.553213 pyeconomics-0.2.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:00:53.561213 pyeconomics-0.2.2/examples/api_configuration/
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/examples/api_configuration/fred_api_configuration.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:00:53.565213 pyeconomics-0.2.2/examples/monetary_policy_rules/
--rw-r--r--   0 runner    (1001) docker     (127)   214512 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/examples/monetary_policy_rules/balanced_approach_rule.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   125883 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/examples/monetary_policy_rules/first_difference_rule.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   286474 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/examples/monetary_policy_rules/monetary_policy_rules.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   118525 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/examples/monetary_policy_rules/taylor_rule.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:00:53.565213 pyeconomics-0.2.2/markdown/
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/markdown/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/markdown/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/markdown/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/markdown/FRED_API_CONFIGURATION.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:00:53.565213 pyeconomics-0.2.2/media/
--rw-r--r--   0 runner    (1001) docker     (127)   181489 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/media/plot_adj_historical_rates.png
--rw-r--r--   0 runner    (1001) docker     (127)   181531 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/media/plot_historical_policy_rates.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:00:53.565213 pyeconomics-0.2.2/pyeconomics/
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/pyeconomics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 05:00:14.000000 pyeconomics-0.2.2/pyeconomics/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:00:53.569213 pyeconomics-0.2.2/pyeconomics/api/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/pyeconomics/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/pyeconomics/api/cache_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     7668 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/pyeconomics/api/fred_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/pyeconomics/api/fred_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:00:53.569213 pyeconomics-0.2.2/pyeconomics/data/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/pyeconomics/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/pyeconomics/data/economic_indicators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/pyeconomics/data/model_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:00:53.569213 pyeconomics-0.2.2/pyeconomics/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/pyeconomics/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:00:53.569213 pyeconomics-0.2.2/pyeconomics/models/monetary_policy/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/pyeconomics/models/monetary_policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9556 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/pyeconomics/models/monetary_policy/balanced_approach_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/pyeconomics/models/monetary_policy/first_difference_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    12879 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/pyeconomics/models/monetary_policy/monetary_policy_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     8327 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/pyeconomics/models/monetary_policy/taylor_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:00:53.569213 pyeconomics-0.2.2/pyeconomics/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/pyeconomics/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6728 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/pyeconomics/utils/bar_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/pyeconomics/utils/fdr_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/pyeconomics/utils/tr_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:00:53.565213 pyeconomics-0.2.2/pyeconomics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23847 2024-05-30 05:00:53.000000 pyeconomics-0.2.2/pyeconomics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-30 05:00:53.000000 pyeconomics-0.2.2/pyeconomics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 05:00:53.000000 pyeconomics-0.2.2/pyeconomics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-30 05:00:53.000000 pyeconomics-0.2.2/pyeconomics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 05:00:53.000000 pyeconomics-0.2.2/pyeconomics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 05:00:53.573213 pyeconomics-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:00:53.573213 pyeconomics-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/tests/test_balanced_approach_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    14924 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/tests/test_bar_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/tests/test_cache_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/tests/test_fdr_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11865 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/tests/test_first_difference_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9744 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/tests/test_fred_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/tests/test_fred_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10175 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/tests/test_monetary_policy_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/tests/test_taylor_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    11867 2024-05-30 05:00:13.000000 pyeconomics-0.2.2/tests/test_tr_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:17:28.721917 pyeconomics-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:17:28.705917 pyeconomics-0.2.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:17:28.705917 pyeconomics-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    24941 2024-05-30 16:17:28.721917 pyeconomics-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23679 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:17:28.709917 pyeconomics-0.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:17:28.709917 pyeconomics-0.2.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    69539 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:17:28.709917 pyeconomics-0.2.3/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/_templates/.keep
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/api_key.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/contact.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/create_roadmap_files.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/docker.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/features.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    19195 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/roadmap.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/roadmap_discounted_cash_flow_models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/roadmap_exchange_rate_models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/roadmap_financial_models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/roadmap_fiscal_policy_models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/roadmap_macroeconomic_models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/roadmap_microeconomic_models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/roadmap_monetary_policy_models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/roadmap_other_economic_models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/roadmap_quantity_of_money_theory.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10580 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:17:28.701917 pyeconomics-0.2.3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:17:28.709917 pyeconomics-0.2.3/examples/api_configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/examples/api_configuration/fred_api_configuration.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:17:28.713917 pyeconomics-0.2.3/examples/monetary_policy_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)   214512 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/examples/monetary_policy_rules/balanced_approach_rule.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   125883 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/examples/monetary_policy_rules/first_difference_rule.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   286474 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/examples/monetary_policy_rules/monetary_policy_rules.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   118525 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/examples/monetary_policy_rules/taylor_rule.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:17:28.713917 pyeconomics-0.2.3/markdown/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/markdown/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/markdown/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/markdown/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/markdown/FRED_API_CONFIGURATION.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:17:28.713917 pyeconomics-0.2.3/media/
+-rw-r--r--   0 runner    (1001) docker     (127)   181489 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/media/plot_adj_historical_rates.png
+-rw-r--r--   0 runner    (1001) docker     (127)   181531 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/media/plot_historical_policy_rates.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:17:28.713917 pyeconomics-0.2.3/pyeconomics/
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyeconomics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyeconomics/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:17:28.713917 pyeconomics-0.2.3/pyeconomics/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyeconomics/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyeconomics/api/cache_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7668 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyeconomics/api/fred_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyeconomics/api/fred_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:17:28.717917 pyeconomics-0.2.3/pyeconomics/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyeconomics/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyeconomics/data/economic_indicators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyeconomics/data/model_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:17:28.717917 pyeconomics-0.2.3/pyeconomics/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyeconomics/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:17:28.717917 pyeconomics-0.2.3/pyeconomics/models/monetary_policy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyeconomics/models/monetary_policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9556 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyeconomics/models/monetary_policy/balanced_approach_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyeconomics/models/monetary_policy/first_difference_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12879 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyeconomics/models/monetary_policy/monetary_policy_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8327 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyeconomics/models/monetary_policy/taylor_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:17:28.717917 pyeconomics-0.2.3/pyeconomics/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyeconomics/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6728 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyeconomics/utils/bar_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyeconomics/utils/fdr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyeconomics/utils/tr_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:17:28.713917 pyeconomics-0.2.3/pyeconomics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    24941 2024-05-30 16:17:28.000000 pyeconomics-0.2.3/pyeconomics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-30 16:17:28.000000 pyeconomics-0.2.3/pyeconomics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 16:17:28.000000 pyeconomics-0.2.3/pyeconomics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-30 16:17:28.000000 pyeconomics-0.2.3/pyeconomics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 16:17:28.000000 pyeconomics-0.2.3/pyeconomics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 16:17:28.721917 pyeconomics-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:17:28.721917 pyeconomics-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/tests/test_balanced_approach_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14924 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/tests/test_bar_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/tests/test_cache_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/tests/test_fdr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11865 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/tests/test_first_difference_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9744 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/tests/test_fred_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/tests/test_fred_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10175 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/tests/test_monetary_policy_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/tests/test_taylor_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11867 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/tests/test_tr_utils.py
```

### Comparing `pyeconomics-0.2.2/.dockerignore` & `pyeconomics-0.2.3/.dockerignore`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/.editorconfig` & `pyeconomics-0.2.3/.editorconfig`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/.github/workflows/docs.yml` & `pyeconomics-0.2.3/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/.github/workflows/release.yml` & `pyeconomics-0.2.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/.github/workflows/tests.yml` & `pyeconomics-0.2.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/.gitignore` & `pyeconomics-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/Dockerfile` & `pyeconomics-0.2.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/LICENSE` & `pyeconomics-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/MANIFEST.in` & `pyeconomics-0.2.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/PKG-INFO` & `pyeconomics-0.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pyeconomics
-Version: 0.2.2
+Version: 0.2.3
 Summary: A library for economic and financial analysis
 Home-page: https://github.com/nathanramoscfa/pyeconomics
 Author: Nathan Ramos, CFA
 Author-email: nathan.ramos.github@gmail.com
 Project-URL: Bug Reports, https://github.com/nathanramoscfa/pyeconomics/issues
 Project-URL: Source, https://github.com/nathanramoscfa/pyeconomics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Requires-Python: >=3.11, <3.13
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fredapi~=0.5.1
 Requires-Dist: jupyterlab~=4.1.8
 Requires-Dist: keyring~=25.2.0
@@ -52,22 +52,22 @@
 | **Maintainability** | [![Maintainability](https://api.codeclimate.com/v1/badges/8d0d8b5a5bed8fe94814/maintainability)](https://codeclimate.com/github/nathanramoscfa/pyeconomics/maintainability)                                                                                                                                                                                                                                  |
 | **Code Style**      | [![Code Style: Flake8](https://img.shields.io/badge/code%20style-flake8-brightgreen.svg)](https://github.com/PyCQA/flake8)                                                                                                                                                                                                                                                                                   |
 | **Dependencies**    | [![Dependency Status](https://img.shields.io/librariesio/github/nathanramoscfa/pyeconomics)](https://libraries.io/github/nathanramoscfa/pyeconomics)                                                                                                                                                                                                                                                         |
 | **Security**        | [![Security Status](https://snyk.io/test/github/nathanramoscfa/pyeconomics/badge.svg)](https://snyk.io/test/github/nathanramoscfa/pyeconomics)                                                                                                                                                                                                                                                               |
 
 ## Table of Contents
 
-- [Introduction](#introduction)
-- [Features](#features)
-- [Installation](#installation)
-- [Usage](#usage)
-- [Docker](#docker)
-- [Roadmap](#roadmap)
-- [Contributing](#contributing)
-- [Contact](#contact)
+- [Introduction](https://github.com/nathanramoscfa/pyeconomics?tab=readme-ov-file#introduction)
+- [Features](https://github.com/nathanramoscfa/pyeconomics?tab=readme-ov-file#features)
+- [Installation](https://github.com/nathanramoscfa/pyeconomics?tab=readme-ov-file#installation)
+- [Usage](https://github.com/nathanramoscfa/pyeconomics?tab=readme-ov-file#usage)
+- [Docker](https://github.com/nathanramoscfa/pyeconomics?tab=readme-ov-file#docker)
+- [Roadmap](https://github.com/nathanramoscfa/pyeconomics?tab=readme-ov-file#roadmap)
+- [Contributing](https://github.com/nathanramoscfa/pyeconomics?tab=readme-ov-file#contributing)
+- [Contact](https://github.com/nathanramoscfa/pyeconomics?tab=readme-ov-file#contact)
 
 ## Introduction
 
 PyEconomics is a versatile and comprehensive library that integrates various
 economic and financial models. It is designed to support the development and
 analysis of monetary policy rules, exchange rate models, macroeconomic and
 microeconomic models, discounted cash flow models, and much more.
@@ -126,16 +126,16 @@
 
 Some features of PyEconomics require access to the FRED API. To use these 
 features, you need to configure your FRED API access. 
 
 A detailed step-by-step guide on obtaining and securely storing your FRED API 
 key is available here:
 
-- [FRED API Key Configuration Guide (Markdown)](markdown/FRED_API_CONFIGURATION.md)
-- [FRED API Key Configuration Guide (Jupyter Notebook)](examples/api_configuration/fred_api_configuration.ipynb)
+- [FRED API Key Configuration Guide (Markdown)](https://github.com/nathanramoscfa/pyeconomics/blob/main/markdown/FRED_API_CONFIGURATION.md)
+- [FRED API Key Configuration Guide (Jupyter Notebook)](https://github.com/nathanramoscfa/pyeconomics/blob/main/examples/api_configuration/fred_api_configuration.ipynb)
 
 ## Usage
 
 Here are some basic examples of how to use PyEconomics for calculating and visualizing monetary policy rules.
 
 ### Example 1: Calculate Current Policy Rule Estimates
 
@@ -144,16 +144,16 @@
 import pyeconomics as pyecon
 
 # Calculate policy rule estimates
 policy_estimates = pyecon.calculate_policy_rule_estimates(verbose=True)
 ```
 
 Verbose Print Statement:
-```
 
+```text
 ┌───────────────────────────────────────────────────────────────────────────────────┐
 │                           Interest Rate Policy Estimates                          │
 ├───────────────────────────────────────────────────────────────────────────────────┤
 │ Taylor Rule (TR)                                                      6.17%       │
 │ Balanced Approach Rule (BAR)                                          6.68%       │
 │ Balanced Approach Shortfalls Rule (BASR)                              5.66%       │
 │ First Difference Rule (FDR)                                           5.97%       │
@@ -186,15 +186,15 @@
     apply_elb=apply_elb,
     verbose=True
 )
 ```
 
 Verbose Print Statement:
 
-```
+```text
 ┌───────────────────────────────────────────────────────────────────────────────────┐
 │                      Adjusted Interest Rate Policy Estimates                      │
 ├───────────────────────────────────────────────────────────────────────────────────┤
 │ Taylor Rule (TR)                                                      5.70%       │
 │ Balanced Approach Rule (BAR)                                          5.86%       │
 │ Balanced Approach Shortfalls Rule (BASR)                              5.55%       │
 │ First Difference Rule (FDR)                                           5.64%       │
@@ -220,15 +220,15 @@
 
 # Calculate policy rule estimates
 policy_estimates = pyecon.taylor_rule(verbose=True)
 ```
 
 Verbose Print Statement:
 
-```
+```text
 ==== Economic Indicators =================================================
 Current Inflation:                               3.04%
 Target Inflation:                                2.00%
 Current Unemployment Rate:                       3.90%
 Natural Unemployment Rate:                       4.41%
 Long-Term Real Interest Rate:                    2.10%
 Current Fed Rate:                                5.50%
@@ -274,15 +274,17 @@
 # Calculate historical policy rates
 historical_policy_estimates = pyecon.calculate_historical_policy_rates().dropna()
 
 # Plot historical policy rates
 pyecon.plot_historical_rule_estimates(historical_policy_estimates)
 ```
 
-![plot_historical_policy.png](media/plot_historical_policy_rates.png)
+<p style="text-align: center;">
+    <img width="100%" src="https://github.com/nathanramoscfa/pyeconomics/blob/main/media/plot_historical_policy_rates.png?raw=true" alt="Policy Rules Plot">
+</p>
 
 ### Example 5: Calculate and Plot the Adjusted Historical Policy Rules Adjusted
 
 ```python
 # Import pyeconomics modules
 import pyeconomics as pyecon
 
@@ -297,19 +299,22 @@
 ).dropna()
 
 # Plot adjusted historical policy rates
 pyecon.plot_historical_rule_estimates(
     adjusted_historical_policy_estimates,
     adjusted=True)
 ```
-![plot_adj_historical_rates.png](media/plot_adj_historical_rates.png)
+
+<p style="text-align: center;">
+    <img width="100%" src="https://github.com/nathanramoscfa/pyeconomics/blob/main/media/plot_adj_historical_rates.png?raw=true" alt="Policy Rules Plot">
+</p>
 
 ### Examples
 
-For more comprehensive examples, refer to the [examples](examples) directory in
+For more comprehensive examples, refer to the [examples](https://github.com/nathanramoscfa/pyeconomics/tree/main/examples) directory in
 the repository.
 
 ## Docker
 
 To run PyEconomics using Docker, follow these steps:
 
 1. **Configure the .env File**:
@@ -353,15 +358,15 @@
 
 By using Docker, you ensure a consistent environment for running and testing 
 PyEconomics.
 
 ## Roadmap
 
 The following models and categories are planned for future development. 
-[Contributions](#contributing) are welcome!
+[Contributions](https://github.com/nathanramoscfa/pyeconomics/blob/main/markdown/CONTRIBUTING.md) are welcome!
 
 <details>
 <summary><strong>Monetary Policy Models</strong></summary>
 
 - Taylor Rule
 - Balanced Approach Rule
 - First Difference Rule
@@ -467,18 +472,18 @@
 
 </details>
 
 ## Contributing
 
 Contributions are welcome! If you have a model you'd like to implement or an 
 improvement to an existing model, please refer to our detailed 
-[Contributing Guide](markdown/CONTRIBUTING.md).
+[Contributing Guide](https://github.com/nathanramoscfa/pyeconomics/blob/main/markdown/CONTRIBUTING.md).
 
 By participating in this project, you agree to abide by the 
-[Code of Conduct](markdown/CODE_OF_CONDUCT.md).
+[Code of Conduct](https://github.com/nathanramoscfa/pyeconomics/blob/main/markdown/CODE_OF_CONDUCT.md).
 
 Thank you for your contributions!
 
 ## Contact
 
 If you have any questions, suggestions, or need support, feel free to reach out.
```

### Comparing `pyeconomics-0.2.2/README.md` & `pyeconomics-0.2.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -20,22 +20,22 @@
 | **Maintainability** | [![Maintainability](https://api.codeclimate.com/v1/badges/8d0d8b5a5bed8fe94814/maintainability)](https://codeclimate.com/github/nathanramoscfa/pyeconomics/maintainability)                                                                                                                                                                                                                                  |
 | **Code Style**      | [![Code Style: Flake8](https://img.shields.io/badge/code%20style-flake8-brightgreen.svg)](https://github.com/PyCQA/flake8)                                                                                                                                                                                                                                                                                   |
 | **Dependencies**    | [![Dependency Status](https://img.shields.io/librariesio/github/nathanramoscfa/pyeconomics)](https://libraries.io/github/nathanramoscfa/pyeconomics)                                                                                                                                                                                                                                                         |
 | **Security**        | [![Security Status](https://snyk.io/test/github/nathanramoscfa/pyeconomics/badge.svg)](https://snyk.io/test/github/nathanramoscfa/pyeconomics)                                                                                                                                                                                                                                                               |
 
 ## Table of Contents
 
-- [Introduction](#introduction)
-- [Features](#features)
-- [Installation](#installation)
-- [Usage](#usage)
-- [Docker](#docker)
-- [Roadmap](#roadmap)
-- [Contributing](#contributing)
-- [Contact](#contact)
+- [Introduction](https://github.com/nathanramoscfa/pyeconomics?tab=readme-ov-file#introduction)
+- [Features](https://github.com/nathanramoscfa/pyeconomics?tab=readme-ov-file#features)
+- [Installation](https://github.com/nathanramoscfa/pyeconomics?tab=readme-ov-file#installation)
+- [Usage](https://github.com/nathanramoscfa/pyeconomics?tab=readme-ov-file#usage)
+- [Docker](https://github.com/nathanramoscfa/pyeconomics?tab=readme-ov-file#docker)
+- [Roadmap](https://github.com/nathanramoscfa/pyeconomics?tab=readme-ov-file#roadmap)
+- [Contributing](https://github.com/nathanramoscfa/pyeconomics?tab=readme-ov-file#contributing)
+- [Contact](https://github.com/nathanramoscfa/pyeconomics?tab=readme-ov-file#contact)
 
 ## Introduction
 
 PyEconomics is a versatile and comprehensive library that integrates various
 economic and financial models. It is designed to support the development and
 analysis of monetary policy rules, exchange rate models, macroeconomic and
 microeconomic models, discounted cash flow models, and much more.
@@ -94,16 +94,16 @@
 
 Some features of PyEconomics require access to the FRED API. To use these 
 features, you need to configure your FRED API access. 
 
 A detailed step-by-step guide on obtaining and securely storing your FRED API 
 key is available here:
 
-- [FRED API Key Configuration Guide (Markdown)](markdown/FRED_API_CONFIGURATION.md)
-- [FRED API Key Configuration Guide (Jupyter Notebook)](examples/api_configuration/fred_api_configuration.ipynb)
+- [FRED API Key Configuration Guide (Markdown)](https://github.com/nathanramoscfa/pyeconomics/blob/main/markdown/FRED_API_CONFIGURATION.md)
+- [FRED API Key Configuration Guide (Jupyter Notebook)](https://github.com/nathanramoscfa/pyeconomics/blob/main/examples/api_configuration/fred_api_configuration.ipynb)
 
 ## Usage
 
 Here are some basic examples of how to use PyEconomics for calculating and visualizing monetary policy rules.
 
 ### Example 1: Calculate Current Policy Rule Estimates
 
@@ -112,16 +112,16 @@
 import pyeconomics as pyecon
 
 # Calculate policy rule estimates
 policy_estimates = pyecon.calculate_policy_rule_estimates(verbose=True)
 ```
 
 Verbose Print Statement:
-```
 
+```text
 ┌───────────────────────────────────────────────────────────────────────────────────┐
 │                           Interest Rate Policy Estimates                          │
 ├───────────────────────────────────────────────────────────────────────────────────┤
 │ Taylor Rule (TR)                                                      6.17%       │
 │ Balanced Approach Rule (BAR)                                          6.68%       │
 │ Balanced Approach Shortfalls Rule (BASR)                              5.66%       │
 │ First Difference Rule (FDR)                                           5.97%       │
@@ -154,15 +154,15 @@
     apply_elb=apply_elb,
     verbose=True
 )
 ```
 
 Verbose Print Statement:
 
-```
+```text
 ┌───────────────────────────────────────────────────────────────────────────────────┐
 │                      Adjusted Interest Rate Policy Estimates                      │
 ├───────────────────────────────────────────────────────────────────────────────────┤
 │ Taylor Rule (TR)                                                      5.70%       │
 │ Balanced Approach Rule (BAR)                                          5.86%       │
 │ Balanced Approach Shortfalls Rule (BASR)                              5.55%       │
 │ First Difference Rule (FDR)                                           5.64%       │
@@ -188,15 +188,15 @@
 
 # Calculate policy rule estimates
 policy_estimates = pyecon.taylor_rule(verbose=True)
 ```
 
 Verbose Print Statement:
 
-```
+```text
 ==== Economic Indicators =================================================
 Current Inflation:                               3.04%
 Target Inflation:                                2.00%
 Current Unemployment Rate:                       3.90%
 Natural Unemployment Rate:                       4.41%
 Long-Term Real Interest Rate:                    2.10%
 Current Fed Rate:                                5.50%
@@ -242,15 +242,17 @@
 # Calculate historical policy rates
 historical_policy_estimates = pyecon.calculate_historical_policy_rates().dropna()
 
 # Plot historical policy rates
 pyecon.plot_historical_rule_estimates(historical_policy_estimates)
 ```
 
-![plot_historical_policy.png](media/plot_historical_policy_rates.png)
+<p style="text-align: center;">
+    <img width="100%" src="https://github.com/nathanramoscfa/pyeconomics/blob/main/media/plot_historical_policy_rates.png?raw=true" alt="Policy Rules Plot">
+</p>
 
 ### Example 5: Calculate and Plot the Adjusted Historical Policy Rules Adjusted
 
 ```python
 # Import pyeconomics modules
 import pyeconomics as pyecon
 
@@ -265,19 +267,22 @@
 ).dropna()
 
 # Plot adjusted historical policy rates
 pyecon.plot_historical_rule_estimates(
     adjusted_historical_policy_estimates,
     adjusted=True)
 ```
-![plot_adj_historical_rates.png](media/plot_adj_historical_rates.png)
+
+<p style="text-align: center;">
+    <img width="100%" src="https://github.com/nathanramoscfa/pyeconomics/blob/main/media/plot_adj_historical_rates.png?raw=true" alt="Policy Rules Plot">
+</p>
 
 ### Examples
 
-For more comprehensive examples, refer to the [examples](examples) directory in
+For more comprehensive examples, refer to the [examples](https://github.com/nathanramoscfa/pyeconomics/tree/main/examples) directory in
 the repository.
 
 ## Docker
 
 To run PyEconomics using Docker, follow these steps:
 
 1. **Configure the .env File**:
@@ -321,15 +326,15 @@
 
 By using Docker, you ensure a consistent environment for running and testing 
 PyEconomics.
 
 ## Roadmap
 
 The following models and categories are planned for future development. 
-[Contributions](#contributing) are welcome!
+[Contributions](https://github.com/nathanramoscfa/pyeconomics/blob/main/markdown/CONTRIBUTING.md) are welcome!
 
 <details>
 <summary><strong>Monetary Policy Models</strong></summary>
 
 - Taylor Rule
 - Balanced Approach Rule
 - First Difference Rule
@@ -435,18 +440,18 @@
 
 </details>
 
 ## Contributing
 
 Contributions are welcome! If you have a model you'd like to implement or an 
 improvement to an existing model, please refer to our detailed 
-[Contributing Guide](markdown/CONTRIBUTING.md).
+[Contributing Guide](https://github.com/nathanramoscfa/pyeconomics/blob/main/markdown/CONTRIBUTING.md).
 
 By participating in this project, you agree to abide by the 
-[Code of Conduct](markdown/CODE_OF_CONDUCT.md).
+[Code of Conduct](https://github.com/nathanramoscfa/pyeconomics/blob/main/markdown/CODE_OF_CONDUCT.md).
 
 Thank you for your contributions!
 
 ## Contact
 
 If you have any questions, suggestions, or need support, feel free to reach out.
```

### Comparing `pyeconomics-0.2.2/docs/Makefile` & `pyeconomics-0.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/docs/_static/logo.png` & `pyeconomics-0.2.3/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/docs/conf.py` & `pyeconomics-0.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/docs/contact.rst` & `pyeconomics-0.2.3/docs/contact.rst`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/docs/create_roadmap_files.bat` & `pyeconomics-0.2.3/docs/create_roadmap_files.bat`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/docs/docker.rst` & `pyeconomics-0.2.3/docs/docker.rst`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/docs/features.rst` & `pyeconomics-0.2.3/docs/features.rst`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/docs/index.rst` & `pyeconomics-0.2.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/docs/introduction.rst` & `pyeconomics-0.2.3/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/docs/make.bat` & `pyeconomics-0.2.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/docs/usage.rst` & `pyeconomics-0.2.3/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/examples/api_configuration/fred_api_configuration.ipynb` & `pyeconomics-0.2.3/examples/api_configuration/fred_api_configuration.ipynb`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/examples/monetary_policy_rules/balanced_approach_rule.ipynb` & `pyeconomics-0.2.3/examples/monetary_policy_rules/balanced_approach_rule.ipynb`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/examples/monetary_policy_rules/first_difference_rule.ipynb` & `pyeconomics-0.2.3/examples/monetary_policy_rules/first_difference_rule.ipynb`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/examples/monetary_policy_rules/monetary_policy_rules.ipynb` & `pyeconomics-0.2.3/examples/monetary_policy_rules/monetary_policy_rules.ipynb`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/examples/monetary_policy_rules/taylor_rule.ipynb` & `pyeconomics-0.2.3/examples/monetary_policy_rules/taylor_rule.ipynb`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/markdown/CHANGELOG.md` & `pyeconomics-0.2.3/markdown/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/markdown/CODE_OF_CONDUCT.md` & `pyeconomics-0.2.3/markdown/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/markdown/CONTRIBUTING.md` & `pyeconomics-0.2.3/markdown/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/markdown/FRED_API_CONFIGURATION.md` & `pyeconomics-0.2.3/markdown/FRED_API_CONFIGURATION.md`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/media/plot_adj_historical_rates.png` & `pyeconomics-0.2.3/media/plot_adj_historical_rates.png`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/media/plot_historical_policy_rates.png` & `pyeconomics-0.2.3/media/plot_historical_policy_rates.png`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/pyeconomics/__init__.py` & `pyeconomics-0.2.3/pyeconomics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/pyeconomics/api/cache_manager.py` & `pyeconomics-0.2.3/pyeconomics/api/cache_manager.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/pyeconomics/api/fred_api.py` & `pyeconomics-0.2.3/pyeconomics/api/fred_api.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/pyeconomics/api/fred_data.py` & `pyeconomics-0.2.3/pyeconomics/api/fred_data.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/pyeconomics/data/economic_indicators.py` & `pyeconomics-0.2.3/pyeconomics/data/economic_indicators.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/pyeconomics/data/model_parameters.py` & `pyeconomics-0.2.3/pyeconomics/data/model_parameters.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/pyeconomics/models/monetary_policy/__init__.py` & `pyeconomics-0.2.3/pyeconomics/models/monetary_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/pyeconomics/models/monetary_policy/balanced_approach_rule.py` & `pyeconomics-0.2.3/pyeconomics/models/monetary_policy/balanced_approach_rule.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/pyeconomics/models/monetary_policy/first_difference_rule.py` & `pyeconomics-0.2.3/pyeconomics/models/monetary_policy/first_difference_rule.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/pyeconomics/models/monetary_policy/monetary_policy_rules.py` & `pyeconomics-0.2.3/pyeconomics/models/monetary_policy/monetary_policy_rules.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/pyeconomics/models/monetary_policy/taylor_rule.py` & `pyeconomics-0.2.3/pyeconomics/models/monetary_policy/taylor_rule.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/pyeconomics/utils/bar_utils.py` & `pyeconomics-0.2.3/pyeconomics/utils/bar_utils.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/pyeconomics/utils/fdr_utils.py` & `pyeconomics-0.2.3/pyeconomics/utils/fdr_utils.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/pyeconomics/utils/tr_utils.py` & `pyeconomics-0.2.3/pyeconomics/utils/tr_utils.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/pyeconomics.egg-info/PKG-INFO` & `pyeconomics-0.2.3/pyeconomics.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pyeconomics
-Version: 0.2.2
+Version: 0.2.3
 Summary: A library for economic and financial analysis
 Home-page: https://github.com/nathanramoscfa/pyeconomics
 Author: Nathan Ramos, CFA
 Author-email: nathan.ramos.github@gmail.com
 Project-URL: Bug Reports, https://github.com/nathanramoscfa/pyeconomics/issues
 Project-URL: Source, https://github.com/nathanramoscfa/pyeconomics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Requires-Python: >=3.11, <3.13
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fredapi~=0.5.1
 Requires-Dist: jupyterlab~=4.1.8
 Requires-Dist: keyring~=25.2.0
@@ -52,22 +52,22 @@
 | **Maintainability** | [![Maintainability](https://api.codeclimate.com/v1/badges/8d0d8b5a5bed8fe94814/maintainability)](https://codeclimate.com/github/nathanramoscfa/pyeconomics/maintainability)                                                                                                                                                                                                                                  |
 | **Code Style**      | [![Code Style: Flake8](https://img.shields.io/badge/code%20style-flake8-brightgreen.svg)](https://github.com/PyCQA/flake8)                                                                                                                                                                                                                                                                                   |
 | **Dependencies**    | [![Dependency Status](https://img.shields.io/librariesio/github/nathanramoscfa/pyeconomics)](https://libraries.io/github/nathanramoscfa/pyeconomics)                                                                                                                                                                                                                                                         |
 | **Security**        | [![Security Status](https://snyk.io/test/github/nathanramoscfa/pyeconomics/badge.svg)](https://snyk.io/test/github/nathanramoscfa/pyeconomics)                                                                                                                                                                                                                                                               |
 
 ## Table of Contents
 
-- [Introduction](#introduction)
-- [Features](#features)
-- [Installation](#installation)
-- [Usage](#usage)
-- [Docker](#docker)
-- [Roadmap](#roadmap)
-- [Contributing](#contributing)
-- [Contact](#contact)
+- [Introduction](https://github.com/nathanramoscfa/pyeconomics?tab=readme-ov-file#introduction)
+- [Features](https://github.com/nathanramoscfa/pyeconomics?tab=readme-ov-file#features)
+- [Installation](https://github.com/nathanramoscfa/pyeconomics?tab=readme-ov-file#installation)
+- [Usage](https://github.com/nathanramoscfa/pyeconomics?tab=readme-ov-file#usage)
+- [Docker](https://github.com/nathanramoscfa/pyeconomics?tab=readme-ov-file#docker)
+- [Roadmap](https://github.com/nathanramoscfa/pyeconomics?tab=readme-ov-file#roadmap)
+- [Contributing](https://github.com/nathanramoscfa/pyeconomics?tab=readme-ov-file#contributing)
+- [Contact](https://github.com/nathanramoscfa/pyeconomics?tab=readme-ov-file#contact)
 
 ## Introduction
 
 PyEconomics is a versatile and comprehensive library that integrates various
 economic and financial models. It is designed to support the development and
 analysis of monetary policy rules, exchange rate models, macroeconomic and
 microeconomic models, discounted cash flow models, and much more.
@@ -126,16 +126,16 @@
 
 Some features of PyEconomics require access to the FRED API. To use these 
 features, you need to configure your FRED API access. 
 
 A detailed step-by-step guide on obtaining and securely storing your FRED API 
 key is available here:
 
-- [FRED API Key Configuration Guide (Markdown)](markdown/FRED_API_CONFIGURATION.md)
-- [FRED API Key Configuration Guide (Jupyter Notebook)](examples/api_configuration/fred_api_configuration.ipynb)
+- [FRED API Key Configuration Guide (Markdown)](https://github.com/nathanramoscfa/pyeconomics/blob/main/markdown/FRED_API_CONFIGURATION.md)
+- [FRED API Key Configuration Guide (Jupyter Notebook)](https://github.com/nathanramoscfa/pyeconomics/blob/main/examples/api_configuration/fred_api_configuration.ipynb)
 
 ## Usage
 
 Here are some basic examples of how to use PyEconomics for calculating and visualizing monetary policy rules.
 
 ### Example 1: Calculate Current Policy Rule Estimates
 
@@ -144,16 +144,16 @@
 import pyeconomics as pyecon
 
 # Calculate policy rule estimates
 policy_estimates = pyecon.calculate_policy_rule_estimates(verbose=True)
 ```
 
 Verbose Print Statement:
-```
 
+```text
 ┌───────────────────────────────────────────────────────────────────────────────────┐
 │                           Interest Rate Policy Estimates                          │
 ├───────────────────────────────────────────────────────────────────────────────────┤
 │ Taylor Rule (TR)                                                      6.17%       │
 │ Balanced Approach Rule (BAR)                                          6.68%       │
 │ Balanced Approach Shortfalls Rule (BASR)                              5.66%       │
 │ First Difference Rule (FDR)                                           5.97%       │
@@ -186,15 +186,15 @@
     apply_elb=apply_elb,
     verbose=True
 )
 ```
 
 Verbose Print Statement:
 
-```
+```text
 ┌───────────────────────────────────────────────────────────────────────────────────┐
 │                      Adjusted Interest Rate Policy Estimates                      │
 ├───────────────────────────────────────────────────────────────────────────────────┤
 │ Taylor Rule (TR)                                                      5.70%       │
 │ Balanced Approach Rule (BAR)                                          5.86%       │
 │ Balanced Approach Shortfalls Rule (BASR)                              5.55%       │
 │ First Difference Rule (FDR)                                           5.64%       │
@@ -220,15 +220,15 @@
 
 # Calculate policy rule estimates
 policy_estimates = pyecon.taylor_rule(verbose=True)
 ```
 
 Verbose Print Statement:
 
-```
+```text
 ==== Economic Indicators =================================================
 Current Inflation:                               3.04%
 Target Inflation:                                2.00%
 Current Unemployment Rate:                       3.90%
 Natural Unemployment Rate:                       4.41%
 Long-Term Real Interest Rate:                    2.10%
 Current Fed Rate:                                5.50%
@@ -274,15 +274,17 @@
 # Calculate historical policy rates
 historical_policy_estimates = pyecon.calculate_historical_policy_rates().dropna()
 
 # Plot historical policy rates
 pyecon.plot_historical_rule_estimates(historical_policy_estimates)
 ```
 
-![plot_historical_policy.png](media/plot_historical_policy_rates.png)
+<p style="text-align: center;">
+    <img width="100%" src="https://github.com/nathanramoscfa/pyeconomics/blob/main/media/plot_historical_policy_rates.png?raw=true" alt="Policy Rules Plot">
+</p>
 
 ### Example 5: Calculate and Plot the Adjusted Historical Policy Rules Adjusted
 
 ```python
 # Import pyeconomics modules
 import pyeconomics as pyecon
 
@@ -297,19 +299,22 @@
 ).dropna()
 
 # Plot adjusted historical policy rates
 pyecon.plot_historical_rule_estimates(
     adjusted_historical_policy_estimates,
     adjusted=True)
 ```
-![plot_adj_historical_rates.png](media/plot_adj_historical_rates.png)
+
+<p style="text-align: center;">
+    <img width="100%" src="https://github.com/nathanramoscfa/pyeconomics/blob/main/media/plot_adj_historical_rates.png?raw=true" alt="Policy Rules Plot">
+</p>
 
 ### Examples
 
-For more comprehensive examples, refer to the [examples](examples) directory in
+For more comprehensive examples, refer to the [examples](https://github.com/nathanramoscfa/pyeconomics/tree/main/examples) directory in
 the repository.
 
 ## Docker
 
 To run PyEconomics using Docker, follow these steps:
 
 1. **Configure the .env File**:
@@ -353,15 +358,15 @@
 
 By using Docker, you ensure a consistent environment for running and testing 
 PyEconomics.
 
 ## Roadmap
 
 The following models and categories are planned for future development. 
-[Contributions](#contributing) are welcome!
+[Contributions](https://github.com/nathanramoscfa/pyeconomics/blob/main/markdown/CONTRIBUTING.md) are welcome!
 
 <details>
 <summary><strong>Monetary Policy Models</strong></summary>
 
 - Taylor Rule
 - Balanced Approach Rule
 - First Difference Rule
@@ -467,18 +472,18 @@
 
 </details>
 
 ## Contributing
 
 Contributions are welcome! If you have a model you'd like to implement or an 
 improvement to an existing model, please refer to our detailed 
-[Contributing Guide](markdown/CONTRIBUTING.md).
+[Contributing Guide](https://github.com/nathanramoscfa/pyeconomics/blob/main/markdown/CONTRIBUTING.md).
 
 By participating in this project, you agree to abide by the 
-[Code of Conduct](markdown/CODE_OF_CONDUCT.md).
+[Code of Conduct](https://github.com/nathanramoscfa/pyeconomics/blob/main/markdown/CODE_OF_CONDUCT.md).
 
 Thank you for your contributions!
 
 ## Contact
 
 If you have any questions, suggestions, or need support, feel free to reach out.
```

### Comparing `pyeconomics-0.2.2/pyeconomics.egg-info/SOURCES.txt` & `pyeconomics-0.2.3/pyeconomics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/setup.py` & `pyeconomics-0.2.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Intended Audience :: Financial and Insurance Industry',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
-        'Topic :: Software Development :: Libraries :: Python Modules',
+        'Topic :: Office/Business :: Financial',
         'Topic :: Office/Business :: Financial :: Investment'
     ],
     python_requires='>=3.11, <3.13',
     project_urls={
         'Bug Reports': 'https://github.com/nathanramoscfa/pyeconomics/issues',
         'Source': 'https://github.com/nathanramoscfa/pyeconomics',
     },
```

### Comparing `pyeconomics-0.2.2/tests/conftest.py` & `pyeconomics-0.2.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/tests/test_balanced_approach_rule.py` & `pyeconomics-0.2.3/tests/test_balanced_approach_rule.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/tests/test_bar_utils.py` & `pyeconomics-0.2.3/tests/test_bar_utils.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/tests/test_cache_manager.py` & `pyeconomics-0.2.3/tests/test_cache_manager.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/tests/test_fdr_utils.py` & `pyeconomics-0.2.3/tests/test_fdr_utils.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/tests/test_first_difference_rule.py` & `pyeconomics-0.2.3/tests/test_first_difference_rule.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/tests/test_fred_api.py` & `pyeconomics-0.2.3/tests/test_fred_api.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/tests/test_fred_data.py` & `pyeconomics-0.2.3/tests/test_fred_data.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/tests/test_monetary_policy_rules.py` & `pyeconomics-0.2.3/tests/test_monetary_policy_rules.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/tests/test_taylor_rule.py` & `pyeconomics-0.2.3/tests/test_taylor_rule.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.2/tests/test_tr_utils.py` & `pyeconomics-0.2.3/tests/test_tr_utils.py`

 * *Files identical despite different names*

