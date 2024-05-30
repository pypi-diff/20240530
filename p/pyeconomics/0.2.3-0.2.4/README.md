# Comparing `tmp/pyeconomics-0.2.3.tar.gz` & `tmp/pyeconomics-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyeconomics-0.2.3.tar", last modified: Thu May 30 16:17:28 2024, max compression
+gzip compressed data, was "pyeconomics-0.2.4.tar", last modified: Thu May 30 18:29:40 2024, max compression
```

## Comparing `pyeconomics-0.2.3.tar` & `pyeconomics-0.2.4.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:17:28.721917 pyeconomics-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:17:28.705917 pyeconomics-0.2.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:17:28.705917 pyeconomics-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    24941 2024-05-30 16:17:28.721917 pyeconomics-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23679 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:17:28.709917 pyeconomics-0.2.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:17:28.709917 pyeconomics-0.2.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    69539 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:17:28.709917 pyeconomics-0.2.3/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/_templates/.keep
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/api_key.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/contact.rst
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/create_roadmap_files.bat
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/docker.rst
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/features.rst
--rw-r--r--   0 runner    (1001) docker     (127)    19195 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/roadmap.rst
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/roadmap_discounted_cash_flow_models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/roadmap_exchange_rate_models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/roadmap_financial_models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/roadmap_fiscal_policy_models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/roadmap_macroeconomic_models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/roadmap_microeconomic_models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/roadmap_monetary_policy_models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/roadmap_other_economic_models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/roadmap_quantity_of_money_theory.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10580 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:17:28.701917 pyeconomics-0.2.3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:17:28.709917 pyeconomics-0.2.3/examples/api_configuration/
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/examples/api_configuration/fred_api_configuration.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:17:28.713917 pyeconomics-0.2.3/examples/monetary_policy_rules/
--rw-r--r--   0 runner    (1001) docker     (127)   214512 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/examples/monetary_policy_rules/balanced_approach_rule.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   125883 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/examples/monetary_policy_rules/first_difference_rule.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   286474 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/examples/monetary_policy_rules/monetary_policy_rules.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   118525 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/examples/monetary_policy_rules/taylor_rule.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:17:28.713917 pyeconomics-0.2.3/markdown/
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/markdown/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/markdown/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/markdown/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/markdown/FRED_API_CONFIGURATION.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:17:28.713917 pyeconomics-0.2.3/media/
--rw-r--r--   0 runner    (1001) docker     (127)   181489 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/media/plot_adj_historical_rates.png
--rw-r--r--   0 runner    (1001) docker     (127)   181531 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/media/plot_historical_policy_rates.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:17:28.713917 pyeconomics-0.2.3/pyeconomics/
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyeconomics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyeconomics/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:17:28.713917 pyeconomics-0.2.3/pyeconomics/api/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyeconomics/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyeconomics/api/cache_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     7668 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyeconomics/api/fred_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyeconomics/api/fred_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:17:28.717917 pyeconomics-0.2.3/pyeconomics/data/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyeconomics/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyeconomics/data/economic_indicators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyeconomics/data/model_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:17:28.717917 pyeconomics-0.2.3/pyeconomics/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyeconomics/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:17:28.717917 pyeconomics-0.2.3/pyeconomics/models/monetary_policy/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyeconomics/models/monetary_policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9556 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyeconomics/models/monetary_policy/balanced_approach_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyeconomics/models/monetary_policy/first_difference_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    12879 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyeconomics/models/monetary_policy/monetary_policy_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     8327 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyeconomics/models/monetary_policy/taylor_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:17:28.717917 pyeconomics-0.2.3/pyeconomics/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyeconomics/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6728 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyeconomics/utils/bar_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyeconomics/utils/fdr_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyeconomics/utils/tr_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:17:28.713917 pyeconomics-0.2.3/pyeconomics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    24941 2024-05-30 16:17:28.000000 pyeconomics-0.2.3/pyeconomics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-30 16:17:28.000000 pyeconomics-0.2.3/pyeconomics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 16:17:28.000000 pyeconomics-0.2.3/pyeconomics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-30 16:17:28.000000 pyeconomics-0.2.3/pyeconomics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 16:17:28.000000 pyeconomics-0.2.3/pyeconomics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 16:17:28.721917 pyeconomics-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:17:28.721917 pyeconomics-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/tests/test_balanced_approach_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    14924 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/tests/test_bar_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/tests/test_cache_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/tests/test_fdr_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11865 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/tests/test_first_difference_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9744 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/tests/test_fred_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/tests/test_fred_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10175 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/tests/test_monetary_policy_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/tests/test_taylor_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    11867 2024-05-30 16:16:52.000000 pyeconomics-0.2.3/tests/test_tr_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:29:40.166037 pyeconomics-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:29:40.150036 pyeconomics-0.2.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:29:40.154037 pyeconomics-0.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    24943 2024-05-30 18:29:40.166037 pyeconomics-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23681 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:29:40.158037 pyeconomics-0.2.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:29:40.158037 pyeconomics-0.2.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    69539 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:29:40.158037 pyeconomics-0.2.4/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/docs/_templates/.keep
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/docs/api_key.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/docs/contact.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/docs/create_roadmap_files.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/docs/docker.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/docs/features.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    19770 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/docs/roadmap.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/docs/roadmap_discounted_cash_flow_models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/docs/roadmap_exchange_rate_models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/docs/roadmap_financial_models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/docs/roadmap_fiscal_policy_models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/docs/roadmap_macroeconomic_models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/docs/roadmap_microeconomic_models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/docs/roadmap_monetary_policy_models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/docs/roadmap_other_economic_models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/docs/roadmap_quantity_of_money_theory.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10580 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:29:40.146036 pyeconomics-0.2.4/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:29:40.158037 pyeconomics-0.2.4/examples/api_configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/examples/api_configuration/fred_api_configuration.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:29:40.158037 pyeconomics-0.2.4/examples/monetary_policy_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)   214512 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/examples/monetary_policy_rules/balanced_approach_rule.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   125883 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/examples/monetary_policy_rules/first_difference_rule.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   286474 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/examples/monetary_policy_rules/monetary_policy_rules.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   118525 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/examples/monetary_policy_rules/taylor_rule.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:29:40.158037 pyeconomics-0.2.4/markdown/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/markdown/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/markdown/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/markdown/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/markdown/FRED_API_CONFIGURATION.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:29:40.158037 pyeconomics-0.2.4/media/
+-rw-r--r--   0 runner    (1001) docker     (127)   181489 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/media/plot_adj_historical_rates.png
+-rw-r--r--   0 runner    (1001) docker     (127)   181531 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/media/plot_historical_policy_rates.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:29:40.162037 pyeconomics-0.2.4/pyeconomics/
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/pyeconomics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 18:29:02.000000 pyeconomics-0.2.4/pyeconomics/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:29:40.162037 pyeconomics-0.2.4/pyeconomics/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/pyeconomics/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/pyeconomics/api/cache_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7668 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/pyeconomics/api/fred_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/pyeconomics/api/fred_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:29:40.162037 pyeconomics-0.2.4/pyeconomics/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/pyeconomics/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/pyeconomics/data/economic_indicators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/pyeconomics/data/model_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:29:40.162037 pyeconomics-0.2.4/pyeconomics/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/pyeconomics/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:29:40.162037 pyeconomics-0.2.4/pyeconomics/models/monetary_policy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/pyeconomics/models/monetary_policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9556 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/pyeconomics/models/monetary_policy/balanced_approach_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/pyeconomics/models/monetary_policy/first_difference_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12879 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/pyeconomics/models/monetary_policy/monetary_policy_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8327 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/pyeconomics/models/monetary_policy/taylor_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:29:40.162037 pyeconomics-0.2.4/pyeconomics/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/pyeconomics/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6728 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/pyeconomics/utils/bar_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/pyeconomics/utils/fdr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/pyeconomics/utils/tr_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:29:40.162037 pyeconomics-0.2.4/pyeconomics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    24943 2024-05-30 18:29:40.000000 pyeconomics-0.2.4/pyeconomics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-30 18:29:40.000000 pyeconomics-0.2.4/pyeconomics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 18:29:40.000000 pyeconomics-0.2.4/pyeconomics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-30 18:29:40.000000 pyeconomics-0.2.4/pyeconomics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 18:29:40.000000 pyeconomics-0.2.4/pyeconomics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 18:29:40.166037 pyeconomics-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:29:40.166037 pyeconomics-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/tests/test_balanced_approach_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14924 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/tests/test_bar_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/tests/test_cache_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/tests/test_fdr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11865 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/tests/test_first_difference_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9744 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/tests/test_fred_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/tests/test_fred_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10175 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/tests/test_monetary_policy_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/tests/test_taylor_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11867 2024-05-30 18:29:01.000000 pyeconomics-0.2.4/tests/test_tr_utils.py
```

### Comparing `pyeconomics-0.2.3/.dockerignore` & `pyeconomics-0.2.4/.dockerignore`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/.editorconfig` & `pyeconomics-0.2.4/.editorconfig`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/.github/workflows/docs.yml` & `pyeconomics-0.2.4/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/.github/workflows/release.yml` & `pyeconomics-0.2.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/.github/workflows/tests.yml` & `pyeconomics-0.2.4/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/.gitignore` & `pyeconomics-0.2.4/.gitignore`

 * *Files 12% similar despite different names*

```diff
@@ -104,14 +104,16 @@
 .DS_Store
 Thumbs.db
 
 # Miscellaneous files
 *.csv
 *.json
 secrets.py
+render_readme.py
+output.html
 
 # Virtual environments
 env/
 venv/
 ENV/
 env.bak/
 venv.bak/
```

### Comparing `pyeconomics-0.2.3/Dockerfile` & `pyeconomics-0.2.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/LICENSE` & `pyeconomics-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/MANIFEST.in` & `pyeconomics-0.2.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/PKG-INFO` & `pyeconomics-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyeconomics
-Version: 0.2.3
+Version: 0.2.4
 Summary: A library for economic and financial analysis
 Home-page: https://github.com/nathanramoscfa/pyeconomics
 Author: Nathan Ramos, CFA
 Author-email: nathan.ramos.github@gmail.com
 Project-URL: Bug Reports, https://github.com/nathanramoscfa/pyeconomics/issues
 Project-URL: Source, https://github.com/nathanramoscfa/pyeconomics
 Classifier: Development Status :: 3 - Alpha
@@ -145,15 +145,15 @@
 
 # Calculate policy rule estimates
 policy_estimates = pyecon.calculate_policy_rule_estimates(verbose=True)
 ```
 
 Verbose Print Statement:
 
-```text
+<pre>
 ┌───────────────────────────────────────────────────────────────────────────────────┐
 │                           Interest Rate Policy Estimates                          │
 ├───────────────────────────────────────────────────────────────────────────────────┤
 │ Taylor Rule (TR)                                                      6.17%       │
 │ Balanced Approach Rule (BAR)                                          6.68%       │
 │ Balanced Approach Shortfalls Rule (BASR)                              5.66%       │
 │ First Difference Rule (FDR)                                           5.97%       │
@@ -165,15 +165,15 @@
 │                                Policy Prescription                                │
 ├───────────────────────────────────────────────────────────────────────────────────┤
 │ Taylor Rule (TR) suggests raising the rate by 0.75%.                              │
 │ Balanced Approach Rule (BAR) suggests raising the rate by 1.25%.                  │
 │ Balanced Approach Shortfalls Rule (BASR) suggests raising the rate by 0.25%.      │
 │ First Difference Rule (FDR) suggests raising the rate by 0.50%.                   │
 └───────────────────────────────────────────────────────────────────────────────────┘
-```
+</pre>
 
 ### Example 2: Adjust Taylor Rule for Effective Lower Bound (ELB) and Policy Inertia
 
 ```python
 # Import pyeconomics
 import pyeconomics as pyecon
 
@@ -186,15 +186,15 @@
     apply_elb=apply_elb,
     verbose=True
 )
 ```
 
 Verbose Print Statement:
 
-```text
+<pre>
 ┌───────────────────────────────────────────────────────────────────────────────────┐
 │                      Adjusted Interest Rate Policy Estimates                      │
 ├───────────────────────────────────────────────────────────────────────────────────┤
 │ Taylor Rule (TR)                                                      5.70%       │
 │ Balanced Approach Rule (BAR)                                          5.86%       │
 │ Balanced Approach Shortfalls Rule (BASR)                              5.55%       │
 │ First Difference Rule (FDR)                                           5.64%       │
@@ -206,15 +206,15 @@
 │                            Adjusted Policy Prescription                           │
 ├───────────────────────────────────────────────────────────────────────────────────┤
 │ Taylor Rule (TR) suggests raising the rate by 0.25%.                              │
 │ Balanced Approach Rule (BAR) suggests raising the rate by 0.25%.                  │
 │ Balanced Approach Shortfalls Rule (BASR) suggests maintaining the current rate.   │
 │ First Difference Rule (FDR) suggests raising the rate by 0.25%.                   │
 └───────────────────────────────────────────────────────────────────────────────────┘
-```
+</pre>
 
 ### Example 3: Calculate Current Taylor Rule Estimates
 
 ```python
 # Import pyeconomics modules
 import pyeconomics as pyecon
```

### Comparing `pyeconomics-0.2.3/README.md` & `pyeconomics-0.2.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 
 # Calculate policy rule estimates
 policy_estimates = pyecon.calculate_policy_rule_estimates(verbose=True)
 ```
 
 Verbose Print Statement:
 
-```text
+<pre>
 ┌───────────────────────────────────────────────────────────────────────────────────┐
 │                           Interest Rate Policy Estimates                          │
 ├───────────────────────────────────────────────────────────────────────────────────┤
 │ Taylor Rule (TR)                                                      6.17%       │
 │ Balanced Approach Rule (BAR)                                          6.68%       │
 │ Balanced Approach Shortfalls Rule (BASR)                              5.66%       │
 │ First Difference Rule (FDR)                                           5.97%       │
@@ -133,15 +133,15 @@
 │                                Policy Prescription                                │
 ├───────────────────────────────────────────────────────────────────────────────────┤
 │ Taylor Rule (TR) suggests raising the rate by 0.75%.                              │
 │ Balanced Approach Rule (BAR) suggests raising the rate by 1.25%.                  │
 │ Balanced Approach Shortfalls Rule (BASR) suggests raising the rate by 0.25%.      │
 │ First Difference Rule (FDR) suggests raising the rate by 0.50%.                   │
 └───────────────────────────────────────────────────────────────────────────────────┘
-```
+</pre>
 
 ### Example 2: Adjust Taylor Rule for Effective Lower Bound (ELB) and Policy Inertia
 
 ```python
 # Import pyeconomics
 import pyeconomics as pyecon
 
@@ -154,15 +154,15 @@
     apply_elb=apply_elb,
     verbose=True
 )
 ```
 
 Verbose Print Statement:
 
-```text
+<pre>
 ┌───────────────────────────────────────────────────────────────────────────────────┐
 │                      Adjusted Interest Rate Policy Estimates                      │
 ├───────────────────────────────────────────────────────────────────────────────────┤
 │ Taylor Rule (TR)                                                      5.70%       │
 │ Balanced Approach Rule (BAR)                                          5.86%       │
 │ Balanced Approach Shortfalls Rule (BASR)                              5.55%       │
 │ First Difference Rule (FDR)                                           5.64%       │
@@ -174,15 +174,15 @@
 │                            Adjusted Policy Prescription                           │
 ├───────────────────────────────────────────────────────────────────────────────────┤
 │ Taylor Rule (TR) suggests raising the rate by 0.25%.                              │
 │ Balanced Approach Rule (BAR) suggests raising the rate by 0.25%.                  │
 │ Balanced Approach Shortfalls Rule (BASR) suggests maintaining the current rate.   │
 │ First Difference Rule (FDR) suggests raising the rate by 0.25%.                   │
 └───────────────────────────────────────────────────────────────────────────────────┘
-```
+</pre>
 
 ### Example 3: Calculate Current Taylor Rule Estimates
 
 ```python
 # Import pyeconomics modules
 import pyeconomics as pyecon
```

### Comparing `pyeconomics-0.2.3/docs/Makefile` & `pyeconomics-0.2.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/docs/_static/logo.png` & `pyeconomics-0.2.4/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/docs/conf.py` & `pyeconomics-0.2.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/docs/contact.rst` & `pyeconomics-0.2.4/docs/contact.rst`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/docs/create_roadmap_files.bat` & `pyeconomics-0.2.4/docs/create_roadmap_files.bat`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/docs/docker.rst` & `pyeconomics-0.2.4/docs/docker.rst`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/docs/features.rst` & `pyeconomics-0.2.4/docs/features.rst`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/docs/index.rst` & `pyeconomics-0.2.4/docs/index.rst`

 * *Files 9% similar despite different names*

```diff
@@ -36,1165 +36,1201 @@
 00000230: 6465 6c69 6e67 2061 6e64 2061 6e61 6c79  deling and analy
 00000240: 7369 732e 0a0a 2e2e 206c 6973 742d 7461  sis..... list-ta
 00000250: 626c 653a 3a0a 2020 203a 6865 6164 6572  ble::.   :header
 00000260: 2d72 6f77 733a 2031 0a0a 2020 202a 202d  -rows: 1..   * -
 00000270: 2043 6174 6567 6f72 790a 2020 2020 202d   Category.     -
 00000280: 2042 6164 6765 0a20 2020 2a20 2d20 2a2a   Badge.   * - **
 00000290: 5465 7374 696e 672a 2a0a 2020 2020 202d  Testing**.     -
-000002a0: 2060 215b 7079 7465 7374 5d28 6874 7470   `![pytest](http
-000002b0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6e  s://github.com/n
-000002c0: 6174 6861 6e72 616d 6f73 6366 612f 7079  athanramoscfa/py
-000002d0: 6563 6f6e 6f6d 6963 732f 6163 7469 6f6e  economics/action
-000002e0: 732f 776f 726b 666c 6f77 732f 7465 7374  s/workflows/test
-000002f0: 732e 796d 6c2f 6261 6467 652e 7376 6729  s.yml/badge.svg)
-00000300: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000310: 2e63 6f6d 2f6e 6174 6861 6e72 616d 6f73  .com/nathanramos
-00000320: 6366 612f 7079 6563 6f6e 6f6d 6963 732f  cfa/pyeconomics/
-00000330: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
-00000340: 732f 7465 7374 732e 796d 6c29 205b 215b  s/tests.yml) [![
-00000350: 636f 6465 636f 765d 2868 7474 7073 3a2f  codecov](https:/
-00000360: 2f63 6f64 6563 6f76 2e69 6f2f 6768 2f6e  /codecov.io/gh/n
-00000370: 6174 6861 6e72 616d 6f73 6366 612f 7079  athanramoscfa/py
-00000380: 6563 6f6e 6f6d 6963 732f 6772 6170 682f  economics/graph/
-00000390: 6261 6467 652e 7376 673f 746f 6b65 6e3d  badge.svg?token=
-000003a0: 4931 4352 4844 4e37 3353 295d 2868 7474  I1CRHDN73S)](htt
-000003b0: 7073 3a2f 2f63 6f64 6563 6f76 2e69 6f2f  ps://codecov.io/
-000003c0: 6768 2f6e 6174 6861 6e72 616d 6f73 6366  gh/nathanramoscf
-000003d0: 612f 7079 6563 6f6e 6f6d 6963 7329 600a  a/pyeconomics)`.
-000003e0: 2020 202a 202d 202a 2a50 6163 6b61 6765     * - **Package
-000003f0: 2a2a 0a20 2020 2020 2d20 605b 215b 5079  **.     - `[![Py
-00000400: 5049 204c 6174 6573 7420 5265 6c65 6173  PI Latest Releas
-00000410: 655d 2868 7474 7073 3a2f 2f69 6d67 2e73  e](https://img.s
-00000420: 6869 656c 6473 2e69 6f2f 7079 7069 2f76  hields.io/pypi/v
-00000430: 2f70 7965 636f 6e6f 6d69 6373 2e73 7667  /pyeconomics.svg
-00000440: 295d 2868 7474 7073 3a2f 2f70 7970 692e  )](https://pypi.
-00000450: 6f72 672f 7072 6f6a 6563 742f 7079 6563  org/project/pyec
-00000460: 6f6e 6f6d 6963 732f 2920 215b 5079 7468  onomics/) ![Pyth
-00000470: 6f6e 2056 6572 7369 6f6e 5d28 6874 7470  on Version](http
-00000480: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000490: 696f 2f70 7970 692f 7079 7665 7273 696f  io/pypi/pyversio
-000004a0: 6e73 2f70 7965 636f 6e6f 6d69 6373 2920  ns/pyeconomics) 
-000004b0: 5b21 5b50 7950 4920 446f 776e 6c6f 6164  [![PyPI Download
-000004c0: 735d 2868 7474 7073 3a2f 2f73 7461 7469  s](https://stati
-000004d0: 632e 7065 7079 2e74 6563 682f 6261 6467  c.pepy.tech/badg
-000004e0: 652f 7079 6563 6f6e 6f6d 6963 7329 5d28  e/pyeconomics)](
-000004f0: 6874 7470 733a 2f2f 7065 7079 2e74 6563  https://pepy.tec
-00000500: 682f 7072 6f6a 6563 742f 7079 6563 6f6e  h/project/pyecon
-00000510: 6f6d 6963 7329 205b 215b 4c69 6365 6e73  omics) [![Licens
-00000520: 653a 204d 4954 5d28 6874 7470 733a 2f2f  e: MIT](https://
-00000530: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
-00000540: 6164 6765 2f4c 6963 656e 7365 2d4d 4954  adge/License-MIT
-00000550: 2d62 7269 6768 7467 7265 656e 2e73 7667  -brightgreen.svg
-00000560: 295d 2868 7474 7073 3a2f 2f6f 7065 6e73  )](https://opens
-00000570: 6f75 7263 652e 6f72 672f 6c69 6365 6e73  ource.org/licens
-00000580: 6573 2f4d 4954 2960 0a20 2020 2a20 2d20  es/MIT)`.   * - 
-00000590: 2a2a 446f 6375 6d65 6e74 6174 696f 6e2a  **Documentation*
-000005a0: 2a0a 2020 2020 202d 2060 5b21 5b44 6f63  *.     - `[![Doc
-000005b0: 756d 656e 7461 7469 6f6e 2053 7461 7475  umentation Statu
-000005c0: 735d 2868 7474 7073 3a2f 2f72 6561 6474  s](https://readt
-000005d0: 6865 646f 6373 2e6f 7267 2f70 726f 6a65  hedocs.org/proje
-000005e0: 6374 732f 7079 6563 6f6e 6f6d 6963 732f  cts/pyeconomics/
-000005f0: 6261 6467 652f 3f76 6572 7369 6f6e 3d6c  badge/?version=l
-00000600: 6174 6573 7429 5d28 6874 7470 733a 2f2f  atest)](https://
-00000610: 7079 6563 6f6e 6f6d 6963 732e 7265 6164  pyeconomics.read
-00000620: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
-00000630: 7465 7374 2f3f 6261 6467 653d 6c61 7465  test/?badge=late
-00000640: 7374 2960 0a20 2020 2a20 2d20 2a2a 5265  st)`.   * - **Re
-00000650: 6c65 6173 652a 2a0a 2020 2020 202d 2060  lease**.     - `
-00000660: 5b21 5b52 656c 6561 7365 2053 7461 7475  [![Release Statu
-00000670: 735d 2868 7474 7073 3a2f 2f67 6974 6875  s](https://githu
-00000680: 622e 636f 6d2f 6e61 7468 616e 7261 6d6f  b.com/nathanramo
-00000690: 7363 6661 2f70 7965 636f 6e6f 6d69 6373  scfa/pyeconomics
-000006a0: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-000006b0: 7773 2f72 656c 6561 7365 2e79 6d6c 2f62  ws/release.yml/b
-000006c0: 6164 6765 2e73 7667 295d 2868 7474 7073  adge.svg)](https
-000006d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6e61  ://github.com/na
-000006e0: 7468 616e 7261 6d6f 7363 6661 2f70 7965  thanramoscfa/pye
-000006f0: 636f 6e6f 6d69 6373 2f61 6374 696f 6e73  conomics/actions
-00000700: 2f77 6f72 6b66 6c6f 7773 2f72 656c 6561  /workflows/relea
-00000710: 7365 2e79 6d6c 2960 0a20 2020 2a20 2d20  se.yml)`.   * - 
-00000720: 2a2a 4275 696c 6420 5374 6174 7573 2a2a  **Build Status**
-00000730: 0a20 2020 2020 2d20 605b 215b 4275 696c  .     - `[![Buil
-00000740: 6420 5374 6174 7573 5d28 6874 7470 733a  d Status](https:
-00000750: 2f2f 6769 7468 7562 2e63 6f6d 2f6e 6174  //github.com/nat
-00000760: 6861 6e72 616d 6f73 6366 612f 7079 6563  hanramoscfa/pyec
-00000770: 6f6e 6f6d 6963 732f 6163 7469 6f6e 732f  onomics/actions/
-00000780: 776f 726b 666c 6f77 732f 7465 7374 732e  workflows/tests.
-00000790: 796d 6c2f 6261 6467 652e 7376 6729 5d28  yml/badge.svg)](
-000007a0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000007b0: 6f6d 2f6e 6174 6861 6e72 616d 6f73 6366  om/nathanramoscf
-000007c0: 612f 7079 6563 6f6e 6f6d 6963 732f 6163  a/pyeconomics/ac
-000007d0: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
-000007e0: 7465 7374 732e 796d 6c29 600a 2020 202a  tests.yml)`.   *
-000007f0: 202d 202a 2a4d 6169 6e74 6169 6e61 6269   - **Maintainabi
-00000800: 6c69 7479 2a2a 0a20 2020 2020 2d20 605b  lity**.     - `[
-00000810: 215b 4d61 696e 7461 696e 6162 696c 6974  ![Maintainabilit
-00000820: 795d 2868 7474 7073 3a2f 2f61 7069 2e63  y](https://api.c
-00000830: 6f64 6563 6c69 6d61 7465 2e63 6f6d 2f76  odeclimate.com/v
-00000840: 312f 6261 6467 6573 2f38 6430 6438 6235  1/badges/8d0d8b5
-00000850: 6135 6265 6438 6665 3934 3831 342f 6d61  a5bed8fe94814/ma
-00000860: 696e 7461 696e 6162 696c 6974 7929 5d28  intainability)](
-00000870: 6874 7470 733a 2f2f 636f 6465 636c 696d  https://codeclim
-00000880: 6174 652e 636f 6d2f 6769 7468 7562 2f6e  ate.com/github/n
-00000890: 6174 6861 6e72 616d 6f73 6366 612f 7079  athanramoscfa/py
-000008a0: 6563 6f6e 6f6d 6963 732f 6d61 696e 7461  economics/mainta
-000008b0: 696e 6162 696c 6974 7929 600a 2020 202a  inability)`.   *
-000008c0: 202d 202a 2a43 6f64 6520 5374 796c 652a   - **Code Style*
-000008d0: 2a0a 2020 2020 202d 2060 5b21 5b43 6f64  *.     - `[![Cod
-000008e0: 6520 5374 796c 653a 2046 6c61 6b65 385d  e Style: Flake8]
-000008f0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000900: 656c 6473 2e69 6f2f 6261 6467 652f 636f  elds.io/badge/co
-00000910: 6465 2532 3073 7479 6c65 2d66 6c61 6b65  de%20style-flake
-00000920: 382d 6272 6967 6874 6772 6565 6e2e 7376  8-brightgreen.sv
-00000930: 6729 5d28 6874 7470 733a 2f2f 6769 7468  g)](https://gith
-00000940: 7562 2e63 6f6d 2f50 7943 5141 2f66 6c61  ub.com/PyCQA/fla
-00000950: 6b65 3829 600a 2020 202a 202d 202a 2a44  ke8)`.   * - **D
-00000960: 6570 656e 6465 6e63 6965 732a 2a0a 2020  ependencies**.  
-00000970: 2020 202d 2060 5b21 5b44 6570 656e 6465     - `[![Depende
-00000980: 6e63 7920 5374 6174 7573 5d28 6874 7470  ncy Status](http
-00000990: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-000009a0: 696f 2f6c 6962 7261 7269 6573 696f 2f67  io/librariesio/g
-000009b0: 6974 6875 622f 6e61 7468 616e 7261 6d6f  ithub/nathanramo
-000009c0: 7363 6661 2f70 7965 636f 6e6f 6d69 6373  scfa/pyeconomics
-000009d0: 295d 2868 7474 7073 3a2f 2f6c 6962 7261  )](https://libra
-000009e0: 7269 6573 2e69 6f2f 6769 7468 7562 2f6e  ries.io/github/n
-000009f0: 6174 6861 6e72 616d 6f73 6366 612f 7079  athanramoscfa/py
-00000a00: 6563 6f6e 6f6d 6963 7329 600a 2020 202a  economics)`.   *
-00000a10: 202d 202a 2a53 6563 7572 6974 792a 2a0a   - **Security**.
-00000a20: 2020 2020 202d 2060 5b21 5b53 6563 7572       - `[![Secur
-00000a30: 6974 7920 5374 6174 7573 5d28 6874 7470  ity Status](http
-00000a40: 733a 2f2f 736e 796b 2e69 6f2f 7465 7374  s://snyk.io/test
-00000a50: 2f67 6974 6875 622f 6e61 7468 616e 7261  /github/nathanra
-00000a60: 6d6f 7363 6661 2f70 7965 636f 6e6f 6d69  moscfa/pyeconomi
-00000a70: 6373 2f62 6164 6765 2e73 7667 295d 2868  cs/badge.svg)](h
-00000a80: 7474 7073 3a2f 2f73 6e79 6b2e 696f 2f74  ttps://snyk.io/t
-00000a90: 6573 742f 6769 7468 7562 2f6e 6174 6861  est/github/natha
-00000aa0: 6e72 616d 6f73 6366 612f 7079 6563 6f6e  nramoscfa/pyecon
-00000ab0: 6f6d 6963 7329 600a 0a43 6f6e 7465 6e74  omics)`..Content
-00000ac0: 730a 3d3d 3d3d 3d3d 3d3d 0a0a 2e2e 2074  s.========.... t
-00000ad0: 6f63 7472 6565 3a3a 0a20 2020 3a6d 6178  octree::.   :max
-00000ae0: 6465 7074 683a 2032 0a20 2020 3a63 6170  depth: 2.   :cap
-00000af0: 7469 6f6e 3a20 436f 6e74 656e 7473 3a0a  tion: Contents:.
-00000b00: 0a20 2020 696e 7472 6f64 7563 7469 6f6e  .   introduction
-00000b10: 0a20 2020 6665 6174 7572 6573 0a20 2020  .   features.   
-00000b20: 696e 7374 616c 6c61 7469 6f6e 0a20 2020  installation.   
-00000b30: 6170 695f 6b65 790a 2020 2075 7361 6765  api_key.   usage
-00000b40: 0a20 2020 646f 636b 6572 0a20 2020 726f  .   docker.   ro
-00000b50: 6164 6d61 700a 2020 2063 6f6e 7472 6962  admap.   contrib
-00000b60: 7574 696e 670a 2020 2063 6f6e 7461 6374  uting.   contact
-00000b70: 0a0a 496e 7472 6f64 7563 7469 6f6e 0a3d  ..Introduction.=
-00000b80: 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 0a50 7945  ===========..PyE
-00000b90: 636f 6e6f 6d69 6373 2069 7320 6120 7665  conomics is a ve
-00000ba0: 7273 6174 696c 6520 616e 6420 636f 6d70  rsatile and comp
-00000bb0: 7265 6865 6e73 6976 6520 6c69 6272 6172  rehensive librar
-00000bc0: 7920 7468 6174 2069 6e74 6567 7261 7465  y that integrate
-00000bd0: 7320 7661 7269 6f75 730a 6563 6f6e 6f6d  s various.econom
-00000be0: 6963 2061 6e64 2066 696e 616e 6369 616c  ic and financial
-00000bf0: 206d 6f64 656c 732e 2049 7420 6973 2064   models. It is d
-00000c00: 6573 6967 6e65 6420 746f 2073 7570 706f  esigned to suppo
-00000c10: 7274 2074 6865 2064 6576 656c 6f70 6d65  rt the developme
-00000c20: 6e74 2061 6e64 0a61 6e61 6c79 7369 7320  nt and.analysis 
-00000c30: 6f66 206d 6f6e 6574 6172 7920 706f 6c69  of monetary poli
-00000c40: 6379 2072 756c 6573 2c20 6578 6368 616e  cy rules, exchan
-00000c50: 6765 2072 6174 6520 6d6f 6465 6c73 2c20  ge rate models, 
-00000c60: 6d61 6372 6f65 636f 6e6f 6d69 6320 616e  macroeconomic an
-00000c70: 640a 6d69 6372 6f65 636f 6e6f 6d69 6320  d.microeconomic 
-00000c80: 6d6f 6465 6c73 2c20 6469 7363 6f75 6e74  models, discount
-00000c90: 6564 2063 6173 6820 666c 6f77 206d 6f64  ed cash flow mod
-00000ca0: 656c 732c 2061 6e64 206d 7563 6820 6d6f  els, and much mo
-00000cb0: 7265 2e0a 0a46 6561 7475 7265 730a 3d3d  re...Features.==
-00000cc0: 3d3d 3d3d 3d3d 0a0a 4375 7272 656e 7420  ======..Current 
-00000cd0: 4665 6174 7572 6573 0a2d 2d2d 2d2d 2d2d  Features.-------
-00000ce0: 2d2d 2d2d 2d2d 2d2d 2d0a 0a2d 202a 2a4d  ---------..- **M
-00000cf0: 6f6e 6574 6172 7920 506f 6c69 6379 2052  onetary Policy R
-00000d00: 756c 6573 2a2a 3a20 496d 706c 656d 656e  ules**: Implemen
-00000d10: 7461 7469 6f6e 206f 6620 7765 6c6c 2d6b  tation of well-k
-00000d20: 6e6f 776e 206d 6f6e 6574 6172 7920 706f  nown monetary po
-00000d30: 6c69 6379 2072 756c 6573 2e0a 2d20 2a2a  licy rules..- **
-00000d40: 4361 6368 6520 4d61 6e61 6765 6d65 6e74  Cache Management
-00000d50: 2a2a 3a20 4566 6669 6369 656e 7420 6361  **: Efficient ca
-00000d60: 6368 696e 6720 666f 7220 4150 4920 6361  ching for API ca
-00000d70: 6c6c 7320 746f 2069 6d70 726f 7665 2070  lls to improve p
-00000d80: 6572 666f 726d 616e 6365 0a20 2061 6e64  erformance.  and
-00000d90: 2072 6564 7563 6520 7265 6475 6e64 616e   reduce redundan
-00000da0: 7420 6461 7461 2066 6574 6368 696e 672e  t data fetching.
-00000db0: 0a0a 506c 616e 6e65 6420 4665 6174 7572  ..Planned Featur
-00000dc0: 6573 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  es.-------------
-00000dd0: 2d2d 2d0a 0a2d 202a 2a45 7863 6861 6e67  ---..- **Exchang
-00000de0: 6520 5261 7465 204d 6f64 656c 732a 2a3a  e Rate Models**:
-00000df0: 204d 6f64 656c 7320 666f 7220 7072 6564   Models for pred
-00000e00: 6963 7469 6e67 2066 7574 7572 6520 6578  icting future ex
-00000e10: 6368 616e 6765 2072 6174 6573 2e0a 2d20  change rates..- 
-00000e20: 2a2a 4d61 6372 6f65 636f 6e6f 6d69 6320  **Macroeconomic 
-00000e30: 4d6f 6465 6c73 2a2a 3a20 436f 6d70 7265  Models**: Compre
-00000e40: 6865 6e73 6976 6520 6d61 6372 6f65 636f  hensive macroeco
-00000e50: 6e6f 6d69 6320 6d6f 6465 6c73 2e0a 2d20  nomic models..- 
-00000e60: 2a2a 4d69 6372 6f65 636f 6e6f 6d69 6320  **Microeconomic 
-00000e70: 4d6f 6465 6c73 2a2a 3a20 4465 7461 696c  Models**: Detail
-00000e80: 6564 206d 6963 726f 6563 6f6e 6f6d 6963  ed microeconomic
-00000e90: 206d 6f64 656c 732e 0a2d 202a 2a44 6973   models..- **Dis
-00000ea0: 636f 756e 7465 6420 4361 7368 2046 6c6f  counted Cash Flo
-00000eb0: 7720 4d6f 6465 6c73 2a2a 3a20 4164 7661  w Models**: Adva
-00000ec0: 6e63 6564 206d 6f64 656c 7320 666f 7220  nced models for 
-00000ed0: 6469 7363 6f75 6e74 6564 2063 6173 6820  discounted cash 
-00000ee0: 666c 6f77 0a20 2061 6e61 6c79 7369 732e  flow.  analysis.
-00000ef0: 0a2d 202a 2a46 696e 616e 6369 616c 204d  .- **Financial M
-00000f00: 6f64 656c 732a 2a3a 2049 6e63 6c75 6469  odels**: Includi
-00000f10: 6e67 2043 4150 4d20 616e 6420 706f 7274  ng CAPM and port
-00000f20: 666f 6c69 6f20 6f70 7469 6d69 7a61 7469  folio optimizati
-00000f30: 6f6e 2e0a 2d20 2a2a 4669 7363 616c 2050  on..- **Fiscal P
-00000f40: 6f6c 6963 7920 4d6f 6465 6c73 2a2a 3a20  olicy Models**: 
-00000f50: 546f 6f6c 7320 746f 2061 6e61 6c79 7a65  Tools to analyze
-00000f60: 2074 6178 6174 696f 6e2c 2067 6f76 6572   taxation, gover
-00000f70: 6e6d 656e 7420 7370 656e 6469 6e67 2c20  nment spending, 
-00000f80: 616e 640a 2020 7075 626c 6963 2064 6562  and.  public deb
-00000f90: 742e 0a2d 202a 2a41 6464 6974 696f 6e61  t..- **Additiona
-00000fa0: 6c20 4563 6f6e 6f6d 6963 204d 6f64 656c  l Economic Model
-00000fb0: 732a 2a3a 2053 7570 706f 7274 2066 6f72  s**: Support for
-00000fc0: 2062 6568 6176 696f 7261 6c20 6563 6f6e   behavioral econ
-00000fd0: 6f6d 6963 732c 2061 6765 6e74 2d62 6173  omics, agent-bas
-00000fe0: 6564 0a20 206d 6f64 656c 732c 2061 6e64  ed.  models, and
-00000ff0: 2069 6e74 6572 6e61 7469 6f6e 616c 2074   international t
-00001000: 7261 6465 206d 6f64 656c 732e 0a0a 496e  rade models...In
-00001010: 7374 616c 6c61 7469 6f6e 0a3d 3d3d 3d3d  stallation.=====
-00001020: 3d3d 3d3d 3d3d 3d0a 0a54 6f20 696e 7374  =======..To inst
-00001030: 616c 6c20 5079 4563 6f6e 6f6d 6963 732c  all PyEconomics,
-00001040: 2075 7365 2060 6070 6970 6060 3a0a 0a2e   use ``pip``:...
-00001050: 2e20 636f 6465 2d62 6c6f 636b 3a3a 2073  . code-block:: s
-00001060: 680a 0a20 2020 7069 7020 696e 7374 616c  h..   pip instal
-00001070: 6c20 7079 6563 6f6e 6f6d 6963 730a 0a46  l pyeconomics..F
-00001080: 726f 6d20 536f 7572 6365 0a2d 2d2d 2d2d  rom Source.-----
-00001090: 2d2d 2d2d 2d2d 0a0a 4966 2079 6f75 2077  ------..If you w
-000010a0: 616e 7420 746f 2069 6e73 7461 6c6c 2074  ant to install t
-000010b0: 6865 2070 6163 6b61 6765 2066 726f 6d20  he package from 
-000010c0: 7468 6520 736f 7572 6365 2063 6f64 652c  the source code,
-000010d0: 2066 6f6c 6c6f 7720 7468 6573 6520 7374   follow these st
-000010e0: 6570 733a 0a0a 312e 2043 6c6f 6e65 2074  eps:..1. Clone t
-000010f0: 6865 2072 6570 6f73 6974 6f72 793a 0a0a  he repository:..
-00001100: 2020 2020 2e2e 2063 6f64 652d 626c 6f63      .. code-bloc
-00001110: 6b3a 3a20 7368 0a0a 2020 2020 2020 2067  k:: sh..       g
-00001120: 6974 2063 6c6f 6e65 2068 7474 7073 3a2f  it clone https:/
-00001130: 2f67 6974 6875 622e 636f 6d2f 6e61 7468  /github.com/nath
-00001140: 616e 7261 6d6f 7363 6661 2f70 7965 636f  anramoscfa/pyeco
-00001150: 6e6f 6d69 6373 2e67 6974 0a0a 322e 2043  nomics.git..2. C
-00001160: 6861 6e67 6520 746f 2074 6865 2070 726f  hange to the pro
-00001170: 6a65 6374 2064 6972 6563 746f 7279 3a0a  ject directory:.
-00001180: 0a20 2020 202e 2e20 636f 6465 2d62 6c6f  .    .. code-blo
-00001190: 636b 3a3a 2073 680a 0a20 2020 2020 2020  ck:: sh..       
-000011a0: 6364 2070 7965 636f 6e6f 6d69 6373 0a0a  cd pyeconomics..
-000011b0: 332e 2049 6e73 7461 6c6c 2074 6865 2070  3. Install the p
-000011c0: 6163 6b61 6765 3a0a 0a20 2020 202e 2e20  ackage:..    .. 
-000011d0: 636f 6465 2d62 6c6f 636b 3a3a 2073 680a  code-block:: sh.
-000011e0: 0a20 2020 2020 2020 7069 7020 696e 7374  .       pip inst
-000011f0: 616c 6c20 2e0a 0a41 5049 204b 6579 0a3d  all ...API Key.=
-00001200: 3d3d 3d3d 3d3d 0a0a 536f 6d65 2066 6561  ======..Some fea
-00001210: 7475 7265 7320 6f66 2050 7945 636f 6e6f  tures of PyEcono
-00001220: 6d69 6373 2072 6571 7569 7265 2061 6363  mics require acc
-00001230: 6573 7320 746f 2074 6865 2046 5245 4420  ess to the FRED 
-00001240: 4150 492e 2054 6f20 7573 6520 7468 6573  API. To use thes
-00001250: 650a 6665 6174 7572 6573 2c20 796f 7520  e.features, you 
-00001260: 6e65 6564 2074 6f20 636f 6e66 6967 7572  need to configur
-00001270: 6520 796f 7572 2046 5245 4420 4150 4920  e your FRED API 
-00001280: 6163 6365 7373 2e0a 0a41 2064 6574 6169  access...A detai
-00001290: 6c65 6420 7374 6570 2d62 792d 7374 6570  led step-by-step
-000012a0: 2067 7569 6465 206f 6e20 6f62 7461 696e   guide on obtain
-000012b0: 696e 6720 616e 6420 7365 6375 7265 6c79  ing and securely
-000012c0: 2073 746f 7269 6e67 2079 6f75 7220 4652   storing your FR
-000012d0: 4544 2041 5049 0a6b 6579 2069 7320 6176  ED API.key is av
-000012e0: 6169 6c61 626c 6520 6865 7265 3a0a 0a2d  ailable here:..-
-000012f0: 2060 4652 4544 2041 5049 204b 6579 2043   `FRED API Key C
-00001300: 6f6e 6669 6775 7261 7469 6f6e 2047 7569  onfiguration Gui
-00001310: 6465 2028 4d61 726b 646f 776e 2920 3c6d  de (Markdown) <m
-00001320: 6172 6b64 6f77 6e2f 4652 4544 5f41 5049  arkdown/FRED_API
-00001330: 5f43 4f4e 4649 4755 5241 5449 4f4e 2e6d  _CONFIGURATION.m
-00001340: 643e 605f 0a2d 2060 4652 4544 2041 5049  d>`_.- `FRED API
-00001350: 204b 6579 2043 6f6e 6669 6775 7261 7469   Key Configurati
-00001360: 6f6e 2047 7569 6465 2028 4a75 7079 7465  on Guide (Jupyte
-00001370: 7220 4e6f 7465 626f 6f6b 2920 3c65 7861  r Notebook) <exa
-00001380: 6d70 6c65 732f 6170 695f 636f 6e66 6967  mples/api_config
-00001390: 7572 6174 696f 6e2f 6672 6564 5f61 7069  uration/fred_api
-000013a0: 5f63 6f6e 6669 6775 7261 7469 6f6e 2e69  _configuration.i
-000013b0: 7079 6e62 3e60 5f0a 0a55 7361 6765 0a3d  pynb>`_..Usage.=
-000013c0: 3d3d 3d3d 0a0a 4865 7265 2061 7265 2073  ====..Here are s
-000013d0: 6f6d 6520 6261 7369 6320 6578 616d 706c  ome basic exampl
-000013e0: 6573 206f 6620 686f 7720 746f 2075 7365  es of how to use
-000013f0: 2050 7945 636f 6e6f 6d69 6373 2066 6f72   PyEconomics for
-00001400: 2063 616c 6375 6c61 7469 6e67 2061 6e64   calculating and
-00001410: 2076 6973 7561 6c69 7a69 6e67 206d 6f6e   visualizing mon
-00001420: 6574 6172 7920 706f 6c69 6379 2072 756c  etary policy rul
-00001430: 6573 2e0a 0a45 7861 6d70 6c65 2031 3a20  es...Example 1: 
-00001440: 4361 6c63 756c 6174 6520 4375 7272 656e  Calculate Curren
-00001450: 7420 506f 6c69 6379 2052 756c 6520 4573  t Policy Rule Es
-00001460: 7469 6d61 7465 730a 2d2d 2d2d 2d2d 2d2d  timates.--------
-00001470: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001480: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001490: 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 2e2e 2063  ----------.... c
-000014a0: 6f64 652d 626c 6f63 6b3a 3a20 7079 7468  ode-block:: pyth
-000014b0: 6f6e 0a0a 2020 2023 2049 6d70 6f72 7420  on..   # Import 
-000014c0: 7079 6563 6f6e 6f6d 6963 730a 2020 2069  pyeconomics.   i
-000014d0: 6d70 6f72 7420 7079 6563 6f6e 6f6d 6963  mport pyeconomic
-000014e0: 7320 6173 2070 7965 636f 6e0a 0a20 2020  s as pyecon..   
-000014f0: 2320 4361 6c63 756c 6174 6520 706f 6c69  # Calculate poli
-00001500: 6379 2072 756c 6520 6573 7469 6d61 7465  cy rule estimate
-00001510: 730a 2020 2070 6f6c 6963 795f 6573 7469  s.   policy_esti
-00001520: 6d61 7465 7320 3d20 7079 6563 6f6e 2e63  mates = pyecon.c
-00001530: 616c 6375 6c61 7465 5f70 6f6c 6963 795f  alculate_policy_
-00001540: 7275 6c65 5f65 7374 696d 6174 6573 2876  rule_estimates(v
-00001550: 6572 626f 7365 3d54 7275 6529 0a0a 5665  erbose=True)..Ve
-00001560: 7262 6f73 6520 5072 696e 7420 5374 6174  rbose Print Stat
-00001570: 656d 656e 743a 0a0a 2e2e 2063 6f64 652d  ement:.... code-
-00001580: 626c 6f63 6b3a 3a20 6e6f 6e65 0a0a 2020  block:: none..  
-00001590: 20e2 948c e294 80e2 9480 e294 80e2 9480   ...............
-000015a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000015b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000015c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000015d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000015e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000015f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001600: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001610: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001620: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001630: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001640: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001650: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001660: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001670: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001680: 80e2 9480 e294 80e2 9480 e294 80e2 9490  ................
-00001690: 0a20 2020 e294 8220 2020 2020 2020 2020  .   ...         
-000016a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016b0: 2020 496e 7465 7265 7374 2052 6174 6520    Interest Rate 
-000016c0: 506f 6c69 6379 2045 7374 696d 6174 6573  Policy Estimates
-000016d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016e0: 2020 2020 2020 2020 2020 e294 820a 2020            ....  
-000016f0: 20e2 949c e294 80e2 9480 e294 80e2 9480   ...............
-00001700: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001710: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001720: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001730: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001740: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001750: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001760: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001770: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001780: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001790: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000017a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000017b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000017c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000017d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000017e0: 80e2 9480 e294 80e2 9480 e294 80e2 94a4  ................
-000017f0: 0a20 2020 e294 8220 5461 796c 6f72 2052  .   ... Taylor R
-00001800: 756c 6520 2854 5229 2020 2020 2020 2020  ule (TR)        
-00001810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001830: 2020 2020 2020 2020 2020 2020 2020 362e                6.
-00001840: 3137 2520 2020 2020 2020 e294 820a 2020  17%       ....  
-00001850: 20e2 9482 2042 616c 616e 6365 6420 4170   ... Balanced Ap
-00001860: 7072 6f61 6368 2052 756c 6520 2842 4152  proach Rule (BAR
-00001870: 2920 2020 2020 2020 2020 2020 2020 2020  )               
-00001880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001890: 2020 2020 2020 2020 2020 2036 2e36 3825             6.68%
-000018a0: 2020 2020 2020 20e2 9482 0a20 2020 e294         ....   ..
-000018b0: 8220 4261 6c61 6e63 6564 2041 7070 726f  . Balanced Appro
-000018c0: 6163 6820 5368 6f72 7466 616c 6c73 2052  ach Shortfalls R
-000018d0: 756c 6520 2842 4153 5229 2020 2020 2020  ule (BASR)      
+000002a0: 202e 2e20 7261 773a 3a20 6874 6d6c 0a0a   .. raw:: html..
+000002b0: 2020 2020 2020 2020 2020 203c 6120 6872             <a hr
+000002c0: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+000002d0: 7562 2e63 6f6d 2f6e 6174 6861 6e72 616d  ub.com/nathanram
+000002e0: 6f73 6366 612f 7079 6563 6f6e 6f6d 6963  oscfa/pyeconomic
+000002f0: 732f 6163 7469 6f6e 732f 776f 726b 666c  s/actions/workfl
+00000300: 6f77 732f 7465 7374 732e 796d 6c22 3e3c  ows/tests.yml"><
+00000310: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00000320: 2f67 6974 6875 622e 636f 6d2f 6e61 7468  /github.com/nath
+00000330: 616e 7261 6d6f 7363 6661 2f70 7965 636f  anramoscfa/pyeco
+00000340: 6e6f 6d69 6373 2f61 6374 696f 6e73 2f77  nomics/actions/w
+00000350: 6f72 6b66 6c6f 7773 2f74 6573 7473 2e79  orkflows/tests.y
+00000360: 6d6c 2f62 6164 6765 2e73 7667 2220 616c  ml/badge.svg" al
+00000370: 743d 2270 7974 6573 7422 3e3c 2f61 3e0a  t="pytest"></a>.
+00000380: 2020 2020 2020 2020 2020 203c 6120 6872             <a hr
+00000390: 6566 3d22 6874 7470 733a 2f2f 636f 6465  ef="https://code
+000003a0: 636f 762e 696f 2f67 682f 6e61 7468 616e  cov.io/gh/nathan
+000003b0: 7261 6d6f 7363 6661 2f70 7965 636f 6e6f  ramoscfa/pyecono
+000003c0: 6d69 6373 223e 3c69 6d67 2073 7263 3d22  mics"><img src="
+000003d0: 6874 7470 733a 2f2f 636f 6465 636f 762e  https://codecov.
+000003e0: 696f 2f67 682f 6e61 7468 616e 7261 6d6f  io/gh/nathanramo
+000003f0: 7363 6661 2f70 7965 636f 6e6f 6d69 6373  scfa/pyeconomics
+00000400: 2f67 7261 7068 2f62 6164 6765 2e73 7667  /graph/badge.svg
+00000410: 3f74 6f6b 656e 3d49 3143 5248 444e 3733  ?token=I1CRHDN73
+00000420: 5322 2061 6c74 3d22 636f 6465 636f 7622  S" alt="codecov"
+00000430: 3e3c 2f61 3e0a 2020 202a 202d 202a 2a50  ></a>.   * - **P
+00000440: 6163 6b61 6765 2a2a 0a20 2020 2020 2d20  ackage**.     - 
+00000450: 2e2e 2072 6177 3a3a 2068 746d 6c0a 0a20  .. raw:: html.. 
+00000460: 2020 2020 2020 2020 2020 3c61 2068 7265            <a hre
+00000470: 663d 2268 7474 7073 3a2f 2f70 7970 692e  f="https://pypi.
+00000480: 6f72 672f 7072 6f6a 6563 742f 7079 6563  org/project/pyec
+00000490: 6f6e 6f6d 6963 732f 223e 3c69 6d67 2073  onomics/"><img s
+000004a0: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+000004b0: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+000004c0: 762f 7079 6563 6f6e 6f6d 6963 732e 7376  v/pyeconomics.sv
+000004d0: 6722 2061 6c74 3d22 5079 5049 204c 6174  g" alt="PyPI Lat
+000004e0: 6573 7420 5265 6c65 6173 6522 3e3c 2f61  est Release"></a
+000004f0: 3e0a 2020 2020 2020 2020 2020 203c 696d  >.           <im
+00000500: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
+00000510: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+00000520: 7069 2f70 7976 6572 7369 6f6e 732f 7079  pi/pyversions/py
+00000530: 6563 6f6e 6f6d 6963 7322 2061 6c74 3d22  economics" alt="
+00000540: 5079 7468 6f6e 2056 6572 7369 6f6e 223e  Python Version">
+00000550: 0a20 2020 2020 2020 2020 2020 3c61 2068  .           <a h
+00000560: 7265 663d 2268 7474 7073 3a2f 2f70 6570  ref="https://pep
+00000570: 792e 7465 6368 2f70 726f 6a65 6374 2f70  y.tech/project/p
+00000580: 7965 636f 6e6f 6d69 6373 223e 3c69 6d67  yeconomics"><img
+00000590: 2073 7263 3d22 6874 7470 733a 2f2f 7374   src="https://st
+000005a0: 6174 6963 2e70 6570 792e 7465 6368 2f62  atic.pepy.tech/b
+000005b0: 6164 6765 2f70 7965 636f 6e6f 6d69 6373  adge/pyeconomics
+000005c0: 2220 616c 743d 2250 7950 4920 446f 776e  " alt="PyPI Down
+000005d0: 6c6f 6164 7322 3e3c 2f61 3e0a 2020 2020  loads"></a>.    
+000005e0: 2020 2020 2020 203c 6120 6872 6566 3d22         <a href="
+000005f0: 6874 7470 733a 2f2f 6f70 656e 736f 7572  https://opensour
+00000600: 6365 2e6f 7267 2f6c 6963 656e 7365 732f  ce.org/licenses/
+00000610: 4d49 5422 3e3c 696d 6720 7372 633d 2268  MIT"><img src="h
+00000620: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000630: 6473 2e69 6f2f 6261 6467 652f 4c69 6365  ds.io/badge/Lice
+00000640: 6e73 652d 4d49 542d 6272 6967 6874 6772  nse-MIT-brightgr
+00000650: 6565 6e2e 7376 6722 2061 6c74 3d22 4c69  een.svg" alt="Li
+00000660: 6365 6e73 653a 204d 4954 223e 3c2f 613e  cense: MIT"></a>
+00000670: 0a20 2020 2a20 2d20 2a2a 446f 6375 6d65  .   * - **Docume
+00000680: 6e74 6174 696f 6e2a 2a0a 2020 2020 202d  ntation**.     -
+00000690: 202e 2e20 7261 773a 3a20 6874 6d6c 0a0a   .. raw:: html..
+000006a0: 2020 2020 2020 2020 2020 203c 6120 6872             <a hr
+000006b0: 6566 3d22 6874 7470 733a 2f2f 7079 6563  ef="https://pyec
+000006c0: 6f6e 6f6d 6963 732e 7265 6164 7468 6564  onomics.readthed
+000006d0: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+000006e0: 2f3f 6261 6467 653d 6c61 7465 7374 223e  /?badge=latest">
+000006f0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000700: 2f2f 7265 6164 7468 6564 6f63 732e 6f72  //readthedocs.or
+00000710: 672f 7072 6f6a 6563 7473 2f70 7965 636f  g/projects/pyeco
+00000720: 6e6f 6d69 6373 2f62 6164 6765 2f3f 7665  nomics/badge/?ve
+00000730: 7273 696f 6e3d 6c61 7465 7374 2220 616c  rsion=latest" al
+00000740: 743d 2244 6f63 756d 656e 7461 7469 6f6e  t="Documentation
+00000750: 2053 7461 7475 7322 3e3c 2f61 3e0a 2020   Status"></a>.  
+00000760: 202a 202d 202a 2a52 656c 6561 7365 2a2a   * - **Release**
+00000770: 0a20 2020 2020 2d20 2e2e 2072 6177 3a3a  .     - .. raw::
+00000780: 2068 746d 6c0a 0a20 2020 2020 2020 2020   html..         
+00000790: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+000007a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6e61  ://github.com/na
+000007b0: 7468 616e 7261 6d6f 7363 6661 2f70 7965  thanramoscfa/pye
+000007c0: 636f 6e6f 6d69 6373 2f61 6374 696f 6e73  conomics/actions
+000007d0: 2f77 6f72 6b66 6c6f 7773 2f72 656c 6561  /workflows/relea
+000007e0: 7365 2e79 6d6c 223e 3c69 6d67 2073 7263  se.yml"><img src
+000007f0: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+00000800: 2e63 6f6d 2f6e 6174 6861 6e72 616d 6f73  .com/nathanramos
+00000810: 6366 612f 7079 6563 6f6e 6f6d 6963 732f  cfa/pyeconomics/
+00000820: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
+00000830: 732f 7265 6c65 6173 652e 796d 6c2f 6261  s/release.yml/ba
+00000840: 6467 652e 7376 6722 2061 6c74 3d22 5265  dge.svg" alt="Re
+00000850: 6c65 6173 6520 5374 6174 7573 223e 3c2f  lease Status"></
+00000860: 613e 0a20 2020 2a20 2d20 2a2a 4275 696c  a>.   * - **Buil
+00000870: 6420 5374 6174 7573 2a2a 0a20 2020 2020  d Status**.     
+00000880: 2d20 2e2e 2072 6177 3a3a 2068 746d 6c0a  - .. raw:: html.
+00000890: 0a20 2020 2020 2020 2020 2020 3c61 2068  .           <a h
+000008a0: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+000008b0: 6875 622e 636f 6d2f 6e61 7468 616e 7261  hub.com/nathanra
+000008c0: 6d6f 7363 6661 2f70 7965 636f 6e6f 6d69  moscfa/pyeconomi
+000008d0: 6373 2f61 6374 696f 6e73 2f77 6f72 6b66  cs/actions/workf
+000008e0: 6c6f 7773 2f74 6573 7473 2e79 6d6c 223e  lows/tests.yml">
+000008f0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000900: 2f2f 6769 7468 7562 2e63 6f6d 2f6e 6174  //github.com/nat
+00000910: 6861 6e72 616d 6f73 6366 612f 7079 6563  hanramoscfa/pyec
+00000920: 6f6e 6f6d 6963 732f 6163 7469 6f6e 732f  onomics/actions/
+00000930: 776f 726b 666c 6f77 732f 7465 7374 732e  workflows/tests.
+00000940: 796d 6c2f 6261 6467 652e 7376 6722 2061  yml/badge.svg" a
+00000950: 6c74 3d22 4275 696c 6420 5374 6174 7573  lt="Build Status
+00000960: 223e 3c2f 613e 0a20 2020 2a20 2d20 2a2a  "></a>.   * - **
+00000970: 4d61 696e 7461 696e 6162 696c 6974 792a  Maintainability*
+00000980: 2a0a 2020 2020 202d 202e 2e20 7261 773a  *.     - .. raw:
+00000990: 3a20 6874 6d6c 0a0a 2020 2020 2020 2020  : html..        
+000009a0: 2020 203c 6120 6872 6566 3d22 6874 7470     <a href="http
+000009b0: 733a 2f2f 636f 6465 636c 696d 6174 652e  s://codeclimate.
+000009c0: 636f 6d2f 6769 7468 7562 2f6e 6174 6861  com/github/natha
+000009d0: 6e72 616d 6f73 6366 612f 7079 6563 6f6e  nramoscfa/pyecon
+000009e0: 6f6d 6963 732f 6d61 696e 7461 696e 6162  omics/maintainab
+000009f0: 696c 6974 7922 3e3c 696d 6720 7372 633d  ility"><img src=
+00000a00: 2268 7474 7073 3a2f 2f61 7069 2e63 6f64  "https://api.cod
+00000a10: 6563 6c69 6d61 7465 2e63 6f6d 2f76 312f  eclimate.com/v1/
+00000a20: 6261 6467 6573 2f38 6430 6438 6235 6135  badges/8d0d8b5a5
+00000a30: 6265 6438 6665 3934 3831 342f 6d61 696e  bed8fe94814/main
+00000a40: 7461 696e 6162 696c 6974 7922 2061 6c74  tainability" alt
+00000a50: 3d22 4d61 696e 7461 696e 6162 696c 6974  ="Maintainabilit
+00000a60: 7922 3e3c 2f61 3e0a 2020 202a 202d 202a  y"></a>.   * - *
+00000a70: 2a43 6f64 6520 5374 796c 652a 2a0a 2020  *Code Style**.  
+00000a80: 2020 202d 202e 2e20 7261 773a 3a20 6874     - .. raw:: ht
+00000a90: 6d6c 0a0a 2020 2020 2020 2020 2020 203c  ml..           <
+00000aa0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000ab0: 6769 7468 7562 2e63 6f6d 2f50 7943 5141  github.com/PyCQA
+00000ac0: 2f66 6c61 6b65 3822 3e3c 696d 6720 7372  /flake8"><img sr
+00000ad0: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+00000ae0: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+00000af0: 636f 6465 2532 3073 7479 6c65 2d66 6c61  code%20style-fla
+00000b00: 6b65 382d 6272 6967 6874 6772 6565 6e2e  ke8-brightgreen.
+00000b10: 7376 6722 2061 6c74 3d22 436f 6465 2053  svg" alt="Code S
+00000b20: 7479 6c65 3a20 466c 616b 6538 223e 3c2f  tyle: Flake8"></
+00000b30: 613e 0a20 2020 2a20 2d20 2a2a 4465 7065  a>.   * - **Depe
+00000b40: 6e64 656e 6369 6573 2a2a 0a20 2020 2020  ndencies**.     
+00000b50: 2d20 2e2e 2072 6177 3a3a 2068 746d 6c0a  - .. raw:: html.
+00000b60: 0a20 2020 2020 2020 2020 2020 3c61 2068  .           <a h
+00000b70: 7265 663d 2268 7474 7073 3a2f 2f6c 6962  ref="https://lib
+00000b80: 7261 7269 6573 2e69 6f2f 6769 7468 7562  raries.io/github
+00000b90: 2f6e 6174 6861 6e72 616d 6f73 6366 612f  /nathanramoscfa/
+00000ba0: 7079 6563 6f6e 6f6d 6963 7322 3e3c 696d  pyeconomics"><im
+00000bb0: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
+00000bc0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6c69  mg.shields.io/li
+00000bd0: 6272 6172 6965 7369 6f2f 6769 7468 7562  brariesio/github
+00000be0: 2f6e 6174 6861 6e72 616d 6f73 6366 612f  /nathanramoscfa/
+00000bf0: 7079 6563 6f6e 6f6d 6963 7322 2061 6c74  pyeconomics" alt
+00000c00: 3d22 4465 7065 6e64 656e 6379 2053 7461  ="Dependency Sta
+00000c10: 7475 7322 3e3c 2f61 3e0a 2020 202a 202d  tus"></a>.   * -
+00000c20: 202a 2a53 6563 7572 6974 792a 2a0a 2020   **Security**.  
+00000c30: 2020 202d 202e 2e20 7261 773a 3a20 6874     - .. raw:: ht
+00000c40: 6d6c 0a0a 2020 2020 2020 2020 2020 203c  ml..           <
+00000c50: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000c60: 736e 796b 2e69 6f2f 7465 7374 2f67 6974  snyk.io/test/git
+00000c70: 6875 622f 6e61 7468 616e 7261 6d6f 7363  hub/nathanramosc
+00000c80: 6661 2f70 7965 636f 6e6f 6d69 6373 223e  fa/pyeconomics">
+00000c90: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000ca0: 2f2f 736e 796b 2e69 6f2f 7465 7374 2f67  //snyk.io/test/g
+00000cb0: 6974 6875 622f 6e61 7468 616e 7261 6d6f  ithub/nathanramo
+00000cc0: 7363 6661 2f70 7965 636f 6e6f 6d69 6373  scfa/pyeconomics
+00000cd0: 2f62 6164 6765 2e73 7667 2220 616c 743d  /badge.svg" alt=
+00000ce0: 2253 6563 7572 6974 7920 5374 6174 7573  "Security Status
+00000cf0: 223e 3c2f 613e 0a0a 436f 6e74 656e 7473  "></a>..Contents
+00000d00: 0a3d 3d3d 3d3d 3d3d 3d0a 0a2e 2e20 746f  .========.... to
+00000d10: 6374 7265 653a 3a0a 2020 203a 6d61 7864  ctree::.   :maxd
+00000d20: 6570 7468 3a20 320a 2020 203a 6361 7074  epth: 2.   :capt
+00000d30: 696f 6e3a 2043 6f6e 7465 6e74 733a 0a0a  ion: Contents:..
+00000d40: 2020 2069 6e74 726f 6475 6374 696f 6e0a     introduction.
+00000d50: 2020 2066 6561 7475 7265 730a 2020 2069     features.   i
+00000d60: 6e73 7461 6c6c 6174 696f 6e0a 2020 2061  nstallation.   a
+00000d70: 7069 5f6b 6579 0a20 2020 7573 6167 650a  pi_key.   usage.
+00000d80: 2020 2064 6f63 6b65 720a 2020 2072 6f61     docker.   roa
+00000d90: 646d 6170 0a20 2020 636f 6e74 7269 6275  dmap.   contribu
+00000da0: 7469 6e67 0a20 2020 636f 6e74 6163 740a  ting.   contact.
+00000db0: 0a49 6e74 726f 6475 6374 696f 6e0a 3d3d  .Introduction.==
+00000dc0: 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a 5079 4563  ==========..PyEc
+00000dd0: 6f6e 6f6d 6963 7320 6973 2061 2076 6572  onomics is a ver
+00000de0: 7361 7469 6c65 2061 6e64 2063 6f6d 7072  satile and compr
+00000df0: 6568 656e 7369 7665 206c 6962 7261 7279  ehensive library
+00000e00: 2074 6861 7420 696e 7465 6772 6174 6573   that integrates
+00000e10: 2076 6172 696f 7573 0a65 636f 6e6f 6d69   various.economi
+00000e20: 6320 616e 6420 6669 6e61 6e63 6961 6c20  c and financial 
+00000e30: 6d6f 6465 6c73 2e20 4974 2069 7320 6465  models. It is de
+00000e40: 7369 676e 6564 2074 6f20 7375 7070 6f72  signed to suppor
+00000e50: 7420 7468 6520 6465 7665 6c6f 706d 656e  t the developmen
+00000e60: 7420 616e 640a 616e 616c 7973 6973 206f  t and.analysis o
+00000e70: 6620 6d6f 6e65 7461 7279 2070 6f6c 6963  f monetary polic
+00000e80: 7920 7275 6c65 732c 2065 7863 6861 6e67  y rules, exchang
+00000e90: 6520 7261 7465 206d 6f64 656c 732c 206d  e rate models, m
+00000ea0: 6163 726f 6563 6f6e 6f6d 6963 2061 6e64  acroeconomic and
+00000eb0: 0a6d 6963 726f 6563 6f6e 6f6d 6963 206d  .microeconomic m
+00000ec0: 6f64 656c 732c 2064 6973 636f 756e 7465  odels, discounte
+00000ed0: 6420 6361 7368 2066 6c6f 7720 6d6f 6465  d cash flow mode
+00000ee0: 6c73 2c20 616e 6420 6d75 6368 206d 6f72  ls, and much mor
+00000ef0: 652e 0a0a 4665 6174 7572 6573 0a3d 3d3d  e...Features.===
+00000f00: 3d3d 3d3d 3d0a 0a43 7572 7265 6e74 2046  =====..Current F
+00000f10: 6561 7475 7265 730a 2d2d 2d2d 2d2d 2d2d  eatures.--------
+00000f20: 2d2d 2d2d 2d2d 2d2d 0a0a 2d20 2a2a 4d6f  --------..- **Mo
+00000f30: 6e65 7461 7279 2050 6f6c 6963 7920 5275  netary Policy Ru
+00000f40: 6c65 732a 2a3a 2049 6d70 6c65 6d65 6e74  les**: Implement
+00000f50: 6174 696f 6e20 6f66 2077 656c 6c2d 6b6e  ation of well-kn
+00000f60: 6f77 6e20 6d6f 6e65 7461 7279 2070 6f6c  own monetary pol
+00000f70: 6963 7920 7275 6c65 732e 0a2d 202a 2a43  icy rules..- **C
+00000f80: 6163 6865 204d 616e 6167 656d 656e 742a  ache Management*
+00000f90: 2a3a 2045 6666 6963 6965 6e74 2063 6163  *: Efficient cac
+00000fa0: 6869 6e67 2066 6f72 2041 5049 2063 616c  hing for API cal
+00000fb0: 6c73 2074 6f20 696d 7072 6f76 6520 7065  ls to improve pe
+00000fc0: 7266 6f72 6d61 6e63 650a 2020 616e 6420  rformance.  and 
+00000fd0: 7265 6475 6365 2072 6564 756e 6461 6e74  reduce redundant
+00000fe0: 2064 6174 6120 6665 7463 6869 6e67 2e0a   data fetching..
+00000ff0: 0a50 6c61 6e6e 6564 2046 6561 7475 7265  .Planned Feature
+00001000: 730a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  s.--------------
+00001010: 2d2d 0a0a 2d20 2a2a 4578 6368 616e 6765  --..- **Exchange
+00001020: 2052 6174 6520 4d6f 6465 6c73 2a2a 3a20   Rate Models**: 
+00001030: 4d6f 6465 6c73 2066 6f72 2070 7265 6469  Models for predi
+00001040: 6374 696e 6720 6675 7475 7265 2065 7863  cting future exc
+00001050: 6861 6e67 6520 7261 7465 732e 0a2d 202a  hange rates..- *
+00001060: 2a4d 6163 726f 6563 6f6e 6f6d 6963 204d  *Macroeconomic M
+00001070: 6f64 656c 732a 2a3a 2043 6f6d 7072 6568  odels**: Compreh
+00001080: 656e 7369 7665 206d 6163 726f 6563 6f6e  ensive macroecon
+00001090: 6f6d 6963 206d 6f64 656c 732e 0a2d 202a  omic models..- *
+000010a0: 2a4d 6963 726f 6563 6f6e 6f6d 6963 204d  *Microeconomic M
+000010b0: 6f64 656c 732a 2a3a 2044 6574 6169 6c65  odels**: Detaile
+000010c0: 6420 6d69 6372 6f65 636f 6e6f 6d69 6320  d microeconomic 
+000010d0: 6d6f 6465 6c73 2e0a 2d20 2a2a 4469 7363  models..- **Disc
+000010e0: 6f75 6e74 6564 2043 6173 6820 466c 6f77  ounted Cash Flow
+000010f0: 204d 6f64 656c 732a 2a3a 2041 6476 616e   Models**: Advan
+00001100: 6365 6420 6d6f 6465 6c73 2066 6f72 2064  ced models for d
+00001110: 6973 636f 756e 7465 6420 6361 7368 2066  iscounted cash f
+00001120: 6c6f 770a 2020 616e 616c 7973 6973 2e0a  low.  analysis..
+00001130: 2d20 2a2a 4669 6e61 6e63 6961 6c20 4d6f  - **Financial Mo
+00001140: 6465 6c73 2a2a 3a20 496e 636c 7564 696e  dels**: Includin
+00001150: 6720 4341 504d 2061 6e64 2070 6f72 7466  g CAPM and portf
+00001160: 6f6c 696f 206f 7074 696d 697a 6174 696f  olio optimizatio
+00001170: 6e2e 0a2d 202a 2a46 6973 6361 6c20 506f  n..- **Fiscal Po
+00001180: 6c69 6379 204d 6f64 656c 732a 2a3a 2054  licy Models**: T
+00001190: 6f6f 6c73 2074 6f20 616e 616c 797a 6520  ools to analyze 
+000011a0: 7461 7861 7469 6f6e 2c20 676f 7665 726e  taxation, govern
+000011b0: 6d65 6e74 2073 7065 6e64 696e 672c 2061  ment spending, a
+000011c0: 6e64 0a20 2070 7562 6c69 6320 6465 6274  nd.  public debt
+000011d0: 2e0a 2d20 2a2a 4164 6469 7469 6f6e 616c  ..- **Additional
+000011e0: 2045 636f 6e6f 6d69 6320 4d6f 6465 6c73   Economic Models
+000011f0: 2a2a 3a20 5375 7070 6f72 7420 666f 7220  **: Support for 
+00001200: 6265 6861 7669 6f72 616c 2065 636f 6e6f  behavioral econo
+00001210: 6d69 6373 2c20 6167 656e 742d 6261 7365  mics, agent-base
+00001220: 640a 2020 6d6f 6465 6c73 2c20 616e 6420  d.  models, and 
+00001230: 696e 7465 726e 6174 696f 6e61 6c20 7472  international tr
+00001240: 6164 6520 6d6f 6465 6c73 2e0a 0a49 6e73  ade models...Ins
+00001250: 7461 6c6c 6174 696f 6e0a 3d3d 3d3d 3d3d  tallation.======
+00001260: 3d3d 3d3d 3d3d 0a0a 546f 2069 6e73 7461  ======..To insta
+00001270: 6c6c 2050 7945 636f 6e6f 6d69 6373 2c20  ll PyEconomics, 
+00001280: 7573 6520 6060 7069 7060 603a 0a0a 2e2e  use ``pip``:....
+00001290: 2063 6f64 652d 626c 6f63 6b3a 3a20 7368   code-block:: sh
+000012a0: 0a0a 2020 2070 6970 2069 6e73 7461 6c6c  ..   pip install
+000012b0: 2070 7965 636f 6e6f 6d69 6373 0a0a 4672   pyeconomics..Fr
+000012c0: 6f6d 2053 6f75 7263 650a 2d2d 2d2d 2d2d  om Source.------
+000012d0: 2d2d 2d2d 2d0a 0a49 6620 796f 7520 7761  -----..If you wa
+000012e0: 6e74 2074 6f20 696e 7374 616c 6c20 7468  nt to install th
+000012f0: 6520 7061 636b 6167 6520 6672 6f6d 2074  e package from t
+00001300: 6865 2073 6f75 7263 6520 636f 6465 2c20  he source code, 
+00001310: 666f 6c6c 6f77 2074 6865 7365 2073 7465  follow these ste
+00001320: 7073 3a0a 0a31 2e20 436c 6f6e 6520 7468  ps:..1. Clone th
+00001330: 6520 7265 706f 7369 746f 7279 3a0a 0a20  e repository:.. 
+00001340: 2020 202e 2e20 636f 6465 2d62 6c6f 636b     .. code-block
+00001350: 3a3a 2073 680a 0a20 2020 2020 2020 6769  :: sh..       gi
+00001360: 7420 636c 6f6e 6520 6874 7470 733a 2f2f  t clone https://
+00001370: 6769 7468 7562 2e63 6f6d 2f6e 6174 6861  github.com/natha
+00001380: 6e72 616d 6f73 6366 612f 7079 6563 6f6e  nramoscfa/pyecon
+00001390: 6f6d 6963 732e 6769 740a 0a32 2e20 4368  omics.git..2. Ch
+000013a0: 616e 6765 2074 6f20 7468 6520 7072 6f6a  ange to the proj
+000013b0: 6563 7420 6469 7265 6374 6f72 793a 0a0a  ect directory:..
+000013c0: 2020 2020 2e2e 2063 6f64 652d 626c 6f63      .. code-bloc
+000013d0: 6b3a 3a20 7368 0a0a 2020 2020 2020 2063  k:: sh..       c
+000013e0: 6420 7079 6563 6f6e 6f6d 6963 730a 0a33  d pyeconomics..3
+000013f0: 2e20 496e 7374 616c 6c20 7468 6520 7061  . Install the pa
+00001400: 636b 6167 653a 0a0a 2020 2020 2e2e 2063  ckage:..    .. c
+00001410: 6f64 652d 626c 6f63 6b3a 3a20 7368 0a0a  ode-block:: sh..
+00001420: 2020 2020 2020 2070 6970 2069 6e73 7461         pip insta
+00001430: 6c6c 202e 0a0a 4150 4920 4b65 790a 3d3d  ll ...API Key.==
+00001440: 3d3d 3d3d 3d0a 0a53 6f6d 6520 6665 6174  =====..Some feat
+00001450: 7572 6573 206f 6620 5079 4563 6f6e 6f6d  ures of PyEconom
+00001460: 6963 7320 7265 7175 6972 6520 6163 6365  ics require acce
+00001470: 7373 2074 6f20 7468 6520 4652 4544 2041  ss to the FRED A
+00001480: 5049 2e20 546f 2075 7365 2074 6865 7365  PI. To use these
+00001490: 0a66 6561 7475 7265 732c 2079 6f75 206e  .features, you n
+000014a0: 6565 6420 746f 2063 6f6e 6669 6775 7265  eed to configure
+000014b0: 2079 6f75 7220 4652 4544 2041 5049 2061   your FRED API a
+000014c0: 6363 6573 732e 0a0a 4120 6465 7461 696c  ccess...A detail
+000014d0: 6564 2073 7465 702d 6279 2d73 7465 7020  ed step-by-step 
+000014e0: 6775 6964 6520 6f6e 206f 6274 6169 6e69  guide on obtaini
+000014f0: 6e67 2061 6e64 2073 6563 7572 656c 7920  ng and securely 
+00001500: 7374 6f72 696e 6720 796f 7572 2046 5245  storing your FRE
+00001510: 4420 4150 490a 6b65 7920 6973 2061 7661  D API.key is ava
+00001520: 696c 6162 6c65 2068 6572 653a 0a0a 2d20  ilable here:..- 
+00001530: 6046 5245 4420 4150 4920 4b65 7920 436f  `FRED API Key Co
+00001540: 6e66 6967 7572 6174 696f 6e20 4775 6964  nfiguration Guid
+00001550: 6520 284d 6172 6b64 6f77 6e29 203c 6d61  e (Markdown) <ma
+00001560: 726b 646f 776e 2f46 5245 445f 4150 495f  rkdown/FRED_API_
+00001570: 434f 4e46 4947 5552 4154 494f 4e2e 6d64  CONFIGURATION.md
+00001580: 3e60 5f0a 2d20 6046 5245 4420 4150 4920  >`_.- `FRED API 
+00001590: 4b65 7920 436f 6e66 6967 7572 6174 696f  Key Configuratio
+000015a0: 6e20 4775 6964 6520 284a 7570 7974 6572  n Guide (Jupyter
+000015b0: 204e 6f74 6562 6f6f 6b29 203c 6578 616d   Notebook) <exam
+000015c0: 706c 6573 2f61 7069 5f63 6f6e 6669 6775  ples/api_configu
+000015d0: 7261 7469 6f6e 2f66 7265 645f 6170 695f  ration/fred_api_
+000015e0: 636f 6e66 6967 7572 6174 696f 6e2e 6970  configuration.ip
+000015f0: 796e 623e 605f 0a0a 5573 6167 650a 3d3d  ynb>`_..Usage.==
+00001600: 3d3d 3d0a 0a48 6572 6520 6172 6520 736f  ===..Here are so
+00001610: 6d65 2062 6173 6963 2065 7861 6d70 6c65  me basic example
+00001620: 7320 6f66 2068 6f77 2074 6f20 7573 6520  s of how to use 
+00001630: 5079 4563 6f6e 6f6d 6963 7320 666f 7220  PyEconomics for 
+00001640: 6361 6c63 756c 6174 696e 6720 616e 6420  calculating and 
+00001650: 7669 7375 616c 697a 696e 6720 6d6f 6e65  visualizing mone
+00001660: 7461 7279 2070 6f6c 6963 7920 7275 6c65  tary policy rule
+00001670: 732e 0a0a 4578 616d 706c 6520 313a 2043  s...Example 1: C
+00001680: 616c 6375 6c61 7465 2043 7572 7265 6e74  alculate Current
+00001690: 2050 6f6c 6963 7920 5275 6c65 2045 7374   Policy Rule Est
+000016a0: 696d 6174 6573 0a2d 2d2d 2d2d 2d2d 2d2d  imates.---------
+000016b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000016c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000016d0: 2d2d 2d2d 2d2d 2d2d 2d0a 0a2e 2e20 636f  ---------.... co
+000016e0: 6465 2d62 6c6f 636b 3a3a 2070 7974 686f  de-block:: pytho
+000016f0: 6e0a 0a20 2020 2320 496d 706f 7274 2070  n..   # Import p
+00001700: 7965 636f 6e6f 6d69 6373 0a20 2020 696d  yeconomics.   im
+00001710: 706f 7274 2070 7965 636f 6e6f 6d69 6373  port pyeconomics
+00001720: 2061 7320 7079 6563 6f6e 0a0a 2020 2023   as pyecon..   #
+00001730: 2043 616c 6375 6c61 7465 2070 6f6c 6963   Calculate polic
+00001740: 7920 7275 6c65 2065 7374 696d 6174 6573  y rule estimates
+00001750: 0a20 2020 706f 6c69 6379 5f65 7374 696d  .   policy_estim
+00001760: 6174 6573 203d 2070 7965 636f 6e2e 6361  ates = pyecon.ca
+00001770: 6c63 756c 6174 655f 706f 6c69 6379 5f72  lculate_policy_r
+00001780: 756c 655f 6573 7469 6d61 7465 7328 7665  ule_estimates(ve
+00001790: 7262 6f73 653d 5472 7565 290a 0a56 6572  rbose=True)..Ver
+000017a0: 626f 7365 2050 7269 6e74 2053 7461 7465  bose Print State
+000017b0: 6d65 6e74 3a0a 0a2e 2e20 636f 6465 2d62  ment:.... code-b
+000017c0: 6c6f 636b 3a3a 206e 6f6e 650a 0a20 2020  lock:: none..   
+000017d0: e294 8ce2 9480 e294 80e2 9480 e294 80e2  ................
+000017e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000017f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001800: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001810: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001820: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001830: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001840: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001850: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001860: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001870: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001880: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001890: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000018a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000018b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000018c0: e294 80e2 9480 e294 80e2 9480 e294 900a  ................
+000018d0: 2020 20e2 9482 2020 2020 2020 2020 2020     ...          
 000018e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018f0: 2020 2020 2020 2020 352e 3636 2520 2020          5.66%   
-00001900: 2020 2020 e294 820a 2020 20e2 9482 2046      ....   ... F
-00001910: 6972 7374 2044 6966 6665 7265 6e63 6520  irst Difference 
-00001920: 5275 6c65 2028 4644 5229 2020 2020 2020  Rule (FDR)      
-00001930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001950: 2020 2020 2035 2e39 3725 2020 2020 2020       5.97%      
-00001960: 20e2 9482 0a20 2020 e294 9ce2 9480 e294   ....   ........
-00001970: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001980: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001990: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000019a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000019b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000019c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000019d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000019e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000019f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001a00: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001a10: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001a20: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001a30: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001a40: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001a50: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001a60: 80e2 9480 e294 a40a 2020 20e2 9482 2046  ........   ... F
-00001a70: 6564 6572 616c 2046 756e 6473 2052 6174  ederal Funds Rat
-00001a80: 6520 2846 4652 2920 2020 2020 2020 2020  e (FFR)         
-00001a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ab0: 2020 2020 2035 2e35 3025 2020 2020 2020       5.50%      
-00001ac0: 20e2 9482 0a20 2020 e294 9ce2 9480 e294   ....   ........
-00001ad0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001ae0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001af0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001b00: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001b10: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001b20: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001b30: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001b40: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001b50: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001b60: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001b70: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001b80: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001b90: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001ba0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001bb0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001bc0: 80e2 9480 e294 a40a 2020 20e2 9482 2041  ........   ... A
-00001bd0: 7320 6f66 2044 6174 6520 2020 2020 2020  s of Date       
-00001be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c00: 2020 2020 2020 2020 2020 2020 2020 4d61                Ma
-00001c10: 7920 3230 2c20 3230 3234 2020 2020 2020  y 20, 2024      
-00001c20: 20e2 9482 0a20 2020 e294 9ce2 9480 e294   ....   ........
+000018f0: 2049 6e74 6572 6573 7420 5261 7465 2050   Interest Rate P
+00001900: 6f6c 6963 7920 4573 7469 6d61 7465 7320  olicy Estimates 
+00001910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001920: 2020 2020 2020 2020 20e2 9482 0a20 2020           ....   
+00001930: e294 9ce2 9480 e294 80e2 9480 e294 80e2  ................
+00001940: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001950: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001960: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001970: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001980: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001990: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000019a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000019b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000019c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000019d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000019e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000019f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001a00: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001a10: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001a20: e294 80e2 9480 e294 80e2 9480 e294 a40a  ................
+00001a30: 2020 20e2 9482 2054 6179 6c6f 7220 5275     ... Taylor Ru
+00001a40: 6c65 2028 5452 2920 2020 2020 2020 2020  le (TR)         
+00001a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a70: 2020 2020 2020 2020 2020 2020 2036 2e31               6.1
+00001a80: 3725 2020 2020 2020 20e2 9482 0a20 2020  7%       ....   
+00001a90: e294 8220 4261 6c61 6e63 6564 2041 7070  ... Balanced App
+00001aa0: 726f 6163 6820 5275 6c65 2028 4241 5229  roach Rule (BAR)
+00001ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ad0: 2020 2020 2020 2020 2020 362e 3638 2520            6.68% 
+00001ae0: 2020 2020 2020 e294 820a 2020 20e2 9482        ....   ...
+00001af0: 2042 616c 616e 6365 6420 4170 7072 6f61   Balanced Approa
+00001b00: 6368 2053 686f 7274 6661 6c6c 7320 5275  ch Shortfalls Ru
+00001b10: 6c65 2028 4241 5352 2920 2020 2020 2020  le (BASR)       
+00001b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b30: 2020 2020 2020 2035 2e36 3625 2020 2020         5.66%    
+00001b40: 2020 20e2 9482 0a20 2020 e294 8220 4669     ....   ... Fi
+00001b50: 7273 7420 4469 6666 6572 656e 6365 2052  rst Difference R
+00001b60: 756c 6520 2846 4452 2920 2020 2020 2020  ule (FDR)       
+00001b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b90: 2020 2020 352e 3937 2520 2020 2020 2020      5.97%       
+00001ba0: e294 820a 2020 20e2 949c e294 80e2 9480  ....   .........
+00001bb0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001bc0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001bd0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001be0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001bf0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001c00: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001c10: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001c20: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00001c30: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00001c40: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00001c50: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00001c60: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00001c70: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00001c80: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00001c90: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001ca0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001cb0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001cc0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001cd0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001ce0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001cf0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001d00: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001d10: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001d20: 80e2 9480 e294 a40a 2020 20e2 9482 2020  ........   ...  
-00001d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d40: 2020 2020 2020 2020 2020 2020 2020 506f                Po
-00001d50: 6c69 6379 2050 7265 7363 7269 7074 696f  licy Prescriptio
-00001d60: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-00001d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d80: 20e2 9482 0a20 2020 e294 9ce2 9480 e294   ....   ........
+00001ca0: e294 80e2 94a4 0a20 2020 e294 8220 4665  .......   ... Fe
+00001cb0: 6465 7261 6c20 4675 6e64 7320 5261 7465  deral Funds Rate
+00001cc0: 2028 4646 5229 2020 2020 2020 2020 2020   (FFR)          
+00001cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001cf0: 2020 2020 352e 3530 2520 2020 2020 2020      5.50%       
+00001d00: e294 820a 2020 20e2 949c e294 80e2 9480  ....   .........
+00001d10: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001d20: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001d30: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001d40: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001d50: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001d60: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001d70: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001d80: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00001d90: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00001da0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00001db0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00001dc0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00001dd0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00001de0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00001df0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001e00: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001e10: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001e20: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001e30: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001e40: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001e50: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001e60: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001e70: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001e80: 80e2 9480 e294 a40a 2020 20e2 9482 2054  ........   ... T
-00001e90: 6179 6c6f 7220 5275 6c65 2028 5452 2920  aylor Rule (TR) 
-00001ea0: 7375 6767 6573 7473 2072 6169 7369 6e67  suggests raising
-00001eb0: 2074 6865 2072 6174 6520 6279 2030 2e37   the rate by 0.7
-00001ec0: 3525 2e20 2020 2020 2020 2020 2020 2020  5%.             
-00001ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ee0: 20e2 9482 0a20 2020 e294 8220 4261 6c61   ....   ... Bala
-00001ef0: 6e63 6564 2041 7070 726f 6163 6820 5275  nced Approach Ru
-00001f00: 6c65 2028 4241 5229 2073 7567 6765 7374  le (BAR) suggest
-00001f10: 7320 7261 6973 696e 6720 7468 6520 7261  s raising the ra
-00001f20: 7465 2062 7920 312e 3235 252e 2020 2020  te by 1.25%.    
-00001f30: 2020 2020 2020 2020 2020 2020 2020 e294                ..
-00001f40: 820a 2020 20e2 9482 2042 616c 616e 6365  ..   ... Balance
-00001f50: 6420 4170 7072 6f61 6368 2053 686f 7274  d Approach Short
-00001f60: 6661 6c6c 7320 5275 6c65 2028 4241 5352  falls Rule (BASR
-00001f70: 2920 7375 6767 6573 7473 2072 6169 7369  ) suggests raisi
-00001f80: 6e67 2074 6865 2072 6174 6520 6279 2030  ng the rate by 0
-00001f90: 2e32 3525 2e20 2020 2020 20e2 9482 0a20  .25%.      .... 
-00001fa0: 2020 e294 8220 4669 7273 7420 4469 6666    ... First Diff
-00001fb0: 6572 656e 6365 2052 756c 6520 2846 4452  erence Rule (FDR
-00001fc0: 2920 7375 6767 6573 7473 2072 6169 7369  ) suggests raisi
-00001fd0: 6e67 2074 6865 2072 6174 6520 6279 2030  ng the rate by 0
-00001fe0: 2e35 3025 2e20 2020 2020 2020 2020 2020  .50%.           
-00001ff0: 2020 2020 2020 2020 e294 820a 2020 20e2          ....   .
-00002000: 9494 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002010: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002020: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002030: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002040: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002050: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002060: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002070: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002080: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002090: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000020a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000020b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000020c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000020d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000020e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000020f0: 9480 e294 80e2 9480 e294 80e2 9498 0a0a  ................
-00002100: 4578 616d 706c 6520 323a 2041 646a 7573  Example 2: Adjus
-00002110: 7420 5461 796c 6f72 2052 756c 6520 666f  t Taylor Rule fo
-00002120: 7220 4566 6665 6374 6976 6520 4c6f 7765  r Effective Lowe
-00002130: 7220 426f 756e 6420 2845 4c42 2920 616e  r Bound (ELB) an
-00002140: 6420 506f 6c69 6379 2049 6e65 7274 6961  d Policy Inertia
-00002150: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .---------------
-00002160: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002170: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002180: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002190: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000021a0: 2d0a 0a2e 2e20 636f 6465 2d62 6c6f 636b  -.... code-block
-000021b0: 3a3a 2070 7974 686f 6e0a 0a20 2020 2320  :: python..   # 
-000021c0: 496d 706f 7274 2070 7965 636f 6e6f 6d69  Import pyeconomi
-000021d0: 6373 0a20 2020 696d 706f 7274 2070 7965  cs.   import pye
-000021e0: 636f 6e6f 6d69 6373 2061 7320 7079 6563  conomics as pyec
-000021f0: 6f6e 0a0a 2020 2023 2041 646a 7573 746d  on..   # Adjustm
-00002200: 656e 7420 5061 7261 6d65 7465 7273 0a20  ent Parameters. 
-00002210: 2020 7268 6f20 3d20 302e 3720 2023 2050    rho = 0.7  # P
-00002220: 6f6c 6963 7920 496e 6572 7469 6120 436f  olicy Inertia Co
-00002230: 6566 6669 6369 656e 740a 2020 2061 7070  efficient.   app
-00002240: 6c79 5f65 6c62 203d 2054 7275 6520 2023  ly_elb = True  #
-00002250: 2041 7070 6c79 2045 6666 6563 7469 7665   Apply Effective
-00002260: 204c 6f77 6572 2042 6f75 6e64 0a0a 2020   Lower Bound..  
-00002270: 2061 646a 7573 7465 645f 706f 6c69 6379   adjusted_policy
-00002280: 5f65 7374 696d 6174 6573 203d 2070 7965  _estimates = pye
-00002290: 636f 6e2e 6361 6c63 756c 6174 655f 706f  con.calculate_po
-000022a0: 6c69 6379 5f72 756c 655f 6573 7469 6d61  licy_rule_estima
-000022b0: 7465 7328 0a20 2020 2020 2020 7268 6f3d  tes(.       rho=
-000022c0: 7268 6f2c 0a20 2020 2020 2020 6170 706c  rho,.       appl
-000022d0: 795f 656c 623d 6170 706c 795f 656c 622c  y_elb=apply_elb,
-000022e0: 0a20 2020 2020 2020 7665 7262 6f73 653d  .       verbose=
-000022f0: 5472 7565 0a20 2020 290a 0a56 6572 626f  True.   )..Verbo
-00002300: 7365 2050 7269 6e74 2053 7461 7465 6d65  se Print Stateme
-00002310: 6e74 3a0a 0a2e 2e20 636f 6465 2d62 6c6f  nt:.... code-blo
-00002320: 636b 3a3a 206e 6f6e 650a 0a20 2020 e294  ck:: none..   ..
-00002330: 8ce2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002340: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002350: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002360: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002370: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002380: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002390: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000023a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000023b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000023c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000023d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000023e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000023f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002400: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002410: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002420: 80e2 9480 e294 80e2 9480 e294 900a 2020  ..............  
-00002430: 20e2 9482 2020 2020 2020 2020 2020 2020   ...            
-00002440: 2020 2020 2020 2020 2020 4164 6a75 7374            Adjust
-00002450: 6564 2049 6e74 6572 6573 7420 5261 7465  ed Interest Rate
-00002460: 2050 6f6c 6963 7920 4573 7469 6d61 7465   Policy Estimate
-00002470: 7320 2020 2020 2020 2020 2020 2020 2020  s               
-00002480: 2020 2020 2020 20e2 9482 0a20 2020 e294         ....   ..
-00002490: 9ce2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000024a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000024b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000024c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000024d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000024e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000024f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002500: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002510: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002520: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002530: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002540: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002550: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002560: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002570: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002580: 80e2 9480 e294 80e2 9480 e294 a40a 2020  ..............  
-00002590: 20e2 9482 2054 6179 6c6f 7220 5275 6c65   ... Taylor Rule
-000025a0: 2028 5452 2920 2020 2020 2020 2020 2020   (TR)           
-000025b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025d0: 2020 2020 2020 2020 2020 2035 2e37 3025             5.70%
-000025e0: 2020 2020 2020 20e2 9482 0a20 2020 e294         ....   ..
-000025f0: 8220 4261 6c61 6e63 6564 2041 7070 726f  . Balanced Appro
-00002600: 6163 6820 5275 6c65 2028 4241 5229 2020  ach Rule (BAR)  
-00002610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002630: 2020 2020 2020 2020 352e 3836 2520 2020          5.86%   
-00002640: 2020 2020 e294 820a 2020 20e2 9482 2042      ....   ... B
-00002650: 616c 616e 6365 6420 4170 7072 6f61 6368  alanced Approach
-00002660: 2053 686f 7274 6661 6c6c 7320 5275 6c65   Shortfalls Rule
-00002670: 2028 4241 5352 2920 2020 2020 2020 2020   (BASR)         
-00002680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002690: 2020 2020 2035 2e35 3525 2020 2020 2020       5.55%      
-000026a0: 20e2 9482 0a20 2020 e294 8220 4669 7273   ....   ... Firs
-000026b0: 7420 4469 6666 6572 656e 6365 2052 756c  t Difference Rul
-000026c0: 6520 2846 4452 2920 2020 2020 2020 2020  e (FDR)         
-000026d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026f0: 2020 352e 3634 2520 2020 2020 2020 e294    5.64%       ..
-00002700: 820a 2020 20e2 949c e294 80e2 9480 e294  ..   ...........
-00002710: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002720: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002730: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002740: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002750: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002760: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002770: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002780: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002790: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000027a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000027b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000027c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000027d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000027e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000027f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002800: 80e2 94a4 0a20 2020 e294 8220 4665 6465  .....   ... Fede
-00002810: 7261 6c20 4675 6e64 7320 5261 7465 2028  ral Funds Rate (
-00002820: 4646 5229 2020 2020 2020 2020 2020 2020  FFR)            
-00002830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002850: 2020 352e 3530 2520 2020 2020 2020 e294    5.50%       ..
-00002860: 820a 2020 20e2 949c e294 80e2 9480 e294  ..   ...........
-00002870: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002880: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002890: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000028a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000028b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000028c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000028d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000028e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000028f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002900: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002910: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002920: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002930: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002940: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002950: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002960: 80e2 94a4 0a20 2020 e294 8220 4173 206f  .....   ... As o
-00002970: 6620 4461 7465 2020 2020 2020 2020 2020  f Date          
-00002980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029a0: 2020 2020 2020 2020 2020 204d 6179 2032             May 2
-000029b0: 312c 2032 3032 3420 2020 2020 2020 e294  1, 2024       ..
-000029c0: 820a 2020 20e2 949c e294 80e2 9480 e294  ..   ...........
+00001e00: e294 80e2 94a4 0a20 2020 e294 8220 4173  .......   ... As
+00001e10: 206f 6620 4461 7465 2020 2020 2020 2020   of Date        
+00001e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e40: 2020 2020 2020 2020 2020 2020 204d 6179               May
+00001e50: 2032 302c 2032 3032 3420 2020 2020 2020   20, 2024       
+00001e60: e294 820a 2020 20e2 949c e294 80e2 9480  ....   .........
+00001e70: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001e80: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001e90: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001ea0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001eb0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001ec0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001ed0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001ee0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001ef0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001f00: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001f10: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001f20: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001f30: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001f40: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001f50: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001f60: e294 80e2 94a4 0a20 2020 e294 8220 2020  .......   ...   
+00001f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f80: 2020 2020 2020 2020 2020 2020 2050 6f6c               Pol
+00001f90: 6963 7920 5072 6573 6372 6970 7469 6f6e  icy Prescription
+00001fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001fc0: e294 820a 2020 20e2 949c e294 80e2 9480  ....   .........
+00001fd0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001fe0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001ff0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002000: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002010: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002020: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002030: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002040: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002050: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002060: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002070: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002080: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002090: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000020a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000020b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000020c0: e294 80e2 94a4 0a20 2020 e294 8220 5461  .......   ... Ta
+000020d0: 796c 6f72 2052 756c 6520 2854 5229 2073  ylor Rule (TR) s
+000020e0: 7567 6765 7374 7320 7261 6973 696e 6720  uggests raising 
+000020f0: 7468 6520 7261 7465 2062 7920 302e 3735  the rate by 0.75
+00002100: 252e 2020 2020 2020 2020 2020 2020 2020  %.              
+00002110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002120: e294 820a 2020 20e2 9482 2042 616c 616e  ....   ... Balan
+00002130: 6365 6420 4170 7072 6f61 6368 2052 756c  ced Approach Rul
+00002140: 6520 2842 4152 2920 7375 6767 6573 7473  e (BAR) suggests
+00002150: 2072 6169 7369 6e67 2074 6865 2072 6174   raising the rat
+00002160: 6520 6279 2031 2e32 3525 2e20 2020 2020  e by 1.25%.     
+00002170: 2020 2020 2020 2020 2020 2020 20e2 9482               ...
+00002180: 0a20 2020 e294 8220 4261 6c61 6e63 6564  .   ... Balanced
+00002190: 2041 7070 726f 6163 6820 5368 6f72 7466   Approach Shortf
+000021a0: 616c 6c73 2052 756c 6520 2842 4153 5229  alls Rule (BASR)
+000021b0: 2073 7567 6765 7374 7320 7261 6973 696e   suggests raisin
+000021c0: 6720 7468 6520 7261 7465 2062 7920 302e  g the rate by 0.
+000021d0: 3235 252e 2020 2020 2020 e294 820a 2020  25%.      ....  
+000021e0: 20e2 9482 2046 6972 7374 2044 6966 6665   ... First Diffe
+000021f0: 7265 6e63 6520 5275 6c65 2028 4644 5229  rence Rule (FDR)
+00002200: 2073 7567 6765 7374 7320 7261 6973 696e   suggests raisin
+00002210: 6720 7468 6520 7261 7465 2062 7920 302e  g the rate by 0.
+00002220: 3530 252e 2020 2020 2020 2020 2020 2020  50%.            
+00002230: 2020 2020 2020 20e2 9482 0a20 2020 e294         ....   ..
+00002240: 94e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002250: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002260: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002270: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002280: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002290: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000022a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000022b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000022c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000022d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000022e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000022f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002300: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002310: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002320: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002330: 80e2 9480 e294 80e2 9480 e294 980a 0a45  ...............E
+00002340: 7861 6d70 6c65 2032 3a20 4164 6a75 7374  xample 2: Adjust
+00002350: 2054 6179 6c6f 7220 5275 6c65 2066 6f72   Taylor Rule for
+00002360: 2045 6666 6563 7469 7665 204c 6f77 6572   Effective Lower
+00002370: 2042 6f75 6e64 2028 454c 4229 2061 6e64   Bound (ELB) and
+00002380: 2050 6f6c 6963 7920 496e 6572 7469 610a   Policy Inertia.
+00002390: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000023a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000023b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000023c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000023d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000023e0: 0a0a 2e2e 2063 6f64 652d 626c 6f63 6b3a  .... code-block:
+000023f0: 3a20 7079 7468 6f6e 0a0a 2020 2023 2049  : python..   # I
+00002400: 6d70 6f72 7420 7079 6563 6f6e 6f6d 6963  mport pyeconomic
+00002410: 730a 2020 2069 6d70 6f72 7420 7079 6563  s.   import pyec
+00002420: 6f6e 6f6d 6963 7320 6173 2070 7965 636f  onomics as pyeco
+00002430: 6e0a 0a20 2020 2320 4164 6a75 7374 6d65  n..   # Adjustme
+00002440: 6e74 2050 6172 616d 6574 6572 730a 2020  nt Parameters.  
+00002450: 2072 686f 203d 2030 2e37 2020 2320 506f   rho = 0.7  # Po
+00002460: 6c69 6379 2049 6e65 7274 6961 2043 6f65  licy Inertia Coe
+00002470: 6666 6963 6965 6e74 0a20 2020 6170 706c  fficient.   appl
+00002480: 795f 656c 6220 3d20 5472 7565 2020 2320  y_elb = True  # 
+00002490: 4170 706c 7920 4566 6665 6374 6976 6520  Apply Effective 
+000024a0: 4c6f 7765 7220 426f 756e 640a 0a20 2020  Lower Bound..   
+000024b0: 6164 6a75 7374 6564 5f70 6f6c 6963 795f  adjusted_policy_
+000024c0: 6573 7469 6d61 7465 7320 3d20 7079 6563  estimates = pyec
+000024d0: 6f6e 2e63 616c 6375 6c61 7465 5f70 6f6c  on.calculate_pol
+000024e0: 6963 795f 7275 6c65 5f65 7374 696d 6174  icy_rule_estimat
+000024f0: 6573 280a 2020 2020 2020 2072 686f 3d72  es(.       rho=r
+00002500: 686f 2c0a 2020 2020 2020 2061 7070 6c79  ho,.       apply
+00002510: 5f65 6c62 3d61 7070 6c79 5f65 6c62 2c0a  _elb=apply_elb,.
+00002520: 2020 2020 2020 2076 6572 626f 7365 3d54         verbose=T
+00002530: 7275 650a 2020 2029 0a0a 5665 7262 6f73  rue.   )..Verbos
+00002540: 6520 5072 696e 7420 5374 6174 656d 656e  e Print Statemen
+00002550: 743a 0a0a 2e2e 2063 6f64 652d 626c 6f63  t:.... code-bloc
+00002560: 6b3a 3a20 6e6f 6e65 0a0a 2020 20e2 948c  k:: none..   ...
+00002570: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002580: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002590: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000025a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000025b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000025c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000025d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000025e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000025f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002600: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002610: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002620: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002630: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002640: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002650: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002660: e294 80e2 9480 e294 80e2 9490 0a20 2020  .............   
+00002670: e294 8220 2020 2020 2020 2020 2020 2020  ...             
+00002680: 2020 2020 2020 2020 2041 646a 7573 7465           Adjuste
+00002690: 6420 496e 7465 7265 7374 2052 6174 6520  d Interest Rate 
+000026a0: 506f 6c69 6379 2045 7374 696d 6174 6573  Policy Estimates
+000026b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000026c0: 2020 2020 2020 e294 820a 2020 20e2 949c        ....   ...
+000026d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000026e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000026f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002700: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002710: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002720: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002730: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002740: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002750: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002760: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002770: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002780: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002790: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000027a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000027b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000027c0: e294 80e2 9480 e294 80e2 94a4 0a20 2020  .............   
+000027d0: e294 8220 5461 796c 6f72 2052 756c 6520  ... Taylor Rule 
+000027e0: 2854 5229 2020 2020 2020 2020 2020 2020  (TR)            
+000027f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002810: 2020 2020 2020 2020 2020 352e 3730 2520            5.70% 
+00002820: 2020 2020 2020 e294 820a 2020 20e2 9482        ....   ...
+00002830: 2042 616c 616e 6365 6420 4170 7072 6f61   Balanced Approa
+00002840: 6368 2052 756c 6520 2842 4152 2920 2020  ch Rule (BAR)   
+00002850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002870: 2020 2020 2020 2035 2e38 3625 2020 2020         5.86%    
+00002880: 2020 20e2 9482 0a20 2020 e294 8220 4261     ....   ... Ba
+00002890: 6c61 6e63 6564 2041 7070 726f 6163 6820  lanced Approach 
+000028a0: 5368 6f72 7466 616c 6c73 2052 756c 6520  Shortfalls Rule 
+000028b0: 2842 4153 5229 2020 2020 2020 2020 2020  (BASR)          
+000028c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028d0: 2020 2020 352e 3535 2520 2020 2020 2020      5.55%       
+000028e0: e294 820a 2020 20e2 9482 2046 6972 7374  ....   ... First
+000028f0: 2044 6966 6665 7265 6e63 6520 5275 6c65   Difference Rule
+00002900: 2028 4644 5229 2020 2020 2020 2020 2020   (FDR)          
+00002910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002930: 2035 2e36 3425 2020 2020 2020 20e2 9482   5.64%       ...
+00002940: 0a20 2020 e294 9ce2 9480 e294 80e2 9480  .   ............
+00002950: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002960: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002970: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002980: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002990: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000029a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000029b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000029c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 000029d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 000029e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 000029f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00002a00: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00002a10: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00002a20: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00002a30: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002a40: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002a50: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002a60: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002a70: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002a80: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002a90: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002aa0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002ab0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002ac0: 80e2 94a4 0a20 2020 e294 8220 2020 2020  .....   ...     
-00002ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ae0: 2020 2020 2020 2041 646a 7573 7465 6420         Adjusted 
-00002af0: 506f 6c69 6379 2050 7265 7363 7269 7074  Policy Prescript
-00002b00: 696f 6e20 2020 2020 2020 2020 2020 2020  ion             
-00002b10: 2020 2020 2020 2020 2020 2020 2020 e294                ..
-00002b20: 820a 2020 20e2 949c e294 80e2 9480 e294  ..   ...........
+00002a40: e294 a40a 2020 20e2 9482 2046 6564 6572  ....   ... Feder
+00002a50: 616c 2046 756e 6473 2052 6174 6520 2846  al Funds Rate (F
+00002a60: 4652 2920 2020 2020 2020 2020 2020 2020  FR)             
+00002a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a90: 2035 2e35 3025 2020 2020 2020 20e2 9482   5.50%       ...
+00002aa0: 0a20 2020 e294 9ce2 9480 e294 80e2 9480  .   ............
+00002ab0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002ac0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002ad0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002ae0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002af0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002b00: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002b10: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002b20: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00002b30: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00002b40: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00002b50: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00002b60: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00002b70: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00002b80: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00002b90: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002ba0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002bb0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002bc0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002bd0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002be0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002bf0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002c00: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002c10: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002c20: 80e2 94a4 0a20 2020 e294 8220 5461 796c  .....   ... Tayl
-00002c30: 6f72 2052 756c 6520 2854 5229 2073 7567  or Rule (TR) sug
-00002c40: 6765 7374 7320 7261 6973 696e 6720 7468  gests raising th
-00002c50: 6520 7261 7465 2062 7920 302e 3235 252e  e rate by 0.25%.
-00002c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c70: 2020 2020 2020 2020 2020 2020 2020 e294                ..
-00002c80: 820a 2020 20e2 9482 2042 616c 616e 6365  ..   ... Balance
-00002c90: 6420 4170 7072 6f61 6368 2052 756c 6520  d Approach Rule 
-00002ca0: 2842 4152 2920 7375 6767 6573 7473 2072  (BAR) suggests r
-00002cb0: 6169 7369 6e67 2074 6865 2072 6174 6520  aising the rate 
-00002cc0: 6279 2030 2e32 3525 2e20 2020 2020 2020  by 0.25%.       
-00002cd0: 2020 2020 2020 2020 2020 20e2 9482 0a20             .... 
-00002ce0: 2020 e294 8220 4261 6c61 6e63 6564 2041    ... Balanced A
-00002cf0: 7070 726f 6163 6820 5368 6f72 7466 616c  pproach Shortfal
-00002d00: 6c73 2052 756c 6520 2842 4153 5229 2073  ls Rule (BASR) s
-00002d10: 7567 6765 7374 7320 6d61 696e 7461 696e  uggests maintain
-00002d20: 696e 6720 7468 6520 6375 7272 656e 7420  ing the current 
-00002d30: 7261 7465 2e20 2020 e294 820a 2020 20e2  rate.   ....   .
-00002d40: 9482 2046 6972 7374 2044 6966 6665 7265  .. First Differe
-00002d50: 6e63 6520 5275 6c65 2028 4644 5229 2073  nce Rule (FDR) s
-00002d60: 7567 6765 7374 7320 7261 6973 696e 6720  uggests raising 
-00002d70: 7468 6520 7261 7465 2062 7920 302e 3235  the rate by 0.25
-00002d80: 252e 2020 2020 2020 2020 2020 2020 2020  %.              
-00002d90: 2020 2020 20e2 9482 0a20 2020 e294 94e2       ....   ....
-00002da0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002db0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002dc0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002dd0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002de0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002df0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002e00: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002e10: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002e20: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002e30: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002e40: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002e50: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002e60: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002e70: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002e80: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002e90: 9480 e294 80e2 9480 e294 980a 0a45 7861  .............Exa
-00002ea0: 6d70 6c65 2033 3a20 4361 6c63 756c 6174  mple 3: Calculat
-00002eb0: 6520 4375 7272 656e 7420 5461 796c 6f72  e Current Taylor
-00002ec0: 2052 756c 6520 4573 7469 6d61 7465 730a   Rule Estimates.
-00002ed0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002ee0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002ef0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002f00: 2d2d 0a0a 2e2e 2063 6f64 652d 626c 6f63  --.... code-bloc
-00002f10: 6b3a 3a20 7079 7468 6f6e 0a0a 2020 2023  k:: python..   #
-00002f20: 2049 6d70 6f72 7420 7079 6563 6f6e 6f6d   Import pyeconom
-00002f30: 6963 7320 6d6f 6475 6c65 730a 2020 2069  ics modules.   i
-00002f40: 6d70 6f72 7420 7079 6563 6f6e 6f6d 6963  mport pyeconomic
-00002f50: 7320 6173 2070 7965 636f 6e0a 0a20 2020  s as pyecon..   
-00002f60: 2320 4361 6c63 756c 6174 6520 706f 6c69  # Calculate poli
-00002f70: 6379 2072 756c 6520 6573 7469 6d61 7465  cy rule estimate
-00002f80: 730a 2020 2070 6f6c 6963 795f 6573 7469  s.   policy_esti
-00002f90: 6d61 7465 7320 3d20 7079 6563 6f6e 2e74  mates = pyecon.t
-00002fa0: 6179 6c6f 725f 7275 6c65 2876 6572 626f  aylor_rule(verbo
-00002fb0: 7365 3d54 7275 6529 0a0a 5665 7262 6f73  se=True)..Verbos
-00002fc0: 6520 5072 696e 7420 5374 6174 656d 656e  e Print Statemen
-00002fd0: 743a 0a0a 2e2e 2063 6f64 652d 626c 6f63  t:.... code-bloc
-00002fe0: 6b3a 3a20 6e6f 6e65 0a0a 2020 203d 3d3d  k:: none..   ===
-00002ff0: 3d20 4563 6f6e 6f6d 6963 2049 6e64 6963  = Economic Indic
-00003000: 6174 6f72 7320 3d3d 3d3d 3d3d 3d3d 3d3d  ators ==========
-00003010: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00003020: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00003030: 3d3d 3d3d 3d3d 3d0a 2020 2043 7572 7265  =======.   Curre
-00003040: 6e74 2049 6e66 6c61 7469 6f6e 3a20 2020  nt Inflation:   
-00003050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003060: 2020 2020 2020 2020 2020 2020 332e 3034              3.04
-00003070: 250a 2020 2054 6172 6765 7420 496e 666c  %.   Target Infl
-00003080: 6174 696f 6e3a 2020 2020 2020 2020 2020  ation:          
-00003090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030a0: 2020 2020 2020 322e 3030 250a 2020 2043        2.00%.   C
-000030b0: 7572 7265 6e74 2055 6e65 6d70 6c6f 796d  urrent Unemploym
-000030c0: 656e 7420 5261 7465 3a20 2020 2020 2020  ent Rate:       
-000030d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030e0: 332e 3930 250a 2020 204e 6174 7572 616c  3.90%.   Natural
-000030f0: 2055 6e65 6d70 6c6f 796d 656e 7420 5261   Unemployment Ra
-00003100: 7465 3a20 2020 2020 2020 2020 2020 2020  te:             
-00003110: 2020 2020 2020 2020 2020 342e 3431 250a            4.41%.
-00003120: 2020 204c 6f6e 672d 5465 726d 2052 6561     Long-Term Rea
-00003130: 6c20 496e 7465 7265 7374 2052 6174 653a  l Interest Rate:
-00003140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003150: 2020 2020 322e 3130 250a 2020 2043 7572      2.10%.   Cur
-00003160: 7265 6e74 2046 6564 2052 6174 653a 2020  rent Fed Rate:  
-00003170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003180: 2020 2020 2020 2020 2020 2020 2020 352e                5.
-00003190: 3530 250a 2020 2041 7320 6f66 2044 6174  50%.   As of Dat
-000031a0: 653a 2020 2020 2020 2020 2020 2020 2020  e:              
-000031b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031c0: 2020 2020 2020 2020 4d61 7920 3231 2c20          May 21, 
-000031d0: 3230 3234 0a0a 2020 203d 3d3d 3d20 4761  2024..   ==== Ga
-000031e0: 7073 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ps =============
-000031f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00003200: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00003210: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00003220: 3d3d 3d0a 2020 2049 6e66 6c61 7469 6f6e  ===.   Inflation
-00003230: 2047 6170 3a20 2020 2020 2020 2020 2020   Gap:           
-00003240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003250: 2020 2020 2020 2020 312e 3034 250a 2020          1.04%.  
-00003260: 2055 6e65 6d70 6c6f 796d 656e 7420 4761   Unemployment Ga
-00003270: 703a 2020 2020 2020 2020 2020 2020 2020  p:              
-00003280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003290: 2020 302e 3531 250a 0a20 2020 3d3d 3d3d    0.51%..   ====
-000032a0: 2054 6179 6c6f 7220 5275 6c65 203d 3d3d   Taylor Rule ===
-000032b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000032c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000032d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000032e0: 3d3d 3d3d 3d3d 0a20 2020 2020 4c6f 6e67  ======.     Long
-000032f0: 2d54 6572 6d20 5265 616c 2049 6e74 6572  -Term Real Inter
-00003300: 6573 7420 5261 7465 3a20 2020 2020 2020  est Rate:       
-00003310: 2020 2020 2020 2020 2020 2032 2e31 3025             2.10%
-00003320: 0a20 2020 2020 4375 7272 656e 7420 496e  .     Current In
-00003330: 666c 6174 696f 6e3a 2020 2020 2020 2020  flation:        
-00003340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003350: 2020 2020 202b 2033 2e30 3425 0a20 2020       + 3.04%.   
-00003360: 2020 416c 7068 6120 2a20 496e 666c 6174    Alpha * Inflat
-00003370: 696f 6e20 4761 703a 2020 2020 2020 2020  ion Gap:        
+00002ba0: e294 a40a 2020 20e2 9482 2041 7320 6f66  ....   ... As of
+00002bb0: 2044 6174 6520 2020 2020 2020 2020 2020   Date           
+00002bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002be0: 2020 2020 2020 2020 2020 4d61 7920 3231            May 21
+00002bf0: 2c20 3230 3234 2020 2020 2020 20e2 9482  , 2024       ...
+00002c00: 0a20 2020 e294 9ce2 9480 e294 80e2 9480  .   ............
+00002c10: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002c20: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002c30: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002c40: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002c50: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002c60: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002c70: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002c80: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002c90: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002ca0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002cb0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002cc0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002cd0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002ce0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002cf0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002d00: e294 a40a 2020 20e2 9482 2020 2020 2020  ....   ...      
+00002d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d20: 2020 2020 2020 4164 6a75 7374 6564 2050        Adjusted P
+00002d30: 6f6c 6963 7920 5072 6573 6372 6970 7469  olicy Prescripti
+00002d40: 6f6e 2020 2020 2020 2020 2020 2020 2020  on              
+00002d50: 2020 2020 2020 2020 2020 2020 20e2 9482               ...
+00002d60: 0a20 2020 e294 9ce2 9480 e294 80e2 9480  .   ............
+00002d70: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002d80: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002d90: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002da0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002db0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002dc0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002dd0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002de0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002df0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002e00: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002e10: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002e20: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002e30: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002e40: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002e50: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002e60: e294 a40a 2020 20e2 9482 2054 6179 6c6f  ....   ... Taylo
+00002e70: 7220 5275 6c65 2028 5452 2920 7375 6767  r Rule (TR) sugg
+00002e80: 6573 7473 2072 6169 7369 6e67 2074 6865  ests raising the
+00002e90: 2072 6174 6520 6279 2030 2e32 3525 2e20   rate by 0.25%. 
+00002ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002eb0: 2020 2020 2020 2020 2020 2020 20e2 9482               ...
+00002ec0: 0a20 2020 e294 8220 4261 6c61 6e63 6564  .   ... Balanced
+00002ed0: 2041 7070 726f 6163 6820 5275 6c65 2028   Approach Rule (
+00002ee0: 4241 5229 2073 7567 6765 7374 7320 7261  BAR) suggests ra
+00002ef0: 6973 696e 6720 7468 6520 7261 7465 2062  ising the rate b
+00002f00: 7920 302e 3235 252e 2020 2020 2020 2020  y 0.25%.        
+00002f10: 2020 2020 2020 2020 2020 e294 820a 2020            ....  
+00002f20: 20e2 9482 2042 616c 616e 6365 6420 4170   ... Balanced Ap
+00002f30: 7072 6f61 6368 2053 686f 7274 6661 6c6c  proach Shortfall
+00002f40: 7320 5275 6c65 2028 4241 5352 2920 7375  s Rule (BASR) su
+00002f50: 6767 6573 7473 206d 6169 6e74 6169 6e69  ggests maintaini
+00002f60: 6e67 2074 6865 2063 7572 7265 6e74 2072  ng the current r
+00002f70: 6174 652e 2020 20e2 9482 0a20 2020 e294  ate.   ....   ..
+00002f80: 8220 4669 7273 7420 4469 6666 6572 656e  . First Differen
+00002f90: 6365 2052 756c 6520 2846 4452 2920 7375  ce Rule (FDR) su
+00002fa0: 6767 6573 7473 2072 6169 7369 6e67 2074  ggests raising t
+00002fb0: 6865 2072 6174 6520 6279 2030 2e32 3525  he rate by 0.25%
+00002fc0: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
+00002fd0: 2020 2020 e294 820a 2020 20e2 9494 e294      ....   .....
+00002fe0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002ff0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003000: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003010: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003020: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003030: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003040: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003050: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003060: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003070: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003080: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003090: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000030a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000030b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000030c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000030d0: 80e2 9480 e294 80e2 9498 0a0a 4578 616d  ............Exam
+000030e0: 706c 6520 333a 2043 616c 6375 6c61 7465  ple 3: Calculate
+000030f0: 2043 7572 7265 6e74 2054 6179 6c6f 7220   Current Taylor 
+00003100: 5275 6c65 2045 7374 696d 6174 6573 0a2d  Rule Estimates.-
+00003110: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003120: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003130: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003140: 2d0a 0a2e 2e20 636f 6465 2d62 6c6f 636b  -.... code-block
+00003150: 3a3a 2070 7974 686f 6e0a 0a20 2020 2320  :: python..   # 
+00003160: 496d 706f 7274 2070 7965 636f 6e6f 6d69  Import pyeconomi
+00003170: 6373 206d 6f64 756c 6573 0a20 2020 696d  cs modules.   im
+00003180: 706f 7274 2070 7965 636f 6e6f 6d69 6373  port pyeconomics
+00003190: 2061 7320 7079 6563 6f6e 0a0a 2020 2023   as pyecon..   #
+000031a0: 2043 616c 6375 6c61 7465 2070 6f6c 6963   Calculate polic
+000031b0: 7920 7275 6c65 2065 7374 696d 6174 6573  y rule estimates
+000031c0: 0a20 2020 706f 6c69 6379 5f65 7374 696d  .   policy_estim
+000031d0: 6174 6573 203d 2070 7965 636f 6e2e 7461  ates = pyecon.ta
+000031e0: 796c 6f72 5f72 756c 6528 7665 7262 6f73  ylor_rule(verbos
+000031f0: 653d 5472 7565 290a 0a56 6572 626f 7365  e=True)..Verbose
+00003200: 2050 7269 6e74 2053 7461 7465 6d65 6e74   Print Statement
+00003210: 3a0a 0a2e 2e20 636f 6465 2d62 6c6f 636b  :.... code-block
+00003220: 3a3a 206e 6f6e 650a 0a20 2020 3d3d 3d3d  :: none..   ====
+00003230: 2045 636f 6e6f 6d69 6320 496e 6469 6361   Economic Indica
+00003240: 746f 7273 203d 3d3d 3d3d 3d3d 3d3d 3d3d  tors ===========
+00003250: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00003260: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00003270: 3d3d 3d3d 3d3d 0a20 2020 4375 7272 656e  ======.   Curren
+00003280: 7420 496e 666c 6174 696f 6e3a 2020 2020  t Inflation:    
+00003290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000032a0: 2020 2020 2020 2020 2020 2033 2e30 3425             3.04%
+000032b0: 0a20 2020 5461 7267 6574 2049 6e66 6c61  .   Target Infla
+000032c0: 7469 6f6e 3a20 2020 2020 2020 2020 2020  tion:           
+000032d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000032e0: 2020 2020 2032 2e30 3025 0a20 2020 4375       2.00%.   Cu
+000032f0: 7272 656e 7420 556e 656d 706c 6f79 6d65  rrent Unemployme
+00003300: 6e74 2052 6174 653a 2020 2020 2020 2020  nt Rate:        
+00003310: 2020 2020 2020 2020 2020 2020 2020 2033                 3
+00003320: 2e39 3025 0a20 2020 4e61 7475 7261 6c20  .90%.   Natural 
+00003330: 556e 656d 706c 6f79 6d65 6e74 2052 6174  Unemployment Rat
+00003340: 653a 2020 2020 2020 2020 2020 2020 2020  e:              
+00003350: 2020 2020 2020 2020 2034 2e34 3125 0a20           4.41%. 
+00003360: 2020 4c6f 6e67 2d54 6572 6d20 5265 616c    Long-Term Real
+00003370: 2049 6e74 6572 6573 7420 5261 7465 3a20   Interest Rate: 
 00003380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003390: 202b 2030 2e35 3020 2a20 312e 3034 250a   + 0.50 * 1.04%.
-000033a0: 2020 2020 2042 6574 6120 2a20 4f6b 756e       Beta * Okun
-000033b0: 2046 6163 746f 7220 2a20 556e 656d 706c   Factor * Unempl
-000033c0: 6f79 6d65 6e74 2047 6170 3a20 2020 2020  oyment Gap:     
-000033d0: 2020 2020 2b20 302e 3530 202a 2032 2e30      + 0.50 * 2.0
-000033e0: 3020 2a20 302e 3531 250a 2020 202d 2d2d  0 * 0.51%.   ---
-000033f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003400: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003410: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003420: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003430: 2d2d 2d2d 2d2d 2d0a 2020 2020 2055 6e61  -------.     Una
-00003440: 646a 7573 7465 6420 5461 796c 6f72 2052  djusted Taylor R
-00003450: 756c 6520 4573 7469 6d61 7465 3a20 2020  ule Estimate:   
-00003460: 2020 2020 2020 2020 2020 2020 362e 3137              6.17
-00003470: 250a 0a20 2020 3d3d 3d3d 2041 646a 7573  %..   ==== Adjus
-00003480: 7465 6420 5461 796c 6f72 2052 756c 6520  ted Taylor Rule 
-00003490: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000034a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000034b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000034c0: 0a20 2020 2020 4566 6665 6374 6976 6520  .     Effective 
-000034d0: 4c6f 7765 7220 426f 756e 6420 2845 4c42  Lower Bound (ELB
-000034e0: 2920 4164 6a75 7374 6d65 6e74 3a0a 2020  ) Adjustment:.  
-000034f0: 2020 204d 6178 696d 756d 206f 6620 5461     Maximum of Ta
-00003500: 796c 6f72 2052 756c 6520 6f72 2045 4c42  ylor Rule or ELB
-00003510: 3a20 2020 2020 2020 2020 2020 2020 2020  :               
-00003520: 2020 6d61 7828 362e 3137 252c 2030 2e31    max(6.17%, 0.1
-00003530: 3225 290a 2020 202d 2d2d 2d2d 2d2d 2d2d  2%).   ---------
-00003540: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003550: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003560: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003570: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003580: 2d0a 2020 2020 2054 6179 6c6f 7220 5275  -.     Taylor Ru
-00003590: 6c65 2041 646a 7573 7465 6420 666f 7220  le Adjusted for 
-000035a0: 454c 423a 2020 2020 2020 2020 2020 2020  ELB:            
-000035b0: 2020 2020 2020 362e 3137 250a 0a20 2020        6.17%..   
-000035c0: 2020 506f 6c69 6379 2049 6e65 7274 6961    Policy Inertia
-000035d0: 2041 646a 7573 746d 656e 743a 0a20 2020   Adjustment:.   
-000035e0: 2020 506f 6c69 6379 2049 6e65 7274 6961    Policy Inertia
-000035f0: 2043 6f65 6666 6963 6965 6e74 2028 7268   Coefficient (rh
-00003600: 6f29 3a20 2020 2020 2020 2020 2020 2020  o):             
-00003610: 2030 2e37 300a 2020 2020 2043 7572 7265   0.70.     Curre
-00003620: 6e74 2046 6564 2052 6174 653a 2020 2020  nt Fed Rate:    
-00003630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003640: 2020 2020 2020 2020 2020 2a20 352e 3530            * 5.50
-00003650: 250a 2020 2020 2041 646a 7573 746d 656e  %.     Adjustmen
-00003660: 7420 436f 6566 6669 6369 656e 7420 2831  t Coefficient (1
-00003670: 202d 2072 686f 293a 2020 2020 2020 2020   - rho):        
-00003680: 2020 2020 2020 2b20 2831 202d 2030 2e37        + (1 - 0.7
-00003690: 3029 0a20 2020 2020 5461 796c 6f72 2052  0).     Taylor R
-000036a0: 756c 6520 4164 6a75 7374 6564 2066 6f72  ule Adjusted for
-000036b0: 2045 4c42 3a20 2020 2020 2020 2020 2020   ELB:           
-000036c0: 2020 2020 2020 202a 2036 2e31 3725 0a20         * 6.17%. 
-000036d0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
-000036e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000036f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003700: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003710: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
-00003720: 2020 4164 6a75 7374 6564 2054 6179 6c6f    Adjusted Taylo
-00003730: 7220 5275 6c65 2045 7374 696d 6174 653a  r Rule Estimate:
-00003740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003750: 2035 2e37 3025 0a0a 2020 203d 3d3d 3d20   5.70%..   ==== 
-00003760: 506f 6c69 6379 2050 7265 7363 7269 7074  Policy Prescript
-00003770: 696f 6e20 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ion ============
-00003780: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00003790: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000037a0: 3d3d 3d3d 3d0a 2020 2020 2054 6865 2041  =====.     The A
-000037b0: 646a 7573 7465 6420 5461 796c 6f72 2052  djusted Taylor R
-000037c0: 756c 6520 4573 7469 6d61 7465 2069 7320  ule Estimate is 
-000037d0: 302e 3230 2520 6869 6768 6572 2074 6861  0.20% higher tha
-000037e0: 6e20 7468 6520 4375 7272 656e 740a 2020  n the Current.  
-000037f0: 2020 2046 6564 2052 6174 652e 2054 6865     Fed Rate. The
-00003800: 2046 6564 2073 686f 756c 6420 636f 6e73   Fed should cons
-00003810: 6964 6572 2072 6169 7369 6e67 2074 6865  ider raising the
-00003820: 2069 6e74 6572 6573 7420 7261 7465 2062   interest rate b
-00003830: 7920 302e 3235 252e 0a0a 4578 616d 706c  y 0.25%...Exampl
-00003840: 6520 343a 2043 616c 6375 6c61 7465 2061  e 4: Calculate a
-00003850: 6e64 2050 6c6f 7420 4869 7374 6f72 6963  nd Plot Historic
-00003860: 616c 2050 6f6c 6963 7920 5275 6c65 2045  al Policy Rule E
-00003870: 7374 696d 6174 6573 0a2d 2d2d 2d2d 2d2d  stimates.-------
-00003880: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003890: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000038a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000038b0: 2d2d 2d2d 2d2d 2d0a 0a2e 2e20 636f 6465  -------.... code
-000038c0: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0a  -block:: python.
-000038d0: 0a20 2020 2320 496d 706f 7274 2070 7965  .   # Import pye
-000038e0: 636f 6e6f 6d69 6373 206d 6f64 756c 6573  conomics modules
-000038f0: 0a20 2020 696d 706f 7274 2070 7965 636f  .   import pyeco
-00003900: 6e6f 6d69 6373 2061 7320 7079 6563 6f6e  nomics as pyecon
-00003910: 0a0a 2020 2023 2043 616c 6375 6c61 7465  ..   # Calculate
-00003920: 2068 6973 746f 7269 6361 6c20 706f 6c69   historical poli
-00003930: 6379 2072 6174 6573 0a20 2020 6869 7374  cy rates.   hist
-00003940: 6f72 6963 616c 5f70 6f6c 6963 795f 6573  orical_policy_es
-00003950: 7469 6d61 7465 7320 3d20 7079 6563 6f6e  timates = pyecon
-00003960: 2e63 616c 6375 6c61 7465 5f68 6973 746f  .calculate_histo
-00003970: 7269 6361 6c5f 706f 6c69 6379 5f72 6174  rical_policy_rat
-00003980: 6573 2829 2e64 726f 706e 6128 290a 0a20  es().dropna().. 
-00003990: 2020 2320 506c 6f74 2068 6973 746f 7269    # Plot histori
-000039a0: 6361 6c20 706f 6c69 6379 2072 6174 6573  cal policy rates
-000039b0: 0a20 2020 7079 6563 6f6e 2e70 6c6f 745f  .   pyecon.plot_
-000039c0: 6869 7374 6f72 6963 616c 5f72 756c 655f  historical_rule_
-000039d0: 6573 7469 6d61 7465 7328 6869 7374 6f72  estimates(histor
-000039e0: 6963 616c 5f70 6f6c 6963 795f 6573 7469  ical_policy_esti
-000039f0: 6d61 7465 7329 0a0a 2e2e 2069 6d61 6765  mates).... image
-00003a00: 3a3a 202e 2e2f 6d65 6469 612f 706c 6f74  :: ../media/plot
-00003a10: 5f68 6973 746f 7269 6361 6c5f 706f 6c69  _historical_poli
-00003a20: 6379 5f72 6174 6573 2e70 6e67 0a0a 4578  cy_rates.png..Ex
-00003a30: 616d 706c 6520 353a 2043 616c 6375 6c61  ample 5: Calcula
-00003a40: 7465 2061 6e64 2050 6c6f 7420 7468 6520  te and Plot the 
-00003a50: 4164 6a75 7374 6564 2048 6973 746f 7269  Adjusted Histori
-00003a60: 6361 6c20 506f 6c69 6379 2052 756c 6573  cal Policy Rules
-00003a70: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .---------------
-00003a80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003a90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003aa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003ab0: 2d2d 2d0a 0a2e 2e20 636f 6465 2d62 6c6f  ---.... code-blo
-00003ac0: 636b 3a3a 2070 7974 686f 6e0a 0a20 2020  ck:: python..   
-00003ad0: 2320 496d 706f 7274 2070 7965 636f 6e6f  # Import pyecono
-00003ae0: 6d69 6373 206d 6f64 756c 6573 0a20 2020  mics modules.   
-00003af0: 696d 706f 7274 2070 7965 636f 6e6f 6d69  import pyeconomi
-00003b00: 6373 2061 7320 7079 6563 6f6e 0a0a 2020  cs as pyecon..  
-00003b10: 2023 2041 646a 7573 746d 656e 7420 5061   # Adjustment Pa
-00003b20: 7261 6d65 7465 7273 0a20 2020 7268 6f20  rameters.   rho 
-00003b30: 3d20 302e 3720 2023 2050 6f6c 6963 7920  = 0.7  # Policy 
-00003b40: 496e 6572 7469 6120 436f 6566 6669 6369  Inertia Coeffici
-00003b50: 656e 740a 2020 2061 7070 6c79 5f65 6c62  ent.   apply_elb
-00003b60: 203d 2054 7275 6520 2023 2041 7070 6c79   = True  # Apply
-00003b70: 2045 6666 6563 7469 7665 204c 6f77 6572   Effective Lower
-00003b80: 2042 6f75 6e64 0a0a 2020 2023 2043 616c   Bound..   # Cal
-00003b90: 6375 6c61 7465 2061 646a 7573 7465 6420  culate adjusted 
-00003ba0: 6869 7374 6f72 6963 616c 2070 6f6c 6963  historical polic
-00003bb0: 7920 7261 7465 730a 2020 2061 646a 7573  y rates.   adjus
-00003bc0: 7465 645f 6869 7374 6f72 6963 616c 5f70  ted_historical_p
-00003bd0: 6f6c 6963 795f 6573 7469 6d61 7465 7320  olicy_estimates 
-00003be0: 3d20 7079 6563 6f6e 2e63 616c 6375 6c61  = pyecon.calcula
-00003bf0: 7465 5f68 6973 746f 7269 6361 6c5f 706f  te_historical_po
-00003c00: 6c69 6379 5f72 6174 6573 280a 2020 2020  licy_rates(.    
-00003c10: 2020 2072 686f 3d72 686f 2c0a 2020 2020     rho=rho,.    
-00003c20: 2020 2061 7070 6c79 5f65 6c62 3d61 7070     apply_elb=app
-00003c30: 6c79 5f65 6c62 0a20 2020 292e 6472 6f70  ly_elb.   ).drop
-00003c40: 6e61 2829 0a0a 2020 2023 2050 6c6f 7420  na()..   # Plot 
-00003c50: 6164 6a75 7374 6564 2068 6973 746f 7269  adjusted histori
-00003c60: 6361 6c20 706f 6c69 6379 2072 6174 6573  cal policy rates
-00003c70: 0a20 2020 7079 6563 6f6e 2e70 6c6f 745f  .   pyecon.plot_
-00003c80: 6869 7374 6f72 6963 616c 5f72 756c 655f  historical_rule_
-00003c90: 6573 7469 6d61 7465 7328 0a20 2020 2020  estimates(.     
-00003ca0: 2020 6164 6a75 7374 6564 5f68 6973 746f    adjusted_histo
-00003cb0: 7269 6361 6c5f 706f 6c69 6379 5f65 7374  rical_policy_est
-00003cc0: 696d 6174 6573 2c0a 2020 2020 2020 2061  imates,.       a
-00003cd0: 646a 7573 7465 643d 5472 7565 0a20 2020  djusted=True.   
-00003ce0: 290a 0a2e 2e20 696d 6167 653a 3a20 2e2e  ).... image:: ..
-00003cf0: 2f6d 6564 6961 2f70 6c6f 745f 6164 6a5f  /media/plot_adj_
-00003d00: 6869 7374 6f72 6963 616c 5f72 6174 6573  historical_rates
-00003d10: 2e70 6e67 0a0a 4578 616d 706c 6573 0a3d  .png..Examples.=
-00003d20: 3d3d 3d3d 3d3d 3d0a 0a46 6f72 206d 6f72  =======..For mor
-00003d30: 6520 636f 6d70 7265 6865 6e73 6976 6520  e comprehensive 
-00003d40: 6578 616d 706c 6573 2c20 7265 6665 7220  examples, refer 
-00003d50: 746f 2074 6865 2060 6578 616d 706c 6573  to the `examples
-00003d60: 203c 6578 616d 706c 6573 3e60 5f20 6469   <examples>`_ di
-00003d70: 7265 6374 6f72 7920 696e 0a74 6865 2072  rectory in.the r
-00003d80: 6570 6f73 6974 6f72 792e 0a0a 526f 6164  epository...Road
-00003d90: 6d61 700a 3d3d 3d3d 3d3d 3d0a 0a54 6865  map.=======..The
-00003da0: 2066 6f6c 6c6f 7769 6e67 206d 6f64 656c   following model
-00003db0: 7320 616e 6420 6361 7465 676f 7269 6573  s and categories
-00003dc0: 2061 7265 2070 6c61 6e6e 6564 2066 6f72   are planned for
-00003dd0: 2066 7574 7572 6520 6465 7665 6c6f 706d   future developm
-00003de0: 656e 742e 0a60 436f 6e74 7269 6275 7469  ent..`Contributi
-00003df0: 6f6e 7320 3c63 6f6e 7472 6962 7574 696e  ons <contributin
-00003e00: 673e 605f 2061 7265 2077 656c 636f 6d65  g>`_ are welcome
-00003e10: 210a 0a2e 2e20 7275 6272 6963 3a3a 204d  !.... rubric:: M
-00003e20: 6f6e 6574 6172 7920 506f 6c69 6379 204d  onetary Policy M
-00003e30: 6f64 656c 730a 0a2d 2054 6179 6c6f 7220  odels..- Taylor 
-00003e40: 5275 6c65 0a2d 2042 616c 616e 6365 6420  Rule.- Balanced 
-00003e50: 4170 7072 6f61 6368 2052 756c 650a 2d20  Approach Rule.- 
-00003e60: 4669 7273 7420 4469 6666 6572 656e 6365  First Difference
-00003e70: 2052 756c 650a 2d20 4d63 4361 6c6c 756d   Rule.- McCallum
-00003e80: 2052 756c 650a 2d20 4f72 7068 616e 6964   Rule.- Orphanid
-00003e90: 6573 2052 756c 650a 2d20 4672 6965 646d  es Rule.- Friedm
-00003ea0: 616e 2052 756c 650a 2d20 496e 7465 7265  an Rule.- Intere
-00003eb0: 7374 2052 6174 6520 536d 6f6f 7468 696e  st Rate Smoothin
-00003ec0: 6720 4d6f 6465 6c73 0a0a 2e2e 2072 7562  g Models.... rub
-00003ed0: 7269 633a 3a20 5175 616e 7469 7479 206f  ric:: Quantity o
-00003ee0: 6620 4d6f 6e65 7920 5468 656f 7279 0a0a  f Money Theory..
-00003ef0: 2d20 4669 7368 6572 2045 7175 6174 696f  - Fisher Equatio
-00003f00: 6e0a 2d20 4361 6d62 7269 6467 6520 4571  n.- Cambridge Eq
-00003f10: 7561 7469 6f6e 0a2d 2056 656c 6f63 6974  uation.- Velocit
-00003f20: 7920 6f66 204d 6f6e 6579 204d 6f64 656c  y of Money Model
-00003f30: 730a 2d20 5175 616e 7469 7479 2054 6865  s.- Quantity The
-00003f40: 6f72 7920 6f66 204d 6f6e 6579 2028 5154  ory of Money (QT
-00003f50: 4d29 0a2d 204d 6f6e 6579 2044 656d 616e  M).- Money Deman
-00003f60: 6420 4675 6e63 7469 6f6e 2028 4d64 290a  d Function (Md).
-00003f70: 0a2e 2e20 7275 6272 6963 3a3a 2045 636f  ... rubric:: Eco
-00003f80: 6e6f 6d69 6320 4d6f 6465 6c73 2074 6f20  nomic Models to 
-00003f90: 5072 6564 6963 7420 4675 7475 7265 2045  Predict Future E
-00003fa0: 7863 6861 6e67 6520 5261 7465 730a 0a2d  xchange Rates..-
-00003fb0: 2050 7572 6368 6173 696e 6720 506f 7765   Purchasing Powe
-00003fc0: 7220 5061 7269 7479 2028 5050 5029 0a2d  r Parity (PPP).-
-00003fd0: 2049 6e74 6572 6573 7420 5261 7465 2050   Interest Rate P
-00003fe0: 6172 6974 7920 2849 5250 290a 2d20 4d6f  arity (IRP).- Mo
-00003ff0: 6e65 7461 7279 204d 6f64 656c 7320 6f66  netary Models of
-00004000: 2045 7863 6861 6e67 6520 5261 7465 730a   Exchange Rates.
-00004010: 2d20 506f 7274 666f 6c69 6f20 4261 6c61  - Portfolio Bala
-00004020: 6e63 6520 4d6f 6465 6c73 0a2d 2042 6568  nce Models.- Beh
-00004030: 6176 696f 7261 6c20 4571 7569 6c69 6272  avioral Equilibr
-00004040: 6975 6d20 4578 6368 616e 6765 2052 6174  ium Exchange Rat
-00004050: 6520 2842 4545 5229 0a2d 2046 756e 6461  e (BEER).- Funda
-00004060: 6d65 6e74 616c 2045 7175 696c 6962 7269  mental Equilibri
-00004070: 756d 2045 7863 6861 6e67 6520 5261 7465  um Exchange Rate
-00004080: 2028 4645 4552 290a 0a2e 2e20 7275 6272   (FEER).... rubr
-00004090: 6963 3a3a 204d 6163 726f 6563 6f6e 6f6d  ic:: Macroeconom
-000040a0: 6963 204d 6f64 656c 730a 0a2d 2049 532d  ic Models..- IS-
-000040b0: 4c4d 204d 6f64 656c 0a2d 2041 442d 4153  LM Model.- AD-AS
-000040c0: 204d 6f64 656c 0a2d 2053 6f6c 6f77 2047   Model.- Solow G
-000040d0: 726f 7774 6820 4d6f 6465 6c0a 2d20 4e65  rowth Model.- Ne
-000040e0: 7720 4b65 796e 6573 6961 6e20 4d6f 6465  w Keynesian Mode
-000040f0: 6c73 0a2d 2052 4243 2028 5265 616c 2042  ls.- RBC (Real B
-00004100: 7573 696e 6573 7320 4379 636c 6529 204d  usiness Cycle) M
-00004110: 6f64 656c 0a2d 2044 5347 4520 2844 796e  odel.- DSGE (Dyn
-00004120: 616d 6963 2053 746f 6368 6173 7469 6320  amic Stochastic 
-00004130: 4765 6e65 7261 6c20 4571 7569 6c69 6272  General Equilibr
-00004140: 6975 6d29 204d 6f64 656c 730a 0a2e 2e20  ium) Models.... 
-00004150: 7275 6272 6963 3a3a 204d 6963 726f 6563  rubric:: Microec
-00004160: 6f6e 6f6d 6963 204d 6f64 656c 730a 0a2d  onomic Models..-
-00004170: 2053 7570 706c 7920 616e 6420 4465 6d61   Supply and Dema
-00004180: 6e64 204d 6f64 656c 730a 2d20 436f 6e73  nd Models.- Cons
-00004190: 756d 6572 2043 686f 6963 6520 5468 656f  umer Choice Theo
-000041a0: 7279 0a2d 2050 726f 6475 6374 696f 6e20  ry.- Production 
-000041b0: 5468 656f 7279 0a2d 2043 6f73 7420 4675  Theory.- Cost Fu
-000041c0: 6e63 7469 6f6e 730a 2d20 4761 6d65 2054  nctions.- Game T
-000041d0: 6865 6f72 7920 4d6f 6465 6c73 0a2d 204d  heory Models.- M
-000041e0: 6172 6b65 7420 5374 7275 6374 7572 6520  arket Structure 
-000041f0: 4d6f 6465 6c73 2028 5065 7266 6563 7420  Models (Perfect 
-00004200: 436f 6d70 6574 6974 696f 6e2c 204d 6f6e  Competition, Mon
-00004210: 6f70 6f6c 792c 204f 6c69 676f 706f 6c79  opoly, Oligopoly
-00004220: 290a 0a2e 2e20 7275 6272 6963 3a3a 2044  ).... rubric:: D
-00004230: 6973 636f 756e 7465 6420 4361 7368 2046  iscounted Cash F
-00004240: 6c6f 7720 4d6f 6465 6c73 0a0a 2d20 4469  low Models..- Di
-00004250: 7669 6465 6e64 2044 6973 636f 756e 7420  vidend Discount 
-00004260: 4d6f 6465 6c20 2844 444d 290a 2d20 4672  Model (DDM).- Fr
-00004270: 6565 2043 6173 6820 466c 6f77 2074 6f20  ee Cash Flow to 
-00004280: 4571 7569 7479 2028 4643 4645 290a 2d20  Equity (FCFE).- 
-00004290: 4672 6565 2043 6173 6820 466c 6f77 2074  Free Cash Flow t
-000042a0: 6f20 4669 726d 2028 4643 4646 290a 2d20  o Firm (FCFF).- 
-000042b0: 4e65 7420 5072 6573 656e 7420 5661 6c75  Net Present Valu
-000042c0: 6520 284e 5056 290a 2d20 496e 7465 726e  e (NPV).- Intern
-000042d0: 616c 2052 6174 6520 6f66 2052 6574 7572  al Rate of Retur
-000042e0: 6e20 2849 5252 290a 2d20 4164 6a75 7374  n (IRR).- Adjust
-000042f0: 6564 2050 7265 7365 6e74 2056 616c 7565  ed Present Value
-00004300: 2028 4150 5629 0a0a 2e2e 2072 7562 7269   (APV).... rubri
-00004310: 633a 3a20 4669 6e61 6e63 6961 6c20 4d6f  c:: Financial Mo
-00004320: 6465 6c73 0a0a 2d20 4361 7069 7461 6c20  dels..- Capital 
-00004330: 4173 7365 7420 5072 6963 696e 6720 4d6f  Asset Pricing Mo
-00004340: 6465 6c20 2843 4150 4d29 0a2d 2041 7262  del (CAPM).- Arb
-00004350: 6974 7261 6765 2050 7269 6369 6e67 2054  itrage Pricing T
-00004360: 6865 6f72 7920 2841 5054 290a 2d20 426c  heory (APT).- Bl
-00004370: 6163 6b2d 5363 686f 6c65 7320 4f70 7469  ack-Scholes Opti
-00004380: 6f6e 2050 7269 6369 6e67 204d 6f64 656c  on Pricing Model
-00004390: 0a2d 2042 6f6e 6420 5661 6c75 6174 696f  .- Bond Valuatio
-000043a0: 6e20 4d6f 6465 6c73 0a2d 2043 7265 6469  n Models.- Credi
-000043b0: 7420 5269 736b 204d 6f64 656c 7320 2865  t Risk Models (e
-000043c0: 2e67 2e2c 204d 6572 746f 6e20 4d6f 6465  .g., Merton Mode
-000043d0: 6c29 0a2d 2050 6f72 7466 6f6c 696f 204f  l).- Portfolio O
-000043e0: 7074 696d 697a 6174 696f 6e20 4d6f 6465  ptimization Mode
-000043f0: 6c73 2028 652e 672e 2c20 4d61 726b 6f77  ls (e.g., Markow
-00004400: 6974 7a20 4d6f 6465 6c29 0a0a 2e2e 2072  itz Model).... r
-00004410: 7562 7269 633a 3a20 4669 7363 616c 2050  ubric:: Fiscal P
-00004420: 6f6c 6963 7920 4d6f 6465 6c73 0a0a 2d20  olicy Models..- 
-00004430: 5461 7861 7469 6f6e 2061 6e64 2047 6f76  Taxation and Gov
-00004440: 6572 6e6d 656e 7420 5370 656e 6469 6e67  ernment Spending
-00004450: 204d 6f64 656c 730a 2d20 4275 6467 6574   Models.- Budget
-00004460: 2044 6566 6963 6974 204d 6f64 656c 730a   Deficit Models.
-00004470: 2d20 5075 626c 6963 2044 6562 7420 4d6f  - Public Debt Mo
-00004480: 6465 6c73 0a2d 2046 6973 6361 6c20 4d75  dels.- Fiscal Mu
-00004490: 6c74 6970 6c69 6572 204d 6f64 656c 730a  ltiplier Models.
-000044a0: 2d20 4c61 6666 6572 2043 7572 7665 0a2d  - Laffer Curve.-
-000044b0: 2052 6963 6172 6469 616e 2045 7175 6976   Ricardian Equiv
-000044c0: 616c 656e 6365 0a0a 2e2e 2072 7562 7269  alence.... rubri
-000044d0: 633a 3a20 4f74 6865 7220 5765 6c6c 2d4b  c:: Other Well-K
-000044e0: 6e6f 776e 2045 636f 6e6f 6d69 6320 4d6f  nown Economic Mo
-000044f0: 6465 6c73 0a0a 2d20 4265 6861 7669 6f72  dels..- Behavior
-00004500: 616c 2045 636f 6e6f 6d69 6373 204d 6f64  al Economics Mod
-00004510: 656c 730a 2d20 4167 656e 742d 4261 7365  els.- Agent-Base
-00004520: 6420 4d6f 6465 6c73 0a2d 2045 6e76 6972  d Models.- Envir
-00004530: 6f6e 6d65 6e74 616c 2045 636f 6e6f 6d69  onmental Economi
-00004540: 6373 204d 6f64 656c 730a 2d20 496e 7465  cs Models.- Inte
-00004550: 726e 6174 696f 6e61 6c20 5472 6164 6520  rnational Trade 
-00004560: 4d6f 6465 6c73 2028 652e 672e 2c20 4865  Models (e.g., He
-00004570: 636b 7363 6865 722d 4f68 6c69 6e20 4d6f  ckscher-Ohlin Mo
-00004580: 6465 6c29 0a2d 204c 6162 6f72 204d 6172  del).- Labor Mar
-00004590: 6b65 7420 4d6f 6465 6c73 0a2d 2048 6561  ket Models.- Hea
-000045a0: 6c74 6820 4563 6f6e 6f6d 6963 7320 4d6f  lth Economics Mo
-000045b0: 6465 6c73 0a0a 436f 6e74 7269 6275 7469  dels..Contributi
-000045c0: 6e67 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a  ng.============.
-000045d0: 0a43 6f6e 7472 6962 7574 696f 6e73 2061  .Contributions a
-000045e0: 7265 2077 656c 636f 6d65 2120 4966 2079  re welcome! If y
-000045f0: 6f75 2068 6176 6520 6120 6d6f 6465 6c20  ou have a model 
-00004600: 796f 7527 6420 6c69 6b65 2074 6f20 696d  you'd like to im
-00004610: 706c 656d 656e 7420 6f72 2061 6e0a 696d  plement or an.im
-00004620: 7072 6f76 656d 656e 7420 746f 2061 6e20  provement to an 
-00004630: 6578 6973 7469 6e67 206d 6f64 656c 2c20  existing model, 
-00004640: 706c 6561 7365 2072 6566 6572 2074 6f20  please refer to 
-00004650: 6f75 7220 6465 7461 696c 6564 0a60 436f  our detailed.`Co
-00004660: 6e74 7269 6275 7469 6e67 2047 7569 6465  ntributing Guide
-00004670: 203c 6d61 726b 646f 776e 2f43 4f4e 5452   <markdown/CONTR
-00004680: 4942 5554 494e 472e 6d64 3e60 5f2e 0a0a  IBUTING.md>`_...
-00004690: 4279 2070 6172 7469 6369 7061 7469 6e67  By participating
-000046a0: 2069 6e20 7468 6973 2070 726f 6a65 6374   in this project
-000046b0: 2c20 796f 7520 6167 7265 6520 746f 2061  , you agree to a
-000046c0: 6269 6465 2062 7920 7468 650a 6043 6f64  bide by the.`Cod
-000046d0: 6520 6f66 2043 6f6e 6475 6374 203c 6d61  e of Conduct <ma
-000046e0: 726b 646f 776e 2f43 4f44 455f 4f46 5f43  rkdown/CODE_OF_C
-000046f0: 4f4e 4455 4354 2e6d 643e 605f 2e0a 0a54  ONDUCT.md>`_...T
-00004700: 6861 6e6b 2079 6f75 2066 6f72 2079 6f75  hank you for you
-00004710: 7220 636f 6e74 7269 6275 7469 6f6e 7321  r contributions!
-00004720: 0a0a 436f 6e74 6163 740a 3d3d 3d3d 3d3d  ..Contact.======
-00004730: 3d0a 0a49 6620 796f 7520 6861 7665 2061  =..If you have a
-00004740: 6e79 2071 7565 7374 696f 6e73 2c20 7375  ny questions, su
-00004750: 6767 6573 7469 6f6e 732c 206f 7220 6e65  ggestions, or ne
-00004760: 6564 2073 7570 706f 7274 2c20 6665 656c  ed support, feel
-00004770: 2066 7265 6520 746f 2072 6561 6368 206f   free to reach o
-00004780: 7574 2e0a 0a4e 6174 6861 6e20 5261 6d6f  ut...Nathan Ramo
-00004790: 732c 2043 4641 0a2d 2d2d 2d2d 2d2d 2d2d  s, CFA.---------
-000047a0: 2d2d 2d2d 2d2d 2d2d 0a0a 5765 6c63 6f6d  --------..Welcom
-000047b0: 6520 746f 206d 7920 4769 7448 7562 2120  e to my GitHub! 
-000047c0: 4927 6d20 4e61 7468 616e 2c20 616e 2069  I'm Nathan, an i
-000047d0: 6e64 6570 656e 6465 6e74 2046 696e 7465  ndependent Finte
-000047e0: 6368 2044 6576 656c 6f70 6572 2077 6974  ch Developer wit
-000047f0: 6820 610a 4368 6172 7465 7265 6420 4669  h a.Chartered Fi
-00004800: 6e61 6e63 6961 6c20 416e 616c 7973 7420  nancial Analyst 
-00004810: 2843 4641 2920 6465 7369 676e 6174 696f  (CFA) designatio
-00004820: 6e2c 2073 7065 6369 616c 697a 696e 6720  n, specializing 
-00004830: 696e 2050 7974 686f 6e2d 6261 7365 640a  in Python-based.
-00004840: 6669 6e61 6e63 6961 6c20 616e 616c 7973  financial analys
-00004850: 6973 2c20 7175 616e 7469 7461 7469 7665  is, quantitative
-00004860: 2073 7472 6174 6567 6965 732c 2061 6e64   strategies, and
-00004870: 2061 7574 6f6d 6174 6564 2074 7261 6469   automated tradi
-00004880: 6e67 2070 726f 6772 616d 732e 0a43 7572  ng programs..Cur
-00004890: 7265 6e74 6c79 2c20 4927 6d20 6120 6669  rently, I'm a fi
-000048a0: 6e74 6563 6820 636f 6e73 756c 7461 6e74  ntech consultant
-000048b0: 206f 7065 6e20 746f 206e 6577 2063 6c69   open to new cli
-000048c0: 656e 7473 2e20 5363 6865 6475 6c65 2061  ents. Schedule a
-000048d0: 206d 6565 7469 6e67 0a77 6974 6820 6d65   meeting.with me
-000048e0: 2074 6f20 6469 7363 7573 7320 636f 6c6c   to discuss coll
-000048f0: 6162 6f72 6174 696e 6720 6f6e 2079 6f75  aborating on you
-00004900: 7220 6e65 7874 2070 726f 6a65 6374 206f  r next project o
-00004910: 7220 746f 206c 6561 726e 206d 6f72 6520  r to learn more 
-00004920: 6162 6f75 740a 6d79 2073 6572 7669 6365  about.my service
-00004930: 732e 0a0a f09f 9385 2060 5363 6865 6475  s....... `Schedu
-00004940: 6c65 2061 204d 6565 7469 6e67 2077 6974  le a Meeting wit
-00004950: 6820 4d65 203c 6874 7470 733a 2f2f 6361  h Me <https://ca
-00004960: 6c65 6e64 6c79 2e63 6f6d 2f6e 7263 6170  lendly.com/nrcap
-00004970: 6974 616c 6d61 6e61 6765 6d65 6e74 2f67  italmanagement/g
-00004980: 6974 6875 622d 6d65 6574 696e 673e 605f  ithub-meeting>`_
-00004990: 0a0a 436f 6e6e 6563 7420 7769 7468 204d  ..Connect with M
-000049a0: 650a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  e.--------------
-000049b0: 2d0a 0a2d 202a 2a45 6d61 696c 2a2a 3a20  -..- **Email**: 
-000049c0: 606e 6174 6861 6e2e 7261 6d6f 732e 6769  `nathan.ramos.gi
-000049d0: 7468 7562 4067 6d61 696c 2e63 6f6d 203c  thub@gmail.com <
-000049e0: 6d61 696c 746f 3a6e 6174 6861 6e2e 7261  mailto:nathan.ra
-000049f0: 6d6f 732e 6769 7468 7562 4067 6d61 696c  mos.github@gmail
-00004a00: 2e63 6f6d 3e60 5f0a 2d20 2a2a 5477 6974  .com>`_.- **Twit
-00004a10: 7465 722a 2a3a 2060 406e 6174 6861 6e72  ter**: `@nathanr
-00004a20: 616d 6f73 6366 6120 3c68 7474 7073 3a2f  amoscfa <https:/
-00004a30: 2f74 7769 7474 6572 2e63 6f6d 2f6e 6174  /twitter.com/nat
-00004a40: 6861 6e72 616d 6f73 6366 613e 605f 0a0a  hanramoscfa>`_..
-00004a50: 4665 656c 2066 7265 6520 746f 2063 6f6e  Feel free to con
-00004a60: 6e65 6374 2077 6974 6820 6d65 2066 6f72  nect with me for
-00004a70: 2061 6e79 2069 6e71 7569 7269 6573 206f   any inquiries o
-00004a80: 7220 636f 6c6c 6162 6f72 6174 696f 6e20  r collaboration 
-00004a90: 6f70 706f 7274 756e 6974 6965 732e 0a0a  opportunities...
-00004aa0: 496e 6469 6365 7320 616e 6420 7461 626c  Indices and tabl
-00004ab0: 6573 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  es.=============
-00004ac0: 3d3d 3d3d 3d0a 0a2a 203a 7265 663a 6067  =====..* :ref:`g
-00004ad0: 656e 696e 6465 7860 0a2a 203a 7265 663a  enindex`.* :ref:
-00004ae0: 606d 6f64 696e 6465 7860 0a2a 203a 7265  `modindex`.* :re
-00004af0: 663a 6073 6561 7263 6860 0a              f:`search`.
+00003390: 2020 2032 2e31 3025 0a20 2020 4375 7272     2.10%.   Curr
+000033a0: 656e 7420 4665 6420 5261 7465 3a20 2020  ent Fed Rate:   
+000033b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000033c0: 2020 2020 2020 2020 2020 2020 2035 2e35               5.5
+000033d0: 3025 0a20 2020 4173 206f 6620 4461 7465  0%.   As of Date
+000033e0: 3a20 2020 2020 2020 2020 2020 2020 2020  :               
+000033f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003400: 2020 2020 2020 204d 6179 2032 312c 2032         May 21, 2
+00003410: 3032 340a 0a20 2020 3d3d 3d3d 2047 6170  024..   ==== Gap
+00003420: 7320 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  s ==============
+00003430: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00003440: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00003450: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00003460: 3d3d 0a20 2020 496e 666c 6174 696f 6e20  ==.   Inflation 
+00003470: 4761 703a 2020 2020 2020 2020 2020 2020  Gap:            
+00003480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003490: 2020 2020 2020 2031 2e30 3425 0a20 2020         1.04%.   
+000034a0: 556e 656d 706c 6f79 6d65 6e74 2047 6170  Unemployment Gap
+000034b0: 3a20 2020 2020 2020 2020 2020 2020 2020  :               
+000034c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000034d0: 2030 2e35 3125 0a0a 2020 203d 3d3d 3d20   0.51%..   ==== 
+000034e0: 5461 796c 6f72 2052 756c 6520 3d3d 3d3d  Taylor Rule ====
+000034f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00003500: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00003510: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00003520: 3d3d 3d3d 3d0a 2020 2020 204c 6f6e 672d  =====.     Long-
+00003530: 5465 726d 2052 6561 6c20 496e 7465 7265  Term Real Intere
+00003540: 7374 2052 6174 653a 2020 2020 2020 2020  st Rate:        
+00003550: 2020 2020 2020 2020 2020 322e 3130 250a            2.10%.
+00003560: 2020 2020 2043 7572 7265 6e74 2049 6e66       Current Inf
+00003570: 6c61 7469 6f6e 3a20 2020 2020 2020 2020  lation:         
+00003580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003590: 2020 2020 2b20 332e 3034 250a 2020 2020      + 3.04%.    
+000035a0: 2041 6c70 6861 202a 2049 6e66 6c61 7469   Alpha * Inflati
+000035b0: 6f6e 2047 6170 3a20 2020 2020 2020 2020  on Gap:         
+000035c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000035d0: 2b20 302e 3530 202a 2031 2e30 3425 0a20  + 0.50 * 1.04%. 
+000035e0: 2020 2020 4265 7461 202a 204f 6b75 6e20      Beta * Okun 
+000035f0: 4661 6374 6f72 202a 2055 6e65 6d70 6c6f  Factor * Unemplo
+00003600: 796d 656e 7420 4761 703a 2020 2020 2020  yment Gap:      
+00003610: 2020 202b 2030 2e35 3020 2a20 322e 3030     + 0.50 * 2.00
+00003620: 202a 2030 2e35 3125 0a20 2020 2d2d 2d2d   * 0.51%.   ----
+00003630: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003640: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003650: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003660: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003670: 2d2d 2d2d 2d2d 0a20 2020 2020 556e 6164  ------.     Unad
+00003680: 6a75 7374 6564 2054 6179 6c6f 7220 5275  justed Taylor Ru
+00003690: 6c65 2045 7374 696d 6174 653a 2020 2020  le Estimate:    
+000036a0: 2020 2020 2020 2020 2020 2036 2e31 3725             6.17%
+000036b0: 0a0a 2020 203d 3d3d 3d20 4164 6a75 7374  ..   ==== Adjust
+000036c0: 6564 2054 6179 6c6f 7220 5275 6c65 203d  ed Taylor Rule =
+000036d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000036e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000036f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a  ===============.
+00003700: 2020 2020 2045 6666 6563 7469 7665 204c       Effective L
+00003710: 6f77 6572 2042 6f75 6e64 2028 454c 4229  ower Bound (ELB)
+00003720: 2041 646a 7573 746d 656e 743a 0a20 2020   Adjustment:.   
+00003730: 2020 4d61 7869 6d75 6d20 6f66 2054 6179    Maximum of Tay
+00003740: 6c6f 7220 5275 6c65 206f 7220 454c 423a  lor Rule or ELB:
+00003750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003760: 206d 6178 2836 2e31 3725 2c20 302e 3132   max(6.17%, 0.12
+00003770: 2529 0a20 2020 2d2d 2d2d 2d2d 2d2d 2d2d  %).   ----------
+00003780: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003790: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000037a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000037b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000037c0: 0a20 2020 2020 5461 796c 6f72 2052 756c  .     Taylor Rul
+000037d0: 6520 4164 6a75 7374 6564 2066 6f72 2045  e Adjusted for E
+000037e0: 4c42 3a20 2020 2020 2020 2020 2020 2020  LB:             
+000037f0: 2020 2020 2036 2e31 3725 0a0a 2020 2020       6.17%..    
+00003800: 2050 6f6c 6963 7920 496e 6572 7469 6120   Policy Inertia 
+00003810: 4164 6a75 7374 6d65 6e74 3a0a 2020 2020  Adjustment:.    
+00003820: 2050 6f6c 6963 7920 496e 6572 7469 6120   Policy Inertia 
+00003830: 436f 6566 6669 6369 656e 7420 2872 686f  Coefficient (rho
+00003840: 293a 2020 2020 2020 2020 2020 2020 2020  ):              
+00003850: 302e 3730 0a20 2020 2020 4375 7272 656e  0.70.     Curren
+00003860: 7420 4665 6420 5261 7465 3a20 2020 2020  t Fed Rate:     
+00003870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003880: 2020 2020 2020 2020 202a 2035 2e35 3025           * 5.50%
+00003890: 0a20 2020 2020 4164 6a75 7374 6d65 6e74  .     Adjustment
+000038a0: 2043 6f65 6666 6963 6965 6e74 2028 3120   Coefficient (1 
+000038b0: 2d20 7268 6f29 3a20 2020 2020 2020 2020  - rho):         
+000038c0: 2020 2020 202b 2028 3120 2d20 302e 3730       + (1 - 0.70
+000038d0: 290a 2020 2020 2054 6179 6c6f 7220 5275  ).     Taylor Ru
+000038e0: 6c65 2041 646a 7573 7465 6420 666f 7220  le Adjusted for 
+000038f0: 454c 423a 2020 2020 2020 2020 2020 2020  ELB:            
+00003900: 2020 2020 2020 2a20 362e 3137 250a 2020        * 6.17%.  
+00003910: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+00003920: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003930: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003940: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003950: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
+00003960: 2041 646a 7573 7465 6420 5461 796c 6f72   Adjusted Taylor
+00003970: 2052 756c 6520 4573 7469 6d61 7465 3a20   Rule Estimate: 
+00003980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003990: 352e 3730 250a 0a20 2020 3d3d 3d3d 2050  5.70%..   ==== P
+000039a0: 6f6c 6963 7920 5072 6573 6372 6970 7469  olicy Prescripti
+000039b0: 6f6e 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  on =============
+000039c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000039d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000039e0: 3d3d 3d3d 0a20 2020 2020 5468 6520 4164  ====.     The Ad
+000039f0: 6a75 7374 6564 2054 6179 6c6f 7220 5275  justed Taylor Ru
+00003a00: 6c65 2045 7374 696d 6174 6520 6973 2030  le Estimate is 0
+00003a10: 2e32 3025 2068 6967 6865 7220 7468 616e  .20% higher than
+00003a20: 2074 6865 2043 7572 7265 6e74 0a20 2020   the Current.   
+00003a30: 2020 4665 6420 5261 7465 2e20 5468 6520    Fed Rate. The 
+00003a40: 4665 6420 7368 6f75 6c64 2063 6f6e 7369  Fed should consi
+00003a50: 6465 7220 7261 6973 696e 6720 7468 6520  der raising the 
+00003a60: 696e 7465 7265 7374 2072 6174 6520 6279  interest rate by
+00003a70: 2030 2e32 3525 2e0a 0a45 7861 6d70 6c65   0.25%...Example
+00003a80: 2034 3a20 4361 6c63 756c 6174 6520 616e   4: Calculate an
+00003a90: 6420 506c 6f74 2048 6973 746f 7269 6361  d Plot Historica
+00003aa0: 6c20 506f 6c69 6379 2052 756c 6520 4573  l Policy Rule Es
+00003ab0: 7469 6d61 7465 730a 2d2d 2d2d 2d2d 2d2d  timates.--------
+00003ac0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003ad0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003ae0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003af0: 2d2d 2d2d 2d2d 0a0a 2e2e 2063 6f64 652d  ------.... code-
+00003b00: 626c 6f63 6b3a 3a20 7079 7468 6f6e 0a0a  block:: python..
+00003b10: 2020 2023 2049 6d70 6f72 7420 7079 6563     # Import pyec
+00003b20: 6f6e 6f6d 6963 7320 6d6f 6475 6c65 730a  onomics modules.
+00003b30: 2020 2069 6d70 6f72 7420 7079 6563 6f6e     import pyecon
+00003b40: 6f6d 6963 7320 6173 2070 7965 636f 6e0a  omics as pyecon.
+00003b50: 0a20 2020 2320 4361 6c63 756c 6174 6520  .   # Calculate 
+00003b60: 6869 7374 6f72 6963 616c 2070 6f6c 6963  historical polic
+00003b70: 7920 7261 7465 730a 2020 2068 6973 746f  y rates.   histo
+00003b80: 7269 6361 6c5f 706f 6c69 6379 5f65 7374  rical_policy_est
+00003b90: 696d 6174 6573 203d 2070 7965 636f 6e2e  imates = pyecon.
+00003ba0: 6361 6c63 756c 6174 655f 6869 7374 6f72  calculate_histor
+00003bb0: 6963 616c 5f70 6f6c 6963 795f 7261 7465  ical_policy_rate
+00003bc0: 7328 292e 6472 6f70 6e61 2829 0a0a 2020  s().dropna()..  
+00003bd0: 2023 2050 6c6f 7420 6869 7374 6f72 6963   # Plot historic
+00003be0: 616c 2070 6f6c 6963 7920 7261 7465 730a  al policy rates.
+00003bf0: 2020 2070 7965 636f 6e2e 706c 6f74 5f68     pyecon.plot_h
+00003c00: 6973 746f 7269 6361 6c5f 7275 6c65 5f65  istorical_rule_e
+00003c10: 7374 696d 6174 6573 2868 6973 746f 7269  stimates(histori
+00003c20: 6361 6c5f 706f 6c69 6379 5f65 7374 696d  cal_policy_estim
+00003c30: 6174 6573 290a 0a2e 2e20 696d 6167 653a  ates).... image:
+00003c40: 3a20 2e2e 2f6d 6564 6961 2f70 6c6f 745f  : ../media/plot_
+00003c50: 6869 7374 6f72 6963 616c 5f70 6f6c 6963  historical_polic
+00003c60: 795f 7261 7465 732e 706e 670a 0a45 7861  y_rates.png..Exa
+00003c70: 6d70 6c65 2035 3a20 4361 6c63 756c 6174  mple 5: Calculat
+00003c80: 6520 616e 6420 506c 6f74 2074 6865 2041  e and Plot the A
+00003c90: 646a 7573 7465 6420 4869 7374 6f72 6963  djusted Historic
+00003ca0: 616c 2050 6f6c 6963 7920 5275 6c65 730a  al Policy Rules.
+00003cb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003cc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003cd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003ce0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003cf0: 2d2d 0a0a 2e2e 2063 6f64 652d 626c 6f63  --.... code-bloc
+00003d00: 6b3a 3a20 7079 7468 6f6e 0a0a 2020 2023  k:: python..   #
+00003d10: 2049 6d70 6f72 7420 7079 6563 6f6e 6f6d   Import pyeconom
+00003d20: 6963 7320 6d6f 6475 6c65 730a 2020 2069  ics modules.   i
+00003d30: 6d70 6f72 7420 7079 6563 6f6e 6f6d 6963  mport pyeconomic
+00003d40: 7320 6173 2070 7965 636f 6e0a 0a20 2020  s as pyecon..   
+00003d50: 2320 4164 6a75 7374 6d65 6e74 2050 6172  # Adjustment Par
+00003d60: 616d 6574 6572 730a 2020 2072 686f 203d  ameters.   rho =
+00003d70: 2030 2e37 2020 2320 506f 6c69 6379 2049   0.7  # Policy I
+00003d80: 6e65 7274 6961 2043 6f65 6666 6963 6965  nertia Coefficie
+00003d90: 6e74 0a20 2020 6170 706c 795f 656c 6220  nt.   apply_elb 
+00003da0: 3d20 5472 7565 2020 2320 4170 706c 7920  = True  # Apply 
+00003db0: 4566 6665 6374 6976 6520 4c6f 7765 7220  Effective Lower 
+00003dc0: 426f 756e 640a 0a20 2020 2320 4361 6c63  Bound..   # Calc
+00003dd0: 756c 6174 6520 6164 6a75 7374 6564 2068  ulate adjusted h
+00003de0: 6973 746f 7269 6361 6c20 706f 6c69 6379  istorical policy
+00003df0: 2072 6174 6573 0a20 2020 6164 6a75 7374   rates.   adjust
+00003e00: 6564 5f68 6973 746f 7269 6361 6c5f 706f  ed_historical_po
+00003e10: 6c69 6379 5f65 7374 696d 6174 6573 203d  licy_estimates =
+00003e20: 2070 7965 636f 6e2e 6361 6c63 756c 6174   pyecon.calculat
+00003e30: 655f 6869 7374 6f72 6963 616c 5f70 6f6c  e_historical_pol
+00003e40: 6963 795f 7261 7465 7328 0a20 2020 2020  icy_rates(.     
+00003e50: 2020 7268 6f3d 7268 6f2c 0a20 2020 2020    rho=rho,.     
+00003e60: 2020 6170 706c 795f 656c 623d 6170 706c    apply_elb=appl
+00003e70: 795f 656c 620a 2020 2029 2e64 726f 706e  y_elb.   ).dropn
+00003e80: 6128 290a 0a20 2020 2320 506c 6f74 2061  a()..   # Plot a
+00003e90: 646a 7573 7465 6420 6869 7374 6f72 6963  djusted historic
+00003ea0: 616c 2070 6f6c 6963 7920 7261 7465 730a  al policy rates.
+00003eb0: 2020 2070 7965 636f 6e2e 706c 6f74 5f68     pyecon.plot_h
+00003ec0: 6973 746f 7269 6361 6c5f 7275 6c65 5f65  istorical_rule_e
+00003ed0: 7374 696d 6174 6573 280a 2020 2020 2020  stimates(.      
+00003ee0: 2061 646a 7573 7465 645f 6869 7374 6f72   adjusted_histor
+00003ef0: 6963 616c 5f70 6f6c 6963 795f 6573 7469  ical_policy_esti
+00003f00: 6d61 7465 732c 0a20 2020 2020 2020 6164  mates,.       ad
+00003f10: 6a75 7374 6564 3d54 7275 650a 2020 2029  justed=True.   )
+00003f20: 0a0a 2e2e 2069 6d61 6765 3a3a 202e 2e2f  .... image:: ../
+00003f30: 6d65 6469 612f 706c 6f74 5f61 646a 5f68  media/plot_adj_h
+00003f40: 6973 746f 7269 6361 6c5f 7261 7465 732e  istorical_rates.
+00003f50: 706e 670a 0a45 7861 6d70 6c65 730a 3d3d  png..Examples.==
+00003f60: 3d3d 3d3d 3d3d 0a0a 466f 7220 6d6f 7265  ======..For more
+00003f70: 2063 6f6d 7072 6568 656e 7369 7665 2065   comprehensive e
+00003f80: 7861 6d70 6c65 732c 2072 6566 6572 2074  xamples, refer t
+00003f90: 6f20 7468 6520 6065 7861 6d70 6c65 7320  o the `examples 
+00003fa0: 3c65 7861 6d70 6c65 733e 605f 2064 6972  <examples>`_ dir
+00003fb0: 6563 746f 7279 2069 6e0a 7468 6520 7265  ectory in.the re
+00003fc0: 706f 7369 746f 7279 2e0a 0a52 6f61 646d  pository...Roadm
+00003fd0: 6170 0a3d 3d3d 3d3d 3d3d 0a0a 5468 6520  ap.=======..The 
+00003fe0: 666f 6c6c 6f77 696e 6720 6d6f 6465 6c73  following models
+00003ff0: 2061 6e64 2063 6174 6567 6f72 6965 7320   and categories 
+00004000: 6172 6520 706c 616e 6e65 6420 666f 7220  are planned for 
+00004010: 6675 7475 7265 2064 6576 656c 6f70 6d65  future developme
+00004020: 6e74 2e0a 6043 6f6e 7472 6962 7574 696f  nt..`Contributio
+00004030: 6e73 203c 636f 6e74 7269 6275 7469 6e67  ns <contributing
+00004040: 3e60 5f20 6172 6520 7765 6c63 6f6d 6521  >`_ are welcome!
+00004050: 0a0a 2e2e 2072 7562 7269 633a 3a20 4d6f  .... rubric:: Mo
+00004060: 6e65 7461 7279 2050 6f6c 6963 7920 4d6f  netary Policy Mo
+00004070: 6465 6c73 0a0a 2d20 5461 796c 6f72 2052  dels..- Taylor R
+00004080: 756c 650a 2d20 4261 6c61 6e63 6564 2041  ule.- Balanced A
+00004090: 7070 726f 6163 6820 5275 6c65 0a2d 2046  pproach Rule.- F
+000040a0: 6972 7374 2044 6966 6665 7265 6e63 6520  irst Difference 
+000040b0: 5275 6c65 0a2d 204d 6343 616c 6c75 6d20  Rule.- McCallum 
+000040c0: 5275 6c65 0a2d 204f 7270 6861 6e69 6465  Rule.- Orphanide
+000040d0: 7320 5275 6c65 0a2d 2046 7269 6564 6d61  s Rule.- Friedma
+000040e0: 6e20 5275 6c65 0a2d 2049 6e74 6572 6573  n Rule.- Interes
+000040f0: 7420 5261 7465 2053 6d6f 6f74 6869 6e67  t Rate Smoothing
+00004100: 204d 6f64 656c 730a 0a2e 2e20 7275 6272   Models.... rubr
+00004110: 6963 3a3a 2051 7561 6e74 6974 7920 6f66  ic:: Quantity of
+00004120: 204d 6f6e 6579 2054 6865 6f72 790a 0a2d   Money Theory..-
+00004130: 2046 6973 6865 7220 4571 7561 7469 6f6e   Fisher Equation
+00004140: 0a2d 2043 616d 6272 6964 6765 2045 7175  .- Cambridge Equ
+00004150: 6174 696f 6e0a 2d20 5665 6c6f 6369 7479  ation.- Velocity
+00004160: 206f 6620 4d6f 6e65 7920 4d6f 6465 6c73   of Money Models
+00004170: 0a2d 2051 7561 6e74 6974 7920 5468 656f  .- Quantity Theo
+00004180: 7279 206f 6620 4d6f 6e65 7920 2851 544d  ry of Money (QTM
+00004190: 290a 2d20 4d6f 6e65 7920 4465 6d61 6e64  ).- Money Demand
+000041a0: 2046 756e 6374 696f 6e20 284d 6429 0a0a   Function (Md)..
+000041b0: 2e2e 2072 7562 7269 633a 3a20 4563 6f6e  .. rubric:: Econ
+000041c0: 6f6d 6963 204d 6f64 656c 7320 746f 2050  omic Models to P
+000041d0: 7265 6469 6374 2046 7574 7572 6520 4578  redict Future Ex
+000041e0: 6368 616e 6765 2052 6174 6573 0a0a 2d20  change Rates..- 
+000041f0: 5075 7263 6861 7369 6e67 2050 6f77 6572  Purchasing Power
+00004200: 2050 6172 6974 7920 2850 5050 290a 2d20   Parity (PPP).- 
+00004210: 496e 7465 7265 7374 2052 6174 6520 5061  Interest Rate Pa
+00004220: 7269 7479 2028 4952 5029 0a2d 204d 6f6e  rity (IRP).- Mon
+00004230: 6574 6172 7920 4d6f 6465 6c73 206f 6620  etary Models of 
+00004240: 4578 6368 616e 6765 2052 6174 6573 0a2d  Exchange Rates.-
+00004250: 2050 6f72 7466 6f6c 696f 2042 616c 616e   Portfolio Balan
+00004260: 6365 204d 6f64 656c 730a 2d20 4265 6861  ce Models.- Beha
+00004270: 7669 6f72 616c 2045 7175 696c 6962 7269  vioral Equilibri
+00004280: 756d 2045 7863 6861 6e67 6520 5261 7465  um Exchange Rate
+00004290: 2028 4245 4552 290a 2d20 4675 6e64 616d   (BEER).- Fundam
+000042a0: 656e 7461 6c20 4571 7569 6c69 6272 6975  ental Equilibriu
+000042b0: 6d20 4578 6368 616e 6765 2052 6174 6520  m Exchange Rate 
+000042c0: 2846 4545 5229 0a0a 2e2e 2072 7562 7269  (FEER).... rubri
+000042d0: 633a 3a20 4d61 6372 6f65 636f 6e6f 6d69  c:: Macroeconomi
+000042e0: 6320 4d6f 6465 6c73 0a0a 2d20 4953 2d4c  c Models..- IS-L
+000042f0: 4d20 4d6f 6465 6c0a 2d20 4144 2d41 5320  M Model.- AD-AS 
+00004300: 4d6f 6465 6c0a 2d20 536f 6c6f 7720 4772  Model.- Solow Gr
+00004310: 6f77 7468 204d 6f64 656c 0a2d 204e 6577  owth Model.- New
+00004320: 204b 6579 6e65 7369 616e 204d 6f64 656c   Keynesian Model
+00004330: 730a 2d20 5242 4320 2852 6561 6c20 4275  s.- RBC (Real Bu
+00004340: 7369 6e65 7373 2043 7963 6c65 2920 4d6f  siness Cycle) Mo
+00004350: 6465 6c0a 2d20 4453 4745 2028 4479 6e61  del.- DSGE (Dyna
+00004360: 6d69 6320 5374 6f63 6861 7374 6963 2047  mic Stochastic G
+00004370: 656e 6572 616c 2045 7175 696c 6962 7269  eneral Equilibri
+00004380: 756d 2920 4d6f 6465 6c73 0a0a 2e2e 2072  um) Models.... r
+00004390: 7562 7269 633a 3a20 4d69 6372 6f65 636f  ubric:: Microeco
+000043a0: 6e6f 6d69 6320 4d6f 6465 6c73 0a0a 2d20  nomic Models..- 
+000043b0: 5375 7070 6c79 2061 6e64 2044 656d 616e  Supply and Deman
+000043c0: 6420 4d6f 6465 6c73 0a2d 2043 6f6e 7375  d Models.- Consu
+000043d0: 6d65 7220 4368 6f69 6365 2054 6865 6f72  mer Choice Theor
+000043e0: 790a 2d20 5072 6f64 7563 7469 6f6e 2054  y.- Production T
+000043f0: 6865 6f72 790a 2d20 436f 7374 2046 756e  heory.- Cost Fun
+00004400: 6374 696f 6e73 0a2d 2047 616d 6520 5468  ctions.- Game Th
+00004410: 656f 7279 204d 6f64 656c 730a 2d20 4d61  eory Models.- Ma
+00004420: 726b 6574 2053 7472 7563 7475 7265 204d  rket Structure M
+00004430: 6f64 656c 7320 2850 6572 6665 6374 2043  odels (Perfect C
+00004440: 6f6d 7065 7469 7469 6f6e 2c20 4d6f 6e6f  ompetition, Mono
+00004450: 706f 6c79 2c20 4f6c 6967 6f70 6f6c 7929  poly, Oligopoly)
+00004460: 0a0a 2e2e 2072 7562 7269 633a 3a20 4469  .... rubric:: Di
+00004470: 7363 6f75 6e74 6564 2043 6173 6820 466c  scounted Cash Fl
+00004480: 6f77 204d 6f64 656c 730a 0a2d 2044 6976  ow Models..- Div
+00004490: 6964 656e 6420 4469 7363 6f75 6e74 204d  idend Discount M
+000044a0: 6f64 656c 2028 4444 4d29 0a2d 2046 7265  odel (DDM).- Fre
+000044b0: 6520 4361 7368 2046 6c6f 7720 746f 2045  e Cash Flow to E
+000044c0: 7175 6974 7920 2846 4346 4529 0a2d 2046  quity (FCFE).- F
+000044d0: 7265 6520 4361 7368 2046 6c6f 7720 746f  ree Cash Flow to
+000044e0: 2046 6972 6d20 2846 4346 4629 0a2d 204e   Firm (FCFF).- N
+000044f0: 6574 2050 7265 7365 6e74 2056 616c 7565  et Present Value
+00004500: 2028 4e50 5629 0a2d 2049 6e74 6572 6e61   (NPV).- Interna
+00004510: 6c20 5261 7465 206f 6620 5265 7475 726e  l Rate of Return
+00004520: 2028 4952 5229 0a2d 2041 646a 7573 7465   (IRR).- Adjuste
+00004530: 6420 5072 6573 656e 7420 5661 6c75 6520  d Present Value 
+00004540: 2841 5056 290a 0a2e 2e20 7275 6272 6963  (APV).... rubric
+00004550: 3a3a 2046 696e 616e 6369 616c 204d 6f64  :: Financial Mod
+00004560: 656c 730a 0a2d 2043 6170 6974 616c 2041  els..- Capital A
+00004570: 7373 6574 2050 7269 6369 6e67 204d 6f64  sset Pricing Mod
+00004580: 656c 2028 4341 504d 290a 2d20 4172 6269  el (CAPM).- Arbi
+00004590: 7472 6167 6520 5072 6963 696e 6720 5468  trage Pricing Th
+000045a0: 656f 7279 2028 4150 5429 0a2d 2042 6c61  eory (APT).- Bla
+000045b0: 636b 2d53 6368 6f6c 6573 204f 7074 696f  ck-Scholes Optio
+000045c0: 6e20 5072 6963 696e 6720 4d6f 6465 6c0a  n Pricing Model.
+000045d0: 2d20 426f 6e64 2056 616c 7561 7469 6f6e  - Bond Valuation
+000045e0: 204d 6f64 656c 730a 2d20 4372 6564 6974   Models.- Credit
+000045f0: 2052 6973 6b20 4d6f 6465 6c73 2028 652e   Risk Models (e.
+00004600: 672e 2c20 4d65 7274 6f6e 204d 6f64 656c  g., Merton Model
+00004610: 290a 2d20 506f 7274 666f 6c69 6f20 4f70  ).- Portfolio Op
+00004620: 7469 6d69 7a61 7469 6f6e 204d 6f64 656c  timization Model
+00004630: 7320 2865 2e67 2e2c 204d 6172 6b6f 7769  s (e.g., Markowi
+00004640: 747a 204d 6f64 656c 290a 0a2e 2e20 7275  tz Model).... ru
+00004650: 6272 6963 3a3a 2046 6973 6361 6c20 506f  bric:: Fiscal Po
+00004660: 6c69 6379 204d 6f64 656c 730a 0a2d 2054  licy Models..- T
+00004670: 6178 6174 696f 6e20 616e 6420 476f 7665  axation and Gove
+00004680: 726e 6d65 6e74 2053 7065 6e64 696e 6720  rnment Spending 
+00004690: 4d6f 6465 6c73 0a2d 2042 7564 6765 7420  Models.- Budget 
+000046a0: 4465 6669 6369 7420 4d6f 6465 6c73 0a2d  Deficit Models.-
+000046b0: 2050 7562 6c69 6320 4465 6274 204d 6f64   Public Debt Mod
+000046c0: 656c 730a 2d20 4669 7363 616c 204d 756c  els.- Fiscal Mul
+000046d0: 7469 706c 6965 7220 4d6f 6465 6c73 0a2d  tiplier Models.-
+000046e0: 204c 6166 6665 7220 4375 7276 650a 2d20   Laffer Curve.- 
+000046f0: 5269 6361 7264 6961 6e20 4571 7569 7661  Ricardian Equiva
+00004700: 6c65 6e63 650a 0a2e 2e20 7275 6272 6963  lence.... rubric
+00004710: 3a3a 204f 7468 6572 2057 656c 6c2d 4b6e  :: Other Well-Kn
+00004720: 6f77 6e20 4563 6f6e 6f6d 6963 204d 6f64  own Economic Mod
+00004730: 656c 730a 0a2d 2042 6568 6176 696f 7261  els..- Behaviora
+00004740: 6c20 4563 6f6e 6f6d 6963 7320 4d6f 6465  l Economics Mode
+00004750: 6c73 0a2d 2041 6765 6e74 2d42 6173 6564  ls.- Agent-Based
+00004760: 204d 6f64 656c 730a 2d20 456e 7669 726f   Models.- Enviro
+00004770: 6e6d 656e 7461 6c20 4563 6f6e 6f6d 6963  nmental Economic
+00004780: 7320 4d6f 6465 6c73 0a2d 2049 6e74 6572  s Models.- Inter
+00004790: 6e61 7469 6f6e 616c 2054 7261 6465 204d  national Trade M
+000047a0: 6f64 656c 7320 2865 2e67 2e2c 2048 6563  odels (e.g., Hec
+000047b0: 6b73 6368 6572 2d4f 686c 696e 204d 6f64  kscher-Ohlin Mod
+000047c0: 656c 290a 2d20 4c61 626f 7220 4d61 726b  el).- Labor Mark
+000047d0: 6574 204d 6f64 656c 730a 2d20 4865 616c  et Models.- Heal
+000047e0: 7468 2045 636f 6e6f 6d69 6373 204d 6f64  th Economics Mod
+000047f0: 656c 730a 0a43 6f6e 7472 6962 7574 696e  els..Contributin
+00004800: 670a 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a  g.============..
+00004810: 436f 6e74 7269 6275 7469 6f6e 7320 6172  Contributions ar
+00004820: 6520 7765 6c63 6f6d 6521 2049 6620 796f  e welcome! If yo
+00004830: 7520 6861 7665 2061 206d 6f64 656c 2079  u have a model y
+00004840: 6f75 2764 206c 696b 6520 746f 2069 6d70  ou'd like to imp
+00004850: 6c65 6d65 6e74 206f 7220 616e 0a69 6d70  lement or an.imp
+00004860: 726f 7665 6d65 6e74 2074 6f20 616e 2065  rovement to an e
+00004870: 7869 7374 696e 6720 6d6f 6465 6c2c 2070  xisting model, p
+00004880: 6c65 6173 6520 7265 6665 7220 746f 206f  lease refer to o
+00004890: 7572 2064 6574 6169 6c65 640a 6043 6f6e  ur detailed.`Con
+000048a0: 7472 6962 7574 696e 6720 4775 6964 6520  tributing Guide 
+000048b0: 3c6d 6172 6b64 6f77 6e2f 434f 4e54 5249  <markdown/CONTRI
+000048c0: 4255 5449 4e47 2e6d 643e 605f 2e0a 0a42  BUTING.md>`_...B
+000048d0: 7920 7061 7274 6963 6970 6174 696e 6720  y participating 
+000048e0: 696e 2074 6869 7320 7072 6f6a 6563 742c  in this project,
+000048f0: 2079 6f75 2061 6772 6565 2074 6f20 6162   you agree to ab
+00004900: 6964 6520 6279 2074 6865 0a60 436f 6465  ide by the.`Code
+00004910: 206f 6620 436f 6e64 7563 7420 3c6d 6172   of Conduct <mar
+00004920: 6b64 6f77 6e2f 434f 4445 5f4f 465f 434f  kdown/CODE_OF_CO
+00004930: 4e44 5543 542e 6d64 3e60 5f2e 0a0a 5468  NDUCT.md>`_...Th
+00004940: 616e 6b20 796f 7520 666f 7220 796f 7572  ank you for your
+00004950: 2063 6f6e 7472 6962 7574 696f 6e73 210a   contributions!.
+00004960: 0a43 6f6e 7461 6374 0a3d 3d3d 3d3d 3d3d  .Contact.=======
+00004970: 0a0a 4966 2079 6f75 2068 6176 6520 616e  ..If you have an
+00004980: 7920 7175 6573 7469 6f6e 732c 2073 7567  y questions, sug
+00004990: 6765 7374 696f 6e73 2c20 6f72 206e 6565  gestions, or nee
+000049a0: 6420 7375 7070 6f72 742c 2066 6565 6c20  d support, feel 
+000049b0: 6672 6565 2074 6f20 7265 6163 6820 6f75  free to reach ou
+000049c0: 742e 0a0a 4e61 7468 616e 2052 616d 6f73  t...Nathan Ramos
+000049d0: 2c20 4346 410a 2d2d 2d2d 2d2d 2d2d 2d2d  , CFA.----------
+000049e0: 2d2d 2d2d 2d2d 2d0a 0a57 656c 636f 6d65  -------..Welcome
+000049f0: 2074 6f20 6d79 2047 6974 4875 6221 2049   to my GitHub! I
+00004a00: 276d 204e 6174 6861 6e2c 2061 6e20 696e  'm Nathan, an in
+00004a10: 6465 7065 6e64 656e 7420 4669 6e74 6563  dependent Fintec
+00004a20: 6820 4465 7665 6c6f 7065 7220 7769 7468  h Developer with
+00004a30: 2061 0a43 6861 7274 6572 6564 2046 696e   a.Chartered Fin
+00004a40: 616e 6369 616c 2041 6e61 6c79 7374 2028  ancial Analyst (
+00004a50: 4346 4129 2064 6573 6967 6e61 7469 6f6e  CFA) designation
+00004a60: 2c20 7370 6563 6961 6c69 7a69 6e67 2069  , specializing i
+00004a70: 6e20 5079 7468 6f6e 2d62 6173 6564 0a66  n Python-based.f
+00004a80: 696e 616e 6369 616c 2061 6e61 6c79 7369  inancial analysi
+00004a90: 732c 2071 7561 6e74 6974 6174 6976 6520  s, quantitative 
+00004aa0: 7374 7261 7465 6769 6573 2c20 616e 6420  strategies, and 
+00004ab0: 6175 746f 6d61 7465 6420 7472 6164 696e  automated tradin
+00004ac0: 6720 7072 6f67 7261 6d73 2e0a 4375 7272  g programs..Curr
+00004ad0: 656e 746c 792c 2049 276d 2061 2066 696e  ently, I'm a fin
+00004ae0: 7465 6368 2063 6f6e 7375 6c74 616e 7420  tech consultant 
+00004af0: 6f70 656e 2074 6f20 6e65 7720 636c 6965  open to new clie
+00004b00: 6e74 732e 2053 6368 6564 756c 6520 6120  nts. Schedule a 
+00004b10: 6d65 6574 696e 670a 7769 7468 206d 6520  meeting.with me 
+00004b20: 746f 2064 6973 6375 7373 2063 6f6c 6c61  to discuss colla
+00004b30: 626f 7261 7469 6e67 206f 6e20 796f 7572  borating on your
+00004b40: 206e 6578 7420 7072 6f6a 6563 7420 6f72   next project or
+00004b50: 2074 6f20 6c65 6172 6e20 6d6f 7265 2061   to learn more a
+00004b60: 626f 7574 0a6d 7920 7365 7276 6963 6573  bout.my services
+00004b70: 2e0a 0af0 9f93 8520 6053 6368 6564 756c  ....... `Schedul
+00004b80: 6520 6120 4d65 6574 696e 6720 7769 7468  e a Meeting with
+00004b90: 204d 6520 3c68 7474 7073 3a2f 2f63 616c   Me <https://cal
+00004ba0: 656e 646c 792e 636f 6d2f 6e72 6361 7069  endly.com/nrcapi
+00004bb0: 7461 6c6d 616e 6167 656d 656e 742f 6769  talmanagement/gi
+00004bc0: 7468 7562 2d6d 6565 7469 6e67 3e60 5f0a  thub-meeting>`_.
+00004bd0: 0a43 6f6e 6e65 6374 2077 6974 6820 4d65  .Connect with Me
+00004be0: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .---------------
+00004bf0: 0a0a 2d20 2a2a 456d 6169 6c2a 2a3a 2060  ..- **Email**: `
+00004c00: 6e61 7468 616e 2e72 616d 6f73 2e67 6974  nathan.ramos.git
+00004c10: 6875 6240 676d 6169 6c2e 636f 6d20 3c6d  hub@gmail.com <m
+00004c20: 6169 6c74 6f3a 6e61 7468 616e 2e72 616d  ailto:nathan.ram
+00004c30: 6f73 2e67 6974 6875 6240 676d 6169 6c2e  os.github@gmail.
+00004c40: 636f 6d3e 605f 0a2d 202a 2a54 7769 7474  com>`_.- **Twitt
+00004c50: 6572 2a2a 3a20 6040 6e61 7468 616e 7261  er**: `@nathanra
+00004c60: 6d6f 7363 6661 203c 6874 7470 733a 2f2f  moscfa <https://
+00004c70: 7477 6974 7465 722e 636f 6d2f 6e61 7468  twitter.com/nath
+00004c80: 616e 7261 6d6f 7363 6661 3e60 5f0a 0a46  anramoscfa>`_..F
+00004c90: 6565 6c20 6672 6565 2074 6f20 636f 6e6e  eel free to conn
+00004ca0: 6563 7420 7769 7468 206d 6520 666f 7220  ect with me for 
+00004cb0: 616e 7920 696e 7175 6972 6965 7320 6f72  any inquiries or
+00004cc0: 2063 6f6c 6c61 626f 7261 7469 6f6e 206f   collaboration o
+00004cd0: 7070 6f72 7475 6e69 7469 6573 2e0a 0a49  pportunities...I
+00004ce0: 6e64 6963 6573 2061 6e64 2074 6162 6c65  ndices and table
+00004cf0: 730a 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  s.==============
+00004d00: 3d3d 3d3d 0a0a 2a20 3a72 6566 3a60 6765  ====..* :ref:`ge
+00004d10: 6e69 6e64 6578 600a 2a20 3a72 6566 3a60  nindex`.* :ref:`
+00004d20: 6d6f 6469 6e64 6578 600a 2a20 3a72 6566  modindex`.* :ref
+00004d30: 3a60 7365 6172 6368 600a                 :`search`.
```

### Comparing `pyeconomics-0.2.3/docs/introduction.rst` & `pyeconomics-0.2.4/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/docs/make.bat` & `pyeconomics-0.2.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/docs/usage.rst` & `pyeconomics-0.2.4/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/examples/api_configuration/fred_api_configuration.ipynb` & `pyeconomics-0.2.4/examples/api_configuration/fred_api_configuration.ipynb`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/examples/monetary_policy_rules/balanced_approach_rule.ipynb` & `pyeconomics-0.2.4/examples/monetary_policy_rules/balanced_approach_rule.ipynb`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/examples/monetary_policy_rules/first_difference_rule.ipynb` & `pyeconomics-0.2.4/examples/monetary_policy_rules/first_difference_rule.ipynb`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/examples/monetary_policy_rules/monetary_policy_rules.ipynb` & `pyeconomics-0.2.4/examples/monetary_policy_rules/monetary_policy_rules.ipynb`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/examples/monetary_policy_rules/taylor_rule.ipynb` & `pyeconomics-0.2.4/examples/monetary_policy_rules/taylor_rule.ipynb`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/markdown/CHANGELOG.md` & `pyeconomics-0.2.4/markdown/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/markdown/CODE_OF_CONDUCT.md` & `pyeconomics-0.2.4/markdown/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/markdown/CONTRIBUTING.md` & `pyeconomics-0.2.4/markdown/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/markdown/FRED_API_CONFIGURATION.md` & `pyeconomics-0.2.4/markdown/FRED_API_CONFIGURATION.md`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/media/plot_adj_historical_rates.png` & `pyeconomics-0.2.4/media/plot_adj_historical_rates.png`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/media/plot_historical_policy_rates.png` & `pyeconomics-0.2.4/media/plot_historical_policy_rates.png`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/pyeconomics/__init__.py` & `pyeconomics-0.2.4/pyeconomics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/pyeconomics/api/cache_manager.py` & `pyeconomics-0.2.4/pyeconomics/api/cache_manager.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/pyeconomics/api/fred_api.py` & `pyeconomics-0.2.4/pyeconomics/api/fred_api.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/pyeconomics/api/fred_data.py` & `pyeconomics-0.2.4/pyeconomics/api/fred_data.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/pyeconomics/data/economic_indicators.py` & `pyeconomics-0.2.4/pyeconomics/data/economic_indicators.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/pyeconomics/data/model_parameters.py` & `pyeconomics-0.2.4/pyeconomics/data/model_parameters.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/pyeconomics/models/monetary_policy/__init__.py` & `pyeconomics-0.2.4/pyeconomics/models/monetary_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/pyeconomics/models/monetary_policy/balanced_approach_rule.py` & `pyeconomics-0.2.4/pyeconomics/models/monetary_policy/balanced_approach_rule.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/pyeconomics/models/monetary_policy/first_difference_rule.py` & `pyeconomics-0.2.4/pyeconomics/models/monetary_policy/first_difference_rule.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/pyeconomics/models/monetary_policy/monetary_policy_rules.py` & `pyeconomics-0.2.4/pyeconomics/models/monetary_policy/monetary_policy_rules.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/pyeconomics/models/monetary_policy/taylor_rule.py` & `pyeconomics-0.2.4/pyeconomics/models/monetary_policy/taylor_rule.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/pyeconomics/utils/bar_utils.py` & `pyeconomics-0.2.4/pyeconomics/utils/bar_utils.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/pyeconomics/utils/fdr_utils.py` & `pyeconomics-0.2.4/pyeconomics/utils/fdr_utils.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/pyeconomics/utils/tr_utils.py` & `pyeconomics-0.2.4/pyeconomics/utils/tr_utils.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/pyeconomics.egg-info/PKG-INFO` & `pyeconomics-0.2.4/pyeconomics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyeconomics
-Version: 0.2.3
+Version: 0.2.4
 Summary: A library for economic and financial analysis
 Home-page: https://github.com/nathanramoscfa/pyeconomics
 Author: Nathan Ramos, CFA
 Author-email: nathan.ramos.github@gmail.com
 Project-URL: Bug Reports, https://github.com/nathanramoscfa/pyeconomics/issues
 Project-URL: Source, https://github.com/nathanramoscfa/pyeconomics
 Classifier: Development Status :: 3 - Alpha
@@ -145,15 +145,15 @@
 
 # Calculate policy rule estimates
 policy_estimates = pyecon.calculate_policy_rule_estimates(verbose=True)
 ```
 
 Verbose Print Statement:
 
-```text
+<pre>
 ┌───────────────────────────────────────────────────────────────────────────────────┐
 │                           Interest Rate Policy Estimates                          │
 ├───────────────────────────────────────────────────────────────────────────────────┤
 │ Taylor Rule (TR)                                                      6.17%       │
 │ Balanced Approach Rule (BAR)                                          6.68%       │
 │ Balanced Approach Shortfalls Rule (BASR)                              5.66%       │
 │ First Difference Rule (FDR)                                           5.97%       │
@@ -165,15 +165,15 @@
 │                                Policy Prescription                                │
 ├───────────────────────────────────────────────────────────────────────────────────┤
 │ Taylor Rule (TR) suggests raising the rate by 0.75%.                              │
 │ Balanced Approach Rule (BAR) suggests raising the rate by 1.25%.                  │
 │ Balanced Approach Shortfalls Rule (BASR) suggests raising the rate by 0.25%.      │
 │ First Difference Rule (FDR) suggests raising the rate by 0.50%.                   │
 └───────────────────────────────────────────────────────────────────────────────────┘
-```
+</pre>
 
 ### Example 2: Adjust Taylor Rule for Effective Lower Bound (ELB) and Policy Inertia
 
 ```python
 # Import pyeconomics
 import pyeconomics as pyecon
 
@@ -186,15 +186,15 @@
     apply_elb=apply_elb,
     verbose=True
 )
 ```
 
 Verbose Print Statement:
 
-```text
+<pre>
 ┌───────────────────────────────────────────────────────────────────────────────────┐
 │                      Adjusted Interest Rate Policy Estimates                      │
 ├───────────────────────────────────────────────────────────────────────────────────┤
 │ Taylor Rule (TR)                                                      5.70%       │
 │ Balanced Approach Rule (BAR)                                          5.86%       │
 │ Balanced Approach Shortfalls Rule (BASR)                              5.55%       │
 │ First Difference Rule (FDR)                                           5.64%       │
@@ -206,15 +206,15 @@
 │                            Adjusted Policy Prescription                           │
 ├───────────────────────────────────────────────────────────────────────────────────┤
 │ Taylor Rule (TR) suggests raising the rate by 0.25%.                              │
 │ Balanced Approach Rule (BAR) suggests raising the rate by 0.25%.                  │
 │ Balanced Approach Shortfalls Rule (BASR) suggests maintaining the current rate.   │
 │ First Difference Rule (FDR) suggests raising the rate by 0.25%.                   │
 └───────────────────────────────────────────────────────────────────────────────────┘
-```
+</pre>
 
 ### Example 3: Calculate Current Taylor Rule Estimates
 
 ```python
 # Import pyeconomics modules
 import pyeconomics as pyecon
```

### Comparing `pyeconomics-0.2.3/pyeconomics.egg-info/SOURCES.txt` & `pyeconomics-0.2.4/pyeconomics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/setup.py` & `pyeconomics-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/tests/conftest.py` & `pyeconomics-0.2.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/tests/test_balanced_approach_rule.py` & `pyeconomics-0.2.4/tests/test_balanced_approach_rule.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/tests/test_bar_utils.py` & `pyeconomics-0.2.4/tests/test_bar_utils.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/tests/test_cache_manager.py` & `pyeconomics-0.2.4/tests/test_cache_manager.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/tests/test_fdr_utils.py` & `pyeconomics-0.2.4/tests/test_fdr_utils.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/tests/test_first_difference_rule.py` & `pyeconomics-0.2.4/tests/test_first_difference_rule.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/tests/test_fred_api.py` & `pyeconomics-0.2.4/tests/test_fred_api.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/tests/test_fred_data.py` & `pyeconomics-0.2.4/tests/test_fred_data.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/tests/test_monetary_policy_rules.py` & `pyeconomics-0.2.4/tests/test_monetary_policy_rules.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/tests/test_taylor_rule.py` & `pyeconomics-0.2.4/tests/test_taylor_rule.py`

 * *Files identical despite different names*

### Comparing `pyeconomics-0.2.3/tests/test_tr_utils.py` & `pyeconomics-0.2.4/tests/test_tr_utils.py`

 * *Files identical despite different names*

