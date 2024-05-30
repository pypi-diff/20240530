# Comparing `tmp/persistent-5.2.tar.gz` & `tmp/persistent-6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "persistent-5.2.tar", last modified: Fri Feb 16 08:32:12 2024, max compression
+gzip compressed data, was "persistent-6.0.tar", last modified: Thu May 30 07:18:19 2024, max compression
```

## Comparing `persistent-5.2.tar` & `persistent-6.0.tar`

### file list

```diff
@@ -1,76 +1,91 @@
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-16 08:32:12.258904 persistent-5.2/
--rw-r--r--   0 m.howitz   (502) staff       (20)      626 2024-02-16 08:32:11.000000 persistent-5.2/.coveragerc
--rwxr-xr-x   0 m.howitz   (502) staff       (20)     2255 2024-02-16 08:32:11.000000 persistent-5.2/.manylinux-install.sh
--rwxr-xr-x   0 m.howitz   (502) staff       (20)      509 2024-02-16 08:32:11.000000 persistent-5.2/.manylinux.sh
--rw-r--r--   0 m.howitz   (502) staff       (20)      664 2024-02-16 08:32:11.000000 persistent-5.2/.readthedocs.yaml
--rw-r--r--   0 m.howitz   (502) staff       (20)    17529 2024-02-16 08:32:11.000000 persistent-5.2/CHANGES.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      799 2024-02-16 08:32:11.000000 persistent-5.2/CONTRIBUTING.md
--rw-r--r--   0 m.howitz   (502) staff       (20)       32 2024-02-16 08:32:11.000000 persistent-5.2/COPYRIGHT.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2024-02-16 08:32:11.000000 persistent-5.2/LICENSE.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)      434 2024-02-16 08:32:11.000000 persistent-5.2/MANIFEST.in
--rw-r--r--   0 m.howitz   (502) staff       (20)    21121 2024-02-16 08:32:12.258782 persistent-5.2/PKG-INFO
--rw-r--r--   0 m.howitz   (502) staff       (20)     1834 2024-02-16 08:32:11.000000 persistent-5.2/README.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     1989 2024-02-16 08:32:11.000000 persistent-5.2/appveyor.yml
--rw-r--r--   0 m.howitz   (502) staff       (20)      196 2024-02-16 08:32:11.000000 persistent-5.2/buildout.cfg
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-16 08:32:12.249912 persistent-5.2/docs/
--rw-r--r--   0 m.howitz   (502) staff       (20)     4606 2024-02-16 08:32:11.000000 persistent-5.2/docs/Makefile
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-16 08:32:12.250775 persistent-5.2/docs/api/
--rw-r--r--   0 m.howitz   (502) staff       (20)     6569 2024-02-16 08:32:11.000000 persistent-5.2/docs/api/attributes.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     1831 2024-02-16 08:32:11.000000 persistent-5.2/docs/api/cache.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      386 2024-02-16 08:32:11.000000 persistent-5.2/docs/api/collections.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      553 2024-02-16 08:32:11.000000 persistent-5.2/docs/api/interfaces.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     3862 2024-02-16 08:32:11.000000 persistent-5.2/docs/api/pickling.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      187 2024-02-16 08:32:11.000000 persistent-5.2/docs/api.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       28 2024-02-16 08:32:11.000000 persistent-5.2/docs/changes.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     8683 2024-02-16 08:32:11.000000 persistent-5.2/docs/conf.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1721 2024-02-16 08:32:11.000000 persistent-5.2/docs/glossary.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      472 2024-02-16 08:32:11.000000 persistent-5.2/docs/index.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     4519 2024-02-16 08:32:11.000000 persistent-5.2/docs/make.bat
--rw-r--r--   0 m.howitz   (502) staff       (20)       68 2024-02-16 08:32:11.000000 persistent-5.2/docs/requirements.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)    12416 2024-02-16 08:32:11.000000 persistent-5.2/docs/using.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      538 2024-02-16 08:32:12.259197 persistent-5.2/setup.cfg
--rw-r--r--   0 m.howitz   (502) staff       (20)     4703 2024-02-16 08:32:11.000000 persistent-5.2/setup.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-16 08:32:12.245491 persistent-5.2/src/
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-16 08:32:12.253926 persistent-5.2/src/persistent/
--rw-r--r--   0 m.howitz   (502) staff       (20)     1508 2024-02-16 08:32:11.000000 persistent-5.2/src/persistent/__init__.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1464 2024-02-16 08:32:11.000000 persistent-5.2/src/persistent/_compat.h
--rw-r--r--   0 m.howitz   (502) staff       (20)     6878 2024-02-16 08:32:11.000000 persistent-5.2/src/persistent/_compat.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1959 2024-02-16 08:32:11.000000 persistent-5.2/src/persistent/_ring_build.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    16671 2024-02-16 08:32:11.000000 persistent-5.2/src/persistent/_timestamp.c
--rw-r--r--   0 m.howitz   (502) staff       (20)    47651 2024-02-16 08:32:11.000000 persistent-5.2/src/persistent/cPersistence.c
--rw-r--r--   0 m.howitz   (502) staff       (20)     5105 2024-02-16 08:32:11.000000 persistent-5.2/src/persistent/cPersistence.h
--rw-r--r--   0 m.howitz   (502) staff       (20)    42156 2024-02-16 08:32:11.000000 persistent-5.2/src/persistent/cPickleCache.c
--rw-r--r--   0 m.howitz   (502) staff       (20)      751 2024-02-16 08:32:11.000000 persistent-5.2/src/persistent/dict.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    18439 2024-02-16 08:32:11.000000 persistent-5.2/src/persistent/interfaces.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     4551 2024-02-16 08:32:11.000000 persistent-5.2/src/persistent/list.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     5715 2024-02-16 08:32:11.000000 persistent-5.2/src/persistent/mapping.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    22814 2024-02-16 08:32:11.000000 persistent-5.2/src/persistent/persistence.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    18771 2024-02-16 08:32:11.000000 persistent-5.2/src/persistent/picklecache.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1853 2024-02-16 08:32:11.000000 persistent-5.2/src/persistent/ring.c
--rw-r--r--   0 m.howitz   (502) staff       (20)     2640 2024-02-16 08:32:11.000000 persistent-5.2/src/persistent/ring.h
--rw-r--r--   0 m.howitz   (502) staff       (20)     6641 2024-02-16 08:32:11.000000 persistent-5.2/src/persistent/ring.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-16 08:32:12.257927 persistent-5.2/src/persistent/tests/
--rw-r--r--   0 m.howitz   (502) staff       (20)       10 2024-02-16 08:32:11.000000 persistent-5.2/src/persistent/tests/__init__.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     4214 2024-02-16 08:32:11.000000 persistent-5.2/src/persistent/tests/attrhooks.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     2798 2024-02-16 08:32:11.000000 persistent-5.2/src/persistent/tests/cucumbers.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     3423 2024-02-16 08:32:11.000000 persistent-5.2/src/persistent/tests/test__compat.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1286 2024-02-16 08:32:11.000000 persistent-5.2/src/persistent/tests/test_compile_flags.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1867 2024-02-16 08:32:11.000000 persistent-5.2/src/persistent/tests/test_docs.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    10649 2024-02-16 08:32:11.000000 persistent-5.2/src/persistent/tests/test_list.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    10087 2024-02-16 08:32:11.000000 persistent-5.2/src/persistent/tests/test_mapping.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    77507 2024-02-16 08:32:11.000000 persistent-5.2/src/persistent/tests/test_persistence.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    45136 2024-02-16 08:32:11.000000 persistent-5.2/src/persistent/tests/test_picklecache.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     3320 2024-02-16 08:32:11.000000 persistent-5.2/src/persistent/tests/test_ring.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    15098 2024-02-16 08:32:11.000000 persistent-5.2/src/persistent/tests/test_timestamp.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    11299 2024-02-16 08:32:11.000000 persistent-5.2/src/persistent/tests/test_wref.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     3387 2024-02-16 08:32:11.000000 persistent-5.2/src/persistent/tests/utils.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     6124 2024-02-16 08:32:11.000000 persistent-5.2/src/persistent/timestamp.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     4083 2024-02-16 08:32:11.000000 persistent-5.2/src/persistent/wref.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-16 08:32:12.258243 persistent-5.2/src/persistent.egg-info/
--rw-r--r--   0 m.howitz   (502) staff       (20)    21121 2024-02-16 08:32:12.000000 persistent-5.2/src/persistent.egg-info/PKG-INFO
--rw-r--r--   0 m.howitz   (502) staff       (20)     1686 2024-02-16 08:32:12.000000 persistent-5.2/src/persistent.egg-info/SOURCES.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)        1 2024-02-16 08:32:12.000000 persistent-5.2/src/persistent.egg-info/dependency_links.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)        1 2024-02-16 08:32:12.000000 persistent-5.2/src/persistent.egg-info/not-zip-safe
--rw-r--r--   0 m.howitz   (502) staff       (20)      170 2024-02-16 08:32:12.000000 persistent-5.2/src/persistent.egg-info/requires.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)       11 2024-02-16 08:32:12.000000 persistent-5.2/src/persistent.egg-info/top_level.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)     2251 2024-02-16 08:32:11.000000 persistent-5.2/tox.ini
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 07:18:19.368452 persistent-6.0/
+-rw-r--r--   0 jens       (501) staff       (20)      651 2024-05-30 06:42:43.000000 persistent-6.0/.coveragerc
+-rwxr-xr-x   0 jens       (501) staff       (20)     2189 2024-05-30 06:42:43.000000 persistent-6.0/.manylinux-install.sh
+-rwxr-xr-x   0 jens       (501) staff       (20)      509 2024-05-30 06:42:43.000000 persistent-6.0/.manylinux.sh
+-rw-r--r--   0 jens       (501) staff       (20)      664 2024-05-30 06:42:43.000000 persistent-6.0/.readthedocs.yaml
+-rw-r--r--   0 jens       (501) staff       (20)    17629 2024-05-30 06:43:09.000000 persistent-6.0/CHANGES.rst
+-rw-r--r--   0 jens       (501) staff       (20)      799 2024-05-30 06:42:43.000000 persistent-6.0/CONTRIBUTING.md
+-rw-r--r--   0 jens       (501) staff       (20)       32 2022-11-03 13:57:25.000000 persistent-6.0/COPYRIGHT.txt
+-rw-r--r--   0 jens       (501) staff       (20)     2070 2022-11-03 13:57:25.000000 persistent-6.0/LICENSE.txt
+-rw-r--r--   0 jens       (501) staff       (20)      413 2024-05-30 06:42:43.000000 persistent-6.0/MANIFEST.in
+-rw-r--r--   0 jens       (501) staff       (20)    21313 2024-05-30 07:18:19.368370 persistent-6.0/PKG-INFO
+-rw-r--r--   0 jens       (501) staff       (20)     1834 2022-11-16 09:58:56.000000 persistent-6.0/README.rst
+-rw-r--r--   0 jens       (501) staff       (20)      196 2022-11-03 13:57:25.000000 persistent-6.0/buildout.cfg
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 07:18:19.359737 persistent-6.0/docs/
+-rw-r--r--   0 jens       (501) staff       (20)     4606 2022-11-03 13:57:25.000000 persistent-6.0/docs/Makefile
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 07:18:19.356172 persistent-6.0/docs/_build/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 07:18:19.359972 persistent-6.0/docs/_build/doctest/
+-rw-r--r--   0 jens       (501) staff       (20)      833 2024-04-03 07:09:08.000000 persistent-6.0/docs/_build/doctest/output.txt
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 07:18:19.356211 persistent-6.0/docs/_build/html/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 07:18:19.360658 persistent-6.0/docs/_build/html/_sources/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 07:18:19.361498 persistent-6.0/docs/_build/html/_sources/api/
+-rw-r--r--   0 jens       (501) staff       (20)     6569 2022-11-03 13:57:25.000000 persistent-6.0/docs/_build/html/_sources/api/attributes.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     1831 2022-11-03 13:57:25.000000 persistent-6.0/docs/_build/html/_sources/api/cache.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)      386 2022-11-03 13:57:25.000000 persistent-6.0/docs/_build/html/_sources/api/collections.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)      553 2022-11-03 13:57:25.000000 persistent-6.0/docs/_build/html/_sources/api/interfaces.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     3862 2022-11-03 13:57:25.000000 persistent-6.0/docs/_build/html/_sources/api/pickling.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)      187 2022-11-03 13:57:25.000000 persistent-6.0/docs/_build/html/_sources/api.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)       28 2022-11-03 13:57:25.000000 persistent-6.0/docs/_build/html/_sources/changes.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     1721 2022-11-03 13:57:25.000000 persistent-6.0/docs/_build/html/_sources/glossary.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)      472 2022-11-03 13:57:25.000000 persistent-6.0/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)    12416 2022-11-03 13:57:25.000000 persistent-6.0/docs/_build/html/_sources/using.rst.txt
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 07:18:19.362222 persistent-6.0/docs/api/
+-rw-r--r--   0 jens       (501) staff       (20)     6569 2022-11-03 13:57:25.000000 persistent-6.0/docs/api/attributes.rst
+-rw-r--r--   0 jens       (501) staff       (20)     1831 2022-11-03 13:57:25.000000 persistent-6.0/docs/api/cache.rst
+-rw-r--r--   0 jens       (501) staff       (20)      386 2022-11-03 13:57:25.000000 persistent-6.0/docs/api/collections.rst
+-rw-r--r--   0 jens       (501) staff       (20)      553 2022-11-03 13:57:25.000000 persistent-6.0/docs/api/interfaces.rst
+-rw-r--r--   0 jens       (501) staff       (20)     3862 2022-11-03 13:57:25.000000 persistent-6.0/docs/api/pickling.rst
+-rw-r--r--   0 jens       (501) staff       (20)      187 2022-11-03 13:57:25.000000 persistent-6.0/docs/api.rst
+-rw-r--r--   0 jens       (501) staff       (20)       28 2022-11-03 13:57:25.000000 persistent-6.0/docs/changes.rst
+-rw-r--r--   0 jens       (501) staff       (20)     8683 2023-10-05 12:50:50.000000 persistent-6.0/docs/conf.py
+-rw-r--r--   0 jens       (501) staff       (20)     1721 2022-11-03 13:57:25.000000 persistent-6.0/docs/glossary.rst
+-rw-r--r--   0 jens       (501) staff       (20)      472 2022-11-03 13:57:25.000000 persistent-6.0/docs/index.rst
+-rw-r--r--   0 jens       (501) staff       (20)     4519 2022-11-03 13:57:25.000000 persistent-6.0/docs/make.bat
+-rw-r--r--   0 jens       (501) staff       (20)       68 2023-10-05 12:50:50.000000 persistent-6.0/docs/requirements.txt
+-rw-r--r--   0 jens       (501) staff       (20)    12416 2022-11-03 13:57:25.000000 persistent-6.0/docs/using.rst
+-rw-r--r--   0 jens       (501) staff       (20)      509 2024-05-30 07:18:19.368642 persistent-6.0/setup.cfg
+-rw-r--r--   0 jens       (501) staff       (20)     4883 2024-05-30 06:46:21.000000 persistent-6.0/setup.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 07:18:19.356461 persistent-6.0/src/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 07:18:19.364928 persistent-6.0/src/persistent/
+-rw-r--r--   0 jens       (501) staff       (20)     1510 2024-04-03 07:02:42.000000 persistent-6.0/src/persistent/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)     1464 2023-01-03 12:38:43.000000 persistent-6.0/src/persistent/_compat.h
+-rw-r--r--   0 jens       (501) staff       (20)     6892 2024-04-03 07:02:42.000000 persistent-6.0/src/persistent/_compat.py
+-rw-r--r--   0 jens       (501) staff       (20)     1990 2024-04-03 07:02:42.000000 persistent-6.0/src/persistent/_ring_build.py
+-rw-r--r--   0 jens       (501) staff       (20)    16671 2023-01-03 12:38:43.000000 persistent-6.0/src/persistent/_timestamp.c
+-rw-r--r--   0 jens       (501) staff       (20)    47651 2023-01-03 12:38:43.000000 persistent-6.0/src/persistent/cPersistence.c
+-rw-r--r--   0 jens       (501) staff       (20)     5105 2022-11-03 13:57:25.000000 persistent-6.0/src/persistent/cPersistence.h
+-rw-r--r--   0 jens       (501) staff       (20)    42156 2023-01-03 12:38:43.000000 persistent-6.0/src/persistent/cPickleCache.c
+-rw-r--r--   0 jens       (501) staff       (20)      947 2024-04-03 07:02:42.000000 persistent-6.0/src/persistent/dict.py
+-rw-r--r--   0 jens       (501) staff       (20)    18385 2024-04-03 07:02:42.000000 persistent-6.0/src/persistent/interfaces.py
+-rw-r--r--   0 jens       (501) staff       (20)     4563 2024-04-03 07:02:42.000000 persistent-6.0/src/persistent/list.py
+-rw-r--r--   0 jens       (501) staff       (20)     5686 2024-05-16 15:28:23.000000 persistent-6.0/src/persistent/mapping.py
+-rw-r--r--   0 jens       (501) staff       (20)    22419 2024-05-16 15:28:23.000000 persistent-6.0/src/persistent/persistence.py
+-rw-r--r--   0 jens       (501) staff       (20)    18715 2024-05-16 15:28:23.000000 persistent-6.0/src/persistent/picklecache.py
+-rw-r--r--   0 jens       (501) staff       (20)     1853 2022-11-03 13:57:25.000000 persistent-6.0/src/persistent/ring.c
+-rw-r--r--   0 jens       (501) staff       (20)     2640 2022-11-03 13:57:25.000000 persistent-6.0/src/persistent/ring.h
+-rw-r--r--   0 jens       (501) staff       (20)     6401 2024-05-16 15:28:23.000000 persistent-6.0/src/persistent/ring.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 07:18:19.367776 persistent-6.0/src/persistent/tests/
+-rw-r--r--   0 jens       (501) staff       (20)       10 2022-11-03 13:57:25.000000 persistent-6.0/src/persistent/tests/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)     4218 2024-04-03 07:02:42.000000 persistent-6.0/src/persistent/tests/attrhooks.py
+-rw-r--r--   0 jens       (501) staff       (20)     2797 2024-04-03 07:02:42.000000 persistent-6.0/src/persistent/tests/cucumbers.py
+-rw-r--r--   0 jens       (501) staff       (20)     3422 2024-05-16 15:28:23.000000 persistent-6.0/src/persistent/tests/test__compat.py
+-rw-r--r--   0 jens       (501) staff       (20)     1286 2022-11-03 13:57:25.000000 persistent-6.0/src/persistent/tests/test_compile_flags.py
+-rw-r--r--   0 jens       (501) staff       (20)     1779 2024-05-16 15:28:23.000000 persistent-6.0/src/persistent/tests/test_docs.py
+-rw-r--r--   0 jens       (501) staff       (20)    10483 2024-05-16 15:28:23.000000 persistent-6.0/src/persistent/tests/test_list.py
+-rw-r--r--   0 jens       (501) staff       (20)     9967 2024-05-16 15:28:23.000000 persistent-6.0/src/persistent/tests/test_mapping.py
+-rw-r--r--   0 jens       (501) staff       (20)    77570 2024-05-16 15:28:23.000000 persistent-6.0/src/persistent/tests/test_persistence.py
+-rw-r--r--   0 jens       (501) staff       (20)    45207 2024-05-16 15:28:23.000000 persistent-6.0/src/persistent/tests/test_picklecache.py
+-rw-r--r--   0 jens       (501) staff       (20)     3286 2024-05-16 15:28:23.000000 persistent-6.0/src/persistent/tests/test_ring.py
+-rw-r--r--   0 jens       (501) staff       (20)    15050 2024-05-16 15:28:23.000000 persistent-6.0/src/persistent/tests/test_timestamp.py
+-rw-r--r--   0 jens       (501) staff       (20)    11245 2024-04-03 07:02:42.000000 persistent-6.0/src/persistent/tests/test_wref.py
+-rw-r--r--   0 jens       (501) staff       (20)     3400 2024-04-03 07:02:42.000000 persistent-6.0/src/persistent/tests/utils.py
+-rw-r--r--   0 jens       (501) staff       (20)     6059 2024-05-16 15:28:23.000000 persistent-6.0/src/persistent/timestamp.py
+-rw-r--r--   0 jens       (501) staff       (20)     4082 2024-04-03 07:02:42.000000 persistent-6.0/src/persistent/wref.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 07:18:19.368011 persistent-6.0/src/persistent.egg-info/
+-rw-r--r--   0 jens       (501) staff       (20)    21313 2024-05-30 07:18:19.000000 persistent-6.0/src/persistent.egg-info/PKG-INFO
+-rw-r--r--   0 jens       (501) staff       (20)     2146 2024-05-30 07:18:19.000000 persistent-6.0/src/persistent.egg-info/SOURCES.txt
+-rw-r--r--   0 jens       (501) staff       (20)        1 2024-05-30 07:18:19.000000 persistent-6.0/src/persistent.egg-info/dependency_links.txt
+-rw-r--r--   0 jens       (501) staff       (20)        1 2022-11-03 13:59:25.000000 persistent-6.0/src/persistent.egg-info/not-zip-safe
+-rw-r--r--   0 jens       (501) staff       (20)      285 2024-05-30 07:18:19.000000 persistent-6.0/src/persistent.egg-info/requires.txt
+-rw-r--r--   0 jens       (501) staff       (20)       11 2024-05-30 07:18:19.000000 persistent-6.0/src/persistent.egg-info/top_level.txt
+-rw-r--r--   0 jens       (501) staff       (20)     2173 2024-05-30 06:42:43.000000 persistent-6.0/tox.ini
```

### Comparing `persistent-5.2/.coveragerc` & `persistent-6.0/.coveragerc`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Generated from:
 # https://github.com/zopefoundation/meta/tree/master/config/c-code
 [run]
-source = persistent
+source = src/persistent
 # New in 5.0; required for the GHA coveralls submission.
 relative_files = True
 branch = true
 omit =
      src/persistent/_ring_build.py
 
 [paths]
@@ -13,14 +13,15 @@
     src/
     .tox/*/lib/python*/site-packages/
     .tox/pypy*/site-packages/
 
 [report]
 show_missing = true
 precision = 2
+ignore_errors = True
 exclude_lines =
     except ImportError:
     if __name__ == '__main__':
     pragma: no cover
     pragma: nocover
     raise AssertionError
     raise NotImplementedError
```

### Comparing `persistent-5.2/.manylinux-install.sh` & `persistent-6.0/.manylinux-install.sh`

 * *Files 7% similar despite different names*

```diff
@@ -25,35 +25,33 @@
 
 # We need some libraries because we build wheels from scratch:
 yum -y install libffi-devel
 
 tox_env_map() {
     case $1 in
         *"cp313"*) echo 'py313';;
-        *"cp37"*) echo 'py37';;
         *"cp38"*) echo 'py38';;
         *"cp39"*) echo 'py39';;
         *"cp310"*) echo 'py310';;
         *"cp311"*) echo 'py311';;
         *"cp312"*) echo 'py312';;
         *) echo 'py';;
     esac
 }
 
 # Compile wheels
 for PYBIN in /opt/python/*/bin; do
     if \
-       [[ "${PYBIN}" == *"cp313"* ]] || \
-       [[ "${PYBIN}" == *"cp311"* ]] || \
-       [[ "${PYBIN}" == *"cp312"* ]] || \
-       [[ "${PYBIN}" == *"cp37"* ]] || \
-       [[ "${PYBIN}" == *"cp38"* ]] || \
-       [[ "${PYBIN}" == *"cp39"* ]] || \
-       [[ "${PYBIN}" == *"cp310"* ]] ; then
-        if [[ "${PYBIN}" == *"cp313"* ]] ; then
+       [[ "${PYBIN}" == *"cp313/"* ]] || \
+       [[ "${PYBIN}" == *"cp311/"* ]] || \
+       [[ "${PYBIN}" == *"cp312/"* ]] || \
+       [[ "${PYBIN}" == *"cp38/"* ]] || \
+       [[ "${PYBIN}" == *"cp39/"* ]] || \
+       [[ "${PYBIN}" == *"cp310/"* ]] ; then
+        if [[ "${PYBIN}" == *"cp313/"* ]] ; then
             "${PYBIN}/pip" install --pre -e /io/
             "${PYBIN}/pip" wheel /io/ --pre -w wheelhouse/
         else
             "${PYBIN}/pip" install -e /io/
             "${PYBIN}/pip" wheel /io/ -w wheelhouse/
         fi
         if [ `uname -m` == 'aarch64' ]; then
```

### Comparing `persistent-5.2/.readthedocs.yaml` & `persistent-6.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `persistent-5.2/CHANGES.rst` & `persistent-6.0/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 ==========================
  ``persistent`` Changelog
 ==========================
 
+6.0 (2024-05-30)
+================
+
+- Drop support for Python 3.7.
+
+- Build Windows wheels on GHA.
+
+
 5.2 (2024-02-16)
 ================
 
 - Add preliminary support for Python 3.13a3.
 
 
 5.1 (2023-10-05)
```

### Comparing `persistent-5.2/CONTRIBUTING.md` & `persistent-6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `persistent-5.2/LICENSE.txt` & `persistent-6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `persistent-5.2/PKG-INFO` & `persistent-6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 Metadata-Version: 2.1
 Name: persistent
-Version: 5.2
+Version: 6.0
 Summary: Translucent persistent objects
 Home-page: https://github.com/zopefoundation/persistent/
 Author: Zope Foundation and Contributors
 Author-email: zodb-dev@zope.org
 License: ZPL 2.1
 Project-URL: Documentation, https://persistent.readthedocs.io
 Project-URL: Issue Tracker, https://github.com/zopefoundation/persistent/issues
 Project-URL: Sources, https://github.com/zopefoundation/persistent
 Classifier: Development Status :: 6 - Mature
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Framework :: ZODB
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 License-File: LICENSE.txt
+Requires-Dist: zope.deferredimport
 Requires-Dist: zope.interface
 Requires-Dist: cffi; platform_python_implementation == "CPython"
+Requires-Dist: cffi>=1.17.0rc1; platform_python_implementation == "CPython" and python_version >= "3.13a0"
 Provides-Extra: test
 Requires-Dist: zope.testrunner; extra == "test"
 Requires-Dist: manuel; extra == "test"
 Provides-Extra: testing
 Provides-Extra: docs
 Requires-Dist: Sphinx; extra == "docs"
 Requires-Dist: repoze.sphinx.autointerface; extra == "docs"
@@ -80,14 +81,22 @@
    version of  the ``persistent`` package.
 
 
 ==========================
  ``persistent`` Changelog
 ==========================
 
+6.0 (2024-05-30)
+================
+
+- Drop support for Python 3.7.
+
+- Build Windows wheels on GHA.
+
+
 5.2 (2024-02-16)
 ================
 
 - Add preliminary support for Python 3.13a3.
 
 
 5.1 (2023-10-05)
```

### Comparing `persistent-5.2/README.rst` & `persistent-6.0/README.rst`

 * *Files identical despite different names*

### Comparing `persistent-5.2/docs/Makefile` & `persistent-6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `persistent-5.2/docs/api/attributes.rst` & `persistent-6.0/docs/_build/html/_sources/api/attributes.rst.txt`

 * *Files identical despite different names*

### Comparing `persistent-5.2/docs/api/cache.rst` & `persistent-6.0/docs/_build/html/_sources/api/cache.rst.txt`

 * *Files identical despite different names*

### Comparing `persistent-5.2/docs/api/interfaces.rst` & `persistent-6.0/docs/_build/html/_sources/api/interfaces.rst.txt`

 * *Files identical despite different names*

### Comparing `persistent-5.2/docs/api/pickling.rst` & `persistent-6.0/docs/_build/html/_sources/api/pickling.rst.txt`

 * *Files identical despite different names*

### Comparing `persistent-5.2/docs/conf.py` & `persistent-6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `persistent-5.2/docs/glossary.rst` & `persistent-6.0/docs/_build/html/_sources/glossary.rst.txt`

 * *Files identical despite different names*

### Comparing `persistent-5.2/docs/make.bat` & `persistent-6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `persistent-5.2/docs/using.rst` & `persistent-6.0/docs/_build/html/_sources/using.rst.txt`

 * *Files identical despite different names*

### Comparing `persistent-5.2/setup.py` & `persistent-6.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,33 +8,40 @@
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 
-import platform
 import os
+import platform
 
 from setuptools import Extension
 from setuptools import find_packages
 from setuptools import setup
 
-version = '5.2'
+
+version = '6.0'
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 
 def _read_file(filename):
     with open(os.path.join(here, filename)) as f:
         return f.read()
 
 
 README = (_read_file('README.rst') + '\n\n' + _read_file('CHANGES.rst'))
 
+PY313_CFFI_GH_DEP = (
+    "cffi >= 1.17.0rc1; "
+    "platform_python_implementation == 'CPython' and "
+    "python_version >= '3.13a0'"
+)
+
 
 define_macros = (
     # We currently use macros like PyBytes_AS_STRING
     # and internal functions like _PyObject_GetDictPtr
     # that make it impossible to use the stable (limited) API.
     # ('Py_LIMITED_API', '0x03050000'),
 )
@@ -90,15 +97,14 @@
       description='Translucent persistent objects',
       long_description=README,
       classifiers=[
           "Development Status :: 6 - Mature",
           "License :: OSI Approved :: Zope Public License",
           "Programming Language :: Python",
           "Programming Language :: Python :: 3",
-          "Programming Language :: Python :: 3.7",
           "Programming Language :: Python :: 3.8",
           "Programming Language :: Python :: 3.9",
           "Programming Language :: Python :: 3.10",
           "Programming Language :: Python :: 3.11",
           "Programming Language :: Python :: 3.12",
           "Programming Language :: Python :: Implementation :: CPython",
           "Programming Language :: Python :: Implementation :: PyPy",
@@ -132,16 +138,19 @@
           'testing': (),
           'docs': [
               'Sphinx',
               'repoze.sphinx.autointerface',
               'sphinx_rtd_theme',
           ],
       },
-      python_requires='>=3.7',
+      python_requires='>=3.8',
       install_requires=[
+          'zope.deferredimport',
           'zope.interface',
           "cffi ; platform_python_implementation == 'CPython'",
+          PY313_CFFI_GH_DEP,
       ],
       setup_requires=[
           "cffi ; platform_python_implementation == 'CPython'",
+          PY313_CFFI_GH_DEP,
       ],
       entry_points={})
```

### Comparing `persistent-5.2/src/persistent/__init__.py` & `persistent-6.0/src/persistent/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,30 +14,32 @@
 """Prefer C implementations of Persistent / PickleCache / TimeStamp.
 
 Fall back to pure Python implementations.
 """
 
 import sys
 
+
 __all__ = [
     'IPersistent',
     'Persistent',
     'GHOST',
     'UPTODATE',
     'CHANGED',
     'STICKY',
     'PickleCache',
     'TimeStamp',
 ]
 
 # Take care not to shadow the module names
 from persistent import interfaces as _interfaces
-from persistent import timestamp as _timestamp
 from persistent import persistence as _persistence
 from persistent import picklecache as _picklecache
+from persistent import timestamp as _timestamp
+
 
 IPersistent = _interfaces.IPersistent
 Persistent = _persistence.Persistent
 GHOST = _interfaces.GHOST
 UPTODATE = _interfaces.UPTODATE
 CHANGED = _interfaces.CHANGED
 STICKY = _interfaces.STICKY
```

### Comparing `persistent-5.2/src/persistent/_compat.h` & `persistent-6.0/src/persistent/_compat.h`

 * *Files identical despite different names*

### Comparing `persistent-5.2/src/persistent/_compat.py` & `persistent-6.0/src/persistent/_compat.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,20 +8,21 @@
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 
-import sys
 import os
+import sys
 import types
 
-from zope.interface import implementedBy
 from zope.interface import classImplements
+from zope.interface import implementedBy
+
 
 __all__ = [
     'use_c_impl',
     'PYPY',
 ]
 
 
@@ -48,23 +49,23 @@
     raises the ImportError. Either all optimization modules are
     available or none are.
 
     This does not say whether they should be used or not.
     """
     catch = () if _c_optimizations_required() else (ImportError,)
     try:
+        from persistent import _timestamp
         from persistent import cPersistence
         from persistent import cPickleCache
-        from persistent import _timestamp
         return {
             'persistent.persistence': cPersistence,
             'persistent.picklecache': cPickleCache,
             'persistent.timestamp': _timestamp,
         }
-    except catch: # pragma: no cover (only Jython doesn't build extensions)
+    except catch:  # pragma: no cover (only Jython doesn't build extensions)
         return {}
 
 
 def _c_optimizations_ignored():
     """
     The opposite of `_c_optimizations_required`.
 
@@ -88,15 +89,15 @@
     ``PURE_PYTHON`` environment variable, as defined in `use_c_impl`.
 
     Note that setting ``PURE_PYTHON=0`` forces the use of C optimizations,
     even on PyPy.
     """
     if _c_optimizations_required():
         return True
-    if PYPY: # pragma: no cover
+    if PYPY:  # pragma: no cover
         return False
     return not _c_optimizations_ignored()
 
 
 def use_c_impl(py_impl, name=None, globs=None, mod_name=None):
     """
     Decorator. Given an object implemented in Python, with a name like
@@ -152,15 +153,16 @@
     mod_name = mod_name or globs['__name__']
 
     def find_impl():
         if not _should_attempt_c_optimizations():
             return py_impl
 
         c_opts = _c_optimizations_available()
-        if not c_opts: # pragma: no cover (only Jython doesn't build extensions)
+        # only Jython doesn't build extensions:
+        if not c_opts:  # pragma: no cover
             return py_impl
 
         __traceback_info__ = c_opts
         c_opt = c_opts[mod_name]
         return getattr(c_opt, name)
 
     c_impl = find_impl()
@@ -184,15 +186,15 @@
 
             if new_globals is None:
                 new_globals = v.__globals__.copy()
                 new_globals[py_impl.__name__] = py_impl
             v = types.FunctionType(
                 v.__code__,
                 new_globals,
-                k, # name
+                k,  # name
                 v.__defaults__,
                 v.__closure__,
             )
             if static:
                 v = staticmethod(v)
             setattr(py_impl, k, v)
         # copy the interface declarations.
```

### Comparing `persistent-5.2/src/persistent/_ring_build.py` & `persistent-6.0/src/persistent/_ring_build.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 
 import os
+
 from cffi import FFI
 
+
 this_dir = os.path.dirname(os.path.abspath(__file__))
 
 ffi = FFI()
 with open(os.path.join(this_dir, 'ring.h')) as f:
     cdefs = f.read()
 
 # Define a structure with the same layout as CPersistentRing,
@@ -47,15 +49,15 @@
 
 /* Like the other functions, but taking the CFFI version of the struct. This
  * saves casting at runtime in Python.
  */
 #define cffi_ring_add(ring, elt) ring_add((CPersistentRing*)ring, (CPersistentRing*)elt)
 #define cffi_ring_del(elt) ring_del((CPersistentRing*)elt)
 #define cffi_ring_move_to_head(ring, elt) ring_move_to_head((CPersistentRing*)ring, (CPersistentRing*)elt)
-"""
+"""   # noqa: E501 line too long
 
 ffi.set_source('persistent._ring',
                source,
                include_dirs=[this_dir])
 
 if __name__ == '__main__':
     ffi.compile()
```

### Comparing `persistent-5.2/src/persistent/_timestamp.c` & `persistent-6.0/src/persistent/_timestamp.c`

 * *Files identical despite different names*

### Comparing `persistent-5.2/src/persistent/cPersistence.c` & `persistent-6.0/src/persistent/cPersistence.c`

 * *Files identical despite different names*

### Comparing `persistent-5.2/src/persistent/cPersistence.h` & `persistent-6.0/src/persistent/cPersistence.h`

 * *Files identical despite different names*

### Comparing `persistent-5.2/src/persistent/cPickleCache.c` & `persistent-6.0/src/persistent/cPickleCache.c`

 * *Files identical despite different names*

### Comparing `persistent-5.2/src/persistent/dict.py` & `persistent-6.0/src/persistent/dict.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,10 +7,17 @@
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
+from zope.deferredimport import deprecated
 
-# persistent.dict is deprecated. Use persistent.mapping
-from persistent.mapping import PersistentMapping as PersistentDict
+
+deprecated(
+    "`persistent.dict.PersistentDict` is deprecated. Use"
+    " `persistent.mapping.PersistentMapping` instead."
+    " This backward compatibility shim will be removed in persistent"
+    " version 6.",
+    PersistentDict='persistent.mapping:PersistentMapping',
+)
```

### Comparing `persistent-5.2/src/persistent/interfaces.py` & `persistent-6.0/src/persistent/interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Persistence Interfaces
 """
 
-from zope.interface import Interface
 from zope.interface import Attribute
+from zope.interface import Interface
 
 from persistent._compat import use_c_impl
 
 
 # Allowed values for _p_state. Use the C constants if available (which
 # are defined in cPersistence --- there is no cInterfaces --- so we
 # need to pass the corresponding ``mod_name``), otherwise define some
@@ -28,14 +28,15 @@
 UPTODATE = use_c_impl(0, 'UPTODATE', mod_name='persistent.persistence')
 CHANGED = use_c_impl(1, 'CHANGED', mod_name='persistent.persistence')
 STICKY = use_c_impl(2, 'STICKY', mod_name='persistent.persistence')
 
 
 OID_TYPE = SERIAL_TYPE = bytes
 
+
 class IPersistent(Interface):
     """Python persistent interface
 
     A persistent object can be in one of several states:
 
     - Unsaved
 
@@ -352,14 +353,15 @@
 
         The method unghostifies the object, if necessary.
         The method records the object access, if necessary.
         """
 
 # TODO:  document conflict resolution.
 
+
 class IPersistentDataManager(Interface):
     """Provide services for managing persistent state.
 
     This interface is used by a persistent object to interact with its
     data manager in the context of a transaction.
     """
     _cache = Attribute("The pickle cache associated with this connection.")
@@ -395,21 +397,21 @@
         the changed state.
 
         A subclass could override this method to customize the default
         policy of one transaction manager for each thread.
         """
 
 # Maybe later:
-##     def mtime(object):
-##         """Return the modification time of the object.
+# def mtime(object):
+# """Return the modification time of the object.
 
-##         The modification time may not be known, in which case None
-##         is returned.  If non-None, the return value is the kind of
-##         timestamp supplied by Python's time.time().
-##         """
+# The modification time may not be known, in which case None
+# is returned.  If non-None, the return value is the kind of
+# timestamp supplied by Python's time.time().
+# """
 
 
 class IPickleCache(Interface):
     """ API of the cache for a ZODB connection.
     """
     def __getitem__(oid):
         """ -> the persistent object for OID.
@@ -506,15 +508,14 @@
         If the object's '_p_oid' is not None, raise.
 
         If the object's '_p_jar' is not None, raise.
 
         If 'oid' is already in the cache, raise.
         """
 
-
     def invalidate(to_invalidate):
         """ Invalidate the indicated objects.
 
         o If 'to_invalidate' is a string, treat it as an OID.
 
         o Otherwise, iterate over it as a sequence of OIDs.
 
@@ -533,18 +534,18 @@
 
     def update_object_size_estimation(oid, new_size):
         """Update the cache's size estimation for 'oid', if known to the cache.
         """
 
     cache_size = Attribute('Target size of the cache')
     cache_drain_resistance = Attribute('Factor for draining cache below '
-                                        'target size')
+                                       'target size')
     cache_non_ghost_count = Attribute('Number of non-ghosts in the cache '
-                                        '(XXX how is it different from '
-                                        'ringlen?')
+                                      '(XXX how is it different from '
+                                      'ringlen?')
     cache_data = Attribute("Property:  copy of our 'data' dict")
     cache_klass_count = Attribute("Property: len of 'persistent_classes'")
 
 
 class IExtendedPickleCache(IPickleCache):
     """
     Extra operations for a pickle cache.
```

### Comparing `persistent-5.2/src/persistent/list.py` & `persistent-6.0/src/persistent/list.py`

 * *Files identical despite different names*

```diff
@@ -10,31 +10,33 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE
 #
 ##############################################################################
 
 """Python implementation of persistent list."""
 import sys
-import persistent
 from collections import UserList
 
+import persistent
+
+
 # The slice object you get when you write list[:]
 _SLICE_ALL = slice(None, None, None)
 
 
 class PersistentList(UserList, persistent.Persistent):
     """A persistent wrapper for list objects.
 
     Mutating instances of this class will cause them to be marked
     as changed and automatically persisted.
 
     .. versionchanged:: 4.5.2
-       Using the `clear` method, or deleting a slice (e.g., ``del inst[:]`` or ``del inst[x:x]``)
-       now only results in marking the instance as changed if it actually removed
-       items.
+       Using the `clear` method, or deleting a slice (e.g., ``del inst[:]`` or
+       ``del inst[x:x]``) now only results in marking the instance as changed
+       if it actually removed items.
     """
     __super_getitem = UserList.__getitem__
     __super_setitem = UserList.__setitem__
     __super_delitem = UserList.__delitem__
     __super_iadd = UserList.__iadd__
     __super_imul = UserList.__imul__
     __super_append = UserList.append
@@ -61,15 +63,16 @@
             result = self.__super_getitem(item)
             if isinstance(item, slice):
                 result = self.__class__(result)
             return result
 
     if sys.version_info[:3] < (3, 7, 4):  # pragma: no cover
         # Likewise for __copy__.
-        # See https://github.com/python/cpython/commit/3645d29a1dc2102fdb0f5f0c0129ff2295bcd768
+        # See
+        # https://github.com/python/cpython/commit/3645d29a1dc2102fdb0f5f0c0129ff2295bcd768
         def __copy__(self):
             inst = self.__class__.__new__(self.__class__)
             inst.__dict__.update(self.__dict__)
             # Create a copy and avoid triggering descriptors
             inst.__dict__["data"] = self.__dict__["data"][:]
             return inst
```

### Comparing `persistent-5.2/src/persistent/mapping.py` & `persistent-6.0/src/persistent/mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE
 #
 ##############################################################################
 
 """Python implementation of persistent base types."""
-import persistent
 from collections import UserDict as IterableUserDict
 
+import persistent
+
+
 class default:
 
     def __init__(self, func):
         self.func = func
 
     def __get__(self, inst, class_):
         if inst is None:
@@ -48,21 +50,21 @@
     __super_setitem = IterableUserDict.__setitem__
     __super_clear = IterableUserDict.clear
     __super_update = IterableUserDict.update
     __super_setdefault = IterableUserDict.setdefault
     __super_pop = IterableUserDict.pop
     __super_popitem = IterableUserDict.popitem
 
-
-    # Be sure to make a deep copy of our ``data`` (See PersistentList.)
-    # See https://github.com/python/cpython/commit/3645d29a1dc2102fdb0f5f0c0129ff2295bcd768
+    # Be sure to make a deep copy of our ``data`` (See PersistentList.) See
+    # https://github.com/python/cpython/commit/3645d29a1dc2102fdb0f5f0c0129ff2295bcd768
     # This was fixed in CPython 3.7.4, but we can't rely on that because it
-    # doesn't handle our old ``_container`` appropriately (it goes directly
-    # to ``self.__dict__``, bypassing the descriptor). The code here was initially
+    # doesn't handle our old ``_container`` appropriately (it goes directly to
+    # ``self.__dict__``, bypassing the descriptor). The code here was initially
     # based on the version found in 3.7.4.
+
     def __copy__(self):
         inst = self.__class__.__new__(self.__class__)
         inst.__dict__.update(self.__dict__)
         # Create a copy and avoid triggering descriptors
         if '_container' in inst.__dict__:
             # BWC for ZODB < 3.3.
             data = inst.__dict__.pop('_container')
@@ -135,15 +137,15 @@
 
     # Old implementations (prior to 2001; see
     # https://github.com/zopefoundation/ZODB/commit/c64281cf2830b569eed4f211630a8a61d22a0f0b#diff-b0f568e20f51129c10a096abad27c64a)
     # used ``_container`` rather than ``data``. Use a descriptor to provide
     # ``data`` when we have ``_container`` instead
 
     @default
-    def data(self): # pylint:disable=method-hidden
+    def data(self):
         # We don't want to cause a write on read, so we're careful not to
         # do anything that would cause us to become marked as changed, however,
         # if we're modified, then the saved record will have data, not
         # _container.
         data = self.__dict__.pop('_container')
         self.__dict__['data'] = data
```

### Comparing `persistent-5.2/src/persistent/persistence.py` & `persistent-6.0/src/persistent/persistence.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,38 +7,32 @@
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
+import copyreg
 import struct
+from sys import intern
 
 from zope.interface import implementer
+
 from persistent import interfaces
+from persistent._compat import use_c_impl
 from persistent.interfaces import SERIAL_TYPE
-from persistent.timestamp import TimeStamp
 from persistent.timestamp import _ZERO
-import copyreg
-from sys import intern
-from persistent._compat import use_c_impl
+from persistent.timestamp import TimeStamp
+
 
 __all__ = [
     'Persistent',
     'PersistentPy',
 ]
 
-# We use implementation details of PickleCachePy
-# pylint:disable=protected-access
-# we have lots of not-quite-correct continuation indentation.
-# TODO: Fix that in a whitespace-only commit.
-# pylint:disable=bad-continuation
-# There are a few places we need to work with exact types.
-# pylint:disable=unidiomatic-typecheck
-
 _INITIAL_SERIAL = _ZERO
 
 
 # Bitwise flags
 _CHANGED = 0x0001
 _STICKY = 0x0002
 
@@ -72,15 +66,14 @@
 
 # Represent 8-byte OIDs as hex integer, just like
 # ZODB does.
 _OID_STRUCT = struct.Struct('>Q')
 _OID_UNPACK = _OID_STRUCT.unpack
 
 
-
 @use_c_impl
 @implementer(interfaces.IPersistent)
 class Persistent:
     """ Pure Python implmentation of Persistent base class
     """
     __slots__ = _SLOTS
 
@@ -128,15 +121,15 @@
         return _OGA(self, '_Persistent__oid')
 
     def _set_oid(self, value):
         if value == _OGA(self, '_Persistent__oid'):
             return
         # The C implementation allows *any* value to be
         # used as the _p_oid.
-        #if value is not None:
+        # if value is not None:
         #    if not isinstance(value, OID_TYPE):
         #        raise ValueError('Invalid OID type: %s' % value)
         # The C implementation only forbids changing the OID
         # if we're in a cache, regardless of what the current
         # value or jar is
         if self._p_is_in_cache():
             # match the C error message
@@ -173,25 +166,25 @@
     _p_serial = property(_get_serial, _set_serial, _del_serial)
 
     # _p_changed:  see IPersistent.
     def _get_changed(self):
         if _OGA(self, '_Persistent__jar') is None:
             return False
         flags = _OGA(self, '_Persistent__flags')
-        if flags is None: # ghost
+        if flags is None:  # ghost
             return None
         return bool(flags & _CHANGED)
 
     def _set_changed(self, value):
         if _OGA(self, '_Persistent__flags') is None:
             if value:
                 self._p_activate()
                 self._p_set_changed_flag(value)
         else:
-            if value is None: # -> ghost
+            if value is None:  # -> ghost
                 self._p_deactivate()
             else:
                 self._p_set_changed_flag(value)
 
     def _del_changed(self):
         self._p_invalidate()
 
@@ -206,16 +199,17 @@
         serial = _OGA(self, '_Persistent__serial')
         return TimeStamp(serial).timeTime() if serial is not None else None
 
     _p_mtime = property(_get_mtime)
 
     # _p_state
     def _get_state(self):
-        # Note the use of OGA and caching to avoid recursive calls to __getattribute__:
-        # __getattribute__ calls _p_accessed calls cache.mru() calls _p_state
+        # Note the use of OGA and caching to avoid recursive calls to
+        # __getattribute__: __getattribute__ calls _p_accessed calls
+        # cache.mru() calls _p_state
         if _OGA(self, '_Persistent__jar') is None:
             return interfaces.UPTODATE
         flags = _OGA(self, '_Persistent__flags')
         if flags is None:
             return interfaces.GHOST
         if flags & _CHANGED:
             result = interfaces.CHANGED
@@ -248,14 +242,15 @@
     # The '_p_sticky' property is not (yet) part of the API:  for now,
     # it exists to simplify debugging and testing assertions.
     def _get_sticky(self):
         flags = _OGA(self, '_Persistent__flags')
         if flags is None:
             return False
         return bool(flags & _STICKY)
+
     def _set_sticky(self, value):
         flags = _OGA(self, '_Persistent__flags')
         if flags is None:
             raise ValueError('Ghost')
         if value:
             flags |= _STICKY
         else:
@@ -281,15 +276,15 @@
 
     # Methods from IPersistent.
     def __getattribute__(self, name):
         """ See IPersistent.
         """
         oga = _OGA
         if (not name.startswith('_p_') and
-            name not in _SPECIAL_NAMES):
+                name not in _SPECIAL_NAMES):
             if oga(self, '_Persistent__flags') is None:
                 oga(self, '_p_activate')()
             oga(self, '_p_accessed')()
         return oga(self, name)
 
     def __setattr__(self, name, value):
         special_name = (name in _SPECIAL_WRITE_NAMES or
@@ -300,15 +295,15 @@
                 _OGA(self, '_p_activate')()
             if not volatile:
                 _OGA(self, '_p_accessed')()
         _OSA(self, name, value)
         if (_OGA(self, '_Persistent__jar') is not None and
             _OGA(self, '_Persistent__oid') is not None and
             not special_name and
-            not volatile):
+                not volatile):
             before = _OGA(self, '_Persistent__flags')
             after = before | _CHANGED
             if before != after:
                 _OSA(self, '_Persistent__flags', after)
                 _OGA(self, '_p_register')()
 
     def __delattr__(self, name):
@@ -319,38 +314,37 @@
                 _OGA(self, '_p_activate')()
             _OGA(self, '_p_accessed')()
             before = _OGA(self, '_Persistent__flags')
             after = before | _CHANGED
             if before != after:
                 _OSA(self, '_Persistent__flags', after)
                 if (_OGA(self, '_Persistent__jar') is not None and
-                    _OGA(self, '_Persistent__oid') is not None):
+                        _OGA(self, '_Persistent__oid') is not None):
                     _OGA(self, '_p_register')()
         _ODA(self, name)
 
     def _slotnames(self, _v_exclude=True):
         slotnames = copyreg._slotnames(type(self))
         return [x for x in slotnames
-                   if not x.startswith('_p_') and
-                      not (x.startswith('_v_') and _v_exclude) and
-                      not x.startswith('_Persistent__') and
-                      x not in _SLOTS]
+                if not x.startswith('_p_') and
+                not (x.startswith('_v_') and _v_exclude) and
+                not x.startswith('_Persistent__') and
+                x not in _SLOTS]
 
     def __getstate__(self):
         """ See IPersistent.
         """
         idict = getattr(self, '__dict__', None)
         slotnames = self._slotnames()
         if idict is not None:
-            # TODO: Convert to a dictionary comprehension, avoid the intermediate
-            # list.
-            # pylint:disable=consider-using-dict-comprehension
+            # TODO: Convert to a dictionary comprehension, avoid the
+            # intermediate list.
             d = dict([x for x in idict.items()
-                         if not x[0].startswith('_p_') and
-                            not x[0].startswith('_v_')])
+                      if not x[0].startswith('_p_') and
+                      not x[0].startswith('_v_')])
         else:
             d = None
         if slotnames:
             s = {}
             for slotname in slotnames:
                 value = getattr(self, slotname, self)
                 if value is not self:
@@ -369,15 +363,15 @@
         if inst_dict is not None:
             if idict is None:
                 raise TypeError('No instance dict')
             idict.clear()
             for k, v in inst_dict.items():
                 # Normally the keys for instance attributes are interned.
                 # Do that here, but only if it is possible to do so.
-                idict[intern(k) if type(k) is str else k] = v
+                idict[intern(k) if k.__class__ is str else k] = v
         slotnames = self._slotnames()
         if slotnames:
             for k, v in slots.items():
                 setattr(self, k, v)
 
     def __reduce__(self):
         """ See IPersistent.
@@ -387,15 +381,15 @@
                 (type(self),) + gna(), self.__getstate__())
 
     def _p_activate(self):
         """ See IPersistent.
         """
         oga = _OGA
         before = oga(self, '_Persistent__flags')
-        if before is None: # Only do this if we're a ghost
+        if before is None:  # Only do this if we're a ghost
             # Begin by marking up-to-date in case we bail early
             _OSA(self, '_Persistent__flags', 0)
             jar = oga(self, '_Persistent__jar')
             if jar is None:
                 return
             oid = oga(self, '_Persistent__oid')
             if oid is None:
@@ -407,22 +401,22 @@
             # prevent this, but the C implementation sets it to changed
             # while calling jar.setstate, and this is observable to clients).
             # The main point of this is to prevent changes made during
             # setstate from registering the object with the jar.
             _OSA(self, '_Persistent__flags', interfaces.CHANGED)
             try:
                 jar.setstate(self)
-            except:
+            except BaseException:
                 _OSA(self, '_Persistent__flags', before)
                 raise
             else:
                 # If we succeed, no matter what the implementation
                 # of setstate did, mark ourself as up-to-date. The
                 # C implementation unconditionally does this.
-                _OSA(self, '_Persistent__flags', 0) # up-to-date
+                _OSA(self, '_Persistent__flags', 0)  # up-to-date
 
     # In the C implementation, _p_invalidate winds up calling
     # _p_deactivate. There are ZODB tests that depend on this;
     # it's not documented but there may be code in the wild
     # that does as well
 
     def _p_deactivate(self):
@@ -459,29 +453,30 @@
             # for backward-compatibility reason we release __slots__ only if
             # class does not override __new__
             if type_.__new__ is Persistent.__new__:
                 for slotname in Persistent._slotnames(self, _v_exclude=False):
                     try:
                         getattr(type_, slotname).__delete__(self)
                     except AttributeError:
-                        # AttributeError means slot variable was not initialized at all -
-                        # - we can simply skip its deletion.
+                        # AttributeError means slot variable was not
+                        # initialized at all - we can simply skip its deletion.
                         pass
 
         # Implementation detail: deactivating/invalidating
         # updates the size of the cache (if we have one)
         # by telling it this object no longer takes any bytes
         # (-1 is a magic number to compensate for the implementation,
         # which always adds one to the size given)
         try:
             cache = jar._cache
         except AttributeError:
             pass
         else:
-            cache.update_object_size_estimation(_OGA(self, '_Persistent__oid'), -1)
+            cache.update_object_size_estimation(
+                _OGA(self, '_Persistent__oid'), -1)
             # See notes in PickleCache.sweep for why we have to do this
             cache._persistent_deactivate_ran = True
 
     def _p_getattr(self, name):
         """ See IPersistent.
         """
         if name.startswith('_p_') or name in _SPECIAL_NAMES:
@@ -500,15 +495,16 @@
         self._p_accessed()
         return False
 
     def _p_delattr(self, name):
         """ See IPersistent.
         """
         if name.startswith('_p_'):
-            if name == '_p_oid' and self._p_is_in_cache(_OGA(self, '_Persistent__jar')):
+            if name == '_p_oid' and self._p_is_in_cache(
+                    _OGA(self, '_Persistent__jar')):
                 # The C implementation forbids deleting the oid
                 # if we're already in a cache. Match its error message
                 raise ValueError('can not change _p_jar of cached object')
 
             _ODA(self, name)
             return True
         self._p_activate()
@@ -530,15 +526,14 @@
                 self._p_register()
             _OSA(self, '_Persistent__flags', after)
         else:
             flags = _OGA(self, '_Persistent__flags')
             flags &= ~_CHANGED
             _OSA(self, '_Persistent__flags', flags)
 
-
     def _p_accessed(self):
         # Notify the jar's pickle cache that we have been accessed.
         # This relies on what has been (until now) an implementation
         # detail, the '_cache' attribute of the jar.  We made it a
         # private API to avoid the cycle of keeping a reference to
         # the cache on the persistent object.
 
@@ -554,43 +549,40 @@
         jar = oga(self, '_Persistent__jar')
         if jar is None:
             return
         oid = oga(self, '_Persistent__oid')
         if oid is None:
             return
         flags = oga(self, '_Persistent__flags')
-        if flags is None: # ghost
+        if flags is None:  # ghost
             return
 
-
         # The KeyError arises in ZODB: ZODB.serialize.ObjectWriter
         # can assign a jar and an oid to newly seen persistent objects,
         # but because they are newly created, they aren't in the
         # pickle cache yet. There doesn't seem to be a way to distinguish
         # that at this level, all we can do is catch it.
         # The AttributeError arises in ZODB test cases
         try:
             jar._cache.mru(oid)
         except (AttributeError, KeyError):
             pass
 
-
     def _p_is_in_cache(self, jar=None):
         oid = _OGA(self, '_Persistent__oid')
         if not oid:
             return False
 
         jar = jar or _OGA(self, '_Persistent__jar')
         cache = getattr(jar, '_cache', None)
         if cache is not None:
             return cache.get(oid) is self
         return None
 
     def __repr__(self):
-        # pylint:disable=broad-except
         p_repr_str = ''
         p_repr = getattr(type(self), '_p_repr', None)
         if p_repr is not None:
             try:
                 return p_repr(self)
             except Exception as e:
                 p_repr_str = ' _p_repr {!r}'.format(e)
@@ -612,25 +604,26 @@
 
         if jar is not None:
             try:
                 jar_str = ' in {!r}'.format(jar)
             except Exception as e:
                 jar_str = ' in {!r}'.format(e)
 
+        cls = self.__class__
         return '<{}.{} object at 0x{:x}{}{}{}>'.format(
             # Match the C name for this exact class
-            type(self).__module__ if type(self) is not Persistent else 'persistent',
-            type(self).__name__ if type(self) is not Persistent else 'Persistent',
+            'persistent' if cls is Persistent else cls.__module__,
+            'Persistent' if cls is Persistent else cls.__name__,
             id(self),
             oid_str, jar_str, p_repr_str
         )
 
 
 def _estimated_size_in_24_bits(value):
     if value > 1073741696:
         return 16777215
-    return (value//64) + 1
+    return (value // 64) + 1
 
 
-# This name is bound by the ``@use_c_impl`` decorator to the class defined above.
-# We make sure and list it statically, though, to help out linters.
-PersistentPy = PersistentPy # pylint:disable=undefined-variable,self-assigning-variable
+# This name is bound by the ``@use_c_impl`` decorator to the class defined
+# above. We make sure and list it statically, though, to help out linters.
+PersistentPy = PersistentPy  # noqa: F821 undefined name 'PersistentPy'
```

### Comparing `persistent-5.2/src/persistent/picklecache.py` & `persistent-6.0/src/persistent/picklecache.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,42 +8,36 @@
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 import gc
-
 from weakref import WeakValueDictionary
 
-from zope.interface import implementer
 from zope.interface import classImplements
+from zope.interface import implementer
 
-from persistent._compat import use_c_impl
 from persistent._compat import PYPY
+from persistent._compat import use_c_impl
 from persistent.interfaces import GHOST
-from persistent.interfaces import IPickleCache
-from persistent.interfaces import IExtendedPickleCache
 from persistent.interfaces import OID_TYPE
 from persistent.interfaces import UPTODATE
+from persistent.interfaces import IExtendedPickleCache
+from persistent.interfaces import IPickleCache
 from persistent.persistence import PersistentPy
 from persistent.persistence import _estimated_size_in_24_bits
 from persistent.ring import Ring
 
+
 __all__ = [
     'PickleCache',
     'PickleCachePy',
 ]
 
-# We're tightly coupled to the PersistentPy implementation and access
-# its internals.
-# pylint:disable=protected-access
-
-
-
 _OGA = object.__getattribute__
 _OSA = object.__setattr__
 
 
 def _sweeping_ring(f):
     # A decorator for functions in the PickleCache
     # that are sweeping the entire ring (mutating it);
@@ -55,27 +49,26 @@
             return f(self, *args, **kwargs)
         finally:
             self._is_sweeping_ring = False
     return locked
 
 
 class _WeakValueDictionary:
-    # Maps from OID -> Persistent object, but
-    # only weakly references the Persistent object. This is similar
-    # to ``weakref.WeakValueDictionary``, but is customized depending on the
-    # platform. On PyPy, all objects can cheaply use a WeakRef, so that's
-    # what we actually use. On CPython, though, ``PersistentPy`` cannot be weakly
-    # referenced, so we rely on the fact that the ``id()`` of an object is its
-    # memory location, and we use ``ctypes`` to cast that integer back to
-    # the object.
+    # Maps from OID -> Persistent object, but only weakly references the
+    # Persistent object. This is similar to ``weakref.WeakValueDictionary``,
+    # but is customized depending on the platform. On PyPy, all objects can
+    # cheaply use a WeakRef, so that's what we actually use. On CPython,
+    # though, ``PersistentPy`` cannot be weakly referenced, so we rely on the
+    # fact that the ``id()`` of an object is its memory location, and we use
+    # ``ctypes`` to cast that integer back to the object.
     #
-    # To remove stale addresses, we rely on the ``ffi.gc()`` object with the exact
-    # same lifetime as the ``PersistentPy`` object. It calls us, we get the ``id``
-    # back out of the CData, and clean up.
-    if PYPY: # pragma: no cover
+    # To remove stale addresses, we rely on the ``ffi.gc()`` object with the
+    # exact same lifetime as the ``PersistentPy`` object. It calls us, we get
+    # the ``id`` back out of the CData, and clean up.
+    if PYPY:  # pragma: no cover
         def __init__(self):
             self._data = WeakValueDictionary()
 
         def _from_addr(self, addr):
             return addr
 
         def _save_addr(self, oid, obj):
@@ -203,16 +196,22 @@
         # the ZODB tests depend on this
 
         # The C impl requires either a type or a Persistent subclass
         if not isinstance(value, self._CACHEABLE_TYPES):
             raise TypeError("Cache values must be persistent objects.")
 
         value_oid = value._p_oid
-        if not isinstance(oid, OID_TYPE) or not isinstance(value_oid, OID_TYPE):
-            raise TypeError('OID must be {}: key={} _p_oid={}'.format(OID_TYPE, oid, value_oid))
+        if not isinstance(
+                oid,
+                OID_TYPE) or not isinstance(
+                value_oid,
+                OID_TYPE):
+            raise TypeError(
+                'OID must be {}: key={} _p_oid={}'.format(
+                    OID_TYPE, oid, value_oid))
 
         if value_oid != oid:
             raise ValueError("Cache key does not match oid")
 
         if oid in self.persistent_classes or oid in self.data:
             # Have to be careful here, a GC might have just run
             # and cleaned up the object
@@ -223,21 +222,21 @@
                 raise ValueError('A different object already has the same oid')
         # Match the C impl: it requires a jar. Let this raise AttributeError
         # if no jar is found.
         jar = value._p_jar
         if jar is None:
             raise ValueError("Cached object jar missing")
         # It also requires that it cannot be cached more than one place
-        existing_cache = getattr(jar, '_cache', None) # type: PickleCache
+        existing_cache = getattr(jar, '_cache', None)  # type: PickleCache
         if (existing_cache is not None
                 and existing_cache is not self
                 and oid in existing_cache.data):
             raise ValueError("Cache values may only be in one cache.")
 
-        if isinstance(value, type): # ZODB.persistentclass.PersistentMetaClass
+        if isinstance(value, type):  # ZODB.persistentclass.PersistentMetaClass
             self.persistent_classes[oid] = value
         else:
             self.data[oid] = value
             if _OGA(value, '_p_state') != GHOST and value not in self.ring:
                 self.ring.add(value)
                 self.non_ghost_count += 1
             elif self.data.cleanup_hook:
@@ -267,15 +266,15 @@
     def mru(self, oid):
         """ See IPickleCache.
         """
         if self._is_sweeping_ring:
             # accessess during sweeping, such as with an
             # overridden _p_deactivate, don't mutate the ring
             # because that could leave it inconsistent
-            return False # marker return for tests
+            return False  # marker return for tests
 
         value = self.data[oid]
 
         was_in_ring = value in self.ring
         if not was_in_ring:
             if _OGA(value, '_p_state') != GHOST:
                 self.ring.add(value)
@@ -347,15 +346,15 @@
                 # testConnection.doctest_proper_ghost_initialization_with_empty__p_deactivate
                 obj._p_invalidate_deactivate_helper(False)
         self[oid] = obj
 
     def reify(self, to_reify):
         """ See IPickleCache.
         """
-        if isinstance(to_reify, OID_TYPE): #bytes
+        if isinstance(to_reify, OID_TYPE):  # bytes
             to_reify = [to_reify]
         for oid in to_reify:
             value = self[oid]
             if value._p_state == GHOST:
                 value._p_activate()
                 self.non_ghost_count += 1
                 self.mru(oid)
@@ -426,53 +425,54 @@
     # cache's dictionary). We're trying to keep that to a minimum, but
     # there's no way around it if we want full compatibility.
     _persistent_deactivate_ran = False
 
     @_sweeping_ring
     def _sweep(self, target, target_size_bytes=0):
         ejected = 0
-        # If we find and eject objects that may have been weak referenced,
-        # we need to run a garbage collection to try to clear those references.
-        # Otherwise, it's highly likely that accessing those objects through those
-        # references will try to ``_p_activate()`` them, and since the jar they came
-        # from is probably closed, that will lead to an error. See
-        # https://github.com/zopefoundation/persistent/issues/149
+        # If we find and eject objects that may have been weak referenced, we
+        # need to run a garbage collection to try to clear those references.
+        # Otherwise, it's highly likely that accessing those objects through
+        # those references will try to ``_p_activate()`` them, and since the
+        # jar they came from is probably closed, that will lead to an error.
+        # See https://github.com/zopefoundation/persistent/issues/149
         had_weak_refs = False
         ring = self.ring
         for node, value in ring.iteritems():
-            if ((target or target_size_bytes) # pylint:disable=too-many-boolean-expressions
+            if ((target or target_size_bytes)
                     and (not target or self.non_ghost_count <= target)
                     and (self.total_estimated_size <= target_size_bytes
                          or not target_size_bytes)):
                 break
 
             if value._p_state == UPTODATE:
-                # The C implementation will only evict things that are specifically
-                # in the up-to-date state
+                # The C implementation will only evict things that are
+                # specifically in the up-to-date state
                 self._persistent_deactivate_ran = False
 
                 # sweeping an object out of the cache should also
                 # ghost it---that's what C does. This winds up
                 # calling `update_object_size_estimation`.
                 # Also in C, if this was the last reference to the object,
                 # it removes itself from the `data` dictionary.
                 # If we're under PyPy or Jython, we need to run a GC collection
-                # to make this happen...this is only noticeable though, when
-                # we eject objects. Also, note that we can only take any of these
-                # actions if our _p_deactivate ran, in case of buggy subclasses.
-                # see _persistent_deactivate_ran.
+                # to make this happen...this is only noticeable though, when we
+                # eject objects. Also, note that we can only take any of these
+                # actions if our _p_deactivate ran, in case of buggy
+                # subclasses. see _persistent_deactivate_ran.
 
                 if not had_weak_refs:
-                    had_weak_refs |= getattr(value, '__weakref__', None) is not None
+                    had_weak_refs |= getattr(
+                        value, '__weakref__', None) is not None
 
                 value._p_deactivate()
                 if (self._persistent_deactivate_ran
-                        # Test-cases sneak in non-Persistent objects, sigh, so naturally
-                        # they don't cooperate (without this check a bunch of test_picklecache
-                        # breaks)
+                        # Test-cases sneak in non-Persistent objects, sigh, so
+                        # naturally they don't cooperate (without this check a
+                        # bunch of test_picklecache breaks)
                         or not isinstance(value, self._SWEEPABLE_TYPES)):
                     ring.delete_node(node)
                     ejected += 1
                     self.non_ghost_count -= 1
 
         if ejected and had_weak_refs:
             # Clear the iteration variables, so the objects they point to
@@ -496,11 +496,11 @@
                 # have this method and it must be called for transaction abort
                 # and other forms of invalidation to work
                 persistent_class._p_invalidate()
             except AttributeError:
                 pass
 
 
-# This name is bound by the ``@use_c_impl`` decorator to the class defined above.
-# We make sure and list it statically, though, to help out linters.
-PickleCachePy = PickleCachePy # pylint:disable=undefined-variable,self-assigning-variable
+# This name is bound by the ``@use_c_impl`` decorator to the class defined
+# above. We make sure and list it statically, though, to help out linters.
+PickleCachePy = PickleCachePy  # noqa: F821 undefined name 'PickleCachePy'
 classImplements(PickleCachePy, IExtendedPickleCache)
```

### Comparing `persistent-5.2/src/persistent/ring.c` & `persistent-6.0/src/persistent/ring.c`

 * *Files identical despite different names*

### Comparing `persistent-5.2/src/persistent/ring.h` & `persistent-6.0/src/persistent/ring.h`

 * *Files identical despite different names*

### Comparing `persistent-5.2/src/persistent/ring.py` & `persistent-6.0/src/persistent/ring.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,55 +8,54 @@
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 
-# pylint:disable=inherit-non-class,no-self-argument,redefined-builtin,c-extension-no-member
-# pylint:disable=protected-access
-
 from zope.interface import Interface
 from zope.interface import implementer
 
 from persistent import _ring
 
+
 class IRing(Interface):
-    """Conceptually, a doubly-linked list for efficiently keeping track of least-
-    and most-recently used :class:`persistent.interfaces.IPersistent` objects.
+    """Conceptually, a doubly-linked list for efficiently keeping track of
+    least- and most-recently used :class:`persistent.interfaces.IPersistent`
+    objects.
 
     This is meant to be used by the :class:`persistent.picklecache.PickleCache`
-    and should not be considered a public API. This interface documentation exists
-    to assist development of the picklecache and alternate implementations by
-    explaining assumptions and performance requirements.
+    and should not be considered a public API. This interface documentation
+    exists to assist development of the picklecache and alternate
+    implementations by explaining assumptions and performance requirements.
     """
 
-    def __len__(): # pylint:disable=no-method-argument
+    def __len__():
         """Return the number of persistent objects stored in the ring.
 
         Should be constant time.
         """
 
-    def __contains__(object): # pylint:disable=unexpected-special-method-signature
+    def __contains__(object):
         """Answer whether the given persistent object is found in the ring.
 
         Must not rely on object equality or object hashing, but only
         identity or the `_p_oid`. Should be constant time.
         """
 
     def add(object):
         """Add the persistent object to the ring as most-recently used.
 
         When an object is in the ring, the ring holds a strong
         reference to it so it can be deactivated later by the pickle
         cache. Should be constant time.
 
-        The object should not already be in the ring, but this is not necessarily
-        enforced.
-		"""
+        The object should not already be in the ring, but this is not
+        necessarily enforced.
+        """
 
     def delete(object):
         """Remove the object from the ring if it is present.
 
         Returns a true value if it was present and a false value
         otherwise. An ideal implementation should be constant time,
         but linear time is allowed.
@@ -68,31 +67,32 @@
         The object should already be in the ring, but this is not
         necessarily enforced, and attempting to move an object that is
         not in the ring has undefined consequences. An ideal
         implementation should be constant time, but linear time is
         allowed.
         """
 
-    def __iter__(): # pylint:disable=no-method-argument
-        """Iterate over each persistent object in the ring, in the order of least
-        recently used to most recently used.
+    def __iter__():
+        """Iterate over each persistent object in the ring, in the order of
+        least recently used to most recently used.
 
         Mutating the ring while an iteration is in progress has
         undefined consequences.
         """
 
 
 ffi = _ring.ffi
 _FFI_RING = _ring.lib
 
 _OGA = object.__getattribute__
 _OSA = object.__setattr__
 
 _handles = set()
 
+
 @implementer(IRing)
 class _CFFIRing:
     """A ring backed by a C implementation. All operations are constant time.
 
     It is only available on platforms with ``cffi`` installed.
     """
 
@@ -106,17 +106,17 @@
         self.cleanup_func = cleanup_func
 
         # The Persistent objects themselves are responsible for keeping
         # the CFFI nodes alive, but we need to be able to detect whether
         # or not any given object is in our ring, plus know how many there are.
         # In addition, once an object enters the ring, it must be kept alive
         # so that it can be deactivated.
-        # Note that because this is a strong reference to the
-        # persistent object, its cleanup function --- triggered by the ``ffi.gc``
-        # object it owns --- will never be fired while it is in this dict.
+        # Note that because this is a strong reference to the persistent
+        # object, its cleanup function --- triggered by the ``ffi.gc`` object
+        # it owns --- will never be fired while it is in this dict.
         self.ring_to_obj = {}
 
     def ring_node_for(self, persistent_object, create=True):
         ring_data = _OGA(persistent_object, '_Persistent__ring')
         if ring_data is None:
             if not create:
                 return None
@@ -175,14 +175,14 @@
             # yielding, just in case the current value is
             # removed.
             current = here
             here = here.r_next
             pobj = ring_to_obj[current]
             yield current, pobj
 
-
     def __iter__(self):
         for _, v in self.iteritems():
             yield v
 
+
 # Export the best available implementation
 Ring = _CFFIRing
```

### Comparing `persistent-5.2/src/persistent/tests/attrhooks.py` & `persistent-6.0/src/persistent/tests/attrhooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,38 +14,42 @@
 """Overriding attr methods
 
 Examples for overriding attribute access methods.
 """
 
 from persistent import Persistent
 
+
 def _resettingJar():
     from persistent.tests.utils import ResettingJar
     return ResettingJar()
 
+
 def _rememberingJar():
     from persistent.tests.utils import RememberingJar
     return RememberingJar()
 
 
 class OverridesGetattr(Persistent):
     """Example of overriding __getattr__
     """
+
     def __getattr__(self, name):
         """Get attributes that can't be gotten the usual way
         """
         # Don't pretend we have any special attributes.
         if name.startswith("__") and name.endswrith("__"):
-            raise AttributeError(name) # pragma: no cover
+            raise AttributeError(name)  # pragma: no cover
         return name.upper(), self._p_changed
 
 
 class VeryPrivate(Persistent):
     """Example of overriding __getattribute__, __setattr__, and __delattr__
     """
+
     def __init__(self, **kw):
         self.__dict__['__secret__'] = kw.copy()
 
     def __getattribute__(self, name):
         """Get an attribute value
 
         See the very important note in the comment below!
@@ -73,15 +77,14 @@
         # Maybe it's a method:
         meth = getattr(self.__class__, name, None)
         if meth is None:
             raise AttributeError(name)
 
         return meth.__get__(self, self.__class__)
 
-
     def __setattr__(self, name, value):
         """Set an attribute value
         """
         #################################################################
         # IMPORTANT! READ THIS! 8->
         #
         # We *always* give Persistent a chance first.
```

### Comparing `persistent-5.2/src/persistent/tests/cucumbers.py` & `persistent-6.0/src/persistent/tests/cucumbers.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,30 +11,33 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 # Example objects for pickling.
 
 from persistent import Persistent
 
+
 def print_dict(d):
     d = sorted(d.items())
     print('{%s}' % (', '.join(
         [('{!r}: {!r}'.format(k, v)) for (k, v) in d]
-        )))
+    )))
+
 
 def cmpattrs(self, other, *attrs):
     result = 0
     for attr in attrs:
         if attr[:3] in ('_v_', '_p_'):
             raise AssertionError("_v_ and _p_ attrs not allowed")
         lhs = getattr(self, attr, None)
         rhs = getattr(other, attr, None)
         result += lhs != rhs
     return result
 
+
 class Simple(Persistent):
     def __init__(self, name, **kw):
         self.__name__ = name
         self.__dict__.update(kw)
         self._v_favorite_color = 'blue'
         self._p_foo = 'bar'
```

### Comparing `persistent-5.2/src/persistent/tests/test__compat.py` & `persistent-6.0/src/persistent/tests/test__compat.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,32 +12,33 @@
 #
 ##############################################################################
 """
 Tests for ``persistent._compat``
 
 """
 
-import unittest
 import os
+import unittest
 
 from persistent import _compat as compat
 
+
 class TestCOptimizationsFuncs(unittest.TestCase):
-    # pylint:disable=protected-access
+
     def setUp(self):
         self.env_val = os.environ.get('PURE_PYTHON', self)
         self.orig_pypy = compat.PYPY
         compat.PYPY = False
 
     def tearDown(self):
         compat.PYPY = self.orig_pypy
         if self.env_val is not self:
             # Reset to what it was to begin with.
             os.environ['PURE_PYTHON'] = self.env_val
-        else: # pragma: no cover
+        else:  # pragma: no cover
             # It wasn't present before, make sure it's not present now.
             os.environ.pop('PURE_PYTHON', None)
 
         self.env_val = None
 
     def _set_env(self, val):
         if val is not None:
@@ -85,21 +86,23 @@
                 (None, True),
                 ('', True),
                 ('0', True),
                 ('1', False),
                 ('Yes', False)
         ):
             self._set_env(val)
-            self.assertEqual(expected, compat._should_attempt_c_optimizations())
+            self.assertEqual(
+                expected, compat._should_attempt_c_optimizations())
 
     def test_should_attempt_pypy(self):
         compat.PYPY = True
         for val, expected in (
                 (None, False),
                 ('', False),
                 ('0', True),
                 ('1', False),
                 ('Yes', False)
         ):
             __traceback_info__ = val
             self._set_env(val)
-            self.assertEqual(expected, compat._should_attempt_c_optimizations())
+            self.assertEqual(
+                expected, compat._should_attempt_c_optimizations())
```

### Comparing `persistent-5.2/src/persistent/tests/test_compile_flags.py` & `persistent-6.0/src/persistent/tests/test_compile_flags.py`

 * *Files identical despite different names*

### Comparing `persistent-5.2/src/persistent/tests/test_docs.py` & `persistent-6.0/src/persistent/tests/test_docs.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,20 +12,17 @@
 #
 ##############################################################################
 """
 Tests for the documentation.
 """
 
 
-# disable: accessing protected members, too many methods
-# pylint: disable=W0212,R0904
-
+import doctest
 import os.path
 import unittest
-import doctest
 
 import manuel.capture
 import manuel.codeblock
 import manuel.doctest
 import manuel.ignore
 import manuel.testing
```

### Comparing `persistent-5.2/src/persistent/tests/test_list.py` & `persistent-6.0/src/persistent/tests/test_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,30 +12,30 @@
 #
 ##############################################################################
 """Tests for PersistentList
 """
 
 import unittest
 
-
 from persistent.tests.utils import TrivialJar
 from persistent.tests.utils import copy_test
 
 
 l0 = []
 l1 = [0]
 l2 = [0, 1]
 
-# pylint:disable=protected-access
 
 class OtherList:
     def __init__(self, initlist):
         self.__data = initlist
+
     def __len__(self):
         return len(self.__data)
+
     def __getitem__(self, i):
         return self.__data[i]
 
 
 class TestPList(unittest.TestCase):
 
     def _getTargetClass(self):
@@ -167,17 +167,17 @@
         uu2 = u2[:]
         del uu2[1:]
         del uu2[:1]
         eq(uu2, [], "uu2 == []")
 
         # Test __add__, __radd__, __mul__ and __rmul__
 
-        #self.assertTrue(u1 + [] == [] + u1 == u1, "u1 + [] == [] + u1 == u1")
+        # self.assertTrue(u1 + [] == [] + u1 == u1, "u1 + [] == [] + u1 == u1")
         self.assertTrue(u1 + [1] == u2, "u1 + [1] == u2")
-        #self.assertTrue([-1] + u1 == [-1, 0], "[-1] + u1 == [-1, 0]")
+        # self.assertTrue([-1] + u1 == [-1, 0], "[-1] + u1 == [-1, 0]")
         self.assertTrue(u2 == u2*1 == 1*u2, "u2 == u2*1 == 1*u2")
         self.assertTrue(u2+u2 == u2*2 == 2*u2, "u2+u2 == u2*2 == 2*u2")
         self.assertTrue(u2+u2+u2 == u2*3 == 3*u2, "u2+u2+u2 == u2*3 == 3*u2")
 
         # Test append
 
         u = u1[:]
@@ -206,15 +206,14 @@
 
         # Test count
         u = u2*3
         eq(u.count(0), 3, "u.count(0) == 3")
         eq(u.count(1), 3, "u.count(1) == 3")
         eq(u.count(2), 0, "u.count(2) == 0")
 
-
         # Test index
 
         eq(u2.index(0), 0, "u2.index(0) == 0")
         eq(u2.index(1), 1, "u2.index(1) == 1")
         with self.assertRaises(ValueError):
             u2.index(2)
 
@@ -384,14 +383,7 @@
         self.assertIsInstance(inst2, MyList)
         self.assertIsNone(inst2._p_jar)
 
     def test_copy(self):
         inst = self._makeOne()
         inst.append(42)
         copy_test(self, inst)
-
-
-def test_suite():
-    return unittest.defaultTestLoader.loadTestsFromName(__name__)
-
-if __name__ == '__main__':
-    unittest.main()
```

### Comparing `persistent-5.2/src/persistent/tests/test_mapping.py` & `persistent-6.0/src/persistent/tests/test_mapping.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,19 +9,17 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 import unittest
 
-
 from persistent.tests.utils import TrivialJar
 from persistent.tests.utils import copy_test
 
-# pylint:disable=blacklisted-name, protected-access
 
 class Test_default(unittest.TestCase):
 
     def _getTargetClass(self):
         from persistent.mapping import default
         return default
 
@@ -29,25 +27,27 @@
         return self._getTargetClass()(func)
 
     def test___get___from_class(self):
         def _test(inst):
             raise AssertionError("Must not be caled")
 
         descr = self._makeOne(_test)
+
         class Foo:
             testing = descr
         self.assertIs(Foo.testing, descr)
 
-
     def test___get___from_instance(self):
         _called_with = []
+
         def _test(inst):
             _called_with.append(inst)
             return 'TESTING'
         descr = self._makeOne(_test)
+
         class Foo:
             testing = descr
         foo = Foo()
         self.assertEqual(foo.testing, 'TESTING')
         self.assertEqual(_called_with, [foo])
 
 
@@ -73,30 +73,31 @@
         state = m.__getstate__()
         self.assertTrue('foo' in state)
         self.assertFalse('_v_baz' in state)
 
     def testTheWorld(self):
         # Test constructors
         l0 = {}
-        l1 = {0:0}
-        l2 = {0:0, 1:1}
+        l1 = {0: 0}
+        l2 = {0: 0, 1: 1}
         u = self._makeOne()
         u0 = self._makeOne(l0)
         u1 = self._makeOne(l1)
         u2 = self._makeOne(l2)
 
         uu = self._makeOne(u)
         uu0 = self._makeOne(u0)
         uu1 = self._makeOne(u1)
         uu2 = self._makeOne(u2)
 
         class OtherMapping(dict):
             def __init__(self, initmapping):
                 dict.__init__(self)
                 self.__data = initmapping
+
             def items(self):
                 raise AssertionError("Not called")
         self._makeOne(OtherMapping(u0))
         self._makeOne([(0, 0), (1, 1)])
 
         # Test __repr__
         eq = self.assertEqual
@@ -139,15 +140,15 @@
 
         # Test get
 
         for i in range(len(u2)):
             eq(u2.get(i), i, "u2.get(i) == i")
             eq(u2.get(i, 5), i, "u2.get(i, 5) == i")
 
-        for i in min(u2)-1, max(u2)+1:
+        for i in min(u2) - 1, max(u2) + 1:
             eq(u2.get(i), None, "u2.get(i) == None")
             eq(u2.get(i, 5), 5, "u2.get(i, 5) == 5")
 
         # Test __setitem__
 
         uu2[0] = 0
         uu2[1] = 100
@@ -159,25 +160,25 @@
         del uu2[0]
         with self.assertRaises(KeyError):
             del uu2[0]
 
         # Test __contains__
         for i in u2:
             self.assertTrue(i in u2, "i in u2")
-        for i in min(u2)-1, max(u2)+1:
+        for i in min(u2) - 1, max(u2) + 1:
             self.assertTrue(i not in u2, "i not in u2")
 
         # Test update
 
-        l = {"a":"b"}
-        u = self._makeOne(l)
+        l_ = {"a": "b"}
+        u = self._makeOne(l_)
         u.update(u2)
         for i in u:
-            self.assertTrue(i in l or i in u2, "i in l or i in u2")
-        for i in l:
+            self.assertTrue(i in l_ or i in u2, "i in l or i in u2")
+        for i in l_:
             self.assertTrue(i in u, "i in u")
         for i in u2:
             self.assertTrue(i in u, "i in u")
 
         # Test setdefault
 
         x = u2.setdefault(0, 5)
@@ -317,11 +318,7 @@
     def _getTargetClass(self):
         from persistent.dict import PersistentDict
         return PersistentDict
 
     def test_PD_is_alias_to_PM(self):
         from persistent.mapping import PersistentMapping
         self.assertIs(self._getTargetClass(), PersistentMapping)
-
-
-def test_suite():
-    return unittest.defaultTestLoader.loadTestsFromName(__name__)
```

### Comparing `persistent-5.2/src/persistent/tests/test_persistence.py` & `persistent-6.0/src/persistent/tests/test_persistence.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,27 +8,21 @@
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 
+import copyreg
 import re
 import unittest
+from collections import UserDict as IterableUserDict
 
-import copyreg
 from persistent._compat import PYPY
 from persistent.tests.utils import skipIfNoCExtension
-from collections import UserDict as IterableUserDict
-
-# pylint:disable=R0904,W0212,E1101
-# pylint:disable=attribute-defined-outside-init,too-many-lines
-# pylint:disable=blacklisted-name,useless-object-inheritance
-# Hundreds of unused jar and OID vars make this useless
-# pylint:disable=unused-variable
 
 
 class _Persistent_Base:
 
     def _getTargetClass(self):
         # concrete testcase classes must override
         raise NotImplementedError()
@@ -41,84 +35,95 @@
         return self._makeCache(jar)
 
     def _makeOne(self, *args, **kw):
         return self._getTargetClass()(*args, **kw)
 
     def _makeJar(self, real_cache=False):
         from zope.interface import implementer
+
         from persistent.interfaces import IPersistentDataManager
 
         @implementer(IPersistentDataManager)
         class _Jar:
             _cache = None
             # Set this to a value to have our `setstate`
             # pass it through to the object's __setstate__
             setstate_calls_object = None
 
             # Set this to a value to have our `setstate`
             # set the _p_serial of the object
             setstate_sets_serial = None
+
             def __init__(self):
                 self._loaded = []
                 self._registered = []
+
             def setstate(self, obj):
                 self._loaded.append(obj._p_oid)
                 if self.setstate_calls_object is not None:
                     obj.__setstate__(self.setstate_calls_object)
                 if self.setstate_sets_serial is not None:
                     obj._p_serial = self.setstate_sets_serial
+
             def register(self, obj):
                 self._registered.append(obj._p_oid)
 
         jar = _Jar()
-        jar._cache = self._makeRealCache(jar) if real_cache else self._makeCache(jar)
+        jar._cache = self._makeRealCache(
+            jar) if real_cache else self._makeCache(jar)
         return jar
 
     def _makeBrokenJar(self):
         from zope.interface import implementer
+
         from persistent.interfaces import IPersistentDataManager
 
         @implementer(IPersistentDataManager)
         class _BrokenJar:
             def __init__(self):
                 self.called = 0
+
             def register(self, ob):
                 self.called += 1
                 raise NotImplementedError()
+
             def setstate(self, ob):
                 raise NotImplementedError()
 
         jar = _BrokenJar()
         jar._cache = self._makeCache(jar)
         return jar
 
     def _makeOneWithJar(self, klass=None, broken_jar=False, real_cache=False):
         OID = b'\x01' * 8
         if klass is not None:
             inst = klass()
         else:
             inst = self._makeOne()
-        jar = self._makeJar(real_cache=real_cache) if not broken_jar else self._makeBrokenJar()
-        jar._cache.new_ghost(OID, inst) # assigns _p_jar, _p_oid
+        jar = self._makeJar(
+            real_cache=real_cache) if not broken_jar else self._makeBrokenJar()
+        jar._cache.new_ghost(OID, inst)  # assigns _p_jar, _p_oid
         # Be sure it really returned a ghost.
         assert inst._p_status == 'ghost'
         return inst, jar, OID
 
     def test_class_conforms_to_IPersistent(self):
         from zope.interface.verify import verifyClass
+
         from persistent.interfaces import IPersistent
         verifyClass(IPersistent, self._getTargetClass())
 
     def test_instance_conforms_to_IPersistent(self):
         from zope.interface.verify import verifyObject
+
         from persistent.interfaces import IPersistent
         verifyObject(IPersistent, self._makeOne())
 
     def test_instance_cannot_be_weakly_referenced(self):
-        if PYPY: # pragma: no cover
+        if PYPY:  # pragma: no cover
             self.skipTest('On PyPy, everything can be weakly referenced')
         import weakref
         inst = self._makeOne()
         with self.assertRaises(TypeError):
             weakref.ref(inst)
 
     def test_ctor(self):
@@ -134,14 +139,15 @@
     def test_del_jar_no_jar(self):
         inst = self._makeOne()
         del inst._p_jar  # does not raise
         self.assertEqual(inst._p_jar, None)
 
     def test_del_jar_while_in_cache(self):
         inst, _, OID = self._makeOneWithJar()
+
         def _test():
             del inst._p_jar
         self.assertRaises(ValueError, _test)
 
     def test_del_jar_like_ZODB_abort(self):
         # When a ZODB connection aborts, it removes registered objects from
         # the cache, deletes their jar, deletes their OID, and finally sets
@@ -180,15 +186,15 @@
 
     def test_assign_p_jar_w_valid_jar(self):
         jar = self._makeJar()
         inst = self._makeOne()
         inst._p_jar = jar
         self.assertEqual(inst._p_status, 'saved')
         self.assertTrue(inst._p_jar is jar)
-        inst._p_jar = jar # reassign only to same DM
+        inst._p_jar = jar  # reassign only to same DM
 
     def test_assign_p_jar_not_in_cache_allowed(self):
         jar = self._makeJar()
         inst = self._makeOne()
         inst._p_jar = jar
         # Both of these are allowed
         inst._p_jar = self._makeJar()
@@ -223,23 +229,24 @@
         inst._p_oid = OID1
         inst._p_oid = None
         self.assertEqual(inst._p_oid, None)
 
     def test_assign_p_oid_w_new_oid_w_jar(self):
         inst, jar, OID = self._makeOneWithJar()
         new_OID = b'\x02' * 8
+
         def _test():
             inst._p_oid = new_OID
         self.assertRaises(ValueError, _test)
 
     def test_assign_p_oid_not_in_cache_allowed(self):
         jar = self._makeJar()
         inst = self._makeOne()
         inst._p_jar = jar
-        inst._p_oid = 1 # anything goes
+        inst._p_oid = 1  # anything goes
         inst._p_oid = 42
         self.assertEqual(inst._p_oid, 42)
 
     def test_delete_p_oid_wo_jar(self):
         OID = b'\x01' * 8
         inst = self._makeOne()
         inst._p_oid = OID
@@ -268,32 +275,36 @@
         inst, jar, OID = self._makeOneWithJar()
         del jar._cache[OID]
         del inst._p_oid
         self.assertEqual(inst._p_oid, None)
 
     def test_assign_p_serial_w_invalid_type(self):
         inst = self._makeOne()
+
         def _test():
             inst._p_serial = object()
         self.assertRaises(ValueError, _test)
 
     def test_assign_p_serial_w_None(self):
         inst = self._makeOne()
+
         def _test():
             inst._p_serial = None
         self.assertRaises(ValueError, _test)
 
     def test_assign_p_serial_too_short(self):
         inst = self._makeOne()
+
         def _test():
             inst._p_serial = b'\x01\x02\x03'
         self.assertRaises(ValueError, _test)
 
     def test_assign_p_serial_too_long(self):
         inst = self._makeOne()
+
         def _test():
             inst._p_serial = b'\x01\x02\x03' * 3
         self.assertRaises(ValueError, _test)
 
     def test_assign_p_serial_w_valid_serial(self):
         SERIAL = b'\x01' * 8
         inst = self._makeOne()
@@ -360,30 +371,30 @@
         self.assertEqual(list(jar._loaded), [OID])
         self.assertEqual(list(jar._registered), [OID])
 
     def test_assign_p_changed_false_from_ghost(self):
         inst, jar, OID = self._makeOneWithJar()
         inst._p_deactivate()
         inst._p_changed = False
-        self.assertEqual(inst._p_status, 'ghost') # ??? this is what C does
+        self.assertEqual(inst._p_status, 'ghost')  # ??? this is what C does
         self.assertEqual(list(jar._loaded), [])
         self.assertEqual(list(jar._registered), [])
 
     def test_assign_p_changed_none_from_saved(self):
         inst, jar, OID = self._makeOneWithJar()
         inst._p_activate()
         jar._loaded = []
         inst._p_changed = None
         self.assertEqual(inst._p_status, 'ghost')
         self.assertEqual(list(jar._loaded), [])
         self.assertEqual(list(jar._registered), [])
 
     def test_assign_p_changed_true_from_saved(self):
         inst, jar, OID = self._makeOneWithJar()
-        inst._p_activate() # XXX
+        inst._p_activate()  # XXX
         jar._loaded[:] = []
         inst._p_changed = True
         self.assertEqual(inst._p_status, 'changed')
         self.assertEqual(list(jar._loaded), [])
         self.assertEqual(list(jar._registered), [OID])
 
     def test_assign_p_changed_false_from_saved(self):
@@ -427,15 +438,15 @@
         inst._p_changed = False
         self.assertEqual(inst._p_status, 'saved')
         self.assertEqual(list(jar._loaded), [])
         self.assertEqual(list(jar._registered), [])
 
     def test_assign_p_changed_none_when_sticky(self):
         inst, jar, OID = self._makeOneWithJar()
-        inst._p_activate() # XXX
+        inst._p_activate()  # XXX
         inst._p_changed = False
         inst._p_sticky = True
         inst._p_changed = None
         self.assertEqual(inst._p_status, 'sticky')
         self.assertEqual(inst._p_changed, False)
         self.assertEqual(inst._p_sticky, True)
 
@@ -480,46 +491,48 @@
         del inst._p_changed
         self.assertEqual(inst._p_status, 'ghost')
         self.assertEqual(list(jar._loaded), [])
         self.assertEqual(list(jar._registered), [])
 
     def test_delete_p_changed_when_sticky(self):
         inst, jar, OID = self._makeOneWithJar()
-        inst._p_activate() # XXX
+        inst._p_activate()  # XXX
         inst._p_changed = False
         inst._p_sticky = True
         del inst._p_changed
         self.assertEqual(inst._p_status, 'ghost')
         self.assertEqual(inst._p_changed, None)
         self.assertEqual(inst._p_sticky, False)
 
     def test_assign_p_sticky_true_when_ghost(self):
         inst, jar, OID = self._makeOneWithJar()
-        inst._p_deactivate() # XXX
+        inst._p_deactivate()  # XXX
+
         def _test():
             inst._p_sticky = True
         self.assertRaises(ValueError, _test)
 
     def test_assign_p_sticky_false_when_ghost(self):
         inst, jar, OID = self._makeOneWithJar()
-        inst._p_deactivate() # XXX
+        inst._p_deactivate()  # XXX
+
         def _test():
             inst._p_sticky = False
         self.assertRaises(ValueError, _test)
 
     def test_assign_p_sticky_true_non_ghost(self):
         inst, jar, OID = self._makeOneWithJar()
-        inst._p_activate() # XXX
+        inst._p_activate()  # XXX
         inst._p_changed = False
         inst._p_sticky = True
         self.assertTrue(inst._p_sticky)
 
     def test_assign_p_sticky_false_non_ghost(self):
         inst, jar, OID = self._makeOneWithJar()
-        inst._p_activate() # XXX
+        inst._p_activate()  # XXX
         inst._p_changed = False
         inst._p_sticky = False
         self.assertFalse(inst._p_sticky)
 
     def test__p_status_unsaved(self):
         inst = self._makeOne()
         self.assertEqual(inst._p_status, 'unsaved')
@@ -540,15 +553,15 @@
         inst._p_activate()
         inst._p_changed = True
         inst._p_sticky = True
         self.assertEqual(inst._p_status, 'sticky')
 
     def test__p_status_saved(self):
         inst, jar, OID = self._makeOneWithJar()
-        inst._p_activate() # XXX
+        inst._p_activate()  # XXX
         inst._p_changed = False
         self.assertEqual(inst._p_status, 'saved')
 
     def test__p_status_saved_sticky(self):
         # 'sticky' is not a state, but a separate flag.
         inst, jar, OID = self._makeOneWithJar()
         inst._p_activate()
@@ -601,15 +614,15 @@
         inst._p_activate()
         inst._p_changed = True
         inst._p_sticky = True
         self.assertEqual(inst._p_state, 2)
 
     def test__p_state_saved(self):
         inst, jar, OID = self._makeOneWithJar()
-        inst._p_activate() # XXX
+        inst._p_activate()  # XXX
         inst._p_changed = False
         self.assertEqual(inst._p_state, 0)
 
     def test__p_state_saved_sticky(self):
         # 'sticky' is not a state, but a separate flag.
         inst, jar, OID = self._makeOneWithJar()
         inst._p_activate()
@@ -640,14 +653,15 @@
             constructor = str
 
         with self.assertRaises(TypeError):
             inst._p_estimated_size = constructor(1)
 
     def test_assign_p_estimated_size_negative(self):
         inst = self._makeOne()
+
         def _test():
             inst._p_estimated_size = -1
         self.assertRaises(ValueError, _test)
 
     def test_assign_p_estimated_size_small(self):
         inst = self._makeOne()
         inst._p_estimated_size = 123
@@ -668,15 +682,15 @@
                  '_p_oid',
                  '_p_changed',
                  '_p_serial',
                  '_p_state',
                  '_p_estimated_size',
                  '_p_sticky',
                  '_p_status',
-                ]
+                 ]
         inst, jar, OID = self._makeOneWithJar()
         self._clearMRU(jar)
         for name in NAMES:
             getattr(inst, name)
         self._checkMRU(jar, [])
         # _p_mtime is special, it activates the object
         getattr(inst, '_p_mtime')
@@ -728,15 +742,15 @@
         # This comes from the C implementation and is maintained
         # for backwards compatibility. (For example, Persistent and
         # ExtensionClass.Base/Acquisition take special care to mix together.)
         class Base:
             def __getattribute__(self, name):
                 if name == 'magic':
                     return 42
-                return super().__getattribute__(name) # pragma: no cover
+                return super().__getattribute__(name)  # pragma: no cover
 
         self.assertEqual(getattr(Base(), 'magic'), 42)
 
         class Derived(self._getTargetClass(), Base):
             pass
 
         self.assertRaises(AttributeError, getattr, Derived(), 'magic')
@@ -747,15 +761,15 @@
         inst._p_activate()
         NAMES = [('_p_jar', jar),
                  ('_p_oid', OID),
                  ('_p_changed', False),
                  ('_p_serial', SERIAL),
                  ('_p_estimated_size', 0),
                  ('_p_sticky', False),
-                ]
+                 ]
         self._clearMRU(jar)
         for name, value in NAMES:
             setattr(inst, name, value)
         self._checkMRU(jar, [])
 
     def test___setattr___v__name(self):
         class Derived(self._getTargetClass()):
@@ -855,53 +869,56 @@
         self.assertEqual(jar._registered, [])
         self.assertEqual(getattr(inst, 'normal', None), 'after')
         self.assertEqual(inst._p_status, 'changed')
 
     def test___delattr___p__names(self):
         NAMES = ['_p_changed',
                  '_p_serial',
-                ]
+                 ]
         inst, jar, OID = self._makeOneWithJar()
         self._clearMRU(jar)
         jar._registered = []
         for name in NAMES:
             delattr(inst, name)
         self._checkMRU(jar, [])
         self.assertEqual(jar._registered, [])
 
     def test___delattr__normal_name_from_unsaved(self):
         class Derived(self._getTargetClass()):
             normal = 'before'
+
             def __init__(self):
                 self.__dict__['normal'] = 'after'
         inst = Derived()
         delattr(inst, 'normal')
         self.assertEqual(getattr(inst, 'normal', None), 'before')
 
     def test___delattr__normal_name_from_ghost(self, real_cache=False):
         class Derived(self._getTargetClass()):
             normal = 'before'
         inst, jar, OID = self._makeOneWithJar(Derived, real_cache=real_cache)
         inst._p_deactivate()
         self._clearMRU(jar)
         jar._registered = []
+
         def _test():
             delattr(inst, 'normal')
         self.assertRaises(AttributeError, _test)
-        self.assertEqual(inst._p_status, 'changed') # ??? this is what C does
+        self.assertEqual(inst._p_status, 'changed')  # ??? this is what C does
         self._checkMRU(jar, [OID])
         self.assertEqual(jar._registered, [OID])
         self.assertEqual(getattr(inst, 'normal', None), 'before')
 
     def test___delattr__normal_name_from_ghost_real_cache(self):
         self.test___delattr__normal_name_from_ghost(real_cache=True)
 
     def test___delattr__normal_name_from_saved(self, real_cache=False):
         class Derived(self._getTargetClass()):
             normal = 'before'
+
             def __init__(self):
                 self.__dict__['normal'] = 'after'
         inst, jar, OID = self._makeOneWithJar(Derived, real_cache=real_cache)
         inst._p_changed = False
         self._clearMRU(jar)
         jar._registered = []
         delattr(inst, 'normal')
@@ -911,14 +928,15 @@
 
     def test___delattr__normal_name_from_saved_real_cache(self):
         self.test___delattr__normal_name_from_saved(real_cache=True)
 
     def test___delattr__normal_name_from_changed(self, real_cache=False):
         class Derived(self._getTargetClass()):
             normal = 'before'
+
             def __init__(self):
                 self.__dict__['normal'] = 'after'
         inst, jar, OID = self._makeOneWithJar(Derived, real_cache=real_cache)
         inst._p_changed = True
         self._clearMRU(jar)
         jar._registered = []
         delattr(inst, 'normal')
@@ -950,38 +968,40 @@
         inst._p_baz = 'bam'
         inst._v_qux = 'spam'
         self.assertEqual(inst.__getstate__(), (None, {'foo': 'bar'}))
 
     def test___getstate___derived_w_slots_in_base_and_derived(self):
         class Base(self._getTargetClass()):
             __slots__ = ('foo',)
+
         class Derived(Base):
             __slots__ = ('baz', 'qux',)
         inst = Derived()
         inst.foo = 'bar'
         inst.baz = 'bam'
         inst.qux = 'spam'
         self.assertEqual(inst.__getstate__(),
                          (None, {'foo': 'bar', 'baz': 'bam', 'qux': 'spam'}))
 
     def test___getstate___derived_w_slots_in_base_but_not_derived(self):
         class Base(self._getTargetClass()):
             __slots__ = ('foo',)
+
         class Derived(Base):
             pass
         inst = Derived()
         inst.foo = 'bar'
         inst.baz = 'bam'
         inst.qux = 'spam'
         self.assertEqual(inst.__getstate__(),
                          ({'baz': 'bam', 'qux': 'spam'}, {'foo': 'bar'}))
 
     def test___setstate___empty(self):
         inst = self._makeOne()
-        inst.__setstate__(None) # doesn't raise, but doesn't change anything
+        inst.__setstate__(None)  # doesn't raise, but doesn't change anything
 
     def test___setstate___nonempty(self):
         from persistent.persistence import _INITIAL_SERIAL
         inst = self._makeOne()
         self.assertRaises((ValueError, TypeError),
                           inst.__setstate__, {'bogus': 1})
         self.assertEqual(inst._p_jar, None)
@@ -1012,25 +1032,27 @@
         inst = Derived()
         inst.__setstate__((None, {'foo': 'bar'}))
         self.assertEqual(inst.foo, 'bar')
 
     def test___setstate___derived_w_slots_in_base_classes(self):
         class Base(self._getTargetClass()):
             __slots__ = ('foo',)
+
         class Derived(Base):
             __slots__ = ('baz', 'qux',)
         inst = Derived()
         inst.__setstate__((None, {'foo': 'bar', 'baz': 'bam', 'qux': 'spam'}))
         self.assertEqual(inst.foo, 'bar')
         self.assertEqual(inst.baz, 'bam')
         self.assertEqual(inst.qux, 'spam')
 
     def test___setstate___derived_w_slots_in_base_but_not_derived(self):
         class Base(self._getTargetClass()):
             __slots__ = ('foo',)
+
         class Derived(Base):
             pass
         inst = Derived()
         inst.__setstate__(({'baz': 'bam', 'qux': 'spam'}, {'foo': 'bar'}))
         self.assertEqual(inst.foo, 'bar')
         self.assertEqual(inst.baz, 'bam')
         self.assertEqual(inst.qux, 'spam')
@@ -1038,26 +1060,28 @@
     if not PYPY:
         def test___setstate___interns_dict_keys(self):
             class Derived(self._getTargetClass()):
                 pass
             inst1 = Derived()
             inst2 = Derived()
             key1 = 'key'
-            key2 = 'ke'; key2 += 'y'  # construct in a way that won't intern the literal
+            key2 = 'ke'
+            key2 += 'y'  # construct in a way that won't intern the literal
             self.assertFalse(key1 is key2)
             inst1.__setstate__({key1: 1})
             inst2.__setstate__({key2: 2})
             key1 = list(inst1.__dict__.keys())[0]
             key2 = list(inst2.__dict__.keys())[0]
             self.assertTrue(key1 is key2)
 
             inst1 = Derived()
             inst2 = Derived()
             key1 = 'key'
-            key2 = 'ke'; key2 += 'y'  # construct in a way that won't intern the literal
+            key2 = 'ke'
+            key2 += 'y'  # construct in a way that won't intern the literal
             self.assertFalse(key1 is key2)
             state1 = IterableUserDict({key1: 1})
             state2 = IterableUserDict({key2: 2})
             k1 = list(state1.keys())[0]
             k2 = list(state2.keys())[0]
             self.assertFalse(k1 is k2)  # verify
             inst1.__setstate__(state1)
@@ -1116,14 +1140,15 @@
         self.assertEqual(second, (Derived,))
         self.assertEqual(third, {})
 
     def test___reduce__w_subclass_having_getnewargs_and_getstate(self):
         class Derived(self._getTargetClass()):
             def __getnewargs__(self):
                 return ('a', 'b')
+
             def __getstate__(self):
                 return {'foo': 'bar'}
         inst = Derived()
         first, second, third = inst.__reduce__()
         self.assertTrue(first is copyreg.__newobj__)
         self.assertEqual(second, (Derived, 'a', 'b'))
         self.assertEqual(third, {'foo': 'bar'})
@@ -1137,123 +1162,131 @@
         cls = getattr(cucumbers, name)
         if not issubclass(cls, self._getTargetClass()):
             self.skipTest("Cucumber is not correct implementation")
         return cls
 
     def test_pickle_roundtrip_simple(self):
         import pickle
+
         # XXX s.b. 'examples'
         Simple = self._get_cucumber('Simple')
         inst = Simple('testing')
         copy = pickle.loads(pickle.dumps(inst))
         self.assertEqual(copy, inst)
         for protocol in 0, 1, 2:
             copy = pickle.loads(pickle.dumps(inst, protocol))
             self.assertEqual(copy, inst)
 
     def test_pickle_roundtrip_w_getnewargs_and_getstate(self):
         import pickle
+
         # XXX s.b. 'examples'
         Custom = self._get_cucumber('Custom')
         inst = Custom('x', 'y')
         copy = pickle.loads(pickle.dumps(inst))
         self.assertEqual(copy, inst)
         for protocol in 0, 1, 2:
             copy = pickle.loads(pickle.dumps(inst, protocol))
             self.assertEqual(copy, inst)
 
     def test_pickle_roundtrip_w_slots_missing_slot(self):
         import pickle
+
         # XXX s.b. 'examples'
         SubSlotted = self._get_cucumber('SubSlotted')
         inst = SubSlotted('x', 'y', 'z')
         copy = pickle.loads(pickle.dumps(inst))
         self.assertEqual(copy, inst)
         for protocol in 0, 1, 2:
             copy = pickle.loads(pickle.dumps(inst, protocol))
             self.assertEqual(copy, inst)
 
     def test_pickle_roundtrip_w_slots_filled_slot(self):
         import pickle
+
         # XXX s.b. 'examples'
         SubSlotted = self._get_cucumber('SubSlotted')
         inst = SubSlotted('x', 'y', 'z')
         inst.s4 = 'a'
         copy = pickle.loads(pickle.dumps(inst))
         self.assertEqual(copy, inst)
         for protocol in 0, 1, 2:
             copy = pickle.loads(pickle.dumps(inst, protocol))
             self.assertEqual(copy, inst)
 
     def test_pickle_roundtrip_w_slots_and_empty_dict(self):
         import pickle
+
         # XXX s.b. 'examples'
         SubSubSlotted = self._get_cucumber('SubSubSlotted')
         inst = SubSubSlotted('x', 'y', 'z')
         copy = pickle.loads(pickle.dumps(inst))
         self.assertEqual(copy, inst)
         for protocol in 0, 1, 2:
             copy = pickle.loads(pickle.dumps(inst, protocol))
             self.assertEqual(copy, inst)
 
     def test_pickle_roundtrip_w_slots_and_filled_dict(self):
         import pickle
+
         # XXX s.b. 'examples'
         SubSubSlotted = self._get_cucumber('SubSubSlotted')
         inst = SubSubSlotted('x', 'y', 'z', foo='bar', baz='bam')
         inst.s4 = 'a'
         copy = pickle.loads(pickle.dumps(inst))
         self.assertEqual(copy, inst)
         for protocol in 0, 1, 2:
             copy = pickle.loads(pickle.dumps(inst, protocol))
             self.assertEqual(copy, inst)
 
     def test__p_activate_from_unsaved(self):
         inst = self._makeOne()
-        inst._p_activate() # noop w/o jar
+        inst._p_activate()  # noop w/o jar
         self.assertEqual(inst._p_status, 'unsaved')
 
     def test__p_activate_from_ghost(self):
         inst, jar, OID = self._makeOneWithJar()
         inst._p_deactivate()
         inst._p_activate()
         self.assertEqual(inst._p_status, 'saved')
 
     def test__p_activate_from_saved(self):
         inst, jar, OID = self._makeOneWithJar()
         inst._p_changed = False
-        inst._p_activate() # noop from 'saved' state
+        inst._p_activate()  # noop from 'saved' state
         self.assertEqual(inst._p_status, 'saved')
 
     def test__p_activate_only_sets_state_once(self):
         inst, jar, OID = self._makeOneWithJar()
         # No matter how many times we call _p_activate, it
         # only sets state once, the first time
-        inst._p_invalidate() # make it a ghost
+        inst._p_invalidate()  # make it a ghost
         self.assertEqual(list(jar._loaded), [])
 
         inst._p_activate()
         self.assertEqual(list(jar._loaded), [OID])
 
         inst._p_activate()
         self.assertEqual(list(jar._loaded), [OID])
 
-    def test__p_activate_leaves_object_in_saved_even_if_object_mutated_self(self):
+    def test__p_activate_leaves_object_in_saved_even_if_object_mutated_self(
+            self):
         # If the object's __setstate__ set's attributes
         # when called by p_activate, the state is still
         # 'saved' when done. Furthemore, the object is not
         # registered with the jar
 
         class WithSetstate(self._getTargetClass()):
             state = None
+
             def __setstate__(self, state):
                 self.state = state
 
         inst, jar, OID = self._makeOneWithJar(klass=WithSetstate)
-        inst._p_invalidate() # make it a ghost
+        inst._p_invalidate()  # make it a ghost
         self.assertEqual(inst._p_status, 'ghost')
 
         jar.setstate_calls_object = 42
         inst._p_activate()
         # It get loaded
         self.assertEqual(list(jar._loaded), [OID])
         # and __setstate__ got called to mutate the object
@@ -1267,14 +1300,15 @@
         inst = self._makeOne()
         inst._p_deactivate()
         self.assertEqual(inst._p_status, 'unsaved')
 
     def test__p_deactivate_from_unsaved_w_dict(self):
         class Derived(self._getTargetClass()):
             normal = 'before'
+
             def __init__(self):
                 self.__dict__['normal'] = 'after'
         inst = Derived()
         inst._p_changed = True
         inst._p_deactivate()
         self.assertEqual(inst._p_status, 'unsaved')
         self.assertEqual(inst.__dict__, {'normal': 'after'})
@@ -1294,14 +1328,15 @@
         self.assertEqual(inst._p_status, 'ghost')
         self.assertEqual(list(jar._loaded), [])
         self.assertEqual(list(jar._registered), [])
 
     def test__p_deactivate_from_saved_w_dict(self):
         class Derived(self._getTargetClass()):
             normal = 'before'
+
             def __init__(self):
                 self.__dict__['normal'] = 'after'
         inst, jar, OID = self._makeOneWithJar(Derived)
         inst._p_activate()
         jar._loaded = []
         inst._p_deactivate()
         self.assertEqual(inst._p_status, 'ghost')
@@ -1333,15 +1368,15 @@
         # assigning None is ignored when dirty
         self.assertEqual(inst._p_status, 'changed')
         self.assertEqual(list(jar._loaded), [])
         self.assertEqual(list(jar._registered), [])
 
     def test__p_deactivate_when_sticky(self):
         inst, jar, OID = self._makeOneWithJar()
-        inst._p_activate() # XXX
+        inst._p_activate()  # XXX
         inst._p_changed = False
         inst._p_sticky = True
         inst._p_deactivate()
         self.assertEqual(inst._p_status, 'sticky')
         self.assertEqual(inst._p_changed, False)
         self.assertEqual(inst._p_sticky, True)
 
@@ -1349,14 +1384,15 @@
         inst = self._makeOne()
         inst._p_invalidate()
         self.assertEqual(inst._p_status, 'unsaved')
 
     def test__p_invalidate_from_unsaved_w_dict(self):
         class Derived(self._getTargetClass()):
             normal = 'before'
+
             def __init__(self):
                 self.__dict__['normal'] = 'after'
         inst = Derived()
         inst._p_invalidate()
         self.assertEqual(inst._p_status, 'unsaved')
         self.assertEqual(inst.__dict__, {'normal': 'after'})
 
@@ -1377,14 +1413,15 @@
         self.assertEqual(inst._p_status, 'ghost')
         self.assertEqual(list(jar._loaded), [])
         self.assertEqual(list(jar._registered), [])
 
     def test__p_invalidate_from_saved_w_dict(self):
         class Derived(self._getTargetClass()):
             normal = 'before'
+
             def __init__(self):
                 self.__dict__['normal'] = 'after'
         inst, jar, OID = self._makeOneWithJar(Derived)
         inst._p_activate()
         jar._loaded = []
         jar._registered = []
         inst._p_invalidate()
@@ -1403,14 +1440,15 @@
         self.assertEqual(inst._p_status, 'ghost')
         self.assertEqual(list(jar._loaded), [])
         self.assertEqual(list(jar._registered), [])
 
     def test__p_invalidate_from_changed_w_dict(self):
         class Derived(self._getTargetClass()):
             normal = 'before'
+
             def __init__(self):
                 self.__dict__['normal'] = 'after'
         inst, jar, OID = self._makeOneWithJar(Derived)
         inst._p_activate()
         inst._p_changed = True
         jar._loaded = []
         jar._registered = []
@@ -1460,19 +1498,20 @@
 
     def test__p_invalidate_from_changed_w_slots_compat(self):
         # check that (for backward-compatibility reason) slots are not released
         # for classes where __new__ is overwritten. Attributes in __dict__
         # should be always released.
         class Derived(self._getTargetClass()):
             __slots__ = ('myattr1', 'myattr2', '__dict__')
+
             def __new__(cls):
                 obj = cls.__base__.__new__(cls)
                 obj.myattr1 = 'value1'
                 obj.myattr2 = 'value2'
-                obj.foo = 'foo1' # .foo & .bar are in __dict__
+                obj.foo = 'foo1'  # .foo & .bar are in __dict__
                 obj.bar = 'bar2'
                 return obj
         inst, jar, OID = self._makeOneWithJar(Derived)
         inst._p_activate()
         inst._p_changed = True
         jar._loaded = []
         jar._registered = []
@@ -1503,32 +1542,31 @@
         copyreg._slotnames(Derived)
 
         inst, jar, OID = self._makeOneWithJar(Derived, broken_jar=True)
         inst._p_invalidate()
         self.assertEqual(inst._p_status, 'ghost')
         self.assertRaises(NotImplementedError, inst._p_activate)
 
-
     def test__p_invalidate_from_sticky(self):
         inst, jar, OID = self._makeOneWithJar()
-        inst._p_activate() # XXX
+        inst._p_activate()  # XXX
         inst._p_changed = False
         inst._p_sticky = True
         self.assertEqual(inst._p_status, 'sticky')
         inst._p_invalidate()
         self.assertEqual(inst._p_status, 'ghost')
         self.assertEqual(inst._p_changed, None)
         self.assertEqual(inst._p_sticky, False)
 
     def test__p_invalidate_from_sticky_w_dict(self):
         class Derived(self._getTargetClass()):
             def __init__(self):
                 self.normal = 'value'
         inst, jar, OID = self._makeOneWithJar(Derived)
-        inst._p_activate() # XXX
+        inst._p_activate()  # XXX
         inst._p_changed = False
         inst._p_sticky = True
         inst._p_invalidate()
         self.assertEqual(inst._p_status, 'ghost')
         self.assertEqual(inst._p_changed, None)
         self.assertEqual(inst._p_sticky, False)
         self.assertEqual(inst.__dict__, {})
@@ -1539,15 +1577,15 @@
                  '_p_changed',
                  '_p_serial',
                  '_p_mtime',
                  '_p_state',
                  '_p_estimated_size',
                  '_p_sticky',
                  '_p_status',
-                ]
+                 ]
         inst, jar, OID = self._makeOneWithJar()
         inst._p_deactivate()
         for name in NAMES:
             self.assertTrue(inst._p_getattr(name))
         self.assertEqual(inst._p_status, 'ghost')
         self.assertEqual(list(jar._loaded), [])
         self._checkMRU(jar, [])
@@ -1588,15 +1626,15 @@
         self.assertEqual(inst._p_status, 'saved')
         self.assertEqual(list(jar._loaded), [OID])
         self._checkMRU(jar, [OID])
 
     def test__p_delattr_w__p__names(self):
         NAMES = ['_p_changed',
                  '_p_serial',
-                ]
+                 ]
         inst, jar, OID = self._makeOneWithJar()
         inst._p_changed = True
         jar._loaded = []
         for name in NAMES:
             self.assertTrue(inst._p_delattr(name))
         self.assertEqual(inst._p_status, 'ghost')
         self.assertEqual(inst._p_changed, None)
@@ -1625,14 +1663,15 @@
                 self.x = 0
 
         p = P()
         p._p_oid = b'1'
         p._p_jar = self._makeBrokenJar()
         self.assertEqual(p._p_state, 0)
         self.assertEqual(p._p_jar.called, 0)
+
         def _try():
             p._p_changed = 1
         self.assertRaises(NotImplementedError, _try)
         self.assertEqual(p._p_jar.called, 1)
         self.assertEqual(p._p_state, 0)
 
     def test__p_activate_w_broken_jar(self):
@@ -1653,56 +1692,68 @@
         # We once had a bug in the `Persistent` class that calculated an
         # incorrect offset for the ``__dict__`` attribute.  It assigned
         # ``__dict__`` and ``_p_jar`` to the same location in memory.
         # This is a simple test to make sure they have different locations.
         class P(self._getTargetClass()):
             def __init__(self):
                 self.x = 0
+
             def inc(self):
                 self.x += 1
         p = P()
         p.inc()
         p.inc()
         self.assertTrue('x' in p.__dict__)
         self.assertTrue(p._p_jar is None)
 
     def test_w_diamond_inheritance(self):
         class A(self._getTargetClass()):
             pass
+
         class B(self._getTargetClass()):
             pass
+
         class C(A, B):
             pass
+
         class D:
             pass
+
         class E(D, B):
             pass
         # no raise
         A(), B(), C(), D(), E()
 
     def test_w_alternate_metaclass(self):
         class alternateMeta(type):
             pass
+
         class alternate:
             __metaclass__ = alternateMeta
+
         class mixedMeta(alternateMeta, type):
             pass
         # no raise
+
         class mixed1(alternate, self._getTargetClass()):
             pass
+
         class mixed2(self._getTargetClass(), alternate):
             pass
 
     def test_setattr_in_subclass_is_not_called_creating_an_instance(self):
         class subclass(self._getTargetClass()):
             _v_setattr_called = False
+
             def __setattr__(self, name, value):
                 raise AssertionError("Should not be called")
         inst = subclass()
-        self.assertEqual(object.__getattribute__(inst, '_v_setattr_called'), False)
+        self.assertEqual(
+            object.__getattribute__(
+                inst, '_v_setattr_called'), False)
 
     def test_can_set__p_attrs_if_subclass_denies_setattr(self):
         # ZODB defines a PersistentBroken subclass that only lets us
         # set things that start with _p, so make sure we can do that
         class Broken(self._getTargetClass()):
             def __setattr__(self, name, value):
                 if name.startswith('_p_'):
@@ -1719,27 +1770,28 @@
 
         broken._p_changed = True
         broken._p_changed = 0
 
     def test_p_invalidate_calls_p_deactivate(self):
         class P(self._getTargetClass()):
             deactivated = False
+
             def _p_deactivate(self):
                 self.deactivated = True
         p = P()
         p._p_invalidate()
         self.assertTrue(p.deactivated)
 
-
     def test_new_ghost_success_not_already_ghost_dict(self):
         # https://github.com/zopefoundation/persistent/issues/49
         # calling new_ghost on an object that already has state just changes
         # its flags, it doesn't destroy the state.
         from persistent.interfaces import GHOST
         from persistent.interfaces import UPTODATE
+
         class TestPersistent(self._getTargetClass()):
             pass
         KEY = b'123'
         jar = self._makeJar()
         cache = self._makeRealCache(jar)
         candidate = TestPersistent()
 
@@ -1754,14 +1806,15 @@
 
     def test_new_ghost_success_not_already_ghost_slot(self):
         # https://github.com/zopefoundation/persistent/issues/49
         # calling new_ghost on an object that already has state just changes
         # its flags, it doesn't destroy the state.
         from persistent.interfaces import GHOST
         from persistent.interfaces import UPTODATE
+
         class TestPersistent(self._getTargetClass()):
             __slots__ = ('set_by_new', '__weakref__')
         KEY = b'123'
         jar = self._makeJar()
         cache = self._makeRealCache(jar)
         candidate = TestPersistent()
         candidate.set_by_new = 1
@@ -1787,15 +1840,16 @@
 
     def _normalized_repr(self, o):
         return self._normalize_repr(repr(o))
 
     def test_repr_no_oid_no_jar(self):
         p = self._makeOne()
         result = self._normalized_repr(p)
-        self.assertEqual(result, '<persistent.Persistent object at 0xdeadbeef>')
+        self.assertEqual(
+            result, '<persistent.Persistent object at 0xdeadbeef>')
 
     def test_repr_no_oid_in_jar(self):
         p = self._makeOne()
 
         class Jar:
             def __repr__(self):
                 return '<SomeJar>'
@@ -1810,69 +1864,73 @@
     def test_repr_oid_no_jar(self):
         p = self._makeOne()
         p._p_oid = self._PACKED_OID
 
         result = self._normalized_repr(p)
         self.assertEqual(
             result,
-            "<persistent.Persistent object at 0xdeadbeef oid " + self._HEX_OID + ">")
+            "<persistent.Persistent object at 0xdeadbeef oid " +
+            self._HEX_OID +
+            ">")
 
     def test_64bit_oid(self):
         import struct
         p = self._makeOne()
         oid_value = 2 << 62
         self.assertEqual(oid_value.bit_length(), 64)
         oid = struct.pack(">Q", oid_value)
         self.assertEqual(oid, b'\x80\x00\x00\x00\x00\x00\x00\x00')
 
         p._p_oid = oid
         result = self._normalized_repr(p)
         self.assertEqual(
             result,
-            '<persistent.Persistent object at 0xdeadbeef oid 0x8000000000000000>'
-        )
+            '<persistent.Persistent object at 0xdeadbeef oid'
+            ' 0x8000000000000000>')
 
     def test_repr_no_oid_repr_jar_raises_exception(self):
         p = self._makeOne()
 
         class Jar:
             def __repr__(self):
                 raise Exception('jar repr failed')
 
         p._p_jar = Jar()
 
         result = self._normalized_repr(p)
         self.assertEqual(
             result,
-            "<persistent.Persistent object at 0xdeadbeef in Exception('jar repr failed')>")
-
+            "<persistent.Persistent object at 0xdeadbeef in"
+            " Exception('jar repr failed')>")
 
     def test_repr_oid_raises_exception_no_jar(self):
         p = self._makeOne()
 
         class BadOID(bytes):
             def __repr__(self):
                 raise Exception("oid repr failed")
 
         # Our OID is bytes, 8 bytes long. We don't call its repr.
         p._p_oid = BadOID(self._PACKED_OID)
 
         result = self._normalized_repr(p)
         self.assertEqual(
             result,
-            "<persistent.Persistent object at 0xdeadbeef oid " + self._HEX_OID + ">")
+            "<persistent.Persistent object at 0xdeadbeef oid " +
+            self._HEX_OID +
+            ">")
 
         # Anything other than 8 bytes, though, we do.
         p._p_oid = BadOID(b'1234567')
 
         result = self._normalized_repr(p)
         self.assertEqual(
             result,
-            "<persistent.Persistent object at 0xdeadbeef oid Exception('oid repr failed')>")
-
+            "<persistent.Persistent object at 0xdeadbeef oid"
+            " Exception('oid repr failed')>")
 
     def test_repr_oid_and_jar_raise_exception(self):
         p = self._makeOne()
 
         class BadOID(bytes):
             def __repr__(self):
                 raise Exception("oid repr failed")
@@ -1880,20 +1938,19 @@
 
         class Jar:
             def __repr__(self):
                 raise Exception('jar repr failed')
 
         p._p_jar = Jar()
 
-
         result = self._normalized_repr(p)
         self.assertEqual(
             result,
-            "<persistent.Persistent object at 0xdeadbeef oid Exception('oid repr failed')"
-            " in Exception('jar repr failed')>")
+            "<persistent.Persistent object at 0xdeadbeef oid"
+            " Exception('oid repr failed') in Exception('jar repr failed')>")
 
     def test_repr_no_oid_repr_jar_raises_baseexception(self):
         p = self._makeOne()
 
         class Jar:
             def __repr__(self):
                 raise BaseException('jar repr failed')
@@ -1927,15 +1984,17 @@
                 return '<SomeJar>'
 
         p._p_jar = Jar()
 
         result = self._normalized_repr(p)
         self.assertEqual(
             result,
-            "<persistent.Persistent object at 0xdeadbeef oid " + self._HEX_OID + " in <SomeJar>>")
+            "<persistent.Persistent object at 0xdeadbeef oid " +
+            self._HEX_OID +
+            " in <SomeJar>>")
 
     def test__p_repr(self):
         class P(self._getTargetClass()):
             def _p_repr(self):
                 return "Override"
         p = P()
         self.assertEqual("Override", repr(p))
@@ -1951,77 +2010,86 @@
             "<persistent.tests.test_persistence.P object at 0xdeadbeef"
             " _p_repr Exception('_p_repr failed')>")
 
         p._p_oid = self._PACKED_OID
         result = self._normalized_repr(p)
         self.assertEqual(
             result,
-            "<persistent.tests.test_persistence.P object at 0xdeadbeef oid " + self._HEX_OID
-            + " _p_repr Exception('_p_repr failed')>")
+            "<persistent.tests.test_persistence.P object at 0xdeadbeef oid " +
+            self._HEX_OID +
+            " _p_repr Exception('_p_repr failed')>")
 
         class Jar:
             def __repr__(self):
                 return '<SomeJar>'
 
         p._p_jar = Jar()
         result = self._normalized_repr(p)
         self.assertEqual(
             result,
-            "<persistent.tests.test_persistence.P object at 0xdeadbeef oid " + self._HEX_OID
-            + " in <SomeJar> _p_repr Exception('_p_repr failed')>")
+            "<persistent.tests.test_persistence.P object at 0xdeadbeef oid " +
+            self._HEX_OID +
+            " in <SomeJar> _p_repr Exception('_p_repr failed')>")
 
     def test__p_repr_in_instance_ignored(self):
         class P(self._getTargetClass()):
             pass
         p = P()
         p._p_repr = lambda: "Instance"
         result = self._normalized_repr(p)
-        self.assertEqual(result,
-                         '<persistent.tests.test_persistence.P object at 0xdeadbeef>')
+        self.assertEqual(
+            result,
+            '<persistent.tests.test_persistence.P object at 0xdeadbeef>')
 
     def test__p_repr_baseexception(self):
         class P(self._getTargetClass()):
             def _p_repr(self):
                 raise BaseException("_p_repr failed")
         p = P()
         with self.assertRaisesRegex(BaseException, '_p_repr failed'):
             repr(p)
 
+
 class PyPersistentTests(unittest.TestCase, _Persistent_Base):
 
     def _getTargetClass(self):
         from persistent.persistence import PersistentPy
-        assert PersistentPy.__module__ == 'persistent.persistence', PersistentPy.__module__
+        self.assertEqual(PersistentPy.__module__, 'persistent.persistence')
         return PersistentPy
 
     def _makeCache(self, jar):
 
         class _Cache:
             def __init__(self, jar):
                 self._jar = jar
                 self._mru = []
                 self._data = {}
+
             def mru(self, oid):
                 self._mru.append(oid)
+
             def new_ghost(self, oid, obj):
                 obj._p_jar = self._jar
                 obj._p_oid = oid
                 # The C implementation always returns actual ghosts,
                 # make sure we do too. However, we can't call
                 # _p_deactivate(), because that clears the dictionary.
                 # The C pickle cache makes the object a ghost just by
                 # setting its status to 'ghost', without going though
                 # _p_deactivate(). Thus, we do the same by setting the
                 # flags.
                 object.__setattr__(obj, '_Persistent__flags', None)
                 self._data[oid] = obj
+
             def get(self, oid):
                 return self._data.get(oid)
+
             def __delitem__(self, oid):
                 del self._data[oid]
+
             def update_object_size_estimation(self, oid, new_size):
                 pass
 
         return _Cache(jar)
 
     def _getRealCacheClass(self):
         from persistent.picklecache import PickleCachePy as PickleCache
@@ -2061,20 +2129,23 @@
         jar._cache.mru = mru
         c1._p_accessed()
         self._checkMRU(jar, [])
 
     def test_accessed_invalidated_with_jar_and_oid_but_no_cache(self):
         # This scenario arises in ZODB tests where the jar is faked
         KEY = b'123'
+
         class Jar:
             accessed = False
+
             def __getattr__(self, name):
                 if name == '_cache':
                     self.accessed = True
                 raise AttributeError(name)
+
             def register(self, *args):
                 pass
         c1 = self._makeOne()
 
         c1._p_oid = KEY
         c1._p_jar = Jar()
         c1._p_changed = True
@@ -2083,15 +2154,15 @@
         self.assertTrue(c1._p_jar.accessed)
 
         c1._p_jar.accessed = False
         c1._p_invalidate_deactivate_helper()
         self.assertTrue(c1._p_jar.accessed)
 
         c1._p_jar.accessed = False
-        c1._Persistent__flags = None # coverage
+        c1._Persistent__flags = None  # coverage
         c1._p_invalidate_deactivate_helper()
         self.assertTrue(c1._p_jar.accessed)
 
     def test_p_activate_with_jar_without_oid(self):
         # Works, but nothing happens
         inst = self._makeOne()
         inst._p_jar = object()
@@ -2118,18 +2189,18 @@
 class CPersistentTests(unittest.TestCase, _Persistent_Base):
 
     def _getTargetClass(self):
         from persistent._compat import _c_optimizations_available as get_c
         return get_c()['persistent.persistence'].Persistent
 
     def _checkMRU(self, jar, value):
-        pass # Figure this out later
+        pass  # Figure this out later
 
     def _clearMRU(self, jar):
-        pass # Figure this out later
+        pass  # Figure this out later
 
     def _makeCache(self, jar):
         from persistent._compat import _c_optimizations_available as get_c
         PickleCache = get_c()['persistent.picklecache'].PickleCache
         return PickleCache(jar)
 
 
@@ -2145,9 +2216,10 @@
         self.assertRaises(TypeError, self._callFUT, '')
 
     def test_w_type(self):
         TO_CREATE = [type, list, tuple, object, dict]
         for typ in TO_CREATE:
             self.assertTrue(isinstance(self._callFUT(typ), typ))
 
+
 def test_suite():
     return unittest.defaultTestLoader.loadTestsFromName(__name__)
```

### Comparing `persistent-5.2/src/persistent/tests/test_picklecache.py` & `persistent-6.0/src/persistent/tests/test_picklecache.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,24 +10,22 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 import gc
 import unittest
 
-from persistent.interfaces import UPTODATE
 from persistent._compat import PYPY
+from persistent.interfaces import UPTODATE
 from persistent.tests.utils import skipIfNoCExtension
 
 
-# pylint:disable=protected-access,too-many-lines,too-many-public-methods
-# pylint:disable=attribute-defined-outside-init,redefined-outer-name
-
 _marker = object()
 
+
 class DummyPersistent:
     _Persistent__ring = None
 
     def _p_invalidate(self):
         from persistent.interfaces import GHOST
         self._p_state = GHOST
 
@@ -44,30 +42,33 @@
     pass
 
 
 class ClosedConnection(DummyConnection):
     def __init__(self, test):
         self.test = test
 
-    def setstate(self, obj): # pragma: no cover
+    def setstate(self, obj):  # pragma: no cover
         self.test.fail("Connection is closed")
 
     def register(self, obj):
         """Does nothing."""
 
+
 def _len(seq):
     return len(list(seq))
 
 
 class PickleCacheTestMixin:
 
     def _getTargetClass(self):
         from persistent.picklecache import PickleCachePy as BasePickleCache
+
         class PickleCache(BasePickleCache):
-            _CACHEABLE_TYPES = BasePickleCache._CACHEABLE_TYPES + (DummyPersistent,)
+            _CACHEABLE_TYPES = BasePickleCache._CACHEABLE_TYPES + \
+                (DummyPersistent,)
         return PickleCache
 
     def _getTargetInterface(self):
         from persistent.interfaces import IPickleCache
         return IPickleCache
 
     def _makeOne(self, jar=None, target_size=10):
@@ -184,15 +185,14 @@
         KEY = b'uptodate'
         cache = self._makeOne()
         uptodate = self._makePersist(state=UPTODATE)
 
         with self.assertRaises(ValueError):
             cache[KEY] = uptodate
 
-
     def test___setitem___non_ghost(self):
         KEY = b'uptodate'
         cache = self._makeOne()
         uptodate = self._makePersist(state=UPTODATE, oid=KEY)
 
         cache[KEY] = uptodate
 
@@ -205,14 +205,15 @@
         self.assertTrue(items[0][1] is uptodate)
         self.assertTrue(cache[KEY] is uptodate)
         self.assertTrue(cache.get(KEY) is uptodate)
 
     def test___setitem___persistent_class(self):
 
         KEY = b'pclass'
+
         class pclass:
             _p_oid = KEY
             _p_jar = DummyConnection()
         cache = self._makeOne(pclass._p_jar)
 
         cache[KEY] = pclass
 
@@ -238,14 +239,15 @@
         with self.assertRaises(KeyError):
             del cache[b'nonesuch']
 
     def test___delitem___w_persistent_class(self):
 
         KEY = b'pclass'
         cache = self._makeOne()
+
         class pclass:
             _p_oid = KEY
             _p_jar = DummyConnection()
         cache = self._makeOne()
 
         cache[KEY] = pclass
         del cache[KEY]
@@ -300,15 +302,14 @@
 
         items = cache.lru_items()
         self.assertEqual(_len(items), 3)
         self.assertEqual(items[0][0], ONE)
         self.assertEqual(items[1][0], TWO)
         self.assertEqual(items[2][0], THREE)
 
-
     def _numbered_oid(self, i):
         return b'oid_%04d' % i
 
     def _populate_cache(self, cache, count=100,
                         state_0=UPTODATE,
                         state_rest=UPTODATE):
 
@@ -322,15 +323,15 @@
 
     def test_incrgc_simple(self):
         cache = self._makeOne()
         oids = self._populate_cache(cache)
         self.assertEqual(cache.cache_non_ghost_count, 100)
 
         cache.incrgc()
-        gc.collect() # banish the ghosts who are no longer in the ring
+        gc.collect()  # banish the ghosts who are no longer in the ring
 
         self.assertEqual(cache.cache_non_ghost_count, 10)
         items = cache.lru_items()
         self.assertEqual(_len(items), 10)
         self.assertEqual(items[0][0], b'oid_0090')
         self.assertEqual(items[1][0], b'oid_0091')
         self.assertEqual(items[2][0], b'oid_0092')
@@ -372,22 +373,23 @@
 
     def test_full_sweep(self):
         cache = self._makeOne()
         oids = self._populate_cache(cache)
         self.assertEqual(cache.cache_non_ghost_count, 100)
 
         cache.full_sweep()
-        gc.collect() # banish the ghosts who are no longer in the ring
+        gc.collect()  # banish the ghosts who are no longer in the ring
 
         self.assertEqual(cache.cache_non_ghost_count, 0)
 
         for oid in oids:
             self.assertTrue(cache.get(oid) is None)
 
-    def test_full_sweep_clears_weakrefs_in_interface(self, sweep_method='full_sweep'):
+    def test_full_sweep_clears_weakrefs_in_interface(
+            self, sweep_method='full_sweep'):
         # https://github.com/zopefoundation/persistent/issues/149
         # Sweeping the cache clears weak refs (for PyPy especially)
         # In the real world, this shows up in the interaction with
         # persistent objects and zope.interface/zope.component,
         # so we use an Interface to demonstrate. This helps find issues
         # like needing to run GC more than once, etc, because of how the
         # object is referenced.
@@ -420,19 +422,21 @@
 
         # Now, try to use that weak reference. If the weak reference is
         # still around, this will raise the error about the connection
         # being closed.
         Interface.changed(None)
 
     def test_incrgc_clears_weakrefs_in_interface(self):
-        self.test_full_sweep_clears_weakrefs_in_interface(sweep_method='incrgc')
+        self.test_full_sweep_clears_weakrefs_in_interface(
+            sweep_method='incrgc')
 
     def test_full_sweep_clears_weakrefs(self, sweep_method='incrgc'):
         # like test_full_sweep_clears_weakrefs_in_interface,
-        # but directly using a weakref. This is the simplest version of the test.
+        # but directly using a weakref. This is the simplest version of the
+        # test.
         from weakref import ref as WeakRef
         gc.disable()
         self.addCleanup(gc.enable)
 
         jar = ClosedConnection(self)
         cache = self._makeOne(jar, 0)
 
@@ -464,15 +468,15 @@
 
     def test_minimize(self):
         cache = self._makeOne()
         oids = self._populate_cache(cache)
         self.assertEqual(cache.cache_non_ghost_count, 100)
 
         cache.minimize()
-        gc.collect() # banish the ghosts who are no longer in the ring
+        gc.collect()  # banish the ghosts who are no longer in the ring
 
         self.assertEqual(cache.cache_non_ghost_count, 0)
 
         for oid in oids:
             self.assertTrue(cache.get(oid) is None)
 
     def test_minimize_turns_into_ghosts(self):
@@ -480,15 +484,15 @@
 
         cache = self._makeOne()
         oid = self._numbered_oid(1)
         obj = cache[oid] = self._makePersist(oid=oid, state=UPTODATE)
         self.assertEqual(cache.cache_non_ghost_count, 1)
 
         cache.minimize()
-        gc.collect() # banish the ghosts who are no longer in the ring
+        gc.collect()  # banish the ghosts who are no longer in the ring
 
         self.assertEqual(cache.cache_non_ghost_count, 0)
 
         self.assertEqual(obj._p_state, GHOST)
 
     def test_new_ghost_non_persistent_object(self):
 
@@ -545,44 +549,46 @@
         self.assertTrue(cache.get(KEY) is candidate)
         self.assertEqual(candidate._p_oid, KEY)
         self.assertEqual(candidate._p_jar, jar)
         self.assertEqual(candidate._p_state, GHOST)
 
     def test_new_ghost_w_pclass_non_ghost(self):
         KEY = b'123'
+
         class Pclass:
             _p_oid = None
             _p_jar = None
         cache = self._makeOne()
         cache.new_ghost(KEY, Pclass)
         self.assertTrue(cache.get(KEY) is Pclass)
         self.assertEqual(Pclass._p_oid, KEY)
         return cache, Pclass, KEY
 
     def test_new_ghost_w_pclass_ghost(self):
         KEY = b'123'
+
         class Pclass:
             _p_oid = None
             _p_jar = None
         cache = self._makeOne()
         cache.new_ghost(KEY, Pclass)
         self.assertTrue(cache.get(KEY) is Pclass)
         self.assertEqual(Pclass._p_oid, KEY)
         return cache, Pclass, KEY
 
     def test_invalidate_miss_single(self):
         KEY = b'123'
         cache = self._makeOne()
-        cache.invalidate(KEY) # doesn't raise
+        cache.invalidate(KEY)  # doesn't raise
 
     def test_invalidate_miss_multiple(self):
         KEY = b'123'
         KEY2 = b'456'
         cache = self._makeOne()
-        cache.invalidate([KEY, KEY2]) # doesn't raise
+        cache.invalidate([KEY, KEY2])  # doesn't raise
 
     def test_invalidate_hit_single_non_ghost(self):
         from persistent.interfaces import GHOST
 
         KEY = b'123'
         jar = DummyConnection()
         cache = self._makeOne(jar)
@@ -610,22 +616,23 @@
         cache.invalidate([KEY2, KEY])
         self.assertEqual(cache.ringlen(), 0)
         self.assertEqual(c1._p_state, GHOST)
         self.assertEqual(c2._p_state, GHOST)
 
     def test_debug_info_w_persistent_class(self):
         KEY = b'pclass'
+
         class pclass:
             _p_oid = KEY
             _p_jar = DummyConnection()
         cache = self._makeOne(pclass._p_jar)
         pclass._p_state = UPTODATE
         cache[KEY] = pclass
 
-        gc.collect() # pypy vs. refcounting
+        gc.collect()  # pypy vs. refcounting
         info = cache.debug_info()
 
         self.assertEqual(len(info), 1)
         # C and Python return different length tuples,
         # and the refcounts are off by one.
         oid = info[0][0]
         typ = info[0][2]
@@ -637,51 +644,50 @@
 
     def test_debug_info_w_normal_object(self):
         KEY = b'uptodate'
         cache = self._makeOne()
         uptodate = self._makePersist(state=UPTODATE, oid=KEY)
         cache[KEY] = uptodate
 
-        gc.collect() # pypy vs. refcounting
+        gc.collect()  # pypy vs. refcounting
         info = cache.debug_info()
 
         self.assertEqual(len(info), 1)
         # C and Python return different length tuples,
         # and the refcounts are off by one.
         oid = info[0][0]
         typ = info[0][2]
         self.assertEqual(oid, KEY)
         self.assertEqual(typ, type(uptodate).__name__)
         return uptodate, info[0]
 
-
     def test_debug_info_w_ghost(self):
         from persistent.interfaces import GHOST
 
         KEY = b'ghost'
         cache = self._makeOne()
         ghost = self._makePersist(state=GHOST, oid=KEY)
         cache[KEY] = ghost
 
-        gc.collect() # pypy vs. refcounting
+        gc.collect()  # pypy vs. refcounting
         info = cache.debug_info()
 
         self.assertEqual(len(info), 1)
         oid, _refc, typ, state = info[0]
         self.assertEqual(oid, KEY)
         self.assertEqual(typ, type(ghost).__name__)
         # In the C implementation, we couldn't actually set the _p_state
         # directly.
         self.assertEqual(state, ghost._p_state)
         return ghost, info[0]
 
     def test_setting_non_persistent_item(self):
         cache = self._makeOne()
-        with self.assertRaisesRegex(TypeError,
-                                    "Cache values must be persistent objects."):
+        with self.assertRaisesRegex(
+                TypeError, "Cache values must be persistent objects."):
             cache[b'12345678'] = object()
 
     def test_setting_without_jar(self):
         cache = self._makeOne()
         p = self._makePersist(jar=None)
         with self.assertRaisesRegex(ValueError,
                                     "Cached object jar missing"):
@@ -710,23 +716,24 @@
     def test_sweep_empty(self):
         cache = self._makeOne()
         # Python returns 0, C returns None
         self.assertFalse(cache.incrgc())
 
     def test_invalidate_persistent_class_calls_p_invalidate(self):
         KEY = b'pclass'
+
         class pclass:
             _p_oid = KEY
             _p_jar = DummyConnection()
             invalidated = False
+
             @classmethod
             def _p_invalidate(cls):
                 cls.invalidated = True
 
-
         cache = self._makeOne(pclass._p_jar)
 
         cache[KEY] = pclass
 
         cache.invalidate(KEY)
 
         self.assertTrue(pclass.invalidated)
@@ -754,21 +761,20 @@
         return IExtendedPickleCache
 
     def test_sweep_of_non_deactivating_object(self):
         jar = DummyConnection()
         cache = self._makeOne(jar)
         p = self._makePersist(jar=jar)
 
-        p._p_state = 0 # non-ghost, get in the ring
+        p._p_state = 0  # non-ghost, get in the ring
         cache[p._p_oid] = p
 
         def bad_deactivate():
             "Doesn't call super, for it's own reasons, so can't be ejected"
 
-
         p._p_deactivate = bad_deactivate
 
         cache._SWEEPABLE_TYPES = DummyPersistent
         self.assertEqual(cache.full_sweep(), 0)
         del cache._SWEEPABLE_TYPES
 
         del p._p_deactivate
@@ -943,14 +949,15 @@
         self.assertEqual(_len(items), 3)
         self.assertEqual(items[0][0], ONE)
         self.assertEqual(items[1][0], TWO)
         self.assertEqual(items[2][0], THREE)
 
     def test_invalidate_hit_pclass(self):
         KEY = b'123'
+
         class Pclass:
             _p_oid = KEY
             _p_jar = DummyConnection()
         cache = self._makeOne(Pclass._p_jar)
         cache[KEY] = Pclass
         self.assertIs(cache.persistent_classes[KEY], Pclass)
         cache.invalidate(KEY)
@@ -974,15 +981,15 @@
         from persistent.interfaces import STICKY
 
         cache = self._makeOne()
         oids = self._populate_cache(cache, state_0=STICKY)
         self.assertEqual(cache.cache_non_ghost_count, 100)
 
         cache.full_sweep()
-        gc.collect() # banish the ghosts who are no longer in the ring
+        gc.collect()  # banish the ghosts who are no longer in the ring
 
         self.assertEqual(cache.cache_non_ghost_count, 1)
 
         self.assertTrue(cache.get(oids[0]) is not None)
         for oid in oids[1:]:
             self.assertTrue(cache.get(oid) is None)
 
@@ -990,27 +997,28 @@
         from persistent.interfaces import CHANGED
 
         cache = self._makeOne()
         oids = self._populate_cache(cache, state_0=CHANGED)
         self.assertEqual(cache.cache_non_ghost_count, 100)
 
         cache.full_sweep()
-        gc.collect() # banish the ghosts who are no longer in the ring
+        gc.collect()  # banish the ghosts who are no longer in the ring
 
         self.assertEqual(cache.cache_non_ghost_count, 1)
 
         self.assertTrue(cache.get(oids[0]) is not None)
         for oid in oids[1:]:
             self.assertTrue(cache.get(oid) is None)
 
     def test_init_with_cacheless_jar(self):
         # Sometimes ZODB tests pass objects that don't
         # have a _cache
         class Jar:
             was_set = False
+
             def __setattr__(self, name, value):
                 if name == '_cache':
                     object.__setattr__(self, 'was_set', True)
                 raise AttributeError(name)
 
         jar = Jar()
         self._makeOne(jar)
@@ -1079,29 +1087,31 @@
         self.assertTrue(items[0][1] is candidate)
         self.assertEqual(candidate._p_state, UPTODATE)
 
     def test_cache_garbage_collection_bytes_also_deactivates_object(self):
 
         class MyPersistent(self._getDummyPersistentClass()):
             def _p_deactivate(self):
-                # mimic what the real persistent object does to update the cache
-                # size; if we don't get deactivated by sweeping, the cache size
-                # won't shrink so this also validates that _p_deactivate gets
-                # called when ejecting an object.
+                # mimic what the real persistent object does to update the
+                # cache size; if we don't get deactivated by sweeping, the
+                # cache size won't shrink so this also validates that
+                # _p_deactivate gets called when ejecting an object.
                 cache.update_object_size_estimation(self._p_oid, -1)
 
         cache = self._makeOne()
         cache.cache_size = 1000
         oids = []
         for i in range(100):
             oid = self._numbered_oid(i)
             oids.append(oid)
-            o = cache[oid] = self._makePersist(oid=oid, kind=MyPersistent, state=UPTODATE)
+            o = cache[oid] = self._makePersist(
+                oid=oid, kind=MyPersistent, state=UPTODATE)
 
-            o._Persistent__size = 0 # must start 0, ZODB sets it AFTER updating the size
+            # must start 0, ZODB sets it AFTER updating the size
+            o._Persistent__size = 0
 
             cache.update_object_size_estimation(oid, 64)
             o._Persistent__size = 2
 
         self.assertEqual(cache.cache_non_ghost_count, 100)
 
         # A GC at this point does nothing
@@ -1119,19 +1129,18 @@
         self.assertTrue(cache.total_estimated_size > 1)
         # A gc shrinks the bytes
         cache.incrgc()
         self.assertEqual(cache.total_estimated_size, 0)
 
         # It also shrank the measured size of the cache,
         # though this may require a GC to be visible.
-        if PYPY: # pragma: no cover
+        if PYPY:  # pragma: no cover
             gc.collect()
         self.assertEqual(len(cache), 1)
 
-
     def test_new_ghost_obj_already_in_cache(self):
         base_result = super().test_new_ghost_obj_already_in_cache()
         cache, key, candidate = base_result
         # If we're sneaky and remove the OID and jar, then we get the duplicate
         # key error. Removing them only works because we're not using a real
         # persistent object.
         candidate._p_oid = None
@@ -1161,61 +1170,62 @@
             o = cache[oid] = self._makePersist(oid=oid,
                                                kind=MyPersistent,
                                                state=UPTODATE)
             # must start 0, ZODB sets it AFTER updating the size
             o._Persistent__size = 0
             cache.update_object_size_estimation(oid, 1)
             o._Persistent__size = 1
-            del o # leave it only in the cache
+            del o  # leave it only in the cache
 
         self.assertEqual(cache.cache_non_ghost_count, 100)
         self.assertEqual(cache.total_estimated_size, 64 * 100)
 
         cache.incrgc()
-        gc.collect() # banish the ghosts who are no longer in the ring
+        gc.collect()  # banish the ghosts who are no longer in the ring
         self.assertEqual(cache.total_estimated_size, 64 * 6)
         self.assertEqual(cache.cache_non_ghost_count, 6)
         self.assertEqual(len(cache), 6)
 
         cache.full_sweep()
-        gc.collect() # banish the ghosts who are no longer in the ring
+        gc.collect()  # banish the ghosts who are no longer in the ring
         self.assertEqual(cache.total_estimated_size, 0)
         self.assertEqual(cache.cache_non_ghost_count, 0)
         self.assertEqual(len(cache), 0)
 
     def test_interpreter_finalization_ffi_cleanup(self):
-        # When the interpreter is busy garbage collecting old objects
-        # and clearing their __dict__ in random orders, the CFFI cleanup
-        # ``ffi.gc()`` cleanup hooks we use on CPython don't
-        # raise errors.
+        # When the interpreter is busy garbage collecting old objects and
+        # clearing their __dict__ in random orders, the CFFI cleanup
+        # ``ffi.gc()`` cleanup hooks we use on CPython don't raise errors.
         #
-        # Prior to Python 3.8, when ``sys.unraisablehook`` was added,
-        # the only way to know if this test fails is to look for AttributeError
-        # on stderr.
+        # Prior to Python 3.8, when ``sys.unraisablehook`` was added, the only
+        # way to know if this test fails is to look for AttributeError on
+        # stderr.
         #
-        # But wait, it gets worse. Prior to https://foss.heptapod.net/pypy/cffi/-/issues/492
-        # (CFFI > 1.14.5, unreleased at this writing), CFFI ignores
-        # ``sys.unraisablehook``, so even on 3.8 the only way to know
-        # a failure is to watch stderr.
+        # But wait, it gets worse. Prior to
+        # https://foss.heptapod.net/pypy/cffi/-/issues/492 (CFFI > 1.14.5,
+        # unreleased at this writing), CFFI ignores ``sys.unraisablehook``, so
+        # even on 3.8 the only way to know a failure is to watch stderr.
         #
         # See https://github.com/zopefoundation/persistent/issues/150
 
         import sys
         unraised = []
         try:
             old_hook = sys.unraisablehook
         except AttributeError:
             pass
-        else: # pragma: no cover
+        else:  # pragma: no cover
             sys.unraisablehook = unraised.append
             self.addCleanup(setattr, sys, 'unraisablehook', old_hook)
 
         cache = self._makeOne()
         oid = self._numbered_oid(42)
-        o = cache[oid] = self._makePersist(oid=oid)
+        # local variable 'o' is assigned to but never used, but needed for the
+        # test to succeed.
+        o = cache[oid] = self._makePersist(oid=oid)  # noqa: F841
         # Clear the dict, or at least part of it.
         # This is coupled to ``cleanup_hook``
         if cache.data.cleanup_hook:
             del cache.data._addr_to_oid
         del cache[oid]
 
         self.assertEqual(unraised, [])
@@ -1236,17 +1246,19 @@
         class DummyPersistent(self._getRealPersistentClass()):
             __slots__ = ()
         return DummyPersistent
 
     def test_inst_does_not_conform_to_IExtendedPickleCache(self):
         # Test that ``@use_c_impl`` is only applying the correct
         # interface declaration to the C implementation.
-        from persistent.interfaces import IExtendedPickleCache
-        from zope.interface.verify import verifyObject
         from zope.interface.exceptions import Invalid
+        from zope.interface.verify import verifyObject
+
+        from persistent.interfaces import IExtendedPickleCache
+
         # We don't claim to implement it.
         self.assertFalse(IExtendedPickleCache.providedBy(self._makeOne()))
         # And we don't even provide everything it asks for.
         # (Exact error depends on version of zope.interface and what we
         # fail to implement. 5.0 probably raises MultipleInvalid).
         with self.assertRaises(Invalid):
             verifyObject(IExtendedPickleCache, self._makeOne(), tentative=True)
@@ -1258,15 +1270,15 @@
     def test_cache_garbage_collection_bytes_with_cache_size_0(self):
 
         class DummyConnection:
             def register(self, obj):
                 pass
 
         dummy_connection = DummyConnection()
-        dummy_connection.register(1) # for coveralls
+        dummy_connection.register(1)  # for coveralls
 
         def makePersistent(oid):
             persist = self._getDummyPersistentClass()()
             persist._p_oid = oid
             persist._p_jar = dummy_connection
             return persist
 
@@ -1279,26 +1291,26 @@
         oids = []
         for i in range(100):
             oid = self._numbered_oid(i)
             oids.append(oid)
             o = cache[oid] = makePersistent(oid)
             cache.update_object_size_estimation(oid, 1)
             o._p_estimated_size = 1
-            del o # leave it only in the cache
+            del o  # leave it only in the cache
 
         self.assertEqual(cache.cache_non_ghost_count, 100)
         self.assertEqual(cache.total_estimated_size, 64 * 100)
 
         cache.incrgc()
         self.assertEqual(cache.total_estimated_size, 64 * 6)
         self.assertEqual(cache.cache_non_ghost_count, 6)
         self.assertEqual(len(cache), 6)
 
         cache.full_sweep()
-        gc.collect() # banish the ghosts who are no longer in the ring
+        gc.collect()  # banish the ghosts who are no longer in the ring
         self.assertEqual(cache.total_estimated_size, 0)
         self.assertEqual(cache.cache_non_ghost_count, 0)
         self.assertEqual(len(cache), 0)
 
 
 class TestWeakValueDictionary(unittest.TestCase):
 
@@ -1307,25 +1319,27 @@
         return _WeakValueDictionary
 
     def _makeOne(self):
         return self._getTargetClass()()
 
     @unittest.skipIf(PYPY, "PyPy doesn't have the cleanup_hook")
     def test_cleanup_hook_gc(self):
-        # A more targeted test than ``test_interpreter_finalization_ffi_cleanup``
-        # See https://github.com/zopefoundation/persistent/issues/150
+        # A more targeted test than
+        # ``test_interpreter_finalization_ffi_cleanup`` See
+        # https://github.com/zopefoundation/persistent/issues/150
         wvd = self._makeOne()
 
         class cdata:
             o = object()
             pobj_id = id(o)
         wvd['key'] = cdata.o
 
         wvd.__dict__.clear()
         wvd.cleanup_hook(cdata)
 
 
 def test_suite():
     return unittest.defaultTestLoader.loadTestsFromName(__name__)
 
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `persistent-5.2/src/persistent/tests/test_ring.py` & `persistent-6.0/src/persistent/tests/test_ring.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,30 +11,29 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 import unittest
 
 from .. import ring
 
-# pylint:disable=protected-access
 
 class DummyPersistent:
     _p_oid = None
     _Persistent__ring = None
     __next_oid = 0
 
     @classmethod
     def _next_oid(cls):
         cls.__next_oid += 1
         return cls.__next_oid
 
     def __init__(self):
         self._p_oid = self._next_oid()
 
-    def __repr__(self): # pragma: no cover
+    def __repr__(self):  # pragma: no cover
         return "<Dummy {!r} at 0x{:x}>".format(self._p_oid, id(self))
 
 
 class CFFIRingTests(unittest.TestCase):
 
     def _getTargetClass(self):
         return ring._CFFIRing
@@ -113,15 +112,14 @@
             p1._Persistent__ring,
             p2._Persistent__ring,
             p3._Persistent__ring,
         ]
         self.assertEqual(3, len(r))
         self.assertEqual([p1, p2, p3], list(r))
 
-
         r.move_to_head(p1)
         self.assertEqual([p2, p3, p1], list(r))
 
         r.move_to_head(p3)
         self.assertEqual([p2, p1, p3], list(r))
 
         r.move_to_head(p3)
```

### Comparing `persistent-5.2/src/persistent/tests/test_timestamp.py` & `persistent-6.0/src/persistent/tests/test_timestamp.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 ##############################################################################
 import unittest
 from contextlib import contextmanager
 
 from persistent.tests.utils import skipIfNoCExtension
 
 
-
 class Test__UTC(unittest.TestCase):
 
     def _getTargetClass(self):
         from persistent.timestamp import _UTC
         return _UTC
 
     def _makeOne(self, *args, **kw):
@@ -62,28 +61,28 @@
                     (1, 2),
                     (1, 2, 3),
                     (1, 2, 3, 4),
                     (1, 2, 3, 4, 5),
                     ('1', '2', '3', '4', '5', '6'),
                     (1, 2, 3, 4, 5, 6, 7),
                     (b'123',),
-                   ]
+                    ]
         for args in BAD_ARGS:
             with self.assertRaises((TypeError, ValueError)):
                 self._makeOne(*args)
 
     def test_ctor_from_invalid_strings(self):
         BAD_ARGS = [''
                     '\x00',
                     '\x00' * 2,
                     '\x00' * 3,
                     '\x00' * 4,
                     '\x00' * 5,
                     '\x00' * 7,
-                   ]
+                    ]
         for args in BAD_ARGS:
             self.assertRaises((TypeError, ValueError), self._makeOne, *args)
 
     def test_ctor_from_string(self):
         from persistent.timestamp import _makeUTC
         ZERO = _makeUTC(1900, 1, 1, 0, 0, 0)
         EPOCH = _makeUTC(1970, 1, 1, 0, 0, 0)
@@ -153,14 +152,15 @@
     def test_repr(self):
         SERIAL = b'\x01' * 8
         ts = self._makeOne(SERIAL)
         self.assertEqual(repr(ts), repr(SERIAL))
 
     def test_comparisons_to_non_timestamps(self):
         import operator
+
         # Check the corner cases when comparing non-comparable types
         ts = self._makeOne(2011, 2, 16, 14, 37, 22.0)
 
         def check_common(op, passes):
             if passes == 'neither':
                 self.assertFalse(op(ts, None))
                 self.assertFalse(op(None, ts))
@@ -207,43 +207,41 @@
 
     MAX_32_BITS = 2 ** 31 - 1
     MAX_64_BITS = 2 ** 63 - 1
 
     def __init__(self):
         from persistent import timestamp as MUT
         self.MUT = MUT
-        # pylint:disable=protected-access
         self.orig_maxint = MUT._MAXINT
 
         self.is_32_bit_hash = self.orig_maxint == self.MAX_32_BITS
 
         self.orig_c_long = None
         self.c_int64 = None
         self.c_int32 = None
         if MUT.c_long is not None:
             import ctypes
             self.orig_c_long = MUT.c_long
             self.c_int32 = ctypes.c_int32
             self.c_int64 = ctypes.c_int64
             # win32, even on 64-bit long, has funny sizes
             self.is_32_bit_hash = self.c_int32 == ctypes.c_long
-        self.expected_hash = self.bit_32_hash if self.is_32_bit_hash else self.bit_64_hash
+        self.expected_hash = (
+            self.bit_32_hash if self.is_32_bit_hash else self.bit_64_hash)
 
     @contextmanager
     def _use_hash(self, maxint, c_long):
-        # pylint:disable=protected-access
         try:
             self.MUT._MAXINT = maxint
             self.MUT.c_long = c_long
             yield
         finally:
             self.MUT._MAXINT = self.orig_maxint
             self.MUT.c_long = self.orig_c_long
 
-
     def use_32bit(self):
         return self._use_hash(self.MAX_32_BITS, self.c_int32)
 
     def use_64bit(self):
         return self._use_hash(self.MAX_64_BITS, self.c_int64)
 
 
@@ -289,15 +287,16 @@
     """
 
     def _make_many_instants(self):
         # Given the above data, return many slight variations on
         # it to test matching
         yield Instant.now_ts_args
         for i in range(2000):
-            yield Instant.now_ts_args[:-1] + (Instant.now_ts_args[-1] + (i % 60.0)/100.0, )
+            yield Instant.now_ts_args[:-1] + (
+                Instant.now_ts_args[-1] + (i % 60.0) / 100.0, )
 
     def _makeC(self, *args, **kwargs):
         from persistent._compat import _c_optimizations_available as get_c
         return get_c()['persistent.timestamp'].TimeStamp(*args, **kwargs)
 
     def _makePy(self, *args, **kwargs):
         from persistent.timestamp import TimeStampPy
@@ -422,9 +421,10 @@
         self.test_seconds_precision(seconds=6.5555)
         self.test_seconds_precision(seconds=6.55555)
         self.test_seconds_precision(seconds=6.555555)
         self.test_seconds_precision(seconds=6.5555555)
         self.test_seconds_precision(seconds=6.55555555)
         self.test_seconds_precision(seconds=6.555555555)
 
+
 def test_suite():
     return unittest.defaultTestLoader.loadTestsFromName(__name__)
```

### Comparing `persistent-5.2/src/persistent/tests/test_wref.py` & `persistent-6.0/src/persistent/tests/test_wref.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,88 +38,88 @@
         self.assertTrue(wref._v_ob is target)
         self.assertEqual(wref.oid, b'OID')
         self.assertTrue(wref.dm is jar)
         self.assertEqual(wref.database_name, 'testing')
 
     def test___call___target_in_volatile(self):
         target = _makeTarget()
-        target._p_jar = jar = _makeJar()
+        target._p_jar = _makeJar()
         wref = self._makeOne(target)
         self.assertTrue(wref() is target)
 
     def test___call___target_in_jar(self):
         target = _makeTarget()
         target._p_jar = jar = _makeJar()
         jar[target._p_oid] = target
         wref = self._makeOne(target)
         del wref._v_ob
         self.assertTrue(wref() is target)
 
     def test___call___target_not_in_jar(self):
         target = _makeTarget()
-        target._p_jar = jar = _makeJar()
+        target._p_jar = _makeJar()
         wref = self._makeOne(target)
         del wref._v_ob
         self.assertTrue(wref() is None)
 
     def test___hash___w_target(self):
         target = _makeTarget()
-        target._p_jar = jar = _makeJar()
+        target._p_jar = _makeJar()
         wref = self._makeOne(target)
         self.assertEqual(hash(wref), hash(target))
 
     def test___hash___wo_target(self):
         target = _makeTarget()
-        target._p_jar = jar = _makeJar()
+        target._p_jar = _makeJar()
         wref = self._makeOne(target)
         del wref._v_ob
         self.assertRaises(TypeError, hash, wref)
 
     def test___eq___w_non_weakref(self):
         target = _makeTarget()
         lhs = self._makeOne(target)
         self.assertNotEqual(lhs, object())
         # Test belt-and-suspenders directly
         self.assertFalse(lhs.__eq__(object()))
 
     def test___eq___w_both_same_target(self):
         target = _makeTarget()
         lhs = self._makeOne(target)
-        rhs_target = _makeTarget()
+        _makeTarget()
         rhs = self._makeOne(target)
         self.assertEqual(lhs, rhs)
 
     def test___eq___w_both_different_targets(self):
         lhs_target = _makeTarget(oid='LHS')
         lhs = self._makeOne(lhs_target)
         rhs_target = _makeTarget(oid='RHS')
         rhs = self._makeOne(rhs_target)
         self.assertNotEqual(lhs, rhs)
 
     def test___eq___w_lhs_gone_target_not_in_jar(self):
         target = _makeTarget()
-        target._p_jar = jar = _makeJar()
+        target._p_jar = _makeJar()
         lhs = self._makeOne(target)
         del lhs._v_ob
         rhs = self._makeOne(target)
         self.assertRaises(TypeError, lambda: lhs == rhs)
 
     def test___eq___w_lhs_gone_target_in_jar(self):
         target = _makeTarget()
         target._p_jar = jar = _makeJar()
         jar[target._p_oid] = target
         lhs = self._makeOne(target)
         del lhs._v_ob
-        rhs_target = _makeTarget()
+        _makeTarget()
         rhs = self._makeOne(target)
         self.assertEqual(lhs, rhs)
 
     def test___eq___w_rhs_gone_target_not_in_jar(self):
         target = _makeTarget()
-        target._p_jar = jar = _makeJar()
+        target._p_jar = _makeJar()
         lhs = self._makeOne(target)
         rhs = self._makeOne(target)
         del rhs._v_ob
         self.assertRaises(TypeError, lambda: lhs == rhs)
 
     def test___eq___w_rhs_gone_target_in_jar(self):
         target = _makeTarget()
@@ -188,20 +188,20 @@
         VALUE3 = b'VALUE3'
         key = jar[KEY] = _makeTarget(oid=KEY)
         key._p_jar = jar
         kref = WeakRef(key)
         value = jar[VALUE] = _makeTarget(oid=VALUE)
         value._p_jar = jar
         key2 = _makeTarget(oid=KEY2)
-        key2._p_jar = jar # not findable
+        key2._p_jar = jar  # not findable
         kref2 = WeakRef(key2)
         del kref2._v_ob  # force a miss
         value2 = jar[VALUE2] = _makeTarget(oid=VALUE2)
         value2._p_jar = jar
-        key3 = jar[KEY3] = _makeTarget(oid=KEY3) # findable
+        key3 = jar[KEY3] = _makeTarget(oid=KEY3)  # findable
         key3._p_jar = jar
         kref3 = WeakRef(key3)
         del kref3._v_ob  # force a miss, but win in the lookup
         value3 = jar[VALUE3] = _makeTarget(oid=VALUE3)
         value3._p_jar = jar
         pwkd = self._makeOne(None)
         pwkd.__setstate__({'data':
@@ -223,14 +223,15 @@
     def test___getitem___miss(self):
         jar = _makeJar()
         key = jar['key'] = _makeTarget(oid='KEY')
         key._p_jar = jar
         value = jar['value'] = _makeTarget(oid='VALUE')
         value._p_jar = jar
         pwkd = self._makeOne(None)
+
         def _try():
             return pwkd[key]
         self.assertRaises(KeyError, _try)
 
     def test___delitem__(self):
         jar = _makeJar()
         key = jar['key'] = _makeTarget(oid='KEY')
@@ -244,14 +245,15 @@
     def test___delitem___miss(self):
         jar = _makeJar()
         key = jar['key'] = _makeTarget(oid='KEY')
         key._p_jar = jar
         value = jar['value'] = _makeTarget(oid='VALUE')
         value._p_jar = jar
         pwkd = self._makeOne(None)
+
         def _try():
             del pwkd[key]
         self.assertRaises(KeyError, _try)
 
     def test_get_miss_w_explicit_default(self):
         jar = _makeJar()
         key = jar['key'] = _makeTarget(oid='KEY')
@@ -274,15 +276,15 @@
         key._p_jar = jar
         value = jar['value'] = _makeTarget(oid='VALUE')
         value._p_jar = jar
         pwkd = self._makeOne([(key, value)])
         self.assertTrue(key in pwkd)
 
     def test___iter___empty(self):
-        jar = _makeJar()
+        _makeJar()
         pwkd = self._makeOne(None)
         self.assertEqual(list(pwkd), [])
 
     def test___iter___filled(self):
         jar = _makeJar()
         key = jar['key'] = _makeTarget(oid='KEY')
         key._p_jar = jar
@@ -312,27 +314,33 @@
         target = self._makeOne(None)
         target.update(source)
         self.assertTrue(target[key] is value)
 
 
 def _makeTarget(oid=b'OID'):
     from persistent import Persistent
+
     class Derived(Persistent):
         def __hash__(self):
             return hash(self._p_oid)
+
         def __eq__(self, other):
             return self._p_oid == other._p_oid
-        def __repr__(self): # pragma: no cover
+
+        def __repr__(self):  # pragma: no cover
             return 'Derived: %s' % self._p_oid
     derived = Derived()
     derived._p_oid = oid
     return derived
 
+
 def _makeJar():
     class _DB:
         database_name = 'testing'
+
     class _Jar(dict):
-        db = lambda self: _DB()
+        def db(self): return _DB()
     return _Jar()
 
+
 def test_suite():
     return unittest.defaultTestLoader.loadTestsFromName(__name__)
```

### Comparing `persistent-5.2/src/persistent/tests/utils.py` & `persistent-6.0/src/persistent/tests/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,62 +3,65 @@
     Jar that only supports registering objects so ``_p_changed``
     can be tested.
     """
 
     def register(self, ob):
         """Does nothing"""
 
+
 class ResettingJar:
     """Testing stub for _p_jar attribute.
     """
+
     def __init__(self):
-        from persistent import PickleCache # XXX stub it!
-        from persistent.interfaces import IPersistentDataManager
         from zope.interface import directlyProvides
+
+        from persistent import PickleCache  # XXX stub it!
+        from persistent.interfaces import IPersistentDataManager
         self.cache = self._cache = PickleCache(self)
         self.oid = 1
         self.registered = {}
         directlyProvides(self, IPersistentDataManager)
 
     def add(self, obj):
         import struct
         obj._p_oid = struct.pack(">Q", self.oid)
         self.oid += 1
         obj._p_jar = self
         self.cache[obj._p_oid] = obj
 
-
     # the following methods must be implemented to be a jar
 
     def setstate(self, obj):
         # Trivial setstate() implementation that just re-initializes
         # the object.  This isn't what setstate() is supposed to do,
         # but it suffices for the tests.
         obj.__class__.__init__(obj)
 
+
 class RememberingJar:
     """Testing stub for _p_jar attribute.
     """
+
     def __init__(self):
-        from persistent import PickleCache # XXX stub it!
+        from persistent import PickleCache  # XXX stub it!
         self.cache = PickleCache(self)
         self.oid = 1
         self.registered = {}
 
     def add(self, obj):
         import struct
         obj._p_oid = struct.pack(">Q", self.oid)
         self.oid += 1
         obj._p_jar = self
         self.cache[obj._p_oid] = obj
         # Remember object's state for later.
         self.obj = obj
         self.remembered = obj.__getstate__()
 
-
     def fake_commit(self):
         self.remembered = self.obj.__getstate__()
         self.obj._p_changed = 0
 
     # the following methods must be implemented to be a jar
 
     def register(self, obj):
@@ -70,14 +73,15 @@
         # This isn't what setstate() is supposed to do,
         # but it suffices for the tests.
         obj.__setstate__(self.remembered)
 
 
 def copy_test(self, obj):
     import copy
+
     # Test copy.copy. Do this first, because depending on the
     # version of Python, `UserDict.copy()` may wind up
     # mutating the original object's ``data`` (due to our
     # BWC with ``_container``). This shows up only as a failure
     # of coverage.
     obj.test = [1234]  # Make sure instance vars are also copied.
     obj_copy = copy.copy(obj)
@@ -91,17 +95,19 @@
     self.assertEqual(obj.data, obj_copy.data)
 
     return obj_copy
 
 
 def skipIfNoCExtension(o):
     import unittest
-    from persistent._compat import _should_attempt_c_optimizations
+
     from persistent._compat import _c_optimizations_available
     from persistent._compat import _c_optimizations_ignored
+    from persistent._compat import _should_attempt_c_optimizations
 
-    if _should_attempt_c_optimizations() and not _c_optimizations_available(): # pragma: no cover
+    if _should_attempt_c_optimizations(
+    ) and not _c_optimizations_available():  # pragma: no cover
         return unittest.expectedFailure(o)
     return unittest.skipIf(
         _c_optimizations_ignored() or not _c_optimizations_available(),
         "The C extension is not available"
     )(o)
```

### Comparing `persistent-5.2/src/persistent/timestamp.py` & `persistent-6.0/src/persistent/timestamp.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,84 +10,90 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 __all__ = ('TimeStamp',)
 
 import datetime
+import functools
 import math
 import struct
 import sys
-import functools
 from datetime import timezone
 
 from persistent._compat import use_c_impl
 
+
 _RAWTYPE = bytes
 _MAXINT = sys.maxsize
 
 _ZERO = b'\x00' * 8
 
 __all__ = [
     'TimeStamp',
     'TimeStampPy',
 ]
 
 try:
     # Make sure to overflow and wraparound just
     # like the C code does.
     from ctypes import c_long
-except ImportError: # pragma: no cover
+except ImportError:  # pragma: no cover
     # XXX: This is broken on 64-bit windows, where
     # sizeof(long) != sizeof(Py_ssize_t)
     # sizeof(long) == 4, sizeof(Py_ssize_t) == 8
     # It can be fixed by setting _MAXINT = 2 ** 31 - 1 on all
     # win32 platforms, but then that breaks PyPy3 64 bit for an unknown
     # reason.
     c_long = None
+
     def _wraparound(x):
-        return int(((x + (_MAXINT + 1)) & ((_MAXINT << 1) + 1)) - (_MAXINT + 1))
+        return int(((x + (_MAXINT + 1)) & ((_MAXINT << 1) + 1))
+                   - (_MAXINT + 1))
 else:
     def _wraparound(x):
         return c_long(x).value
 
 
 def _UTC():
     return timezone.utc
 
 
 def _makeUTC(y, mo, d, h, mi, s):
-    s = round(s, 6) # microsecond precision, to match the C implementation
+    s = round(s, 6)  # microsecond precision, to match the C implementation
     usec, sec = math.modf(s)
     sec = int(sec)
     usec = int(usec * 1e6)
     return datetime.datetime(y, mo, d, h, mi, sec, usec, tzinfo=_UTC())
 
+
 _EPOCH = _makeUTC(1970, 1, 1, 0, 0, 0)
 
-_TS_SECOND_BYTES_BIAS = 60.0 / (1<<16) / (1<<16)
+_TS_SECOND_BYTES_BIAS = 60.0 / (1 << 16) / (1 << 16)
+
 
 def _makeRaw(year, month, day, hour, minute, second):
     a = (((year - 1900) * 12 + month - 1) * 31 + day - 1)
     a = (a * 24 + hour) * 60 + minute
-    b = int(second / _TS_SECOND_BYTES_BIAS) # Don't round() this; the C version just truncates
+    # Don't round() this; the C version just truncates
+    b = int(second / _TS_SECOND_BYTES_BIAS)
     return struct.pack('>II', a, b)
 
+
 def _parseRaw(octets):
     a, b = struct.unpack('>II', octets)
     minute = a % 60
     hour = a // 60 % 24
     day = a // (60 * 24) % 31 + 1
     month = a // (60 * 24 * 31) % 12 + 1
     year = a // (60 * 24 * 31 * 12) + 1900
     second = b * _TS_SECOND_BYTES_BIAS
     return (year, month, day, hour, minute, second)
 
 
-
 @use_c_impl
 @functools.total_ordering
 class TimeStamp:
     __slots__ = ('_raw', '_elements')
 
     def __init__(self, *args):
         self._elements = None
@@ -95,19 +101,19 @@
             raw = args[0]
             if not isinstance(raw, _RAWTYPE):
                 raise TypeError('Raw octets must be of type: %s' % _RAWTYPE)
             if len(raw) != 8:
                 raise TypeError('Raw must be 8 octets')
             self._raw = raw
         elif len(args) == 6:
-            self._raw = _makeRaw(*args) # pylint:disable=no-value-for-parameter
-            # Note that we don't preserve the incoming arguments in self._elements,
-            # we derive them from the raw value. This is because the incoming
-            # seconds value could have more precision than would survive
-            # in the raw data, so we must be consistent.
+            self._raw = _makeRaw(*args)
+            # Note that we don't preserve the incoming arguments in
+            # self._elements, we derive them from the raw value. This is
+            # because the incoming seconds value could have more precision than
+            # would survive in the raw data, so we must be consistent.
         else:
             raise TypeError('Pass either a single 8-octet arg '
                             'or 5 integers and a float')
 
         self._elements = _parseRaw(self._raw)
 
     def raw(self):
@@ -151,15 +157,14 @@
 
         If self already qualifies, return self.
 
         Otherwise, return a new instance one moment later than 'other'.
         """
         if not isinstance(other, self.__class__):
             raise ValueError()
-        # pylint:disable=protected-access
         if self._raw > other._raw:
             return self
         a, b = struct.unpack('>II', other._raw)
         later = struct.pack('>II', a, b + 1)
         return self.__class__(later)
 
     def __eq__(self, other):
@@ -180,24 +185,24 @@
         x = a[0] << 7
         for i in a:
             x = (1000003 * x) ^ i
         x ^= 8
 
         x = _wraparound(x)
 
-        if x == -1: # pragma: no cover
+        if x == -1:  # pragma: no cover
             # The C version has this condition, but it's not clear
             # why; it's also not immediately obvious what bytestring
             # would generate this---hence the no-cover
             x = -2
         return x
 
     def __lt__(self, other):
         try:
             return self.raw() < other.raw()
         except AttributeError:
             return NotImplemented
 
 
-# This name is bound by the ``@use_c_impl`` decorator to the class defined above.
-# We make sure and list it statically, though, to help out linters.
-TimeStampPy = TimeStampPy # pylint:disable=undefined-variable,self-assigning-variable
+# This name is bound by the ``@use_c_impl`` decorator to the class defined
+# above. We make sure and list it statically, though, to help out linters.
+TimeStampPy = TimeStampPy  # noqa: F821 undefined name 'TimeStampPy'
```

### Comparing `persistent-5.2/src/persistent/wref.py` & `persistent-6.0/src/persistent/wref.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,18 @@
 #
 ##############################################################################
 """ZODB-based persistent weakrefs
 """
 
 from persistent import Persistent
 
+
 WeakRefMarker = object()
 
+
 class WeakRef:
     """Persistent weak references
 
     Persistent weak references are used much like Python weak
     references.  The major difference is that you can't specify an
     object to be called when the object is removed from the database.
     """
@@ -79,27 +81,27 @@
         if adict is not None:
             keys = getattr(adict, "keys", None)
             if keys is None:
                 adict = dict(adict)
             self.update(adict)
         # XXX 'kwargs' is pointless, because keys must be strings, but we
         #     are going to try (and fail) to wrap a WeakRef around them.
-        if kwargs: # pragma: no cover
+        if kwargs:  # pragma: no cover
             self.update(kwargs)
 
     def __getstate__(self):
         state = Persistent.__getstate__(self)
         state['data'] = list(state['data'].items())
         return state
 
     def __setstate__(self, state):
         state['data'] = {
             k: v for (k, v) in state['data']
             if k() is not None
-            }
+        }
         Persistent.__setstate__(self, state)
 
     def __setitem__(self, key, value):
         self.data[WeakRef(key)] = value
 
     def __getitem__(self, key):
         return self.data[WeakRef(key)]
```

### Comparing `persistent-5.2/src/persistent.egg-info/PKG-INFO` & `persistent-6.0/src/persistent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 Metadata-Version: 2.1
 Name: persistent
-Version: 5.2
+Version: 6.0
 Summary: Translucent persistent objects
 Home-page: https://github.com/zopefoundation/persistent/
 Author: Zope Foundation and Contributors
 Author-email: zodb-dev@zope.org
 License: ZPL 2.1
 Project-URL: Documentation, https://persistent.readthedocs.io
 Project-URL: Issue Tracker, https://github.com/zopefoundation/persistent/issues
 Project-URL: Sources, https://github.com/zopefoundation/persistent
 Classifier: Development Status :: 6 - Mature
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Framework :: ZODB
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 License-File: LICENSE.txt
+Requires-Dist: zope.deferredimport
 Requires-Dist: zope.interface
 Requires-Dist: cffi; platform_python_implementation == "CPython"
+Requires-Dist: cffi>=1.17.0rc1; platform_python_implementation == "CPython" and python_version >= "3.13a0"
 Provides-Extra: test
 Requires-Dist: zope.testrunner; extra == "test"
 Requires-Dist: manuel; extra == "test"
 Provides-Extra: testing
 Provides-Extra: docs
 Requires-Dist: Sphinx; extra == "docs"
 Requires-Dist: repoze.sphinx.autointerface; extra == "docs"
@@ -80,14 +81,22 @@
    version of  the ``persistent`` package.
 
 
 ==========================
  ``persistent`` Changelog
 ==========================
 
+6.0 (2024-05-30)
+================
+
+- Drop support for Python 3.7.
+
+- Build Windows wheels on GHA.
+
+
 5.2 (2024-02-16)
 ================
 
 - Add preliminary support for Python 3.13a3.
 
 
 5.1 (2023-10-05)
```

### Comparing `persistent-5.2/src/persistent.egg-info/SOURCES.txt` & `persistent-6.0/src/persistent.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -4,28 +4,38 @@
 .readthedocs.yaml
 CHANGES.rst
 CONTRIBUTING.md
 COPYRIGHT.txt
 LICENSE.txt
 MANIFEST.in
 README.rst
-appveyor.yml
 buildout.cfg
 setup.cfg
 setup.py
 tox.ini
 docs/Makefile
 docs/api.rst
 docs/changes.rst
 docs/conf.py
 docs/glossary.rst
 docs/index.rst
 docs/make.bat
 docs/requirements.txt
 docs/using.rst
+docs/_build/doctest/output.txt
+docs/_build/html/_sources/api.rst.txt
+docs/_build/html/_sources/changes.rst.txt
+docs/_build/html/_sources/glossary.rst.txt
+docs/_build/html/_sources/index.rst.txt
+docs/_build/html/_sources/using.rst.txt
+docs/_build/html/_sources/api/attributes.rst.txt
+docs/_build/html/_sources/api/cache.rst.txt
+docs/_build/html/_sources/api/collections.rst.txt
+docs/_build/html/_sources/api/interfaces.rst.txt
+docs/_build/html/_sources/api/pickling.rst.txt
 docs/api/attributes.rst
 docs/api/cache.rst
 docs/api/collections.rst
 docs/api/interfaces.rst
 docs/api/pickling.rst
 src/persistent/__init__.py
 src/persistent/_compat.h
```

### Comparing `persistent-5.2/tox.ini` & `persistent-6.0/tox.ini`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # Generated from:
 # https://github.com/zopefoundation/meta/tree/master/config/c-code
 [tox]
 minversion = 4.0
 envlist =
     lint
-    py37,py37-pure
     py38,py38-pure
     py39,py39-pure
     py310,py310-pure
     py311,py311-pure
     py312,py312-pure
     py313,py313-pure
     pypy3
     docs
     coverage
 
 [testenv]
 usedevelop = true
 pip_pre = py313: true
 deps =
+    setuptools < 69
     py37: urllib3 < 2
     Sphinx
 setenv =
     pure: PURE_PYTHON=1
     !pure-!pypy3: PURE_PYTHON=0
     py312: VIRTUALENV_PIP=23.1.2
     py312: PIP_REQUIRE_VIRTUALENV=0
@@ -41,15 +41,14 @@
     coverage
     py37: urllib3 < 2
 setenv =
     PURE_PYTHON=1
 commands =
     mkdir -p {toxinidir}/parts/htmlcov
     coverage run -m zope.testrunner --test-path=src {posargs:-vc}
-    python -c 'import os, subprocess; subprocess.check_call("coverage run -a -m zope.testrunner --test-path=src", env=dict(os.environ, PURE_PYTHON="1"), shell=True)'
     python -c 'import os, subprocess; subprocess.check_call("coverage run -a -m zope.testrunner --test-path=src", env=dict(os.environ, PURE_PYTHON="0"), shell=True)'
     coverage html -i
     coverage report -i -m --fail-under=99.8
 [testenv:release-check]
 description = ensure that the distribution is ready to release
 basepython = python3
 skip_install = true
@@ -58,25 +57,27 @@
     build
     check-manifest
     check-python-versions >= 0.20.0
     wheel
 commands_pre =
 commands =
     check-manifest
-    check-python-versions
+    check-python-versions --only setup.py,tox.ini,.github/workflows/tests.yml
     python -m build --sdist --no-isolation
     twine check dist/*
 
 [testenv:lint]
 basepython = python3
 skip_install = true
 deps =
     isort
+    flake8
 commands =
     isort --check-only --diff {toxinidir}/src {toxinidir}/setup.py
+    flake8 src setup.py
 
 [testenv:isort-apply]
 basepython = python3
 skip_install = true
 commands_pre =
 deps =
     isort
```

