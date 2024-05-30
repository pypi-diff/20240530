# Comparing `tmp/fedfind-5.2.0.tar.gz` & `tmp/fedfind-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedfind-5.2.0.tar", last modified: Thu May 16 21:19:56 2024, max compression
+gzip compressed data, was "fedfind-5.3.0.tar", last modified: Thu May 30 19:48:52 2024, max compression
```

## Comparing `fedfind-5.2.0.tar` & `fedfind-5.3.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-05-16 21:19:56.833216 fedfind-5.2.0/
--rw-rw-r--   0 adamw     (1000) adamw     (1000)       86 2019-06-18 21:22:51.000000 fedfind-5.2.0/.gitignore
--rw-rw-r--   0 adamw     (1000) adamw     (1000)       29 2019-06-18 21:22:51.000000 fedfind-5.2.0/.pylintrc
--rw-r--r--   0 adamw     (1000) adamw     (1000)      143 2023-10-19 16:24:10.000000 fedfind-5.2.0/.zuul.yaml
--rw-r--r--   0 adamw     (1000) adamw     (1000)    40810 2024-05-16 21:18:41.000000 fedfind-5.2.0/CHANGELOG.md
--rw-rw-r--   0 adamw     (1000) adamw     (1000)    35147 2015-02-09 17:48:14.000000 fedfind-5.2.0/COPYING
--rw-rw-r--   0 adamw     (1000) adamw     (1000)       37 2019-06-18 21:22:51.000000 fedfind-5.2.0/MANIFEST.in
--rw-r--r--   0 adamw     (1000) adamw     (1000)    27819 2024-05-16 21:19:56.832216 fedfind-5.2.0/PKG-INFO
--rw-r--r--   0 adamw     (1000) adamw     (1000)    27184 2023-10-19 16:24:10.000000 fedfind-5.2.0/README.md
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-05-16 21:19:56.829216 fedfind-5.2.0/ci/
--rw-r--r--   0 adamw     (1000) adamw     (1000)      397 2023-10-19 16:24:10.000000 fedfind-5.2.0/ci/tox.yaml
--rwxr-xr-x   0 adamw     (1000) adamw     (1000)      251 2023-10-19 16:24:10.000000 fedfind-5.2.0/fedfindlocal.py
--rwxr-xr-x   0 adamw     (1000) adamw     (1000)     3811 2024-04-23 22:13:33.000000 fedfind-5.2.0/gen-allstable
--rw-r--r--   0 adamw     (1000) adamw     (1000)       62 2023-10-19 16:24:10.000000 fedfind-5.2.0/install.requires
--rw-r--r--   0 adamw     (1000) adamw     (1000)      334 2023-10-19 16:24:10.000000 fedfind-5.2.0/pyproject.toml
--rwxr-xr-x   0 adamw     (1000) adamw     (1000)      658 2023-10-19 16:24:10.000000 fedfind-5.2.0/release.sh
--rw-r--r--   0 adamw     (1000) adamw     (1000)       38 2024-05-16 21:19:56.833216 fedfind-5.2.0/setup.cfg
--rw-r--r--   0 adamw     (1000) adamw     (1000)     1899 2024-05-16 21:19:34.000000 fedfind-5.2.0/setup.py
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-05-16 21:19:56.828216 fedfind-5.2.0/src/
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-05-16 21:19:56.829216 fedfind-5.2.0/src/fedfind/
--rw-r--r--   0 adamw     (1000) adamw     (1000)      934 2024-05-16 21:19:34.000000 fedfind-5.2.0/src/fedfind/__init__.py
--rwxr-xr-x   0 adamw     (1000) adamw     (1000)    10798 2024-05-16 20:33:22.000000 fedfind-5.2.0/src/fedfind/cli.py
--rw-r--r--   0 adamw     (1000) adamw     (1000)     7151 2024-04-23 21:43:29.000000 fedfind-5.2.0/src/fedfind/const.py
--rw-r--r--   0 adamw     (1000) adamw     (1000)     2502 2023-10-19 16:24:10.000000 fedfind-5.2.0/src/fedfind/exceptions.py
--rw-r--r--   0 adamw     (1000) adamw     (1000)    32015 2024-05-15 17:51:07.000000 fedfind-5.2.0/src/fedfind/helpers.py
--rw-r--r--   0 adamw     (1000) adamw     (1000)   100735 2024-05-16 21:10:04.000000 fedfind-5.2.0/src/fedfind/release.py
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-05-16 21:19:56.832216 fedfind-5.2.0/src/fedfind.egg-info/
--rw-r--r--   0 adamw     (1000) adamw     (1000)    27819 2024-05-16 21:19:56.000000 fedfind-5.2.0/src/fedfind.egg-info/PKG-INFO
--rw-rw-r--   0 adamw     (1000) adamw     (1000)     1715 2024-05-16 21:19:56.000000 fedfind-5.2.0/src/fedfind.egg-info/SOURCES.txt
--rw-rw-r--   0 adamw     (1000) adamw     (1000)        1 2024-05-16 21:19:56.000000 fedfind-5.2.0/src/fedfind.egg-info/dependency_links.txt
--rw-rw-r--   0 adamw     (1000) adamw     (1000)       45 2024-05-16 21:19:56.000000 fedfind-5.2.0/src/fedfind.egg-info/entry_points.txt
--rw-rw-r--   0 adamw     (1000) adamw     (1000)       68 2024-05-16 21:19:56.000000 fedfind-5.2.0/src/fedfind.egg-info/requires.txt
--rw-rw-r--   0 adamw     (1000) adamw     (1000)        8 2024-05-16 21:19:56.000000 fedfind-5.2.0/src/fedfind.egg-info/top_level.txt
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-05-16 21:19:56.830216 fedfind-5.2.0/tests/
--rw-r--r--   0 adamw     (1000) adamw     (1000)     7601 2024-05-15 18:18:27.000000 fedfind-5.2.0/tests/conftest.py
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-05-16 21:19:56.832216 fedfind-5.2.0/tests/data/
--rw-r--r--   0 adamw     (1000) adamw     (1000)  1035277 2024-04-23 21:30:59.000000 fedfind-5.2.0/tests/data/allstable.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)   293981 2024-04-23 22:34:02.000000 fedfind-5.2.0/tests/data/compose-urls-20240423.json
--rwxr-xr-x   0 adamw     (1000) adamw     (1000)     1437 2023-10-19 16:24:10.000000 fedfind-5.2.0/tests/data/fedfindloc.py
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-05-16 21:19:56.828216 fedfind-5.2.0/tests/data/http/
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-05-16 21:19:56.828216 fedfind-5.2.0/tests/data/http/pub/
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-05-16 21:19:56.832216 fedfind-5.2.0/tests/data/http/pub/alt/
--rw-r--r--   0 adamw     (1000) adamw     (1000)   215056 2024-05-16 21:15:20.000000 fedfind-5.2.0/tests/data/http/pub/alt/imagelist-alt
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-05-16 21:19:56.832216 fedfind-5.2.0/tests/data/http/pub/archive/
--rw-r--r--   0 adamw     (1000) adamw     (1000)   146475 2024-05-16 21:15:21.000000 fedfind-5.2.0/tests/data/http/pub/archive/imagelist-archive
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-05-16 21:19:56.832216 fedfind-5.2.0/tests/data/http/pub/fedora/
--rw-r--r--   0 adamw     (1000) adamw     (1000)    33469 2024-05-16 21:15:20.000000 fedfind-5.2.0/tests/data/http/pub/fedora/imagelist-fedora
--rw-rw-r--   0 adamw     (1000) adamw     (1000)    38788 2019-06-18 21:22:51.000000 fedfind-5.2.0/tests/data/pdc-compimages-Fedora-24-20160614.0.json
--rw-rw-r--   0 adamw     (1000) adamw     (1000)    43446 2019-06-18 21:22:51.000000 fedfind-5.2.0/tests/data/pdc-compimages-Fedora-25-20161115.0.json
--rw-rw-r--   0 adamw     (1000) adamw     (1000)    73734 2019-06-18 21:22:51.000000 fedfind-5.2.0/tests/data/pdc-compimages-Fedora-26-20170705.0.json
--rw-rw-r--   0 adamw     (1000) adamw     (1000)    70323 2019-06-18 21:22:51.000000 fedfind-5.2.0/tests/data/pdc-compimages-Fedora-27-20171105.0.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)    81069 2023-10-19 16:24:10.000000 fedfind-5.2.0/tests/data/pdc-compimages-Fedora-28-20180425.0.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)    59560 2023-10-19 16:24:10.000000 fedfind-5.2.0/tests/data/pdc-compimages-Fedora-29-20181024.1.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)    61551 2023-10-19 16:24:10.000000 fedfind-5.2.0/tests/data/pdc-compimages-Fedora-30-20190425.0.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)    57550 2023-10-19 16:24:10.000000 fedfind-5.2.0/tests/data/pdc-compimages-Fedora-31-20191023.0.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)    59948 2023-10-19 16:24:10.000000 fedfind-5.2.0/tests/data/pdc-compimages-Fedora-32-20200422.0.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)    65722 2023-10-19 16:24:10.000000 fedfind-5.2.0/tests/data/pdc-compimages-Fedora-33-20201019.0.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)    63265 2023-10-19 16:24:10.000000 fedfind-5.2.0/tests/data/pdc-compimages-Fedora-34-20210423.0.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)    66775 2023-10-19 16:24:10.000000 fedfind-5.2.0/tests/data/pdc-compimages-Fedora-35-20211026.0.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)    65980 2023-10-19 16:24:10.000000 fedfind-5.2.0/tests/data/pdc-compimages-Fedora-36-20220504.1.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)    27726 2023-10-19 16:24:10.000000 fedfind-5.2.0/tests/data/pdc-compimages-Fedora-37-20221105.0.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)    29444 2023-10-19 16:24:10.000000 fedfind-5.2.0/tests/data/pdc-compimages-Fedora-38-20230413.1.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)    64647 2024-04-23 22:28:11.000000 fedfind-5.2.0/tests/data/pdc-compimages-Fedora-39-20231031.1.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)    70999 2024-04-23 22:26:25.000000 fedfind-5.2.0/tests/data/pdc-compimages-Fedora-40-20240414.0.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)    29635 2023-10-19 16:24:10.000000 fedfind-5.2.0/tests/test_helpers.py
--rw-r--r--   0 adamw     (1000) adamw     (1000)    56539 2024-05-16 21:14:46.000000 fedfind-5.2.0/tests/test_release.py
--rw-r--r--   0 adamw     (1000) adamw     (1000)       58 2023-10-19 16:24:10.000000 fedfind-5.2.0/tests.requires
--rw-r--r--   0 adamw     (1000) adamw     (1000)      549 2023-10-19 16:24:10.000000 fedfind-5.2.0/tox.ini
--rw-r--r--   0 adamw     (1000) adamw     (1000)       39 2023-10-19 16:24:10.000000 fedfind-5.2.0/tox.requires
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-05-30 19:48:52.507849 fedfind-5.3.0/
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)       86 2019-06-18 21:22:51.000000 fedfind-5.3.0/.gitignore
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)       29 2019-06-18 21:22:51.000000 fedfind-5.3.0/.pylintrc
+-rw-r--r--   0 adamw     (1000) adamw     (1000)      143 2023-10-19 16:24:10.000000 fedfind-5.3.0/.zuul.yaml
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    41338 2024-05-30 19:47:44.000000 fedfind-5.3.0/CHANGELOG.md
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)    35147 2015-02-09 17:48:14.000000 fedfind-5.3.0/COPYING
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)       37 2019-06-18 21:22:51.000000 fedfind-5.3.0/MANIFEST.in
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    28231 2024-05-30 19:48:52.506849 fedfind-5.3.0/PKG-INFO
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    27596 2024-05-30 19:35:59.000000 fedfind-5.3.0/README.md
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-05-30 19:48:52.503849 fedfind-5.3.0/ci/
+-rw-r--r--   0 adamw     (1000) adamw     (1000)      397 2023-10-19 16:24:10.000000 fedfind-5.3.0/ci/tox.yaml
+-rwxr-xr-x   0 adamw     (1000) adamw     (1000)      251 2023-10-19 16:24:10.000000 fedfind-5.3.0/fedfindlocal.py
+-rwxr-xr-x   0 adamw     (1000) adamw     (1000)     3811 2024-04-23 22:13:33.000000 fedfind-5.3.0/gen-allstable
+-rw-r--r--   0 adamw     (1000) adamw     (1000)       62 2023-10-19 16:24:10.000000 fedfind-5.3.0/install.requires
+-rw-r--r--   0 adamw     (1000) adamw     (1000)      334 2023-10-19 16:24:10.000000 fedfind-5.3.0/pyproject.toml
+-rwxr-xr-x   0 adamw     (1000) adamw     (1000)      658 2023-10-19 16:24:10.000000 fedfind-5.3.0/release.sh
+-rw-r--r--   0 adamw     (1000) adamw     (1000)       38 2024-05-30 19:48:52.507849 fedfind-5.3.0/setup.cfg
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     1899 2024-05-30 19:48:35.000000 fedfind-5.3.0/setup.py
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-05-30 19:48:52.502849 fedfind-5.3.0/src/
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-05-30 19:48:52.504849 fedfind-5.3.0/src/fedfind/
+-rw-r--r--   0 adamw     (1000) adamw     (1000)      934 2024-05-30 19:48:35.000000 fedfind-5.3.0/src/fedfind/__init__.py
+-rwxr-xr-x   0 adamw     (1000) adamw     (1000)    10798 2024-05-16 20:33:22.000000 fedfind-5.3.0/src/fedfind/cli.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     7151 2024-04-23 21:43:29.000000 fedfind-5.3.0/src/fedfind/const.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     2502 2023-10-19 16:24:10.000000 fedfind-5.3.0/src/fedfind/exceptions.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    32783 2024-05-30 19:35:05.000000 fedfind-5.3.0/src/fedfind/helpers.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)   100735 2024-05-29 23:07:08.000000 fedfind-5.3.0/src/fedfind/release.py
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-05-30 19:48:52.506849 fedfind-5.3.0/src/fedfind.egg-info/
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    28231 2024-05-30 19:48:52.000000 fedfind-5.3.0/src/fedfind.egg-info/PKG-INFO
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)     1715 2024-05-30 19:48:52.000000 fedfind-5.3.0/src/fedfind.egg-info/SOURCES.txt
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)        1 2024-05-30 19:48:52.000000 fedfind-5.3.0/src/fedfind.egg-info/dependency_links.txt
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)       45 2024-05-30 19:48:52.000000 fedfind-5.3.0/src/fedfind.egg-info/entry_points.txt
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)       68 2024-05-30 19:48:52.000000 fedfind-5.3.0/src/fedfind.egg-info/requires.txt
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)        8 2024-05-30 19:48:52.000000 fedfind-5.3.0/src/fedfind.egg-info/top_level.txt
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-05-30 19:48:52.504849 fedfind-5.3.0/tests/
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     7601 2024-05-15 18:18:27.000000 fedfind-5.3.0/tests/conftest.py
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-05-30 19:48:52.506849 fedfind-5.3.0/tests/data/
+-rw-r--r--   0 adamw     (1000) adamw     (1000)  1035277 2024-04-23 21:30:59.000000 fedfind-5.3.0/tests/data/allstable.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)   293981 2024-04-23 22:34:02.000000 fedfind-5.3.0/tests/data/compose-urls-20240423.json
+-rwxr-xr-x   0 adamw     (1000) adamw     (1000)     1437 2023-10-19 16:24:10.000000 fedfind-5.3.0/tests/data/fedfindloc.py
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-05-30 19:48:52.502849 fedfind-5.3.0/tests/data/http/
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-05-30 19:48:52.502849 fedfind-5.3.0/tests/data/http/pub/
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-05-30 19:48:52.506849 fedfind-5.3.0/tests/data/http/pub/alt/
+-rw-r--r--   0 adamw     (1000) adamw     (1000)   215056 2024-05-30 19:42:01.000000 fedfind-5.3.0/tests/data/http/pub/alt/imagelist-alt
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-05-30 19:48:52.506849 fedfind-5.3.0/tests/data/http/pub/archive/
+-rw-r--r--   0 adamw     (1000) adamw     (1000)   146475 2024-05-30 19:42:01.000000 fedfind-5.3.0/tests/data/http/pub/archive/imagelist-archive
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2024-05-30 19:48:52.506849 fedfind-5.3.0/tests/data/http/pub/fedora/
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    33469 2024-05-30 19:42:01.000000 fedfind-5.3.0/tests/data/http/pub/fedora/imagelist-fedora
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)    38788 2019-06-18 21:22:51.000000 fedfind-5.3.0/tests/data/pdc-compimages-Fedora-24-20160614.0.json
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)    43446 2019-06-18 21:22:51.000000 fedfind-5.3.0/tests/data/pdc-compimages-Fedora-25-20161115.0.json
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)    73734 2019-06-18 21:22:51.000000 fedfind-5.3.0/tests/data/pdc-compimages-Fedora-26-20170705.0.json
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)    70323 2019-06-18 21:22:51.000000 fedfind-5.3.0/tests/data/pdc-compimages-Fedora-27-20171105.0.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    81069 2023-10-19 16:24:10.000000 fedfind-5.3.0/tests/data/pdc-compimages-Fedora-28-20180425.0.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    59560 2023-10-19 16:24:10.000000 fedfind-5.3.0/tests/data/pdc-compimages-Fedora-29-20181024.1.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    61551 2023-10-19 16:24:10.000000 fedfind-5.3.0/tests/data/pdc-compimages-Fedora-30-20190425.0.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    57550 2023-10-19 16:24:10.000000 fedfind-5.3.0/tests/data/pdc-compimages-Fedora-31-20191023.0.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    59948 2023-10-19 16:24:10.000000 fedfind-5.3.0/tests/data/pdc-compimages-Fedora-32-20200422.0.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    65722 2023-10-19 16:24:10.000000 fedfind-5.3.0/tests/data/pdc-compimages-Fedora-33-20201019.0.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    63265 2023-10-19 16:24:10.000000 fedfind-5.3.0/tests/data/pdc-compimages-Fedora-34-20210423.0.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    66775 2023-10-19 16:24:10.000000 fedfind-5.3.0/tests/data/pdc-compimages-Fedora-35-20211026.0.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    65980 2023-10-19 16:24:10.000000 fedfind-5.3.0/tests/data/pdc-compimages-Fedora-36-20220504.1.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    27726 2023-10-19 16:24:10.000000 fedfind-5.3.0/tests/data/pdc-compimages-Fedora-37-20221105.0.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    29444 2023-10-19 16:24:10.000000 fedfind-5.3.0/tests/data/pdc-compimages-Fedora-38-20230413.1.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    64647 2024-04-23 22:28:11.000000 fedfind-5.3.0/tests/data/pdc-compimages-Fedora-39-20231031.1.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    70999 2024-04-23 22:26:25.000000 fedfind-5.3.0/tests/data/pdc-compimages-Fedora-40-20240414.0.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    31348 2024-05-30 19:40:43.000000 fedfind-5.3.0/tests/test_helpers.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    56539 2024-05-16 21:14:46.000000 fedfind-5.3.0/tests/test_release.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)       58 2023-10-19 16:24:10.000000 fedfind-5.3.0/tests.requires
+-rw-r--r--   0 adamw     (1000) adamw     (1000)      549 2023-10-19 16:24:10.000000 fedfind-5.3.0/tox.ini
+-rw-r--r--   0 adamw     (1000) adamw     (1000)       39 2023-10-19 16:24:10.000000 fedfind-5.3.0/tox.requires
```

### Comparing `fedfind-5.2.0/CHANGELOG.md` & `fedfind-5.3.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,20 @@
 ## Changelog
 
+### 5.3.0 - 2024-05-30
+
+*   [fedfind-5.3.0.tar.gz](https://files.pythonhosted.org/packages/source/f/fedfind/fedfind-5.3.0.tar.gz)
+
+1.  **NEW**: honor `FEDFIND_NO_CACHE` environment variable to disable persistent caching
+
+Setting this variable disables the caching of PDC query responses and dl.fp.o file lists. This
+can interfere with test suites that use something like pyvcr to "record" and "replay" remote
+transactions, if a required PDC response or file list is cached on the system of the user
+generating the "recording".
+
 ### 5.2.0 - 2024-05-16
 
 *   [fedfind-5.2.0.tar.gz](https://files.pythonhosted.org/packages/source/f/fedfind/fedfind-5.2.0.tar.gz)
 
 1.  **NEW**: add `relnum` property to `Release` instances, representing the release number
 2.  **NEW**: add `eol` property to `Release` instances, indicating EOL date
 3.  **NEW**: re-introduce ``Updates`` and ``UpdatesTesting`` classes and support
```

### Comparing `fedfind-5.2.0/COPYING` & `fedfind-5.3.0/COPYING`

 * *Files identical despite different names*

### Comparing `fedfind-5.2.0/PKG-INFO` & `fedfind-5.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedfind
-Version: 5.2.0
+Version: 5.3.0
 Summary: Fedora Finder finds Fedora - images, more to come?
 Home-page: https://pagure.io/fedora-qa/fedfind
 Author: Adam Williamson
 Author-email: awilliam@redhat.com
 License: GPLv3+
 Keywords: fedora release image media iso
 Classifier: Development Status :: 5 - Production/Stable
@@ -186,14 +186,16 @@
 
 When used as a module it caches properties and image lists for the lifetime of the release instance. The image list files are cached (in `~/.cache/fedfind`) based on the 'last modified time' provided by the server they come from: for each new release instance, fedfind will hit the server to retrieve the last modified time header, but if the cached copy matches that time, it will not re-download the file. These files are also quite small so will not take long to download in any case. If the download fails for some reason, but we do have a cached copy of the necessary lists, fedfind will work but log a warning that it's using cached data which may be outdated.
 
 Certain PDC queries, whose results are never expected to change, are also cached (again in `~/.cache/fedfind`), to speed up repeated searches and reduce load on PDC.
 
 If `~/.cache/fedfind` is not writeable for the user running fedfind, we fall back to using a temporary cache location that is only valid for the life of the process (and deleted on exit). This at least ensures fedfind will work in this case, but results in it being slower and doing more round trips.
 
+You can set the environment variable `FEDFIND_NO_CACHE` to any value to disable this caching. File lists will still be written to `~/.cache/fedfind`, but the cached copy will never be used, the list will be re-downloaded each time it is requested. PDC queries will not be cached at all. This is intended for downstream projects whose test suites are affected by the caching (specifically, one that uses pyvcr).
+
 It shouldn't use too much bandwidth (though I haven't really measured), but obviously the server admins won't be happy with me if the servers get inundated with fedfind requests, so don't go *completely* crazy with it - if you want to do something script-y, please at least use the module and re-use release instances so the queries get cached.
 
 ### Can't find what ain't there
 
 All releases other than stable releases disappear. fedfind can find stable releases all the way back to Fedora Core 1, but it is not going to find Fedora 14 Alpha, Fedora 19 Beta TC3, or nightlies from more than 2-3 weeks ago. This isn't a bug in fedfind - those images literally are not publicly available any more. Nightlies only stick around for a few weeks, candidate composes for a given milestone usually disappear once we've moved on another couple of milestones, and pre-releases (Alphas and Betas) usually disappear some time after the release in question goes stable. fedfind will only find what's actually there.
 
 Also note that fedfind is not designed to find even *notional* locations for old non-stable releases. Due to their ephemeral nature, the patterns it uses for nightly builds and candidate composes only reflect current practice, and will simply be updated any time that practice changes. It doesn't have a big store of knowledge of what exact naming conventions we used for old composes. If you do `comp = fedfind.release.Compose(12, 'Final', 'TC4')` and read out `comp.location` or something what you get is almost certainly *not* the location where Fedora 12 Final TC4 actually lived when it was around.
```

### Comparing `fedfind-5.2.0/README.md` & `fedfind-5.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -167,14 +167,16 @@
 
 When used as a module it caches properties and image lists for the lifetime of the release instance. The image list files are cached (in `~/.cache/fedfind`) based on the 'last modified time' provided by the server they come from: for each new release instance, fedfind will hit the server to retrieve the last modified time header, but if the cached copy matches that time, it will not re-download the file. These files are also quite small so will not take long to download in any case. If the download fails for some reason, but we do have a cached copy of the necessary lists, fedfind will work but log a warning that it's using cached data which may be outdated.
 
 Certain PDC queries, whose results are never expected to change, are also cached (again in `~/.cache/fedfind`), to speed up repeated searches and reduce load on PDC.
 
 If `~/.cache/fedfind` is not writeable for the user running fedfind, we fall back to using a temporary cache location that is only valid for the life of the process (and deleted on exit). This at least ensures fedfind will work in this case, but results in it being slower and doing more round trips.
 
+You can set the environment variable `FEDFIND_NO_CACHE` to any value to disable this caching. File lists will still be written to `~/.cache/fedfind`, but the cached copy will never be used, the list will be re-downloaded each time it is requested. PDC queries will not be cached at all. This is intended for downstream projects whose test suites are affected by the caching (specifically, one that uses pyvcr).
+
 It shouldn't use too much bandwidth (though I haven't really measured), but obviously the server admins won't be happy with me if the servers get inundated with fedfind requests, so don't go *completely* crazy with it - if you want to do something script-y, please at least use the module and re-use release instances so the queries get cached.
 
 ### Can't find what ain't there
 
 All releases other than stable releases disappear. fedfind can find stable releases all the way back to Fedora Core 1, but it is not going to find Fedora 14 Alpha, Fedora 19 Beta TC3, or nightlies from more than 2-3 weeks ago. This isn't a bug in fedfind - those images literally are not publicly available any more. Nightlies only stick around for a few weeks, candidate composes for a given milestone usually disappear once we've moved on another couple of milestones, and pre-releases (Alphas and Betas) usually disappear some time after the release in question goes stable. fedfind will only find what's actually there.
 
 Also note that fedfind is not designed to find even *notional* locations for old non-stable releases. Due to their ephemeral nature, the patterns it uses for nightly builds and candidate composes only reflect current practice, and will simply be updated any time that practice changes. It doesn't have a big store of knowledge of what exact naming conventions we used for old composes. If you do `comp = fedfind.release.Compose(12, 'Final', 'TC4')` and read out `comp.location` or something what you get is almost certainly *not* the location where Fedora 12 Final TC4 actually lived when it was around.
```

### Comparing `fedfind-5.2.0/gen-allstable` & `fedfind-5.3.0/gen-allstable`

 * *Files identical despite different names*

### Comparing `fedfind-5.2.0/release.sh` & `fedfind-5.3.0/release.sh`

 * *Files identical despite different names*

### Comparing `fedfind-5.2.0/setup.py` & `fedfind-5.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         LONGDESC = f.read()
 except TypeError:
     with open(path.join(HERE, 'README.md')) as f:
         LONGDESC = f.read()
 
 setup(
     name="fedfind",
-    version="5.2.0",
+    version="5.3.0",
     entry_points={'console_scripts': ['fedfind = fedfind.cli:main'],},
     author="Adam Williamson",
     author_email="awilliam@redhat.com",
     description="Fedora Finder finds Fedora - images, more to come?",
     license="GPLv3+",
     keywords="fedora release image media iso",
     url="https://pagure.io/fedora-qa/fedfind",
```

### Comparing `fedfind-5.2.0/src/fedfind/__init__.py` & `fedfind-5.3.0/src/fedfind/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,10 +18,10 @@
 """Library and CLI tool for locating and getting information about
 Fedora composes.
 """
 
 from __future__ import unicode_literals
 from __future__ import print_function
 
-__version__ = "5.2.0"
+__version__ = "5.3.0"
 
 # vim: set textwidth=100 ts=8 et sw=4:
```

### Comparing `fedfind-5.2.0/src/fedfind/cli.py` & `fedfind-5.3.0/src/fedfind/cli.py`

 * *Files identical despite different names*

### Comparing `fedfind-5.2.0/src/fedfind/const.py` & `fedfind-5.3.0/src/fedfind/const.py`

 * *Files identical despite different names*

### Comparing `fedfind-5.2.0/src/fedfind/exceptions.py` & `fedfind-5.3.0/src/fedfind/exceptions.py`

 * *Files identical despite different names*

### Comparing `fedfind-5.2.0/src/fedfind/helpers.py` & `fedfind-5.3.0/src/fedfind/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 
 """Miscellaneous small functions that don't need to be class methods."""
 
 from __future__ import unicode_literals
 from __future__ import print_function
 
 import atexit
-import codecs
 import copy
 import datetime
+import io
 import json
 import logging
 import os
 import re
 import shutil
 import tempfile
 import time
@@ -362,48 +362,55 @@
 def pdc_query(path, params=None):
     # pylint:disable=too-many-locals,too-many-statements
     """Light 'API client', sorta, for PDC. Just handles sending a
     request to a given API path with the appropriate header to get
     a JSON response, parsing the response, and handling multi-page
     responses. params is a dict of query params. Caches certain
     responses which are very unlikely ever to change in fedfind's
-    cache directory.
+    cache directory, unless a magic file that tells it not to do
+    this exists (this is for the convenience of downstream test
+    suites which are thrown off by the caching).
     """
     logger.debug("pdc_query: path is %s", path)
-    # load the query cache
-    cachefile = os.path.join(CACHEDIR, "pdcquery.json")
-    try:
-        with codecs.open(cachefile, "r", encoding="utf-8") as cachefh:
-            cache = json.loads(cachefh.read())
-    except (IOError, OSError):
-        # file doesn't exist, etc.
-        cache = {}
+    usecache = True
+    if os.environ.get("FEDFIND_NO_CACHE"):
+        usecache = False
+    if usecache:
+        # load the query cache
+        cachefile = os.path.join(CACHEDIR, "pdcquery.json")
+        try:
+            with io.open(cachefile, "r", encoding="utf-8") as cachefh:
+                cache = json.loads(cachefh.read())
+        except (IOError, OSError):
+            # file doesn't exist, etc.
+            cache = {}
 
     # handle params (as we use them in the cache key)
     if not params:
         params = []
     # turn param dict into tuple list (we need to handle both dicts
     # and tuple lists, and you can't always turn a tuple list into a
     # dict because parameter names can be repeated)
     try:
         params = list(params.items())
     except AttributeError:
         pass
     baseurl = "/".join((fedfind.const.PDC_API, path.strip("/"))) + "/"
     logger.debug("pdc_query: baseurl is: %s", baseurl)
-    # cache key is the URL of the query, but without the page param
-    cachekey = "?".join((baseurl, urlencode(params)))
+    if usecache:
+        # cache key is the URL of the query, but without the page param
+        cachekey = "?".join((baseurl, urlencode(params)))
 
-    # check cache, return if hit
-    try:
-        ret = cache[cachekey]
-        logger.debug("pdc_query: cache hit!")
-        return ret
-    except KeyError:
-        pass
+        # check cache, return if hit
+        try:
+            ret = cache[cachekey]
+            logger.debug("pdc_query: cache hit!")
+            return ret
+        except KeyError:
+            pass
 
     # otherwise, actually do the query
     results = []
     # we figured out the params earlier, for the cache key, just add
     # 'page' and re-do the URL
     pgcnt = 1
     params.append(("page", str(pgcnt)))
@@ -428,35 +435,35 @@
             break
 
     # decide whether to cache results
     writecache = False
     # we always cache compose-images results, as if we get a result
     # it's a 'hit' and will never change (query for non-existent
     # compose gives a 404)
-    if path.startswith("compose-images/"):
+    if path.startswith("compose-images/") and usecache:
         logger.debug("pdc_query: caching result for %s", path)
         cache[cachekey] = results
         writecache = True
     # we cache 'composes' results if they're specific and we got a
     # result
-    if path == "composes" and results:
+    if path == "composes" and results and usecache:
         parkeys = [param[0] for param in params]
         if "compose_id" in parkeys or all(key in parkeys for key in ("release", "compose_label")):
             logger.debug("pdc_query: caching 'composes' result")
             cache[cachekey] = results
             writecache = True
 
     # write cache if we decided to
-    if writecache:
+    if writecache and usecache:
         # I've seen CACHEDIR suddenly vanish, when it's a temp dir; let's
         # check and re-create it if necessary
         if not os.path.exists(CACHEDIR):
             os.makedirs(CACHEDIR)
 
-        with codecs.open(cachefile, "w", encoding="utf-8") as cachefh:
+        with io.open(cachefile, "w", encoding="utf-8") as cachefh:
             cachefh.write(json.dumps(cache, separators=(",", ":"), indent=0))
 
     return results
 
 
 def find_cid(string):
     """Find a Fedora compose ID (or a fedfind fake CID) in a string."""
@@ -795,24 +802,33 @@
     # Determine the URL
     if flist not in ("fedora", "alt", "archive"):
         raise ValueError("_get_filelist: must be fedora, archive or alt!")
     fname = "imagelist-{}".format(flist)
     url = "/".join((fedfind.const.HTTPS_DL, flist, fname))
     logger.debug("_get_filelist: url is %s", url)
 
-    # Determine the cache location
-    cachefile = os.path.join(CACHEDIR, fname)
-    logger.debug("_get_filelist: cachefile is %s", cachefile)
-
-    # Get the cache file handle, if file is present
-    try:
-        cachefh = codecs.open(cachefile, "r", encoding="utf-8")
-    except (IOError, OSError):
+    cachef = os.path.join(CACHEDIR, fname)
+    usecache = True
+    if os.environ.get("FEDFIND_NO_CACHE"):
+        # we'll still actually write the data to the cache dir,
+        # because that's kinda wired in. but by setting cachefh to
+        # None, we will always redownload it
+        usecache = False
         cachefh = None
 
+    if usecache:
+        # Determine the cache location
+        logger.debug("_get_filelist: cachef is %s", cachef)
+
+        # Get the cache file handle, if file is present
+        try:
+            cachefh = io.open(cachef, "r", encoding="utf-8")  # pylint:disable=consider-using-with
+        except (IOError, OSError):
+            cachefh = None
+
     # Get the response and last modified date
     try:
         resp = urlopen_retries(url)
         modified = resp.headers["last-modified"]
     except ValueError:
         if cachefh:
             logger.warning(
@@ -841,39 +857,40 @@
             cachedate = ""
         if cachedate == modified:
             logger.debug("_get_filelist: cache hit, returning")
             if record:
                 logger.debug("Updating record")
                 record["cache"] = True
             return cachefh
+        cachefh.close()
 
     # If we got here, either we don't have a cache file at all or the
     # dates don't match. So we need to re-download it
 
     # I've seen CACHEDIR suddenly vanish, when it's a temp dir; let's
     # check and re-create it if necessary
     if not os.path.exists(CACHEDIR):
         os.makedirs(CACHEDIR)
 
-    with codecs.open(cachefile + ".tmp", "w", encoding="utf-8") as cachefh:
+    with io.open(cachef + ".tmp", "w", encoding="utf-8") as cachefh:
         # Write the modified date line
         cachefh.write(modified + "\n")
-    with open(cachefile + ".tmp", "ab") as cachefh:
+    with open(cachef + ".tmp", "ab") as cachefh:
         # Now download and write the file, in 1MB chunks at a time
         while True:
             chunk = resp.read(1024 * 1024)
             if chunk:
                 cachefh.write(chunk)
                 cachefh.flush()
             else:
                 break
 
-    os.rename(cachefile + ".tmp", cachefile)
+    os.rename(cachef + ".tmp", cachef)
 
     # Now open the read-only filehandle, iterate out the date line,
     # and return
-    cachefh = codecs.open(cachefile, "r", encoding="utf-8")
+    cachefh = io.open(cachef, "r", encoding="utf-8")  # pylint:disable=consider-using-with
     next(cachefh)
     return cachefh
 
 
 # vim: set textwidth=100 ts=8 et sw=4:
```

### Comparing `fedfind-5.2.0/src/fedfind/release.py` & `fedfind-5.3.0/src/fedfind/release.py`

 * *Files identical despite different names*

### Comparing `fedfind-5.2.0/src/fedfind.egg-info/PKG-INFO` & `fedfind-5.3.0/src/fedfind.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedfind
-Version: 5.2.0
+Version: 5.3.0
 Summary: Fedora Finder finds Fedora - images, more to come?
 Home-page: https://pagure.io/fedora-qa/fedfind
 Author: Adam Williamson
 Author-email: awilliam@redhat.com
 License: GPLv3+
 Keywords: fedora release image media iso
 Classifier: Development Status :: 5 - Production/Stable
@@ -186,14 +186,16 @@
 
 When used as a module it caches properties and image lists for the lifetime of the release instance. The image list files are cached (in `~/.cache/fedfind`) based on the 'last modified time' provided by the server they come from: for each new release instance, fedfind will hit the server to retrieve the last modified time header, but if the cached copy matches that time, it will not re-download the file. These files are also quite small so will not take long to download in any case. If the download fails for some reason, but we do have a cached copy of the necessary lists, fedfind will work but log a warning that it's using cached data which may be outdated.
 
 Certain PDC queries, whose results are never expected to change, are also cached (again in `~/.cache/fedfind`), to speed up repeated searches and reduce load on PDC.
 
 If `~/.cache/fedfind` is not writeable for the user running fedfind, we fall back to using a temporary cache location that is only valid for the life of the process (and deleted on exit). This at least ensures fedfind will work in this case, but results in it being slower and doing more round trips.
 
+You can set the environment variable `FEDFIND_NO_CACHE` to any value to disable this caching. File lists will still be written to `~/.cache/fedfind`, but the cached copy will never be used, the list will be re-downloaded each time it is requested. PDC queries will not be cached at all. This is intended for downstream projects whose test suites are affected by the caching (specifically, one that uses pyvcr).
+
 It shouldn't use too much bandwidth (though I haven't really measured), but obviously the server admins won't be happy with me if the servers get inundated with fedfind requests, so don't go *completely* crazy with it - if you want to do something script-y, please at least use the module and re-use release instances so the queries get cached.
 
 ### Can't find what ain't there
 
 All releases other than stable releases disappear. fedfind can find stable releases all the way back to Fedora Core 1, but it is not going to find Fedora 14 Alpha, Fedora 19 Beta TC3, or nightlies from more than 2-3 weeks ago. This isn't a bug in fedfind - those images literally are not publicly available any more. Nightlies only stick around for a few weeks, candidate composes for a given milestone usually disappear once we've moved on another couple of milestones, and pre-releases (Alphas and Betas) usually disappear some time after the release in question goes stable. fedfind will only find what's actually there.
 
 Also note that fedfind is not designed to find even *notional* locations for old non-stable releases. Due to their ephemeral nature, the patterns it uses for nightly builds and candidate composes only reflect current practice, and will simply be updated any time that practice changes. It doesn't have a big store of knowledge of what exact naming conventions we used for old composes. If you do `comp = fedfind.release.Compose(12, 'Final', 'TC4')` and read out `comp.location` or something what you get is almost certainly *not* the location where Fedora 12 Final TC4 actually lived when it was around.
```

### Comparing `fedfind-5.2.0/src/fedfind.egg-info/SOURCES.txt` & `fedfind-5.3.0/src/fedfind.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fedfind-5.2.0/tests/conftest.py` & `fedfind-5.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fedfind-5.2.0/tests/data/allstable.json` & `fedfind-5.3.0/tests/data/allstable.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.2.0/tests/data/compose-urls-20240423.json` & `fedfind-5.3.0/tests/data/compose-urls-20240423.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.2.0/tests/data/fedfindloc.py` & `fedfind-5.3.0/tests/data/fedfindloc.py`

 * *Files identical despite different names*

### Comparing `fedfind-5.2.0/tests/data/http/pub/alt/imagelist-alt` & `fedfind-5.3.0/tests/data/http/pub/alt/imagelist-alt`

 * *Files identical despite different names*

### Comparing `fedfind-5.2.0/tests/data/http/pub/archive/imagelist-archive` & `fedfind-5.3.0/tests/data/http/pub/archive/imagelist-archive`

 * *Files identical despite different names*

### Comparing `fedfind-5.2.0/tests/data/http/pub/fedora/imagelist-fedora` & `fedfind-5.3.0/tests/data/http/pub/fedora/imagelist-fedora`

 * *Files identical despite different names*

### Comparing `fedfind-5.2.0/tests/data/pdc-compimages-Fedora-24-20160614.0.json` & `fedfind-5.3.0/tests/data/pdc-compimages-Fedora-24-20160614.0.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.2.0/tests/data/pdc-compimages-Fedora-25-20161115.0.json` & `fedfind-5.3.0/tests/data/pdc-compimages-Fedora-25-20161115.0.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.2.0/tests/data/pdc-compimages-Fedora-26-20170705.0.json` & `fedfind-5.3.0/tests/data/pdc-compimages-Fedora-26-20170705.0.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.2.0/tests/data/pdc-compimages-Fedora-27-20171105.0.json` & `fedfind-5.3.0/tests/data/pdc-compimages-Fedora-27-20171105.0.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.2.0/tests/data/pdc-compimages-Fedora-28-20180425.0.json` & `fedfind-5.3.0/tests/data/pdc-compimages-Fedora-28-20180425.0.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.2.0/tests/data/pdc-compimages-Fedora-29-20181024.1.json` & `fedfind-5.3.0/tests/data/pdc-compimages-Fedora-29-20181024.1.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.2.0/tests/data/pdc-compimages-Fedora-30-20190425.0.json` & `fedfind-5.3.0/tests/data/pdc-compimages-Fedora-30-20190425.0.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.2.0/tests/data/pdc-compimages-Fedora-31-20191023.0.json` & `fedfind-5.3.0/tests/data/pdc-compimages-Fedora-31-20191023.0.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.2.0/tests/data/pdc-compimages-Fedora-32-20200422.0.json` & `fedfind-5.3.0/tests/data/pdc-compimages-Fedora-32-20200422.0.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.2.0/tests/data/pdc-compimages-Fedora-33-20201019.0.json` & `fedfind-5.3.0/tests/data/pdc-compimages-Fedora-33-20201019.0.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.2.0/tests/data/pdc-compimages-Fedora-34-20210423.0.json` & `fedfind-5.3.0/tests/data/pdc-compimages-Fedora-34-20210423.0.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.2.0/tests/data/pdc-compimages-Fedora-35-20211026.0.json` & `fedfind-5.3.0/tests/data/pdc-compimages-Fedora-35-20211026.0.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.2.0/tests/data/pdc-compimages-Fedora-36-20220504.1.json` & `fedfind-5.3.0/tests/data/pdc-compimages-Fedora-36-20220504.1.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.2.0/tests/data/pdc-compimages-Fedora-37-20221105.0.json` & `fedfind-5.3.0/tests/data/pdc-compimages-Fedora-37-20221105.0.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.2.0/tests/data/pdc-compimages-Fedora-38-20230413.1.json` & `fedfind-5.3.0/tests/data/pdc-compimages-Fedora-38-20230413.1.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.2.0/tests/data/pdc-compimages-Fedora-39-20231031.1.json` & `fedfind-5.3.0/tests/data/pdc-compimages-Fedora-39-20231031.1.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.2.0/tests/data/pdc-compimages-Fedora-40-20240414.0.json` & `fedfind-5.3.0/tests/data/pdc-compimages-Fedora-40-20240414.0.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.2.0/tests/test_helpers.py` & `fedfind-5.3.0/tests/test_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 # pylint: disable=too-many-public-methods
 
 """Tests for helpers.py."""
 
 from __future__ import unicode_literals
 from __future__ import print_function
 
-import codecs
 import datetime
 import hashlib
+import io
 import os
 import shutil
 
 try:
     # Python >= 3.3
     from unittest import mock
 except ImportError:
@@ -337,14 +337,36 @@
         data.
         """
         assert fedfind.helpers.pdc_query("composes") == ["some", "results"]
         # first (and only) positional arg to the download_json call should be a Request
         req = fakejson.call_args[0][0]
         assert isinstance(req, Request)
 
+    @mock.patch("fedfind.helpers.download_json", return_value=PDC_JSON, autospec=True)
+    def test_pdc_query_cache(self, fakejson, clean_home):
+        """Check pdc_query cache enable/disable works."""
+        assert not os.path.exists(os.path.join(clean_home, ".cache", "fedfind", "pdcquery.json"))
+        # test with caching disabled
+        with mock.patch.dict(os.environ, {"FEDFIND_NO_CACHE": "1"}):
+            # we use a path under compose-images as these are always cached
+            fedfind.helpers.pdc_query("compose-images/Fedora-40-20240414.0/")
+        # cache should not exist
+        assert not os.path.exists(os.path.join(clean_home, ".cache", "fedfind", "pdcquery.json"))
+        # now, with it enabled
+        fedfind.helpers.pdc_query("compose-images/Fedora-40-20240414.0/")
+        # cache should exist
+        assert os.path.exists(os.path.join(clean_home, ".cache", "fedfind", "pdcquery.json"))
+        # check whether using it works
+        fakejson.side_effect = ValueError("nope")
+        fedfind.helpers.pdc_query("compose-images/Fedora-40-20240414.0/")
+        # ...and we error out if it's turned off
+        with mock.patch.dict(os.environ, {"FEDFIND_NO_CACHE": "1"}):
+            with pytest.raises(ValueError):
+                fedfind.helpers.pdc_query("compose-images/Fedora-40-20240414.0/")
+
     def test_find_cid(self):
         """Check find_cid works correctly, with various common and
         tricky cases.
         """
         res = fedfind.helpers.find_cid("https://foo.com/compose/Fedora-24-20160314.n.0/compose")
         assert res == "Fedora-24-20160314.n.0"
         res = fedfind.helpers.find_cid("https://foo.com/compose/Fedora-24-20160314.0/compose")
@@ -827,37 +849,47 @@
             record = {}
             with fedfind.helpers._get_filelist(flist=flist, record=record) as testfh:
                 assert testfh.name == os.path.join(
                     clean_home, ".cache", "fedfind", "imagelist-{}".format(flist)
                 )
                 for line in testfh:
                     gotcksum.update(line.encode("utf-8"))
-            with codecs.open(origfile, encoding="utf-8") as origfh:
+            with io.open(origfile, encoding="utf-8") as origfh:
                 for line in origfh:
                     origcksum.update(line.encode("utf-8"))
             assert gotcksum.digest() == origcksum.digest()
             return record
 
+        # prime the cache
         check_file(flist)
+
+        # try with caching disabled, check we don't use it
+        with mock.patch.dict(os.environ, {"FEDFIND_NO_CACHE": "1"}):
+            record = check_file(flist)
+        assert record["cache"] is False
+
+        # now with caching enabled, check we hit cache
         record = check_file(flist)
         assert record["cache"] is True
 
+        # now with the server file time updated, we should not use the
+        # cached copy
         record = check_file(flist, touch=True)
         assert record["cache"] is False
 
         # now make the download fail: we should still work using the
         # cached copy, but warn about it
         origconst = fedfind.const.HTTPS_DL
         fedfind.const.HTTPS_DL = "http://localhost:5001/nonexistent"
         check_file(flist)
         # Reset the constant
         fedfind.const.HTTPS_DL = origconst
 
     @mock.patch("fedfind.helpers.download_json", return_value=PDC_JSON, autospec=True)
-    def test_cachedir_vanish(self, http, clean_home):
+    def test_cachedir_vanish(self, fakejson, clean_home, http):
         """Test that we recover from the cache dir suddenly vanishing.
         I saw this happen on openqa01 once - I think when we're using
         a temp dir as the cache location, it can get cleaned up by
         systemd or so while we're running.
         """
         fedfind.helpers._get_filelist(flist="fedora")
         assert os.path.exists(os.path.join(clean_home, ".cache", "fedfind"))
```

### Comparing `fedfind-5.2.0/tests/test_release.py` & `fedfind-5.3.0/tests/test_release.py`

 * *Files identical despite different names*

### Comparing `fedfind-5.2.0/tox.ini` & `fedfind-5.3.0/tox.ini`

 * *Files identical despite different names*

