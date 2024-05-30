# Comparing `tmp/nested_pandas-0.1.tar.gz` & `tmp/nested_pandas-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nested_pandas-0.1.tar", last modified: Fri May 17 22:11:48 2024, max compression
+gzip compressed data, was "nested_pandas-0.1.1.tar", last modified: Thu May 30 21:37:07 2024, max compression
```

## Comparing `nested_pandas-0.1.tar` & `nested_pandas-0.1.1.tar`

### file list

```diff
@@ -1,98 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:48.400506 nested_pandas-0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-17 22:11:43.000000 nested_pandas-0.1/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-17 22:11:43.000000 nested_pandas-0.1/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-17 22:11:43.000000 nested_pandas-0.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:48.388506 nested_pandas-0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:48.388506 nested_pandas-0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-17 22:11:43.000000 nested_pandas-0.1/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-17 22:11:43.000000 nested_pandas-0.1/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-17 22:11:43.000000 nested_pandas-0.1/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-17 22:11:43.000000 nested_pandas-0.1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-17 22:11:43.000000 nested_pandas-0.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:48.392506 nested_pandas-0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-17 22:11:43.000000 nested_pandas-0.1/.github/workflows/asv-main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-17 22:11:43.000000 nested_pandas-0.1/.github/workflows/asv-nightly.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-05-17 22:11:43.000000 nested_pandas-0.1/.github/workflows/asv-pr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-17 22:11:43.000000 nested_pandas-0.1/.github/workflows/build-documentation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-17 22:11:43.000000 nested_pandas-0.1/.github/workflows/pre-commit-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-17 22:11:43.000000 nested_pandas-0.1/.github/workflows/publish-benchmarks-pr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-17 22:11:43.000000 nested_pandas-0.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-17 22:11:43.000000 nested_pandas-0.1/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-17 22:11:43.000000 nested_pandas-0.1/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-17 22:11:43.000000 nested_pandas-0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-05-17 22:11:43.000000 nested_pandas-0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-17 22:11:43.000000 nested_pandas-0.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-17 22:11:43.000000 nested_pandas-0.1/.setup_dev.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-17 22:11:43.000000 nested_pandas-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-05-17 22:11:48.400506 nested_pandas-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-17 22:11:43.000000 nested_pandas-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:48.392506 nested_pandas-0.1/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:43.000000 nested_pandas-0.1/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-05-17 22:11:43.000000 nested_pandas-0.1/benchmarks/asv.conf.json
--rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-05-17 22:11:43.000000 nested_pandas-0.1/benchmarks/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:48.392506 nested_pandas-0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-17 22:11:43.000000 nested_pandas-0.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:48.392506 nested_pandas-0.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-17 22:11:43.000000 nested_pandas-0.1/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-17 22:11:43.000000 nested_pandas-0.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:48.392506 nested_pandas-0.1/docs/gettingstarted/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-17 22:11:43.000000 nested_pandas-0.1/docs/gettingstarted/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-17 22:11:43.000000 nested_pandas-0.1/docs/gettingstarted/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6213 2024-05-17 22:11:43.000000 nested_pandas-0.1/docs/gettingstarted/quickstart.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-17 22:11:43.000000 nested_pandas-0.1/docs/gettingstarted.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-17 22:11:43.000000 nested_pandas-0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-17 22:11:43.000000 nested_pandas-0.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:48.392506 nested_pandas-0.1/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-17 22:11:43.000000 nested_pandas-0.1/docs/tutorials/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    10299 2024-05-17 22:11:43.000000 nested_pandas-0.1/docs/tutorials/data_loading_notebook.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    22558 2024-05-17 22:11:43.000000 nested_pandas-0.1/docs/tutorials/low_level.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-17 22:11:43.000000 nested_pandas-0.1/docs/tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (127)    80633 2024-05-17 22:11:43.000000 nested_pandas-0.1/nestedframe.png
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-17 22:11:43.000000 nested_pandas-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 22:11:48.400506 nested_pandas-0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:48.384506 nested_pandas-0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:48.396506 nested_pandas-0.1/src/nested_pandas/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-17 22:11:43.000000 nested_pandas-0.1/src/nested_pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-17 22:11:48.000000 nested_pandas-0.1/src/nested_pandas/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:48.396506 nested_pandas-0.1/src/nested_pandas/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-17 22:11:43.000000 nested_pandas-0.1/src/nested_pandas/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-17 22:11:43.000000 nested_pandas-0.1/src/nested_pandas/datasets/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-17 22:11:43.000000 nested_pandas-0.1/src/nested_pandas/example_benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:48.396506 nested_pandas-0.1/src/nested_pandas/nestedframe/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-17 22:11:43.000000 nested_pandas-0.1/src/nested_pandas/nestedframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19997 2024-05-17 22:11:43.000000 nested_pandas-0.1/src/nested_pandas/nestedframe/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-17 22:11:43.000000 nested_pandas-0.1/src/nested_pandas/nestedframe/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-17 22:11:43.000000 nested_pandas-0.1/src/nested_pandas/nestedframe/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:43.000000 nested_pandas-0.1/src/nested_pandas/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:48.396506 nested_pandas-0.1/src/nested_pandas/series/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:43.000000 nested_pandas-0.1/src/nested_pandas/series/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9403 2024-05-17 22:11:43.000000 nested_pandas-0.1/src/nested_pandas/series/accessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7921 2024-05-17 22:11:43.000000 nested_pandas-0.1/src/nested_pandas/series/dtype.py
--rw-r--r--   0 runner    (1001) docker     (127)    28917 2024-05-17 22:11:43.000000 nested_pandas-0.1/src/nested_pandas/series/ext_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     9689 2024-05-17 22:11:43.000000 nested_pandas-0.1/src/nested_pandas/series/packer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-17 22:11:43.000000 nested_pandas-0.1/src/nested_pandas/series/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:48.396506 nested_pandas-0.1/src/nested_pandas/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-17 22:11:43.000000 nested_pandas-0.1/src/nested_pandas/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-17 22:11:43.000000 nested_pandas-0.1/src/nested_pandas/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:48.400506 nested_pandas-0.1/src/nested_pandas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-05-17 22:11:48.000000 nested_pandas-0.1/src/nested_pandas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-05-17 22:11:48.000000 nested_pandas-0.1/src/nested_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 22:11:48.000000 nested_pandas-0.1/src/nested_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-17 22:11:48.000000 nested_pandas-0.1/src/nested_pandas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-17 22:11:48.000000 nested_pandas-0.1/src/nested_pandas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:48.388506 nested_pandas-0.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:48.400506 nested_pandas-0.1/tests/nested_pandas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:43.000000 nested_pandas-0.1/tests/nested_pandas/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:48.400506 nested_pandas-0.1/tests/nested_pandas/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-17 22:11:43.000000 nested_pandas-0.1/tests/nested_pandas/datasets/test_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:48.400506 nested_pandas-0.1/tests/nested_pandas/nestedframe/
--rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-05-17 22:11:43.000000 nested_pandas-0.1/tests/nested_pandas/nestedframe/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)    11450 2024-05-17 22:11:43.000000 nested_pandas-0.1/tests/nested_pandas/nestedframe/test_nestedframe.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-17 22:11:43.000000 nested_pandas-0.1/tests/nested_pandas/nestedframe/test_nestedframe_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:48.400506 nested_pandas-0.1/tests/nested_pandas/series/
--rw-r--r--   0 runner    (1001) docker     (127)    20676 2024-05-17 22:11:43.000000 nested_pandas-0.1/tests/nested_pandas/series/test_accessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-05-17 22:11:43.000000 nested_pandas-0.1/tests/nested_pandas/series/test_dtype.py
--rw-r--r--   0 runner    (1001) docker     (127)    55014 2024-05-17 22:11:43.000000 nested_pandas-0.1/tests/nested_pandas/series/test_ext_array.py
--rw-r--r--   0 runner    (1001) docker     (127)    11656 2024-05-17 22:11:43.000000 nested_pandas-0.1/tests/nested_pandas/series/test_packer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 22:11:48.400506 nested_pandas-0.1/tests/nested_pandas/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-17 22:11:43.000000 nested_pandas-0.1/tests/nested_pandas/utils/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:37:07.853983 nested_pandas-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:37:07.841983 nested_pandas-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:37:07.841983 nested_pandas-0.1.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:37:07.841983 nested_pandas-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/.github/workflows/asv-main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/.github/workflows/asv-nightly.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/.github/workflows/asv-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/.github/workflows/build-documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/.github/workflows/pre-commit-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/.github/workflows/publish-benchmarks-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/.setup_dev.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-05-30 21:37:07.853983 nested_pandas-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:37:07.841983 nested_pandas-0.1.1/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/benchmarks/asv.conf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/benchmarks/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:37:07.845983 nested_pandas-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:37:07.845983 nested_pandas-0.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:37:07.845983 nested_pandas-0.1.1/docs/gettingstarted/
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/docs/gettingstarted/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/docs/gettingstarted/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6213 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/docs/gettingstarted/quickstart.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/docs/gettingstarted.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:37:07.845983 nested_pandas-0.1.1/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/docs/tutorials/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10299 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/docs/tutorials/data_loading_notebook.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    20291 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/docs/tutorials/low_level.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/docs/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    80633 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/nestedframe.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 21:37:07.853983 nested_pandas-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:37:07.837983 nested_pandas-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:37:07.845983 nested_pandas-0.1.1/src/nested_pandas/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/src/nested_pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-30 21:37:07.000000 nested_pandas-0.1.1/src/nested_pandas/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:37:07.845983 nested_pandas-0.1.1/src/nested_pandas/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/src/nested_pandas/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/src/nested_pandas/datasets/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/src/nested_pandas/example_benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:37:07.849983 nested_pandas-0.1.1/src/nested_pandas/nestedframe/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/src/nested_pandas/nestedframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19091 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/src/nested_pandas/nestedframe/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/src/nested_pandas/nestedframe/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/src/nested_pandas/nestedframe/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/src/nested_pandas/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:37:07.849983 nested_pandas-0.1.1/src/nested_pandas/series/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/src/nested_pandas/series/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/src/nested_pandas/series/accessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7921 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/src/nested_pandas/series/dtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33766 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/src/nested_pandas/series/ext_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9762 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/src/nested_pandas/series/packer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/src/nested_pandas/series/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:37:07.849983 nested_pandas-0.1.1/src/nested_pandas/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/src/nested_pandas/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/src/nested_pandas/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:37:07.853983 nested_pandas-0.1.1/src/nested_pandas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-05-30 21:37:07.000000 nested_pandas-0.1.1/src/nested_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-30 21:37:07.000000 nested_pandas-0.1.1/src/nested_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 21:37:07.000000 nested_pandas-0.1.1/src/nested_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-30 21:37:07.000000 nested_pandas-0.1.1/src/nested_pandas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-30 21:37:07.000000 nested_pandas-0.1.1/src/nested_pandas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:37:07.837983 nested_pandas-0.1.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:37:07.849983 nested_pandas-0.1.1/tests/nested_pandas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/tests/nested_pandas/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:37:07.849983 nested_pandas-0.1.1/tests/nested_pandas/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/tests/nested_pandas/datasets/test_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:37:07.849983 nested_pandas-0.1.1/tests/nested_pandas/e2e_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/tests/nested_pandas/e2e_tests/test_issue89.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:37:07.849983 nested_pandas-0.1.1/tests/nested_pandas/nestedframe/
+-rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/tests/nested_pandas/nestedframe/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11998 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/tests/nested_pandas/nestedframe/test_nestedframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/tests/nested_pandas/nestedframe/test_nestedframe_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:37:07.849983 nested_pandas-0.1.1/tests/nested_pandas/series/
+-rw-r--r--   0 runner    (1001) docker     (127)    30461 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/tests/nested_pandas/series/test_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/tests/nested_pandas/series/test_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61445 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/tests/nested_pandas/series/test_ext_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12404 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/tests/nested_pandas/series/test_packer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:37:07.853983 nested_pandas-0.1.1/tests/nested_pandas/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-30 21:37:02.000000 nested_pandas-0.1.1/tests/nested_pandas/utils/test_utils.py
```

### Comparing `nested_pandas-0.1/.copier-answers.yml` & `nested_pandas-0.1.1/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `nested_pandas-0.1/.gitattributes` & `nested_pandas-0.1.1/.gitattributes`

 * *Files identical despite different names*

### Comparing `nested_pandas-0.1/.github/ISSUE_TEMPLATE/1-bug_report.md` & `nested_pandas-0.1.1/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `nested_pandas-0.1/.github/ISSUE_TEMPLATE/2-feature_request.md` & `nested_pandas-0.1.1/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `nested_pandas-0.1/.github/pull_request_template.md` & `nested_pandas-0.1.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `nested_pandas-0.1/.github/workflows/asv-main.yml` & `nested_pandas-0.1.1/.github/workflows/asv-main.yml`

 * *Files identical despite different names*

### Comparing `nested_pandas-0.1/.github/workflows/asv-nightly.yml` & `nested_pandas-0.1.1/.github/workflows/asv-nightly.yml`

 * *Files identical despite different names*

### Comparing `nested_pandas-0.1/.github/workflows/asv-pr.yml` & `nested_pandas-0.1.1/.github/workflows/asv-pr.yml`

 * *Files identical despite different names*

### Comparing `nested_pandas-0.1/.github/workflows/build-documentation.yml` & `nested_pandas-0.1.1/.github/workflows/build-documentation.yml`

 * *Files identical despite different names*

### Comparing `nested_pandas-0.1/.github/workflows/pre-commit-ci.yml` & `nested_pandas-0.1.1/.github/workflows/pre-commit-ci.yml`

 * *Files identical despite different names*

### Comparing `nested_pandas-0.1/.github/workflows/publish-benchmarks-pr.yml` & `nested_pandas-0.1.1/.github/workflows/publish-benchmarks-pr.yml`

 * *Files identical despite different names*

### Comparing `nested_pandas-0.1/.github/workflows/publish-to-pypi.yml` & `nested_pandas-0.1.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `nested_pandas-0.1/.github/workflows/smoke-test.yml` & `nested_pandas-0.1.1/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `nested_pandas-0.1/.github/workflows/testing-and-coverage.yml` & `nested_pandas-0.1.1/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `nested_pandas-0.1/.gitignore` & `nested_pandas-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `nested_pandas-0.1/.pre-commit-config.yaml` & `nested_pandas-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nested_pandas-0.1/.setup_dev.sh` & `nested_pandas-0.1.1/.setup_dev.sh`

 * *Files identical despite different names*

### Comparing `nested_pandas-0.1/LICENSE` & `nested_pandas-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nested_pandas-0.1/PKG-INFO` & `nested_pandas-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nested-pandas
-Version: 0.1
+Version: 0.1.1
 Author-email: LINCC Frameworks <brantd@uw.edu>
 License: MIT License
         
         Copyright (c) 2023 LINCC Frameworks
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -43,14 +43,22 @@
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 
 # nested-pandas
+
+[![Template](https://img.shields.io/badge/Template-LINCC%20Frameworks%20Python%20Project%20Template-brightgreen)](https://lincc-ppt.readthedocs.io/en/latest/)
+
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/lincc-frameworks/nested-pandas/smoke-test.yml)](https://github.com/lincc-frameworks/nested-pandas/actions/workflows/smoke-test.yml)
+[![codecov](https://codecov.io/gh/lincc-frameworks/nested-pandas/branch/main/graph/badge.svg)](https://codecov.io/gh/lincc-frameworks/nested-pandas)
+[![Read the Docs](https://img.shields.io/readthedocs/nested-pandas)](https://nested-pandas.readthedocs.io/)
+[![benchmarks](https://img.shields.io/github/actions/workflow/status/lincc-frameworks/nested-pandas/asv-main.yml?label=benchmarks)](https://lincc-frameworks.github.io/nested-pandas/)
+
 An extension of pandas for efficient representation of nested
 associated datasets.
 
 Nested-Pandas extends the [pandas](https://pandas.pydata.org/) package with 
 tooling and support for nested dataframes packed into values of top-level 
 dataframe columns. [Pyarrow](https://arrow.apache.org/docs/python/index.html) 
 is used internally to aid in scalability and performance.
@@ -69,17 +77,10 @@
 
 
 
 This is a LINCC Frameworks project - find more information about LINCC Frameworks [here](https://lsstdiscoveryalliance.org/programs/lincc-frameworks/).
 
 
 
-[![Template](https://img.shields.io/badge/Template-LINCC%20Frameworks%20Python%20Project%20Template-brightgreen)](https://lincc-ppt.readthedocs.io/en/latest/)
-
-[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/lincc-frameworks/nested-pandas/smoke-test.yml)](https://github.com/lincc-frameworks/nested-pandas/actions/workflows/smoke-test.yml)
-[![codecov](https://codecov.io/gh/lincc-frameworks/nested-pandas/branch/main/graph/badge.svg)](https://codecov.io/gh/lincc-frameworks/nested-pandas)
-[![Read the Docs](https://img.shields.io/readthedocs/nested-pandas)](https://nested-pandas.readthedocs.io/)
-[![benchmarks](https://img.shields.io/github/actions/workflow/status/lincc-frameworks/nested-pandas/asv-main.yml?label=benchmarks)](https://lincc-frameworks.github.io/nested-pandas/)
-
 ## Acknowledgements
 
 This project is supported by Schmidt Sciences.
```

### Comparing `nested_pandas-0.1/README.md` & `nested_pandas-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,16 @@
 # nested-pandas
+
+[![Template](https://img.shields.io/badge/Template-LINCC%20Frameworks%20Python%20Project%20Template-brightgreen)](https://lincc-ppt.readthedocs.io/en/latest/)
+
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/lincc-frameworks/nested-pandas/smoke-test.yml)](https://github.com/lincc-frameworks/nested-pandas/actions/workflows/smoke-test.yml)
+[![codecov](https://codecov.io/gh/lincc-frameworks/nested-pandas/branch/main/graph/badge.svg)](https://codecov.io/gh/lincc-frameworks/nested-pandas)
+[![Read the Docs](https://img.shields.io/readthedocs/nested-pandas)](https://nested-pandas.readthedocs.io/)
+[![benchmarks](https://img.shields.io/github/actions/workflow/status/lincc-frameworks/nested-pandas/asv-main.yml?label=benchmarks)](https://lincc-frameworks.github.io/nested-pandas/)
+
 An extension of pandas for efficient representation of nested
 associated datasets.
 
 Nested-Pandas extends the [pandas](https://pandas.pydata.org/) package with 
 tooling and support for nested dataframes packed into values of top-level 
 dataframe columns. [Pyarrow](https://arrow.apache.org/docs/python/index.html) 
 is used internally to aid in scalability and performance.
@@ -21,17 +29,10 @@
 
 
 
 This is a LINCC Frameworks project - find more information about LINCC Frameworks [here](https://lsstdiscoveryalliance.org/programs/lincc-frameworks/).
 
 
 
-[![Template](https://img.shields.io/badge/Template-LINCC%20Frameworks%20Python%20Project%20Template-brightgreen)](https://lincc-ppt.readthedocs.io/en/latest/)
-
-[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/lincc-frameworks/nested-pandas/smoke-test.yml)](https://github.com/lincc-frameworks/nested-pandas/actions/workflows/smoke-test.yml)
-[![codecov](https://codecov.io/gh/lincc-frameworks/nested-pandas/branch/main/graph/badge.svg)](https://codecov.io/gh/lincc-frameworks/nested-pandas)
-[![Read the Docs](https://img.shields.io/readthedocs/nested-pandas)](https://nested-pandas.readthedocs.io/)
-[![benchmarks](https://img.shields.io/github/actions/workflow/status/lincc-frameworks/nested-pandas/asv-main.yml?label=benchmarks)](https://lincc-frameworks.github.io/nested-pandas/)
-
 ## Acknowledgements
 
 This project is supported by Schmidt Sciences.
```

### Comparing `nested_pandas-0.1/benchmarks/asv.conf.json` & `nested_pandas-0.1.1/benchmarks/asv.conf.json`

 * *Files identical despite different names*

### Comparing `nested_pandas-0.1/benchmarks/benchmarks.py` & `nested_pandas-0.1.1/benchmarks/benchmarks.py`

 * *Files identical despite different names*

### Comparing `nested_pandas-0.1/docs/Makefile` & `nested_pandas-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nested_pandas-0.1/docs/conf.py` & `nested_pandas-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nested_pandas-0.1/docs/gettingstarted/installation.rst` & `nested_pandas-0.1.1/docs/gettingstarted/installation.rst`

 * *Files identical despite different names*

### Comparing `nested_pandas-0.1/docs/gettingstarted/quickstart.ipynb` & `nested_pandas-0.1.1/docs/gettingstarted/quickstart.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991319444444444%*

 * *Differences: {"'cells'": '{10: {\'source\': ["nested-pandas extends the Pandas API, meaning any operation you '*

 * *            'could do in Pandas is available within nested-pandas. However, nested-pandas has '*

 * *            'additional functionality and tooling to better support working with nested datasets. '*

 * *            'For example, let\'s look at `query`:"]}}'}*

```diff
@@ -86,15 +86,15 @@
                 "nf.all_columns"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "nested-pandas extends the Pandas API, meaning any operation you could do in Pandas is available within nested-pandas. However, nested-pandas has additional functionality and tooling to better support working with Nested datasets. For example, let's look at `query`:"
+                "nested-pandas extends the Pandas API, meaning any operation you could do in Pandas is available within nested-pandas. However, nested-pandas has additional functionality and tooling to better support working with nested datasets. For example, let's look at `query`:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `nested_pandas-0.1/docs/gettingstarted.rst` & `nested_pandas-0.1.1/docs/gettingstarted.rst`

 * *Files identical despite different names*

### Comparing `nested_pandas-0.1/docs/index.rst` & `nested_pandas-0.1.1/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -47,9 +47,9 @@
 Learn more about contributing to this repository in our :doc:`Contribution Guide <gettingstarted/contributing>`.
 
 .. toctree::
    :hidden:
 
    Home page <self>
    Getting Started <gettingstarted>
-   Notebooks <notebooks>
+   Tutorials <tutorials>
    API Reference <autoapi/index>
```

### Comparing `nested_pandas-0.1/docs/tutorials/data_loading_notebook.ipynb` & `nested_pandas-0.1.1/docs/tutorials/data_loading_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `nested_pandas-0.1/docs/tutorials/low_level.ipynb` & `nested_pandas-0.1.1/docs/tutorials/low_level.ipynb`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9940729572077228%*

 * *Differences: {"'cells'": "{1: {'metadata': {replace: OrderedDict()}}, 3: {'metadata': {replace: "*

 * *            "OrderedDict()}}, 5: {'source': {insert: [(2, '`.nest` accessor provides an object "*

 * *            'implementing `Mapping` interface, so you can use it like an immutable '*

 * *            "dictionary.\\n'), (3, 'Keys of this mapping are the names of the nested columns "*

 * *            '(fields), and values are "flat" Series representing the nested data.\\n\'), (4, '*

 * *            "'\\n'), (5, 'The only way to modify the ne […]*

```diff
@@ -13,20 +13,15 @@
                 "It also demonstrates how to convert nested Series to and from different data types, like `pd.ArrowDtype`d Series, flat dataframes, list-array dataframes, and collections of nested elements."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "619f088e7ac0f327",
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2024-05-09T12:43:47.641800Z",
-                    "start_time": "2024-05-09T12:43:47.634903Z"
-                }
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import pandas as pd\n",
                 "import pyarrow as pa\n",
                 "\n",
                 "from nested_pandas import NestedDtype\n",
@@ -45,20 +40,15 @@
                 "This column would represent [light curves](https://en.wikipedia.org/wiki/Light_curve) of some astronomical objects. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "f9dd16a4bb9aaa63",
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2024-05-09T12:43:47.708715Z",
-                    "start_time": "2024-05-09T12:43:47.700005Z"
-                }
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "nested_df = generate_data(4, 3, seed=42)\n",
                 "nested_series = nested_df[\"nested\"]\n",
                 "nested_series[2]"
             ]
         },
@@ -79,28 +69,25 @@
         {
             "cell_type": "markdown",
             "id": "40f0d1e6a2cbbb44",
             "metadata": {},
             "source": [
                 "### `.nest` object is a mapping\n",
                 "\n",
-                "`.nest` accessor provides an object implementing `Mapping` interface, so you can use it like a dictionary.\n",
-                "Keys of this mapping are the names of the nested columns (fields), and values are \"flat\" Series representing the nested data."
+                "`.nest` accessor provides an object implementing `Mapping` interface, so you can use it like an immutable dictionary.\n",
+                "Keys of this mapping are the names of the nested columns (fields), and values are \"flat\" Series representing the nested data.\n",
+                "\n",
+                "The only way to modify the nested data in-place with this interface is to re-assign the whole field with a new data of the same length and dtype, see the discussion about the mutability limitations in [this GitHub issue](https://github.com/lincc-frameworks/nested-pandas/issues/87)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "fb7beb750d3e2893",
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2024-05-09T12:43:47.711893Z",
-                    "start_time": "2024-05-09T12:43:47.709614Z"
-                }
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "list(nested_series.nest.keys())"
             ]
         },
         {
             "cell_type": "markdown",
@@ -110,20 +97,15 @@
                 "You can also get a list of fields with `.fields` attribute"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "56b0d9ffc5820d22",
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2024-05-09T12:43:47.714235Z",
-                    "start_time": "2024-05-09T12:43:47.712499Z"
-                }
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "nested_series.nest.fields"
             ]
         },
         {
             "cell_type": "markdown",
@@ -133,20 +115,15 @@
                 "The value of each key is a \"flat\" Series with repeated index, so the original index of the `nested_series` is repeated for each element of the nested data. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "30ee9a430b6ff641",
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2024-05-09T12:43:47.717863Z",
-                    "start_time": "2024-05-09T12:43:47.715368Z"
-                }
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "nested_series.nest[\"t\"]"
             ]
         },
         {
             "cell_type": "markdown",
@@ -156,60 +133,58 @@
                 "You can also get a subset of nested columns as a new nested Series"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "f0db15d31b289140",
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2024-05-09T12:43:47.720405Z",
-                    "start_time": "2024-05-09T12:43:47.718626Z"
-                }
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "nested_series.nest[[\"t\", \"flux\"]].dtype"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "3ea3e533239f964c",
             "metadata": {},
             "source": [
                 "You can add new columns, drop existing ones, or modify the existing ones.\n",
-                "The modification is currently limited to the case when you replace the whole \"flat\" Series with a new one of the same length.\n",
+                "These operations would create new nested Series, however they would create shallow copies of the rest of the fields, so they are quite efficient.\n",
+                "\n",
+                "The in-place modification is currently limited to the case when you replace the whole \"flat\" Series with a new one of the same length and compatible dtype.\n",
                 "When modifying the nested data, only the column you are working with is changed, the rest of the data are not affected and not copied."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "66ae5cc26fa17458",
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2024-05-09T12:43:47.726619Z",
-                    "start_time": "2024-05-09T12:43:47.721070Z"
-                }
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "new_series = nested_series.copy()\n",
                 "\n",
                 "# Change the data in-place\n",
                 "new_series.nest[\"flux\"] = new_series.nest[\"flux\"] - new_series.nest[\"flux\"].mean()\n",
                 "\n",
-                "# Add new column\n",
-                "new_series.nest[\"lsst_band\"] = \"lsst_\" + new_series.nest[\"band\"]\n",
+                "# Create a new series with a new column\n",
+                "new_series = new_series.nest.with_field(\"lsst_band\", \"lsst_\" + new_series.nest[\"band\"])\n",
                 "\n",
-                "# Drop the column, .pop() method is also available\n",
-                "del new_series.nest[\"band\"]\n",
+                "# Create a new series with a column removed, you can also pass a list of columns to remove\n",
+                "new_series = new_series.nest.without_field(\"band\")\n",
                 "\n",
                 "# Add a new column with a python list instead of a Series\n",
-                "new_series.nest[\"new_column\"] = [1, 2] * (new_series.nest.flat_length // 2)\n",
+                "new_series = new_series.nest.with_field(\n",
+                "    \"new_column\",\n",
+                "    [1, 2] * (new_series.nest.flat_length // 2),\n",
+                ")\n",
+                "\n",
+                "# Create a new series, with a column dtype changed\n",
+                "new_series = new_series.nest.with_field(\"t\", new_series.nest[\"t\"].astype(np.int8))\n",
                 "\n",
                 "new_series.nest.to_flat()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "f00e61bbdc730fea",
@@ -224,35 +199,25 @@
                 "Both representations are copy-free, so they could be done very efficiently. The only additional overhead when accessing a \"flat\" representation is the creation of a new repeating index."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "ce6d519d8d37ead3",
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2024-05-09T12:43:47.768616Z",
-                    "start_time": "2024-05-09T12:43:47.764343Z"
-                }
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "nested_series.nest.to_flat([\"flux\", \"t\"])"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "2421b91387487995",
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2024-05-09T12:43:47.798697Z",
-                    "start_time": "2024-05-09T12:43:47.795583Z"
-                }
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "lists_df = nested_series.nest.to_lists()  # may also accept a list of fields (nested columns) to get\n",
                 "lists_df[\"t\"].list.len()  # here we use pandas' build-in list accessor to get the length of each list"
             ]
         },
         {
@@ -263,27 +228,20 @@
                 "List-arrays may be assigned back to the nested Series"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "f2c205e95affb9ba",
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2024-05-09T12:43:47.833034Z",
-                    "start_time": "2024-05-09T12:43:47.827805Z"
-                }
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "new_series = nested_series.copy()\n",
-                "\n",
                 "# Adjust each time to be relative to the first observation\n",
                 "dt = new_series.nest.to_lists()[\"t\"].apply(lambda t: t - t.min())\n",
-                "new_series.nest.set_list_field(\"dt\", dt)\n",
+                "new_series = new_series.nest.with_list_field(\"dt\", dt)\n",
                 "new_series.nest.to_flat()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "93f73bf28d48bfdc",
             "metadata": {},
@@ -309,36 +267,26 @@
                 "So the conversion is quite straightforward, and doesn't require any data copying. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "8ef96243c6d74aff",
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2024-05-09T12:43:47.875752Z",
-                    "start_time": "2024-05-09T12:43:47.872293Z"
-                }
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "struct_series = pd.Series(nested_series, dtype=nested_series.dtype.to_pandas_arrow_dtype())\n",
                 "struct_series.struct.field(\"flux\")  # pandas build-in accessor for struct-arrays"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "422e719861ae40f6",
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2024-05-09T12:43:47.925465Z",
-                    "start_time": "2024-05-09T12:43:47.922965Z"
-                }
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "nested_series.equals(pd.Series(struct_series, dtype=NestedDtype.from_pandas_arrow_dtype(struct_series.dtype)))"
             ]
         },
         {
             "cell_type": "markdown",
@@ -360,36 +308,26 @@
                 "You can also use `pack()` to create a nested Series from a flat dataframe with repeated index, for example from a one given by `.nest.to_flat()` method."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "926f2c9fcffc5f03",
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2024-05-09T12:43:47.937490Z",
-                    "start_time": "2024-05-09T12:43:47.933878Z"
-                }
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "new_series = pack(nested_series.nest.to_flat())\n",
                 "new_series.equals(nested_series)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "3a1d2025c232ac82",
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2024-05-09T12:43:47.969831Z",
-                    "start_time": "2024-05-09T12:43:47.964948Z"
-                }
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "series_from_flat = pack(\n",
                 "    pd.DataFrame(\n",
                 "        {\n",
                 "            \"t\": [1, 2, 3, 4, 5, 6],\n",
                 "            \"flux\": [0.1, 0.2, 0.3, 0.4, 0.5, 0.6],\n",
@@ -418,20 +356,15 @@
                 "All the elements must have the same columns (fields), but may have the different length of the nested data.    "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "2de4619726ab3d5c",
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2024-05-09T12:43:47.991261Z",
-                    "start_time": "2024-05-09T12:43:47.986129Z"
-                }
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "series_from_pack = pack(\n",
                 "    [\n",
                 "        pd.DataFrame({\"t\": [1, 2, 3], \"flux\": [0.1, 0.2, 0.3]}),\n",
                 "        {\"t\": [4, 5], \"flux\": [0.4, 0.5]},\n",
                 "        None,\n",
@@ -450,20 +383,15 @@
                 "If we are not happy with the default dtype, we can specify it explicitly, see more details on how to do it in the next section, here we just show an example."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "9c63ae45dd0b6a29",
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2024-05-09T12:43:47.995869Z",
-                    "start_time": "2024-05-09T12:43:47.992016Z"
-                }
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "series_from_pack = pack(\n",
                 "    [\n",
                 "        pd.DataFrame({\"t\": [1, 2, 3], \"flux\": [0.1, 0.2, 0.3]}),\n",
                 "        {\"t\": [4, 5], \"flux\": [0.4, 0.5]},\n",
                 "        None,\n",
@@ -496,20 +424,15 @@
                 "This is the same as using `pack()` function, but you need to specify the dtype explicitly."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "1284d9b536b9e784",
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2024-05-09T12:43:48.000441Z",
-                    "start_time": "2024-05-09T12:43:47.996620Z"
-                }
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "series_from_dtype = pd.Series(\n",
                 "    [\n",
                 "        pd.NA,\n",
                 "        pd.DataFrame({\"t\": [1, 2, 3], \"band\": [\"g\", \"r\", \"r\"]}),\n",
                 "        {\"t\": np.array([4, 5]), \"band\": [None, \"r\"]},\n",
@@ -527,20 +450,15 @@
                 "`pyarrow` native objects are also supported. Scalars:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "b7c7fd878bc97f68",
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2024-05-09T12:43:48.004677Z",
-                    "start_time": "2024-05-09T12:43:48.001129Z"
-                }
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "series_pa_type = pa.struct({\"t\": pa.list_(pa.float64()), \"band\": pa.list_(pa.string())})\n",
                 "scalar_pa_type = pa.struct({\"t\": pa.list_(pa.int16()), \"band\": pa.list_(pa.string())})\n",
                 "series_from_pa_scalars = pd.Series(\n",
                 "    # Scalars will be cast to the given type\n",
                 "    [\n",
@@ -564,20 +482,15 @@
                 "Construction with `pyarrow` struct arrays is the cheapest way to create a nested Series. It is very semilliar to initialisation of a `pd.Series` of `pd.ArrowDtype` type."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "e837d25dcb0a2b4d",
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2024-05-09T12:43:48.015257Z",
-                    "start_time": "2024-05-09T12:43:48.013217Z"
-                }
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "pa_struct_array = pa.StructArray.from_arrays(\n",
                 "    [\n",
                 "        [\n",
                 "            np.arange(10),\n",
                 "            np.arange(5),\n",
@@ -607,20 +520,15 @@
                 "We have already seen how to convert nested Series to `pd.ArrowDtype`d Series, to a flat dataframe, or to a list-array dataframe. Let's summarize it here one more time:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "116c902ea8681c9e",
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2024-05-09T12:43:48.040801Z",
-                    "start_time": "2024-05-09T12:43:48.038106Z"
-                }
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "# Convert to pd.ArrowDtype Series of struct-arrays\n",
                 "arrow_dtyped_series = pd.Series(nested_series, dtype=nested_series.dtype.to_pandas_arrow_dtype())\n",
                 "# Convert to a flat dataframe\n",
                 "flat_df = nested_series.nest.to_flat()\n",
                 "# Convert to a list-array dataframe\n",
@@ -637,20 +545,15 @@
                 "Single element representation of the nested Series is `pd.DataFrame`, so iteration over the nested Series would yield `pd.DataFrame` objects."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "30ea40dee30795d1",
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2024-05-09T12:43:48.055678Z",
-                    "start_time": "2024-05-09T12:43:48.050677Z"
-                }
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "for element in nested_series:\n",
                 "    print(element)"
             ]
         },
         {
@@ -661,20 +564,15 @@
                 "All collections built with iterables would have `pd.DataFrame` as elements:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "81f6c1f98dfc26a9",
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2024-05-09T12:43:48.060166Z",
-                    "start_time": "2024-05-09T12:43:48.056425Z"
-                }
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "nested_elements = list(nested_series)\n",
                 "nested_elements[-1]"
             ]
         },
         {
@@ -685,38 +583,28 @@
                 "Nested Series also supports direct conversion to numpy array of object dtype:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "69ed758c48c55015",
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2024-05-09T12:43:48.063115Z",
-                    "start_time": "2024-05-09T12:43:48.060863Z"
-                }
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "nested_series_with_na = pack([None, pd.NA, {\"t\": [1, 2], \"flux\": [0.1, None]}])\n",
                 "# Would have None for top-level missed data\n",
                 "np_array1 = np.array(nested_series_with_na)\n",
                 "print(f\"{np_array1[0] = }\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "99ce9d18bc69ae49",
-            "metadata": {
-                "ExecuteTime": {
-                    "end_time": "2024-05-09T12:43:48.088986Z",
-                    "start_time": "2024-05-09T12:43:48.086255Z"
-                }
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "# Would have empty pd.DataFrame for top-level missed data\n",
                 "np_array2 = nested_series_with_na.to_numpy(na_value=pd.DataFrame())\n",
                 "print(f\"{np_array2[0] = }\")"
             ]
         }
```

### Comparing `nested_pandas-0.1/nestedframe.png` & `nested_pandas-0.1.1/nestedframe.png`

 * *Files identical despite different names*

### Comparing `nested_pandas-0.1/pyproject.toml` & `nested_pandas-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nested_pandas-0.1/src/nested_pandas/datasets/generation.py` & `nested_pandas-0.1.1/src/nested_pandas/datasets/generation.py`

 * *Files identical despite different names*

### Comparing `nested_pandas-0.1/src/nested_pandas/nestedframe/core.py` & `nested_pandas-0.1.1/src/nested_pandas/nestedframe/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,15 +95,17 @@
         -------
         NestedFrame
             A new NestedFrame with the added nested column.
         """
         # Add sources to objects
         packed = packer.pack(obj, name=name, dtype=dtype)
         label = packed.name
-        return self.assign(**{f"{label}": packed})
+        new_df = self.copy()
+        new_df[label] = packed
+        return new_df
 
     def _split_query(self, expr) -> dict:
         """Splits a pandas query into multiple subqueries for nested and base layers"""
         # Ensure query has needed spacing for upcoming split
         expr = _ensure_spacing(expr)
         nest_exprs = {col: [] for col in self.nested_columns + ["base"]}  # type: dict
         split_expr = expr.split(" ")
@@ -343,15 +345,15 @@
                 subset=subset,
                 inplace=inplace,
                 ignore_index=ignore_index,
             )
         )
         return new_df
 
-    def reduce(self, func, *args, **kwargs) -> NestedFrame:
+    def reduce(self, func, *args, **kwargs) -> NestedFrame:  # type: ignore[override]
         """
         Takes a function and applies it to each top-level row of the NestedFrame.
 
         The user may specify which columns the function is applied to, with
         columns from the 'base' layer being passsed to the function as
         scalars and columns from the nested layers being passed as numpy arrays.
 
@@ -407,43 +409,23 @@
             raise ValueError("No columns in `*args` specified to apply function to")
 
         # The remaining args are the extra arguments to the function other than columns
         extra_args: tuple[Any, ...] = ()  # empty tuple to make mypy happy
         if len(requested_columns) < len(args):
             extra_args = args[len(requested_columns) :]
 
-        # find targeted layers
-        layers = np.unique([col[0] for col in requested_columns])
-
-        # build a flat dataframe with array columns to apply to the function
-        apply_df = NestedFrame()
-        for layer in layers:
+        iterators = []
+        for layer, col in requested_columns:
             if layer == "base":
-                columns = [col[1] for col in requested_columns if col[0] == layer]
-                apply_df = apply_df.join(self[columns], how="outer")
+                iterators.append(self[col])
             else:
-                # TODO: It should be faster to pass these columns to to_lists, but its 20x slower
-                # columns = [col[1] for col in requested_columns if col[0] == layer]
-                apply_df = apply_df.join(self[layer].nest.to_lists(), how="outer")
+                iterators.append(self[layer].array.iter_field_lists(col))
 
-        # Translates the requested columns into the scalars or arrays we pass to func.
-        def translate_cols(frame, layer, col):
-            if layer == "base":
-                # We pass the "base" column as a scalar
-                return frame[col]
-            return np.asarray(frame[col])
-
-        # send arrays along to the apply call
-        result = apply_df.apply(
-            lambda x: func(
-                *[translate_cols(x, layer, col) for layer, col in requested_columns], *extra_args, **kwargs
-            ),
-            axis=1,  # to apply func on each row of our nested frame)
-        )
-        return result
+        results = [func(*cols, *extra_args, **kwargs) for cols in zip(*iterators)]
+        return NestedFrame(results, index=self.index)
 
     def to_parquet(self, path, by_layer=False, **kwargs) -> None:
         """Creates parquet file(s) with the data of a NestedFrame, either
         as a single parquet file where each nested dataset is packed into its
         own column or as an individual parquet file for each layer.
 
         Note that here we always opt to use the pyarrow engine for writing
```

### Comparing `nested_pandas-0.1/src/nested_pandas/nestedframe/io.py` & `nested_pandas-0.1.1/src/nested_pandas/nestedframe/io.py`

 * *Files identical despite different names*

### Comparing `nested_pandas-0.1/src/nested_pandas/nestedframe/utils.py` & `nested_pandas-0.1.1/src/nested_pandas/nestedframe/utils.py`

 * *Files identical despite different names*

### Comparing `nested_pandas-0.1/src/nested_pandas/series/accessor.py` & `nested_pandas-0.1.1/src/nested_pandas/series/accessor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Python 3.9 doesn't support "|" for types
 from __future__ import annotations
 
-from collections.abc import Generator, MutableMapping
+from collections import defaultdict
+from collections.abc import Generator, Mapping
 from typing import cast
 
 import numpy as np
 import pandas as pd
 import pyarrow as pa
 from numpy.typing import ArrayLike
 from pandas.api.extensions import register_series_accessor
@@ -13,15 +14,15 @@
 from nested_pandas.series.dtype import NestedDtype
 from nested_pandas.series.packer import pack_sorted_df_into_struct
 
 __all__ = ["NestSeriesAccessor"]
 
 
 @register_series_accessor("nest")
-class NestSeriesAccessor(MutableMapping):
+class NestSeriesAccessor(Mapping):
     """Accessor for operations on Series of NestedDtype
 
     This accessor implements `MutableMapping` interface over the fields of the
     struct, so you can access, change and delete the fields as if it was a
     dictionary, with `[]`, `[] =` and `del` operators.
     """
 
@@ -49,22 +50,27 @@
         pd.DataFrame
             Dataframe of list-arrays.
         """
         fields = fields if fields is not None else list(self._series.array.field_names)
         if len(fields) == 0:
             raise ValueError("Cannot convert a struct with no fields to lists")
 
-        struct_array = cast(pa.StructArray, pa.array(self._series))
+        list_chunks = defaultdict(list)
+        for chunk in self._series.array._chunked_array.iterchunks():
+            struct_array = cast(pa.StructArray, chunk)
+            for field in fields:
+                list_array = cast(pa.ListArray, struct_array.field(field))
+                list_chunks[field].append(list_array)
 
         list_series = {}
-        for field in fields:
-            list_array = cast(pa.ListArray, struct_array.field(field))
+        for field, chunks in list_chunks.items():
+            chunked_array = pa.chunked_array(chunks)
             list_series[field] = pd.Series(
-                list_array,
-                dtype=pd.ArrowDtype(list_array.type),
+                chunked_array,
+                dtype=pd.ArrowDtype(chunked_array.type),
                 index=self._series.index,
                 name=field,
                 copy=False,
             )
 
         return pd.DataFrame(list_series)
 
@@ -81,87 +87,128 @@
         pd.DataFrame
             Dataframe of flat arrays.
         """
         fields = fields if fields is not None else list(self._series.array.field_names)
         if len(fields) == 0:
             raise ValueError("Cannot flatten a struct with no fields")
 
-        struct_array = cast(pa.StructArray, pa.array(self._series))
+        index = pd.Series(self.get_flat_index(), name=self._series.index.name)
+
+        flat_chunks = defaultdict(list)
+        for chunk in self._series.array._chunked_array.iterchunks():
+            struct_array = cast(pa.StructArray, chunk)
+            for field in fields:
+                list_array = cast(pa.ListArray, struct_array.field(field))
+                flat_array = list_array.flatten()
+                flat_chunks[field].append(flat_array)
 
         flat_series = {}
-        index = None
-        for field in fields:
-            list_array = cast(pa.ListArray, struct_array.field(field))
-            flat_array = list_array.flatten()
-            if index is None:
-                index = self.get_flat_index()
+        for field, chunks in flat_chunks.items():
+            chunked_array = pa.chunked_array(chunks)
             flat_series[field] = pd.Series(
-                flat_array,
+                chunked_array,
                 index=pd.Series(index, name=self._series.index.name),
                 name=field,
                 copy=False,
-                dtype=pd.ArrowDtype(flat_array.type),
+                dtype=pd.ArrowDtype(chunked_array.type),
             )
 
         return pd.DataFrame(flat_series)
 
     @property
     def flat_length(self) -> int:
         """Length of the flat arrays"""
         return self._series.array.flat_length
 
     @property
     def fields(self) -> list[str]:
         """Names of the nested columns"""
         return self._series.array.field_names
 
-    def set_flat_field(self, field: str, value: ArrayLike) -> None:
-        """Set the field from flat-array of values, in-place
+    def with_field(self, field: str, value: ArrayLike) -> pd.Series:
+        """Set the field from flat-array of values and return a new series
+
+        It is an alias for `.nest.with_flat_field`.
+
+        Parameters
+        ----------
+        field : str
+            Name of the field to set. If not present, it will be added.
+        value : ArrayLike
+            Array of values to set. It must be a scalar or have the same length
+             as the flat arrays, e.g. `self.flat_length`.
+
+        Returns
+        -------
+        pd.Series
+            The new series with the field set.
+        """
+        return self.with_flat_field(field, value)
+
+    def with_flat_field(self, field: str, value: ArrayLike) -> pd.Series:
+        """Set the field from flat-array of values and return a new series
 
         Parameters
         ----------
         field : str
             Name of the field to set. If not present, it will be added.
         value : ArrayLike
             Array of values to set. It must be a scalar or have the same length
              as the flat arrays, e.g. `self.flat_length`.
+
+        Returns
+        -------
+        pd.Series
+            The new series with the field set.
         """
-        self._series.array.set_flat_field(field, value)
+        new_array = self._series.array.copy()
+        new_array.set_flat_field(field, value)
+        return pd.Series(new_array, copy=False, index=self._series.index, name=self._series.name)
 
-    def set_list_field(self, field: str, value: ArrayLike) -> None:
-        """Set the field from list-array, in-place
+    def with_list_field(self, field: str, value: ArrayLike) -> pd.Series:
+        """Set the field from list-array of values and return a new series
 
         Parameters
         ----------
         field : str
             Name of the field to set. If not present, it will be added.
         value : ArrayLike
             Array of values to set. It must be a list-array of the same length
              as the series, e.g. length of the series.
+
+        Returns
+        -------
+        pd.Series
+            The new series with the field set.
         """
-        self._series.array.set_list_field(field, value)
+        new_array = self._series.array.copy()
+        new_array.set_list_field(field, value)
+        return pd.Series(new_array, copy=False, index=self._series.index, name=self._series.name)
+
+    def without_field(self, field: str | list[str]) -> pd.Series:
+        """Remove the field(s) from the series and return a new series
 
-    # I intentionally don't call it `drop` or `drop_field` because `pd.DataFrame.drop` is not inplace
-    # by default, and I wouldn't like to surprise the user.
-    def pop_field(self, field: str) -> pd.Series:
-        """Delete the field from the struct and return it.
+        Note, that at least one field must be left in the series.
 
         Parameters
         ----------
-        field : str
-            Name of the field to delete.
+        field : str or list[str]
+            Name of the field(s) to remove.
 
         Returns
         -------
         pd.Series
-            The deleted field.
+            The new series without the field(s).
         """
-        series = self[field]
-        self._series.array.pop_field(field)
-        return series
+        if isinstance(field, str):
+            field = [field]
+
+        new_array = self._series.array.copy()
+        new_array.pop_fields(field)
+        return pd.Series(new_array, copy=False, index=self._series.index, name=self._series.name)
 
     def query_flat(self, query: str) -> pd.Series:
         """Query the flat arrays with a boolean expression
 
         Currently, it will remove empty rows from the output series.
         # TODO: preserve the index keeping empty rows
 
@@ -241,28 +288,34 @@
         if isinstance(key, list):
             new_array = self._series.array.view_fields(key)
             return pd.Series(new_array, index=self._series.index, name=self._series.name)
 
         return self.get_flat_series(key)
 
     def __setitem__(self, key: str, value: ArrayLike) -> None:
+        """Replace the field values from flat-array of values
+
+        Currently, only replacement of the whole field is supported, the length
+        and dtype of the input value must match the field.
+        https://github.com/lincc-frameworks/nested-pandas/issues/87
+        """
         # TODO: we can be much-much smarter about the performance here
         # TODO: think better about underlying pa.ChunkArray in both self._series.array and value
 
         ndim = np.ndim(value)
 
         # Everything is empty, do nothing
         if len(self._series) == 0 and ndim != 0:
             array = pa.array(value, from_pandas=True)
             if len(array) == 0:
                 return
 
         # Set single value for all rows
         if ndim == 0:
-            self.set_flat_field(key, value)
+            self._series.array.set_flat_field(key, value, keep_dtype=True)
             return
 
         if isinstance(value, pd.Series) and not self.get_flat_index().equals(value.index):
             raise ValueError("Cannot set field with a Series of different index")
 
         pa_array = pa.array(value, from_pandas=True)
 
@@ -270,17 +323,26 @@
         if len(pa_array) != self.flat_length:
             ValueError(
                 f"Cannot set field {key} with value of length {len(pa_array)}, the value is expected to be "
                 f"either a scalar, a 'flat' array of length {self.flat_length}, or a 'list' array of length "
                 f"{len(self._series)}."
             )
 
-        self.set_flat_field(key, pa_array)
-
-    def __delitem__(self, key: str) -> None:
-        self.pop_field(key)
+        self._series.array.set_flat_field(key, pa_array, keep_dtype=True)
 
     def __iter__(self) -> Generator[str, None, None]:
-        yield from iter(self._series.array.field_names)
+        return iter(self._series.array.field_names)
 
     def __len__(self) -> int:
         return len(self._series.array.field_names)
+
+    def __eq__(self, other) -> bool:
+        if not isinstance(other, type(self)):
+            return False
+        return self._series.equals(other._series)
+
+    def clear(self) -> None:
+        """Mandatory MutableMapping method, always fails with NotImplementedError
+
+        The reason is that we cannot delete all nested fields from the nested series.
+        """
+        raise NotImplementedError("Cannot delete fields from nested series")
```

### Comparing `nested_pandas-0.1/src/nested_pandas/series/dtype.py` & `nested_pandas-0.1.1/src/nested_pandas/series/dtype.py`

 * *Files identical despite different names*

### Comparing `nested_pandas-0.1/src/nested_pandas/series/ext_array.py` & `nested_pandas-0.1.1/src/nested_pandas/series/ext_array.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 # typing.Self and "|" union syntax don't exist in Python 3.9
 from __future__ import annotations
 
-from collections.abc import Iterator, Sequence
+from collections.abc import Generator, Iterable, Iterator, Sequence
 from typing import Any, Callable, cast
 
 import numpy as np
 import pandas as pd
 import pyarrow as pa
 from numpy.typing import ArrayLike
 from pandas import Index
@@ -138,32 +138,32 @@
         return super()._from_factorized(values, original)
 
     def __getitem__(self, item):
         item = check_array_indexer(self, item)
 
         if isinstance(item, np.ndarray):
             if len(item) == 0:
-                return type(self)(pa.chunked_array([], type=self._pa_array.type), validate=False)
+                return type(self)(pa.chunked_array([], type=self._chunked_array.type), validate=False)
             pa_item = pa.array(item)
             if item.dtype.kind in "iu":
-                return type(self)(self._pa_array.take(pa_item), validate=False)
+                return type(self)(self._chunked_array.take(pa_item), validate=False)
             if item.dtype.kind == "b":
-                return type(self)(self._pa_array.filter(pa_item), validate=False)
+                return type(self)(self._chunked_array.filter(pa_item), validate=False)
             # It should be covered by check_array_indexer above
             raise IndexError(
                 "Only integers, slices and integer or " "boolean arrays are valid indices."
             )  # pragma: no cover
 
         if isinstance(item, tuple):
             item = unpack_tuple_and_ellipses(item)
 
         if item is Ellipsis:
             item = slice(None)
 
-        scalar_or_array = self._pa_array[item]
+        scalar_or_array = self._chunked_array[item]
         if isinstance(scalar_or_array, pa.StructScalar):
             return self._convert_struct_scalar_to_df(scalar_or_array, copy=False)
         # Logically, it must be a pa.ChunkedArray if it is not a scalar
         pa_array = cast(pa.ChunkedArray, scalar_or_array)
         return type(self)(pa_array, validate=False)
 
     def __setitem__(self, key, value) -> None:
@@ -208,22 +208,22 @@
             value = pa.array([scalar] * pa.compute.sum(pa_mask).as_py())
 
         if argsort is not None:
             value = value.take(argsort)
 
         # We cannot use pa.compute.replace_with_mask(), it is not implemented for struct arrays:
         # https://github.com/apache/arrow/issues/29558
-        # self._pa_array = pa.compute.replace_with_mask(self._pa_array, pa_mask, value)
-        self._pa_array = replace_with_mask(self._pa_array, pa_mask, value)
+        # self._chunked_array = pa.compute.replace_with_mask(self._chunked_array, pa_mask, value)
+        self._chunked_array = replace_with_mask(self._chunked_array, pa_mask, value)
 
     def __len__(self) -> int:
-        return len(self._pa_array)
+        return len(self._chunked_array)
 
     def __iter__(self) -> Iterator[pd.DataFrame]:
-        for value in self._pa_array:
+        for value in self._chunked_array:
             yield self._convert_struct_scalar_to_df(value, copy=False)
 
     # We do not implement it yet, because pa.compute.equal does not work for struct arrays
     # ArrowExtensionArray does not implement it for struct arrays neither
     def __eq__(self, other):
         return super().__eq__(other)
 
@@ -251,43 +251,43 @@
         """
         if na_value is no_default:
             na_value = None
 
         # Hack with np.empty is the only way to force numpy to create 1-d array of objects
         result = np.empty(shape=len(self), dtype=object)
 
-        for i, value in enumerate(self._pa_array):
+        for i, value in enumerate(self._chunked_array):
             result[i] = self._convert_struct_scalar_to_df(value, copy=copy, na_value=na_value)
 
         return result
 
     @property
     def dtype(self) -> NestedDtype:
         """ExtensionArray dtype"""
         return self._dtype
 
     @property
     def nbytes(self) -> int:
         """Number of bytes consumed by the data in memory."""
-        return self._pa_array.nbytes
+        return self._chunked_array.nbytes
 
     def isna(self) -> np.ndarray:
         """Boolean NumPy array indicating if each value is missing."""
         # Fast paths adopted from ArrowExtensionArray
-        null_count = self._pa_array.null_count
+        null_count = self._chunked_array.null_count
         if null_count == 0:
             return np.zeros(len(self), dtype=bool)
         if null_count == len(self):
             return np.ones(len(self), dtype=bool)
 
-        return self._pa_array.is_null().to_numpy()
+        return self._chunked_array.is_null().to_numpy()
 
     @property
     def _hasna(self) -> bool:
-        return self._pa_array.null_count > 0
+        return self._chunked_array.null_count > 0
 
     # We do not implement it yet, neither ArrowExtensionArray does for struct arrays
     def interpolate(
         self,
         *,
         method: InterpolateOptions,
         axis: int,
@@ -351,47 +351,47 @@
             When `indices` contains negative values other than ``-1``
             and `allow_fill` is True.
         """
         # Massively adopted from ArrowExtensionArray
 
         indices_array = np.asanyarray(indices)
 
-        if len(self._pa_array) == 0 and (indices_array >= 0).any():
+        if len(self._chunked_array) == 0 and (indices_array >= 0).any():
             raise IndexError("cannot do a non-empty take from empty array")
-        if indices_array.size > 0 and indices_array.max() >= len(self._pa_array):
+        if indices_array.size > 0 and indices_array.max() >= len(self._chunked_array):
             raise IndexError("out of bounds value in 'indices'.")
 
         if allow_fill:
             fill_value = self._box_pa_scalar(fill_value, pa_type=self._pyarrow_dtype)
 
             fill_mask = indices_array < 0
             if not fill_mask.any():
                 # Nothing to fill
-                return type(self)(self._pa_array.take(indices))
-            validate_indices(indices_array, len(self._pa_array))
+                return type(self)(self._chunked_array.take(indices))
+            validate_indices(indices_array, len(self._chunked_array))
             indices_array = pa.array(indices_array, mask=fill_mask)
 
-            result = self._pa_array.take(indices_array)
+            result = self._chunked_array.take(indices_array)
             if not pa.compute.is_null(fill_value).as_py():
                 result = pa.compute.if_else(fill_mask, fill_value, result)
             return type(self)(result)
 
         if (indices_array < 0).any():
             # Don't modify in-place
             indices_array = np.copy(indices_array)
-            indices_array[indices_array < 0] += len(self._pa_array)
-        return type(self)(self._pa_array.take(indices_array))
+            indices_array[indices_array < 0] += len(self._chunked_array)
+        return type(self)(self._chunked_array.take(indices_array))
 
     def copy(self) -> Self:  # type: ignore[name-defined] # noqa: F821
         """Return a copy of the extension array.
 
         This implementation returns a shallow copy of the extension array,
         because the underlying PyArrow array is immutable.
         """
-        return type(self)(self._pa_array)
+        return type(self)(self._chunked_array)
 
     def _formatter(self, boxed: bool = False) -> Callable[[Any], str | None]:
         # TODO: make formatted strings more pretty
         # https://github.com/lincc-frameworks/nested-pandas/issues/50
         if boxed:
 
             def box_formatter(value):
@@ -401,15 +401,15 @@
                 return str(scalar.as_py())
 
             return box_formatter
         return repr
 
     @classmethod
     def _concat_same_type(cls, to_concat: Sequence[Self]) -> Self:  # type: ignore[name-defined] # noqa: F821
-        chunks = [chunk for array in to_concat for chunk in array._pa_array.iterchunks()]
+        chunks = [chunk for array in to_concat for chunk in array._chunked_array.iterchunks()]
         pa_array = pa.chunked_array(chunks)
         return cls(pa_array)
 
     def equals(self, other) -> bool:
         """
         Check equality with another NestedExtensionArray.
 
@@ -421,46 +421,46 @@
         Returns
         -------
         bool
             Whether the two NestedExtensionArrays are equal.
         """
         if not isinstance(other, type(self)):
             return False
-        return self._pa_array == other._pa_array
+        return self._chunked_array == other._chunked_array
 
     def dropna(self) -> Self:
         """Return a new ExtensionArray with missing values removed.
 
         Note that this applies to the top-level struct array, not to the list arrays.
         """
-        return type(self)(pa.compute.drop_null(self._pa_array))
+        return type(self)(pa.compute.drop_null(self._chunked_array))
 
     # End of ExtensionArray overrides #
 
     # Additional magic methods #
 
     def __arrow_array__(self, type=None):
         """Convert the extension array to a PyArrow array."""
         if type is None:
-            return self._pa_array
-        return self._pa_array.cast(type)
+            return self._chunked_array
+        return self._chunked_array.cast(type)
 
     def __array__(self, dtype=None):
         """Convert the extension array to a numpy array."""
         return self.to_numpy(dtype=dtype, copy=False)
 
     # Adopted from ArrowExtensionArray
     def __getstate__(self):
         state = self.__dict__.copy()
-        state["_pa_array"] = self._pa_array.combine_chunks()
+        state["_chunked_array"] = self._chunked_array.combine_chunks()
         return state
 
     # Adopted from ArrowExtensionArray
     def __setstate__(self, state):
-        state["_pa_array"] = pa.chunked_array(state["_pa_array"])
+        state["_chunked_array"] = pa.chunked_array(state["_chunked_array"])
         self.__dict__.update(state)
 
     # End of Additional magic methods #
 
     @classmethod
     def _box_pa_scalar(cls, value, *, pa_type: pa.DataType | None) -> pa.Scalar:
         """Convert a value to a PyArrow scalar with the specified type."""
@@ -474,15 +474,15 @@
             return convert_df_to_pa_scalar(value, pa_type=pa_type)
         return pa.scalar(value, type=pa_type, from_pandas=True)
 
     @classmethod
     def _box_pa_array(cls, value, *, pa_type: pa.DataType | None) -> pa.Array | pa.ChunkedArray:
         """Convert a value to a PyArrow array with the specified type."""
         if isinstance(value, cls):
-            pa_array = value._pa_array
+            pa_array = value._chunked_array
         elif isinstance(value, (pa.Array, pa.ChunkedArray)):
             pa_array = value
         else:
             try:
                 pa_array = pa.array(value, type=pa_type)
             except (ValueError, TypeError, KeyError):
                 scalars: list[pa.Scalar] = []
@@ -516,25 +516,25 @@
         of the same lengths.
         """
         if pa.compute.is_null(value).as_py():
             return na_value
         d = {name: pd.Series(list_scalar.values, copy=copy) for name, list_scalar in value.items()}
         return pd.DataFrame(d, copy=False)
 
-    _pa_array: pa.ChunkedArray
+    _chunked_array: pa.ChunkedArray
     _dtype: NestedDtype
 
     def __init__(self, values: pa.Array | pa.ChunkedArray, *, validate: bool = True) -> None:
         if isinstance(values, pa.Array):
             values = pa.chunked_array([values])
 
         if validate:
             self._validate(values)
 
-        self._pa_array = values
+        self._chunked_array = values
         self._dtype = NestedDtype(values.type)
 
     @classmethod
     def from_sequence(cls, scalars, *, dtype: NestedDtype | pd.ArrowDtype | pa.DataType = None) -> Self:  # type: ignore[name-defined] # noqa: F821
         """Construct a NestedExtensionArray from a sequence of items
 
         Parameters
@@ -554,14 +554,19 @@
         return cls._from_sequence(scalars, dtype=dtype)
 
     @property
     def _pyarrow_dtype(self) -> pa.DataType:
         """PyArrow data type of the extension array"""
         return self._dtype.pyarrow_dtype
 
+    @property
+    def chunked_array(self) -> pa.ChunkedArray:
+        """The underlying PyArrow ChunkedArray"""
+        return self._chunked_array
+
     @staticmethod
     def _validate(array: pa.ChunkedArray) -> None:
         """Raises ValueError if the input array is not a struct array with all fields being
         list arrays of the same lengths.
         """
         for chunk in array.iterchunks():
             if not pa.types.is_struct(chunk.type):
@@ -585,158 +590,253 @@
     @classmethod
     def from_arrow_ext_array(cls, array: ArrowExtensionArray) -> Self:  # type: ignore[name-defined] # noqa: F821
         """Create a NestedExtensionArray from pandas' ArrowExtensionArray"""
         return cls(array._pa_array)
 
     def to_arrow_ext_array(self) -> ArrowExtensionArray:
         """Convert the extension array to pandas' ArrowExtensionArray"""
-        return ArrowExtensionArray(self._pa_array)
+        return ArrowExtensionArray(self._chunked_array)
 
-    def _replace_pa_array(self, pa_array: pa.ChunkedArray, *, validate: bool) -> None:
+    def _replace_chunked_array(self, pa_array: pa.ChunkedArray, *, validate: bool) -> None:
         if validate:
             self._validate(pa_array)
-        self._pa_array = pa_array
+        self._chunked_array = pa_array
         self._dtype = NestedDtype(pa_array.chunk(0).type)
 
     @property
-    def list_offsets(self) -> pa.ChunkedArray:
+    def list_offsets(self) -> pa.Array:
         """The list offsets of the field arrays.
 
         It is a chunk array of list offsets of the first field array.
         (Since all fields are validated to have the same offsets.)
 
         Returns
         -------
         pa.ChunkedArray
             The list offsets of the field arrays.
         """
-        return pa.chunked_array([chunk.field(0).offsets for chunk in self._pa_array.iterchunks()])
+        # Quick and cheap path for a single chunk
+        if self._chunked_array.num_chunks == 1:
+            struct_array = cast(pa.StructArray, self._chunked_array.chunk(0))
+            return cast(pa.ListArray, struct_array.field(0)).offsets
+
+        chunks = []
+        # The offset of the current chunk in the flat array.
+        # Offset arrays use int32 type, so we cast to it
+        chunk_offset = pa.scalar(0, type=pa.int32())
+        for chunk in self._chunked_array.iterchunks():
+            list_array = cast(pa.ListArray, chunk.field(0))
+            if chunk_offset.equals(pa.scalar(0, type=pa.int32())):
+                offsets = list_array.offsets
+            else:
+                offsets = pa.compute.add(list_array.offsets[1:], chunk_offset)
+            chunks.append(offsets)
+            chunk_offset = offsets[-1]
+        return pa.concat_arrays(chunks)
 
     @property
     def field_names(self) -> list[str]:
         """Names of the nested columns"""
-        return [field.name for field in self._pa_array.chunk(0).type]
+        return [field.name for field in self._chunked_array.chunk(0).type]
 
     @property
     def flat_length(self) -> int:
         """Length of the flat arrays"""
-        return sum(chunk.field(0).value_lengths().sum().as_py() for chunk in self._pa_array.iterchunks())
+        return sum(chunk.field(0).value_lengths().sum().as_py() for chunk in self._chunked_array.iterchunks())
+
+    @property
+    def num_chunks(self) -> int:
+        """Number of chunks in underlying pyarrow.ChunkedArray"""
+        return self._chunked_array.num_chunks
+
+    def iter_field_lists(self, field: str) -> Generator[np.ndarray, None, None]:
+        """Iterate over single field nested lists, as numpy arrays
+
+        Parameters
+        ----------
+        field : str
+            The name of the field to iterate over.
+
+        Yields
+        ------
+        np.ndarray
+            The numpy array view over a list scalar.
+        """
+        for chunk in self._chunked_array.iterchunks():
+            struct_array: pa.StructArray = cast(pa.StructArray, chunk)
+            list_array: pa.ListArray = cast(pa.ListArray, struct_array.field(field))
+            for list_scalar in list_array:
+                yield np.asarray(list_scalar.values)
 
     def view_fields(self, fields: str | list[str]) -> Self:  # type: ignore[name-defined] # noqa: F821
-        """Get a view of the series with only the specified fields
+        """Get a view of the extension array with only the specified fields
 
         Parameters
         ----------
         fields : str or list of str
             The name of the field or a list of names of the fields to include.
 
         Returns
         -------
         NestedExtensionArray
-            The view of the series with only the specified fields.
+            The view of the array with only the specified fields.
         """
         if isinstance(fields, str):
             fields = [fields]
         if len(set(fields)) != len(fields):
             raise ValueError("Duplicate field names are not allowed")
         if not set(fields).issubset(self.field_names):
             raise ValueError(f"Some fields are not found, given: {fields}, available: {self.field_names}")
 
         chunks = []
-        for chunk in self._pa_array.iterchunks():
+        for chunk in self._chunked_array.iterchunks():
             chunk = cast(pa.StructArray, chunk)
             struct_dict = {}
             for field in fields:
                 struct_dict[field] = chunk.field(field)
             struct_array = pa.StructArray.from_arrays(struct_dict.values(), struct_dict.keys())
             chunks.append(struct_array)
         pa_array = pa.chunked_array(chunks)
 
         return self.__class__(pa_array, validate=False)
 
-    def set_flat_field(self, field: str, value: ArrayLike) -> None:
+    def set_flat_field(self, field: str, value: ArrayLike, *, keep_dtype: bool = False) -> None:
         """Set the field from flat-array of values
 
+        Note that if this updates the dtype, it would not affect the dtype of
+        the pd.Series back-ended by this extension array.
+
         Parameters
         ----------
         field : str
             The name of the field.
         value : ArrayLike
             The 'flat' array of values to be set.
+        keep_dtype : bool, default False
+            Whether to keep the original dtype of the field. If True,
+            now new field will be created, and the dtype of the existing
+            field will be kept. If False, the dtype of the field will be
+            inferred from the input value.
         """
         # TODO: optimize for the case when the input is a pa.ChunkedArray
 
+        if keep_dtype:
+            if field not in self.field_names:
+                raise ValueError(
+                    "If keep_dtype is True, the field must exist in the series. "
+                    f"Got: {field}, available: {self.field_names}"
+                )
+            # Get the current element type of list-array
+            pa_type = self._chunked_array.chunk(0).field(field).type.value_type
+        else:
+            pa_type = None
+
         if np.ndim(value) == 0:
             value = np.repeat(value, self.flat_length)
 
-        pa_array = pa.array(value)
+        try:
+            pa_array = pa.array(value, from_pandas=True, type=pa_type)
+        except (ValueError, TypeError) as e:
+            raise TypeError(
+                f"New values must be convertible to the existing element pyarrow type, {pa_type}. "
+                "If you want to replace field with values of a new type, use series.nest.with_flat_field() "
+                "or NestedExtensionArray.set_flat_field(..., keep_dtype=False) instead."
+            ) from e
 
         if len(pa_array) != self.flat_length:
             raise ValueError("The input must be a struct_scalar or have the same length as the flat arrays")
 
-        offsets = self.list_offsets.combine_chunks()
-        list_array = pa.ListArray.from_arrays(values=pa_array, offsets=offsets)
+        list_array = pa.ListArray.from_arrays(values=pa_array, offsets=self.list_offsets)
 
-        return self.set_list_field(field, list_array)
+        return self.set_list_field(field, list_array, keep_dtype=keep_dtype)
 
-    def set_list_field(self, field: str, value: ArrayLike) -> None:
+    def set_list_field(self, field: str, value: ArrayLike, *, keep_dtype: bool = False) -> None:
         """Set the field from list-array
 
+        Note that if this updates the dtype, it would not affect the dtype of
+        the pd.Series back-ended by this extension array.
+
         Parameters
         ----------
         field : str
             The name of the field.
         value : ArrayLike
             The list-array of values to be set.
+        keep_dtype : bool, default False
+            Whether to keep the original dtype of the field. If True,
+            now new field will be created, and the dtype of the existing
+            field will be kept. If False, the dtype of the field will be
+            inferred from the input value.
         """
         # TODO: optimize for the case when the input is a pa.ChunkedArray
 
-        pa_array = pa.array(value)
+        if keep_dtype:
+            if field not in self.field_names:
+                raise ValueError(
+                    "If keep_dtype is True, the field must exist in the series. "
+                    f"Got: {field}, available: {self.field_names}"
+                )
+            pa_type = self._chunked_array.chunk(0).field(field).type
+        else:
+            pa_type = None
+
+        try:
+            pa_array = pa.array(value, from_pandas=True, type=pa_type)
+        except (ValueError, TypeError) as e:
+            raise TypeError(
+                f"New values must be convertible to the existing list pyarrow type, {pa_type}. "
+                "If you want to replace field with values of a new type, use series.nest.with_list_field() "
+                "or NestedExtensionArray.set_list_field(..., keep_dtype=False) instead."
+            ) from e
 
         if not is_pa_type_a_list(pa_array.type):
             raise ValueError(f"Expected a list array, got {pa_array.type}")
 
         if len(pa_array) != len(self):
             raise ValueError("The length of the list-array must be equal to the length of the series")
 
         chunks = []
-        for sl, chunk in enumerate_chunks(self._pa_array):
+        for sl, chunk in enumerate_chunks(self._chunked_array):
             chunk = cast(pa.StructArray, chunk)
 
-            # Build a new struct array. We collect all existing fields and add the new one.
+            # Build a new struct array. We collect all existing fields and add/replace the new one.
             struct_dict = {}
             for pa_field in chunk.type:
                 struct_dict[pa_field.name] = chunk.field(pa_field.name)
-            struct_dict[field] = pa.array(pa_array[sl])
+            struct_dict[field] = pa_array[sl]
 
             struct_array = pa.StructArray.from_arrays(struct_dict.values(), struct_dict.keys())
             chunks.append(struct_array)
-        pa_array = pa.chunked_array(chunks)
+        chunked_array = pa.chunked_array(chunks)
+
+        self._replace_chunked_array(chunked_array, validate=True)
 
-        self._replace_pa_array(pa_array, validate=True)
+    def pop_fields(self, fields: Iterable[str]):
+        """Delete fields from the struct array
 
-    def pop_field(self, field: str):
-        """Delete a field from the struct array
+        Note that at least one field must be left in the struct array.
 
         Parameters
         ----------
-        field : str
-            The name of the field to be deleted.
+        fields : iterable of str
+            The names of the fields to delete.
         """
-        if field not in self.field_names:
-            raise ValueError(f"Field '{field}' not found")
+        fields = frozenset(fields)
+
+        if not fields.issubset(self.field_names):
+            raise ValueError(f"Some fields are not found, given: {fields}, available: {self.field_names}")
 
-        if len(self.field_names) == 1:
-            raise ValueError("Cannot delete the last field")
+        if len(self.field_names) - len(fields) == 0:
+            raise ValueError("Cannot delete all fields")
 
         chunks = []
-        for chunk in self._pa_array.iterchunks():
+        for chunk in self._chunked_array.iterchunks():
             chunk = cast(pa.StructArray, chunk)
             struct_dict = {}
             for pa_field in chunk.type:
-                if pa_field.name != field:
+                if pa_field.name not in fields:
                     struct_dict[pa_field.name] = chunk.field(pa_field.name)
             struct_array = pa.StructArray.from_arrays(struct_dict.values(), struct_dict.keys())
             chunks.append(struct_array)
         pa_array = pa.chunked_array(chunks)
 
-        self._replace_pa_array(pa_array, validate=False)
+        self._replace_chunked_array(pa_array, validate=False)
```

### Comparing `nested_pandas-0.1/src/nested_pandas/series/packer.py` & `nested_pandas-0.1.1/src/nested_pandas/series/packer.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,8 +293,11 @@
         raise ValueError("The index must be sorted")
 
     # pd.Index.duplicated returns False for the first occurance and True for all others.
     # So our offsets would be indexes of these False values with the array length in the end.
     offset_but_last = np.nonzero(~index.duplicated(keep="first"))[0]
     offset = np.append(offset_but_last, len(index))
 
+    # Arrow uses int32 for offsets
+    offset = offset.astype(np.int32)
+
     return offset
```

### Comparing `nested_pandas-0.1/src/nested_pandas/series/utils.py` & `nested_pandas-0.1.1/src/nested_pandas/series/utils.py`

 * *Files identical despite different names*

### Comparing `nested_pandas-0.1/src/nested_pandas/utils/utils.py` & `nested_pandas-0.1.1/src/nested_pandas/utils/utils.py`

 * *Files identical despite different names*

### Comparing `nested_pandas-0.1/src/nested_pandas.egg-info/PKG-INFO` & `nested_pandas-0.1.1/src/nested_pandas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nested-pandas
-Version: 0.1
+Version: 0.1.1
 Author-email: LINCC Frameworks <brantd@uw.edu>
 License: MIT License
         
         Copyright (c) 2023 LINCC Frameworks
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -43,14 +43,22 @@
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 
 # nested-pandas
+
+[![Template](https://img.shields.io/badge/Template-LINCC%20Frameworks%20Python%20Project%20Template-brightgreen)](https://lincc-ppt.readthedocs.io/en/latest/)
+
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/lincc-frameworks/nested-pandas/smoke-test.yml)](https://github.com/lincc-frameworks/nested-pandas/actions/workflows/smoke-test.yml)
+[![codecov](https://codecov.io/gh/lincc-frameworks/nested-pandas/branch/main/graph/badge.svg)](https://codecov.io/gh/lincc-frameworks/nested-pandas)
+[![Read the Docs](https://img.shields.io/readthedocs/nested-pandas)](https://nested-pandas.readthedocs.io/)
+[![benchmarks](https://img.shields.io/github/actions/workflow/status/lincc-frameworks/nested-pandas/asv-main.yml?label=benchmarks)](https://lincc-frameworks.github.io/nested-pandas/)
+
 An extension of pandas for efficient representation of nested
 associated datasets.
 
 Nested-Pandas extends the [pandas](https://pandas.pydata.org/) package with 
 tooling and support for nested dataframes packed into values of top-level 
 dataframe columns. [Pyarrow](https://arrow.apache.org/docs/python/index.html) 
 is used internally to aid in scalability and performance.
@@ -69,17 +77,10 @@
 
 
 
 This is a LINCC Frameworks project - find more information about LINCC Frameworks [here](https://lsstdiscoveryalliance.org/programs/lincc-frameworks/).
 
 
 
-[![Template](https://img.shields.io/badge/Template-LINCC%20Frameworks%20Python%20Project%20Template-brightgreen)](https://lincc-ppt.readthedocs.io/en/latest/)
-
-[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/lincc-frameworks/nested-pandas/smoke-test.yml)](https://github.com/lincc-frameworks/nested-pandas/actions/workflows/smoke-test.yml)
-[![codecov](https://codecov.io/gh/lincc-frameworks/nested-pandas/branch/main/graph/badge.svg)](https://codecov.io/gh/lincc-frameworks/nested-pandas)
-[![Read the Docs](https://img.shields.io/readthedocs/nested-pandas)](https://nested-pandas.readthedocs.io/)
-[![benchmarks](https://img.shields.io/github/actions/workflow/status/lincc-frameworks/nested-pandas/asv-main.yml?label=benchmarks)](https://lincc-frameworks.github.io/nested-pandas/)
-
 ## Acknowledgements
 
 This project is supported by Schmidt Sciences.
```

### Comparing `nested_pandas-0.1/src/nested_pandas.egg-info/SOURCES.txt` & `nested_pandas-0.1.1/src/nested_pandas.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 src/nested_pandas/series/ext_array.py
 src/nested_pandas/series/packer.py
 src/nested_pandas/series/utils.py
 src/nested_pandas/utils/__init__.py
 src/nested_pandas/utils/utils.py
 tests/nested_pandas/conftest.py
 tests/nested_pandas/datasets/test_generation.py
+tests/nested_pandas/e2e_tests/test_issue89.py
 tests/nested_pandas/nestedframe/test_io.py
 tests/nested_pandas/nestedframe/test_nestedframe.py
 tests/nested_pandas/nestedframe/test_nestedframe_utils.py
 tests/nested_pandas/series/test_accessor.py
 tests/nested_pandas/series/test_dtype.py
 tests/nested_pandas/series/test_ext_array.py
 tests/nested_pandas/series/test_packer.py
```

### Comparing `nested_pandas-0.1/tests/nested_pandas/datasets/test_generation.py` & `nested_pandas-0.1.1/tests/nested_pandas/datasets/test_generation.py`

 * *Files identical despite different names*

### Comparing `nested_pandas-0.1/tests/nested_pandas/nestedframe/test_io.py` & `nested_pandas-0.1.1/tests/nested_pandas/nestedframe/test_io.py`

 * *Files identical despite different names*

### Comparing `nested_pandas-0.1/tests/nested_pandas/nestedframe/test_nestedframe.py` & `nested_pandas-0.1.1/tests/nested_pandas/nestedframe/test_nestedframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 import pandas as pd
+import pyarrow as pa
 import pytest
 from nested_pandas import NestedFrame
 from pandas.testing import assert_frame_equal
 
 
 def test_nestedframe_construction():
     """Test NestedFrame construction"""
@@ -126,14 +127,27 @@
 
     base = base.add_nested(nested, "nested")
 
     assert "nested" in base.columns
     assert pd.isna(base.loc[1]["nested"])
 
 
+def test_add_nested_for_empty_df():
+    """Test that .add_nested() works for empty frame and empty input"""
+    base = NestedFrame(data={"a": [], "b": []}, index=[])
+    nested = pd.DataFrame(data={"c": []}, index=[])
+    new_base = base.add_nested(nested, "nested")
+
+    # Check original frame is unchanged
+    assert_frame_equal(base, NestedFrame(data={"a": [], "b": []}, index=[]))
+
+    assert "nested" in new_base.columns
+    assert_frame_equal(new_base.nested.nest.to_flat(), nested.astype(pd.ArrowDtype(pa.float64())))
+
+
 def test_query():
     """Test that NestedFrame.query handles nested queries correctly"""
 
     base = NestedFrame(data={"a": [1, 2, 3], "b": [2, 4, 6]}, index=[0, 1, 2])
 
     nested = pd.DataFrame(
         data={"c": [0, 2, 4, 1, 4, 3, 1, 4, 1], "d": [5, 4, 7, 5, 3, 1, 9, 3, 4]},
```

### Comparing `nested_pandas-0.1/tests/nested_pandas/series/test_accessor.py` & `nested_pandas-0.1.1/tests/nested_pandas/series/test_accessor.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import pandas as pd
 import pyarrow as pa
 import pytest
 from nested_pandas import NestedDtype
 from nested_pandas.series.ext_array import NestedExtensionArray
-from nested_pandas.series.packer import pack_flat
+from nested_pandas.series.packer import pack_flat, pack_seq
 from numpy.testing import assert_array_equal
 from pandas.testing import assert_frame_equal, assert_index_equal, assert_series_equal
 
 
 def test_registered():
     """Test that the series accessor .nest is registered."""
     struct_array = pa.StructArray.from_arrays(
@@ -66,14 +66,47 @@
                 index=[0, 1],
             ),
         },
     )
     assert_frame_equal(lists, desired)
 
 
+def test_to_lists_for_chunked_array():
+    """ ""Test that the .nest.to_lists() when underlying array is chunked"""
+    struct_array = pa.StructArray.from_arrays(
+        arrays=[
+            [np.array([1.0, 2.0, 3.0]), -np.array([1.0, 2.0, 1.0])],
+            [np.array([4.0, 5.0, 6.0]), -np.array([3.0, 4.0, 5.0])],
+        ],
+        names=["a", "b"],
+    )
+    chunked_array = pa.chunked_array([struct_array] * 3)
+    assert chunked_array.length() == 6
+    series = pd.Series(chunked_array, dtype=NestedDtype(chunked_array.type), index=[0, 1, 2, 3, 4, 5])
+    assert series.array.num_chunks == 3
+
+    lists = series.nest.to_lists()
+
+    desired = pd.DataFrame(
+        data={
+            "a": pd.Series(
+                data=[np.array([1.0, 2.0, 3.0]), -np.array([1.0, 2.0, 1.0])] * 3,
+                dtype=pd.ArrowDtype(pa.list_(pa.float64())),
+                index=[0, 1, 2, 3, 4, 5],
+            ),
+            "b": pd.Series(
+                data=[np.array([4.0, 5.0, 6.0]), -np.array([3.0, 4.0, 5.0])] * 3,
+                dtype=pd.ArrowDtype(pa.list_(pa.float64())),
+                index=[0, 1, 2, 3, 4, 5],
+            ),
+        },
+    )
+    assert_frame_equal(lists, desired)
+
+
 def test_to_lists_with_fields():
     """Test that the .nest.to_lists(fields=...) method works."""
     struct_array = pa.StructArray.from_arrays(
         arrays=[
             pa.array([np.array([1.0, 2.0, 3.0]), -np.array([1.0, 2.0, 1.0])]),
             pa.array([np.array([4.0, 5.0, 6.0]), -np.array([3.0, 4.0, 5.0])]),
         ],
@@ -150,14 +183,51 @@
     assert_array_equal(flat.index, desired.index)
     assert flat.index.name == desired.index.name
 
     for column in flat.columns:
         assert_array_equal(flat[column], desired[column])
 
 
+def test_to_flat_for_chunked_array():
+    """Test that the .nest.to_flat() when underlying array is pa.ChunkedArray."""
+    struct_array = pa.StructArray.from_arrays(
+        arrays=[
+            [np.array([1.0, 2.0, 3.0]), -np.array([1.0, 2.0, 1.0])],
+            [np.array([4.0, 5.0, 6.0]), -np.array([3.0, 4.0, 5.0])],
+        ],
+        names=["a", "b"],
+    )
+    chunked_array = pa.chunked_array([struct_array] * 3)
+    assert chunked_array.length() == 6
+    series = pd.Series(chunked_array, dtype=NestedDtype(chunked_array.type), index=[0, 1, 2, 3, 4, 5])
+    assert series.array.num_chunks == 3
+
+    flat = series.nest.to_flat()
+
+    desired = pd.DataFrame(
+        data={
+            "a": pd.Series(
+                data=[1.0, 2.0, 3.0, -1.0, -2.0, -1.0] * 3,
+                name="a",
+                index=np.repeat([0, 1, 2, 3, 4, 5], 3),
+                dtype=pd.ArrowDtype(pa.float64()),
+            ),
+            "b": pd.Series(
+                data=[4.0, 5.0, 6.0, -3.0, -4.0, -5.0] * 3,
+                name="b",
+                index=np.repeat([0, 1, 2, 3, 4, 5], 3),
+                dtype=pd.ArrowDtype(pa.float64()),
+            ),
+        },
+        index=pd.Index(np.repeat([0, 1, 2, 3, 4, 5], 3)),
+    )
+
+    assert_frame_equal(flat, desired)
+
+
 def test_to_flat_with_fields():
     """Test that the .nest.to_flat(fields=...) method works."""
     struct_array = pa.StructArray.from_arrays(
         arrays=[
             pa.array([np.array([1.0, 2.0, 3.0]), np.array([1.0, 2.0, 1.0])]),
             pa.array([-np.array([4.0, 5.0, 6.0]), -np.array([3.0, 4.0, 5.0])]),
         ],
@@ -225,85 +295,157 @@
         names=["a", "b"],
     )
     series = pd.Series(struct_array, dtype=NestedDtype(struct_array.type), index=[0, 1])
 
     assert series.nest.flat_length == 6
 
 
-def test_set_flat_field():
+def test_with_flat_field():
     """Test that the .nest.set_flat_field() method works."""
     struct_array = pa.StructArray.from_arrays(
         arrays=[
             pa.array([np.array([1.0, 2.0, 3.0]), np.array([1.0, 2.0, 1.0])]),
             pa.array([-np.array([4.0, 5.0, 6.0]), -np.array([3.0, 4.0, 5.0])]),
         ],
         names=["a", "b"],
     )
     series = pd.Series(struct_array, dtype=NestedDtype(struct_array.type), index=[0, 1])
 
-    series.nest.set_flat_field("a", np.array(["a", "b", "c", "d", "e", "f"]))
+    new_series = series.nest.with_flat_field("a", np.array(["a", "b", "c", "d", "e", "f"]))
 
     assert_series_equal(
-        series.nest["a"],
+        new_series.nest["a"],
         pd.Series(
             data=["a", "b", "c", "d", "e", "f"],
             index=[0, 0, 0, 1, 1, 1],
             name="a",
             dtype=pd.ArrowDtype(pa.string()),
         ),
     )
 
 
-def test_set_list_field():
+def test_with_field():
+    """Test that .nest.with_field is just an alias to .nest.with_flat_field."""
+    struct_array = pa.StructArray.from_arrays(
+        arrays=[
+            pa.array([np.array([1.0, 2.0, 3.0]), np.array([1.0, 2.0, 1.0])]),
+            pa.array([-np.array([4.0, 5.0, 6.0]), -np.array([3.0, 4.0, 5.0])]),
+        ],
+        names=["a", "b"],
+    )
+    series = pd.Series(struct_array, dtype=NestedDtype(struct_array.type), index=[0, 1])
+    assert_series_equal(
+        series.nest.with_field("a", np.array(["a", "b", "c", "d", "e", "f"])),
+        series.nest.with_flat_field("a", np.array(["a", "b", "c", "d", "e", "f"])),
+    )
+
+
+def test_with_list_field():
     """Test that the .nest.set_list_field() method works."""
     struct_array = pa.StructArray.from_arrays(
         arrays=[
             pa.array([np.array([1.0, 2.0, 3.0]), np.array([1.0, 2.0, 1.0])]),
             pa.array([-np.array([4.0, 5.0, 6.0]), -np.array([3.0, 4.0, 5.0])]),
         ],
         names=["a", "b"],
     )
     series = pd.Series(struct_array, dtype=NestedDtype(struct_array.type), index=[0, 1])
 
-    series.nest.set_list_field("c", [["a", "b", "c"], ["d", "e", "f"]])
+    new_series = series.nest.with_list_field("c", [["a", "b", "c"], ["d", "e", "f"]])
 
     assert_series_equal(
-        series.nest["c"],
+        new_series.nest["c"],
         pd.Series(
             data=["a", "b", "c", "d", "e", "f"],
             index=[0, 0, 0, 1, 1, 1],
             name="c",
             dtype=pd.ArrowDtype(pa.string()),
         ),
     )
 
 
-def test_pop_field():
-    """Test that the .nest.pop_field() method works."""
+def test_without_field_single_field():
+    """Test .nest.without_field("field")"""
     struct_array = pa.StructArray.from_arrays(
         arrays=[
-            pa.array([np.array([1.0, 2.0, 3.0]), np.array([1.0, 2.0, 1.0])]),
-            pa.array([-np.array([4.0, 5.0, 6.0]), -np.array([3.0, 4.0, 5.0])]),
+            pa.array([np.array([1, 2, 3]), np.array([4, 5, 6])]),
+            pa.array([np.array([6, 4, 2]), np.array([1, 2, 3])]),
         ],
         names=["a", "b"],
     )
-    series = pd.Series(struct_array, dtype=NestedDtype(struct_array.type), index=[0, 1])
+    series = pd.Series(struct_array, dtype=NestedDtype(struct_array.type), index=[5, 7])
 
-    a = series.nest.pop_field("a")
+    new_series = series.nest.without_field("a")
 
-    assert_array_equal(series.nest.fields, ["b"])
-    assert_series_equal(
-        a,
-        pd.Series(
-            [1.0, 2.0, 3.0, 1.0, 2.0, 1.0],
-            dtype=pd.ArrowDtype(pa.float64()),
-            index=[0, 0, 0, 1, 1, 1],
-            name="a",
-        ),
+    desired_struct_array = pa.StructArray.from_arrays(
+        arrays=[
+            pa.array([np.array([6, 4, 2]), np.array([1, 2, 3])]),
+        ],
+        names=["b"],
     )
+    desired = pd.Series(desired_struct_array, dtype=NestedDtype(desired_struct_array.type), index=[5, 7])
+
+    assert_series_equal(new_series, desired)
+
+
+def test_without_field_multiple_fields():
+    """Test .nest.without_field(["field1", "field2"])"""
+    struct_array = pa.StructArray.from_arrays(
+        arrays=[
+            pa.array([np.array([1, 2, 3]), np.array([4, 5, 6])]),
+            pa.array([np.array([6, 4, 2]), np.array([1, 2, 3])]),
+            pa.array([["a", "b", "c"], ["d", "e", "f"]]),
+        ],
+        names=["a", "b", "c"],
+    )
+    series = pd.Series(struct_array, dtype=NestedDtype(struct_array.type), index=[5, 7])
+
+    new_series = series.nest.without_field(["a", "b"])
+
+    desired_struct_array = pa.StructArray.from_arrays(
+        arrays=[
+            pa.array([["a", "b", "c"], ["d", "e", "f"]]),
+        ],
+        names=["c"],
+    )
+    desired = pd.Series(desired_struct_array, dtype=NestedDtype(desired_struct_array.type), index=[5, 7])
+
+    assert_series_equal(new_series, desired)
+
+
+def test_without_field_raises_for_missing_field():
+    """Test .nest.without_field("field") raises for missing field."""
+    struct_array = pa.StructArray.from_arrays(
+        arrays=[
+            pa.array([np.array([1, 2, 3]), np.array([4, 5, 6])]),
+            pa.array([np.array([6, 4, 2]), np.array([1, 2, 3])]),
+            pa.array([["a", "b", "c"], ["d", "e", "f"]]),
+        ],
+        names=["a", "b", "c"],
+    )
+    series = pd.Series(struct_array, dtype=NestedDtype(struct_array.type), index=[5, 7])
+
+    with pytest.raises(ValueError):
+        _ = series.nest.without_field("d")
+
+
+def test_without_field_raises_for_missing_fields():
+    """Test .nest.without_field(["field1", "field2"]) raises for missing fields."""
+    struct_array = pa.StructArray.from_arrays(
+        arrays=[
+            pa.array([np.array([1, 2, 3]), np.array([4, 5, 6])]),
+            pa.array([np.array([6, 4, 2]), np.array([1, 2, 3])]),
+            pa.array([["a", "b", "c"], ["d", "e", "f"]]),
+        ],
+        names=["a", "b", "c"],
+    )
+    series = pd.Series(struct_array, dtype=NestedDtype(struct_array.type), index=[5, 7])
+
+    with pytest.raises(ValueError):
+        _ = series.nest.without_field(["a", "d"])
 
 
 def test_query_flat_1():
     """Test that the .nest.query_flat() method works."""
     struct_array = pa.StructArray.from_arrays(
         arrays=[
             pa.array([np.array([1.0, 2.0, 3.0]), np.array([4.0, 5.0, 6.0])]),
@@ -385,14 +527,28 @@
             dtype=pd.ArrowDtype(pa.list_(pa.int64())),
             index=[5, 7],
             name="a",
         ),
     )
 
 
+def test_get():
+    """Test .nest.get() which is implemented by the base class"""
+    series = pack_seq(
+        [
+            pd.DataFrame({"a": [1, 2, 3], "b": [1.0, 5.0, 6.0]}),
+            pd.DataFrame({"a": [1, 2], "b": [None, 0.0]}),
+            None,
+        ]
+    )
+    assert_series_equal(series.nest.get("a"), series.nest.to_flat()["a"])
+    assert_series_equal(series.nest.get("b"), series.nest.to_flat()["b"])
+    assert series.nest.get("c", "default_value") == "default_value"
+
+
 def test___getitem___single_field():
     """Test that the .nest["field"] works for a single field."""
     struct_array = pa.StructArray.from_arrays(
         arrays=[
             pa.array([np.array([1.0, 2.0, 3.0]), np.array([1.0, 2.0, 1.0])]),
             pa.array([-np.array([4.0, 5.0, 6.0]), -np.array([3.0, 4.0, 5.0])]),
         ],
@@ -457,23 +613,23 @@
             pa.array([np.array([1.0, 2.0, 3.0]), np.array([1.0, 2.0, 1.0])]),
             pa.array([-np.array([4.0, 5.0, 6.0]), -np.array([3.0, 4.0, 5.0])]),
         ],
         names=["a", "b"],
     )
     series = pd.Series(struct_array, dtype=NestedDtype(struct_array.type), index=[0, 1])
 
-    series.nest["a"] = np.array(["a", "b", "c", "d", "e", "f"])
+    series.nest["a"] = np.arange(6, 0, -1)
 
     assert_series_equal(
         series.nest["a"],
         pd.Series(
-            data=["a", "b", "c", "d", "e", "f"],
+            data=[6, 5, 4, 3, 2, 1],
             index=[0, 0, 0, 1, 1, 1],
             name="a",
-            dtype=pd.ArrowDtype(pa.string()),
+            dtype=pd.ArrowDtype(pa.float64()),
         ),
     )
 
 
 def test___setitem___with_series_with_index():
     """Test that the .nest["field"] = pd.Series(...) works for a single field."""
     struct_array = pa.StructArray.from_arrays(
@@ -482,39 +638,39 @@
             pa.array([-np.array([4.0, 5.0, 6.0]), -np.array([3.0, 4.0, 5.0])]),
         ],
         names=["a", "b"],
     )
     series = pd.Series(struct_array, dtype=NestedDtype(struct_array.type), index=[0, 1])
 
     flat_series = pd.Series(
-        data=["a", "b", "c", "d", "e", "f"],
+        data=np.arange(6, 0, -1),
         index=[0, 0, 0, 1, 1, 1],
         name="a",
-        dtype=pd.ArrowDtype(pa.string()),
+        dtype=pd.ArrowDtype(pa.float32()),
     )
 
     series.nest["a"] = flat_series
 
     assert_series_equal(
         series.nest["a"],
-        flat_series,
+        flat_series.astype(pd.ArrowDtype(pa.float64())),
     )
     assert_series_equal(
         series.nest.get_list_series("a"),
         pd.Series(
-            data=[np.array(["a", "b", "c"]), np.array(["d", "e", "f"])],
-            dtype=pd.ArrowDtype(pa.list_(pa.string())),
+            data=[np.array([6, 5, 4]), np.array([3, 2, 1])],
+            dtype=pd.ArrowDtype(pa.list_(pa.float64())),
             index=[0, 1],
             name="a",
         ),
     )
 
 
 def test___setitem___empty_series():
-    """Test that the series.nest["field"] = [] for empty series."""
+    """Test that series.nest["field"] = [] does nothing for empty series."""
     empty_series = pd.Series([], dtype=NestedDtype.from_fields({"a": pa.float64()}))
     empty_series.nest["a"] = []
     assert len(empty_series) == 0
 
 
 def test___setitem___with_single_value():
     """Test series.nest["field"] = const"""
@@ -523,26 +679,42 @@
             pa.array([np.array([1.0, 2.0, 3.0])]),
             pa.array([-np.array([4.0, 5.0, 6.0])]),
         ],
         names=["a", "b"],
     )
     series = pd.Series(struct_array, dtype=NestedDtype(struct_array.type), index=[0])
 
-    series.nest["a"] = 1.0
+    series.nest["a"] = -1.0
+
     assert_series_equal(
         series.nest["a"],
         pd.Series(
-            data=[1.0, 1.0, 1.0],
+            data=[-1.0, -1.0, -1.0],
             index=[0, 0, 0],
             name="a",
             dtype=pd.ArrowDtype(pa.float64()),
         ),
     )
 
 
+def test___setitem___raises_for_wrong_dtype():
+    """Test that the .nest["field"] = ... raises for a wrong dtype."""
+    struct_array = pa.StructArray.from_arrays(
+        arrays=[
+            pa.array([np.array([1.0, 2.0, 3.0]), np.array([1.0, 2.0, 1.0])]),
+            pa.array([-np.array([4.0, 5.0, 6.0]), -np.array([3.0, 4.0, 5.0])]),
+        ],
+        names=["a", "b"],
+    )
+    series = pd.Series(struct_array, dtype=NestedDtype(struct_array.type), index=[0, 1])
+
+    with pytest.raises(TypeError):
+        series.nest["a"] = np.array(["a", "b", "c", "d", "e", "f"])
+
+
 def test___setitem___raises_for_wrong_length():
     """Test that the .nest["field"] = ... raises for a wrong length."""
     struct_array = pa.StructArray.from_arrays(
         arrays=[
             pa.array([np.array([1.0, 2.0, 3.0]), np.array([1.0, 2.0, 1.0])]),
             pa.array([-np.array([4.0, 5.0, 6.0]), -np.array([3.0, 4.0, 5.0])]),
         ],
@@ -572,28 +744,34 @@
         dtype=pd.ArrowDtype(pa.float64()),
     )
 
     with pytest.raises(ValueError):
         series.nest["a"] = flat_series
 
 
-def test___delitem__():
-    """Test that the `del .nest["field"]` works."""
+def test___setitem___raises_for_new_field():
+    """Test that series.nest["field"] = ... raises for a new field."""
+    series = pack_seq([{"a": [1, 2, 3]}, {"a": [4, None]}])
+    with pytest.raises(ValueError):
+        series.nest["b"] = series.nest["a"] - 1
+
+
+def test___delitem___raises():
+    """Test that the `del .nest["field"]` is not implemented."""
     struct_array = pa.StructArray.from_arrays(
         arrays=[
             pa.array([np.array([1.0, 2.0, 3.0]), np.array([1.0, 2.0, 1.0])]),
             pa.array([-np.array([4.0, 5.0, 6.0]), -np.array([3.0, 4.0, 5.0])]),
         ],
         names=["a", "b"],
     )
     series = pd.Series(struct_array, dtype=NestedDtype(struct_array.type), index=[0, 1])
 
-    del series.nest["a"]
-
-    assert_array_equal(series.nest.fields, ["b"])
+    with pytest.raises(AttributeError):
+        del series.nest["a"]
 
 
 def test___iter__():
     """Test that the iter(.nest) works."""
     struct_array = pa.StructArray.from_arrays(
         arrays=[
             pa.array([np.array([1.0, 2.0, 3.0]), np.array([1.0, 2.0, 1.0])]),
@@ -640,7 +818,101 @@
         filtered,
         pd.DataFrame(
             data={"c": [0.0, 2, 4, 1, 3, 1, 4, 1], "d": [5, 4, 7, 5, 1, 9, 3, 4]},
             index=[0, 0, 0, 1, 1, 2, 2, 2],
         ),
         check_dtype=False,  # filtered's Series are pd.ArrowDtype
     )
+
+
+def test___contains__():
+    """Test that the `"field" in .nest` works.
+
+    We haven't implemented it, but base class does
+    """
+    series = pack_seq([pd.DataFrame({"a": [1, 2, 3]})])
+    assert "a" in series.nest
+    assert "x" not in series.nest
+
+
+def test___eq__():
+    """Test that one.nest == other.nest works."""
+
+    series1 = pack_seq([pd.DataFrame({"a": [1, 2, 3]})])
+    series2 = pack_seq([pd.DataFrame({"b": [1, 2, 3]})])
+    series3 = pack_seq([pd.DataFrame({"a": [1, 2, 3, 4]})])
+    series4 = pack_seq([pd.DataFrame({"a": [1, 2, 3], "b": [3, 2, 1]})])
+
+    assert series1.nest == series1.nest
+
+    assert series2.nest == series2.nest
+    assert series1.nest != series2.nest
+
+    assert series3.nest == series3.nest
+    assert series1.nest != series3.nest
+
+    assert series4.nest == series4.nest
+    assert series1.nest != series4.nest
+
+
+def test___eq___false_for_different_types():
+    """Test that one.nest == other.nest is False for different types."""
+    seq = [{"a": [1, 2, 3]}, {"a": [4, None]}]
+    series = pack_seq(seq)
+    assert series.nest != pd.Series(seq, dtype=pd.ArrowDtype(pa.struct([("a", pa.list_(pa.int64()))])))
+
+
+def test_clear_raises():
+    """Test that .nest.clear() raises - we cannot handle nested series with no fields"""
+    series = pack_seq([pd.DataFrame({"a": [1, 2, 3], "b": [3, 2, 1]}), None])
+    with pytest.raises(NotImplementedError):
+        series.nest.clear()
+
+
+def test_popitem_raises():
+    """Test .nest.popitem() raises"""
+    series = pack_seq(
+        [pd.DataFrame({"a": [1, 2, 3], "b": [3, 2, 1]}), pd.DataFrame({"a": [1, 2], "b": [2.0, None]}), None]
+    )
+
+    with pytest.raises(AttributeError):
+        _ = series.nest.popitem()
+
+
+def test_setdefault_raises():
+    """Test .nest.setdefault() is not implemented"""
+    series = pack_seq([{"a": [1, 2, 3]}, {"a": [4, None]}])
+    with pytest.raises(AttributeError):
+        series.nest.setdefault("b", series.nest["a"] * 2.0)
+
+
+def test_update_raises():
+    """test series.nest.update(other.nest) is not implemented"""
+    series1 = pack_seq([{"a": [1, 2, 3], "b": [4, 5, 6]}, {"a": [4, None], "b": [7, 8]}])
+    series2 = pack_seq(
+        [
+            {"b": ["x", "y", "z"], "c": [-2.0, -3.0, -4.0]},
+            {"b": ["!", "?"], "c": [-5.0, -6.0]},
+        ]
+    )
+    with pytest.raises(AttributeError):
+        series1.nest.update(series2.nest)
+
+
+def test_items():
+    """Test series.nest.items() implemented by the base class"""
+    series = pack_seq([{"a": [1, 2, 3], "b": [3, 2, 1]}, {"a": [4, None], "b": [7, 8]}])
+    for key, value in series.nest.items():
+        assert_series_equal(value, series.nest[key])
+
+
+def test_keys():
+    """Test series.nest.keys() implemented by the base class"""
+    series = pack_seq([{"a": [1, 2, 3], "b": [3, 2, 1]}, {"a": [4, None], "b": [7, 8]}])
+    assert_array_equal(list(series.nest.keys()), ["a", "b"])
+
+
+def test_values():
+    """Test series.nest.values() implemented by the base class"""
+    series = pack_seq([{"a": [1, 2, 3], "b": [3, 2, 1]}, {"a": [4, None], "b": [7, 8]}])
+    for value in series.nest.values():
+        assert_series_equal(value, series.nest[value.name])
```

### Comparing `nested_pandas-0.1/tests/nested_pandas/series/test_dtype.py` & `nested_pandas-0.1.1/tests/nested_pandas/series/test_dtype.py`

 * *Files identical despite different names*

### Comparing `nested_pandas-0.1/tests/nested_pandas/series/test_ext_array.py` & `nested_pandas-0.1.1/tests/nested_pandas/series/test_ext_array.py`

 * *Files 8% similar despite different names*

```diff
@@ -200,15 +200,15 @@
     new_pa_type = pa.struct([pa.field("a", pa.list_(pa.float64())), pa.field("b", pa.list_(pa.float64()))])
 
     pa_array = pa.array(
         [{"a": a, "b": b}, {"a": a, "b": b}, None],
         type=pa_type,
     )
 
-    actual = NestedExtensionArray.from_sequence(pa_array, dtype=new_pa_type)._pa_array
+    actual = NestedExtensionArray.from_sequence(pa_array, dtype=new_pa_type).chunked_array
     desired = pa.chunked_array([pa_array.cast(new_pa_type)])
     # pyarrow doesn't convert pandas boxed missing values to nulls in nested arrays
     assert actual == desired
 
 
 def test_ext_array_dtype():
     """Test that the dtype of the extension array is correct."""
@@ -521,15 +521,15 @@
             pa.array([np.array([7, 8]), np.array([5, 6])]),
             pa.array([np.array([300.0, 400.0]), np.array([100.0, 200.0])]),
         ],
         names=["a", "b"],
     )
     desired = NestedExtensionArray(desired_struct_array)
 
-    assert ext_array._pa_array == desired._pa_array
+    assert ext_array.chunked_array == desired.chunked_array
     assert ext_array.equals(desired)
 
 
 def test___setitem___other_ext_array():
     """Tests nested_ext_array[[1,0]] = pd.Series([pd.DataFrame(...), pd.DataFrame(...), ...])"""
     struct_array = pa.StructArray.from_arrays(
         arrays=[
@@ -584,27 +584,60 @@
 def test_series_built_raises(data):
     """Test that the extension array raises an error when the data is not valid."""
     pa_array = pa.array(data)
     with pytest.raises(ValueError):
         _array = NestedExtensionArray(pa_array)
 
 
-def test_list_offsets():
-    """Test that the list offsets are correct."""
+def test_chunked_array():
+    """Test that the .chunked_array property is correct."""
+    struct_array = pa.StructArray.from_arrays(
+        arrays=[
+            pa.array([np.array([1, 2, 3]), np.array([1, 2, 1])]),
+            pa.array([-np.array([4.0, 5.0, 6.0]), -np.array([3.0, 4.0, 5.0])]),
+        ],
+        names=["a", "b"],
+    )
+    ext_array = NestedExtensionArray(struct_array)
+
+    # pyarrow returns a single bool for ==
+    assert ext_array.chunked_array == pa.chunked_array(struct_array)
+
+
+def test_list_offsets_single_chunk():
+    """Test that the .list_offset property is correct for a single chunk."""
     struct_array = pa.StructArray.from_arrays(
         arrays=[
             pa.array([np.array([1, 2, 3]), np.array([1, 2, 1])], type=pa.list_(pa.uint8())),
             pa.array([-np.array([4.0, 5.0, 6.0]), -np.array([3.0, 4.0, 5.0])]),
         ],
         names=["a", "b"],
     )
     ext_array = NestedExtensionArray(struct_array)
 
-    desired = pa.chunked_array([pa.array([0, 3, 6])])
-    assert_array_equal(ext_array.list_offsets, desired)
+    desired = pa.array([0, 3, 6], type=pa.int32())
+    # pyarrow returns a single bool for ==
+    assert ext_array.list_offsets == desired
+
+
+def test_list_offsets_multiple_chunks():
+    """Test that the .list_offset property is correct for multiple chunks."""
+    struct_array = pa.StructArray.from_arrays(
+        arrays=[
+            pa.array([np.array([1, 2, 3]), np.array([1, 2, 1])], type=pa.list_(pa.uint8())),
+            pa.array([-np.array([4.0, 5.0, 6.0]), -np.array([3.0, 4.0, 5.0])]),
+        ],
+        names=["a", "b"],
+    )
+    chunked_arrray = pa.chunked_array([struct_array, struct_array[:1], struct_array])
+    ext_array = NestedExtensionArray(chunked_arrray)
+
+    desired = chunked_arrray.combine_chunks().field("a").offsets
+    # pyarrow returns a single bool for ==
+    assert ext_array.list_offsets == desired
 
 
 def test___getitem___with_integer():
     """Test [i] is a valid DataFrame."""
     struct_array = pa.StructArray.from_arrays(
         arrays=[
             pa.array([np.array([1.0, 2.0, 3.0]), np.array([1.0, 2.0, 1.0])]),
@@ -1203,14 +1236,45 @@
         names=["a", "b"],
     )
     ext_array = NestedExtensionArray(struct_array)
 
     assert ext_array.flat_length == 7
 
 
+def test_num_chunks():
+    """Tests .num_chunks property."""
+    struct_array = pa.StructArray.from_arrays(
+        arrays=[
+            pa.array([np.array([1.0, 2.0, 3.0]), np.array([1.0, 2.0, 1.0, 2.0])]),
+            pa.array([-np.array([4.0, 5.0, 6.0]), -np.array([3.0, 4.0, 5.0, 6.0])]),
+        ],
+        names=["a", "b"],
+    )
+    chunked_array = pa.chunked_array([struct_array] * 7)
+    ext_array = NestedExtensionArray(chunked_array)
+
+    assert ext_array.num_chunks == 7
+
+
+def test_iter_field_lists():
+    """Test .iter_field_lists() yields the correct field lists"""
+    a = [[1, 2, 3], [1, 2, 3, 4]]
+    b = [np.array(["a", "b", "c"]), np.array(["x", "y", "z", "w"])]
+    struct_array = pa.StructArray.from_arrays(
+        arrays=[a, b],
+        names=["a", "b"],
+    )
+    ext_array = NestedExtensionArray(struct_array)
+
+    for actual, desired in zip(ext_array.iter_field_lists("a"), a):
+        assert_array_equal(actual, desired)
+    for actual, desired in zip(ext_array.iter_field_lists("b"), b):
+        assert_array_equal(actual, desired)
+
+
 def test_view_fields_with_single_field():
     """Tests ext_array.view("field")"""
     arrays = [
         pa.array([np.array([1.0, 2.0, 3.0]), np.array([1.0, 2.0, 1.0, 2.0])]),
         pa.array([-np.array([4.0, 5.0, 6.0]), -np.array([3.0, 4.0, 5.0, 6.0])]),
     ]
     ext_array = NestedExtensionArray(
@@ -1335,14 +1399,50 @@
         names=["a", "b"],
     )
     desired = NestedExtensionArray(desired_struct_array)
 
     assert_series_equal(pd.Series(ext_array), pd.Series(desired))
 
 
+def test_set_flat_field_keep_dtype_raises_for_wrong_dtype():
+    """Tests that set_flat_field(keep_dtype=True) raises for a wrong input dtype."""
+    struct_array = pa.StructArray.from_arrays(
+        arrays=[
+            pa.array([np.array([1.0, 2.0, 3.0]), np.array([1.0, 2.0, 3.0, 4.0])]),
+            pa.array([-np.array([4.0, 5.0, 6.0]), -np.array([3.0, 4.0, 5.0, 6.0])]),
+        ],
+        names=["a", "b"],
+    )
+    ext_array = NestedExtensionArray(struct_array)
+
+    with pytest.raises(TypeError):
+        ext_array.set_flat_field("b", ["x", "y", "z", "w", "v", "u", "t"], keep_dtype=True)
+
+    # Do not raise when keep_dtype=False
+    ext_array.set_flat_field("b", ["x", "y", "z", "w", "v", "u", "t"], keep_dtype=False)
+
+
+def test_set_flat_field_keep_dtype_raises_for_new_field():
+    """Tests that set_flat_field(keep_dtype=True) raises for a new field."""
+    struct_array = pa.StructArray.from_arrays(
+        arrays=[
+            pa.array([np.array([1.0, 2.0, 3.0]), np.array([1.0, 2.0, 3.0, 4.0])]),
+            pa.array([-np.array([4.0, 5.0, 6.0]), -np.array([3.0, 4.0, 5.0, 6.0])]),
+        ],
+        names=["a", "b"],
+    )
+    ext_array = NestedExtensionArray(struct_array)
+
+    with pytest.raises(ValueError):
+        ext_array.set_flat_field("c", [True, False, True, False, True, False, True], keep_dtype=True)
+
+    # Do not raise when keep_dtype=False
+    ext_array.set_flat_field("c", [True, False, True, False, True, False, True], keep_dtype=False)
+
+
 def test_set_list_field_new_field():
     """Tests setting a new field with a new "list" array"""
     struct_array = pa.StructArray.from_arrays(
         arrays=[
             pa.array([np.array([1.0, 2.0, 3.0]), np.array([1.0, 2.0, 1.0, 2.0])]),
             pa.array([-np.array([4.0, 5.0, 6.0]), -np.array([3.0, 4.0, 5.0, 6.0])]),
         ],
@@ -1418,75 +1518,146 @@
 
     longer_array = np.array([[1.0, 2.0, 3.0], [1.0, 2.0]], dtype=object)
 
     with pytest.raises(ValueError):
         ext_array.set_list_field("b", longer_array)
 
 
-def test_pop_field():
+def test_set_list_field_keep_dtype_raises_for_wrong_dtype():
+    """Tests that set_list_field(keep_dtype=True) raises for a wrong input dtype."""
+    struct_array = pa.StructArray.from_arrays(
+        arrays=[
+            pa.array([np.array([1.0, 2.0, 3.0]), np.array([1.0, 2.0, 3.0])]),
+            pa.array([-np.array([4.0, 5.0, 6.0]), -np.array([3.0, 4.0, 5.0])]),
+        ],
+        names=["a", "b"],
+    )
+    ext_array = NestedExtensionArray(struct_array)
+
+    with pytest.raises(TypeError):
+        ext_array.set_list_field("b", [["x", "y", "z"]] * 2, keep_dtype=True)
+
+    # Do not raise when keep_dtype=False
+    ext_array.set_list_field("b", [["x", "y", "z"]] * 2, keep_dtype=False)
+
+
+def test_set_list_field_keep_dtype_raises_for_new_field():
+    """Tests that set_list_field(keep_dtype=True) raises for a new field."""
+    struct_array = pa.StructArray.from_arrays(
+        arrays=[
+            pa.array([np.array([1.0, 2.0, 3.0])]),
+            pa.array([-np.array([4.0, 5.0, 6.0])]),
+        ],
+        names=["a", "b"],
+    )
+    ext_array = NestedExtensionArray(struct_array)
+
+    with pytest.raises(ValueError):
+        ext_array.set_list_field("c", [["x", "y", "z"]], keep_dtype=True)
+
+    # Do not raise when keep_dtype=False
+    ext_array.set_list_field("c", [["x", "y", "z"]], keep_dtype=False)
+
+
+def test_pop_fields():
     """Tests that we can pop a field from the extension array."""
     struct_array = pa.StructArray.from_arrays(
         arrays=[
             pa.array([np.array([1.0, 2.0, 3.0]), np.array([1.0, 2.0, 1.0, 2.0])]),
             pa.array([-np.array([4.0, 5.0, 6.0]), -np.array([3.0, 4.0, 5.0, 6.0])]),
             pa.array([np.array(["x", "y", "z"]), np.array(["x1", "x2", "x3", "x4"])]),
         ],
         names=["a", "b", "c"],
     )
     ext_array = NestedExtensionArray(struct_array)
 
-    ext_array.pop_field("c")
+    ext_array.pop_fields(["c"])
 
     desired_struct_array = pa.StructArray.from_arrays(
         arrays=[
             pa.array([np.array([1.0, 2.0, 3.0]), np.array([1.0, 2.0, 1.0, 2.0])]),
             pa.array([-np.array([4.0, 5.0, 6.0]), -np.array([3.0, 4.0, 5.0, 6.0])]),
         ],
         names=["a", "b"],
     )
     desired = NestedExtensionArray(desired_struct_array)
 
     assert_series_equal(pd.Series(ext_array), pd.Series(desired))
 
 
-def test_pop_field_raises_for_invalid_field():
+def test_pop_fields_multiple_fields():
+    """Tests that we can pop multiple fields from the extension array."""
+    struct_array = pa.StructArray.from_arrays(
+        arrays=[
+            pa.array([np.array([1.0, 2.0, 3.0]), np.array([1.0, 2.0, 1.0, 2.0])]),
+            pa.array([-np.array([4.0, 5.0, 6.0]), -np.array([3.0, 4.0, 5.0, 6.0])]),
+            pa.array([np.array(["x", "y", "z"]), np.array(["x1", "x2", "x3", "x4"])]),
+        ],
+        names=["a", "b", "c"],
+    )
+    ext_array = NestedExtensionArray(struct_array)
+
+    ext_array.pop_fields(["a", "c"])
+
+    desired_struct_array = pa.StructArray.from_arrays(
+        arrays=[pa.array([-np.array([4.0, 5.0, 6.0]), -np.array([3.0, 4.0, 5.0, 6.0])])],
+        names=["b"],
+    )
+    desired = NestedExtensionArray(desired_struct_array)
+
+    assert_series_equal(pd.Series(ext_array), pd.Series(desired))
+
+
+def test_pop_fields_raises_for_invalid_field():
     """Tests that we raise an error when trying to pop a field that does not exist."""
     struct_array = pa.StructArray.from_arrays(
         arrays=[
             pa.array([np.array([1.0, 2.0, 3.0])]),
             pa.array([-np.array([4.0, 5.0, 6.0])]),
         ],
         names=["a", "b"],
     )
     ext_array = NestedExtensionArray(struct_array)
 
     with pytest.raises(ValueError):
-        ext_array.pop_field("c")
+        ext_array.pop_fields(["c"])
+
+
+def test_pop_fields_raises_for_some_invalid_fields():
+    """Tests that we raise an error when trying to pop some fields that do not exist."""
+    struct_array = pa.StructArray.from_arrays(
+        arrays=[
+            pa.array([np.array([1.0, 2.0, 3.0])]),
+            pa.array([-np.array([4.0, 5.0, 6.0])]),
+        ],
+        names=["a", "b"],
+    )
+    ext_array = NestedExtensionArray(struct_array)
+
+    with pytest.raises(ValueError):
+        ext_array.pop_fields(["a", "c"])
 
 
 def test_delete_last_field_raises():
     """Tests that we raise an error when trying to delete the last field left."""
     struct_array = pa.StructArray.from_arrays(
         arrays=[
             pa.array([np.array([1.0, 2.0, 3.0]), np.array([1.0, 2.0, 1.0, 2.0])]),
             pa.array([-np.array([4.0, 5.0, 6.0]), -np.array([3.0, 4.0, 5.0, 6.0])]),
             pa.array([np.array(["x", "y", "z"]), np.array(["x1", "x2", "x3", "x4"])]),
         ],
         names=["a", "b", "c"],
     )
     ext_array = NestedExtensionArray(struct_array)
 
-    ext_array.pop_field("a")
-    assert ext_array.field_names == ["b", "c"]
-
-    ext_array.pop_field("c")
+    ext_array.pop_fields(["c", "a"])
     assert ext_array.field_names == ["b"]
 
     with pytest.raises(ValueError):
-        ext_array.pop_field("b")
+        ext_array.pop_fields(["b"])
 
 
 def test_from_arrow_ext_array():
     """Tests that we can create a NestedExtensionArray from an ArrowExtensionArray."""
     struct_array = pa.StructArray.from_arrays(
         arrays=[
             pa.array([np.array([1, 2, 3]), np.array([1, 2, 1, 2])]),
```

### Comparing `nested_pandas-0.1/tests/nested_pandas/series/test_packer.py` & `nested_pandas-0.1.1/tests/nested_pandas/series/test_packer.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,14 +4,25 @@
 import pytest
 from nested_pandas import NestedDtype
 from nested_pandas.series import packer
 from numpy.testing import assert_array_equal
 from pandas.testing import assert_frame_equal, assert_series_equal
 
 
+def offsets_reused(nested_series):
+    """Check if the offset buffers are reused for all columns of the nested series"""
+    lists_df = nested_series.nest.to_lists()
+    first_offset_buffers = None
+    for column in lists_df.columns:
+        offset_buffers = pa.array(lists_df[column]).offsets.buffers()
+        if first_offset_buffers is None:
+            first_offset_buffers = offset_buffers
+        assert offset_buffers == first_offset_buffers
+
+
 def test_pack_with_flat_df():
     """Test pack(pd.DataFrame)."""
     df = pd.DataFrame(
         data={
             "a": [1, 2, 3, 4],
             "b": [0, 1, 0, 1],
         },
@@ -24,14 +35,15 @@
             (np.array([1, 3]), np.array([0, 0])),
             (np.array([2, 4]), np.array([1, 1])),
         ],
         index=pd.MultiIndex.from_arrays(([1, 1], [1, 2])),
         dtype=NestedDtype.from_fields(dict(a=pa.int64(), b=pa.int64())),
         name="series",
     )
+    offsets_reused(series)
     assert_series_equal(series, desired)
 
 
 def test_pack_with_flat_df_and_index():
     """Test pack(pd.DataFrame)."""
     df = pd.DataFrame(
         data={
@@ -47,14 +59,15 @@
             (np.array([1, 3]), np.array([0, 0])),
             (np.array([2, 4]), np.array([1, 1])),
         ],
         index=[101, 102],
         dtype=NestedDtype.from_fields(dict(a=pa.int64(), b=pa.int64())),
         name="series",
     )
+    offsets_reused(series)
     assert_series_equal(series, desired)
 
 
 def test_pack_with_series_of_dfs():
     """Test pack(pd.Series([pd.DataFrame(), ...]))."""
     input_series = pd.Series(
         [
@@ -81,14 +94,15 @@
             (np.array([1, 2]), np.array([0, 1])),
             (np.array([3, 4]), np.array([0, 1])),
         ],
         index=[1, 2],
         name="nested",
         dtype=NestedDtype.from_fields(dict(a=pa.int64(), b=pa.int64())),
     )
+    offsets_reused(series)
     assert_series_equal(series, desired)
 
 
 def test_pack_flat():
     """Test pack_flat()."""
     df = pd.DataFrame(
         data={
@@ -105,15 +119,15 @@
             (np.array([3, 4]), np.array([0, 1])),
             (np.array([5, 6]), np.array([0, 1])),
             (np.array([7, 8, 9]), np.array([0, 1, 0])),
         ],
         index=[1, 2, 3, 4],
         dtype=NestedDtype.from_fields(dict(a=pa.int64(), b=pa.int64())),
     )
-
+    offsets_reused(actual)
     assert_series_equal(actual, desired)
 
 
 def test_pack_sorted_df_into_struct():
     """Test pack_sorted_df_into_struct()."""
     df = pd.DataFrame(
         data={
@@ -130,15 +144,15 @@
             (np.array([3, 4]), np.array([0, 1])),
             (np.array([5, 6]), np.array([0, 1])),
             (np.array([7, 8, 9]), np.array([0, 1, 0])),
         ],
         index=[1, 2, 3, 4],
         dtype=NestedDtype.from_fields(dict(a=pa.int64(), b=pa.int64())),
     )
-
+    offsets_reused(actual)
     assert_series_equal(actual, desired)
 
 
 def test_pack_sorted_df_into_struct_raises_when_not_sorted():
     """Test pack_sorted_df_into_struct() raises when not sorted."""
     df = pd.DataFrame(
         data={
@@ -168,14 +182,15 @@
                 np.array([0, 1, 0]),
             ],
         },
         index=[1, 2, 3, 4],
         dtype=pd.ArrowDtype(pa.list_(pa.int64())),
     )
     series = packer.pack_lists(packed_df)
+    offsets_reused(series)
 
     for field_name in packed_df.columns:
         assert_series_equal(series.nest.get_list_series(field_name), packed_df[field_name])
 
 
 def test_pack_seq_with_dfs_and_index():
     """Test pack_seq()."""
@@ -217,14 +232,15 @@
             (np.array([3, 4]), np.array([0, 1])),
             (np.array([5, 6]), np.array([0, 1])),
             (np.array([7, 8, 9]), np.array([0, 1, 0])),
         ],
         index=[100, 101, 102, 103],
         dtype=NestedDtype.from_fields(dict(a=pa.int64(), b=pa.int64())),
     )
+    offsets_reused(series)
     assert_series_equal(series, desired)
 
 
 def test_pack_seq_with_different_elements_and_index():
     """Test pack_seq() with different elements and index"""
     seq = [
         pd.DataFrame(
@@ -245,14 +261,15 @@
             None,
             (np.array([3, 4]), np.array([-1, 0])),
             pd.NA,
         ],
         index=[100, 101, 102, 103],
         dtype=NestedDtype.from_fields(dict(a=pa.int64(), b=pa.int64())),
     )
+    offsets_reused(series)
     assert_series_equal(series, desired)
 
 
 def test_pack_seq_with_series_of_dfs():
     """Test pack_seq(pd.Series([pd.DataFrame(), ...]))."""
     input_series = pd.Series(
         [
@@ -286,14 +303,15 @@
             (np.array([3, 4]), np.array([0, 1])),
             (np.array([5, 6]), np.array([0, 1])),
         ],
         index=[100, 101, 102],
         dtype=NestedDtype.from_fields(dict(a=pa.int64(), b=pa.int64())),
         name="series",
     )
+    offsets_reused(series)
     assert_series_equal(series, desired)
 
 
 def test_view_sorted_df_as_list_arrays():
     """Test view_sorted_df_as_list_arrays()."""
     flat_df = pd.DataFrame(
         data={
@@ -398,15 +416,17 @@
             ),
             np.array([0, 1, 4, 6, 8]),
         ),
     ],
 )
 def test_calculate_sorted_index_offsets(index, offsets):
     """Test calculate_sorted_index_offsets()."""
-    assert_array_equal(packer.calculate_sorted_index_offsets(index), offsets)
+    actual = packer.calculate_sorted_index_offsets(index)
+    assert actual.dtype == np.int32
+    assert_array_equal(actual, offsets)
 
 
 def test_calculate_sorted_index_offsets_raises_when_not_sorted():
     """Test calculate_sorted_index_offsets() raises when not sorted."""
     index = pd.Index([1, 2, 1, 2, 3, 3, 4, 4, 4])
     with pytest.raises(ValueError):
         packer.calculate_sorted_index_offsets(index)
```

### Comparing `nested_pandas-0.1/tests/nested_pandas/utils/test_utils.py` & `nested_pandas-0.1.1/tests/nested_pandas/utils/test_utils.py`

 * *Files identical despite different names*

