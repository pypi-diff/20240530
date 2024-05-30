# Comparing `tmp/jsonrpc-py-3.2.9.tar.gz` & `tmp/jsonrpc_py-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonrpc-py-3.2.9.tar", last modified: Sat Mar  9 22:56:10 2024, max compression
+gzip compressed data, was "jsonrpc_py-3.3.0.tar", last modified: Thu May 30 13:59:29 2024, max compression
```

## Comparing `jsonrpc-py-3.2.9.tar` & `jsonrpc_py-3.3.0.tar`

### file list

```diff
@@ -1,111 +1,112 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-09 22:56:10.765873 jsonrpc-py-3.2.9/
--rw-rw-rw-   0 root         (0) root         (0)      214 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)       72 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/.flake8
--rw-rw-rw-   0 root         (0) root         (0)       78 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/.gitattributes
--rw-rw-rw-   0 root         (0) root         (0)      320 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1312 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1499 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)     1277 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/Makefile
--rw-r--r--   0 root         (0) root         (0)     2918 2024-03-09 22:56:10.764873 jsonrpc-py-3.2.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1411 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-09 22:56:10.736873 jsonrpc-py-3.2.9/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-09 22:56:10.730873 jsonrpc-py-3.2.9/docs/changelog/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-09 22:56:10.738873 jsonrpc-py-3.2.9/docs/changelog/v1.x.x/
--rw-rw-rw-   0 root         (0) root         (0)       98 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v1.x.x/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      156 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v1.x.x/v1.0.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      234 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v1.x.x/v1.0.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      346 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v1.x.x/v1.0.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      433 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v1.x.x/v1.0.3.rst
--rw-rw-rw-   0 root         (0) root         (0)      386 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v1.x.x/v1.0.4.rst
--rw-rw-rw-   0 root         (0) root         (0)      567 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v1.x.x/v1.1.0.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-09 22:56:10.746873 jsonrpc-py-3.2.9/docs/changelog/v2.x.x/
--rw-rw-rw-   0 root         (0) root         (0)      233 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v2.x.x/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      322 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v2.x.x/v2.0.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      539 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v2.x.x/v2.0.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      420 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v2.x.x/v2.0.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      421 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v2.x.x/v2.1.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      368 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v2.x.x/v2.2.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      368 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v2.x.x/v2.2.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      182 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v2.x.x/v2.2.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      397 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v2.x.x/v2.2.3.rst
--rw-rw-rw-   0 root         (0) root         (0)      669 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v2.x.x/v2.3.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      466 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v2.x.x/v2.4.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      345 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v2.x.x/v2.4.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      263 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v2.x.x/v2.4.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      314 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v2.x.x/v2.4.3.rst
--rw-rw-rw-   0 root         (0) root         (0)      152 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v2.x.x/v2.4.4.rst
--rw-rw-rw-   0 root         (0) root         (0)      320 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v2.x.x/v2.4.5.rst
--rw-rw-rw-   0 root         (0) root         (0)      270 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v2.x.x/v2.4.6.rst
--rw-rw-rw-   0 root         (0) root         (0)      289 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v2.x.x/v2.4.7.rst
--rw-rw-rw-   0 root         (0) root         (0)      321 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v2.x.x/v2.4.8.rst
--rw-rw-rw-   0 root         (0) root         (0)      154 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v2.x.x/v2.4.9.rst
--rw-rw-rw-   0 root         (0) root         (0)      284 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v2.x.x/v2.5.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      265 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v2.x.x/v2.5.1.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-09 22:56:10.755873 jsonrpc-py-3.2.9/docs/changelog/v3.x.x/
--rw-rw-rw-   0 root         (0) root         (0)      300 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v3.x.x/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      720 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v3.x.x/v3.0.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      278 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v3.x.x/v3.0.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      210 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v3.x.x/v3.0.10.rst
--rw-rw-rw-   0 root         (0) root         (0)      196 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v3.x.x/v3.0.11.rst
--rw-rw-rw-   0 root         (0) root         (0)      209 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v3.x.x/v3.0.12.rst
--rw-rw-rw-   0 root         (0) root         (0)      211 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v3.x.x/v3.0.13.rst
--rw-rw-rw-   0 root         (0) root         (0)      211 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v3.x.x/v3.0.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      206 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v3.x.x/v3.0.3.rst
--rw-rw-rw-   0 root         (0) root         (0)      170 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v3.x.x/v3.0.4.rst
--rw-rw-rw-   0 root         (0) root         (0)      266 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v3.x.x/v3.0.5.rst
--rw-rw-rw-   0 root         (0) root         (0)      355 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v3.x.x/v3.0.6.rst
--rw-rw-rw-   0 root         (0) root         (0)      251 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v3.x.x/v3.0.7.rst
--rw-rw-rw-   0 root         (0) root         (0)      195 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v3.x.x/v3.0.8.rst
--rw-rw-rw-   0 root         (0) root         (0)      198 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v3.x.x/v3.0.9.rst
--rw-rw-rw-   0 root         (0) root         (0)      309 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v3.x.x/v3.1.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      232 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v3.x.x/v3.1.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      222 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v3.x.x/v3.1.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      207 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v3.x.x/v3.1.3.rst
--rw-rw-rw-   0 root         (0) root         (0)      281 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v3.x.x/v3.2.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      331 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v3.x.x/v3.2.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      196 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v3.x.x/v3.2.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      223 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v3.x.x/v3.2.3.rst
--rw-rw-rw-   0 root         (0) root         (0)      443 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v3.x.x/v3.2.4.rst
--rw-rw-rw-   0 root         (0) root         (0)      181 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v3.x.x/v3.2.5.rst
--rw-rw-rw-   0 root         (0) root         (0)      170 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v3.x.x/v3.2.6.rst
--rw-rw-rw-   0 root         (0) root         (0)      215 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v3.x.x/v3.2.7.rst
--rw-rw-rw-   0 root         (0) root         (0)      173 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v3.x.x/v3.2.8.rst
--rw-rw-rw-   0 root         (0) root         (0)      242 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog/v3.x.x/v3.2.9.rst
--rw-rw-rw-   0 root         (0) root         (0)      696 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1461 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     2653 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/deployment.rst
--rw-rw-rw-   0 root         (0) root         (0)     1752 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1867 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/quickstart.rst
--rw-rw-rw-   0 root         (0) root         (0)      863 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/docs/reference.rst
--rw-rw-rw-   0 root         (0) root         (0)     1909 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      276 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-09 22:56:10.765873 jsonrpc-py-3.2.9/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-09 22:56:10.730873 jsonrpc-py-3.2.9/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-09 22:56:10.759873 jsonrpc-py-3.2.9/src/jsonrpc/
--rw-rw-rw-   0 root         (0) root         (0)      590 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/src/jsonrpc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8834 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/src/jsonrpc/asgi.py
--rw-rw-rw-   0 root         (0) root         (0)     4412 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/src/jsonrpc/dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)     2313 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/src/jsonrpc/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     3946 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/src/jsonrpc/lifespan.py
--rw-rw-rw-   0 root         (0) root         (0)       59 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/src/jsonrpc/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     6144 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/src/jsonrpc/requests.py
--rw-rw-rw-   0 root         (0) root         (0)     4152 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/src/jsonrpc/responses.py
--rw-rw-rw-   0 root         (0) root         (0)     2122 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/src/jsonrpc/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)     3533 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/src/jsonrpc/typedefs.py
--rw-rw-rw-   0 root         (0) root         (0)     6489 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/src/jsonrpc/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-09 22:56:10.764873 jsonrpc-py-3.2.9/src/jsonrpc_py.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2918 2024-03-09 22:56:10.000000 jsonrpc-py-3.2.9/src/jsonrpc_py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2798 2024-03-09 22:56:10.000000 jsonrpc-py-3.2.9/src/jsonrpc_py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-09 22:56:10.000000 jsonrpc-py-3.2.9/src/jsonrpc_py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-03-09 22:56:10.000000 jsonrpc-py-3.2.9/src/jsonrpc_py.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-03-09 22:56:10.000000 jsonrpc-py-3.2.9/src/jsonrpc_py.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-09 22:56:10.763873 jsonrpc-py-3.2.9/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13875 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/tests/test_asgi.py
--rw-rw-rw-   0 root         (0) root         (0)     3714 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/tests/test_dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)     1928 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/tests/test_errors.py
--rw-rw-rw-   0 root         (0) root         (0)     5152 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/tests/test_lifespan.py
--rw-rw-rw-   0 root         (0) root         (0)     8215 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/tests/test_requests.py
--rw-rw-rw-   0 root         (0) root         (0)     5833 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/tests/test_responses.py
--rw-rw-rw-   0 root         (0) root         (0)     1200 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/tests/test_serializers.py
--rw-rw-rw-   0 root         (0) root         (0)     7526 2024-03-09 22:55:55.000000 jsonrpc-py-3.2.9/tests/test_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 13:59:29.555700 jsonrpc_py-3.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)      214 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)       72 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)       78 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/.gitattributes
+-rw-rw-rw-   0 root         (0) root         (0)      320 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1312 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1499 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/Makefile
+-rw-r--r--   0 root         (0) root         (0)     2918 2024-05-30 13:59:29.555700 jsonrpc_py-3.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1411 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 13:59:29.538700 jsonrpc_py-3.3.0/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 13:59:29.534700 jsonrpc_py-3.3.0/docs/changelog/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 13:59:29.539700 jsonrpc_py-3.3.0/docs/changelog/v1.x.x/
+-rw-rw-rw-   0 root         (0) root         (0)       98 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v1.x.x/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      156 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v1.x.x/v1.0.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      234 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v1.x.x/v1.0.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      346 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v1.x.x/v1.0.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      433 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v1.x.x/v1.0.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      386 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v1.x.x/v1.0.4.rst
+-rw-rw-rw-   0 root         (0) root         (0)      567 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v1.x.x/v1.1.0.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 13:59:29.544700 jsonrpc_py-3.3.0/docs/changelog/v2.x.x/
+-rw-rw-rw-   0 root         (0) root         (0)      233 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v2.x.x/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      322 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v2.x.x/v2.0.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      539 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v2.x.x/v2.0.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      420 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v2.x.x/v2.0.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      421 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v2.x.x/v2.1.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      368 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v2.x.x/v2.2.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      368 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v2.x.x/v2.2.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      182 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v2.x.x/v2.2.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      397 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v2.x.x/v2.2.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      669 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v2.x.x/v2.3.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      466 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v2.x.x/v2.4.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      345 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v2.x.x/v2.4.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      263 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v2.x.x/v2.4.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      314 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v2.x.x/v2.4.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      152 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v2.x.x/v2.4.4.rst
+-rw-rw-rw-   0 root         (0) root         (0)      320 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v2.x.x/v2.4.5.rst
+-rw-rw-rw-   0 root         (0) root         (0)      270 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v2.x.x/v2.4.6.rst
+-rw-rw-rw-   0 root         (0) root         (0)      289 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v2.x.x/v2.4.7.rst
+-rw-rw-rw-   0 root         (0) root         (0)      321 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v2.x.x/v2.4.8.rst
+-rw-rw-rw-   0 root         (0) root         (0)      154 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v2.x.x/v2.4.9.rst
+-rw-rw-rw-   0 root         (0) root         (0)      284 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v2.x.x/v2.5.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      265 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v2.x.x/v2.5.1.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 13:59:29.549700 jsonrpc_py-3.3.0/docs/changelog/v3.x.x/
+-rw-rw-rw-   0 root         (0) root         (0)      309 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v3.x.x/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      720 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v3.x.x/v3.0.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      278 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v3.x.x/v3.0.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      210 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v3.x.x/v3.0.10.rst
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v3.x.x/v3.0.11.rst
+-rw-rw-rw-   0 root         (0) root         (0)      209 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v3.x.x/v3.0.12.rst
+-rw-rw-rw-   0 root         (0) root         (0)      211 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v3.x.x/v3.0.13.rst
+-rw-rw-rw-   0 root         (0) root         (0)      211 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v3.x.x/v3.0.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      206 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v3.x.x/v3.0.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      170 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v3.x.x/v3.0.4.rst
+-rw-rw-rw-   0 root         (0) root         (0)      266 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v3.x.x/v3.0.5.rst
+-rw-rw-rw-   0 root         (0) root         (0)      355 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v3.x.x/v3.0.6.rst
+-rw-rw-rw-   0 root         (0) root         (0)      251 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v3.x.x/v3.0.7.rst
+-rw-rw-rw-   0 root         (0) root         (0)      195 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v3.x.x/v3.0.8.rst
+-rw-rw-rw-   0 root         (0) root         (0)      198 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v3.x.x/v3.0.9.rst
+-rw-rw-rw-   0 root         (0) root         (0)      309 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v3.x.x/v3.1.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      232 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v3.x.x/v3.1.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      222 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v3.x.x/v3.1.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      207 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v3.x.x/v3.1.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      281 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v3.x.x/v3.2.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      331 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v3.x.x/v3.2.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v3.x.x/v3.2.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      223 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v3.x.x/v3.2.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      443 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v3.x.x/v3.2.4.rst
+-rw-rw-rw-   0 root         (0) root         (0)      181 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v3.x.x/v3.2.5.rst
+-rw-rw-rw-   0 root         (0) root         (0)      170 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v3.x.x/v3.2.6.rst
+-rw-rw-rw-   0 root         (0) root         (0)      215 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v3.x.x/v3.2.7.rst
+-rw-rw-rw-   0 root         (0) root         (0)      173 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v3.x.x/v3.2.8.rst
+-rw-rw-rw-   0 root         (0) root         (0)      242 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v3.x.x/v3.2.9.rst
+-rw-rw-rw-   0 root         (0) root         (0)      228 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog/v3.x.x/v3.3.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      696 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2653 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/deployment.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1752 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/quickstart.rst
+-rw-rw-rw-   0 root         (0) root         (0)      863 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/docs/reference.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1909 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      278 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 13:59:29.555700 jsonrpc_py-3.3.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 13:59:29.535700 jsonrpc_py-3.3.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 13:59:29.552700 jsonrpc_py-3.3.0/src/jsonrpc/
+-rw-rw-rw-   0 root         (0) root         (0)      590 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/src/jsonrpc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8813 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/src/jsonrpc/asgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     4412 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/src/jsonrpc/dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     2313 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/src/jsonrpc/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     3946 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/src/jsonrpc/lifespan.py
+-rw-rw-rw-   0 root         (0) root         (0)       59 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/src/jsonrpc/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     6144 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/src/jsonrpc/requests.py
+-rw-rw-rw-   0 root         (0) root         (0)     4152 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/src/jsonrpc/responses.py
+-rw-rw-rw-   0 root         (0) root         (0)     2122 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/src/jsonrpc/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)     3533 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/src/jsonrpc/typedefs.py
+-rw-rw-rw-   0 root         (0) root         (0)     5583 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/src/jsonrpc/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 13:59:29.555700 jsonrpc_py-3.3.0/src/jsonrpc_py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2918 2024-05-30 13:59:29.000000 jsonrpc_py-3.3.0/src/jsonrpc_py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2831 2024-05-30 13:59:29.000000 jsonrpc_py-3.3.0/src/jsonrpc_py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 13:59:29.000000 jsonrpc_py-3.3.0/src/jsonrpc_py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-30 13:59:29.000000 jsonrpc_py-3.3.0/src/jsonrpc_py.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-30 13:59:29.000000 jsonrpc_py-3.3.0/src/jsonrpc_py.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 13:59:29.554700 jsonrpc_py-3.3.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13922 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/tests/test_asgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     3714 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/tests/test_dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     1928 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/tests/test_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     5152 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/tests/test_lifespan.py
+-rw-rw-rw-   0 root         (0) root         (0)     8215 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/tests/test_requests.py
+-rw-rw-rw-   0 root         (0) root         (0)     5833 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/tests/test_responses.py
+-rw-rw-rw-   0 root         (0) root         (0)     1200 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/tests/test_serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)     7087 2024-05-30 13:59:14.000000 jsonrpc_py-3.3.0/tests/test_utilities.py
```

### Comparing `jsonrpc-py-3.2.9/.gitlab-ci.yml` & `jsonrpc_py-3.3.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.2.9/LICENSE` & `jsonrpc_py-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.2.9/Makefile` & `jsonrpc_py-3.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.2.9/PKG-INFO` & `jsonrpc_py-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonrpc-py
-Version: 3.2.9
+Version: 3.3.0
 Summary: Pure zero-dependency JSON-RPC 2.0 implementation
 Author-email: Andrew Malchuk <andrew.malchuk@yandex.ru>
 Maintainer-email: JSON-RPC Development Group <dev@jsonrpc.ru>
 License: BSD-3-Clause
 Project-URL: Homepage, https://docs.jsonrpc.ru
 Project-URL: Source Code, https://gitlab.com/jsonrpc/jsonrpc-py
 Project-URL: Documentation, https://docs.jsonrpc.ru
```

### Comparing `jsonrpc-py-3.2.9/README.md` & `jsonrpc_py-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.2.9/docs/changelog/v1.x.x/v1.1.0.rst` & `jsonrpc_py-3.3.0/docs/changelog/v1.x.x/v1.1.0.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.2.9/docs/changelog/v2.x.x/v2.0.1.rst` & `jsonrpc_py-3.3.0/docs/changelog/v2.x.x/v2.0.1.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.2.9/docs/changelog/v2.x.x/v2.3.0.rst` & `jsonrpc_py-3.3.0/docs/changelog/v2.x.x/v2.3.0.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.2.9/docs/changelog/v3.x.x/v3.0.0.rst` & `jsonrpc_py-3.3.0/docs/changelog/v3.x.x/v3.0.0.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.2.9/docs/changelog.rst` & `jsonrpc_py-3.3.0/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.2.9/docs/conf.py` & `jsonrpc_py-3.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.2.9/docs/deployment.rst` & `jsonrpc_py-3.3.0/docs/deployment.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.2.9/docs/index.rst` & `jsonrpc_py-3.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.2.9/docs/quickstart.rst` & `jsonrpc_py-3.3.0/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.2.9/docs/reference.rst` & `jsonrpc_py-3.3.0/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.2.9/pyproject.toml` & `jsonrpc_py-3.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.2.9/src/jsonrpc/__init__.py` & `jsonrpc_py-3.3.0/src/jsonrpc/__init__.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.2.9/src/jsonrpc/asgi.py` & `jsonrpc_py-3.3.0/src/jsonrpc/asgi.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 
 from .dispatcher import AsyncDispatcher
 from .errors import Error
 from .lifespan import LifespanEvents, LifespanManager
 from .requests import BatchRequest, Request
 from .responses import BatchResponse, Response
 from .serializers import JSONSerializer
-from .utilities import BackgroundTask, CancellableGather
+from .utilities import CancellableGather, run_in_background
 
 if TYPE_CHECKING:
-    from collections.abc import Generator
+    from collections.abc import Coroutine, Generator
     from typing import Any, ClassVar, TypeAlias
 
     from .typedefs import ASGIReceiveCallable, ASGISendCallable, HTTPConnectionScope, Scope
 
 __all__: tuple[str, ...] = ("ASGIHandler",)
 
 KT = TypeVar("KT")
@@ -214,25 +214,24 @@
 
     @process_request.register
     async def _(self, obj: Error) -> Response:
         return Response(error=obj, response_id=None)
 
     @process_request.register
     async def _(self, obj: Request) -> Response | None:
-        background_task: BackgroundTask[Any] = BackgroundTask.from_coroutine(
-            self.app.dispatcher.dispatch(
-                obj.method,
-                *obj.args,
-                **obj.kwargs,
-            )
+        coroutine: Coroutine[Any, Any, Any] = self.app.dispatcher.dispatch(
+            obj.method,
+            *obj.args,
+            **obj.kwargs,
         )
         if obj.is_notification:
+            run_in_background(coroutine)
             return None
         try:
-            result: Any = await background_task
+            result: Any = await coroutine
             return Response(body=result, response_id=obj.request_id)
         except Error as error:
             return Response(error=error, response_id=obj.request_id)
 
     @process_request.register
     async def _(self, obj: BatchRequest) -> BatchResponse:
         responses: tuple[AnyResponse, ...] = await CancellableGather(map(self.process_request, obj))
```

### Comparing `jsonrpc-py-3.2.9/src/jsonrpc/dispatcher.py` & `jsonrpc_py-3.3.0/src/jsonrpc/dispatcher.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.2.9/src/jsonrpc/errors.py` & `jsonrpc_py-3.3.0/src/jsonrpc/errors.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.2.9/src/jsonrpc/lifespan.py` & `jsonrpc_py-3.3.0/src/jsonrpc/lifespan.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.2.9/src/jsonrpc/requests.py` & `jsonrpc_py-3.3.0/src/jsonrpc/requests.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.2.9/src/jsonrpc/responses.py` & `jsonrpc_py-3.3.0/src/jsonrpc/responses.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.2.9/src/jsonrpc/serializers.py` & `jsonrpc_py-3.3.0/src/jsonrpc/serializers.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.2.9/src/jsonrpc/typedefs.py` & `jsonrpc_py-3.3.0/src/jsonrpc/typedefs.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.2.9/src/jsonrpc/utilities.py` & `jsonrpc_py-3.3.0/src/jsonrpc/utilities.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,81 +1,40 @@
 from __future__ import annotations
 
-from asyncio import TaskGroup, get_running_loop, shield
+from asyncio import Runner, TaskGroup, get_event_loop_policy, get_running_loop
 from collections.abc import MutableMapping
 from contextvars import copy_context
 from dataclasses import dataclass, field
 from functools import partial, total_ordering
 from heapq import heappop, heappush
-from inspect import iscoroutinefunction
-from typing import TYPE_CHECKING, ClassVar, Generic, ParamSpec, TypeVar, final, overload
-from uuid import uuid4
+from inspect import iscoroutine, iscoroutinefunction
+from threading import Thread
+from typing import TYPE_CHECKING, Generic, ParamSpec, TypeVar, final, overload
 
 if TYPE_CHECKING:
-    from asyncio import AbstractEventLoop, Task
+    from asyncio import AbstractEventLoop, AbstractEventLoopPolicy, Task
     from collections.abc import Callable, Coroutine, Generator, Iterable, Iterator
     from contextvars import Context
-    from typing import Any, Final, Literal, Self, TypeGuard
-    from uuid import UUID
+    from typing import Any, Final, Literal, TypeGuard
 
 __all__: tuple[str, ...] = (
-    "BackgroundTask",
     "CancellableGather",
     "ensure_async",
     "is_iterable",
     "make_hashable",
     "PrioritizedItem",
+    "run_in_background",
     "Undefined",
     "UndefinedType",
 )
 
 T = TypeVar("T")
 P = ParamSpec("P")
 
 
-@dataclass(slots=True)
-class BackgroundTask(Generic[T]):
-    registry: ClassVar[set[object]] = set()
-    task: Task[T]
-    task_id: UUID = field(default_factory=uuid4, init=False)
-
-    def __hash__(self) -> int:
-        return hash((self.__class__, self.task_id))
-
-    def __await__(self) -> Generator[Any, None, T]:
-        #: ---
-        #: Create a suitable iterator by calling __await__ on a coroutine.
-        return self.__await_impl__().__await__()
-
-    async def __await_impl__(self) -> T:
-        #: ---
-        #: Wait for a task, shielding it from cancellation.
-        return await shield(self.task)
-
-    @classmethod
-    def from_coroutine(cls, coroutine: Coroutine[Any, Any, T], /) -> Self:
-        loop: AbstractEventLoop = get_running_loop()
-        task: Task[T] = loop.create_task(coroutine)
-        #: ---
-        #: Add a background task to the set. This creates a strong reference.
-        cls.registry.add(background_task := cls(task))
-        #: ---
-        #: To prevent keeping references to finished tasks forever,
-        #: make each task remove its own reference from the set after
-        #: completion:
-        task.add_done_callback(background_task.finish_callback)
-        return background_task
-
-    def finish_callback(self, task: Task[T]) -> bool:
-        self.registry.discard(self)
-        #: ---
-        #: Mark exception retrieved:
-        return task.cancelled() or task.exception() is None
-
-
 @total_ordering
 @dataclass(slots=True)
 class PrioritizedItem(Generic[T]):
     priority: int
     item: T
 
     def __eq__(self, obj: Any) -> bool:
@@ -177,14 +136,27 @@
         #: ---
         #: Non-hashable, non-iterable:
         raise
 
     return obj
 
 
+def run_in_background(coroutine: Coroutine[Any, Any, Any], *, context: Context | None = None) -> None:
+    if not iscoroutine(coroutine):
+        raise ValueError(f"a coroutine was expected, got {type(coroutine).__name__!r}")
+
+    policy: Final[AbstractEventLoopPolicy] = get_event_loop_policy()
+
+    def wrapper() -> None:
+        with Runner(loop_factory=policy.new_event_loop) as runner:
+            runner.run(coroutine, context=context)
+
+    return Thread(target=wrapper, daemon=True).start()
+
+
 @final
 class UndefinedType:
     __slots__: tuple[str, ...] = ()
 
     def __repr__(self) -> Literal["Undefined"]:
         return "Undefined"
```

### Comparing `jsonrpc-py-3.2.9/src/jsonrpc_py.egg-info/PKG-INFO` & `jsonrpc_py-3.3.0/src/jsonrpc_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonrpc-py
-Version: 3.2.9
+Version: 3.3.0
 Summary: Pure zero-dependency JSON-RPC 2.0 implementation
 Author-email: Andrew Malchuk <andrew.malchuk@yandex.ru>
 Maintainer-email: JSON-RPC Development Group <dev@jsonrpc.ru>
 License: BSD-3-Clause
 Project-URL: Homepage, https://docs.jsonrpc.ru
 Project-URL: Source Code, https://gitlab.com/jsonrpc/jsonrpc-py
 Project-URL: Documentation, https://docs.jsonrpc.ru
```

### Comparing `jsonrpc-py-3.2.9/src/jsonrpc_py.egg-info/SOURCES.txt` & `jsonrpc_py-3.3.0/src/jsonrpc_py.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 docs/changelog/v3.x.x/v3.2.3.rst
 docs/changelog/v3.x.x/v3.2.4.rst
 docs/changelog/v3.x.x/v3.2.5.rst
 docs/changelog/v3.x.x/v3.2.6.rst
 docs/changelog/v3.x.x/v3.2.7.rst
 docs/changelog/v3.x.x/v3.2.8.rst
 docs/changelog/v3.x.x/v3.2.9.rst
+docs/changelog/v3.x.x/v3.3.0.rst
 src/jsonrpc/__init__.py
 src/jsonrpc/asgi.py
 src/jsonrpc/dispatcher.py
 src/jsonrpc/errors.py
 src/jsonrpc/lifespan.py
 src/jsonrpc/py.typed
 src/jsonrpc/requests.py
```

### Comparing `jsonrpc-py-3.2.9/tests/test_asgi.py` & `jsonrpc_py-3.3.0/tests/test_asgi.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from collections.abc import MutableMapping
 from http import HTTPMethod, HTTPStatus
 from typing import TYPE_CHECKING
 from unittest import IsolatedAsyncioTestCase as AsyncioTestCase, TestCase
 from unittest.mock import AsyncMock
 from uuid import uuid4
 
-from httpx import AsyncClient
+from httpx import ASGITransport, AsyncClient
 
 from jsonrpc import ASGIHandler, ErrorEnum
 
 if TYPE_CHECKING:
     from typing import Any, Literal
     from uuid import UUID
 
@@ -54,15 +54,15 @@
     def random_id(self) -> str:
         uuid: UUID = uuid4()
         return str(uuid)
 
     def setUp(self) -> None:
         self.app: ASGIHandler = ASGIHandler()
         self.client: AsyncClient = AsyncClient(
-            app=self.app,
+            transport=ASGITransport(self.app),
             base_url="http://testserver",
             headers={"Content-Type": "application/json"},
         )
 
     async def asyncSetUp(self) -> None:
         await self.enterAsyncContext(self.client)
 
@@ -324,15 +324,15 @@
         loop, mock, event = get_running_loop(), AsyncMock(), Event()
 
         @self.app.dispatcher.register(function_name="mock")
         async def _(*args: Any, **kwargs: Any) -> None:
             try:
                 await mock(*args, **kwargs)
             finally:
-                loop.call_soon(event.set)
+                loop.call_soon_threadsafe(event.set)
 
         response: Response = await self.client.post("/", json={"jsonrpc": "2.0", "method": "mock", "params": [1, 2, 3]})
         await event.wait()
         self.assertEqual(response.status_code, HTTPStatus.NO_CONTENT)
         self.assertEqual(response.content, b"")
         mock.assert_awaited_once_with(1, 2, 3)
```

### Comparing `jsonrpc-py-3.2.9/tests/test_dispatcher.py` & `jsonrpc_py-3.3.0/tests/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.2.9/tests/test_errors.py` & `jsonrpc_py-3.3.0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.2.9/tests/test_lifespan.py` & `jsonrpc_py-3.3.0/tests/test_lifespan.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.2.9/tests/test_requests.py` & `jsonrpc_py-3.3.0/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.2.9/tests/test_responses.py` & `jsonrpc_py-3.3.0/tests/test_responses.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.2.9/tests/test_serializers.py` & `jsonrpc_py-3.3.0/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.2.9/tests/test_utilities.py` & `jsonrpc_py-3.3.0/tests/test_utilities.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,22 @@
 from __future__ import annotations
 
-import gc
-from asyncio import create_task, sleep, wait_for
+from asyncio import Event, create_task, get_running_loop, sleep, wait_for
 from dataclasses import is_dataclass
+from types import NoneType
 from typing import TYPE_CHECKING
 from unittest import IsolatedAsyncioTestCase as AsyncioTestCase, TestCase
 from unittest.mock import AsyncMock, MagicMock, sentinel
 
-from jsonrpc.utilities import BackgroundTask, CancellableGather, PrioritizedItem, Undefined, UndefinedType, ensure_async, make_hashable
+from jsonrpc.utilities import CancellableGather, PrioritizedItem, Undefined, UndefinedType, ensure_async, make_hashable, run_in_background
 
 if TYPE_CHECKING:
     from typing import Any, Literal, NoReturn
 
 
-class TestBackgroundTask(AsyncioTestCase):
-    async def test_from_coroutine(self) -> None:
-        mock: AsyncMock = AsyncMock(return_value="for testing purposes")
-        background_task: BackgroundTask[str] = BackgroundTask.from_coroutine(mock(1, 2, 3, key="value"))
-
-        self.assertEqual(hash(background_task), hash((BackgroundTask, background_task.task_id)))
-        self.assertTrue(background_task.registry)
-        self.assertIn(background_task, background_task.registry)
-
-        result: str = await background_task
-        self.assertEqual(result, "for testing purposes")
-        self.assertFalse(background_task.registry)
-        self.assertNotIn(background_task, background_task.registry)
-
-    async def test_with_gc_collect(self) -> None:
-        async def eternity() -> None:
-            await sleep(3600.0)
-
-        BackgroundTask.from_coroutine(eternity())
-        self.assertTrue(BackgroundTask.registry)
-
-        gc.collect()
-        gc.collect()
-        gc.collect()
-
-        del eternity
-        self.assertTrue(BackgroundTask.registry)
-
-    def tearDown(self) -> None:
-        BackgroundTask.registry.clear()
-
-
 class TestCancellableGather(AsyncioTestCase):
     def test_prioritized_item(self) -> None:
         self.assertTrue(is_dataclass(prioritized_item := PrioritizedItem(0, "for testing purposes")))
         self.assertEqual(prioritized_item, PrioritizedItem(0, b"for testing purposes"))
         self.assertNotEqual(prioritized_item, PrioritizedItem(123, "for testing purposes"))
         self.assertLess(prioritized_item, PrioritizedItem(1, "the other one"))
         self.assertNotEqual(prioritized_item, "for testing purposes")
@@ -145,14 +113,34 @@
             AsyncMock(return_value=sentinel.async_def),
         ):
             with self.subTest(mock=mock):
                 result: Any = await ensure_async(mock, 1, 2, 3, key="value")
                 self.assertIs(result, mock.return_value)
                 mock.assert_called_once_with(1, 2, 3, key="value")
 
+    def test_run_in_background_exception(self) -> None:
+        with self.assertRaises(ValueError) as context:
+            run_in_background(None)
+
+        self.assertEqual(str(context.exception), f"a coroutine was expected, got {NoneType.__name__!r}")
+
+    async def test_run_in_background(self) -> None:
+        loop, mock, event = get_running_loop(), AsyncMock(), Event()
+
+        async def background_task() -> None:
+            try:
+                await mock()
+            finally:
+                loop.call_soon_threadsafe(event.set)
+
+        run_in_background(background_task())
+
+        await event.wait()
+        mock.assert_awaited_once()
+
 
 class TestHashable(TestCase):
     def test_equality(self) -> None:
         tests: tuple[tuple[Any, Any], ...] = (
             ([], ()),
             (["a", 1], ("a", 1)),
             ({}, ()),
```

