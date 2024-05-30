# Comparing `tmp/declinate-0.0.2.tar.gz` & `tmp/declinate-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "declinate-0.0.2.tar", last modified: Mon Mar  4 15:07:07 2024, max compression
+gzip compressed data, was "declinate-0.0.3.tar", last modified: Thu May 30 13:21:01 2024, max compression
```

## Comparing `declinate-0.0.2.tar` & `declinate-0.0.3.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 15:07:07.084791 declinate-0.0.2/
--rw-rw-rw-   0 root         (0) root         (0)      105 2024-03-04 15:06:59.000000 declinate-0.0.2/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 15:07:07.069791 declinate-0.0.2/.gitlab/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 15:07:07.074791 declinate-0.0.2/.gitlab/issue_templates/
--rw-rw-rw-   0 root         (0) root         (0)      649 2024-03-04 15:06:59.000000 declinate-0.0.2/.gitlab/issue_templates/bug.md
--rw-rw-rw-   0 root         (0) root         (0)     1084 2024-03-04 15:06:59.000000 declinate-0.0.2/.gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 15:07:07.074791 declinate-0.0.2/.reuse/
--rw-rw-rw-   0 root         (0) root         (0)      462 2024-03-04 15:06:59.000000 declinate-0.0.2/.reuse/dep5
--rw-rw-rw-   0 root         (0) root         (0)      229 2024-03-04 15:06:59.000000 declinate-0.0.2/CHANGES.rst
--rw-rw-rw-   0 root         (0) root         (0)     3372 2024-03-04 15:06:59.000000 declinate-0.0.2/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)    10280 2024-03-04 15:06:59.000000 declinate-0.0.2/LICENSE.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 15:07:07.075791 declinate-0.0.2/LICENSES/
--rw-rw-rw-   0 root         (0) root         (0)    10280 2024-03-04 15:06:59.000000 declinate-0.0.2/LICENSES/Apache-2.0.txt
--rw-rw-rw-   0 root         (0) root         (0)    18375 2024-03-04 15:06:59.000000 declinate-0.0.2/LICENSES/CC-BY-SA-4.0.txt
--rw-rw-rw-   0 root         (0) root         (0)     7048 2024-03-04 15:06:59.000000 declinate-0.0.2/LICENSES/CC0-1.0.txt
--rw-r--r--   0 root         (0) root         (0)     4743 2024-03-04 15:07:07.084791 declinate-0.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3333 2024-03-04 15:06:59.000000 declinate-0.0.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 15:07:07.075791 declinate-0.0.2/docs/
--rw-rw-rw-   0 root         (0) root         (0)       28 2024-03-04 15:06:59.000000 declinate-0.0.2/docs/changes.rst
--rw-rw-rw-   0 root         (0) root         (0)      431 2024-03-04 15:06:59.000000 declinate-0.0.2/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      412 2024-03-04 15:06:59.000000 declinate-0.0.2/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     2567 2024-03-04 15:06:59.000000 declinate-0.0.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)    29211 2024-03-04 15:06:59.000000 declinate-0.0.2/requirements-dev.txt
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-03-04 15:06:59.000000 declinate-0.0.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-04 15:07:07.084791 declinate-0.0.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 15:07:07.070791 declinate-0.0.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 15:07:07.077791 declinate-0.0.2/src/declinate/
--rw-rw-rw-   0 root         (0) root         (0)      110 2024-03-04 15:06:59.000000 declinate-0.0.2/src/declinate/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      771 2024-03-04 15:06:59.000000 declinate-0.0.2/src/declinate/check.py
--rw-rw-rw-   0 root         (0) root         (0)    11191 2024-03-04 15:06:59.000000 declinate-0.0.2/src/declinate/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2059 2024-03-04 15:06:59.000000 declinate-0.0.2/src/declinate/declinate.py
--rw-rw-rw-   0 root         (0) root         (0)    30773 2024-03-04 15:06:59.000000 declinate-0.0.2/src/declinate/gen.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-04 15:06:59.000000 declinate-0.0.2/src/declinate/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 15:07:07.083791 declinate-0.0.2/src/declinate.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4743 2024-03-04 15:07:07.000000 declinate-0.0.2/src/declinate.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1530 2024-03-04 15:07:07.000000 declinate-0.0.2/src/declinate.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-04 15:07:07.000000 declinate-0.0.2/src/declinate.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2024-03-04 15:07:07.000000 declinate-0.0.2/src/declinate.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       90 2024-03-04 15:07:07.000000 declinate-0.0.2/src/declinate.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-03-04 15:07:07.000000 declinate-0.0.2/src/declinate.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 15:07:07.078791 declinate-0.0.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)       91 2024-03-04 15:06:59.000000 declinate-0.0.2/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 15:07:07.079791 declinate-0.0.2/tests/declinate/
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-03-04 15:06:59.000000 declinate-0.0.2/tests/declinate/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 15:07:07.079791 declinate-0.0.2/tests/declinate/cli0_minimal/
--rw-rw-rw-   0 root         (0) root         (0)       87 2024-03-04 15:06:59.000000 declinate-0.0.2/tests/declinate/cli0_minimal/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9441 2024-03-04 15:06:59.000000 declinate-0.0.2/tests/declinate/cli0_minimal/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      175 2024-03-04 15:06:59.000000 declinate-0.0.2/tests/declinate/cli0_minimal/declinate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 15:07:07.080791 declinate-0.0.2/tests/declinate/cli1_arguments/
--rw-rw-rw-   0 root         (0) root         (0)       87 2024-03-04 15:06:59.000000 declinate-0.0.2/tests/declinate/cli1_arguments/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10763 2024-03-04 15:06:59.000000 declinate-0.0.2/tests/declinate/cli1_arguments/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1954 2024-03-04 15:06:59.000000 declinate-0.0.2/tests/declinate/cli1_arguments/declinate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 15:07:07.081791 declinate-0.0.2/tests/declinate/cli2_groups/
--rw-rw-rw-   0 root         (0) root         (0)       87 2024-03-04 15:06:59.000000 declinate-0.0.2/tests/declinate/cli2_groups/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11062 2024-03-04 15:06:59.000000 declinate-0.0.2/tests/declinate/cli2_groups/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2388 2024-03-04 15:06:59.000000 declinate-0.0.2/tests/declinate/cli2_groups/declinate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 15:07:07.081791 declinate-0.0.2/tests/declinate/cli3_withsubcommands/
--rw-rw-rw-   0 root         (0) root         (0)       87 2024-03-04 15:06:59.000000 declinate-0.0.2/tests/declinate/cli3_withsubcommands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10207 2024-03-04 15:06:59.000000 declinate-0.0.2/tests/declinate/cli3_withsubcommands/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      542 2024-03-04 15:06:59.000000 declinate-0.0.2/tests/declinate/cli3_withsubcommands/declinate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 15:07:07.082791 declinate-0.0.2/tests/declinate/cli4_justsubcommands/
--rw-rw-rw-   0 root         (0) root         (0)       87 2024-03-04 15:06:59.000000 declinate-0.0.2/tests/declinate/cli4_justsubcommands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10129 2024-03-04 15:06:59.000000 declinate-0.0.2/tests/declinate/cli4_justsubcommands/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      615 2024-03-04 15:06:59.000000 declinate-0.0.2/tests/declinate/cli4_justsubcommands/declinate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 15:07:07.083791 declinate-0.0.2/tests/declinate/cli5_addargfn/
--rw-rw-rw-   0 root         (0) root         (0)       87 2024-03-04 15:06:59.000000 declinate-0.0.2/tests/declinate/cli5_addargfn/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10385 2024-03-04 15:06:59.000000 declinate-0.0.2/tests/declinate/cli5_addargfn/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      898 2024-03-04 15:06:59.000000 declinate-0.0.2/tests/declinate/cli5_addargfn/declinate.py
--rw-rw-rw-   0 root         (0) root         (0)      456 2024-03-04 15:06:59.000000 declinate-0.0.2/tests/declinate/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)      507 2024-03-04 15:06:59.000000 declinate-0.0.2/tests/declinate/test_consumers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 13:21:01.465451 declinate-0.0.3/
+-rw-rw-rw-   0 root         (0) root         (0)      105 2024-05-30 13:20:52.000000 declinate-0.0.3/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 13:21:01.450451 declinate-0.0.3/.gitlab/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 13:21:01.454451 declinate-0.0.3/.gitlab/issue_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      649 2024-05-30 13:20:52.000000 declinate-0.0.3/.gitlab/issue_templates/bug.md
+-rw-rw-rw-   0 root         (0) root         (0)     1184 2024-05-30 13:20:52.000000 declinate-0.0.3/.gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 13:21:01.455451 declinate-0.0.3/.reuse/
+-rw-rw-rw-   0 root         (0) root         (0)      462 2024-05-30 13:20:52.000000 declinate-0.0.3/.reuse/dep5
+-rw-rw-rw-   0 root         (0) root         (0)      291 2024-05-30 13:20:52.000000 declinate-0.0.3/CHANGES.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3372 2024-05-30 13:20:52.000000 declinate-0.0.3/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)    10280 2024-05-30 13:20:52.000000 declinate-0.0.3/LICENSE.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 13:21:01.455451 declinate-0.0.3/LICENSES/
+-rw-rw-rw-   0 root         (0) root         (0)    10280 2024-05-30 13:20:52.000000 declinate-0.0.3/LICENSES/Apache-2.0.txt
+-rw-rw-rw-   0 root         (0) root         (0)    18375 2024-05-30 13:20:52.000000 declinate-0.0.3/LICENSES/CC-BY-SA-4.0.txt
+-rw-rw-rw-   0 root         (0) root         (0)     7048 2024-05-30 13:20:52.000000 declinate-0.0.3/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 root         (0) root         (0)     4776 2024-05-30 13:21:01.465451 declinate-0.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3333 2024-05-30 13:20:52.000000 declinate-0.0.3/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 13:21:01.456452 declinate-0.0.3/docs/
+-rw-rw-rw-   0 root         (0) root         (0)       28 2024-05-30 13:20:52.000000 declinate-0.0.3/docs/changes.rst
+-rw-rw-rw-   0 root         (0) root         (0)      431 2024-05-30 13:20:52.000000 declinate-0.0.3/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      412 2024-05-30 13:20:52.000000 declinate-0.0.3/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2591 2024-05-30 13:20:52.000000 declinate-0.0.3/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)    29270 2024-05-30 13:20:52.000000 declinate-0.0.3/requirements-dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)      363 2024-05-30 13:20:52.000000 declinate-0.0.3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 13:21:01.465451 declinate-0.0.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 13:21:01.451451 declinate-0.0.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 13:21:01.458451 declinate-0.0.3/src/declinate/
+-rw-rw-rw-   0 root         (0) root         (0)      110 2024-05-30 13:20:52.000000 declinate-0.0.3/src/declinate/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      771 2024-05-30 13:20:52.000000 declinate-0.0.3/src/declinate/check.py
+-rw-rw-rw-   0 root         (0) root         (0)    11230 2024-05-30 13:20:52.000000 declinate-0.0.3/src/declinate/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2059 2024-05-30 13:20:52.000000 declinate-0.0.3/src/declinate/declinate.py
+-rw-rw-rw-   0 root         (0) root         (0)    31637 2024-05-30 13:20:52.000000 declinate-0.0.3/src/declinate/gen.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-30 13:20:52.000000 declinate-0.0.3/src/declinate/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 13:21:01.464451 declinate-0.0.3/src/declinate.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4776 2024-05-30 13:21:01.000000 declinate-0.0.3/src/declinate.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1530 2024-05-30 13:21:01.000000 declinate-0.0.3/src/declinate.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 13:21:01.000000 declinate-0.0.3/src/declinate.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2024-05-30 13:21:01.000000 declinate-0.0.3/src/declinate.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2024-05-30 13:21:01.000000 declinate-0.0.3/src/declinate.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-30 13:21:01.000000 declinate-0.0.3/src/declinate.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 13:21:01.459452 declinate-0.0.3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       91 2024-05-30 13:20:52.000000 declinate-0.0.3/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 13:21:01.460451 declinate-0.0.3/tests/declinate/
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-30 13:20:52.000000 declinate-0.0.3/tests/declinate/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 13:21:01.460451 declinate-0.0.3/tests/declinate/cli0_minimal/
+-rw-rw-rw-   0 root         (0) root         (0)       87 2024-05-30 13:20:52.000000 declinate-0.0.3/tests/declinate/cli0_minimal/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9484 2024-05-30 13:20:52.000000 declinate-0.0.3/tests/declinate/cli0_minimal/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      175 2024-05-30 13:20:52.000000 declinate-0.0.3/tests/declinate/cli0_minimal/declinate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 13:21:01.461451 declinate-0.0.3/tests/declinate/cli1_arguments/
+-rw-rw-rw-   0 root         (0) root         (0)       87 2024-05-30 13:20:52.000000 declinate-0.0.3/tests/declinate/cli1_arguments/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10806 2024-05-30 13:20:52.000000 declinate-0.0.3/tests/declinate/cli1_arguments/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1954 2024-05-30 13:20:52.000000 declinate-0.0.3/tests/declinate/cli1_arguments/declinate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 13:21:01.462452 declinate-0.0.3/tests/declinate/cli2_groups/
+-rw-rw-rw-   0 root         (0) root         (0)       87 2024-05-30 13:20:52.000000 declinate-0.0.3/tests/declinate/cli2_groups/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11097 2024-05-30 13:20:52.000000 declinate-0.0.3/tests/declinate/cli2_groups/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2388 2024-05-30 13:20:52.000000 declinate-0.0.3/tests/declinate/cli2_groups/declinate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 13:21:01.462452 declinate-0.0.3/tests/declinate/cli3_withsubcommands/
+-rw-rw-rw-   0 root         (0) root         (0)       87 2024-05-30 13:20:52.000000 declinate-0.0.3/tests/declinate/cli3_withsubcommands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10250 2024-05-30 13:20:52.000000 declinate-0.0.3/tests/declinate/cli3_withsubcommands/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      542 2024-05-30 13:20:52.000000 declinate-0.0.3/tests/declinate/cli3_withsubcommands/declinate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 13:21:01.463451 declinate-0.0.3/tests/declinate/cli4_justsubcommands/
+-rw-rw-rw-   0 root         (0) root         (0)       87 2024-05-30 13:20:52.000000 declinate-0.0.3/tests/declinate/cli4_justsubcommands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10172 2024-05-30 13:20:52.000000 declinate-0.0.3/tests/declinate/cli4_justsubcommands/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      615 2024-05-30 13:20:52.000000 declinate-0.0.3/tests/declinate/cli4_justsubcommands/declinate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 13:21:01.463451 declinate-0.0.3/tests/declinate/cli5_addargfn/
+-rw-rw-rw-   0 root         (0) root         (0)       87 2024-05-30 13:20:52.000000 declinate-0.0.3/tests/declinate/cli5_addargfn/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10424 2024-05-30 13:20:52.000000 declinate-0.0.3/tests/declinate/cli5_addargfn/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      898 2024-05-30 13:20:52.000000 declinate-0.0.3/tests/declinate/cli5_addargfn/declinate.py
+-rw-rw-rw-   0 root         (0) root         (0)      456 2024-05-30 13:20:52.000000 declinate-0.0.3/tests/declinate/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      507 2024-05-30 13:20:52.000000 declinate-0.0.3/tests/declinate/test_consumers.py
```

### Comparing `declinate-0.0.2/.gitlab/issue_templates/bug.md` & `declinate-0.0.3/.gitlab/issue_templates/bug.md`

 * *Files identical despite different names*

### Comparing `declinate-0.0.2/.gitlab-ci.yml` & `declinate-0.0.3/.gitlab-ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 stages:
   - test
   - build
 
 
 test:
   stage: test
-  image: python:3.10
+  image: python:$VERSION
   script:
-    - python3.10 -m venv venv
+    - python$VERSION -m venv venv
     - venv/bin/python -m pip install -r requirements-dev.txt
     - venv/bin/python -m pip install -e .[dev]
     - venv/bin/python -m pytest --cov=src --cov-report=term --cov-report=xml --junit-xml=report.xml
     - venv/bin/python -m mypy --no-error-summary docs src tests
     - venv/bin/python -m reuse lint
     - venv/bin/python -m ruff check docs src tests
     - venv/bin/python -m ruff format --diff docs src tests
@@ -21,14 +21,20 @@
     paths:
       - public
     reports:
       coverage_report:
         coverage_format: cobertura
         path: coverage.xml
       junit: report.xml
+  parallel:
+    matrix:
+      - VERSION:
+        - "3.10"
+        - "3.11"
+        - "3.12"
 
 
 build:
   stage: build
   image: python:3.10
   script:
     - python3.10 -m venv venv
```

### Comparing `declinate-0.0.2/CONTRIBUTING.rst` & `declinate-0.0.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `declinate-0.0.2/LICENSE.txt` & `declinate-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `declinate-0.0.2/LICENSES/Apache-2.0.txt` & `declinate-0.0.3/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `declinate-0.0.2/LICENSES/CC-BY-SA-4.0.txt` & `declinate-0.0.3/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `declinate-0.0.2/LICENSES/CC0-1.0.txt` & `declinate-0.0.3/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `declinate-0.0.2/PKG-INFO` & `declinate-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: declinate
-Version: 0.0.2
+Version: 0.0.3
 Summary: CLI generator.
 Author-email: Ternaris <team@ternaris.com>
 License: Apache-2.0
 Project-URL: Homepage, https://gitlab.com/ternaris/declinate
 Project-URL: Documentation, https://ternaris.gitlab.io/declinate
 Project-URL: Source, https://gitlab.com/ternaris/declinate
 Project-URL: Issues, https://gitlab.com/ternaris/declinate/issues
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
+Requires-Dist: typing_extensions
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: reuse; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
```

### Comparing `declinate-0.0.2/README.rst` & `declinate-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `declinate-0.0.2/pyproject.toml` & `declinate-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,17 @@
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Typing :: Typed",
 ]
 description = "CLI generator."
-dependencies = []
+dependencies = [
+  "typing_extensions",
+]
 dynamic = ["version"]
 keywords = [
   "cli",
 ]
 license = { text = "Apache-2.0" }
 readme = "README.rst"
 requires-python = ">=3.10"
```

### Comparing `declinate-0.0.2/requirements-dev.txt` & `declinate-0.0.3/requirements-dev.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 #
 #    pip-compile --extra=dev --generate-hashes --output-file=requirements-dev.txt
 #
 alabaster==0.7.16 \
     --hash=sha256:75a8b99c28a5dad50dd7f8ccdd447a121ddb3892da9e53d1ca5cca3106d58d65 \
     --hash=sha256:b46733c07dce03ae4e150330b975c75737fa60f0a7c591b6c8bf4928a28e2c92
     # via sphinx
-babel==2.14.0 \
-    --hash=sha256:6919867db036398ba21eb5c7a0f6b28ab8cbc3ae7a73a44ebe34ae74a4e7d363 \
-    --hash=sha256:efb1a25b7118e67ce3a259bed20545c29cb68be8ad2c784c83689981b7a57287
+babel==2.15.0 \
+    --hash=sha256:08706bdad8d0a3413266ab61bd6c34d0c28d6e1e7badf40a2cebe67644e2e1fb \
+    --hash=sha256:8daf0e265d05768bc6c7a314cf1321e9a123afc328cc635c18622a2f30a04413
     # via sphinx
 binaryornot==0.4.4 \
     --hash=sha256:359501dfc9d40632edc9fac890e19542db1a287bbcfa58175b66658392018061 \
     --hash=sha256:b8b71173c917bddcd2c16070412e369c3ed7f0528926f70cac18a6c97fd563e4
     # via reuse
 boolean-py==4.0 \
     --hash=sha256:17b9a181630e43dde1851d42bef546d616d5d9b4480357514597e78b203d06e4 \
@@ -120,99 +120,99 @@
     --hash=sha256:efcb3f6676480691518c177e3b465bcddf57cea040302f9f4e6e191af91174d4 \
     --hash=sha256:f27273b60488abe721a075bcca6d7f3964f9f6f067c8c4c605743023d7d3944f \
     --hash=sha256:f30c3cb33b24454a82faecaf01b19c18562b1e89558fb6c56de4d9118a032fd5 \
     --hash=sha256:fb69256e180cb6c8a894fee62b3afebae785babc1ee98b81cdf68bbca1987f33 \
     --hash=sha256:fd1abc0d89e30cc4e02e4064dc67fcc51bd941eb395c502aac3ec19fab46b519 \
     --hash=sha256:ff8fa367d09b717b2a17a052544193ad76cd49979c805768879cb63d9ca50561
     # via requests
-coverage[toml]==7.4.3 \
-    --hash=sha256:0209a6369ccce576b43bb227dc8322d8ef9e323d089c6f3f26a597b09cb4d2aa \
-    --hash=sha256:062b0a75d9261e2f9c6d071753f7eef0fc9caf3a2c82d36d76667ba7b6470003 \
-    --hash=sha256:0842571634f39016a6c03e9d4aba502be652a6e4455fadb73cd3a3a49173e38f \
-    --hash=sha256:16bae383a9cc5abab9bb05c10a3e5a52e0a788325dc9ba8499e821885928968c \
-    --hash=sha256:18c7320695c949de11a351742ee001849912fd57e62a706d83dfc1581897fa2e \
-    --hash=sha256:18d90523ce7553dd0b7e23cbb28865db23cddfd683a38fb224115f7826de78d0 \
-    --hash=sha256:1bf25fbca0c8d121a3e92a2a0555c7e5bc981aee5c3fdaf4bb7809f410f696b9 \
-    --hash=sha256:276f6077a5c61447a48d133ed13e759c09e62aff0dc84274a68dc18660104d52 \
-    --hash=sha256:280459f0a03cecbe8800786cdc23067a8fc64c0bd51dc614008d9c36e1659d7e \
-    --hash=sha256:28ca2098939eabab044ad68850aac8f8db6bf0b29bc7f2887d05889b17346454 \
-    --hash=sha256:2c854ce44e1ee31bda4e318af1dbcfc929026d12c5ed030095ad98197eeeaed0 \
-    --hash=sha256:35eb581efdacf7b7422af677b92170da4ef34500467381e805944a3201df2079 \
-    --hash=sha256:37389611ba54fd6d278fde86eb2c013c8e50232e38f5c68235d09d0a3f8aa352 \
-    --hash=sha256:3b253094dbe1b431d3a4ac2f053b6d7ede2664ac559705a704f621742e034f1f \
-    --hash=sha256:3b2eccb883368f9e972e216c7b4c7c06cabda925b5f06dde0650281cb7666a30 \
-    --hash=sha256:451f433ad901b3bb00184d83fd83d135fb682d780b38af7944c9faeecb1e0bfe \
-    --hash=sha256:489763b2d037b164846ebac0cbd368b8a4ca56385c4090807ff9fad817de4113 \
-    --hash=sha256:4af154d617c875b52651dd8dd17a31270c495082f3d55f6128e7629658d63765 \
-    --hash=sha256:506edb1dd49e13a2d4cac6a5173317b82a23c9d6e8df63efb4f0380de0fbccbc \
-    --hash=sha256:6679060424faa9c11808598504c3ab472de4531c571ab2befa32f4971835788e \
-    --hash=sha256:69b9f6f66c0af29642e73a520b6fed25ff9fd69a25975ebe6acb297234eda501 \
-    --hash=sha256:6c00cdc8fa4e50e1cc1f941a7f2e3e0f26cb2a1233c9696f26963ff58445bac7 \
-    --hash=sha256:6c0cdedd3500e0511eac1517bf560149764b7d8e65cb800d8bf1c63ebf39edd2 \
-    --hash=sha256:708a3369dcf055c00ddeeaa2b20f0dd1ce664eeabde6623e516c5228b753654f \
-    --hash=sha256:718187eeb9849fc6cc23e0d9b092bc2348821c5e1a901c9f8975df0bc785bfd4 \
-    --hash=sha256:767b35c3a246bcb55b8044fd3a43b8cd553dd1f9f2c1eeb87a302b1f8daa0524 \
-    --hash=sha256:77fbfc5720cceac9c200054b9fab50cb2a7d79660609200ab83f5db96162d20c \
-    --hash=sha256:7cbde573904625509a3f37b6fecea974e363460b556a627c60dc2f47e2fffa51 \
-    --hash=sha256:8249b1c7334be8f8c3abcaaa996e1e4927b0e5a23b65f5bf6cfe3180d8ca7840 \
-    --hash=sha256:8580b827d4746d47294c0e0b92854c85a92c2227927433998f0d3320ae8a71b6 \
-    --hash=sha256:8640f1fde5e1b8e3439fe482cdc2b0bb6c329f4bb161927c28d2e8879c6029ee \
-    --hash=sha256:9a9babb9466fe1da12417a4aed923e90124a534736de6201794a3aea9d98484e \
-    --hash=sha256:a78ed23b08e8ab524551f52953a8a05d61c3a760781762aac49f8de6eede8c45 \
-    --hash=sha256:abbbd8093c5229c72d4c2926afaee0e6e3140de69d5dcd918b2921f2f0c8baba \
-    --hash=sha256:ae7f19afe0cce50039e2c782bff379c7e347cba335429678450b8fe81c4ef96d \
-    --hash=sha256:b3ec74cfef2d985e145baae90d9b1b32f85e1741b04cd967aaf9cfa84c1334f3 \
-    --hash=sha256:b51bfc348925e92a9bd9b2e48dad13431b57011fd1038f08316e6bf1df107d10 \
-    --hash=sha256:b9a4a8dd3dcf4cbd3165737358e4d7dfbd9d59902ad11e3b15eebb6393b0446e \
-    --hash=sha256:ba3a8aaed13770e970b3df46980cb068d1c24af1a1968b7818b69af8c4347efb \
-    --hash=sha256:c0524de3ff096e15fcbfe8f056fdb4ea0bf497d584454f344d59fce069d3e6e9 \
-    --hash=sha256:c0a120238dd71c68484f02562f6d446d736adcc6ca0993712289b102705a9a3a \
-    --hash=sha256:cbbe5e739d45a52f3200a771c6d2c7acf89eb2524890a4a3aa1a7fa0695d2a47 \
-    --hash=sha256:ce8c50520f57ec57aa21a63ea4f325c7b657386b3f02ccaedeccf9ebe27686e1 \
-    --hash=sha256:cf30900aa1ba595312ae41978b95e256e419d8a823af79ce670835409fc02ad3 \
-    --hash=sha256:d25b937a5d9ffa857d41be042b4238dd61db888533b53bc76dc082cb5a15e914 \
-    --hash=sha256:d6cdecaedea1ea9e033d8adf6a0ab11107b49571bbb9737175444cea6eb72328 \
-    --hash=sha256:dec9de46a33cf2dd87a5254af095a409ea3bf952d85ad339751e7de6d962cde6 \
-    --hash=sha256:ebe7c9e67a2d15fa97b77ea6571ce5e1e1f6b0db71d1d5e96f8d2bf134303c1d \
-    --hash=sha256:ee866acc0861caebb4f2ab79f0b94dbfbdbfadc19f82e6e9c93930f74e11d7a0 \
-    --hash=sha256:f6a09b360d67e589236a44f0c39218a8efba2593b6abdccc300a8862cffc2f94 \
-    --hash=sha256:fcc66e222cf4c719fe7722a403888b1f5e1682d1679bd780e2b26c18bb648cdc \
-    --hash=sha256:fd6545d97c98a192c5ac995d21c894b581f1fd14cf389be90724d21808b657e2
+coverage[toml]==7.5.3 \
+    --hash=sha256:015eddc5ccd5364dcb902eaecf9515636806fa1e0d5bef5769d06d0f31b54523 \
+    --hash=sha256:04aefca5190d1dc7a53a4c1a5a7f8568811306d7a8ee231c42fb69215571944f \
+    --hash=sha256:05ac5f60faa0c704c0f7e6a5cbfd6f02101ed05e0aee4d2822637a9e672c998d \
+    --hash=sha256:0bbddc54bbacfc09b3edaec644d4ac90c08ee8ed4844b0f86227dcda2d428fcb \
+    --hash=sha256:1d2a830ade66d3563bb61d1e3c77c8def97b30ed91e166c67d0632c018f380f0 \
+    --hash=sha256:239a4e75e09c2b12ea478d28815acf83334d32e722e7433471fbf641c606344c \
+    --hash=sha256:244f509f126dc71369393ce5fea17c0592c40ee44e607b6d855e9c4ac57aac98 \
+    --hash=sha256:25a5caf742c6195e08002d3b6c2dd6947e50efc5fc2c2205f61ecb47592d2d83 \
+    --hash=sha256:296a7d9bbc598e8744c00f7a6cecf1da9b30ae9ad51c566291ff1314e6cbbed8 \
+    --hash=sha256:2e079c9ec772fedbade9d7ebc36202a1d9ef7291bc9b3a024ca395c4d52853d7 \
+    --hash=sha256:33ca90a0eb29225f195e30684ba4a6db05dbef03c2ccd50b9077714c48153cac \
+    --hash=sha256:33fc65740267222fc02975c061eb7167185fef4cc8f2770267ee8bf7d6a42f84 \
+    --hash=sha256:341dd8f61c26337c37988345ca5c8ccabeff33093a26953a1ac72e7d0103c4fb \
+    --hash=sha256:34d6d21d8795a97b14d503dcaf74226ae51eb1f2bd41015d3ef332a24d0a17b3 \
+    --hash=sha256:3538d8fb1ee9bdd2e2692b3b18c22bb1c19ffbefd06880f5ac496e42d7bb3884 \
+    --hash=sha256:38a3b98dae8a7c9057bd91fbf3415c05e700a5114c5f1b5b0ea5f8f429ba6614 \
+    --hash=sha256:3d5a67f0da401e105753d474369ab034c7bae51a4c31c77d94030d59e41df5bd \
+    --hash=sha256:50084d3516aa263791198913a17354bd1dc627d3c1639209640b9cac3fef5807 \
+    --hash=sha256:55f689f846661e3f26efa535071775d0483388a1ccfab899df72924805e9e7cd \
+    --hash=sha256:5bc5a8c87714b0c67cfeb4c7caa82b2d71e8864d1a46aa990b5588fa953673b8 \
+    --hash=sha256:62bda40da1e68898186f274f832ef3e759ce929da9a9fd9fcf265956de269dbc \
+    --hash=sha256:705f3d7c2b098c40f5b81790a5fedb274113373d4d1a69e65f8b68b0cc26f6db \
+    --hash=sha256:75e3f4e86804023e991096b29e147e635f5e2568f77883a1e6eed74512659ab0 \
+    --hash=sha256:7b2a19e13dfb5c8e145c7a6ea959485ee8e2204699903c88c7d25283584bfc08 \
+    --hash=sha256:7cec2af81f9e7569280822be68bd57e51b86d42e59ea30d10ebdbb22d2cb7232 \
+    --hash=sha256:8383a6c8cefba1b7cecc0149415046b6fc38836295bc4c84e820872eb5478b3d \
+    --hash=sha256:8c836309931839cca658a78a888dab9676b5c988d0dd34ca247f5f3e679f4e7a \
+    --hash=sha256:8e317953bb4c074c06c798a11dbdd2cf9979dbcaa8ccc0fa4701d80042d4ebf1 \
+    --hash=sha256:923b7b1c717bd0f0f92d862d1ff51d9b2b55dbbd133e05680204465f454bb286 \
+    --hash=sha256:990fb20b32990b2ce2c5f974c3e738c9358b2735bc05075d50a6f36721b8f303 \
+    --hash=sha256:9aad68c3f2566dfae84bf46295a79e79d904e1c21ccfc66de88cd446f8686341 \
+    --hash=sha256:a5812840d1d00eafae6585aba38021f90a705a25b8216ec7f66aebe5b619fb84 \
+    --hash=sha256:a6519d917abb15e12380406d721e37613e2a67d166f9fb7e5a8ce0375744cd45 \
+    --hash=sha256:ab0b028165eea880af12f66086694768f2c3139b2c31ad5e032c8edbafca6ffc \
+    --hash=sha256:aea7da970f1feccf48be7335f8b2ca64baf9b589d79e05b9397a06696ce1a1ec \
+    --hash=sha256:b1196e13c45e327d6cd0b6e471530a1882f1017eb83c6229fc613cd1a11b53cd \
+    --hash=sha256:b368e1aee1b9b75757942d44d7598dcd22a9dbb126affcbba82d15917f0cc155 \
+    --hash=sha256:bde997cac85fcac227b27d4fb2c7608a2c5f6558469b0eb704c5726ae49e1c52 \
+    --hash=sha256:c4c2872b3c91f9baa836147ca33650dc5c172e9273c808c3c3199c75490e709d \
+    --hash=sha256:c59d2ad092dc0551d9f79d9d44d005c945ba95832a6798f98f9216ede3d5f485 \
+    --hash=sha256:d1da0a2e3b37b745a2b2a678a4c796462cf753aebf94edcc87dcc6b8641eae31 \
+    --hash=sha256:d8b7339180d00de83e930358223c617cc343dd08e1aa5ec7b06c3a121aec4e1d \
+    --hash=sha256:dd4b3355b01273a56b20c219e74e7549e14370b31a4ffe42706a8cda91f19f6d \
+    --hash=sha256:e08c470c2eb01977d221fd87495b44867a56d4d594f43739a8028f8646a51e0d \
+    --hash=sha256:f5102a92855d518b0996eb197772f5ac2a527c0ec617124ad5242a3af5e25f85 \
+    --hash=sha256:f542287b1489c7a860d43a7d8883e27ca62ab84ca53c965d11dac1d3a1fab7ce \
+    --hash=sha256:f78300789a708ac1f17e134593f577407d52d0417305435b134805c4fb135adb \
+    --hash=sha256:f81bc26d609bf0fbc622c7122ba6307993c83c795d2d6f6f6fd8c000a770d974 \
+    --hash=sha256:f836c174c3a7f639bded48ec913f348c4761cbf49de4a20a956d3431a7c9cb24 \
+    --hash=sha256:fa21a04112c59ad54f69d80e376f7f9d0f5f9123ab87ecd18fbb9ec3a2beed56 \
+    --hash=sha256:fcf7d1d6f5da887ca04302db8e0e0cf56ce9a5e05f202720e49b3e8157ddb9a9 \
+    --hash=sha256:fd27d8b49e574e50caa65196d908f80e4dff64d7e592d0c59788b45aad7e8b35
     # via pytest-cov
 docutils==0.20.1 \
     --hash=sha256:96f387a2c5562db4476f09f13bbab2192e764cac08ebbf3a34a95d9b1e4a59d6 \
     --hash=sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b
     # via
     #   sphinx
     #   sphinx-rtd-theme
-exceptiongroup==1.2.0 \
-    --hash=sha256:4bfd3996ac73b41e9b9628b04e079f193850720ea5945fc96a08633c66912f14 \
-    --hash=sha256:91f5c769735f051a4290d52edd0858999b57e5876e9f85937691bd4c9fa3ed68
+exceptiongroup==1.2.1 \
+    --hash=sha256:5258b9ed329c5bbdd31a309f53cbfb0b155341807f6ff7606a1e801a891b29ad \
+    --hash=sha256:a4785e48b045528f5bfe627b6ad554ff32def154f42372786903b7abcfe1aa16
     # via pytest
-idna==3.6 \
-    --hash=sha256:9ecdbbd083b06798ae1e86adcbfe8ab1479cf864e4ee30fe4e46a003d12491ca \
-    --hash=sha256:c05567e9c24a6b9faaa835c4821bad0590fbb9d5779e7caa6e1cc4978e7eb24f
+idna==3.7 \
+    --hash=sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc \
+    --hash=sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0
     # via requests
 imagesize==1.4.1 \
     --hash=sha256:0d8d18d08f840c19d0ee7ca1fd82490fdc3729b7ac93f49870406ddde8ef8d8b \
     --hash=sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a
     # via sphinx
 iniconfig==2.0.0 \
     --hash=sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3 \
     --hash=sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374
     # via pytest
-jinja2==3.1.3 \
-    --hash=sha256:7d6d50dd97d52cbc355597bd845fabfbac3f551e1f99619e39a35ce8c370b5fa \
-    --hash=sha256:ac8bd6544d4bb2c9792bf3a159e80bba8fda7f07e81bc3aed565432d5925ba90
+jinja2==3.1.4 \
+    --hash=sha256:4a3aee7acbbe7303aede8e9648d13b8bf88a429282aa6122a993f0ac800cb369 \
+    --hash=sha256:bc5dd2abb727a5319567b7a813e6a2e7318c39f4f487cfe6c89c6f9c7d25197d
     # via
     #   reuse
     #   sphinx
-license-expression==30.2.0 \
-    --hash=sha256:1a7dc2bb2d09cdc983d072e4f9adc787e107e09def84cbb3919baaaf4f8e6fa1 \
-    --hash=sha256:599928edd995c43fc335e0af342076144dc71cb858afa1ed9c1c30c4e81794f5
+license-expression==30.3.0 \
+    --hash=sha256:1295406f736b4f395ff069aec1cebfad53c0fcb3cf57df0f5ec58fc7b905aea5 \
+    --hash=sha256:ae0ba9a829d6909c785dc2f0131f13d10d68318e4a5f28af5ef152d6b52f9b41
     # via reuse
 markupsafe==2.1.5 \
     --hash=sha256:00e046b6dd71aa03a41079792f8473dc494d564611a8f89bbbd7cb93295ebdcf \
     --hash=sha256:075202fa5b72c86ad32dc7d0b56024ebdbcf2048c0ba09f1cde31bfdd57bcfff \
     --hash=sha256:0e397ac966fdf721b2c528cf028494e86172b4feba51d65f81ffd65c63798f3f \
     --hash=sha256:17b950fccb810b3293638215058e432159d2b71005c74371d784862b7e4683f3 \
     --hash=sha256:1f3fbcb7ef1f16e48246f704ab79d79da8a46891e2da03f8783a5b6fa41a9532 \
@@ -268,117 +268,117 @@
     --hash=sha256:ec6a563cff360b50eed26f13adc43e61bc0c04d94b8be985e6fb24b81f6dcfdf \
     --hash=sha256:f5dfb42c4604dddc8e4305050aa6deb084540643ed5804d7455b5df8fe16f5e5 \
     --hash=sha256:fa173ec60341d6bb97a89f5ea19c85c5643c1e7dedebc22f5181eb73573142c5 \
     --hash=sha256:fa9db3f79de01457b03d4f01b34cf91bc0048eb2c3846ff26f66687c2f6d16ab \
     --hash=sha256:fce659a462a1be54d2ffcacea5e3ba2d74daa74f30f5f143fe0c58636e355fdd \
     --hash=sha256:ffee1f21e5ef0d712f9033568f8344d5da8cc2869dbd08d87c84656e6a2d2f68
     # via jinja2
-mypy==1.8.0 \
-    --hash=sha256:028cf9f2cae89e202d7b6593cd98db6759379f17a319b5faf4f9978d7084cdc6 \
-    --hash=sha256:2afecd6354bbfb6e0160f4e4ad9ba6e4e003b767dd80d85516e71f2e955ab50d \
-    --hash=sha256:2b5b6c721bd4aabaadead3a5e6fa85c11c6c795e0c81a7215776ef8afc66de02 \
-    --hash=sha256:42419861b43e6962a649068a61f4a4839205a3ef525b858377a960b9e2de6e0d \
-    --hash=sha256:42c6680d256ab35637ef88891c6bd02514ccb7e1122133ac96055ff458f93fc3 \
-    --hash=sha256:485a8942f671120f76afffff70f259e1cd0f0cfe08f81c05d8816d958d4577d3 \
-    --hash=sha256:4c886c6cce2d070bd7df4ec4a05a13ee20c0aa60cb587e8d1265b6c03cf91da3 \
-    --hash=sha256:4e6d97288757e1ddba10dd9549ac27982e3e74a49d8d0179fc14d4365c7add66 \
-    --hash=sha256:4ef4be7baf08a203170f29e89d79064463b7fc7a0908b9d0d5114e8009c3a259 \
-    --hash=sha256:51720c776d148bad2372ca21ca29256ed483aa9a4cdefefcef49006dff2a6835 \
-    --hash=sha256:52825b01f5c4c1c4eb0db253ec09c7aa17e1a7304d247c48b6f3599ef40db8bd \
-    --hash=sha256:538fd81bb5e430cc1381a443971c0475582ff9f434c16cd46d2c66763ce85d9d \
-    --hash=sha256:5c1538c38584029352878a0466f03a8ee7547d7bd9f641f57a0f3017a7c905b8 \
-    --hash=sha256:6ff8b244d7085a0b425b56d327b480c3b29cafbd2eff27316a004f9a7391ae07 \
-    --hash=sha256:7178def594014aa6c35a8ff411cf37d682f428b3b5617ca79029d8ae72f5402b \
-    --hash=sha256:720a5ca70e136b675af3af63db533c1c8c9181314d207568bbe79051f122669e \
-    --hash=sha256:7f1478736fcebb90f97e40aff11a5f253af890c845ee0c850fe80aa060a267c6 \
-    --hash=sha256:855fe27b80375e5c5878492f0729540db47b186509c98dae341254c8f45f42ae \
-    --hash=sha256:8963b83d53ee733a6e4196954502b33567ad07dfd74851f32be18eb932fb1cb9 \
-    --hash=sha256:9261ed810972061388918c83c3f5cd46079d875026ba97380f3e3978a72f503d \
-    --hash=sha256:99b00bc72855812a60d253420d8a2eae839b0afa4938f09f4d2aa9bb4654263a \
-    --hash=sha256:ab3c84fa13c04aeeeabb2a7f67a25ef5d77ac9d6486ff33ded762ef353aa5592 \
-    --hash=sha256:afe3fe972c645b4632c563d3f3eff1cdca2fa058f730df2b93a35e3b0c538218 \
-    --hash=sha256:d19c413b3c07cbecf1f991e2221746b0d2a9410b59cb3f4fb9557f0365a1a817 \
-    --hash=sha256:df9824ac11deaf007443e7ed2a4a26bebff98d2bc43c6da21b2b64185da011c4 \
-    --hash=sha256:e46f44b54ebddbeedbd3d5b289a893219065ef805d95094d16a0af6630f5d410 \
-    --hash=sha256:f5ac9a4eeb1ec0f1ccdc6f326bcdb464de5f80eb07fb38b5ddd7b0de6bc61e55
+mypy==1.10.0 \
+    --hash=sha256:075cbf81f3e134eadaf247de187bd604748171d6b79736fa9b6c9685b4083061 \
+    --hash=sha256:12b6bfc1b1a66095ab413160a6e520e1dc076a28f3e22f7fb25ba3b000b4ef99 \
+    --hash=sha256:1ec404a7cbe9fc0e92cb0e67f55ce0c025014e26d33e54d9e506a0f2d07fe5de \
+    --hash=sha256:28d0e038361b45f099cc086d9dd99c15ff14d0188f44ac883010e172ce86c38a \
+    --hash=sha256:2b0695d605ddcd3eb2f736cd8b4e388288c21e7de85001e9f85df9187f2b50f9 \
+    --hash=sha256:3236a4c8f535a0631f85f5fcdffba71c7feeef76a6002fcba7c1a8e57c8be1ec \
+    --hash=sha256:3be66771aa5c97602f382230165b856c231d1277c511c9a8dd058be4784472e1 \
+    --hash=sha256:3d087fcbec056c4ee34974da493a826ce316947485cef3901f511848e687c131 \
+    --hash=sha256:3f298531bca95ff615b6e9f2fc0333aae27fa48052903a0ac90215021cdcfa4f \
+    --hash=sha256:4a2b5cdbb5dd35aa08ea9114436e0d79aceb2f38e32c21684dcf8e24e1e92821 \
+    --hash=sha256:4cf18f9d0efa1b16478c4c129eabec36148032575391095f73cae2e722fcf9d5 \
+    --hash=sha256:8b2cbaca148d0754a54d44121b5825ae71868c7592a53b7292eeb0f3fdae95ee \
+    --hash=sha256:8f55583b12156c399dce2df7d16f8a5095291354f1e839c252ec6c0611e86e2e \
+    --hash=sha256:92f93b21c0fe73dc00abf91022234c79d793318b8a96faac147cd579c1671746 \
+    --hash=sha256:9e36fb078cce9904c7989b9693e41cb9711e0600139ce3970c6ef814b6ebc2b2 \
+    --hash=sha256:9fd50226364cd2737351c79807775136b0abe084433b55b2e29181a4c3c878c0 \
+    --hash=sha256:a781f6ad4bab20eef8b65174a57e5203f4be627b46291f4589879bf4e257b97b \
+    --hash=sha256:a87dbfa85971e8d59c9cc1fcf534efe664d8949e4c0b6b44e8ca548e746a8d53 \
+    --hash=sha256:b808e12113505b97d9023b0b5e0c0705a90571c6feefc6f215c1df9381256e30 \
+    --hash=sha256:bc6ac273b23c6b82da3bb25f4136c4fd42665f17f2cd850771cb600bdd2ebeda \
+    --hash=sha256:cd777b780312ddb135bceb9bc8722a73ec95e042f911cc279e2ec3c667076051 \
+    --hash=sha256:da1cbf08fb3b851ab3b9523a884c232774008267b1f83371ace57f412fe308c2 \
+    --hash=sha256:e22e1527dc3d4aa94311d246b59e47f6455b8729f4968765ac1eacf9a4760bc7 \
+    --hash=sha256:f8c083976eb530019175aabadb60921e73b4f45736760826aa1689dda8208aee \
+    --hash=sha256:f90cff89eea89273727d8783fef5d4a934be2fdca11b47def50cf5d311aff727 \
+    --hash=sha256:fa7ef5244615a2523b56c034becde4e9e3f9b034854c93639adb667ec9ec2976 \
+    --hash=sha256:fcfc70599efde5c67862a07a1aaf50e55bce629ace26bb19dc17cece5dd31ca4
     # via declinate (pyproject.toml)
 mypy-extensions==1.0.0 \
     --hash=sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d \
     --hash=sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782
     # via mypy
-packaging==23.2 \
-    --hash=sha256:048fb0e9405036518eaaf48a55953c750c11e1a1b68e0dd1a9d62ed0c092cfc5 \
-    --hash=sha256:8c491190033a9af7e1d931d0b5dacc2ef47509b34dd0de67ed209b5203fc88c7
+packaging==24.0 \
+    --hash=sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5 \
+    --hash=sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9
     # via
     #   pytest
     #   sphinx
-pluggy==1.4.0 \
-    --hash=sha256:7db9f7b503d67d1c5b95f59773ebb58a8c1c288129a88665838012cfb07b8981 \
-    --hash=sha256:8c85c2876142a764e5b7548e7d9a0e0ddb46f5185161049a79b7e974454223be
+pluggy==1.5.0 \
+    --hash=sha256:2cffa88e94fdc978c4c574f15f9e59b7f4201d439195c3715ca9e2486f1d0cf1 \
+    --hash=sha256:44e1ad92c8ca002de6377e165f3e0f1be63266ab4d554740532335b9d75ea669
     # via pytest
-pygments==2.17.2 \
-    --hash=sha256:b27c2826c47d0f3219f29554824c30c5e8945175d888647acd804ddd04af846c \
-    --hash=sha256:da46cec9fd2de5be3a8a784f434e4c4ab670b4ff54d605c4c2717e9d49c4c367
-    # via sphinx
-pytest==8.0.2 \
-    --hash=sha256:d4051d623a2e0b7e51960ba963193b09ce6daeb9759a451844a21e4ddedfc1bd \
-    --hash=sha256:edfaaef32ce5172d5466b5127b42e0d6d35ebbe4453f0e3505d96afd93f6b096
+pygments==2.18.0 \
+    --hash=sha256:786ff802f32e91311bff3889f6e9a86e81505fe99f2735bb6d60ae0c5004f199 \
+    --hash=sha256:b8e6aca0523f3ab76fee51799c488e38782ac06eafcf95e7ba832985c8e7b13a
+    # via sphinx
+pytest==8.2.1 \
+    --hash=sha256:5046e5b46d8e4cac199c373041f26be56fdb81eb4e67dc11d4e10811fc3408fd \
+    --hash=sha256:faccc5d332b8c3719f40283d0d44aa5cf101cec36f88cde9ed8f2bc0538612b1
     # via
     #   declinate (pyproject.toml)
     #   pytest-cov
-pytest-cov==4.1.0 \
-    --hash=sha256:3904b13dfbfec47f003b8e77fd5b589cd11904a21ddf1ab38a64f204d6a10ef6 \
-    --hash=sha256:6ba70b9e97e69fcc3fb45bfeab2d0a138fb65c4d0d6a41ef33983ad114be8c3a
+pytest-cov==5.0.0 \
+    --hash=sha256:4f0764a1219df53214206bf1feea4633c3b558a2925c8b59f144f682861ce652 \
+    --hash=sha256:5837b58e9f6ebd335b0f8060eecce69b662415b16dc503883a02f45dfeb14857
     # via declinate (pyproject.toml)
 python-debian==0.1.49 \
     --hash=sha256:880f3bc52e31599f2a9b432bd7691844286825087fccdcf2f6ffd5cd79a26f9f \
     --hash=sha256:8cf677a30dbcb4be7a99536c17e11308a827a4d22028dc59a67f6c6dd3f0f58c
     # via reuse
-requests==2.31.0 \
-    --hash=sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f \
-    --hash=sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1
-    # via sphinx
-reuse==3.0.1 \
-    --hash=sha256:2f13d9f31268e566e715fffe97299a002376477fada7ccd3d05a1458310cbf98 \
-    --hash=sha256:590ce429ad964c515ed5e18b1f755d9b6cf027943d940d472d107e64ede70a6f
+requests==2.32.3 \
+    --hash=sha256:55365417734eb18255590a9ff9eb97e9e1da868d4ccd6402399eaf68af20a760 \
+    --hash=sha256:70761cfe03c773ceb22aa2f671b4757976145175cdfca038c02654d061d6dcc6
+    # via sphinx
+reuse==3.0.2 \
+    --hash=sha256:73eb8262b84527a90822404e7504f69081854759806830d402ea1e92176f32a6 \
+    --hash=sha256:bf5a65c2dba4b481ee5ace18a3863095ee95ff3e72acaf6cd4446bb83d786970
     # via declinate (pyproject.toml)
-ruff==0.3.0 \
-    --hash=sha256:0886184ba2618d815067cf43e005388967b67ab9c80df52b32ec1152ab49f53a \
-    --hash=sha256:128265876c1d703e5f5e5a4543bd8be47c73a9ba223fd3989d4aa87dd06f312f \
-    --hash=sha256:19eacceb4c9406f6c41af806418a26fdb23120dfe53583df76d1401c92b7c14b \
-    --hash=sha256:23dbb808e2f1d68eeadd5f655485e235c102ac6f12ad31505804edced2a5ae77 \
-    --hash=sha256:2f7dbba46e2827dfcb0f0cc55fba8e96ba7c8700e0a866eb8cef7d1d66c25dcb \
-    --hash=sha256:3ef655c51f41d5fa879f98e40c90072b567c666a7114fa2d9fe004dffba00932 \
-    --hash=sha256:5da894a29ec018a8293d3d17c797e73b374773943e8369cfc50495573d396933 \
-    --hash=sha256:755c22536d7f1889be25f2baf6fedd019d0c51d079e8417d4441159f3bcd30c2 \
-    --hash=sha256:7deb528029bacf845bdbb3dbb2927d8ef9b4356a5e731b10eef171e3f0a85944 \
-    --hash=sha256:9343690f95710f8cf251bee1013bf43030072b9f8d012fbed6ad702ef70d360a \
-    --hash=sha256:a1f3ed501a42f60f4dedb7805fa8d4534e78b4e196f536bac926f805f0743d49 \
-    --hash=sha256:b08b356d06a792e49a12074b62222f9d4ea2a11dca9da9f68163b28c71bf1dd4 \
-    --hash=sha256:cc30a9053ff2f1ffb505a585797c23434d5f6c838bacfe206c0e6cf38c921a1e \
-    --hash=sha256:d0d3d7ef3d4f06433d592e5f7d813314a34601e6c5be8481cccb7fa760aa243e \
-    --hash=sha256:dd73fe7f4c28d317855da6a7bc4aa29a1500320818dd8f27df95f70a01b8171f \
-    --hash=sha256:e1e0d4381ca88fb2b73ea0766008e703f33f460295de658f5467f6f229658c19 \
-    --hash=sha256:e3a4a6d46aef0a84b74fcd201a4401ea9a6cd85614f6a9435f2d33dd8cefbf83
+ruff==0.4.6 \
+    --hash=sha256:04a80acfc862e0e1630c8b738e70dcca03f350bad9e106968a8108379e12b31f \
+    --hash=sha256:0cf5cc02d3ae52dfb0c8a946eb7a1d6ffe4d91846ffc8ce388baa8f627e3bd50 \
+    --hash=sha256:1fa8561489fadf483ffbb091ea94b9c39a00ed63efacd426aae2f197a45e67fc \
+    --hash=sha256:1ff930d6e05f444090a0139e4e13e1e2e1f02bd51bb4547734823c760c621e79 \
+    --hash=sha256:3a6a0a4f4b5f54fff7c860010ab3dd81425445e37d35701a965c0248819dde7a \
+    --hash=sha256:3f9ced5cbb7510fd7525448eeb204e0a22cabb6e99a3cb160272262817d49786 \
+    --hash=sha256:4d5b914818d8047270308fe3e85d9d7f4a31ec86c6475c9f418fbd1624d198e0 \
+    --hash=sha256:4f02284335c766678778475e7698b7ab83abaf2f9ff0554a07b6f28df3b5c259 \
+    --hash=sha256:602ebd7ad909eab6e7da65d3c091547781bb06f5f826974a53dbe563d357e53c \
+    --hash=sha256:735a16407a1a8f58e4c5b913ad6102722e80b562dd17acb88887685ff6f20cf6 \
+    --hash=sha256:9018bf59b3aa8ad4fba2b1dc0299a6e4e60a4c3bc62bbeaea222679865453062 \
+    --hash=sha256:a769ae07ac74ff1a019d6bd529426427c3e30d75bdf1e08bb3d46ac8f417326a \
+    --hash=sha256:a797a87da50603f71e6d0765282098245aca6e3b94b7c17473115167d8dfb0b7 \
+    --hash=sha256:be47700ecb004dfa3fd4dcdddf7322d4e632de3c06cd05329d69c45c0280e618 \
+    --hash=sha256:ea3424793c29906407e3cf417f28fc33f689dacbbadfb52b7e9a809dd535dcef \
+    --hash=sha256:ef995583a038cd4a7edf1422c9e19118e2511b8ba0b015861b4abd26ec5367c5 \
+    --hash=sha256:f13410aabd3b5776f9c5699f42b37a3a348d65498c4310589bc6e5c548dc8a2f
     # via declinate (pyproject.toml)
 snowballstemmer==2.2.0 \
     --hash=sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1 \
     --hash=sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a
     # via sphinx
-sphinx==7.2.6 \
-    --hash=sha256:1e09160a40b956dc623c910118fa636da93bd3ca0b9876a7b3df90f07d691560 \
-    --hash=sha256:9a5160e1ea90688d5963ba09a2dcd8bdd526620edbb65c328728f1b2228d5ab5
+sphinx==7.3.7 \
+    --hash=sha256:413f75440be4cacf328f580b4274ada4565fb2187d696a84970c23f77b64d8c3 \
+    --hash=sha256:a4a7db75ed37531c05002d56ed6948d4c42f473a36f46e1382b0bd76ca9627bc
     # via
     #   declinate (pyproject.toml)
     #   sphinx-autodoc-typehints
     #   sphinx-rtd-theme
     #   sphinxcontrib-jquery
-sphinx-autodoc-typehints==2.0.0 \
-    --hash=sha256:12c0e161f6fe191c2cdfd8fa3caea271f5387d9fbc67ebcd6f4f1f24ce880993 \
-    --hash=sha256:7f2cdac2e70fd9787926b6e9e541cd4ded1e838d2b46fda2a1bb0a75ec5b7f3a
+sphinx-autodoc-typehints==2.1.0 \
+    --hash=sha256:46f1a710b3ed35904f63a77c5e68334c5ee1c2e22828b75fdcd147f1c52c199b \
+    --hash=sha256:51bf8dc77c4fba747e32f0735002a91500747d0553cae616863848e8f5e49fe8
     # via declinate (pyproject.toml)
 sphinx-rtd-theme==2.0.0 \
     --hash=sha256:bd5d7b80622406762073a04ef8fadc5f9151261563d47027de09910ce03afe6b \
     --hash=sha256:ec93d0856dc280cf3aee9a4c9807c60e027c7f7b461b77aeffed682e68f0e586
     # via declinate (pyproject.toml)
 sphinxcontrib-applehelp==1.0.8 \
     --hash=sha256:c40a4f96f3776c4393d933412053962fac2b84f4c99a7982ba42e09576a70619 \
@@ -411,15 +411,18 @@
 tomli==2.0.1 \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
     # via
     #   coverage
     #   mypy
     #   pytest
-typing-extensions==4.10.0 \
-    --hash=sha256:69b1a937c3a517342112fb4c6df7e72fc39a38e7891a5730ed4985b5214b5475 \
-    --hash=sha256:b0abd7c89e8fb96f98db18d86106ff1d90ab692004eb746cf6eda2682f91b3cb
-    # via mypy
+    #   sphinx
+typing-extensions==4.12.0 \
+    --hash=sha256:8cbcdc8606ebcb0d95453ad7dc5065e6237b6aa230a31e81d0f440c30fed5fd8 \
+    --hash=sha256:b349c66bea9016ac22978d800cfff206d5f9816951f12a7d0ec5578b0a819594
+    # via
+    #   declinate (pyproject.toml)
+    #   mypy
 urllib3==2.2.1 \
     --hash=sha256:450b20ec296a467077128bff42b73080516e71b56ff59a60a02bef2232c4fa9d \
     --hash=sha256:d0570876c61ab9e520d776c38acbbb5b05a776d3f9ff98a5c8fd5162a444cf19
     # via requests
```

### Comparing `declinate-0.0.2/src/declinate/check.py` & `declinate-0.0.3/src/declinate/check.py`

 * *Files identical despite different names*

### Comparing `declinate-0.0.2/src/declinate/cli.py` & `declinate-0.0.3/src/declinate/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright 2022 - 2024 Ternaris
 # SPDX-License-Identifier: Apache-2.0
 """Generated declinate CLI."""
 
 # DO NOT EDIT THIS FILE MANUALLY
+# pyright: basic
 # ruff: noqa
 
 from __future__ import annotations
 
 import argparse
 import os
 import re
@@ -313,15 +314,15 @@
 
     next(lexer)
     laststate = lexer.state  # type: ignore[attr-defined]
     try:
         for index, token in enumerate(lexer):
             args.append(token)
             laststate = lexer.state  # type: ignore[attr-defined]
-            if cword is None and lexer.instream.tell() > pos:
+            if cword is None and lexer.instream.tell() > pos:  # type: ignore[attr-defined]
                 cword = index
     except ValueError:
         args.append(lexer.token)
         laststate = 'error'
     if laststate == ' ':
         args.append('')
     if cword is None:
@@ -380,22 +381,22 @@
 
         runargs = {
             k: v for k, v in args.items()
             if k in {
                 'package',
                 'write',
             }
-        }  # yapf: disable
+        }  # fmt: skip
         sys.exit(generate(**runargs))
 
     if _command == 'check':
         from declinate.declinate import check
 
         runargs = {
             k: v for k, v in args.items()
             if k in {
                 'package',
             }
-        }  # yapf: disable
+        }  # fmt: skip
         sys.exit(check(**runargs))
 
     sys.exit(res)
```

### Comparing `declinate-0.0.2/src/declinate/declinate.py` & `declinate-0.0.3/src/declinate/declinate.py`

 * *Files identical despite different names*

### Comparing `declinate-0.0.2/src/declinate/gen.py` & `declinate-0.0.3/src/declinate/gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,52 +11,61 @@
 import sys
 import typing
 from collections.abc import Generator
 from functools import reduce
 from importlib.util import module_from_spec, spec_from_loader
 from itertools import takewhile
 from pathlib import Path
+from types import NoneType
 from typing import (
     TYPE_CHECKING,
     Annotated,
     NamedTuple,
     NoReturn,
-    Union,
+    _SpecialForm as SpecialForm,  # pyright: ignore[reportPrivateUsage]
     cast,
     get_args,
     get_origin,
     get_type_hints,
 )
 
+if sys.version_info >= (3, 12):
+    from typing import override
+else:
+    from typing_extensions import override
+
 if TYPE_CHECKING:
     from collections.abc import Callable
     from types import ModuleType
-    from typing import ParamSpec, TypedDict, _SpecialForm
+    from typing import ParamSpec, TypeAlias, TypedDict
 
     P = ParamSpec('P')
 
     class ArgMetadata(TypedDict, total=False):
         """Argument annotation metadata."""
 
         action: str
         complete: Completer
         dest: str
         flags: list[str]
         group: str
-        help: str
+        help: str | Argtype
         required: bool
         type: Argtype
+        nodefault: str
 
-    ArgDesc = tuple[type, ArgMetadata, bool, bool | bytes | int | float | str]
+    AnyCall: TypeAlias = Callable[[], list[str]]
+    ArgDesc = tuple[type, ArgMetadata, bool, bool | bytes | int | float | str | type | None]
     Completer = Callable[[list[str], str, object], list[str]]
 
 HEADER = [
     '"""Generated declinate CLI."""',
     '',
     '# DO NOT EDIT THIS FILE MANUALLY',
+    '# pyright: basic',
     '# ruff: noqa',
     '',
     'from __future__ import annotations',
     '',
 ]
 
 HEADER_IMPORTS = [
@@ -102,16 +111,18 @@
     '    def _metavar_formatter(',
     '        self,',
     '        action: argparse.Action,',
     '        default_metavar: str,',
     '    ) -> Callable[[int], tuple[str, ...]]:',
     '        if isinstance(action, argparse._SubParsersAction) and action.choices:',
     '            choice_strs = [',
-    '                k for k, v in action.choices.items()'
-    " if not v.description.startswith('SUPPRESS.')",
+    (
+        '                k for k, v in action.choices.items()'
+        " if not v.description.startswith('SUPPRESS.')"
+    ),
     '            ]',
     '            result = f\'{{{",".join(choice_strs)}}}\'',
     '            return lambda x: (result,) * x',
     '        return super()._metavar_formatter(action, default_metavar)',
     '',
     '',
     'class ArgumentParser(argparse.ArgumentParser):',
@@ -161,16 +172,18 @@
     '"""',
     '',
     'COMPLETER_ZSH = """\\',
     '#compdef %(name)s',
     '_completer__%(name)s() {',
     '    local -a values values_descrs',
     '    (( ! $+commands[%(name)s] )) && return 1',
-    '    for reply in '
-    '"${(@f)$(env _COMPLETER=zsh COMP_LINE="$BUFFER" COMP_POINT=$CURSOR %(name)s)}"; do',
+    (
+        '    for reply in '
+        '"${(@f)$(env _COMPLETER=zsh COMP_LINE="$BUFFER" COMP_POINT=$CURSOR %(name)s)}"; do'
+    ),
     '       IFS="," read type value descr <<< "$reply"',
     '       if [[ "$type" == "directory" ]]; then',
     '           _path_files -/',
     '       elif [[ "$type" == "file" ]]; then',
     '           _path_files -f',
     '       elif [[ "$type" == "string" ]]; then',
     '           if [[ -n "$descr" ]]; then',
@@ -317,15 +330,15 @@
     '',
     '    next(lexer)',
     '    laststate = lexer.state  # type: ignore[attr-defined]',
     '    try:',
     '        for index, token in enumerate(lexer):',
     '            args.append(token)',
     '            laststate = lexer.state  # type: ignore[attr-defined]',
-    '            if cword is None and lexer.instream.tell() > pos:',
+    '            if cword is None and lexer.instream.tell() > pos:  # type: ignore[attr-defined]',
     '                cword = index',
     '    except ValueError:',
     '        args.append(lexer.token)',
     "        laststate = 'error'",
     "    if laststate == ' ':",
     "        args.append('')",
     '    if cword is None:',
@@ -373,14 +386,15 @@
 class Argtype:
     """Argument type with identity repr."""
 
     def __init__(self, name: str) -> None:
         """Save name."""
         self.name = name
 
+    @override
     def __repr__(self) -> str:
         """Use raw name as repr."""
         return self.name
 
 
 def get_module(package: str) -> ModuleType:
     """Get module for package.
@@ -396,17 +410,17 @@
     """
     module = importlib.import_module(package=package, name='.declinate')
     otc = typing.TYPE_CHECKING
     typing.TYPE_CHECKING = True
     module = importlib.reload(module)
     assert module
     assert module.__file__
-    importlib.reload(module)
+    res = importlib.reload(module)
     typing.TYPE_CHECKING = otc
-    return module
+    return res
 
 
 class DocstringInfo(NamedTuple):
     """Command information."""
 
     shortdesc: str
     description: str
@@ -421,43 +435,47 @@
     name: str
     module: str
     shortdesc: str
     description: str
     args: dict[str, ArgDesc]
     groups: dict[str, str]
     excgroups: dict[str, str]
-    returntype: type | _SpecialForm
+    returntype: type[int | Generator[None, None, int]] | SpecialForm
     is_async: bool
 
 
 def parse_docstring(doc: str) -> DocstringInfo:
     """Parse docstring."""
     flags = re.A | re.M | re.S
 
     def extract_sections(text: str) -> dict[str, str]:
-        sections = re.findall(
+        sections: list[str] = re.findall(
             r'\n\n^\w+:.*?(?=\n\n^\w+:)',
             '\n\nMain:\n' + text + '\n\nLast:\n',
             flags=flags,
         )
-        res = {}
+        res: dict[str, str] = {}
         argsection = next((x for x in sections if x.startswith('\n\nArgs:\n')), None)
         if argsection:
             idx = sections.index(argsection)
             sections = [reduce(operator.add, sections[:idx]), *sections[idx:]]
         for section in sections:
             parts = section.split(':\n', 1)
             key = parts[0].strip().lower()
             value = parts[1]
             res[key] = value
         return res
 
     def extract_key_value(text: str) -> dict[str, str]:
-        sections = re.findall(r' {4}\w+: .*?(?= {4}\w+: )', text + '\n    Last: ', flags=flags)
-        res = {}
+        sections: list[str] = re.findall(
+            r' {4}\w+: .*?(?= {4}\w+: )',
+            text + '\n    Last: ',
+            flags=flags,
+        )
+        res: dict[str, str] = {}
         for section in sections:
             parts = section.split(': ', 1)
             key = parts[0].strip().lower()
             value = parts[1]
             res[key] = ' '.join(x.strip() for x in value.split('\n')).strip()
         return res
 
@@ -515,42 +533,43 @@
     is_async = inspect.iscoroutinefunction(command)
     if not doc:
         msg = f'No docstring on {command!r}'
         raise DeclinateError(msg)
     docstrinfo = parse_docstring(doc)
 
     signature = inspect.signature(command)
-    hints = get_type_hints(command, include_extras=True)
+    hints: dict[str, type] = get_type_hints(command, include_extras=True)
 
-    args = {}
+    args: dict[str, ArgDesc] = {}
     for argname, parameter in signature.parameters.items():
         annotation = hints[argname]
-        if get_origin(annotation) is Union:
-            annotation = get_args(annotation)[0]
+        if get_origin(annotation) and get_args(annotation)[-1] is NoneType:
+            annotation = cast('type', get_args(annotation)[0])
 
         if get_origin(annotation) is Annotated:
-            annotation, metadata = get_args(annotation)
-            metadata = dict(metadata)
+            annotation, _metadata = cast('tuple[type, list[tuple[str, str]]]', get_args(annotation))
+            metadata: ArgMetadata = cast('ArgMetadata', cast('object', dict(_metadata)))
         else:
             metadata = {}
 
         helpstr = docstrinfo.args[argname]
-        has_default = parameter.default != inspect.Parameter.empty
+        default = cast('bool | bytes | int | float | str | type | None', parameter.default)  # pyright: ignore[reportAny]
+        has_default = default != inspect.Parameter.empty
 
         if 'help' not in metadata:
             if (
                 annotation != bool
                 and has_default
                 and metadata.get('action') != 'count'
                 and metadata.pop('nodefault', None) is None
             ):
-                helpstr += f' (default={parameter.default!r})'
+                helpstr += f' (default={default!r})'
             metadata['help'] = helpstr
 
-        args[argname] = (annotation, metadata, has_default, parameter.default)
+        args[argname] = (annotation, metadata, has_default, default)
 
     return CommandInfo(
         name,
         module,
         docstrinfo.shortdesc,
         docstrinfo.description,
         args,
@@ -612,30 +631,30 @@
         if has_default and default is True:
             metadata['action'] = 'store_false'
         else:
             metadata['action'] = 'store_true'
     elif metadata.get('action') != 'count':
         typ = annotation.__name__
         if typ == 'Sequence':
-            typ = get_args(annotation)[0].__name__
+            typ = cast('type', get_args(annotation)[0]).__name__
         metadata['type'] = Argtype(typ)
 
     param = [f'{x!r}' for x in names]
     param += [f'{k}={v!r}' for k, v in metadata.items()]
 
     if annotation.__module__ != 'builtins':
         imp = f'from {annotation.__module__} import {annotation.__name__}\n'
     else:
         imp = ''
 
     if group := metadata.pop('group', None):
         parent = f'{parent}_{group}'
 
-    if metadata.get('help', '').startswith('SUPPRESS'):
-        metadata['help'] = cast('str', Argtype('argparse.SUPPRESS'))
+    if cast('str', metadata.get('help', '')).startswith('SUPPRESS'):
+        metadata['help'] = Argtype('argparse.SUPPRESS')
 
     if 'complete' in metadata:
         actionname = f'ACTION{len(completers)}'
         completers[actionname] = metadata.pop('complete')
         actionis = f'{actionname} = '
     else:
         actionis = ''
@@ -656,16 +675,16 @@
     command: CommandInfo,
     defargs: dict[str, str],
     completers: dict[str, Completer],
     *,
     is_sub: bool = False,
 ) -> tuple[list[str], list[str]]:
     """Generate argument code, imports, and group information."""
-    code = []
-    imports = []
+    code: list[str] = []
+    imports: list[str] = []
 
     parent = 'SUB' if is_sub else 'PARSER'
 
     args = [
         generate_argument_code(k, v, parent, completers)
         for k, v in command.args.items()
         if k not in defargs
@@ -674,25 +693,25 @@
     for group in sorted(allgroups):
         assert group
         if (helpstr := command.groups.get(group, None)) is not None:
             if helpstr != 'SUPPRESS.':
                 code += [
                     f'{parent}_{group} = {parent}.add_argument_group(',
                     f'    {helpstr!r},',
-                    ')  # yapf: disable',
+                    ')  # fmt: skip',
                 ]
             else:
                 code += [f'{parent}_{group} = {parent}.add_argument_group()']
         else:
             helpstr = command.excgroups[group]
             if helpstr != 'SUPPRESS.':
                 code += [
                     f'{parent}_{group} = {parent}.add_argument_group(',
                     f'    {helpstr!r},',
-                    ').add_mutually_exclusive_group()  # yapf: disable',
+                    ').add_mutually_exclusive_group()  # fmt: skip',
                 ]
             else:
                 code += [f'{parent}_{group} = {parent}.add_mutually_exclusive_group()']
 
     for argcode, argimport, _ in args:
         code += argcode
         imports += [argimport]
@@ -705,15 +724,15 @@
     indent: int,
     *,
     terminal: bool = False,
     context: bool = False,
 ) -> list[str]:
     """Generate code to launch command."""
     spaces = ' ' * indent
-    res = []
+    res: list[str] = []
     if 'argparser' in cmd.args:
         run = f'{cmd.name}(argparser=PARSER, **runargs)'
     else:
         run = f'{cmd.name}(**runargs)'
     if cmd.is_async:
         res += [f'{spaces}import asyncio', '']
         run = f'asyncio.run({run})'
@@ -723,15 +742,15 @@
     else:
         res += [
             f'{spaces}runargs = {{',
             f'{spaces}    k: v for k, v in args.items()',
             f'{spaces}    if k in {{',
             *[f'{spaces}        {x!r},' for x in cmd.args],
             f'{spaces}    }}',
-            f'{spaces}}}  # yapf: disable',
+            f'{spaces}}}  # fmt: skip',
         ]
     if terminal:
         res += [f'{spaces}sys.exit({run})\n']
     elif context:
         res += [f'{spaces}with {run}:']
     else:
         res += [f'{spaces}res = {run}\n']
@@ -753,62 +772,56 @@
     """
     module = get_module(package)
     assert module.__file__
     source = inspect.getsource(module)
     copyright_header = list(takewhile(lambda x: x.startswith('#'), source.split('\n')))
     otc = typing.TYPE_CHECKING
     typing.TYPE_CHECKING = True
-    allfuncs = [module.COMMAND]
-    if addargfn := getattr(module, 'ADDARGFN', None):
-        allfuncs.append(addargfn)
-    if subcommands := getattr(module, 'SUBCOMMANDS', None):
+    allfuncs: list[AnyCall] = [cast('AnyCall', module.COMMAND)]  # pyright: ignore[reportAny]
+    if addargs := cast('AnyCall | None', getattr(module, 'ADDARGFN', None)):
+        allfuncs.append(addargs)
+    if subcommands := cast('list[AnyCall]', getattr(module, 'SUBCOMMANDS', [])):
         allfuncs.extend(subcommands)
     for func in allfuncs:
-        importlib.reload(sys.modules[func.__module__])
+        _ = importlib.reload(sys.modules[func.__module__])
     typing.TYPE_CHECKING = otc
 
     imports = HEADER_IMPORTS.copy()
     completers: dict[str, Completer] = {}
-    res = []
+    res: list[str] = []
 
-    if addargs := getattr(module, 'ADDARGFN', None):
-        defargs = get_type_hints(get_type_hints(addargs)['return'])
-    else:
-        defargs = {}
+    defargs = get_type_hints(cast('type', get_type_hints(addargs)['return'])) if addargs else {}
 
-    root_command = module.COMMAND
+    root_command = allfuncs[0]
     root_commandinfo = inspect_command(root_command)
     for key in defargs:
         assert key in root_commandinfo.args, f'Addarg {key!r} needs to be argument to all commands'
 
     res += ['# fmt: off']
     res += generate_parser_code(root_commandinfo)
     lines, imps = generate_groups_arguments_code(root_commandinfo, defargs, completers)
     res += lines
     imports += imps
 
-    root_executable = root_commandinfo.returntype in (
-        int,
-        Generator[None, None, int],
-    )
+    root_executable = root_commandinfo.returntype in (int, Generator[None, None, int])
     root_context = root_commandinfo.returntype == Generator[None, None, int]
     res.append('')
 
     subinfos = []
-    if subcommands := getattr(module, 'SUBCOMMANDS', None):
+    if subcommands:
         res += [
             'SUBS = PARSER.add_subparsers(',
             "    title='sub commands',",
             "    dest='_command',",
             f'    required={not root_executable},',
             ')',
             '',
         ]
         subinfos = [inspect_command(x) for x in subcommands]
-        hidden = []
+        hidden: list[str] = []
         for commandinfo in subinfos:
             for key in defargs:
                 assert (
                     key in commandinfo.args
                 ), f'Addarg {key!r} needs to be argument to all commands'
 
             if commandinfo.shortdesc.startswith('SUPPRESS.'):
@@ -940,15 +953,15 @@
     spec = spec_from_loader('_trycli', loader=None)
     assert spec
     nmodule = module_from_spec(spec)
     exec(code, nmodule.__dict__)  # noqa: S102
 
     if write:
         clipath = Path(module.__file__).parent / 'cli.py'
-        clipath.write_text(code)
+        _ = clipath.write_text(code)
 
         testcode = [
             *copyright_header,
             '"""Generated declinate CLI tests."""',
             '',
             '# DO NOT EDIT THIS FILE MANUALLY',
             '',
@@ -969,10 +982,10 @@
             '    assert inspect.isfunction(main)',
             '',
         ]
 
         testbase = Path(module.__file__).parents[len(package.split('.')) + 1] / 'tests'
         testpath = testbase / package.replace('.', '/') / 'test_cli.py'
         if testpath.parent.exists():
-            testpath.write_text('\n'.join(testcode))
+            _ = testpath.write_text('\n'.join(testcode))
 
     return code
```

### Comparing `declinate-0.0.2/src/declinate.egg-info/PKG-INFO` & `declinate-0.0.3/src/declinate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: declinate
-Version: 0.0.2
+Version: 0.0.3
 Summary: CLI generator.
 Author-email: Ternaris <team@ternaris.com>
 License: Apache-2.0
 Project-URL: Homepage, https://gitlab.com/ternaris/declinate
 Project-URL: Documentation, https://ternaris.gitlab.io/declinate
 Project-URL: Source, https://gitlab.com/ternaris/declinate
 Project-URL: Issues, https://gitlab.com/ternaris/declinate/issues
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
+Requires-Dist: typing_extensions
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: reuse; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
```

### Comparing `declinate-0.0.2/src/declinate.egg-info/SOURCES.txt` & `declinate-0.0.3/src/declinate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `declinate-0.0.2/tests/declinate/cli0_minimal/cli.py` & `declinate-0.0.3/tests/declinate/cli0_minimal/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright 2022 - 2024 Ternaris
 # SPDX-License-Identifier: Apache-2.0
 """Generated declinate CLI."""
 
 # DO NOT EDIT THIS FILE MANUALLY
+# pyright: basic
 # ruff: noqa
 
 from __future__ import annotations
 
 import argparse
 import os
 import re
@@ -261,15 +262,15 @@
 
     next(lexer)
     laststate = lexer.state  # type: ignore[attr-defined]
     try:
         for index, token in enumerate(lexer):
             args.append(token)
             laststate = lexer.state  # type: ignore[attr-defined]
-            if cword is None and lexer.instream.tell() > pos:
+            if cword is None and lexer.instream.tell() > pos:  # type: ignore[attr-defined]
                 cword = index
     except ValueError:
         args.append(lexer.token)
         laststate = 'error'
     if laststate == ' ':
         args.append('')
     if cword is None:
@@ -318,9 +319,9 @@
 
     from tests.declinate.cli0_minimal.declinate import command
 
     runargs = {
         k: v for k, v in args.items()
         if k in {
         }
-    }  # yapf: disable
+    }  # fmt: skip
     sys.exit(command(**runargs))
```

### Comparing `declinate-0.0.2/tests/declinate/cli1_arguments/cli.py` & `declinate-0.0.3/tests/declinate/cli1_arguments/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright 2022 - 2024 Ternaris
 # SPDX-License-Identifier: Apache-2.0
 """Generated declinate CLI."""
 
 # DO NOT EDIT THIS FILE MANUALLY
+# pyright: basic
 # ruff: noqa
 
 from __future__ import annotations
 
 import argparse
 import os
 import re
@@ -316,15 +317,15 @@
 
     next(lexer)
     laststate = lexer.state  # type: ignore[attr-defined]
     try:
         for index, token in enumerate(lexer):
             args.append(token)
             laststate = lexer.state  # type: ignore[attr-defined]
-            if cword is None and lexer.instream.tell() > pos:
+            if cword is None and lexer.instream.tell() > pos:  # type: ignore[attr-defined]
                 cword = index
     except ValueError:
         args.append(lexer.token)
         laststate = 'error'
     if laststate == ' ':
         args.append('')
     if cword is None:
@@ -383,9 +384,9 @@
             'path',
             'boolean',
             'deffalse_boolean',
             'deftrue_boolean',
             'optional_number',
             'helpover',
         }
-    }  # yapf: disable
+    }  # fmt: skip
     sys.exit(command(argparser=PARSER, **runargs))
```

### Comparing `declinate-0.0.2/tests/declinate/cli1_arguments/declinate.py` & `declinate-0.0.3/tests/declinate/cli1_arguments/declinate.py`

 * *Files identical despite different names*

### Comparing `declinate-0.0.2/tests/declinate/cli2_groups/cli.py` & `declinate-0.0.3/tests/declinate/cli2_groups/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright 2022 - 2024 Ternaris
 # SPDX-License-Identifier: Apache-2.0
 """Generated declinate CLI."""
 
 # DO NOT EDIT THIS FILE MANUALLY
+# pyright: basic
 # ruff: noqa
 
 from __future__ import annotations
 
 import argparse
 import os
 import re
@@ -80,19 +81,19 @@
         '\n'
         'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod\n'
         'tempor incididunt ut labore et dolore magna aliqua.'
     ),
 )
 PARSER_a = PARSER.add_argument_group(
     'Group A.',
-)  # yapf: disable
+)  # fmt: skip
 PARSER_b = PARSER.add_argument_group()
 PARSER_c = PARSER.add_argument_group(
     'Group C.',
-).add_mutually_exclusive_group()  # yapf: disable
+).add_mutually_exclusive_group()  # fmt: skip
 PARSER_d = PARSER.add_mutually_exclusive_group()
 PARSER_a.add_argument(
     '--grpai',
     help='Int in group a.',
     dest='grpa_int',
     required=True,
     type=int,
@@ -326,15 +327,15 @@
 
     next(lexer)
     laststate = lexer.state  # type: ignore[attr-defined]
     try:
         for index, token in enumerate(lexer):
             args.append(token)
             laststate = lexer.state  # type: ignore[attr-defined]
-            if cword is None and lexer.instream.tell() > pos:
+            if cword is None and lexer.instream.tell() > pos:  # type: ignore[attr-defined]
                 cword = index
     except ValueError:
         args.append(lexer.token)
         laststate = 'error'
     if laststate == ' ':
         args.append('')
     if cword is None:
@@ -391,9 +392,9 @@
             'grpb_int',
             'grpb_float',
             'excc_int',
             'excc_float',
             'excd_int',
             'excd_float',
         }
-    }  # yapf: disable
+    }  # fmt: skip
     sys.exit(command(**runargs))
```

### Comparing `declinate-0.0.2/tests/declinate/cli2_groups/declinate.py` & `declinate-0.0.3/tests/declinate/cli2_groups/declinate.py`

 * *Files identical despite different names*

### Comparing `declinate-0.0.2/tests/declinate/cli3_withsubcommands/cli.py` & `declinate-0.0.3/tests/declinate/cli3_withsubcommands/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright 2022 - 2024 Ternaris
 # SPDX-License-Identifier: Apache-2.0
 """Generated declinate CLI."""
 
 # DO NOT EDIT THIS FILE MANUALLY
+# pyright: basic
 # ruff: noqa
 
 from __future__ import annotations
 
 import argparse
 import os
 import re
@@ -281,15 +282,15 @@
 
     next(lexer)
     laststate = lexer.state  # type: ignore[attr-defined]
     try:
         for index, token in enumerate(lexer):
             args.append(token)
             laststate = lexer.state  # type: ignore[attr-defined]
-            if cword is None and lexer.instream.tell() > pos:
+            if cword is None and lexer.instream.tell() > pos:  # type: ignore[attr-defined]
                 cword = index
     except ValueError:
         args.append(lexer.token)
         laststate = 'error'
     if laststate == ' ':
         args.append('')
     if cword is None:
@@ -349,11 +350,11 @@
         from tests.declinate.cli3_withsubcommands.declinate import subcommand
 
         runargs = {
             k: v for k, v in args.items()
             if k in {
                 'number',
             }
-        }  # yapf: disable
+        }  # fmt: skip
         sys.exit(asyncio.run(subcommand(**runargs)))
 
     sys.exit(res)
```

### Comparing `declinate-0.0.2/tests/declinate/cli3_withsubcommands/declinate.py` & `declinate-0.0.3/tests/declinate/cli3_withsubcommands/declinate.py`

 * *Files identical despite different names*

### Comparing `declinate-0.0.2/tests/declinate/cli4_justsubcommands/cli.py` & `declinate-0.0.3/tests/declinate/cli4_justsubcommands/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright 2022 - 2024 Ternaris
 # SPDX-License-Identifier: Apache-2.0
 """Generated declinate CLI."""
 
 # DO NOT EDIT THIS FILE MANUALLY
+# pyright: basic
 # ruff: noqa
 
 from __future__ import annotations
 
 import argparse
 import os
 import re
@@ -281,15 +282,15 @@
 
     next(lexer)
     laststate = lexer.state  # type: ignore[attr-defined]
     try:
         for index, token in enumerate(lexer):
             args.append(token)
             laststate = lexer.state  # type: ignore[attr-defined]
-            if cword is None and lexer.instream.tell() > pos:
+            if cword is None and lexer.instream.tell() > pos:  # type: ignore[attr-defined]
                 cword = index
     except ValueError:
         args.append(lexer.token)
         laststate = 'error'
     if laststate == ' ':
         args.append('')
     if cword is None:
@@ -344,11 +345,11 @@
         from tests.declinate.cli4_justsubcommands.declinate import subcommand
 
         runargs = {
             k: v for k, v in args.items()
             if k in {
                 'number',
             }
-        }  # yapf: disable
+        }  # fmt: skip
         sys.exit(asyncio.run(subcommand(**runargs)))
 
     raise Exception  # pylint: disable=broad-exception-raised
```

### Comparing `declinate-0.0.2/tests/declinate/cli4_justsubcommands/declinate.py` & `declinate-0.0.3/tests/declinate/cli4_justsubcommands/declinate.py`

 * *Files identical despite different names*

### Comparing `declinate-0.0.2/tests/declinate/cli5_addargfn/cli.py` & `declinate-0.0.3/tests/declinate/cli5_addargfn/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright 2022 - 2024 Ternaris
 # SPDX-License-Identifier: Apache-2.0
 """Generated declinate CLI."""
 
 # DO NOT EDIT THIS FILE MANUALLY
+# pyright: basic
 # ruff: noqa
 
 from __future__ import annotations
 
 import argparse
 import os
 import re
@@ -278,15 +279,15 @@
 
     next(lexer)
     laststate = lexer.state  # type: ignore[attr-defined]
     try:
         for index, token in enumerate(lexer):
             args.append(token)
             laststate = lexer.state  # type: ignore[attr-defined]
-            if cword is None and lexer.instream.tell() > pos:
+            if cword is None and lexer.instream.tell() > pos:  # type: ignore[attr-defined]
                 cword = index
     except ValueError:
         args.append(lexer.token)
         laststate = 'error'
     if laststate == ' ':
         args.append('')
     if cword is None:
@@ -341,25 +342,25 @@
 
     runargs = {
         k: v for k, v in args.items()
         if k in {
             'arg_foo',
             'arg_bar',
         }
-    }  # yapf: disable
+    }  # fmt: skip
     res = command(**runargs)
 
     _command = args.pop('_command')
     _subaction = args['subaction'] if 'subaction' in args else None
     if _command == 'subcommand':
         from tests.declinate.cli5_addargfn.declinate import subcommand
 
         runargs = {
             k: v for k, v in args.items()
             if k in {
                 'arg_foo',
                 'arg_bar',
             }
-        }  # yapf: disable
+        }  # fmt: skip
         sys.exit(subcommand(**runargs))
 
     sys.exit(res)
```

### Comparing `declinate-0.0.2/tests/declinate/cli5_addargfn/declinate.py` & `declinate-0.0.3/tests/declinate/cli5_addargfn/declinate.py`

 * *Files identical despite different names*

