# Comparing `tmp/BTrees-5.2.tar.gz` & `tmp/BTrees-6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BTrees-5.2.tar", last modified: Wed Feb  7 08:13:12 2024, max compression
+gzip compressed data, was "BTrees-6.0.tar", last modified: Thu May 30 09:10:27 2024, max compression
```

## Comparing `BTrees-5.2.tar` & `BTrees-6.0.tar`

### file list

```diff
@@ -1,112 +1,129 @@
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-07 08:13:12.545065 BTrees-5.2/
--rw-r--r--   0 m.howitz   (502) staff       (20)      580 2024-02-07 08:13:12.000000 BTrees-5.2/.coveragerc
--rwxr-xr-x   0 m.howitz   (502) staff       (20)     3348 2024-02-07 08:13:12.000000 BTrees-5.2/.manylinux-install.sh
--rwxr-xr-x   0 m.howitz   (502) staff       (20)      509 2024-02-07 08:13:12.000000 BTrees-5.2/.manylinux.sh
--rw-r--r--   0 m.howitz   (502) staff       (20)      664 2024-02-07 08:13:12.000000 BTrees-5.2/.readthedocs.yaml
--rw-r--r--   0 m.howitz   (502) staff       (20)    17667 2024-02-07 08:13:12.000000 BTrees-5.2/CHANGES.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      799 2024-02-07 08:13:12.000000 BTrees-5.2/CONTRIBUTING.md
--rw-r--r--   0 m.howitz   (502) staff       (20)       32 2024-02-07 08:13:12.000000 BTrees-5.2/COPYRIGHT.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2024-02-07 08:13:12.000000 BTrees-5.2/LICENSE.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)      530 2024-02-07 08:13:12.000000 BTrees-5.2/MANIFEST.in
--rw-r--r--   0 m.howitz   (502) staff       (20)    20940 2024-02-07 08:13:12.544940 BTrees-5.2/PKG-INFO
--rw-r--r--   0 m.howitz   (502) staff       (20)     1468 2024-02-07 08:13:12.000000 BTrees-5.2/README.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     1965 2024-02-07 08:13:12.000000 BTrees-5.2/appveyor.yml
--rw-r--r--   0 m.howitz   (502) staff       (20)      833 2024-02-07 08:13:12.000000 BTrees-5.2/buildout.cfg
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-07 08:13:12.530019 BTrees-5.2/docs/
--rw-r--r--   0 m.howitz   (502) staff       (20)     5564 2024-02-07 08:13:12.000000 BTrees-5.2/docs/Makefile
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-07 08:13:12.530361 BTrees-5.2/docs/_static/
--rw-r--r--   0 m.howitz   (502) staff       (20)      363 2024-02-07 08:13:12.000000 BTrees-5.2/docs/_static/custom.css
--rw-r--r--   0 m.howitz   (502) staff       (20)        0 2024-02-07 08:13:12.000000 BTrees-5.2/docs/_static/placeholder.txt
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-07 08:13:12.530518 BTrees-5.2/docs/_templates/
--rw-r--r--   0 m.howitz   (502) staff       (20)        0 2024-02-07 08:13:12.000000 BTrees-5.2/docs/_templates/placeholder.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)     3599 2024-02-07 08:13:12.000000 BTrees-5.2/docs/api.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       28 2024-02-07 08:13:12.000000 BTrees-5.2/docs/changes.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     8990 2024-02-07 08:13:12.000000 BTrees-5.2/docs/conf.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    17124 2024-02-07 08:13:12.000000 BTrees-5.2/docs/development.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      533 2024-02-07 08:13:12.000000 BTrees-5.2/docs/index.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     5096 2024-02-07 08:13:12.000000 BTrees-5.2/docs/make.bat
--rw-r--r--   0 m.howitz   (502) staff       (20)    21780 2024-02-07 08:13:12.000000 BTrees-5.2/docs/overview.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)       72 2024-02-07 08:13:12.000000 BTrees-5.2/docs/requirements.txt
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-07 08:13:12.525301 BTrees-5.2/include/
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-07 08:13:12.525370 BTrees-5.2/include/persistent/
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-07 08:13:12.531028 BTrees-5.2/include/persistent/persistent/
--rw-r--r--   0 m.howitz   (502) staff       (20)     1464 2024-02-07 08:13:12.000000 BTrees-5.2/include/persistent/persistent/_compat.h
--rw-r--r--   0 m.howitz   (502) staff       (20)     5105 2024-02-07 08:13:12.000000 BTrees-5.2/include/persistent/persistent/cPersistence.h
--rw-r--r--   0 m.howitz   (502) staff       (20)     2640 2024-02-07 08:13:12.000000 BTrees-5.2/include/persistent/persistent/ring.h
--rw-r--r--   0 m.howitz   (502) staff       (20)       88 2024-02-07 08:13:12.000000 BTrees-5.2/pyproject.toml
--rw-r--r--   0 m.howitz   (502) staff       (20)      563 2024-02-07 08:13:12.545982 BTrees-5.2/setup.cfg
--rw-r--r--   0 m.howitz   (502) staff       (20)     6790 2024-02-07 08:13:12.000000 BTrees-5.2/setup.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-07 08:13:12.525627 BTrees-5.2/src/
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-07 08:13:12.539750 BTrees-5.2/src/BTrees/
--rw-r--r--   0 m.howitz   (502) staff       (20)    24543 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/BTreeItemsTemplate.c
--rw-r--r--   0 m.howitz   (502) staff       (20)    24056 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/BTreeModuleTemplate.c
--rw-r--r--   0 m.howitz   (502) staff       (20)    75422 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/BTreeTemplate.c
--rw-r--r--   0 m.howitz   (502) staff       (20)    54931 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/BucketTemplate.c
--rw-r--r--   0 m.howitz   (502) staff       (20)    23750 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/Interfaces.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1937 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/Length.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    12070 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/MergeTemplate.c
--rw-r--r--   0 m.howitz   (502) staff       (20)    17264 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/SetOpTemplate.c
--rw-r--r--   0 m.howitz   (502) staff       (20)      281 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/SetOpTemplate.h
--rw-r--r--   0 m.howitz   (502) staff       (20)    19964 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/SetTemplate.c
--rw-r--r--   0 m.howitz   (502) staff       (20)    17788 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/TreeSetTemplate.c
--rw-r--r--   0 m.howitz   (502) staff       (20)     1010 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/_IFBTree.c
--rw-r--r--   0 m.howitz   (502) staff       (20)     1004 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/_IIBTree.c
--rw-r--r--   0 m.howitz   (502) staff       (20)      984 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/_IOBTree.c
--rw-r--r--   0 m.howitz   (502) staff       (20)     1047 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/_IUBTree.c
--rw-r--r--   0 m.howitz   (502) staff       (20)     1082 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/_LFBTree.c
--rw-r--r--   0 m.howitz   (502) staff       (20)     1073 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/_LLBTree.c
--rw-r--r--   0 m.howitz   (502) staff       (20)     1053 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/_LOBTree.c
--rw-r--r--   0 m.howitz   (502) staff       (20)     1115 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/_LQBTree.c
--rw-r--r--   0 m.howitz   (502) staff       (20)      984 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/_OIBTree.c
--rw-r--r--   0 m.howitz   (502) staff       (20)     1053 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/_OLBTree.c
--rw-r--r--   0 m.howitz   (502) staff       (20)      993 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/_OOBTree.c
--rw-r--r--   0 m.howitz   (502) staff       (20)     1091 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/_OQBTree.c
--rw-r--r--   0 m.howitz   (502) staff       (20)     1023 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/_OUBTree.c
--rw-r--r--   0 m.howitz   (502) staff       (20)     1118 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/_QFBTree.c
--rw-r--r--   0 m.howitz   (502) staff       (20)     1113 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/_QLBTree.c
--rw-r--r--   0 m.howitz   (502) staff       (20)     1089 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/_QOBTree.c
--rw-r--r--   0 m.howitz   (502) staff       (20)     1147 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/_QQBTree.c
--rw-r--r--   0 m.howitz   (502) staff       (20)     1050 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/_UFBTree.c
--rw-r--r--   0 m.howitz   (502) staff       (20)     1044 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/_UIBTree.c
--rw-r--r--   0 m.howitz   (502) staff       (20)     1032 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/_UOBTree.c
--rw-r--r--   0 m.howitz   (502) staff       (20)     1086 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/_UUBTree.c
--rw-r--r--   0 m.howitz   (502) staff       (20)     4169 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/__init__.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    52664 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/_base.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1163 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/_compat.h
--rw-r--r--   0 m.howitz   (502) staff       (20)     4072 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/_compat.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    13555 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/_datatypes.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     4673 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/_fsBTree.c
--rw-r--r--   0 m.howitz   (502) staff       (20)     7787 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/_module_builder.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    17421 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/check.py
--rw-r--r--   0 m.howitz   (502) staff       (20)      899 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/floatvaluemacros.h
--rw-r--r--   0 m.howitz   (502) staff       (20)     4072 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/intkeymacros.h
--rw-r--r--   0 m.howitz   (502) staff       (20)     4574 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/intvaluemacros.h
--rw-r--r--   0 m.howitz   (502) staff       (20)     1193 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/objectkeymacros.h
--rw-r--r--   0 m.howitz   (502) staff       (20)      460 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/objectvaluemacros.h
--rw-r--r--   0 m.howitz   (502) staff       (20)    15218 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/sorters.c
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-07 08:13:12.544054 BTrees-5.2/src/BTrees/tests/
--rw-r--r--   0 m.howitz   (502) staff       (20)       23 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/tests/__init__.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    11291 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/tests/_test_builder.py
--rw-r--r--   0 m.howitz   (502) staff       (20)   122582 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/tests/common.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    17867 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/tests/testBTrees.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    21207 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/tests/testConflict.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1629 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/tests/testPersistency.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     2462 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/tests/test_Length.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     5514 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/tests/test_OOBTree.py
--rw-r--r--   0 m.howitz   (502) staff       (20)   110865 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/tests/test__base.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     3126 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/tests/test__datatypes.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     2557 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/tests/test_btreesubclass.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    12511 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/tests/test_check.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1295 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/tests/test_compile_flags.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1791 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/tests/test_dynamic_btrees.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     2372 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/tests/test_fsBTree.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     2348 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/tests/test_utils.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1798 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees/utils.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-07 08:13:12.544280 BTrees-5.2/src/BTrees.egg-info/
--rw-r--r--   0 m.howitz   (502) staff       (20)    20940 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees.egg-info/PKG-INFO
--rw-r--r--   0 m.howitz   (502) staff       (20)     2432 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees.egg-info/SOURCES.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)        1 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees.egg-info/dependency_links.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)        1 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees.egg-info/not-zip-safe
--rw-r--r--   0 m.howitz   (502) staff       (20)      167 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees.egg-info/requires.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)        7 2024-02-07 08:13:12.000000 BTrees-5.2/src/BTrees.egg-info/top_level.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)     2127 2024-02-07 08:13:12.000000 BTrees-5.2/tox.ini
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 09:10:27.497218 BTrees-6.0/
+-rw-r--r--   0 jens       (501) staff       (20)      601 2024-05-30 07:01:26.000000 BTrees-6.0/.coveragerc
+-rwxr-xr-x   0 jens       (501) staff       (20)     3282 2024-05-30 07:01:26.000000 BTrees-6.0/.manylinux-install.sh
+-rwxr-xr-x   0 jens       (501) staff       (20)      509 2024-05-24 12:37:00.000000 BTrees-6.0/.manylinux.sh
+-rw-r--r--   0 jens       (501) staff       (20)      664 2024-05-24 12:37:00.000000 BTrees-6.0/.readthedocs.yaml
+-rw-r--r--   0 jens       (501) staff       (20)    17767 2024-05-30 07:01:42.000000 BTrees-6.0/CHANGES.rst
+-rw-r--r--   0 jens       (501) staff       (20)      799 2024-05-24 12:37:00.000000 BTrees-6.0/CONTRIBUTING.md
+-rw-r--r--   0 jens       (501) staff       (20)       32 2022-11-03 14:08:50.000000 BTrees-6.0/COPYRIGHT.txt
+-rw-r--r--   0 jens       (501) staff       (20)     2070 2022-11-03 14:08:50.000000 BTrees-6.0/LICENSE.txt
+-rw-r--r--   0 jens       (501) staff       (20)      509 2024-05-30 07:01:26.000000 BTrees-6.0/MANIFEST.in
+-rw-r--r--   0 jens       (501) staff       (20)    21041 2024-05-30 09:10:27.497146 BTrees-6.0/PKG-INFO
+-rw-r--r--   0 jens       (501) staff       (20)     1468 2022-11-16 09:58:56.000000 BTrees-6.0/README.rst
+-rw-r--r--   0 jens       (501) staff       (20)      833 2022-11-03 14:08:50.000000 BTrees-6.0/buildout.cfg
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 09:10:27.481210 BTrees-6.0/docs/
+-rw-r--r--   0 jens       (501) staff       (20)     5564 2022-11-03 14:08:50.000000 BTrees-6.0/docs/Makefile
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 09:10:27.476158 BTrees-6.0/docs/_build/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 09:10:27.481346 BTrees-6.0/docs/_build/doctest/
+-rw-r--r--   0 jens       (501) staff       (20)      382 2024-05-16 15:25:07.000000 BTrees-6.0/docs/_build/doctest/output.txt
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 09:10:27.476252 BTrees-6.0/docs/_build/html/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 09:10:27.482252 BTrees-6.0/docs/_build/html/_sources/
+-rw-r--r--   0 jens       (501) staff       (20)     3599 2022-11-03 14:08:50.000000 BTrees-6.0/docs/_build/html/_sources/api.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)       28 2022-11-03 14:08:50.000000 BTrees-6.0/docs/_build/html/_sources/changes.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)    17124 2022-11-03 14:08:50.000000 BTrees-6.0/docs/_build/html/_sources/development.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)      533 2022-11-03 14:08:50.000000 BTrees-6.0/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)    21780 2022-11-03 14:08:50.000000 BTrees-6.0/docs/_build/html/_sources/overview.rst.txt
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 09:10:27.482849 BTrees-6.0/docs/_build/html/_static/
+-rw-r--r--   0 jens       (501) staff       (20)    15094 2024-05-16 15:25:03.000000 BTrees-6.0/docs/_build/html/_static/basic.css
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 09:10:27.483261 BTrees-6.0/docs/_build/html/_static/css/
+-rw-r--r--   0 jens       (501) staff       (20)     3229 2023-04-20 08:47:07.000000 BTrees-6.0/docs/_build/html/_static/css/badge_only.css
+-rw-r--r--   0 jens       (501) staff       (20)   135314 2023-10-05 12:54:55.000000 BTrees-6.0/docs/_build/html/_static/css/theme.css
+-rw-r--r--   0 jens       (501) staff       (20)      363 2022-11-03 14:08:50.000000 BTrees-6.0/docs/_build/html/_static/custom.css
+-rw-r--r--   0 jens       (501) staff       (20)        0 2022-11-03 14:08:50.000000 BTrees-6.0/docs/_build/html/_static/placeholder.txt
+-rw-r--r--   0 jens       (501) staff       (20)     4929 2024-05-16 15:25:03.000000 BTrees-6.0/docs/_build/html/_static/pygments.css
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 09:10:27.483671 BTrees-6.0/docs/_static/
+-rw-r--r--   0 jens       (501) staff       (20)      363 2022-11-03 14:08:50.000000 BTrees-6.0/docs/_static/custom.css
+-rw-r--r--   0 jens       (501) staff       (20)        0 2022-11-03 14:08:50.000000 BTrees-6.0/docs/_static/placeholder.txt
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 09:10:27.483758 BTrees-6.0/docs/_templates/
+-rw-r--r--   0 jens       (501) staff       (20)        0 2022-11-03 14:08:50.000000 BTrees-6.0/docs/_templates/placeholder.txt
+-rw-r--r--   0 jens       (501) staff       (20)     3599 2022-11-03 14:08:50.000000 BTrees-6.0/docs/api.rst
+-rw-r--r--   0 jens       (501) staff       (20)       28 2022-11-03 14:08:50.000000 BTrees-6.0/docs/changes.rst
+-rw-r--r--   0 jens       (501) staff       (20)     9047 2024-05-16 15:22:02.000000 BTrees-6.0/docs/conf.py
+-rw-r--r--   0 jens       (501) staff       (20)    17124 2022-11-03 14:08:50.000000 BTrees-6.0/docs/development.rst
+-rw-r--r--   0 jens       (501) staff       (20)      533 2022-11-03 14:08:50.000000 BTrees-6.0/docs/index.rst
+-rw-r--r--   0 jens       (501) staff       (20)     5096 2022-11-03 14:08:50.000000 BTrees-6.0/docs/make.bat
+-rw-r--r--   0 jens       (501) staff       (20)    21780 2022-11-03 14:08:50.000000 BTrees-6.0/docs/overview.rst
+-rw-r--r--   0 jens       (501) staff       (20)       72 2023-10-05 09:12:23.000000 BTrees-6.0/docs/requirements.txt
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 09:10:27.476507 BTrees-6.0/include/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 09:10:27.476549 BTrees-6.0/include/persistent/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 09:10:27.484243 BTrees-6.0/include/persistent/persistent/
+-rw-r--r--   0 jens       (501) staff       (20)     1464 2023-10-05 09:12:23.000000 BTrees-6.0/include/persistent/persistent/_compat.h
+-rw-r--r--   0 jens       (501) staff       (20)     5105 2023-10-05 09:12:23.000000 BTrees-6.0/include/persistent/persistent/cPersistence.h
+-rw-r--r--   0 jens       (501) staff       (20)     2640 2023-10-05 09:12:23.000000 BTrees-6.0/include/persistent/persistent/ring.h
+-rw-r--r--   0 jens       (501) staff       (20)       88 2022-11-03 14:08:50.000000 BTrees-6.0/pyproject.toml
+-rw-r--r--   0 jens       (501) staff       (20)      581 2024-05-30 09:10:27.497428 BTrees-6.0/setup.cfg
+-rw-r--r--   0 jens       (501) staff       (20)     6714 2024-05-30 07:02:10.000000 BTrees-6.0/setup.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 09:10:27.476692 BTrees-6.0/src/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 09:10:27.494056 BTrees-6.0/src/BTrees/
+-rw-r--r--   0 jens       (501) staff       (20)    24543 2023-01-03 12:38:38.000000 BTrees-6.0/src/BTrees/BTreeItemsTemplate.c
+-rw-r--r--   0 jens       (501) staff       (20)    24056 2023-01-03 12:38:38.000000 BTrees-6.0/src/BTrees/BTreeModuleTemplate.c
+-rw-r--r--   0 jens       (501) staff       (20)    75422 2023-01-03 12:38:38.000000 BTrees-6.0/src/BTrees/BTreeTemplate.c
+-rw-r--r--   0 jens       (501) staff       (20)    54931 2023-01-03 12:38:38.000000 BTrees-6.0/src/BTrees/BucketTemplate.c
+-rw-r--r--   0 jens       (501) staff       (20)    24041 2024-05-30 07:01:26.000000 BTrees-6.0/src/BTrees/Interfaces.py
+-rw-r--r--   0 jens       (501) staff       (20)     1938 2024-05-16 15:22:02.000000 BTrees-6.0/src/BTrees/Length.py
+-rw-r--r--   0 jens       (501) staff       (20)    12070 2022-11-03 14:08:50.000000 BTrees-6.0/src/BTrees/MergeTemplate.c
+-rw-r--r--   0 jens       (501) staff       (20)    17264 2022-11-03 14:08:50.000000 BTrees-6.0/src/BTrees/SetOpTemplate.c
+-rw-r--r--   0 jens       (501) staff       (20)      281 2022-11-03 14:08:50.000000 BTrees-6.0/src/BTrees/SetOpTemplate.h
+-rw-r--r--   0 jens       (501) staff       (20)    19964 2023-01-03 12:38:38.000000 BTrees-6.0/src/BTrees/SetTemplate.c
+-rw-r--r--   0 jens       (501) staff       (20)    17788 2023-01-03 12:38:38.000000 BTrees-6.0/src/BTrees/TreeSetTemplate.c
+-rw-r--r--   0 jens       (501) staff       (20)     1010 2023-01-03 12:38:38.000000 BTrees-6.0/src/BTrees/_IFBTree.c
+-rw-r--r--   0 jens       (501) staff       (20)     1004 2023-01-03 12:38:38.000000 BTrees-6.0/src/BTrees/_IIBTree.c
+-rw-r--r--   0 jens       (501) staff       (20)      984 2023-01-03 12:38:38.000000 BTrees-6.0/src/BTrees/_IOBTree.c
+-rw-r--r--   0 jens       (501) staff       (20)     1047 2023-01-03 12:38:38.000000 BTrees-6.0/src/BTrees/_IUBTree.c
+-rw-r--r--   0 jens       (501) staff       (20)     1082 2023-01-03 12:38:38.000000 BTrees-6.0/src/BTrees/_LFBTree.c
+-rw-r--r--   0 jens       (501) staff       (20)     1073 2023-01-03 12:38:38.000000 BTrees-6.0/src/BTrees/_LLBTree.c
+-rw-r--r--   0 jens       (501) staff       (20)     1053 2023-01-03 12:38:38.000000 BTrees-6.0/src/BTrees/_LOBTree.c
+-rw-r--r--   0 jens       (501) staff       (20)     1115 2023-01-03 12:38:38.000000 BTrees-6.0/src/BTrees/_LQBTree.c
+-rw-r--r--   0 jens       (501) staff       (20)      984 2023-01-03 12:38:38.000000 BTrees-6.0/src/BTrees/_OIBTree.c
+-rw-r--r--   0 jens       (501) staff       (20)     1053 2023-01-03 12:38:38.000000 BTrees-6.0/src/BTrees/_OLBTree.c
+-rw-r--r--   0 jens       (501) staff       (20)      993 2023-01-03 12:38:38.000000 BTrees-6.0/src/BTrees/_OOBTree.c
+-rw-r--r--   0 jens       (501) staff       (20)     1091 2023-01-03 12:38:38.000000 BTrees-6.0/src/BTrees/_OQBTree.c
+-rw-r--r--   0 jens       (501) staff       (20)     1023 2023-01-03 12:38:38.000000 BTrees-6.0/src/BTrees/_OUBTree.c
+-rw-r--r--   0 jens       (501) staff       (20)     1118 2023-01-03 12:38:38.000000 BTrees-6.0/src/BTrees/_QFBTree.c
+-rw-r--r--   0 jens       (501) staff       (20)     1113 2023-01-03 12:38:38.000000 BTrees-6.0/src/BTrees/_QLBTree.c
+-rw-r--r--   0 jens       (501) staff       (20)     1089 2023-01-03 12:38:38.000000 BTrees-6.0/src/BTrees/_QOBTree.c
+-rw-r--r--   0 jens       (501) staff       (20)     1147 2023-01-03 12:38:38.000000 BTrees-6.0/src/BTrees/_QQBTree.c
+-rw-r--r--   0 jens       (501) staff       (20)     1050 2023-01-03 12:38:38.000000 BTrees-6.0/src/BTrees/_UFBTree.c
+-rw-r--r--   0 jens       (501) staff       (20)     1044 2023-01-03 12:38:38.000000 BTrees-6.0/src/BTrees/_UIBTree.c
+-rw-r--r--   0 jens       (501) staff       (20)     1032 2023-01-03 12:38:38.000000 BTrees-6.0/src/BTrees/_UOBTree.c
+-rw-r--r--   0 jens       (501) staff       (20)     1086 2023-01-03 12:38:38.000000 BTrees-6.0/src/BTrees/_UUBTree.c
+-rw-r--r--   0 jens       (501) staff       (20)     4202 2024-05-30 07:01:26.000000 BTrees-6.0/src/BTrees/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)    52318 2024-05-30 07:01:26.000000 BTrees-6.0/src/BTrees/_base.py
+-rw-r--r--   0 jens       (501) staff       (20)     1163 2023-01-03 12:38:38.000000 BTrees-6.0/src/BTrees/_compat.h
+-rw-r--r--   0 jens       (501) staff       (20)     4067 2024-05-30 07:01:26.000000 BTrees-6.0/src/BTrees/_compat.py
+-rw-r--r--   0 jens       (501) staff       (20)    13573 2024-05-30 07:01:26.000000 BTrees-6.0/src/BTrees/_datatypes.py
+-rw-r--r--   0 jens       (501) staff       (20)     4673 2023-01-03 12:38:38.000000 BTrees-6.0/src/BTrees/_fsBTree.c
+-rw-r--r--   0 jens       (501) staff       (20)     7812 2024-05-30 07:01:26.000000 BTrees-6.0/src/BTrees/_module_builder.py
+-rw-r--r--   0 jens       (501) staff       (20)    17442 2024-05-30 07:01:26.000000 BTrees-6.0/src/BTrees/check.py
+-rw-r--r--   0 jens       (501) staff       (20)      899 2022-11-03 14:08:50.000000 BTrees-6.0/src/BTrees/floatvaluemacros.h
+-rw-r--r--   0 jens       (501) staff       (20)     4072 2022-11-03 14:08:50.000000 BTrees-6.0/src/BTrees/intkeymacros.h
+-rw-r--r--   0 jens       (501) staff       (20)     4574 2022-11-03 14:08:50.000000 BTrees-6.0/src/BTrees/intvaluemacros.h
+-rw-r--r--   0 jens       (501) staff       (20)     1193 2023-01-03 12:38:38.000000 BTrees-6.0/src/BTrees/objectkeymacros.h
+-rw-r--r--   0 jens       (501) staff       (20)      460 2022-11-03 14:08:50.000000 BTrees-6.0/src/BTrees/objectvaluemacros.h
+-rw-r--r--   0 jens       (501) staff       (20)    15218 2022-11-03 14:08:50.000000 BTrees-6.0/src/BTrees/sorters.c
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 09:10:27.496628 BTrees-6.0/src/BTrees/tests/
+-rw-r--r--   0 jens       (501) staff       (20)       23 2022-11-03 14:08:50.000000 BTrees-6.0/src/BTrees/tests/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)    11390 2024-05-30 07:01:26.000000 BTrees-6.0/src/BTrees/tests/_test_builder.py
+-rw-r--r--   0 jens       (501) staff       (20)   123085 2024-05-30 07:01:26.000000 BTrees-6.0/src/BTrees/tests/common.py
+-rw-r--r--   0 jens       (501) staff       (20)    17851 2024-05-30 07:01:26.000000 BTrees-6.0/src/BTrees/tests/testBTrees.py
+-rw-r--r--   0 jens       (501) staff       (20)    21243 2024-05-30 07:01:26.000000 BTrees-6.0/src/BTrees/tests/testConflict.py
+-rw-r--r--   0 jens       (501) staff       (20)     1648 2024-05-16 15:22:02.000000 BTrees-6.0/src/BTrees/tests/testPersistency.py
+-rw-r--r--   0 jens       (501) staff       (20)     2463 2024-05-30 07:01:26.000000 BTrees-6.0/src/BTrees/tests/test_Length.py
+-rw-r--r--   0 jens       (501) staff       (20)     5642 2024-05-30 07:01:26.000000 BTrees-6.0/src/BTrees/tests/test_OOBTree.py
+-rw-r--r--   0 jens       (501) staff       (20)   110758 2024-05-30 07:01:26.000000 BTrees-6.0/src/BTrees/tests/test__base.py
+-rw-r--r--   0 jens       (501) staff       (20)     2811 2024-05-30 07:01:26.000000 BTrees-6.0/src/BTrees/tests/test__datatypes.py
+-rw-r--r--   0 jens       (501) staff       (20)     2586 2024-05-30 07:01:26.000000 BTrees-6.0/src/BTrees/tests/test_btreesubclass.py
+-rw-r--r--   0 jens       (501) staff       (20)    10996 2024-05-30 07:01:26.000000 BTrees-6.0/src/BTrees/tests/test_check.py
+-rw-r--r--   0 jens       (501) staff       (20)     1295 2022-11-03 14:08:50.000000 BTrees-6.0/src/BTrees/tests/test_compile_flags.py
+-rw-r--r--   0 jens       (501) staff       (20)     1739 2024-05-30 07:01:26.000000 BTrees-6.0/src/BTrees/tests/test_dynamic_btrees.py
+-rw-r--r--   0 jens       (501) staff       (20)     2376 2024-05-30 07:01:26.000000 BTrees-6.0/src/BTrees/tests/test_fsBTree.py
+-rw-r--r--   0 jens       (501) staff       (20)     2348 2023-01-03 12:38:38.000000 BTrees-6.0/src/BTrees/tests/test_utils.py
+-rw-r--r--   0 jens       (501) staff       (20)     1799 2024-05-30 07:01:26.000000 BTrees-6.0/src/BTrees/utils.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 09:10:27.494620 BTrees-6.0/src/BTrees.egg-info/
+-rw-r--r--   0 jens       (501) staff       (20)    21041 2024-05-30 09:10:27.000000 BTrees-6.0/src/BTrees.egg-info/PKG-INFO
+-rw-r--r--   0 jens       (501) staff       (20)     2892 2024-05-30 09:10:27.000000 BTrees-6.0/src/BTrees.egg-info/SOURCES.txt
+-rw-r--r--   0 jens       (501) staff       (20)        1 2024-05-30 09:10:27.000000 BTrees-6.0/src/BTrees.egg-info/dependency_links.txt
+-rw-r--r--   0 jens       (501) staff       (20)        1 2022-11-03 14:11:01.000000 BTrees-6.0/src/BTrees.egg-info/not-zip-safe
+-rw-r--r--   0 jens       (501) staff       (20)      167 2024-05-30 09:10:27.000000 BTrees-6.0/src/BTrees.egg-info/requires.txt
+-rw-r--r--   0 jens       (501) staff       (20)        7 2024-05-30 09:10:27.000000 BTrees-6.0/src/BTrees.egg-info/top_level.txt
+-rw-r--r--   0 jens       (501) staff       (20)     2215 2024-05-30 07:01:26.000000 BTrees-6.0/tox.ini
```

### Comparing `BTrees-5.2/.coveragerc` & `BTrees-6.0/.coveragerc`

 * *Files 20% similar despite different names*

```diff
@@ -11,14 +11,15 @@
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

### Comparing `BTrees-5.2/.manylinux-install.sh` & `BTrees-6.0/.manylinux-install.sh`

 * *Files 9% similar despite different names*

```diff
@@ -37,35 +37,33 @@
 export PURE_PYTHON=0
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

### Comparing `BTrees-5.2/.readthedocs.yaml` & `BTrees-6.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/CHANGES.rst` & `BTrees-6.0/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 ==================
  BTrees Changelog
 ==================
 
+6.0 (2024-05-30)
+================
+
+- Drop support for Python 3.7.
+
+- Build Windows wheels on GHA.
+
+
 5.2 (2024-02-07)
 ================
 
 - Add preliminary support for Python 3.13 as of 3.13a3.
 
 5.1 (2023-10-05)
 ================
```

### Comparing `BTrees-5.2/CONTRIBUTING.md` & `BTrees-6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/LICENSE.txt` & `BTrees-6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/PKG-INFO` & `BTrees-6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: BTrees
-Version: 5.2
+Version: 6.0
 Summary: Scalable persistent object containers
 Home-page: https://github.com/zopefoundation/BTrees
 Author: Zope Foundation
 Author-email: zodb-dev@zope.org
 License: ZPL 2.1
 Project-URL: Documentation, https://btrees.readthedocs.io
 Project-URL: Issue Tracker, https://github.com/zopefoundation/BTrees/issues
 Project-URL: Sources, https://github.com/zopefoundation/BTrees
 Platform: any
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
+Classifier: Programming Language :: Python :: 3.13
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
 Requires-Dist: persistent>=4.1.0
 Requires-Dist: zope.interface>=5.0.0
 Provides-Extra: test
 Requires-Dist: persistent>=4.4.3; extra == "test"
 Requires-Dist: transaction; extra == "test"
 Requires-Dist: zope.testrunner; extra == "test"
@@ -77,14 +77,22 @@
 further information.
 
 
 ==================
  BTrees Changelog
 ==================
 
+6.0 (2024-05-30)
+================
+
+- Drop support for Python 3.7.
+
+- Build Windows wheels on GHA.
+
+
 5.2 (2024-02-07)
 ================
 
 - Add preliminary support for Python 3.13 as of 3.13a3.
 
 5.1 (2023-10-05)
 ================
```

### Comparing `BTrees-5.2/README.rst` & `BTrees-6.0/README.rst`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/buildout.cfg` & `BTrees-6.0/buildout.cfg`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/docs/Makefile` & `BTrees-6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/docs/api.rst` & `BTrees-6.0/docs/_build/html/_sources/api.rst.txt`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/docs/conf.py` & `BTrees-6.0/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -270,12 +270,12 @@
 
 # How to display URL addresses: 'footnote', 'no', or 'inline'.
 #texinfo_show_urls = 'footnote'
 
 
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
-    'https://docs.python.org/3/': None,
-    'https://persistent.readthedocs.io/en/latest/': None,
-    "https://zodb.org/en/latest/": None,
-    "https://zopeinterface.readthedocs.io/en/latest/": None,
+    'python': ('https://docs.python.org/3/', None),
+    'persistent': ("https://persistent.readthedocs.io/en/latest/", None),
+    'zodb': ("https://zodb.org/en/latest/", None),
+    'zopeinterface': ("https://zopeinterface.readthedocs.io/en/latest/", None),
 }
```

### Comparing `BTrees-5.2/docs/development.rst` & `BTrees-6.0/docs/_build/html/_sources/development.rst.txt`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/docs/index.rst` & `BTrees-6.0/docs/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/docs/make.bat` & `BTrees-6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/docs/overview.rst` & `BTrees-6.0/docs/_build/html/_sources/overview.rst.txt`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/include/persistent/persistent/_compat.h` & `BTrees-6.0/include/persistent/persistent/_compat.h`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/include/persistent/persistent/cPersistence.h` & `BTrees-6.0/include/persistent/persistent/cPersistence.h`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/include/persistent/persistent/ring.h` & `BTrees-6.0/include/persistent/persistent/ring.h`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/setup.cfg` & `BTrees-6.0/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-[bdist_wheel]
-universal = 0
-
 [zest.releaser]
 create-wheel = no
 
 [flake8]
 doctests = 1
+per-file-ignores = 
+	src/BTrees/check.py: F401
 
 [check-manifest]
 ignore = 
 	.editorconfig
 	.meta.toml
 	docs/_build/html/_sources/*
 	docs/_build/doctest/*
```

### Comparing `BTrees-5.2/setup.py` & `BTrees-6.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,25 +10,26 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 
 import os
 import sys
-
 from distutils.errors import CCompilerError
 from distutils.errors import DistutilsExecError
 from distutils.errors import DistutilsPlatformError
 
 from setuptools import Extension
 from setuptools import find_packages
 from setuptools import setup
 from setuptools.command.build_ext import build_ext
 
-version = '5.2'
+
+version = '6.0'
+
 
 def _read(fname):
     here = os.path.abspath(os.path.dirname(__file__))
     with open(os.path.join(here, fname)) as f:
         return f.read()
 
 
@@ -61,14 +62,15 @@
         print('*' * 80)
         if 'bdist_wheel' in sys.argv and not os.environ.get("PURE_PYTHON"):
             # pip uses bdist_wheel by default, and hides the error output.
             # Let this error percolate up so the user can see it.
             # pip will then go ahead and run 'setup.py install' directly.
             raise
 
+
 # Set up dependencies for the BTrees package
 base_btrees_depends = [
     "src/BTrees/BTreeItemsTemplate.c",
     "src/BTrees/BTreeModuleTemplate.c",
     "src/BTrees/BTreeTemplate.c",
     "src/BTrees/BucketTemplate.c",
     "src/BTrees/MergeTemplate.c",
@@ -77,47 +79,47 @@
     "src/BTrees/TreeSetTemplate.c",
     "src/BTrees/sorters.c",
 ]
 
 FLAVORS = {
     "O": "object",
     "F": "float",
-    "I": "int", # Signed 32-bit
-    "L": "int", # Signed 64-bit
-    "U": "int", # Unsigned 32-bit
+    "I": "int",  # Signed 32-bit
+    "L": "int",  # Signed 64-bit
+    "U": "int",  # Unsigned 32-bit
     "Q": "int"  # Unsigned 64-bit (from the printf "q" modifier for quad_t)
 }
 # XXX should 'fs' be in ZODB instead?
 FAMILIES = (
     # Signed 32-bit keys
-    "IO", # object value
-    "II", # self value
-    "IF", # float value
-    "IU", # opposite sign value
+    "IO",  # object value
+    "II",  # self value
+    "IF",  # float value
+    "IU",  # opposite sign value
     # Unsigned 32-bit keys
-    "UO", # object value
-    "UU", # self value
-    "UF", # float value
-    "UI", # opposite sign value
+    "UO",  # object value
+    "UU",  # self value
+    "UF",  # float value
+    "UI",  # opposite sign value
     # Signed 64-bit keys
-    "LO", # object value
-    "LL", # self value
-    "LF", # float value
-    "LQ", # opposite sign value
+    "LO",  # object value
+    "LL",  # self value
+    "LF",  # float value
+    "LQ",  # opposite sign value
     # Unsigned 64-bit keys
-    "QO", # object value
-    "QQ", # self value
-    "QF", # float value
-    "QL", # opposite sign value
+    "QO",  # object value
+    "QQ",  # self value
+    "QF",  # float value
+    "QL",  # opposite sign value
     # Object keys
-    "OO", # object
-    "OI", # 32-bit signed
-    "OU", # 32-bit unsigned
-    "OL", # 64-bit signed
-    "OQ", # 64-bit unsigned
+    "OO",  # object
+    "OI",  # 32-bit signed
+    "OU",  # 32-bit unsigned
+    "OL",  # 64-bit signed
+    "OQ",  # 64-bit unsigned
     "fs",
 )
 
 KEY_H = "src/BTrees/%skeymacros.h"
 VALUE_H = "src/BTrees/%svaluemacros.h"
 
 
@@ -151,66 +153,67 @@
     # Our tests check for the new repr strings
     # generated in persistent 4.4.
     'persistent >= 4.4.3',
     'transaction',
     'zope.testrunner',
 ]
 
-setup(name='BTrees',
-      version=version,
-      description='Scalable persistent object containers',
-      long_description=README,
-      classifiers=[
-          "Development Status :: 6 - Mature",
-          "License :: OSI Approved :: Zope Public License",
-          "Programming Language :: Python",
-          "Programming Language :: Python :: 3",
-          "Programming Language :: Python :: 3.7",
-          "Programming Language :: Python :: 3.8",
-          "Programming Language :: Python :: 3.9",
-          "Programming Language :: Python :: 3.10",
-          "Programming Language :: Python :: 3.11",
-          "Programming Language :: Python :: 3.12",
-          "Programming Language :: Python :: Implementation :: CPython",
-          "Programming Language :: Python :: Implementation :: PyPy",
-          "Framework :: ZODB",
-          "Topic :: Database",
-          "Topic :: Software Development :: Libraries :: Python Modules",
-          "Operating System :: Microsoft :: Windows",
-          "Operating System :: Unix",
-      ],
-      author="Zope Foundation",
-      author_email="zodb-dev@zope.org",
-      url="https://github.com/zopefoundation/BTrees",
-      project_urls={
+setup(
+    name='BTrees',
+    version=version,
+    description='Scalable persistent object containers',
+    long_description=README,
+    classifiers=[
+        "Development Status :: 6 - Mature",
+        "License :: OSI Approved :: Zope Public License",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
+        "Programming Language :: Python :: 3.13",
+        "Programming Language :: Python :: Implementation :: CPython",
+        "Programming Language :: Python :: Implementation :: PyPy",
+        "Framework :: ZODB",
+        "Topic :: Database",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+        "Operating System :: Microsoft :: Windows",
+        "Operating System :: Unix",
+    ],
+    author="Zope Foundation",
+    author_email="zodb-dev@zope.org",
+    url="https://github.com/zopefoundation/BTrees",
+    project_urls={
         'Documentation': 'https://btrees.readthedocs.io',
         'Issue Tracker': 'https://github.com/zopefoundation/BTrees/issues',
         'Sources': 'https://github.com/zopefoundation/BTrees',
-      },
-      license="ZPL 2.1",
-      platforms=["any"],
-      packages=find_packages('src'),
-      package_dir={'': 'src'},
-      include_package_data=True,
-      zip_safe=False,
-      ext_modules=ext_modules,
-      extras_require={
-          'test': TESTS_REQUIRE,
-          'ZODB': [
-              'ZODB',
-          ],
-          'docs': [
-              'Sphinx',
-              'repoze.sphinx.autointerface',
-              'sphinx_rtd_theme',
-          ],
-      },
-      test_suite="BTrees.tests",
-      tests_require=TESTS_REQUIRE,
-      python_requires='>=3.7',
-      install_requires=REQUIRES,
-      cmdclass={
-          'build_ext': optional_build_ext,
-      },
-      entry_points="""\
-      """
+    },
+    license="ZPL 2.1",
+    platforms=["any"],
+    packages=find_packages('src'),
+    package_dir={'': 'src'},
+    include_package_data=True,
+    zip_safe=False,
+    ext_modules=ext_modules,
+    extras_require={
+        'test': TESTS_REQUIRE,
+        'ZODB': [
+            'ZODB',
+        ],
+        'docs': [
+            'Sphinx',
+            'repoze.sphinx.autointerface',
+            'sphinx_rtd_theme',
+        ],
+    },
+    test_suite="BTrees.tests",
+    tests_require=TESTS_REQUIRE,
+    python_requires='>=3.8',
+    install_requires=REQUIRES,
+    cmdclass={
+        'build_ext': optional_build_ext,
+    },
+    entry_points="""\
+    """
 )
```

### Comparing `BTrees-5.2/src/BTrees/BTreeItemsTemplate.c` & `BTrees-6.0/src/BTrees/BTreeItemsTemplate.c`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/src/BTrees/BTreeModuleTemplate.c` & `BTrees-6.0/src/BTrees/BTreeModuleTemplate.c`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/src/BTrees/BTreeTemplate.c` & `BTrees-6.0/src/BTrees/BTreeTemplate.c`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/src/BTrees/BucketTemplate.c` & `BTrees-6.0/src/BTrees/BucketTemplate.c`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/src/BTrees/Interfaces.py` & `BTrees-6.0/src/BTrees/Interfaces.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,21 +8,20 @@
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE
 #
 ##############################################################################
 
-from zope.interface import Interface, Attribute
+from zope.interface import Attribute
+from zope.interface import Interface
+from zope.interface.common.collections import IMapping
 from zope.interface.common.collections import ISized
 from zope.interface.common.sequence import IMinimalSequence
-from zope.interface.common.collections import IMapping
 
-# pylint:disable=inherit-non-class,no-method-argument,no-self-argument
-# pylint:disable=unexpected-special-method-signature
 
 class ICollection(Interface):
     """
     A collection of zero or more objects.
 
     In a boolean context, objects implementing this interface are
     `True` if the collection is non-empty, and `False` if the
@@ -33,14 +32,15 @@
         """Remove all of the items from the collection."""
 
 
 # Backwards compatibility alias. To be removed in 5.0.
 # Docs deprecated only in docs/api.rst.
 IReadSequence = IMinimalSequence
 
+
 class IKeyed(ICollection):
 
     def has_key(key):
         """Check whether the object has an item with the given key.
 
         Return a true value if the key is present, else a false value.
         """
@@ -178,14 +178,15 @@
         """
         As for :meth:`set.symmetric_difference_update`: Update this object,
         keeping only elements found in either set but not in both.
 
         .. versionadded:: 4.8.0
         """
 
+
 class IKeySequence(IKeyed, ISized):
 
     def __getitem__(index):
         """Return the key in the given index position.
 
         This allows iteration with for loops and use in functions,
         like map and list, that read sequences.
@@ -193,14 +194,15 @@
 
 
 class ISet(ISetMutable, IKeySequence):
     """
     A set of unique items stored in a single persistent object.
     """
 
+
 class ITreeSet(ISetMutable):
     """
     A set of unique items stored in a tree of persistent objects.
     """
 
 
 class IMinimalDictionary(IKeyed, IMapping):
@@ -210,39 +212,41 @@
     .. versionchanged:: 4.8.0
        Now extends :class:`zope.interface.common.collections.IMapping`.
     """
 
     def get(key, default):
         """Get the value associated with the given key.
 
-        Return the default if :meth:`~BTrees.Interfaces.IKeyed.has_key` is false
-        with the given key.
+        Return the default if :meth:`~BTrees.Interfaces.IKeyed.has_key` is
+        false with the given key.
         """
 
     def __getitem__(key):
         """Get the value associated with the given key.
 
-        Raise :class:`KeyError` if :meth:`~BTrees.Interfaces.IKeyed.has_key` is false
-        with the given key.
+        Raise :class:`KeyError` if :meth:`~BTrees.Interfaces.IKeyed.has_key`
+        is false with the given key.
         """
 
     def __setitem__(key, value):
         """Set the value associated with the given key."""
 
     def __delitem__(key):
         """Delete the value associated with the given key.
 
-        Raise class:`KeyError` if :meth:`~BTrees.Interfaces.IKeyed.has_key` is false
-        with the given key.
+        Raise class:`KeyError` if :meth:`~BTrees.Interfaces.IKeyed.has_key` is
+        false with the given key.
         """
 
     def values(min=None, max=None, excludemin=False, excludemax=False):
-        """
-        Return an :mod:`IMinimalSequence <zope.interface.common.sequence.IMinimalSequence>`
-        containing the values in the collection.
+        """ Return a minimal sequence containing the values in the collection.
+
+        Return value is an
+        :mod:`IMinimalSequence
+        <zope.interface.common.sequence.IMinimalSequence>`.
 
         The type of the ``IMinimalSequence`` is not specified. It
         could be a `list` or a `tuple` or some other type.
 
         All arguments are optional, and may be specified as keyword
         arguments, or by position.
 
@@ -289,14 +293,15 @@
         *excludemax is specified and true, is further constrained to
         items whose keys are strictly less than *max*. A *max* value
         of `None` is ignored. If *max* is `None` or not specified, and
         *excludemax* is true, the item with the largest key is
         excluded.
         """
 
+
 class IDictionaryIsh(IMinimalDictionary):
 
     def update(collection):
         """Add the items from the given collection object to the collection.
 
         The input collection must be a sequence of (key, value) 2-tuples,
         or an object with an 'items' method that returns a sequence of
@@ -310,28 +315,30 @@
         the minimum value.  This normalization may be a noop, but, for
         integer values, the normalization is division.
         """
 
     def setdefault(key, d):
         """D.setdefault(k, d) -> D.get(k, d), also set D[k]=d if k not in D.
 
-        Return the value like :meth:`~BTrees.Interfaces.IMinimalDictionary.get` except that if key is missing, d is both
-        returned and inserted into the dictionary as the value of k.
+        Return the value like
+        :meth:`~BTrees.Interfaces.IMinimalDictionary.get` except that if key
+        is missing, d is both returned and inserted into the dictionary as the
+        value of k.
 
         Note that, unlike as for Python's :meth:`dict.setdefault`, d is not
         optional.  Python defaults d to None, but that doesn't make sense
         for mappings that can't have None as a value (for example, an
         :class:`~BTrees.IIBTree.IIBTree` can have only integers as values).
         """
 
     def pop(key, d):
         """D.pop(k[, d]) -> v, remove key and return the corresponding value.
 
-        If key is not found, d is returned if given, otherwise :class:`KeyError` is
-        raised.
+        If key is not found, d is returned if given, otherwise
+        :class:`KeyError` is raised.
         """
 
     def popitem():
         """
         D.popitem() -> (k, v), remove and return some (key, value) pair
         as a 2-tuple; but raise KeyError if D is empty.
 
@@ -372,25 +379,29 @@
 
 class IMerge(Interface):
     """Object with methods for merging sets, buckets, and trees.
 
     These methods are supplied in modules that define collection
     classes with particular key and value types. The operations apply
     only to collections from the same module.  For example, the
-    :meth:`BTrees.IIBTree.IIBTree.union` can only be used with :class:`~BTrees.IIBTree.IIBTree`,
-    :class:`~BTrees.IIBTree.IIBucket`, :class:`~BTrees.IIBTree.IISet`, and :class:`~BTrees.IIBTree.IITreeSet`.
-
-    The number protocols methods ``__and__``, ``__or__`` and ``__sub__`` are provided
-    by all the data structures. They are shortcuts for :meth:`~BTrees.Interfaces.IMerge.intersection`,
-    :meth:`~BTrees.Interfaces.IMerge.union` and :meth:`~BTrees.Interfaces.IMerge.difference`.
-
-    The implementing module has a value type. The :class:`~BTrees.IOBTree.IOBTree` and :class:`~BTrees.OOBTree.OOBTree`
-    modules have object value type. The :class:`~BTrees.IIBTree.IIBTree` and :class:`~BTrees.OIBTree.OIBTree` modules
-    have integer value types. Other modules may be defined in the
-    future that have other value types.
+    :meth:`BTrees.IIBTree.IIBTree.union` can only be used with
+    :class:`~BTrees.IIBTree.IIBTree`, :class:`~BTrees.IIBTree.IIBucket`,
+    :class:`~BTrees.IIBTree.IISet`, and :class:`~BTrees.IIBTree.IITreeSet`.
+
+    The number protocols methods ``__and__``, ``__or__`` and ``__sub__`` are
+    provided by all the data structures. They are shortcuts for
+    :meth:`~BTrees.Interfaces.IMerge.intersection`,
+    :meth:`~BTrees.Interfaces.IMerge.union` and
+    :meth:`~BTrees.Interfaces.IMerge.difference`.
+
+    The implementing module has a value type. The
+    :class:`~BTrees.IOBTree.IOBTree` and :class:`~BTrees.OOBTree.OOBTree`
+    modules have object value type. The :class:`~BTrees.IIBTree.IIBTree` and
+    :class:`~BTrees.OIBTree.OIBTree` modules have integer value types. Other
+    modules may be defined in the future that have other value types.
 
     The individual types are classified into set (Set and TreeSet) and
     mapping (Bucket and BTree) types.
     """
 
     def difference(c1, c2):
         """Return the keys or items in c1 for which there is no key in c2.
@@ -543,49 +554,54 @@
         Note that c1 and c2 must be collections.
         """
 
 
 class IMergeIntegerKey(IMerge):
     """:class:`~BTrees.Interfaces.IMerge`-able objects with integer keys.
 
-    Concretely, this means the types in :class:`~BTree.IOBTree.IOBTree` and :class:`~BTrees.IIBTree.IIBTree`.
+    Concretely, this means the types in :class:`~BTree.IOBTree.IOBTree` and
+    :class:`~BTrees.IIBTree.IIBTree`.
     """
 
     def multiunion(seq):
         """Return union of (zero or more) integer sets, as an integer set.
 
         seq is a sequence of objects each convertible to an integer set.
         These objects are convertible to an integer set:
 
         + An integer, which is added to the union.
 
         + A Set or TreeSet from the same module (for example, an
-          :class:`BTrees.IIBTree.TreeSet` for :meth:`BTrees.IIBTree.multiunion`).  The elements of the
-          set are added to the union.
+          :class:`BTrees.IIBTree.TreeSet` for
+          :meth:`BTrees.IIBTree.multiunion`).  The elements of the set are
+          added to the union.
 
         + A Bucket or BTree from the same module (for example, an
-          :class:`BTrees.IOBTree.IOBTree` for :meth:`BTrees.IOBTree.multiunion`).  The keys of the
-          mapping are added to the union.
+          :class:`BTrees.IOBTree.IOBTree` for
+          :meth:`BTrees.IOBTree.multiunion`).  The keys of the mapping are
+          added to the union.
 
         + Any iterable Python object that iterates across integers. This
           will be slower than the above types.
 
         The union is returned as a Set from the same module (for example,
-        :meth:`BTrees.IIBTree.multiunion` returns an :class:`BTrees.IIBTree.IISet`).
+        :meth:`BTrees.IIBTree.multiunion` returns an
+        :class:`BTrees.IIBTree.IISet`).
 
-        The point to this method is that it can run much faster than
-        doing a sequence of two-input :meth:`~BTrees.Interfaces.IMerge.union` calls.  Under the covers,
-        all the integers in all the inputs are sorted via a single
-        linear-time radix sort, then duplicates are removed in a second
+        The point to this method is that it can run much faster than doing a
+        sequence of two-input :meth:`~BTrees.Interfaces.IMerge.union` calls.
+        Under the covers, all the integers in all the inputs are sorted via a
+        single linear-time radix sort, then duplicates are removed in a second
         linear-time pass.
 
         .. versionchanged:: 4.8.0
            Add support for arbitrary iterables of integers.
         """
 
+
 class IBTreeFamily(Interface):
     """the 64-bit or 32-bit family"""
     IF = Attribute('The IIntegerFloatBTreeModule for this family')
     II = Attribute('The IIntegerIntegerBTreeModule for this family')
     IO = Attribute('The IIntegerObjectBTreeModule for this family')
     IU = Attribute('The IIntegerUnsignedBTreeModule for this family')
 
@@ -604,84 +620,99 @@
 
 
 class _IMergeBTreeModule(IBTreeModule, IMerge):
     family = Attribute('The IBTreeFamily of this module')
 
 
 class IIntegerObjectBTreeModule(_IMergeBTreeModule):
-    """keys, or set values, are signed integers; values are objects.
+    """Keys, or set values, are signed ints; values are objects.
 
-    describes IOBTree and LOBTree"""
+    Describes IOBTree and LOBTree.
+    """
 
 
 class IUnsignedObjectBTreeModule(_IMergeBTreeModule):
-    """
-    As for :class:`~BTrees.Interfaces.IIntegerObjectBTreeModule` with unsigned integers.
+    """Keys, or set values, are unsigned ints; values are objects.
+
+    Describes UOBTree and QOBTree.
     """
 
 
 class IObjectIntegerBTreeModule(_IMergeBTreeModule):
-    """keys, or set values, are objects; values are signed integers.
+    """Keys, or set values, are objects; values are signed ints.
 
     Object keys (and set values) must sort reliably (for instance, *not* on
     object id)!  Homogenous key types recommended.
 
-    describes OIBTree and LOBTree"""
+    Describes OIBTree and OLBTree.
+    """
 
 
 class IObjectUnsignedBTreeModule(_IMergeBTreeModule):
-    """
-    As for `IObjectIntegerBTreeModule` with unsigned integers.
+    """Keys, or set values, are objects; values are signed ints.
+
+    Object keys (and set values) must sort reliably (for instance, *not* on
+    object id)!  Homogenous key types recommended.
+
+    Describes OUBTree and OQBTree.
     """
 
 
 class IIntegerIntegerBTreeModule(_IMergeBTreeModule, IMergeIntegerKey):
-    """keys, or set values, are signed integers; values are also signed integers.
+    """Keys, or set values, are signed integers; values are signed integers.
 
-    describes IIBTree and LLBTree"""
+    Describes IIBTree and LLBTree
+    """
 
 
 class IUnsignedUnsignedBTreeModule(_IMergeBTreeModule, IMergeIntegerKey):
-    """
-    As for `IIntegerIntegerBTreeModule` with unsigned integers.
+    """Keys, or set values, are unsigned ints; values are unsigned ints.
+
+    Describes UUBTree and QQBTree
     """
 
 
 class IUnsignedIntegerBTreeModule(_IMergeBTreeModule, IMergeIntegerKey):
-    """
-    As for `IIntegerIntegerBTreeModule` with unsigned integers for keys only.
+    """Keys, or set values, are unsigned ints; values are signed ints.
+
+    Describes UIBTree and QLBTree
     """
 
 
 class IIntegerUnsignedBTreeModule(_IMergeBTreeModule, IMergeIntegerKey):
-    """
-    As for `IIntegerIntegerBTreeModule` with unsigned integers for values only.
+    """Keys, or set values, are signed ints; values are unsigned ints.
+
+    Describes IUBTree and LQBTree
     """
 
 
 class IObjectObjectBTreeModule(IBTreeModule, IMerge):
-    """keys, or set values, are objects; values are also objects.
+    """Keys, or set values, are objects; values are also objects.
 
     Object keys (and set values) must sort reliably (for instance, *not* on
     object id)!  Homogenous key types recommended.
 
-    describes OOBTree"""
+    Note that there's no ``family`` attribute; all families include
+    the OO flavor of BTrees.
 
-    # Note that there's no ``family`` attribute; all families include
-    # the OO flavor of BTrees.
+    Describes OOBTree
+    """
 
 
 class IIntegerFloatBTreeModule(_IMergeBTreeModule):
-    """keys, or set values, are signed integers; values are floats.
+    """Keys, or set values, are signed ints; values are floats.
+
+    Describes IFBTree and LFBTree
+    """
 
-    describes IFBTree and LFBTree"""
 
 class IUnsignedFloatBTreeModule(_IMergeBTreeModule):
-    """
-    As for `IIntegerFloatBTreeModule` with unsigned integers.
+    """Keys, or set values, are unsigned ints; values are floats.
+
+    Describes UFBTree and QFBTree
     """
 
 
 try:
     from ZODB.POSException import BTreesConflictError
 except ImportError:
     class BTreesConflictError(ValueError):
```

### Comparing `BTrees-5.2/src/BTrees/Length.py` & `BTrees-6.0/src/BTrees/Length.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE
 #
 ##############################################################################
 
 import persistent
 
+
 class Length(persistent.Persistent):
     """BTree lengths are often too expensive to compute.
 
     Objects that use BTrees need to keep track of lengths themselves.
     This class provides an object for doing this.
 
     As a bonus, the object support application-level conflict
```

### Comparing `BTrees-5.2/src/BTrees/MergeTemplate.c` & `BTrees-6.0/src/BTrees/MergeTemplate.c`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/src/BTrees/SetOpTemplate.c` & `BTrees-6.0/src/BTrees/SetOpTemplate.c`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/src/BTrees/SetTemplate.c` & `BTrees-6.0/src/BTrees/SetTemplate.c`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/src/BTrees/TreeSetTemplate.c` & `BTrees-6.0/src/BTrees/TreeSetTemplate.c`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/src/BTrees/_IFBTree.c` & `BTrees-6.0/src/BTrees/_IFBTree.c`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/src/BTrees/_IIBTree.c` & `BTrees-6.0/src/BTrees/_IIBTree.c`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/src/BTrees/_IOBTree.c` & `BTrees-6.0/src/BTrees/_IOBTree.c`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/src/BTrees/_IUBTree.c` & `BTrees-6.0/src/BTrees/_IUBTree.c`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/src/BTrees/_LFBTree.c` & `BTrees-6.0/src/BTrees/_LFBTree.c`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/src/BTrees/_LLBTree.c` & `BTrees-6.0/src/BTrees/_LLBTree.c`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/src/BTrees/_LOBTree.c` & `BTrees-6.0/src/BTrees/_LOBTree.c`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/src/BTrees/_LQBTree.c` & `BTrees-6.0/src/BTrees/_LQBTree.c`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/src/BTrees/_OIBTree.c` & `BTrees-6.0/src/BTrees/_OIBTree.c`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/src/BTrees/_OLBTree.c` & `BTrees-6.0/src/BTrees/_OLBTree.c`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/src/BTrees/_OOBTree.c` & `BTrees-6.0/src/BTrees/_OOBTree.c`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/src/BTrees/_OQBTree.c` & `BTrees-6.0/src/BTrees/_OQBTree.c`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/src/BTrees/_OUBTree.c` & `BTrees-6.0/src/BTrees/_OUBTree.c`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/src/BTrees/_QFBTree.c` & `BTrees-6.0/src/BTrees/_QFBTree.c`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/src/BTrees/_QLBTree.c` & `BTrees-6.0/src/BTrees/_QLBTree.c`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/src/BTrees/_QOBTree.c` & `BTrees-6.0/src/BTrees/_QOBTree.c`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/src/BTrees/_QQBTree.c` & `BTrees-6.0/src/BTrees/_QQBTree.c`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/src/BTrees/_UFBTree.c` & `BTrees-6.0/src/BTrees/_UFBTree.c`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/src/BTrees/_UIBTree.c` & `BTrees-6.0/src/BTrees/_UIBTree.c`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/src/BTrees/_UOBTree.c` & `BTrees-6.0/src/BTrees/_UOBTree.c`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/src/BTrees/_UUBTree.c` & `BTrees-6.0/src/BTrees/_UUBTree.c`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/src/BTrees/__init__.py` & `BTrees-6.0/src/BTrees/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,56 +9,59 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 #############################################################################
 
 import sys
+
 import zope.interface
+
 import BTrees.Interfaces
+
 from ._module_builder import create_module
 
+
 __all__ = [
     'family32',
     'family64',
 ]
 
 _FAMILIES = (
     # Signed 32-bit keys
-    "IO", # object value
-    "II", # self value
-    "IF", # float value
-    "IU", # opposite sign value
+    "IO",  # object value
+    "II",  # self value
+    "IF",  # float value
+    "IU",  # opposite sign value
     # Unsigned 32-bit keys
-    "UO", # object value
-    "UU", # self value
-    "UF", # float value
-    "UI", # opposite sign value
+    "UO",  # object value
+    "UU",  # self value
+    "UF",  # float value
+    "UI",  # opposite sign value
     # Signed 64-bit keys
-    "LO", # object value
-    "LL", # self value
-    "LF", # float value
-    "LQ", # opposite sign value
+    "LO",  # object value
+    "LL",  # self value
+    "LF",  # float value
+    "LQ",  # opposite sign value
     # Unsigned 64-bit keys
-    "QO", # object value
-    "QQ", # self value
-    "QF", # float value
-    "QL", # opposite sign value
+    "QO",  # object value
+    "QQ",  # self value
+    "QF",  # float value
+    "QL",  # opposite sign value
     # Object keys
-    "OO", # object
-    "OI", # 32-bit signed
-    "OU", # 32-bit unsigned
-    "OL", # 64-bit signed
-    "OQ", # 64-bit unsigned
+    "OO",  # object
+    "OI",  # 32-bit signed
+    "OU",  # 32-bit unsigned
+    "OL",  # 64-bit signed
+    "OQ",  # 64-bit unsigned
     # Special purpose
-    'fs', # 2-byte -> 6-byte
+    'fs',  # 2-byte -> 6-byte
 )
 
-# XXX: Do this without completely ruining
-# pylint and other static analysis.
+# XXX: Do this without completely ruining static analysis.
 for family in _FAMILIES:
     mod = create_module(family)
     name = vars(mod)['__name__']
     sys.modules[name] = mod
     globals()[name.split('.', 1)[1]] = mod
     __all__.append(name)
 
@@ -82,57 +85,57 @@
         ).format(self._BITSIZE, self.minint, self.maxint, self.maxuint)
 
     def __repr__(self):
         return "<%s>" % (
             self
         )
 
+
 class _Family32(_Family):
     _BITSIZE = 32
-    from BTrees import OIBTree as OI
-    from BTrees import OUBTree as OU
-
     from BTrees import IFBTree as IF
     from BTrees import IIBTree as II
     from BTrees import IOBTree as IO
     from BTrees import IUBTree as IU
-
+    from BTrees import OIBTree as OI
+    from BTrees import OUBTree as OU
     from BTrees import UFBTree as UF
     from BTrees import UIBTree as UI
     from BTrees import UOBTree as UO
     from BTrees import UUBTree as UU
 
     def __reduce__(self):
         return _family32, ()
 
+
 class _Family64(_Family):
     _BITSIZE = 64
-    from BTrees import OLBTree as OI
-    from BTrees import OQBTree as OU
-
     from BTrees import LFBTree as IF
     from BTrees import LLBTree as II
     from BTrees import LOBTree as IO
     from BTrees import LQBTree as IU
-
+    from BTrees import OLBTree as OI
+    from BTrees import OQBTree as OU
     from BTrees import QFBTree as UF
     from BTrees import QLBTree as UI
     from BTrees import QOBTree as UO
     from BTrees import QQBTree as UU
 
     def __reduce__(self):
         return _family64, ()
 
+
 def _family32():
     return family32
-_family32.__safe_for_unpickling__ = True
+_family32.__safe_for_unpickling__ = True  # noqa E305
+
 
 def _family64():
     return family64
-_family64.__safe_for_unpickling__ = True
+_family64.__safe_for_unpickling__ = True  # noqa E305
 
 #: 32-bit BTree family.
 family32 = _Family32()
 
 #: 64-bit BTree family.
 family64 = _Family64()
```

### Comparing `BTrees-5.2/src/BTrees/_base.py` & `BTrees-6.0/src/BTrees/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,26 +12,17 @@
 #
 ##############################################################################
 """Python BTree implementation
 """
 
 from persistent import Persistent
 
-from .Interfaces import BTreesConflictError
 from ._compat import compare
+from .Interfaces import BTreesConflictError
 
-# XXX: Fix these. These ignores are temporary to
-# reduce the noise and help find specific issues during
-# refactoring
-# pylint:disable=too-many-lines,fixme,protected-access
-# pylint:disable=attribute-defined-outside-init,redefined-builtin,no-else-return
-# pylint:disable=redefined-outer-name,bad-continuation,unused-variable
-# pylint:disable=too-many-branches,too-many-statements,arguments-differ,assigning-non-slot
-# pylint:disable=superfluous-parens,inconsistent-return-statements,unidiomatic-typecheck
-# pylint:disable=deprecated-method,consider-using-enumerate
 
 _marker = object()
 
 
 class _Base(Persistent):
 
     __slots__ = ()
@@ -59,38 +50,44 @@
     except ImportError:  # pragma: no cover
         pass
     else:
         def __reduce__(self):
             # Swap out the type constructor for the C version, if present.
             func, typ_gna, state = Persistent.__reduce__(self)
             # We ignore the returned type altogether in favor of
-            # our calculated class (which allows subclasses but replaces our exact
-            # type with the C equivalent)
+            # our calculated class (which allows subclasses but replaces our
+            # exact type with the C equivalent)
             typ = self.__class__
             gna = typ_gna[1:]
             return (func, (typ,) + gna, state)
 
         @property
         def __class__(self):
             type_self = type(self)
-            return type_self._BTree_reduce_as if type_self._BTree_reduce_up_bound is type_self else type_self
+            return (
+                type_self._BTree_reduce_as
+                if type_self._BTree_reduce_up_bound is type_self
+                else type_self
+            )
 
         @property
         def _BTree_reduce_as(self):
             # Return the pickle replacement class for this object.
             # If the C extensions are available, this will be the
             # C type (setup by _fix_pickle), otherwise it will be the real
             # type of this object.
             # This implementation is replaced by _fix_pickle and exists for
             # testing purposes.
             return type(self)  # pragma: no cover
 
         _BTree_reduce_up_bound = _BTree_reduce_as
 
+
 class _ArithmeticMixin:
+
     def __sub__(self, other):
         return difference(self.__class__, self, other)
 
     def __rsub__(self, other):
         return difference(self._set_type, type(self)(other), self)
 
     def __or__(self, other):
@@ -107,18 +104,15 @@
         return (self - other) | (other - self)
 
     __rxor__ = __xor__
 
 
 class _BucketBase(_ArithmeticMixin, _Base):
 
-    __slots__ = ('_keys',
-                 '_next',
-                 '_to_key',
-                )
+    __slots__ = ('_keys', '_next', '_to_key')
 
     def clear(self):
         self._keys = self._key_type()
         self._next = None
 
     def __len__(self):
         return len(self._keys)
@@ -236,35 +230,35 @@
         name = type_self.__name__
         name = name[:-2] if name.endswith("Py") else name
         return "{}.{}({!r})".format(mod, name, items)
 
 
 class _SetIteration:
 
-    __slots__ = ('to_iterate',
-                 'useValues',
-                 '_iter',
-                 'active',
-                 'position',
-                 'key',
-                 'value',
-                )
-
+    __slots__ = (
+        'to_iterate',
+        'useValues',
+        '_iter',
+        'active',
+        'position',
+        'key',
+        'value',
+    )
 
     def __init__(self, to_iterate, useValues=False, default=None, sort=False):
         if to_iterate is None:
             to_iterate = ()
         self.to_iterate = to_iterate
         if sort:
             # Sorting is required for arbitrary iterables in the
             # set functions like difference/union/intersection
             assert not useValues
             if not isinstance(to_iterate, _Base):
-                # We know _Base (Set, Bucket, Tree, TreeSet) will all
-                # iterate in sorted order. Other than that, we have no guarantee.
+                # We know _Base (Set, Bucket, Tree, TreeSet) will all iterate
+                # in sorted order. Other than that, we have no guarantee.
                 self.to_iterate = to_iterate = sorted(self.to_iterate)
 
         if useValues:
             try:
                 itmeth = to_iterate.iteritems
             except AttributeError:
                 if isinstance(to_iterate, dict):
@@ -294,14 +288,15 @@
             self.position += 1
         except StopIteration:
             self.active = False
             self.position = -1
 
         return self
 
+
 class _MutableMappingMixin:
     # Methods defined in collections.abc.MutableMapping that
     # Bucket and Tree should both implement and can implement
     # the same. We don't want to extend that class though,
     # as the C version cannot.
     def popitem(self):
         """
@@ -317,17 +312,19 @@
         return key, value
 
 
 class Bucket(_MutableMappingMixin, _BucketBase):
 
     __slots__ = ()
     _value_type = list
-    _to_value = lambda self, x: x
     VALUE_SAME_CHECK = False
 
+    def _to_value(self, x):
+        return x
+
     def setdefault(self, key, value):
         key, value = self._to_key(key), self._to_value(value)
         status, value = self._set(key, value, True)
         return value
 
     def pop(self, key, default=_marker):
         try:
@@ -392,17 +389,18 @@
         Status is:
               None if no change
                   0 if change, but not size change
                   1 if change and size change
         """
         index = self._search(key)
         if index >= 0:
-            if (ifunset or
+            if (
+                ifunset or
                 self.VALUE_SAME_CHECK and value == self._values[index]
-                ):
+            ):
                 return None, self._values[index]
             self._p_changed = True
             self._values[index] = value
             return 0, value
         else:
             self._p_changed = True
             index = -index - 1
@@ -437,22 +435,26 @@
     def itervalues(self, *args, **kw):
         values = self._values
         return (values[i] for i in range(*self._range(*args, **kw)))
 
     def items(self, *args, **kw):
         keys = self._keys
         values = self._values
-        return [(keys[i], values[i])
-                    for i in range(*self._range(*args, **kw))]
+        return [
+            (keys[i], values[i])
+            for i in range(*self._range(*args, **kw))
+        ]
 
     def iteritems(self, *args, **kw):
         keys = self._keys
         values = self._values
-        return ((keys[i], values[i])
-                    for i in range(*self._range(*args, **kw)))
+        return (
+            (keys[i], values[i])
+            for i in range(*self._range(*args, **kw))
+        )
 
     def __getstate__(self):
         keys = self._keys
         values = self._values
         data = []
         for i in range(len(keys)):
             data.append(keys[i])
@@ -486,16 +488,18 @@
             b_old.__setstate__(s_old)
         b_com = type(self)()
         if s_com is not None:
             b_com.__setstate__(s_com)
         b_new = type(self)()
         if s_new is not None:
             b_new.__setstate__(s_new)
-        if (b_com._next != b_old._next or
-            b_new._next != b_old._next):
+        if (
+            b_com._next != b_old._next or
+            b_new._next != b_old._next
+        ):
             raise BTreesConflictError(-1, -1, -1, 0)
 
         if not b_com or not b_new:
             raise BTreesConflictError(-1, -1, -1, 12)
 
         i_old = _SetIteration(b_old, True)
         i_com = _SetIteration(b_com, True)
@@ -522,107 +526,108 @@
                     elif i_new.value == i_old.value:
                         result[i_old.key] = i_com.value
                     else:
                         raise merge_error(1)
                     i_old.advance()
                     i_com.advance()
                     i_new.advance()
-                elif (cmpON > 0): # insert in new
+                elif (cmpON > 0):  # insert in new
                     merge_output(i_new)
-                elif i_old.value == i_com.value: # deleted new
+                elif i_old.value == i_com.value:  # deleted new
                     if i_new.position == 1:
                         # Deleted the first item.  This will modify the
                         # parent node, so we don't know if merging will be
                         # safe
                         raise merge_error(13)
                     i_old.advance()
                     i_com.advance()
                 else:
                     raise merge_error(2)
             elif cmpON == 0:
-                if cmpOC > 0: # insert committed
+                if cmpOC > 0:  # insert committed
                     merge_output(i_com)
-                elif i_old.value == i_new.value: # delete committed
+                elif i_old.value == i_new.value:  # delete committed
                     if i_com.position == 1:
                         # Deleted the first item.  This will modify the
                         # parent node, so we don't know if merging will be
                         # safe
                         raise merge_error(13)
                     i_old.advance()
                     i_new.advance()
                 else:
                     raise merge_error(3)
-            else: # both keys changed
+            else:  # both keys changed
                 cmpCN = compare(i_com.key, i_new.key)
-                if cmpCN == 0: # dueling insert
+                if cmpCN == 0:  # dueling insert
                     raise merge_error(4)
-                if cmpOC > 0: # insert committed
-                    if cmpCN > 0: # insert i_new first
+                if cmpOC > 0:  # insert committed
+                    if cmpCN > 0:  # insert i_new first
                         merge_output(i_new)
                     else:
                         merge_output(i_com)
-                elif cmpON > 0: # insert i_new
+                elif cmpON > 0:  # insert i_new
                     merge_output(i_new)
                 else:
-                    raise merge_error(5) # both deleted same key
+                    raise merge_error(5)  # both deleted same key
 
-        while i_com.active and i_new.active: # new inserts
+        while i_com.active and i_new.active:  # new inserts
             cmpCN = compare(i_com.key, i_new.key)
             if cmpCN == 0:
-                raise merge_error(6) # dueling insert
-            if cmpCN > 0: # insert new
+                raise merge_error(6)  # dueling insert
+            if cmpCN > 0:  # insert new
                 merge_output(i_new)
-            else: # insert committed
+            else:  # insert committed
                 merge_output(i_com)
 
-        while i_old.active and i_com.active: # new deletes rest of original
+        while i_old.active and i_com.active:  # new deletes rest of original
             cmpOC = compare(i_old.key, i_com.key)
-            if cmpOC > 0: # insert committed
+            if cmpOC > 0:  # insert committed
                 merge_output(i_com)
-            elif cmpOC == 0 and (i_old.value == i_com.value): # del in new
+            elif cmpOC == 0 and (i_old.value == i_com.value):  # del in new
                 i_old.advance()
                 i_com.advance()
-            else: # dueling deletes or delete and change
+            else:  # dueling deletes or delete and change
                 raise merge_error(7)
 
         while i_old.active and i_new.active:
             # committed deletes rest of original
             cmpON = compare(i_old.key, i_new.key)
-            if cmpON > 0: # insert new
+            if cmpON > 0:  # insert new
                 merge_output(i_new)
             elif cmpON == 0 and (i_old.value == i_new.value):
                 # deleted in committed
                 i_old.advance()
                 i_new.advance()
-            else: # dueling deletes or delete and change
+            else:  # dueling deletes or delete and change
                 raise merge_error(8)
 
-        if i_old.active: # dueling deletes
+        if i_old.active:  # dueling deletes
             raise merge_error(9)
 
         while i_com.active:
             merge_output(i_com)
 
         while i_new.active:
             merge_output(i_new)
 
-        if len(result._keys) == 0: #pragma: no cover
+        if len(result._keys) == 0:  # pragma: no cover
             # If the output bucket is empty, conflict resolution doesn't have
             # enough info to unlink it from its containing BTree correctly.
             #
             # XXX TS, 2012-11-16:  I don't think this is possible
             #
             raise merge_error(10)
 
         result._next = b_old._next
         return result.__getstate__()
 
     def __repr__(self):
         return self._repr_helper(self.items())
 
+
 class _MutableSetMixin:
     # Like _MutableMappingMixin, but for sets.
     def isdisjoint(self, other):
         """
         Return True if two sets have a null intersection.
         """
         for value in other:
@@ -714,15 +719,14 @@
             state, self._next = state
         else:
             self._next = None
             state = state[0]
 
         self._keys.extend(state)
 
-
     def _set(self, key, value=None, ifunset=False):
         index = self._search(key)
         if index < 0:
             index = -index - 1
             self._p_changed = True
             self._keys.insert(index, key)
             return True, None
@@ -757,19 +761,21 @@
         b_com = type(self)()
         if s_com is not None:
             b_com.__setstate__(s_com)
         b_new = type(self)()
         if s_new is not None:
             b_new.__setstate__(s_new)
 
-        if (b_com._next != b_old._next or
-            b_new._next != b_old._next): # conflict: com or new changed _next
+        if (
+            b_com._next != b_old._next or
+            b_new._next != b_old._next
+        ):  # conflict: com or new changed _next
             raise BTreesConflictError(-1, -1, -1, 0)
 
-        if not b_com or not b_new: # conflict: com or new empty
+        if not b_com or not b_new:  # conflict: com or new empty
             raise BTreesConflictError(-1, -1, -1, 12)
 
         i_old = _SetIteration(b_old, True)
         i_com = _SetIteration(b_com, True)
         i_new = _SetIteration(b_new, True)
 
         def merge_error(reason):
@@ -782,122 +788,119 @@
             result._keys.append(it.key)
             it.advance()
 
         while i_old.active and i_com.active and i_new.active:
             cmpOC = compare(i_old.key, i_com.key)
             cmpON = compare(i_old.key, i_new.key)
             if cmpOC == 0:
-                if cmpON == 0: # all match
+                if cmpON == 0:  # all match
                     merge_output(i_old)
                     i_com.advance()
                     i_new.advance()
-                elif cmpON > 0: # insert in new
+                elif cmpON > 0:  # insert in new
                     merge_output(i_new)
-                else: # deleted new
+                else:  # deleted new
                     if i_new.position == 1:
                         # Deleted the first item.  This will modify the
                         # parent node, so we don't know if merging will be
                         # safe
                         raise merge_error(13)
                     i_old.advance()
                     i_com.advance()
             elif cmpON == 0:
-                if cmpOC > 0: # insert committed
+                if cmpOC > 0:  # insert committed
                     merge_output(i_com)
-                else: # delete committed
+                else:  # delete committed
                     if i_com.position == 1:
                         # Deleted the first item.  This will modify the
                         # parent node, so we don't know if merging will be
                         # safe
                         raise merge_error(13)
                     i_old.advance()
                     i_new.advance()
-            else: # both com and new keys changed
+            else:  # both com and new keys changed
                 cmpCN = compare(i_com.key, i_new.key)
-                if cmpCN == 0: # both inserted same key
+                if cmpCN == 0:  # both inserted same key
                     raise merge_error(4)
-                if cmpOC > 0: # insert committed
-                    if cmpCN > 0: # insert i_new first
+                if cmpOC > 0:  # insert committed
+                    if cmpCN > 0:  # insert i_new first
                         merge_output(i_new)
                     else:
                         merge_output(i_com)
-                elif cmpON > 0: # insert i_new
+                elif cmpON > 0:  # insert i_new
                     merge_output(i_new)
-                else: # both com and new deleted same key
+                else:  # both com and new deleted same key
                     raise merge_error(5)
 
-        while i_com.active and i_new.active: # new inserts
+        while i_com.active and i_new.active:  # new inserts
             cmpCN = compare(i_com.key, i_new.key)
-            if cmpCN == 0: # dueling insert
+            if cmpCN == 0:  # dueling insert
                 raise merge_error(6)
-            if cmpCN > 0: # insert new
+            if cmpCN > 0:  # insert new
                 merge_output(i_new)
-            else: # insert committed
+            else:  # insert committed
                 merge_output(i_com)
 
-        while i_old.active and i_com.active: # new deletes rest of original
+        while i_old.active and i_com.active:  # new deletes rest of original
             cmpOC = compare(i_old.key, i_com.key)
-            if cmpOC > 0: # insert committed
+            if cmpOC > 0:  # insert committed
                 merge_output(i_com)
-            elif cmpOC == 0: # del in new
+            elif cmpOC == 0:  # del in new
                 i_old.advance()
                 i_com.advance()
-            else: # dueling deletes or delete and change
+            else:  # dueling deletes or delete and change
                 raise merge_error(7)
 
         while i_old.active and i_new.active:
             # committed deletes rest of original
             cmpON = compare(i_old.key, i_new.key)
-            if cmpON > 0: # insert new
+            if cmpON > 0:  # insert new
                 merge_output(i_new)
-            elif cmpON == 0: # deleted in committed
+            elif cmpON == 0:  # deleted in committed
                 i_old.advance()
                 i_new.advance()
-            else: # dueling deletes or delete and change
+            else:  # dueling deletes or delete and change
                 raise merge_error(8)
 
-        if i_old.active: # dueling deletes
+        if i_old.active:  # dueling deletes
             raise merge_error(9)
 
         while i_com.active:
             merge_output(i_com)
 
         while i_new.active:
             merge_output(i_new)
 
-        if len(result._keys) == 0: #pragma: no cover
+        if len(result._keys) == 0:  # pragma: no cover
             # If the output bucket is empty, conflict resolution doesn't have
             # enough info to unlink it from its containing BTree correctly.
             #
             # XXX TS, 2012-11-16:  I don't think this is possible
             #
             raise merge_error(10)
 
         result._next = b_old._next
         return result.__getstate__()
 
     def __repr__(self):
         return self._repr_helper(self._keys)
 
+
 class _TreeItem:
 
-    __slots__ = ('key',
-                 'child',
-                )
+    __slots__ = ('key', 'child')
 
     def __init__(self, key, child):
         self.key = key
         self.child = child
 
 
 class _Tree(_ArithmeticMixin, _Base):
 
-    __slots__ = ('_data',
-                 '_firstbucket',
-                )
+    __slots__ = ('_data', '_firstbucket')
 
     def __new__(cls, *args):
         value = _Base.__new__(cls, *args)
         # Empty trees don't get their __setstate__ called upon
         # unpickling (or __init__, obviously), so clear() is never called
         # and _data and _firstbucket are never defined, unless we do it here.
         value._data = []
@@ -937,20 +940,20 @@
             self._data = []
         self._firstbucket = None
 
     def __bool__(self):
         return bool(self._data)
 
     def __len__(self):
-        l = 0
+        accumulated = 0
         bucket = self._firstbucket
         while bucket is not None:
-            l += len(bucket._keys)
+            accumulated += len(bucket._keys)
             bucket = bucket._next
-        return l
+        return accumulated
 
     @property
     def size(self):
         return len(self._data)
 
     def _search(self, key):
         data = self._data
@@ -1031,22 +1034,23 @@
             raise ValueError('empty tree')
         if max is _marker or max is None:
             return data[-1].child.maxKey()
 
         max = self._to_key(max)
         index = self._search(max)
         if index and compare(data[index].child.minKey(), max) > 0:
-            index -= 1 #pragma: no cover  no idea how to provoke this
+            index -= 1  # pragma: no cover  no idea how to provoke this
         return data[index].child.maxKey(max)
 
-
     def _set(self, key, value=None, ifunset=False):
-        if (self._p_jar is not None and
+        if (
+            self._p_jar is not None and
             self._p_oid is not None and
-            self._p_serial is not None):
+            self._p_serial is not None
+        ):
             self._p_jar.readCurrent(self)
         data = self._data
         if data:
             index = self._search(key)
             child = data[index].child
         else:
             index = 0
@@ -1065,18 +1069,20 @@
                 self._grow(child, index)
 
         # If a BTree contains only a single bucket, BTree.__getstate__()
         # includes the bucket's entire state, and the bucket doesn't get
         # an oid of its own.  So if we have a single oid-less bucket that
         # changed, it's *our* oid that should be marked as changed -- the
         # bucket doesn't have one.
-        if (grew is not None and
+        if (
+            grew is not None and
             type(child) is self._bucket_type and
             len(data) == 1 and
-            child._p_oid is None):
+            child._p_oid is None
+        ):
             self._p_changed = 1
         return result
 
     def _grow(self, child, index):
         self._p_changed = True
         new_child = child._split()
         self._data.insert(index+1, _TreeItem(new_child.minKey(), new_child))
@@ -1096,51 +1102,55 @@
             index = len(data) // 2
 
         next = type(self)()
         next._data = data[index:]
         first = data[index]
         del data[index:]
         if len(data) == 0:
-            self._firstbucket = None # lost our bucket, can't buy no beer
+            self._firstbucket = None  # lost our bucket, can't buy no beer
         if isinstance(first.child, type(self)):
             next._firstbucket = first.child._firstbucket
         else:
             next._firstbucket = first.child
         return next
 
     def _del(self, key):
-        if (self._p_jar is not None and
+        if (
+            self._p_jar is not None and
             self._p_oid is not None and
-            self._p_serial is not None):
+            self._p_serial is not None
+        ):
             self._p_jar.readCurrent(self)
 
         data = self._data
         if not data:
             raise KeyError(key)
 
         index = self._search(key)
         child = data[index].child
 
         removed_first_bucket, value = child._del(key)
 
         # See comment in _set about small trees
-        if (len(data) == 1 and
+        if (
+            len(data) == 1 and
             type(child) is self._bucket_type and
-            child._p_oid is None):
+            child._p_oid is None
+        ):
             self._p_changed = True
 
         # fix up the node key, but not for the 0'th one.
         if index > 0 and child.size and compare(key, data[index].key) == 0:
             self._p_changed = True
             data[index].key = child.minKey()
 
         if removed_first_bucket:
             if index:
                 data[index-1].child._deleteNextBucket()
-                removed_first_bucket = False # clear flag
+                removed_first_bucket = False  # clear flag
             else:
                 self._firstbucket = child._firstbucket
 
         if not child.size:
             if type(child) is self._bucket_type:
                 if index:
                     data[index-1].child._deleteNextBucket()
@@ -1159,21 +1169,21 @@
         data = self._data
 
         if not data:
             # Note: returning None here causes our __setstate__
             # to not be called on unpickling
             return None
 
-        if (len(data) == 1 and
+        if (
+            len(data) == 1 and
             type(data[0].child) is not type(self) and
             data[0].child._p_oid is None
-            ):
+        ):
             return ((data[0].child.__getstate__(), ), )
 
-
         data = iter(data)
         sdata = [next(data).child]
         for item in data:
             sdata.append(item.key)
             sdata.append(item.child)
 
         return tuple(sdata), self._firstbucket
@@ -1228,29 +1238,36 @@
         for i in data:
             assert_(i.child is not None, "BTree has NULL child")
             assert_(type(i.child) is child_class,
                     "BTree children have different types")
             assert_(i.child.size, "Bucket length < 1")
 
         if child_class is type(self):
-            assert_(self._firstbucket is data[0].child._firstbucket,
-                    "BTree has firstbucket different than "
-                    "its first child's firstbucket")
+            assert_(
+                self._firstbucket is data[0].child._firstbucket,
+                "BTree has firstbucket different than "
+                "its first child's firstbucket"
+            )
             for i in range(len(data)-1):
                 data[i].child._check(data[i+1].child._firstbucket)
             data[-1].child._check(nextbucket)
         elif child_class is self._bucket_type:
-            assert_(self._firstbucket is data[0].child,
-                    "Bottom-level BTree node has inconsistent firstbucket "
-                    "belief")
+            assert_(
+                self._firstbucket is data[0].child,
+                "Bottom-level BTree node has inconsistent firstbucket belief"
+            )
             for i in range(len(data)-1):
-                assert_(data[i].child._next is data[i+1].child,
-                       "Bucket next pointer is damaged")
-            assert_(data[-1].child._next is nextbucket,
-                    "Bucket next pointer is damaged")
+                assert_(
+                    data[i].child._next is data[i+1].child,
+                    "Bucket next pointer is damaged"
+                )
+            assert_(
+                data[-1].child._next is nextbucket,
+                "Bucket next pointer is damaged"
+            )
         else:
             assert_(False, "Incorrect child type")
 
     def _p_resolveConflict(self, old, com, new):
         s_old = _get_simple_btree_bucket_state(old)
         s_com = _get_simple_btree_bucket_state(com)
         s_new = _get_simple_btree_bucket_state(new)
@@ -1264,15 +1281,15 @@
 
 
 def _get_simple_btree_bucket_state(state):
     if state is None:
         return state
     if not isinstance(state, tuple):
         raise TypeError("_p_resolveConflict: expected tuple or None for state")
-    if len(state) == 2: # non-degenerate BTree, can't resolve
+    if len(state) == 2:  # non-degenerate BTree, can't resolve
         raise BTreesConflictError(-1, -1, -1, 11)
     # Peel away wrapper to get to only-bucket state.
     if len(state) != 1:
         raise TypeError("_p_resolveConflict: expected 1- or 2-tuple for state")
     state = state[0]
     if not isinstance(state, tuple) or len(state) != 1:
         raise TypeError("_p_resolveConflict: expected 1-tuple containing "
@@ -1281,22 +1298,23 @@
     if not isinstance(state, tuple):
         raise TypeError("_p_resolveConflict: expected tuple for bucket state")
     return state
 
 
 class _TreeItems:
 
-    __slots__ = ('firstbucket',
-                 'itertype',
-                 'iterargs',
-                 'index',
-                 'it',
-                 'v',
-                 '_len',
-                )
+    __slots__ = (
+        'firstbucket',
+        'itertype',
+        'iterargs',
+        'index',
+        'it',
+        'v',
+        '_len',
+    )
 
     def __init__(self, firstbucket, itertype, iterargs):
         self.firstbucket = firstbucket
         self.itertype = itertype
         self.iterargs = iterargs
         self.index = -1
         self.it = iter(self)
@@ -1348,15 +1366,15 @@
             bucket = bucket._next
             done = 1
 
 
 class _TreeIterator:
     """ Faux implementation for BBB only.
     """
-    def __init__(self, items): #pragma: no cover
+    def __init__(self, items):  # pragma: no cover
         raise TypeError(
             "TreeIterators are private implementation details "
             "of the C-based BTrees.\n\n"
             "Please use 'iter(tree)', rather than instantiating "
             "one directly."
         )
 
@@ -1448,21 +1466,25 @@
 def difference(set_type, o1, o2):
     if o1 is None or o2 is None:
         return o1
     i1 = _SetIteration(o1, True, 0)
     i2 = _SetIteration(o2, False, 0, True)
     if i1.useValues:
         result = o1._mapping_type()
+
         def copy(i):
             result._keys.append(i.key)
             result._values.append(i.value)
+
     else:
         result = o1._set_type()
+
         def copy(i):
             result._keys.append(i.key)
+
     while i1.active and i2.active:
         cmp_ = compare(i1.key, i2.key)
         if cmp_ < 0:
             copy(i1)
             i1.advance()
         elif cmp_ == 0:
             i1.advance()
@@ -1470,24 +1492,27 @@
         else:
             i2.advance()
     while i1.active:
         copy(i1)
         i1.advance()
     return result
 
+
 def union(set_type, o1, o2):
     if o1 is None:
         return o2
     if o2 is None:
         return o1
     i1 = _SetIteration(o1, False, 0, True)
     i2 = _SetIteration(o2, False, 0, True)
     result = set_type()
+
     def copy(i):
         result._keys.append(i.key)
+
     while i1.active and i2.active:
         cmp_ = compare(i1.key, i2.key)
         if cmp_ < 0:
             copy(i1)
             i1.advance()
         elif cmp_ == 0:
             copy(i1)
@@ -1500,44 +1525,49 @@
         copy(i1)
         i1.advance()
     while i2.active:
         copy(i2)
         i2.advance()
     return result
 
+
 def intersection(set_type, o1, o2):
     if o1 is None:
         return o2
     if o2 is None:
         return o1
     i1 = _SetIteration(o1, False, 0, True)
     i2 = _SetIteration(o2, False, 0, True)
     result = set_type()
+
     def copy(i):
         result._keys.append(i.key)
+
     while i1.active and i2.active:
         cmp_ = compare(i1.key, i2.key)
         if cmp_ < 0:
             i1.advance()
         elif cmp_ == 0:
             copy(i1)
             i1.advance()
             i2.advance()
         else:
             i2.advance()
     return result
 
+
 def _prepMergeIterators(o1, o2):
     MERGE_DEFAULT = getattr(o1, 'MERGE_DEFAULT', None)
     if MERGE_DEFAULT is None:
         raise TypeError("invalid set operation")
     i1 = _SetIteration(o1, True, MERGE_DEFAULT)
     i2 = _SetIteration(o2, True, MERGE_DEFAULT)
     return i1, i2
 
+
 def weightedUnion(set_type, o1, o2, w1=1, w2=1):
     if o1 is None:
         if o2 is None:
             return 0, None
         return w2, o2
     if o2 is None:
         return w1, o1
@@ -1546,21 +1576,25 @@
     if MERGE is None and i1.useValues and i2.useValues:
         raise TypeError("invalid set operation")
     MERGE_WEIGHT = getattr(o1, 'MERGE_WEIGHT')
     if (not i1.useValues) and i2.useValues:
         i1, i2 = i2, i1
         w1, w2 = w2, w1
     _merging = i1.useValues or i2.useValues
+
     if _merging:
         result = o1._mapping_type()
+
         def copy(i, w):
             result._keys.append(i.key)
             result._values.append(MERGE_WEIGHT(i.value, w))
+
     else:
         result = o1._set_type()
+
         def copy(i, w):
             result._keys.append(i.key)
 
     while i1.active and i2.active:
         cmp_ = compare(i1.key, i2.key)
         if cmp_ < 0:
             copy(i1, w1)
@@ -1578,14 +1612,15 @@
         copy(i1, w1)
         i1.advance()
     while i2.active:
         copy(i2, w2)
         i2.advance()
     return 1, result
 
+
 def weightedIntersection(set_type, o1, o2, w1=1, w2=1):
     if o1 is None:
         if o2 is None:
             return 0, None
         return w2, o2
     if o2 is None:
         return w1, o1
@@ -1613,14 +1648,15 @@
             i2.advance()
         else:
             i2.advance()
     if isinstance(result, (Set, TreeSet)):
         return w1 + w2, result
     return 1, result
 
+
 def multiunion(set_type, seqs):
     # XXX simple/slow implementation. Goal is just to get tests to pass.
     result = set_type()
     for s in seqs:
         try:
             iter(s)
         except TypeError:
@@ -1628,31 +1664,34 @@
         result.update(s)
     return result
 
 
 def MERGE(self, value1, weight1, value2, weight2):
     return (value1 * weight1) + (value2 * weight2)
 
+
 def MERGE_WEIGHT_default(self, value, weight):
     return value
 
+
 def MERGE_WEIGHT_numeric(self, value, weight):
     return value * weight
 
+
 def _fix_pickle(mod_dict, mod_name):
     # Make the pure-Python objects pickle with the same
     # class names and types as the C extensions by setting the appropriate
     # _BTree_reduce_as attribute.
     # If the C extensions are not available, we also change the
     # __name__ attribute of the type to match the C name (otherwise
     # we wind up with *Py in the pickles)
     # Each module must call this as `_fix_pickle(globals(), __name__)`
     # at the bottom.
 
-    mod_prefix = mod_name.split('.')[-1][:2] # BTrees.OOBTree -> 'OO'
+    mod_prefix = mod_name.split('.')[-1][:2]  # BTrees.OOBTree -> 'OO'
     bucket_name = mod_prefix + 'Bucket'
     py_bucket_name = bucket_name + 'Py'
 
     have_c_extensions = mod_dict[bucket_name] is not mod_dict[py_bucket_name]
 
     for name in 'Bucket', 'Set', 'BTree', 'TreeSet', 'TreeIterator':
         raw_name = mod_prefix + name
@@ -1660,27 +1699,27 @@
         try:
             py_type = mod_dict[py_name]
         except KeyError:
             if name == 'TreeIterator':
                 # Optional
                 continue
             raise  # pragma: no cover
-        raw_type = mod_dict[raw_name] # Could be C or Python
+        raw_type = mod_dict[raw_name]  # Could be C or Python
 
         py_type._BTree_reduce_as = raw_type
         py_type._BTree_reduce_up_bound = py_type
 
         if not have_c_extensions:  # pragma: no cover
             # Set FooPy to have the __name__ of simply Foo.
             # We can't do this if the C extension is available,
             # because then mod_dict[FooPy.__name__] is not FooPy
             # and pickle refuses to save something like that.
             # On the other hand (no C extension) this makes our
             # Python pickle match the C version by default
             py_type.__name__ = raw_name
-            py_type.__qualname__ = raw_name # Py 3.3+
+            py_type.__qualname__ = raw_name  # Py 3.3+
 
 
 # tp_name returns full name of a type in the same way as how it is provided by
 # typ->tp_name in C.
 def _tp_name(typ):
     return '.'.join([typ.__module__, typ.__name__])
```

### Comparing `BTrees-5.2/src/BTrees/_compat.h` & `BTrees-6.0/src/BTrees/_compat.h`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/src/BTrees/_compat.py` & `BTrees-6.0/src/BTrees/_compat.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,35 +10,38 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE
 #
 ##############################################################################
 import os
 import sys
 
+
 PYPY = hasattr(sys, 'pypy_version_info')
 
+
 def compare(x, y):
     if x is None:
         if y is None:
             return 0
         else:
             return -1
     elif y is None:
         return 1
     else:
         return (x > y) - (y > x)
 
+
 def _ascii(x):
     return bytes(x, 'ascii')
 
+
 def _c_optimizations_required():
-    """
-    Return a true value if the C optimizations are required.
+    """Return a true value if the C optimizations are required.
 
-    This uses the ``PURE_PYTHON`` variable as documented in `import_c_extension`.
+    Uses the ``PURE_PYTHON`` variable as documented in `import_c_extension`.
     """
     pure_env = os.environ.get('PURE_PYTHON')
     require_c = pure_env == "0"
     return require_c
 
 
 def _c_optimizations_available(module_name):
@@ -51,15 +54,15 @@
 
     This does not say whether they should be used or not.
     """
     import importlib
     catch = () if _c_optimizations_required() else (ImportError,)
     try:
         return importlib.import_module('BTrees._' + module_name)
-    except catch: # pragma: no cover
+    except catch:  # pragma: no cover
         return False
 
 
 def _c_optimizations_ignored():
     """
     The opposite of `_c_optimizations_required`.
     """
```

### Comparing `BTrees-5.2/src/BTrees/_datatypes.py` & `BTrees-6.0/src/BTrees/_datatypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,23 +11,20 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """
 Descriptions of the datatypes supported by this package.
 """
 
-from operator import index as operator__index__
-from struct import Struct
-from struct import error as struct_error
-
-from abc import ABC
+import abc
+import operator
+import struct
 
 from .utils import Lazy
 
-# pylint:disable=raise-missing-from
 
 class DataType:
     """
     Describes a data type used as a value.
 
     Subclasses will be defined for each particular
     supported type.
@@ -74,15 +71,15 @@
 
         The coercion rules will vary by datatype. This exists only
         for test cases. The default is to perform the same validation
         as ``__call__``.
         """
         return self(item)
 
-    def apply_weight(self, item, weight): # pylint:disable=unused-argument
+    def apply_weight(self, item, weight):
         """
         Apply a *weight* multiplier to *item*.
 
         Used when merging data structures. The *item* will be a
         value.
         """
         return item
@@ -172,18 +169,17 @@
     def __call__(self, item):
         return item
 
     def supports_value_union(self):
         return False
 
 
-
-class _HasDefaultComparison(ABC):
+class _HasDefaultComparison(abc.ABC):
     """
-    An `ABC <https://docs.python.org/3/library/abc.html>_` for
+    An `abc.ABC <https://docs.python.org/3/library/abc.html>_` for
     checking whether an item has default comparison.
 
     All we have to do is override ``__subclasshook__`` to implement an
     algorithm determining whether a class has default comparison.
     Python and the ABC machinery will take care of translating
     ``isinstance(thing, _HasDefaultComparison)`` into something like
     ``_HasDefaultComparison.__subclasshook__(type(thing))``. The ABC
@@ -213,21 +209,23 @@
             if defining_class is None:
                 # Implemented in Python
                 return False
             return C.__lt__.__objclass__ is object
     else:
         # PyPy3
         @classmethod
-        def __subclasshook__(cls, C, _object_lt=object.__lt__, _NoneType=type(None)):
+        def __subclasshook__(
+            cls, C, _object_lt=object.__lt__, _NoneType=type(None)
+        ):
             if C is _NoneType:
                 return False
             return C.__lt__ is _object_lt
 
 
-class O(KeyDataType):
+class O(KeyDataType):  # noqa E742
     """
     Arbitrary (sortable) Python objects.
     """
     long_name = 'Object'
     tree_size = 250
     default_bucket_size = 60
 
@@ -235,52 +233,57 @@
         return Any()
 
     def supports_value_union(self):
         return False
 
     def __call__(self, item):
         if isinstance(item, _HasDefaultComparison):
-            raise TypeError("Object of class {} has default comparison".format(type(item).__name__))
+            raise TypeError(
+                "Object of class {} has default comparison".format(
+                    type(item).__name__
+                )
+            )
         return item
 
 
 class _AbstractNativeDataType(KeyDataType):
     """
     Uses `struct.Struct` to verify that the data can fit into a native
     type.
     """
 
     _struct_format = None
     _as_python_type = NotImplementedError
     _required_python_type = object
     _error_description = None
-    _as_packable = operator__index__ # calls ``obj.__index__`` to yield integer
+    _as_packable = operator.index
 
     @Lazy
     def _check_native(self):
-        return Struct(self._struct_format).pack
+        return struct.Struct(self._struct_format).pack
 
     def __call__(self, item):
         try:
-            self._check_native(self._as_packable(item)) # pylint:disable=too-many-function-args
-        except (struct_error, TypeError, ValueError):
+            self._check_native(self._as_packable(item))
+        except (struct.error, TypeError, ValueError):
             # PyPy can raise ValueError converting a negative number to a
             # unsigned value.
             if isinstance(item, int):
                 raise TypeError("Value out of range", item)
             raise TypeError(self._error_description)
 
         return self._as_python_type(item)
 
     def apply_weight(self, item, weight):
         return item * weight
 
     def supports_value_union(self):
         return True
 
+
 class _AbstractIntDataType(_AbstractNativeDataType):
     _as_python_type = int
     _required_python_type = int
     multiplication_identity = 1
     long_name = "Integer"
 
     def getTwoExamples(self):
@@ -304,35 +307,38 @@
         return 0
 
     def get_upper_bound(self):
         exp = 64 if self.using64bits else 32
         return int(2 ** exp - 1)
 
 
-class I(_AbstractIntDataType):
+class I(_AbstractIntDataType):  # noqa E742
     _struct_format = 'i'
     _error_description = "32-bit integer expected"
 
 
 class U(_AbstractUIntDataType):
     _struct_format = 'I'
     _error_description = 'non-negative 32-bit integer expected'
 
 
 class F(_AbstractNativeDataType):
     _struct_format = 'f'
     _as_python_type = float
     _error_description = 'float expected'
-    _as_packable = lambda self, k: k # identity
     multiplication_identity = 1.0
     long_name = 'Float'
 
+    def _as_packable(self, k):  # identity
+        return k
+
     def getTwoExamples(self):
         return 0.5, 1.5
 
+
 class L(_AbstractIntDataType):
     _struct_format = 'q'
     _error_description = '64-bit integer expected'
     using64bits = True
 
 
 class Q(_AbstractUIntDataType):
@@ -349,15 +355,17 @@
     """
     tree_size = 500
     default_bucket_size = 500
     _length = None
 
     def __call__(self, item):
         if not isinstance(item, bytes) or len(item) != self._length:
-            raise TypeError("{}-byte array expected, not {!r}".format(self._length, item))
+            raise TypeError(
+                "{}-byte array expected, not {!r}".format(self._length, item)
+            )
         return item
 
     def supports_value_union(self):
         # We don't implement 'multiunion' for fsBTree.
         return False
 
 
@@ -375,23 +383,23 @@
     prefix_code = 'f'
     _length = 2
 
     # Check it can be converted to a two-byte
     # value. Note that even though we allow negative values
     # that can break test assumptions: -1 < 0 < 1, but the byte
     # values for those are \xff\xff > \x00\x00 < \x00\x01.
-    _as_2_bytes = Struct('>h').pack
+    _as_2_bytes = struct.Struct('>h').pack
 
     def coerce(self, item):
         try:
             return self(item)
         except TypeError:
             try:
-                return self._as_2_bytes(operator__index__(item))
-            except struct_error as e:
+                return self._as_2_bytes(operator.index(item))
+            except struct.error as e:
                 raise TypeError(e)
 
     @staticmethod
     def _make_Bucket_toString():
         def toString(self):
             return b''.join(self._keys) + b''.join(self._values)
         return toString
@@ -414,14 +422,15 @@
         return fromString
 
     def add_extra_methods(self, base_name, cls):
         if base_name == 'Bucket':
             cls.toString = self._make_Bucket_toString()
             cls.fromString = self._make_Bucket_fromString()
 
+
 class s(_AbstractBytes):
     """
     The value type for an ``fs`` tree.
 
     This is a 6-byte suffix of an overall 8-byte value
     like a ZODB object ID or transaction ID.
     """
@@ -436,21 +445,25 @@
         # Negative values have the high bit set, which is incompatible
         # with our transformation.
         return 0
 
     # To coerce an integer, as used in tests, first convert to 8 bytes
     # in big-endian order, then ensure the first two
     # are 0 and cut them off.
-    _as_8_bytes = Struct('>q').pack
+    _as_8_bytes = struct.Struct('>q').pack
 
     def coerce(self, item):
         try:
             return self(item)
         except TypeError:
             try:
-                as_bytes = self._as_8_bytes(operator__index__(item))
-            except struct_error as e:
+                as_bytes = self._as_8_bytes(operator.index(item))
+            except struct.error as e:
                 raise TypeError(e)
 
             if as_bytes[:2] != b'\x00\x00':
-                raise TypeError("Cannot convert {!r} to 6 bytes ({!r})".format(item, as_bytes))
+                raise TypeError(
+                    "Cannot convert {!r} to 6 bytes ({!r})".format(
+                        item, as_bytes
+                    )
+                )
             return as_bytes[2:]
```

### Comparing `BTrees-5.2/src/BTrees/_fsBTree.c` & `BTrees-6.0/src/BTrees/_fsBTree.c`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/src/BTrees/_module_builder.py` & `BTrees-6.0/src/BTrees/_module_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,29 +12,29 @@
 #
 ##############################################################################
 """
 Support functions to eliminate the boilerplate involved in defining
 BTree modules.
 """
 import sys
-from zope.interface import directlyProvides
+
 from zope.interface import classImplements
+from zope.interface import directlyProvides
 
 
 def _create_classes(
         module_name, key_datatype, value_datatype,
 ):
+    from ._base import MERGE  # Won't always want this.
     from ._base import Bucket
-    from ._base import MERGE # Won't always want this.
     from ._base import Set
     from ._base import Tree
     from ._base import TreeSet
     from ._base import _TreeItems as TreeItems
     from ._base import _TreeIterator
-    from ._base import _fix_pickle
 
     classes = {}
 
     prefix = key_datatype.prefix_code + value_datatype.prefix_code
 
     classes['TreeItems'] = classes['TreeItemsPy'] = TreeItems
     for base in (
@@ -79,20 +79,20 @@
         if 'Set' in cls.__name__:
             cls._bucket_type = classes['SetPy']
         else:
             cls._bucket_type = classes['BucketPy']
 
     return classes
 
-def _create_set_operations(module_name, key_type, value_type, set_type):
-    from ._base import set_operation
 
+def _create_set_operations(module_name, key_type, value_type, set_type):
     from ._base import difference
     from ._base import intersection
     from ._base import multiunion
+    from ._base import set_operation
     from ._base import union
     from ._base import weightedIntersection
     from ._base import weightedUnion
 
     ops = {
         op.__name__ + 'Py': set_operation(op, set_type)
         for op in (
@@ -112,38 +112,44 @@
     for key, op in ops.items():
         op.__module__ = module_name
         op.__name__ = key
 
     # TODO: Pickling. These things should be looked up by name.
     return ops
 
+
 def _create_globals(module_name, key_datatype, value_datatype):
     classes = _create_classes(module_name, key_datatype, value_datatype)
     set_type = classes['SetPy']
-    set_ops = _create_set_operations(module_name, key_datatype, value_datatype, set_type)
+    set_ops = _create_set_operations(
+        module_name, key_datatype, value_datatype, set_type,
+    )
 
     classes.update(set_ops)
     return classes
 
 
 def populate_module(mod_globals,
                     key_datatype, value_datatype,
                     interface, module=None):
-    from . import Interfaces as interfaces
-    from ._compat import import_c_extension
     import collections.abc
+
+    from . import Interfaces as interfaces
     from ._base import _fix_pickle
+    from ._compat import import_c_extension
 
     module_name = mod_globals['__name__']
     # Define the Python implementations
-    mod_globals.update(_create_globals(module_name, key_datatype, value_datatype))
+    mod_globals.update(
+        _create_globals(module_name, key_datatype, value_datatype)
+    )
     # Import the C versions, if possible. Whether or not this is possible,
-    # this currently makes the non-`Py' suffixed names available. This should change
-    # if we start defining the Python classes with their natural name, only aliased
-    # to the 'Py` suffix (which simplifies pickling)
+    # this currently makes the non-`Py' suffixed names available. This should
+    # change if we start defining the Python classes with their natural name,
+    # only aliased to the 'Py` suffix (which simplifies pickling)
     import_c_extension(mod_globals)
 
     # Next, define __all__ after all the name aliasing is done.
     # XXX: Maybe derive this from the values we create.
     mod_all = (
         'Bucket', 'Set', 'BTree', 'TreeSet',
         'union', 'intersection', 'difference',
@@ -151,15 +157,17 @@
     )
     prefix = key_datatype.prefix_code + value_datatype.prefix_code
 
     mod_all += tuple(prefix + c for c in ('Bucket', 'Set', 'BTree', 'TreeSet'))
 
     mod_globals['__all__'] = tuple(c for c in mod_all if c in mod_globals)
 
-    mod_globals['using64bits'] = key_datatype.using64bits or value_datatype.using64bits
+    mod_globals['using64bits'] = (
+        key_datatype.using64bits or value_datatype.using64bits
+    )
 
     # XXX: We can probably do better than fix_pickle now;
     # we can know if we're going to be renaming classes
     # ahead of time. See above.
     _fix_pickle(mod_globals, module_name)
 
     # Apply interface definitions.
@@ -177,39 +185,41 @@
     for cls_name, abc in {
             'BTree': collections.abc.MutableMapping,
             'Bucket': collections.abc.MutableMapping,
             'Set': collections.abc.MutableSet,
             'TreeSet': collections.abc.MutableSet,
     }.items():
         abc.register(mod_globals[cls_name])
-        # Because of some quirks in the implementation of ABCMeta.__instancecheck__,
-        # and the shenanigans we currently do to make Python classes pickle without the
-        # 'Py' suffix, it's not actually necessary to register the Python version of the
-        # class. Specifically, ABCMeta asks for the object's ``__class__`` instead of
-        # using ``type()``, and our objects have a ``@property`` for ``__class__`` that returns
-        # the C version.
+        # Because of some quirks in the implementation of
+        # ABCMeta.__instancecheck__, and the shenanigans we currently do to
+        # make Python classes pickle without the 'Py' suffix, it's not actually
+        # necessary to register the Python version of the class. Specifically,
+        # ABCMeta asks for the object's ``__class__`` instead of using
+        # ``type()``, and our objects have a ``@property`` for ``__class__``
+        # that returns the C version.
         #
         # That's too many coincidences to rely on though.
         abc.register(mod_globals[cls_name + 'Py'])
 
     # Set node sizes.
-    for cls_name in (
-            'BTree',
-            'TreeSet',
-    ):
+    for cls_name in ('BTree', 'TreeSet'):
+
         for suffix in ('', 'Py'):
             cls = mod_globals[cls_name + suffix]
-            cls.max_leaf_size = key_datatype.bucket_size_for_value(value_datatype)
+            cls.max_leaf_size = key_datatype.bucket_size_for_value(
+                value_datatype
+            )
             cls.max_internal_size = key_datatype.tree_size
 
 
 def create_module(prefix):
     import types
-    from . import _datatypes as datatypes
+
     from . import Interfaces
+    from . import _datatypes as datatypes
 
     mod = types.ModuleType('BTrees.' + prefix + 'BTree')
 
     key_type = getattr(datatypes, prefix[0])()
     val_type = getattr(datatypes, prefix[1])().as_value_type()
 
     iface_name = 'I' + key_type.long_name + val_type.long_name + 'BTreeModule'
```

### Comparing `BTrees-5.2/src/BTrees/check.py` & `BTrees-6.0/src/BTrees/check.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,22 @@
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE
 #
 ##############################################################################
+# isort: skip_file
 """
 Utilities for working with BTrees (TreeSets, Buckets, and Sets) at a low
 level.
 
 The primary function is check(btree), which performs value-based consistency
-checks of a kind ``BTree._Tree._check()`` does not perform.  See the function docstring
-for details.
+checks of a kind ``BTree._Tree._check()`` does not perform.  See the function
+docstring for details.
 
 display(btree) displays the internal structure of a BTree (TreeSet, etc) to
 stdout.
 
 CAUTION:  When a BTree node has only a single bucket child, it can be
 impossible to get at the bucket from Python code (__getstate__() may squash
 the bucket object out of existence, as a pickling storage optimization).  In
@@ -85,19 +86,18 @@
 from BTrees.OQBTree import OQBTreePy, OQBucketPy, OQSetPy, OQTreeSetPy
 
 from BTrees.fsBTree import fsBTree, fsBucket, fsSet, fsTreeSet
 from BTrees.fsBTree import fsBTreePy, fsBucketPy, fsSetPy, fsTreeSetPy
 
 from BTrees.utils import positive_id
 from BTrees.utils import oid_repr
+from BTrees._compat import compare
 
 TYPE_UNKNOWN, TYPE_BTREE, TYPE_BUCKET = range(3)
 
-from ._compat import compare
-
 _type2kind = {}
 _FAMILIES = (
     'OO', 'OI', 'OU', 'OL', 'OQ',
     'II', 'IO', 'IF', 'IU',
     'LL', 'LO', 'LF', 'LQ',
     'UU', 'UO', 'UF', 'UI',
     'QQ', 'QO', 'QF', 'QL',
@@ -110,24 +110,27 @@
             ('TreeSet', (TYPE_BTREE, False)),
             ('Set', (TYPE_BUCKET, False)),
     ):
         _type2kind[globals()[kv + name]] = kind
         py = kv + name + 'Py'
         _type2kind[globals()[py]] = kind
 
+
 # Return pair
 #
 #     TYPE_BTREE or TYPE_BUCKET, is_mapping
 
+
 def classify(obj):
     return _type2kind[type(obj)]
 
 
 BTREE_EMPTY, BTREE_ONE, BTREE_NORMAL = range(3)
 
+
 # If the BTree is empty, returns
 #
 #     BTREE_EMPTY, [], []
 #
 # If the BTree has only one bucket, sometimes returns
 #
 #     BTREE_ONE, bucket_state, None
@@ -223,14 +226,15 @@
 #
 #     (
 #          (keys[0], values[0], keys[1], values[1], ...,
 #                               keys[len-1], values[len-1]),
 #          <self->next iff non-NULL>
 #     )
 
+
 def crack_bucket(b, is_mapping):
     state = b.__getstate__()
     assert isinstance(state, tuple)
     assert 1 <= len(state) <= 2
     data = state[0]
     if not is_mapping:
         return data, []
@@ -243,28 +247,32 @@
         if i & 1:
             values.append(x)
         else:
             keys.append(x)
         i += 1
     return keys, values
 
+
 def type_and_adr(obj):
     if hasattr(obj, '_p_oid'):
         oid = oid_repr(obj._p_oid)
     else:
         oid = 'None'
-    return "{} (0x{:x} oid={})".format(type(obj).__name__, positive_id(obj), oid)
+    return "{} (0x{:x} oid={})".format(
+        type(obj).__name__, positive_id(obj), oid
+    )
 
-# Walker implements a depth-first search of a BTree (or TreeSet or Set or
-# Bucket).  Subclasses must implement the visit_btree() and visit_bucket()
-# methods, and arrange to call the walk() method.  walk() calls the
-# visit_XYZ() methods once for each node in the tree, in depth-first
-# left-to-right order.
 
 class Walker:
+    # Walker implements a depth-first search of a BTree (or TreeSet or Set or
+    # Bucket).  Subclasses must implement the visit_btree() and visit_bucket()
+    # methods, and arrange to call the walk() method.  walk() calls the
+    # visit_XYZ() methods once for each node in the tree, in depth-first
+    # left-to-right order.
+
     def __init__(self, obj):
         self.obj = obj
 
     # obj is the BTree (BTree or TreeSet).
     # path is a list of indices, from the root.  For example, if a BTree node
     # is child[5] of child[3] of the root BTree, [3, 5].
     # parent is the parent BTree object, or None if this is the root BTree.
@@ -325,16 +333,15 @@
                 elif bkind is BTREE_EMPTY:
                     pass
                 else:
                     assert bkind is BTREE_ONE
                     # Yuck.  There isn't a bucket object to pass on, as
                     # the bucket state is embedded directly in the BTree
                     # state.  Synthesize a bucket.
-                    assert kids is None   # and "keys" is really the bucket
-                                          # state
+                    assert kids is None  # "keys" is really the bucket state
                     bucket = _btree2bucket[type(obj)]()
                     bucket.__setstate__(keys)
                     stack.append((bucket,
                                   path + [0],
                                   obj,
                                   lo,
                                   hi))
@@ -403,15 +410,16 @@
     def complain(self, msg, obj, path):
         s = "{}, in {}, path from root {}".format(
                 msg,
                 type_and_adr(obj),
                 ".".join(map(str, path)))
         self.errors.append(s)
 
-class Printer(Walker): # pragma: no cover
+
+class Printer(Walker):  # pragma: no cover
     def __init__(self, obj):
         Walker.__init__(self, obj)
 
     def display(self):
         self.walk()
 
     def visit_btree(self, obj, path, parent, is_mapping,
@@ -438,29 +446,31 @@
         indent += "    "
         n = len(keys)
         for i in range(n):
             print("%skey %d: %r" % (indent, i, keys[i]),)
             if is_mapping:
                 print("value {!r}".format(values[i]))
 
+
 def check(btree):
     """Check internal value-based invariants in a BTree or TreeSet.
 
-    The ``BTrees._base._Tree._check`` method checks internal C-level pointer consistency.
-    The :func:`~BTrees.check.check` function here checks value-based invariants:  whether the
-    keys in leaf bucket and internal nodes are in strictly increasing order,
-    and whether they all lie in their expected range.  The latter is a subtle
-    invariant that can't be checked locally -- it requires propagating
-    range info down from the root of the tree, and modifying it at each
-    level for each child.
+    The ``BTrees._base._Tree._check`` method checks internal C-level pointer
+    consistency.  The :func:`~BTrees.check.check` function here checks
+    value-based invariants:  whether the keys in leaf bucket and internal nodes
+    are in strictly increasing order, and whether they all lie in their
+    expected range.  The latter is a subtle invariant that can't be checked
+    locally -- it requires propagating range info down from the root of the
+    tree, and modifying it at each level for each child.
 
     Raises :class:`AssertionError` if anything is wrong, with a string detail
     explaining the problems.  The entire tree is checked before
-    :class:`AssertionError` is raised, and the string detail may be large (depending
-    on how much went wrong).
+    :class:`AssertionError` is raised, and the string detail may be large
+    (depending on how much went wrong).
     """
 
     Checker(btree).check()
 
-def display(btree): # pragma: no cover
+
+def display(btree):  # pragma: no cover
     "Display the internal structure of a BTree, Bucket, TreeSet or Set."
     Printer(btree).display()
```

### Comparing `BTrees-5.2/src/BTrees/floatvaluemacros.h` & `BTrees-6.0/src/BTrees/floatvaluemacros.h`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/src/BTrees/intkeymacros.h` & `BTrees-6.0/src/BTrees/intkeymacros.h`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/src/BTrees/intvaluemacros.h` & `BTrees-6.0/src/BTrees/intvaluemacros.h`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/src/BTrees/objectkeymacros.h` & `BTrees-6.0/src/BTrees/objectkeymacros.h`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/src/BTrees/sorters.c` & `BTrees-6.0/src/BTrees/sorters.c`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/src/BTrees/tests/_test_builder.py` & `BTrees-6.0/src/BTrees/tests/_test_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,20 +21,20 @@
 from .common import MappingBase
 from .common import MappingConflictTestBase
 from .common import ModuleTest
 from .common import MultiUnion
 from .common import NormalSetTests
 from .common import SetConflictTestBase
 from .common import SetResult
+from .common import TestLongIntKeys
+from .common import TestLongIntValues
 from .common import Weighted
 from .common import itemsToSet
 from .common import makeMapBuilder
 from .common import makeSetBuilder
-from .common import TestLongIntKeys
-from .common import TestLongIntValues
 
 
 class _FilteredModuleProxy:
     """
     Accesses either ``<name>`` or ``<name>Py`` from a module.
 
     This conveniently lets us avoid lots of 'getattr' calls.
@@ -65,28 +65,31 @@
             for x in tuple_or_klass:
                 yield from f(x)
         else:
             yield tuple_or_klass
 
     return tuple(f(args))
 
+
 class ClassBuilder:
 
     # Use TestAuto as a prefix to avoid clashing with manual tests
     TESTCASE_PREFIX = 'TestAuto'
 
     def __init__(self, btree_module, btree_tests_base=BTreeTests):
         self.btree_module = btree_module
         # These will be instances of _datatypes.DataType
         self.key_type = btree_module.BTreePy._to_key
         self.value_type = btree_module.BTreePy._to_value
 
         class _BoundsMixin:
-            # For test purposes, we can only support negative keys if they are ordered like
-            # integers. Our int -> 2 byte conversion for fsBTree doesn't do this.
+            # For test purposes, we can only support negative keys if they are
+            # ordered like integers. Our int -> 2 byte conversion for fsBTree
+            # doesn't do this.
+            #
             # -1 is \xff\xff which is the largest possible key.
             SUPPORTS_NEGATIVE_KEYS = (
                 self.key_type.get_lower_bound() != 0
                 and self.key_type.coerce(-1) < self.key_type.coerce(0)
             )
             SUPPORTS_NEGATIVE_VALUES = self.value_type.get_lower_bound() != 0
             if SUPPORTS_NEGATIVE_KEYS:
@@ -97,27 +100,26 @@
             coerce_to_key = self.key_type.coerce
             coerce_to_value = self.value_type.coerce
             KEYS = tuple(self.key_type.coerce(x) for x in range(2001))
             VALUES = tuple(self.value_type.coerce(x) for x in range(2001))
 
         self.bounds_mixin = _BoundsMixin
 
-
         self.btree_tests_base = btree_tests_base
 
         self.prefix = btree_module.__name__.split('.', )[-1][:2]
         self.test_module = 'BTrees.tests.test_' + self.prefix + 'BTree'
 
         self.test_classes = {}
         # Keep track of tested classes so that we don't
         # double test in PURE_PYTHON mode (e.g., BTreePy is BTree)
         self.tested_classes = set()
 
     def _store_class(self, test_cls):
-        assert test_cls.__name__ not in self.test_classes, (test_cls, self.test_classes)
+        assert test_cls.__name__ not in self.test_classes
         assert isinstance(test_cls, type)
         assert issubclass(test_cls, unittest.TestCase)
         self.test_classes[test_cls.__name__] = test_cls
 
     def _fixup_and_store_class(self, btree_module, fut, test_cls):
         base = [x for x in test_cls.__bases__
                 if x.__module__ != __name__ and x.__module__ != 'unittest'][0]
@@ -172,15 +174,14 @@
             intersection = btree_module.def_intersection
             # These are specific to Weighted; modules that
             # don't have weighted values can'd do them.
             if base is Weighted:
                 weightedUnion = btree_module.def_weightedUnion
                 weightedIntersection = btree_module.def_weightedIntersection
 
-
             # These are specific to MultiUnion, and may not exist
             # in key types that don't support unions (``'O'``)
             multiunion = getattr(btree_module, 'multiunion', None)
             mkset = btree_module.Set
             mktreeset = btree_module.TreeSet
             mkbtree = tree
 
@@ -214,25 +215,34 @@
                 )
 
         self._fixup_and_store_class(btree_module, '', Test)
 
     def _create_module_test(self):
         from BTrees import Interfaces as interfaces
         mod = self.btree_module
-        iface = getattr(interfaces, 'I' + self.key_type.long_name + self.value_type.long_name
-                        + 'BTreeModule')
+        iface_name = (
+            f'I{self.key_type.long_name}{self.value_type.long_name}'
+            f'BTreeModule'
+        )
+        iface = getattr(interfaces, iface_name)
+
         class Test(ModuleTest, unittest.TestCase):
             prefix = self.prefix
             key_type = self.key_type
             value_type = self.value_type
 
-            _getModule = lambda self: mod
-            _getInterface = lambda self: iface
+            def _getModule(self):
+                return mod
 
-        self._fixup_and_store_class(_FilteredModuleProxy(self.btree_module, ''), '', Test)
+            def _getInterface(self):
+                return iface
+
+        self._fixup_and_store_class(
+            _FilteredModuleProxy(self.btree_module, ''), '', Test
+        )
 
     def _create_type_tests(self, btree_module, type_name, test_bases):
         from BTrees import Interfaces as interfaces
         tree = getattr(btree_module, type_name)
         iface = {
             'BTree': interfaces.IBTree,
             'Bucket': interfaces.IMinimalDictionary,
@@ -286,15 +296,14 @@
                              SetConflictTestBase,)),
                     ('TreeSet', (I_SetsBase,
                                  NormalSetTests,
                                  SetConflictTestBase,))
             ):
                 self._create_type_tests(btree_module, type_name, test_bases)
 
-
             for test_base in set_ops:
                 self._create_set_op_test(btree_module, test_base)
 
             self._create_set_result_test(btree_module)
 
 
 def update_module(test_module_globals, btree_module, *args, **kwargs):
```

### Comparing `BTrees-5.2/src/BTrees/tests/common.py` & `BTrees-6.0/src/BTrees/tests/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,27 +8,29 @@
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE
 #
 ##############################################################################
 
-import sys
 import functools
-import unittest
 import platform
+import sys
+import unittest
 from unittest import skip
 
-from BTrees._compat import _c_optimizations_ignored
+from BTrees._base import _tp_name
 from BTrees._compat import PYPY
-from BTrees._base   import _tp_name
+from BTrees._compat import _c_optimizations_ignored
+
 
 def _no_op(test_method):
     return test_method
 
+
 try:
     __import__('ZODB')
 except ImportError:
     _skip_wo_ZODB = skip('ZODB not available')
 else:
     _skip_wo_ZODB = _no_op
 
@@ -38,31 +40,29 @@
     _skip_on_32_bits = _no_op
 
 if _c_optimizations_ignored():
     skipOnPurePython = skip("Not on Pure Python")
 else:
     skipOnPurePython = _no_op
 
+
 def _skip_if_pure_py_and_py_test(self):
     if _c_optimizations_ignored() and 'Py' in type(self).__name__:
         # No need to run this again. The "C" tests will catch it.
         # This relies on the fact that we always define tests in pairs,
         # one normal/C and one with Py in the name for the Py test.
         raise unittest.SkipTest("Redundant with the C test")
 
-# pylint:disable=too-many-lines
-# pylint:disable=no-member,protected-access,unused-variable,import-error
-# pylint:disable=line-too-long,unidiomatic-typecheck,abstract-method
-# pylint:disable=redefined-builtin
 
 #: The exceptions that can be raised by failed
 #: unsigned conversions. The OverflowError is raised
 #: by the interpreter and is nicer than the manual error.
 UnsignedError = (TypeError, OverflowError)
 
+
 def uses_negative_keys_and_values(func):
     """
     Apply this decorator to tests that use negative keys and values.
 
     If the underlying mapping doesn't support that, it will
     be expected to raise a TypeError or OverflowError.
     """
@@ -71,14 +71,15 @@
         if not (self.SUPPORTS_NEGATIVE_KEYS and self.SUPPORTS_NEGATIVE_VALUES):
             with self.assertRaises(UnsignedError):
                 func(self)
         else:
             func(self)
     return test
 
+
 class SignedMixin:
     SUPPORTS_NEGATIVE_KEYS = True
     SUPPORTS_NEGATIVE_VALUES = True
     #: The values to pass to ``random.randrange()`` to generate
     #: valid keys.
     KEY_RANDRANGE_ARGS = (-2000, 2001)
 
@@ -103,29 +104,32 @@
             # testGhostUnghost() both nail the CPU and seemingly
             # never finish.
             self.db = DB(MappingStorage())
         return self.db.open().root()
 
     def _closeRoot(self, root):
         import transaction
+
         # If we don't commit/abort the transaction, then
         # closing the Connection tends to fail with
         # "Cannot close connection joined to transaction"
         transaction.abort()
         root._p_jar.close()
 
 
 class Base(ZODBAccess, SignedMixin):
     # Tests common to all types: sets, buckets, and BTrees
 
     def _getTargetClass(self):
         raise NotImplementedError("subclass should return the target type")
 
     def _getTargetInterface(self):
-        raise NotImplementedError("subclass must return the expected interface ")
+        raise NotImplementedError(
+            "subclass must return the expected interface "
+        )
 
     def _makeOne(self):
         return self._getTargetClass()()
 
     def setUp(self):
         super().setUp()
         _skip_if_pure_py_and_py_test(self)
@@ -188,33 +192,38 @@
         # Now make sure that it actually has the required methods.
         # First, get the required methods:
         abc_attrs = set(dir(abc))
         # If the method was None, that means it's not required;
         # if it's not callable, it's not a method (None is not callable)
         # If it's a private attribute (starting with only one _), it's
         # an implementation detail to ignore.
-        abc_attrs -= {x for x in abc_attrs
-                         if (x[0] == '_' and x[1] != '_')
-                         or not callable(getattr(abc, x, None))}
+        abc_attrs -= {
+            x for x in abc_attrs if
+            (x[0] == '_' and x[1] != '_') or
+            not callable(getattr(abc, x, None))
+        }
         # Drop things from Python typing and zope.interface that may or may not
         # be present.
         abc_attrs -= {
             '__provides__',
             '__implemented__',
             '__providedBy__',
-            '__class_getitem__', # Python 3.9+
+            '__class_getitem__',  # Python 3.9+
             # Also the equality and comparison operators;
             # we don't implement those methods, but the ABC does.
             '__lt__', '__le__', '__eq__', '__gt__', '__ge__', '__ne__',
         }
         btr_attrs = set(dir(type(t)))
 
         missing_attrs = abc_attrs - btr_attrs
-        self.assertFalse(sorted(missing_attrs),
-                         "Class {!r} is missing these methods: {}".format(type(t), missing_attrs))
+        self.assertFalse(
+            sorted(missing_attrs),
+            "Class {!r} is missing these methods: {}".format(
+                type(t), missing_attrs)
+        )
 
     def testPersistentSubclass(self):
         # Can we subclass this and Persistent?
         # https://github.com/zopefoundation/BTrees/issues/78
         import persistent
 
         class PersistentSubclass(persistent.Persistent):
@@ -315,28 +324,36 @@
         self.assertEqual(list(t.keys(excludemin=True, excludemax=True)), [])
 
         t.clear()
         self._populate(t, 3)
         self.assertEqual(list(t.keys()), [K[0], K[1], K[2]])
         self.assertEqual(list(t.keys(excludemin=True)), [K[1], K[2]])
         self.assertEqual(list(t.keys(excludemax=True)), [K[0], K[1]])
-        self.assertEqual(list(t.keys(excludemin=True, excludemax=True)), [K[1]])
+        self.assertEqual(
+            list(t.keys(excludemin=True, excludemax=True)), [K[1]]
+        )
 
         for low, high, expected in ((-1, 3, [0, 1, 2]), (-1, 2, [0, 1])):
             if self.SUPPORTS_NEGATIVE_KEYS:
-                self.assertEqual(list(t.keys(low, high, excludemin=True, excludemax=True)),
-                                 expected)
+                self.assertEqual(
+                    list(t.keys(low, high, excludemin=True, excludemax=True)),
+                    expected
+                )
             else:
                 with self.assertRaises(UnsignedError):
                     t.keys(low, high, excludemin=True, excludemax=True)
 
-        self.assertEqual(list(t.keys(K[0], K[3], excludemin=True, excludemax=True)),
-                         [K[1], K[2]])
-        self.assertEqual(list(t.keys(K[0], K[2], excludemin=True, excludemax=True)),
-                         [K[1]])
+        self.assertEqual(
+            list(t.keys(K[0], K[3], excludemin=True, excludemax=True)),
+            [K[1], K[2]]
+        )
+        self.assertEqual(
+            list(t.keys(K[0], K[2], excludemin=True, excludemax=True)),
+            [K[1]]
+        )
 
     @_skip_wo_ZODB
     def test_UpdatesDoReadChecksOnInternalNodes(self):
         import transaction
         from ZODB import DB
         from ZODB.MappingStorage import MappingStorage
         t = self._makeOne()
@@ -347,32 +364,38 @@
         store = MappingStorage()
         db = DB(store)
         conn = db.open()
         conn.root.t = t
         transaction.commit()
 
         read = []
+
         def readCurrent(ob):
             read.append(ob)
             conn.__class__.readCurrent(conn, ob)
             return 1
 
         conn.readCurrent = readCurrent
 
         try:
             _add = t.add
             _remove = t.remove
         except AttributeError:
+
             def add(i):
                 t[self.coerce_to_key(i)] = self.coerce_to_value(i)
+
             def remove(i):
                 del t[self.coerce_to_key(i)]
+
         else:
+
             def add(i):
                 _add(self.coerce_to_key(i))
+
             def remove(i):
                 _remove(self.coerce_to_key(i))
 
         # Modifying a thing
         remove(100)
         self.assertTrue(t in read)
         del read[:]
@@ -400,19 +423,21 @@
 
             loaded_one = pickle.loads(dumped_str)
 
             # If we're testing the pure-Python version, but we have the
             # C extension available, then the loaded type will be the C
             # extension but the made type will be the Python version.
             # Otherwise, they match. (Note that if we don't have C extensions
-            # available, the __name__ will be altered to not have Py in it. See _fix_pickle)
+            # available, the __name__ will be altered to not have Py in it.
+            # See _fix_pickle)
             if 'Py' in type(made_one).__name__:
                 self.assertTrue(type(loaded_one) is not type(made_one))
             else:
-                self.assertTrue(type(loaded_one) is type(made_one) is self._getTargetClass(), (type(loaded_one), type(made_one), self._getTargetClass(), repr(dumped_str)))
+                self.assertTrue(type(loaded_one) is type(made_one))
+                self.assertTrue(type(loaded_one) is self._getTargetClass())
 
             dumped_str2 = pickle.dumps(loaded_one, proto)
             self.assertEqual(dumped_str, dumped_str2)
 
     def test_pickle_empty(self):
         # Issue #2
         # Pickling an empty object and unpickling it should result
@@ -468,30 +493,30 @@
         self.assertTrue(issubclass(Sub, type(t)))
 
         if type(t) is not t.__class__:
             # We're fibbing; this breaks issubclass of itself,
             # contrary to the usual mechanism
             self.assertFalse(issubclass(t.__class__, type(t)))
 
-
         class NonSub:
             pass
 
         self.assertFalse(issubclass(NonSub, type(t)))
         self.assertFalse(isinstance(NonSub(), type(t)))
 
-class MappingBase(Base): # pylint:disable=too-many-public-methods
+
+class MappingBase(Base):
     # Tests common to mappings (buckets, btrees)
     SUPPORTS_NEGATIVE_VALUES = True
 
-    def _populate(self, t, l):
+    def _populate(self, t, largest):
         # Make some data
         to_key = self.coerce_to_key
         to_value = self.coerce_to_value
-        for i in range(l):
+        for i in range(largest):
             t[to_key(i)] = to_value(i)
 
     def _getCollectionsABC(self):
         import collections.abc
         return collections.abc.MutableMapping
 
     def test_popitem(self):
@@ -631,15 +656,14 @@
         self.assertFalse(t.has_key(too_big))
         self.assertFalse(t.has_key(too_small))
         self.assertFalse(t.has_key('abc'))
 
     def testValuesWorks(self):
         t = self._makeOne()
         K = self.KEYS
-        V = self.VALUES
         for x in range(100):
             t[K[x]] = self.coerce_to_value(x * x)
         values = t.values()
         for i in range(100):
             v = self.coerce_to_value(i * i)
             self.assertEqual(values[i], v)
         self.assertRaises(IndexError, lambda: values[i + 1])
@@ -686,17 +710,18 @@
         for x in v:
             self.assertEqual(x, K[i])
             i = i + 1
         self.assertRaises(IndexError, lambda: v[i])
 
         for x in range(40):
             lst = t.keys(K[0 + x], K[99 - x])
-            self.assertEqual(list(lst), [K[x] for x in range(0 + x, 99 - x + 1)])
-
-
+            self.assertEqual(
+                list(lst),
+                [K[x] for x in range(0 + x, 99 - x + 1)]
+            )
             lst = t.keys(max=K[99-x], min=K[0+x])
             self.assertEqual(list(lst), [K[x] for x in range(0+x, 99-x+1)])
 
         self.assertEqual(len(v), 100)
 
     @uses_negative_keys_and_values
     def testKeysNegativeIndex(self):
@@ -781,15 +806,15 @@
         self.assertEqual(t.maxKey(K[9]), K[8])
         self.assertEqual(t.minKey(), K[1])
         self.assertEqual(t.minKey(None), K[1])
         self.assertEqual(t.minKey(K[3]), K[3])
         self.assertEqual(t.minKey(K[9]), K[10])
 
         try:
-            too_small = t.minKey() - 1
+            t.minKey() - 1
         except TypeError:
             # we can't do arithmetic with the key type;
             # must be fsBTree.
             return
 
         try:
             t.maxKey(t.minKey() - 1)
@@ -816,31 +841,31 @@
         diff = lsubtract(list(t.keys()), [])
         self.assertEqual(diff, [])
 
     def testUpdate(self):
         import random
         t = self._makeOne()
         d = {}
-        l = []
+        items = []
         for i in range(10000):
             k = random.randrange(*self.KEY_RANDRANGE_ARGS)
             k = self.coerce_to_key(k)
             v = self.coerce_to_value(i)
             d[k] = v
-            l.append((k, v))
+            items.append((k, v))
 
         items = sorted(d.items())
 
         t.update(d)
         self.assertEqual(list(t.items()), items)
 
         t.clear()
         self.assertEqual(list(t.items()), [])
 
-        t.update(l)
+        t.update(items)
         self.assertEqual(list(t.items()), items)
 
     # Before ZODB 3.4.2, update/construction from PersistentMapping failed.
     def testUpdateFromPersistentMapping(self):
         from persistent.mapping import PersistentMapping
         t = self._makeOne()
         K = self.KEYS
@@ -855,15 +880,18 @@
 
     def testEmptyRangeSearches(self):
         t = self._makeOne()
         K = self.KEYS
         V = self.VALUES
         t.update([(K[1], V[1]), (K[5], V[5]), (K[9], V[9])])
         if self.SUPPORTS_NEGATIVE_KEYS and self.SUPPORTS_NEGATIVE_VALUES:
-            self.assertEqual(list(t.keys(self.coerce_to_key(-6), self.coerce_to_key(-4))), [])
+            self.assertEqual(
+                list(t.keys(self.coerce_to_key(-6), self.coerce_to_key(-4))),
+                []
+            )
 
         self.assertEqual(list(t.keys(K[2], K[4])), [])
         self.assertEqual(list(t.keys(K[6], K[8])), [])
         self.assertEqual(list(t.keys(K[10], K[12])), [])
         self.assertEqual(list(t.keys(K[9], K[1])), [])
 
         # For IITreeSets, this one was returning 31 for len(keys), and
@@ -880,15 +908,15 @@
         self.assertEqual(list(t.iterkeys(two_hundred, fifty)), [])
 
         keys = t.keys(max=fifty, min=two_hundred)
         self.assertEqual(len(keys), 0)
         self.assertEqual(list(keys), [])
         self.assertEqual(list(t.iterkeys(max=fifty, min=two_hundred)), [])
 
-    def testSlicing(self): # pylint:disable=too-many-locals
+    def testSlicing(self):
         # Test that slicing of .keys()/.values()/.items() works exactly the
         # same way as slicing a Python list with the same contents.
         # This tests fixes to several bugs in this area, starting with
         # http://collector.zope.org/Zope/419,
         # "BTreeItems slice contains 1 too many elements".
         t = self._makeOne()
         val_multiplier = -2 if self.SUPPORTS_NEGATIVE_VALUES else 2
@@ -996,15 +1024,15 @@
             self.assertEqual(x, keys)
 
             self.assertEqual(list(t.iterkeys()), keys)
             self.assertEqual(list(t.itervalues()), list(t.values()))
             self.assertEqual(list(t.iteritems()), list(t.items()))
 
     @uses_negative_keys_and_values
-    def testRangedIterators(self): # pylint:disable=too-many-locals
+    def testRangedIterators(self):
         t = self._makeOne()
 
         for keys in [], [-2], [1, 4], list(range(-170, 2000, 13)):
             t.clear()
             values = []
             for k in keys:
                 value = -3 * k
@@ -1065,16 +1093,18 @@
 
     def testSimpleExclusivRanges(self):
         K = self.KEYS
         V = self.VALUES
 
         def list_keys(x):
             return [K[k] for k in x]
+
         def list_values(x):
             return [V[k] for k in x]
+
         def as_items(x):
             return [(K[k], V[k]) for k in x]
 
         for methodname, f in (("keys", list_keys),
                               ("values", list_values),
                               ("items", as_items),
                               ("iterkeys", list_keys),
@@ -1112,28 +1142,39 @@
             self._populate(t, 3)
             self.assertEqual(list(meth()), f([0, 1, 2]))
             self.assertEqual(list(meth(excludemin=True)), f([1, 2]))
             self.assertEqual(list(meth(excludemax=True)), f([0, 1]))
             self.assertEqual(list(meth(excludemin=True, excludemax=True)),
                              f([1]))
             if supports_negative:
-                self.assertEqual(list(meth(self.coerce_to_key(-1), K[2], excludemin=True,
-                                           excludemax=True)),
-                                 f([0, 1]))
-
-                self.assertEqual(list(meth(self.coerce_to_key(-1), K[3], excludemin=True,
-                                           excludemax=True)),
-                                 f([0, 1, 2]))
-
-            self.assertEqual(list(meth(K[0], K[3], excludemin=True,
-                                       excludemax=True)),
-                             f([1, 2]))
-            self.assertEqual(list(meth(K[0], K[2], excludemin=True,
-                                       excludemax=True)),
-                             f([1]))
+                self.assertEqual(
+                    list(meth(
+                        self.coerce_to_key(-1),
+                        K[2],
+                        excludemin=True,
+                        excludemax=True,
+                    )), f([0, 1])
+                )
+
+                self.assertEqual(
+                    list(meth(
+                        self.coerce_to_key(-1),
+                        K[3], excludemin=True,
+                        excludemax=True
+                    )), f([0, 1, 2])
+                )
+
+            self.assertEqual(
+                list(meth(K[0], K[3], excludemin=True, excludemax=True)),
+                f([1, 2])
+            )
+            self.assertEqual(
+                list(meth(K[0], K[2], excludemin=True, excludemax=True)),
+                f([1])
+            )
 
     def testSetdefault(self):
         t = self._makeOne()
         K = self.KEYS
         V = self.VALUES
         self.assertEqual(t.setdefault(K[1], V[2]), V[2])
         # That should also have associated 1 with 2 in the tree.
@@ -1145,15 +1186,14 @@
 
         # Not enough arguments.
         self.assertRaises(TypeError, t.setdefault)
         self.assertRaises(TypeError, t.setdefault, K[1])
         # Too many arguments.
         self.assertRaises(TypeError, t.setdefault, K[1], V[2], V[3])
 
-
     def testPop(self):
         t = self._makeOne()
         K = self.KEYS
         V = self.VALUES
         # Empty container.
         # If no default given, raises KeyError.
         self.assertRaises(KeyError, t.pop, K[1])
@@ -1186,15 +1226,15 @@
         self.assertRaises(TypeError, t.pop)
         # Too many arguments.
         self.assertRaises(TypeError, t.pop, K[1], 2, 3)
 
     def __test_key_or_value_type(self, k, v, to_test, kvtype):
         try:
             kvtype(to_test)
-        except Exception as e: # pylint:disable=broad-except
+        except Exception as e:
             with self.assertRaises(type(e)):
                 self._makeOne()[k] = self.coerce_to_value(v)
         else:
             self._makeOne()[k] = self.coerce_to_value(v)
 
     def __test_key(self, k):
         v = self.getTwoValues()[0]
@@ -1232,22 +1272,24 @@
         self.__test_value(2.5)
 
     def test_assign_value_type_None(self):
         self.__test_value(None)
 
     def testNewStyleClassAsKeyNotAllowed(self):
         m = self._makeOne()
+
         class New:
             pass
 
         with self.assertRaises(TypeError):
             m[New] = self.getTwoValues()[0]
 
     def testClassAsKeyNotAllowed(self):
         m = self._makeOne()
+
         class Cls:
             pass
 
         with self.assertRaises(TypeError):
             m[Cls] = self.getTwoValues()[0]
 
     def testNewStyleClassWithCustomMetaClassNotAllowed(self):
@@ -1259,49 +1301,53 @@
         m = self._makeOne()
         with self.assertRaises(TypeError):
             m[cls] = self.getTwoValues()[0]
 
     def testEmptyFirstBucketReportedByGuido(self):
         # This was for Integer keys
         b = self._makeOne()
-        for i in range(29972): # reduce to 29971 and it works
+        for i in range(29972):  # reduce to 29971 and it works
             b[self.coerce_to_key(i)] = self.coerce_to_value(i)
-        for i in range(30): # reduce to 29 and it works
+        for i in range(30):  # reduce to 29 and it works
             del b[self.coerce_to_key(i)]
             try:
                 big_key = self.coerce_to_key(i + 40000)
             except TypeError:
                 # fsBtree only has a two-byte key
                 self.skipTest('Key to big')
             b[big_key] = self.coerce_to_value(i)
 
         self.assertEqual(b.keys()[0], self.KEYS[30])
 
     def testKeyAndValueOverflow(self):
-        if self.key_type.get_upper_bound() is None or self.value_type.get_upper_bound() is None:
+        if (
+            self.key_type.get_upper_bound() is None or
+            self.value_type.get_upper_bound() is None
+        ):
             self.skipTest("Needs bounded key and value")
 
         import struct
 
         good = set()
         b = self._makeOne()
 
         # Some platforms (Windows) use a 32-bit value for long,
         # meaning that PyInt_AsLong and such can throw OverflowError
-        # for values that are in range on most other platforms. And on Python 2,
-        # PyInt_Check can fail with a TypeError starting at small values
+        # for values that are in range on most other platforms. And on Python
+        # 2, PyInt_Check can fail with a TypeError starting at small values
         # like 2147483648. So we look for small longs and catch those errors
         # even when we think we should be in range. In all cases, our code
-        # catches the unexpected error (OverflowError) and turns it into TypeError.
+        # catches the unexpected error (OverflowError) and turns it into
+        # TypeError.
         long_is_32_bit = struct.calcsize('@l') < 8
         in_range_errors = TypeError
         out_of_range_errors = TypeError
 
-        K = self.KEYS
         V = self.VALUES
+
         def trial(i):
             i = int(i)
             __traceback_info__ = i, type(i)
             # As key
             if i > self.key_type.get_upper_bound():
                 with self.assertRaises(out_of_range_errors):
                     b[i] = V[0]
@@ -1351,16 +1397,16 @@
                 self.assertEqual(9, len(b))
 
     @_skip_wo_ZODB
     def testAccessRaisesPOSKeyErrorOnSelf(self):
         # We don't hide a POSKeyError that happens when
         # accessing the object itself in `get()`.
         # See https://github.com/zopefoundation/BTrees/issues/161
-        from ZODB.POSException import POSKeyError
         import transaction
+        from ZODB.POSException import POSKeyError
         transaction.begin()
         m = self._makeOne()
         root = self._getRoot()
         root.m = m
         transaction.commit()
         conn = root._p_jar
         # Ghost the object
@@ -1383,42 +1429,43 @@
                 _ = K[1] in m
 
             with self.assertRaises(POSKeyError):
                 m.pop(K[1])
         finally:
             self._closeRoot(root)
 
+
 class BTreeTests(MappingBase):
     # Tests common to all BTrees
 
     def _getTargetClass(self):
         # Most of the subclasses override _makeOne and not
         # _getTargetClass, so we can get the type that way.
         # TODO: This could change for less repetition in the subclasses,
         # using the name of the class to import the module and find
         # the type.
         if type(self)._makeOne is not BTreeTests._makeOne:
             return type(self._makeOne())
         raise NotImplementedError()
 
-    def _makeOne(self, *args): # pylint:disable=arguments-differ
+    def _makeOne(self, *args):
         return self._getTargetClass()(*args)
 
     def _checkIt(self, t):
         from BTrees.check import check
         t._check()
         check(t)
 
     @_skip_wo_ZODB
     def testAccessRaisesPOSKeyErrorOnNested(self):
         # We don't hide a POSKeyError that happens when
         # accessing sub objects in `get()`.
         # See https://github.com/zopefoundation/BTrees/issues/161
-        from ZODB.POSException import POSKeyError
         import transaction
+        from ZODB.POSException import POSKeyError
         transaction.begin()
         m = self._makeOne()
         root = self._getRoot()
         root.m = m
         self._populate(m, 1000)
         transaction.commit()
         conn = root._p_jar
@@ -1773,15 +1820,18 @@
         self.assertTrue(len(items) > 2)   # at least two buckets and a key
         # All values in the first bucket are < firstkey.  All in the
         # second bucket are >= firstkey, and firstkey is the first key in
         # the second bucket.
         firstkey = items[1]
         therange = t.keys(self.coerce_to_key(before_range_begin), firstkey)
         self.assertEqual(len(therange), firstkey + firstkey_offset)
-        self.assertEqual(list(therange), list(range(range_begin, firstkey + 1)))
+        self.assertEqual(
+            list(therange), list(range(range_begin, firstkey + 1))
+        )
+
         # Now for the tricky part.  If we delete firstkey, the second bucket
         # loses its smallest key, but firstkey remains in the BTree node.
         # If we then do a high-end range search on firstkey, the BTree node
         # directs us to look in the second bucket, but there's no longer any
         # key <= firstkey in that bucket.  The correct answer points to the
         # end of the *first* bucket.  The algorithm has to be smart enough
         # to "go backwards" in the BTree then; if it doesn't, it will
@@ -1838,23 +1888,26 @@
         # to set _p_changed (adding the first item sets it because
         # the _firstbucket gets set, but the second item only grew the
         # existing bucket)
         t = self._makeOne()
         # Note that for the property to actually hold, we have to fake a
         # _p_jar and _p_oid
         t._p_oid = b'\0\0\0\0\0'
+
         class Jar:
             def __init__(self):
                 self._cache = self
                 self.registered = None
 
             def mru(self, arg):
                 pass
+
             def readCurrent(self, arg):
                 pass
+
             def register(self, arg):
                 self.registered = arg
 
         t._p_jar = Jar()
         K = self.KEYS
         V = self.VALUES
         t[K[1]] = V[3]
@@ -1892,23 +1945,26 @@
         # get set
         t = self._makeOne()
         K = self.KEYS
         V = self.VALUES
         # Note that for the property to actually hold, we have to fake a
         # _p_jar and _p_oid
         t._p_oid = b'\0\0\0\0\0'
+
         class Jar:
             def __init__(self):
                 self._cache = self
                 self.registered = None
 
             def mru(self, arg):
                 pass
+
             def readCurrent(self, arg):
                 pass
+
             def register(self, arg):
                 self.registered = arg
 
         t._p_jar = Jar()
         t[K[0]] = V[1]
         t[K[1]] = V[2]
         # reset these, setting _firstbucket triggered a change
@@ -1932,15 +1988,16 @@
             s = pickle.dumps(made_one, proto)
             # It's not legacy
             assert b'TreePy\n' not in s, repr(s)
             # \np for protocol 1, \nq for proto 2,
             assert b'Tree\np' in s or b'Tree\nq' in s, repr(s)
 
             # Now make it pseudo-legacy
-            legacys = s.replace(b'Tree\np', b'TreePy\np').replace(b'Tree\nq', b'TreePy\nq')
+            legacys = s.replace(b'Tree\np', b'TreePy\np')
+            legacys = legacys.replace(b'Tree\nq', b'TreePy\nq')
 
             # It loads up as the specified class
             loaded_one = pickle.loads(legacys)
 
             # It still functions and can be dumped again, as the original class
             s2 = pickle.dumps(loaded_one, proto)
             self.assertTrue(b'Py' not in s2)
@@ -1959,24 +2016,26 @@
             b[K[1]] = V[11]
 
         # xchild is non-BTree class deriving from Persistent
         import persistent
         xchild = persistent.Persistent()
         self.assertIs(xchild._p_oid, None)
 
-        typeErrOK = "tree child %s is neither %s nor %s" % \
-                        (_tp_name(type(xchild)), _tp_name(type(t)),
-                         _tp_name(t._bucket_type))
+        typeErrOK = "tree child {} is neither {} nor {}".format(
+            _tp_name(type(xchild)),
+            _tp_name(type(t)),
+            _tp_name(t._bucket_type)
+        )
 
         # if the following is allowed, e.g.
         # t.__getstate__(), or t[0]=1 corrupt memory and crash.
         with self.assertRaises(TypeError) as exc:
             t.__setstate__(
                 (
-                    (xchild,), # child0 is neither tree nor bucket
+                    (xchild,),  # child0 is neither tree nor bucket
                     b
                 )
             )
         self.assertEqual(str(exc.exception), typeErrOK)
 
         # if the following is allowed, e.g. t[5]=1 corrupts memory and crash.
         with self.assertRaises(TypeError) as exc:
@@ -1992,17 +2051,17 @@
 class NormalSetTests(Base):
     # Test common to all set types
 
     def _getCollectionsABC(self):
         import collections.abc
         return collections.abc.MutableSet
 
-    def _populate(self, t, l):
+    def _populate(self, t, largest):
         # Make some data
-        t.update(self.coerce_to_key(k) for k in range(l))
+        t.update(self.coerce_to_key(k) for k in range(largest))
 
     def test_isdisjoint(self):
         t = self._makeOne()
         K = self.KEYS
         # The empty set is disjoint with itself
         self.assertTrue(t.isdisjoint(t))
         # Empty sequences
@@ -2114,31 +2173,30 @@
 
         t -= t
         self.assertIs(t, orig_t)
         self.assertEqual(set(t), set())
 
     def test___ixor__(self):
         t = self._makeOne()
-        orig_t = t
         K = self.KEYS
         t ^= (K[1],)
-        self.assertEqual(set(t), {K[1],})
+        self.assertEqual(set(t), {K[1]})
         t ^= t
         self.assertEqual(set(t), set())
 
         t ^= (K[1], K[2], K[3])
         self.assertEqual(set(t), {K[1], K[2], K[3]})
         t ^= [K[2], K[3], K[4]]
         self.assertEqual(set(t), {K[1], K[4]})
 
     def test___xor__(self):
         t = self._makeOne()
         K = self.KEYS
         u = t ^ (K[1],)
-        self.assertEqual(set(u), {K[1],})
+        self.assertEqual(set(u), {K[1]})
         u = t ^ t
         self.assertEqual(set(u), set())
 
         u = t ^ (K[1], K[2], K[3])
         self.assertEqual(set(u), {K[1], K[2], K[3]})
         t.update(u)
         u = t ^ [K[2], K[3], K[4]]
@@ -2163,15 +2221,14 @@
             self.assertIn("<BTrees.", r)
             self.assertIn('TreeSet object at', r)
             self.assertIn('oid 0x3132333435363738', r)
 
         # Make sure it's the same between Python and C
         self.assertNotIn('Py', r)
 
-
     def testInsertReturnsValue(self):
         t = self._makeOne()
         K = self.KEYS
         self.assertEqual(t.insert(K[5]), 1)
         self.assertEqual(t.add(K[4]), 1)
 
     def testDuplicateInsert(self):
@@ -2223,15 +2280,14 @@
         for x in r:
             t.insert(x)
         diff = lsubtract(t.keys(), r)
         self.assertEqual(diff, [])
         diff = lsubtract(t.keys(None, None), r)
         self.assertEqual(diff, [])
 
-
     def testClear(self):
         t = self._makeOne()
         r = range(1000)
         K = self.KEYS
         for x in r:
             t.insert(K[x])
         t.clear()
@@ -2280,24 +2336,24 @@
             else:
                 self.fail("expected ValueError")
 
     def testUpdate(self):
         import random
         t = self._makeOne()
         d = {}
-        l = []
+        keys = []
         for i in range(10000):
             k = random.randrange(*self.KEY_RANDRANGE_ARGS)
             k = self.coerce_to_key(k)
             d[k] = self.coerce_to_value(i)
-            l.append(k)
+            keys.append(k)
 
         items = sorted(d.keys())
 
-        t.update(l)
+        t.update(keys)
         self.assertEqual(list(t.keys()), items)
 
     def testEmptyRangeSearches(self):
         t = self._makeOne()
         K = self.KEYS
         t.update([K[1], K[5], K[9]])
         if self.SUPPORTS_NEGATIVE_KEYS:
@@ -2386,23 +2442,26 @@
         # deleting an item in a small set to fail to set _p_changed.
         # There must be at least two objects so that _firstbucket doesn't
         # get set
         t = self._makeOne()
         # Note that for the property to actually hold, we have to fake a
         # _p_jar and _p_oid
         t._p_oid = b'\0\0\0\0\0'
+
         class Jar:
             def __init__(self):
                 self._cache = self
                 self.registered = None
 
             def mru(self, arg):
                 pass
+
             def readCurrent(self, arg):
                 pass
+
             def register(self, arg):
                 self.registered = arg
 
         t._p_jar = Jar()
         t.add(self.KEYS[0])
         t.add(self.KEYS[1])
         # reset these, setting _firstbucket triggered a change
@@ -2417,33 +2476,36 @@
     def testAddingOneSetsChanged(self):
         # A bug in the BTree Set Python implementation once caused
         # adding an object not to set _p_changed
         t = self._makeOne()
         # Note that for the property to actually hold, we have to fake a
         # _p_jar and _p_oid
         t._p_oid = b'\0\0\0\0\0'
+
         class Jar:
             def __init__(self):
                 self._cache = self
                 self.registered = None
 
             def mru(self, arg):
                 pass
+
             def readCurrent(self, arg):
                 pass
+
             def register(self, arg):
                 self.registered = arg
 
         t._p_jar = Jar()
         t.add(self.KEYS[0])
         self.assertTrue(t._p_changed)
         self.assertEqual(t, t._p_jar.registered)
 
-        # Whether or not doing `t.add(0)` again would result in
-        # _p_changed being set depends on whether this is a TreeSet or a plain Set
+        # Whether or not doing `t.add(0)` again would result in _p_changed
+        # being set depends on whether this is a TreeSet or a plain Set
 
 
 class ExtendedSetTests(NormalSetTests):
 
     def testLen(self):
         t = self._makeOne()
         r = range(10000)
@@ -2457,17 +2519,19 @@
         r = range(10000)
         to_key = self.coerce_to_key
         for x in r:
             t.insert(to_key(x))
         for x in r:
             self.assertEqual(t[x], to_key(x))
 
+
 class KeyCoercionFailed(Exception):
     """Raised when we use a static key that we expect to be able to fit."""
 
+
 class InternalKeysMappingTest:
     # There must not be any internal keys not in the BTree
 
     def _makeOne(self):
         return self._getTargetClass()()
 
     def add_key(self, tree, i):
@@ -2492,17 +2556,18 @@
         db = DB()
         conn = db.open()
 
         tree = conn.root.tree = self._makeOne()
         i = 0
 
         # Grow the btree until we have multiple buckets.
-        # (Calling ``__getstate__`` to check the internals is expensive, especially
-        # with the Python implementation, so only do so when we hit the threshold we expect
-        # the tree to grow. This makes the difference between a 6s test and a 0.6s test.)
+        # (Calling ``__getstate__`` to check the internals is expensive,
+        # especially with the Python implementation, so only do so when we hit
+        # the threshold we expect the tree to grow. This makes the difference
+        # between a 6s test and a 0.6s test.)
         bucket_size = self.key_type.bucket_size_for_value(self.value_type)
         tree_size = self.key_type.tree_size
         while 1:
             i += 1
             self.add_key(tree, i)
             if i >= bucket_size:
                 data = tree.__getstate__()[0]
@@ -2546,14 +2611,15 @@
 
 
 class ModuleTest:
     # test for presence of generic names in module
     prefix = ''
     key_type = None
     value_type = None
+
     def _getModule(self):
         raise NotImplementedError
 
     def testNames(self):
         names = ['Bucket', 'BTree', 'Set', 'TreeSet']
         mod = self._getModule()
         mod_all = mod.__all__
@@ -2628,15 +2694,15 @@
         t = self._makeOne()
         with self.assertRaises(TypeError):
             t.update([1, object()])
 
     def __test_key(self, k):
         try:
             self.key_type(k)
-        except Exception as e: # pylint:disable=broad-except
+        except Exception as e:
             with self.assertRaises(type(e)):
                 self._makeOne().insert(k)
         else:
             self._makeOne().insert(k)
 
     def test_key_type_str(self):
         self.__test_key('c')
@@ -2650,15 +2716,15 @@
 
 LARGEST_32_BITS = 2147483647
 SMALLEST_32_BITS = -LARGEST_32_BITS - 1
 
 SMALLEST_POSITIVE_33_BITS = LARGEST_32_BITS + 1
 LARGEST_NEGATIVE_33_BITS = SMALLEST_32_BITS - 1
 
-LARGEST_64_BITS = 0x7fffffffffffffff # Signed. 2**63 - 1
+LARGEST_64_BITS = 0x7fffffffffffffff  # Signed. 2**63 - 1
 SMALLEST_64_BITS = -LARGEST_64_BITS - 1
 
 SMALLEST_POSITIVE_65_BITS = LARGEST_64_BITS + 1
 LARGEST_NEGATIVE_65_BITS = SMALLEST_64_BITS - 1
 
 
 class TestLongIntSupport:
@@ -2674,30 +2740,30 @@
         #
         # These values must be usable as keys.
         return 0, 1
 
     def _skip_if_not_64bit(self):
         mod = sys.modules[self._getTargetClass().__module__]
         if not mod.using64bits:
-            self.skipTest("Needs 64 bit support.") # pragma: no cover
+            self.skipTest("Needs 64 bit support.")  # pragma: no cover
+
 
 class TestLongIntKeys(TestLongIntSupport):
     SUPPORTS_NEGATIVE_KEYS = True
 
     def _makeLong(self, v):
         try:
             return long(v)
-        except NameError: # pragma: no cover
+        except NameError:  # pragma: no cover
             return int(v)
 
     def testLongIntKeysWork(self):
         self._skip_if_not_64bit()
         t = self._makeOne()
         K = self.KEYS
-        V = self.VALUES
         o1, o2 = self.getTwoValues()
         assert o1 != o2
 
         # Test some small key values first:
         one_long = self._makeLong(1)
         t[one_long] = o1
         self.assertEqual(t[K[1]], o1)
@@ -2720,24 +2786,30 @@
         self.assertEqual(list(t.keys(k3, None)), [k3, 1, k1, k2])
         self.assertEqual(list(t.keys(None, k2)), [k3, 1, k1, k2])
 
     def testLongIntKeysOutOfRange(self):
         self._skip_if_not_64bit()
         o1, o2 = self.getTwoValues()
         t = self._makeOne()
-        k1 = SMALLEST_POSITIVE_65_BITS if self.SUPPORTS_NEGATIVE_KEYS else 2**64 + 1
+        k1 = (
+            SMALLEST_POSITIVE_65_BITS
+            if self.SUPPORTS_NEGATIVE_KEYS
+            else 2**64 + 1
+        )
         with self.assertRaises(TypeError):
             t[k1] = self.coerce_to_value(o1)
 
         t = self._makeOne()
         with self.assertRaises(TypeError):
             t[LARGEST_NEGATIVE_65_BITS] = self.coerce_to_value(o1)
 
+
 class TestLongIntValues(TestLongIntSupport):
     SUPPORTS_NEGATIVE_VALUES = True
+
     def testLongIntValuesWork(self):
         self._skip_if_not_64bit()
         t = self._makeOne()
         keys = sorted(self.getTwoKeys())
         k1, k2 = keys
         assert k1 != k2
 
@@ -2752,49 +2824,55 @@
         self.assertEqual(list(t.values()), [v1, v2])
         self.assertEqual(list(t.values(None, None)), [v1, v2])
 
     def testLongIntValuesOutOfRange(self):
         self._skip_if_not_64bit()
         k1, k2 = self.getTwoKeys()
         t = self._makeOne()
-        v1 = SMALLEST_POSITIVE_65_BITS if self.SUPPORTS_NEGATIVE_VALUES else 2**64 + 1
+        v1 = (
+            SMALLEST_POSITIVE_65_BITS
+            if self.SUPPORTS_NEGATIVE_VALUES
+            else 2**64 + 1
+        )
         with self.assertRaises(TypeError):
             t[k1] = self.coerce_to_value(v1)
 
         t = self._makeOne()
         with self.assertRaises(TypeError):
             t[k1] = self.coerce_to_value(LARGEST_NEGATIVE_65_BITS)
 
 
-# Given a mapping builder (IIBTree, OOBucket, etc), return a function
-# that builds an object of that type given only a list of keys.
 def makeMapBuilder(self, mapbuilder):
+    # Given a mapping builder (IIBTree, OOBucket, etc), return a function
+    # that builds an object of that type given only a list of keys.
     def result(keys=(), mapbuilder=mapbuilder, self=self):
         return mapbuilder(list(zip(
             (self.KEYS[k] for k in keys),
             (self.VALUES[k] for k in keys)
         )))
     return result
 
+
 def makeSetBuilder(self, setbuilder):
     def result(keys=(), setbuilder=setbuilder, self=self):
         return setbuilder(self.KEYS[k] for k in keys)
     return result
 
-# Subclasses have to set up:
-#     builders() - function returning functions to build inputs,
-#     each returned callable takes an optional keys arg
-#     intersection, union, difference - set to the type-correct versions
+
 class SetResult:
+    # Subclasses have to set up:
+    #     builders() - function returning functions to build inputs,
+    #     each returned callable takes an optional keys arg
+    #     intersection, union, difference - set to the type-correct versions
     def setUp(self):
         super().setUp()
         _skip_if_pure_py_and_py_test(self)
 
-        rawAkeys = [1,    3,    5, 6] # pylint:disable=bad-whitespace
-        rawBkeys = [   2, 3, 4,    6, 7] # pylint:disable=bad-whitespace
+        rawAkeys = [1,    3,    5, 6]
+        rawBkeys = [   2, 3, 4,    6, 7]  # noqa #201
         self.Akeys = [self.KEYS[k] for k in rawAkeys]
         self.Bkeys = [self.KEYS[k] for k in rawBkeys]
         self.As = [makeset(rawAkeys) for makeset in self.builders()]
         self.Bs = [makeset(rawBkeys) for makeset in self.builders()]
         self.emptys = [makeset() for makeset in self.builders()]
 
     # Slow but obviously correct Python implementations of basic ops.
@@ -2881,17 +2959,18 @@
         return x
 
     def testUnion(self):
         inputs = self.As + self.Bs
         for A in inputs:
             for B in inputs:
                 for convert in lambda x: x, self._reversed, list, tuple, set:
-                    # For all of these tests, we need to be sure we have at least
-                    # one value that is *not* sorted relative to the other.
-                    # See https://github.com/zopefoundation/BTrees/issues/171
+                    # For all of these tests, we need to be sure we have at
+                    # least one value that is *not* sorted relative to the
+                    # other.  See
+                    # https://github.com/zopefoundation/BTrees/issues/171
                     a = convert(A)
                     b = convert(B)
                     if hasattr(b, 'reverse'):
                         b.reverse()
                     __traceback_info__ = a, b
                     C = self.union(a, b)
                     self.assertTrue(not hasattr(C, "values"))
@@ -2918,25 +2997,28 @@
         for A in inputs:
             for B in inputs:
                 for convert in lambda x: x, self._reversed, list, tuple, set:
                     # Difference is unlike the others: The first argument
                     # must be a BTree type, in both C and Python.
                     C = self.difference(A, convert(B))
                     # Difference preserves LHS values.
-                    self.assertEqual(hasattr(C, "values"), hasattr(A, "values"))
+                    self.assertEqual(
+                        hasattr(C, "values"), hasattr(A, "values")
+                    )
                     want = self._difference(A, B)
                     if hasattr(A, "values"):
                         self.assertEqual(list(C.items()), want)
                     else:
                         self.assertEqual(list(C), want)
                     self.assertEqual(set(A) - set(B), set(A - B))
 
-    def testLargerInputs(self): # pylint:disable=too-many-locals
-        from BTrees.IIBTree import IISet # pylint:disable=no-name-in-module
+    def testLargerInputs(self):
         from random import randint
+
+        from BTrees.IIBTree import IISet
         MAXSIZE = 200
         MAXVAL = 400
         K = self.KEYS
         for i in range(3):
             n = randint(0, MAXSIZE)
             Akeys = [randint(1, MAXVAL) for j in range(n)]
             As = [makeset(Akeys) for makeset in self.builders()]
@@ -2953,23 +3035,26 @@
             for op, simulator in ((self.union, self._union),
                                   (self.intersection, self._intersection),
                                   (self.difference, self._difference)):
                 for A in As:
                     for B in Bs:
                         got = op(A, B)
                         want = simulator(Akeys, Bkeys)
-                        self.assertEqual(list(got), want,
-                                         (A, B, Akeys, Bkeys, list(got), want))
+                        self.assertEqual(
+                            list(got), want,
+                            (A, B, Akeys, Bkeys, list(got), want)
+                        )
+
 
-# Subclasses must set up (as class variables):
-#     weightedUnion, weightedIntersection
-#     builders -- sequence of constructors, taking items
-#     union, intersection -- the module routines of those names
-#     mkbucket -- the module bucket builder
 class Weighted(SignedMixin):
+    # Subclasses must set up (as class variables):
+    #     weightedUnion, weightedIntersection
+    #     builders -- sequence of constructors, taking items
+    #     union, intersection -- the module routines of those names
+    #     mkbucket -- the module bucket builder
 
     def setUp(self):
         self.Aitems = [(1, 10), (3, 30), (5, 50), (6, 60)]
         self.Bitems = [(2, 21), (3, 31), (4, 41), (6, 61), (7, 71)]
 
         self.As = [make(self.Aitems) for make in self.builders()]
         self.Bs = [make(self.Bitems) for make in self.builders()]
@@ -3041,15 +3126,18 @@
                 self.assertEqual(got_w, want_w)
                 if isaset(got_s):
                     self.assertEqual(got_s.keys(), want_s)
                 else:
                     self.assertEqual(got_s.items(), want_s)
 
                 for w1, w2 in self.weights:
-                    if (w1 < 0 or w2 < 0) and not self.SUPPORTS_NEGATIVE_VALUES:
+                    if (
+                        (w1 < 0 or w2 < 0) and
+                        not self.SUPPORTS_NEGATIVE_VALUES
+                    ):
                         continue
                     want_w, want_s = self._wunion(A, B, w1, w2)
                     got_w, got_s = self.weightedUnion()(A, B, w1, w2)
                     self.assertEqual(got_w, want_w)
                     if isaset(got_s):
                         self.assertEqual(got_s.keys(), want_s)
                     else:
@@ -3075,41 +3163,47 @@
                 self.assertEqual(got_w, want_w)
                 if isaset(got_s):
                     self.assertEqual(got_s.keys(), want_s)
                 else:
                     self.assertEqual(got_s.items(), want_s)
 
                 for w1, w2 in self.weights:
-                    if (w1 < 0 or w2 < 0) and not self.SUPPORTS_NEGATIVE_VALUES:
+                    if (
+                        (w1 < 0 or w2 < 0) and
+                        not self.SUPPORTS_NEGATIVE_VALUES
+                    ):
                         continue
                     want_w, want_s = self._wintersection(A, B, w1, w2)
                     got_w, got_s = self.weightedIntersection()(A, B, w1, w2)
                     self.assertEqual(got_w, want_w)
                     if isaset(got_s):
                         self.assertEqual(got_s.keys(), want_s)
                     else:
                         self.assertEqual(got_s.items(), want_s)
 
+
 # Given a set builder (like OITreeSet or OISet), return a function that
 # takes a list of (key, value) pairs and builds a set out of the keys.
 def itemsToSet(setbuilder):
     def result(items, setbuilder=setbuilder):
         return setbuilder([key for key, value in items])
     return result
 
+
 # 'thing' is a bucket, btree, set or treeset.  Return true iff it's one of the
 # latter two.
 def isaset(thing):
     return not hasattr(thing, 'values')
 
-# Subclasses must set up (as class variables):
-#     multiunion, union
-#     mkset, mktreeset
-#     mkbucket, mkbtree
+
 class MultiUnion(SignedMixin):
+    # Subclasses must set up (as class variables):
+    #     multiunion, union
+    #     mkset, mktreeset
+    #     mkbucket, mkbtree
 
     def setUp(self):
         super().setUp()
         _skip_if_pure_py_and_py_test(self)
 
     def testEmpty(self):
         self.assertEqual(len(self.multiunion([])), 0)
@@ -3200,15 +3294,18 @@
             raise MyException
 
         with self.assertRaises(MyException):
             self.multiunion((gen(),))
 
     def testBigInput(self):
         N = 100000
-        if (_c_optimizations_ignored() or 'Py' in type(self).__name__) and not PYPY:
+        if (
+            (_c_optimizations_ignored() or 'Py' in type(self).__name__) and
+            not PYPY
+        ):
             # This is extremely slow in CPython implemented in Python,
             # taking 20s or more on a 2015-era laptop
             N = N // 10
         input = self.mkset(list(range(N)))
         output = self.multiunion([input] * 10)
         self.assertEqual(len(output), N)
         self.assertEqual(output.minKey(), 0)
@@ -3239,15 +3336,15 @@
         # The internal set iteration protocol allows "iterating over" a
         # a single key as if it were a set.
         N = 100
         union, mkset = self.union, self.mkset
         slow = mkset()
         for i in range(N):
             slow = union(slow, mkset([i]))
-        fast = self.multiunion(list(range(N))) # like N distinct singleton sets
+        fast = self.multiunion(list(range(N)))  # ~ N distinct singleton sets
         self.assertEqual(len(slow), N)
         self.assertEqual(len(fast), N)
         self.assertEqual(list(slow), list(fast))
         self.assertEqual(list(fast), list(range(N)))
 
 
 class ConflictTestBase(SignedMixin):
@@ -3255,14 +3352,15 @@
 
     storage = None
     db = None
 
     def setUp(self):
         super().setUp()
         _skip_if_pure_py_and_py_test(self)
+
         def identity(x):
             return x
 
         self.key_tx = abs if not self.SUPPORTS_NEGATIVE_KEYS else identity
         self.val_tx = abs if not self.SUPPORTS_NEGATIVE_VALUES else identity
 
     def tearDown(self):
@@ -3273,23 +3371,25 @@
             self.storage.cleanup()
 
     def _makeOne(self):
         return self._getTargetClass()()
 
     def openDB(self):
         import os
-        from ZODB.FileStorage import FileStorage
+
         from ZODB.DB import DB
+        from ZODB.FileStorage import FileStorage
         n = 'fs_tmp__%s' % os.getpid()
         self.storage = FileStorage(n)
         self.db = DB(self.storage)
         return self.db
 
-
-    def _test_merge(self, o1, o2, o3, expect, message='failed to merge', should_fail=False):
+    def _test_merge(
+        self, o1, o2, o3, expect, message='failed to merge', should_fail=False,
+    ):
         from BTrees.Interfaces import BTreesConflictError
         s1 = o1.__getstate__()
         s2 = o2.__getstate__()
         s3 = o3.__getstate__()
         expected = expect.__getstate__()
         if expected is None:
             expected = ((((),),),)
@@ -3309,48 +3409,48 @@
     def _skip_if_only_small_keys(self):
         try:
             self.coerce_to_key(99999)
         except TypeError:
             assert 'fs' in self._getTargetClass().__name__
             self.skipTest("Uses keys too large for fsBTree")
 
-
     def _deletefail(self):
         t = self._makeOne()
         del t[self.KEYS[1]]
 
     def _setupConflict(self):
         if self._getTargetClass().__name__.startswith('fs'):
-            # Too many negative numbers, could be done with a little work though.
+            # Too many negative numbers, could be done with a little work
+            # though.
             self.skipTest("Needs ported to fsBTree")
         key_tx = self.key_tx
-        l = [
+        keys = [
             -5124, -7377, 2274, 8801, -9901, 7327, 1565, 17, -679,
             3686, -3607, 14, 6419, -5637, 6040, -4556, -8622, 3847, 7191,
             -4067
         ]
-        l = [key_tx(v) for v in l]
+        keys = [key_tx(v) for v in keys]
 
         e1 = [(-1704, 0), (5420, 1), (-239, 2), (4024, 3), (-6984, 4)]
         e1 = [(key_tx(k), v) for k, v in e1]
         e2 = [(7745, 0), (4868, 1), (-2548, 2), (-2711, 3), (-3154, 4)]
         e2 = [(key_tx(k), v) for k, v in e2]
 
         base = self._makeOne()
         base.update([
             (self.coerce_to_key(i), self.coerce_to_value(i * i))
-            for i in l[:20]
+            for i in keys[:20]
         ])
         b1 = type(base)(base)
         b2 = type(base)(base)
         bm = type(base)(base)
 
         items = base.items()
 
-        return  base, b1, b2, bm, e1, e2, items
+        return base, b1, b2, bm, e1, e2, items
 
     def testMergeDelete(self):
         base, b1, b2, bm, e1, e2, items = self._setupConflict()
         del b1[items[1][0]]
         del b2[items[5][0]]
         del b1[items[-1][0]]
         del b2[items[-2][0]]
@@ -3401,21 +3501,26 @@
         self._test_merge(base, b1, b2, bm, 'merge conflicting update',
                          should_fail=1)
 
     def testFailMergeDeleteAndUpdate(self):
         base, b1, b2, bm, e1, e2, items = self._setupConflict()
         del b1[items[0][0]]
         b2[items[0][0]] = self.val_tx(-9)
-        self._test_merge(base, b1, b2, bm, 'merge conflicting update and delete',
-                         should_fail=1)
+        self._test_merge(
+            base,
+            b1,
+            b2,
+            bm,
+            'merge conflicting update and delete',
+            should_fail=1,
+        )
 
     def testMergeInserts(self):
         self._skip_if_only_small_keys()
         base, b1, b2, bm, e1, e2, items = self._setupConflict()
-        V = self.VALUES
         b1[self.key_tx(-99999)] = self.val_tx(-99999)
         b1[e1[0][0]] = e1[0][1]
         b2[99999] = self.coerce_to_value(99999)
         b2[e1[2][0]] = e1[2][1]
 
         bm[self.key_tx(-99999)] = self.val_tx(-99999)
         bm[e1[0][0]] = e1[0][1]
@@ -3443,28 +3548,31 @@
         base, b1, b2, bm, e1, e2, items = self._setupConflict()
 
         b1.clear()
         bm.clear()
         b2.update(e2)
         bm.update(e2)
 
-        self._test_merge(base, b1, b2, bm, 'merge insert from empty', should_fail=1)
+        self._test_merge(
+            base, b1, b2, bm, 'merge insert from empty', should_fail=1,
+        )
 
     def testMergeEmpty(self):
         base, b1, b2, bm, e1, e2, items = self._setupConflict()
 
         b1.clear()
         bm.clear()
 
-        self._test_merge(base, b1, b2, bm, 'empty one and not other', should_fail=1)
+        self._test_merge(
+            base, b1, b2, bm, 'empty one and not other', should_fail=1,
+        )
 
     def testFailMergeInsert(self):
         self._skip_if_only_small_keys()
         base, b1, b2, bm, e1, e2, items = self._setupConflict()
-        V = self.VALUES
         b1[self.key_tx(-99999)] = self.val_tx(-99999)
         b1[e1[0][0]] = e1[0][1]
         b2[99999] = self.coerce_to_value(99999)
         b2[e1[0][0]] = e1[0][1]
         self._test_merge(base, b1, b2, bm, 'merge conflicting inserts',
                          should_fail=1)
 
@@ -3476,35 +3584,40 @@
         try:
             self.coerce_to_key(99999)
         except TypeError:
             assert 'fs' in self._getTargetClass().__name__
             self.skipTest("Uses keys too large for fsBTree")
 
     def _setupConflict(self):
-        to_key = lambda x: self.coerce_to_key(self.key_tx(x))
-        l = [to_key(x)for x in [
-            -5124, -7377, 2274, 8801, -9901, 7327, 1565, 17, -679,
-            3686, -3607, 14, 6419, -5637, 6040, -4556, -8622, 3847, 7191,
-            -4067]]
+
+        def to_key(x):
+            return self.coerce_to_key(self.key_tx(x))
+
+        items = [
+            to_key(x)for x in [
+                -5124, -7377, 2274, 8801, -9901, 7327, 1565, 17, -679,
+                3686, -3607, 14, 6419, -5637, 6040, -4556, -8622, 3847, 7191,
+                -4067,
+            ]
+        ]
 
         e1 = [to_key(x) for x in
               [-1704, 5420, -239, 4024, -6984]]
         e2 = [to_key(x) for x in
               [7745, 4868, -2548, -2711, -3154]]
 
-
         base = self._makeOne()
-        base.update(l)
+        base.update(items)
         b1 = base.__class__(base)
         b2 = base.__class__(base)
         bm = base.__class__(base)
 
         items = base.keys()
 
-        return  base, b1, b2, bm, e1, e2, items
+        return base, b1, b2, bm, e1, e2, items
 
     def testMergeDelete(self):
         base, b1, b2, bm, e1, e2, items = self._setupConflict()
         b1.remove(items[1])
         b2.remove(items[5])
         b1.remove(items[-1])
         b2.remove(items[-2])
@@ -3556,45 +3669,52 @@
         base, b1, b2, bm, e1, e2, items = self._setupConflict()
 
         b1.clear()
         bm.clear()
         b2.update(e2)
         bm.update(e2)
 
-        self._test_merge(base, b1, b2, bm, 'merge insert from empty', should_fail=1)
+        self._test_merge(
+            base, b1, b2, bm, 'merge insert from empty', should_fail=1,
+        )
 
     def testMergeEmpty(self):
         base, b1, b2, bm, e1, e2, items = self._setupConflict()
 
         b1.clear()
         bm.clear()
 
-        self._test_merge(base, b1, b2, bm, 'empty one and not other', should_fail=1)
+        self._test_merge(
+            base, b1, b2, bm, 'empty one and not other', should_fail=1,
+        )
 
     def testFailMergeInsert(self):
         self._skip_if_only_small_keys()
         base, b1, b2, bm, e1, e2, items = self._setupConflict()
         b1.insert(self.coerce_to_key(self.key_tx(-99999)))
         b1.insert(e1[0])
         b2.insert(99999)
         b2.insert(e1[0])
         self._test_merge(base, b1, b2, bm, 'merge conflicting inserts',
                          should_fail=1)
 
-## utility functions
+# utility functions
+
 
 def lsubtract(l1, l2):
     l1 = list(l1)
     l2 = list(l2)
     return (list(filter(lambda x, l1=l1: x not in l1, l2)) +
             list(filter(lambda x, l2=l2: x not in l2, l1)))
 
+
 def realseq(itemsob):
     return list(itemsob)
 
+
 def permutations(x):
     # Return a list of all permutations of list x.
     n = len(x)
     if n <= 1:
         return [x]
     result = []
     x0 = x[0]
```

### Comparing `BTrees-5.2/src/BTrees/tests/testBTrees.py` & `BTrees-6.0/src/BTrees/tests/testBTrees.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,17 +54,17 @@
     # answer is the 3 bucket, which requires going in a different direction
     # at the very top node already.  Consider a low-end range search for
     # 9.  The BTree nodes direct it to the 7 bucket, but the correct answer
     # is the 11 bucket.  This is also a nasty-case tree for deletions.
 
     def _build_degenerate_tree(self):
         # Build the buckets and chain them together.
+        from BTrees.check import check
         from BTrees.IIBTree import IISet
         from BTrees.IIBTree import IITreeSet
-        from BTrees.check import check
         bucket11 = IISet([11])
 
         bucket7 = IISet()
         bucket7.__setstate__(((7,), bucket11))
 
         bucket5 = IISet()
         bucket5.__setstate__(((5,), bucket7))
@@ -191,27 +191,24 @@
 
 
 LP294788_ids = {}
 
 
 class ToBeDeleted:
     def __init__(self, id):
-        assert isinstance(id, int) #we don't want to store any object ref here
+        assert isinstance(id, int)  # don't want to store any object ref here
         self.id = id
 
         global LP294788_ids
         LP294788_ids[id] = 1
 
     def __del__(self):
         global LP294788_ids
         LP294788_ids.pop(self.id, None)
 
-    def __cmp__(self, other):
-        return cmp(self.id, other.id)
-
     def __le__(self, other):
         return self.id <= other.id
 
     def __lt__(self, other):
         return self.id < other.id
 
     def __eq__(self, other):
@@ -251,171 +248,173 @@
         # a separate reference dict is populated on object creation
         # and removed in __del__
         # That means what's left in the reference dict is never GC'ed
         # therefore referenced somewhere
         # To simulate real life, some random data is used to exercise the tree
         import gc
         import random
+
         from BTrees.OOBTree import OOBTree
 
         t = OOBTree()
 
         trandom = random.Random('OOBTree')
 
         global LP294788_ids
 
         # /// BTree keys are integers, value is an object
         LP294788_ids = {}
         ids = {}
         for i in range(1024):
             if trandom.random() > 0.1 or not ids:
-                #add
+                # add
                 id = None
                 while id is None or id in ids:
                     id = trandom.randint(0, 1000000)
 
                 ids[id] = 1
                 t[id] = ToBeDeleted(id)
             else:
-                #del
+                # del
                 keys = list(ids.keys())
                 if keys:
                     id = trandom.choice(list(ids.keys()))
                     del t[id]
                     del ids[id]
 
         ids = ids.keys()
         trandom.shuffle(list(ids))
         for id in ids:
             del t[id]
         ids = None
 
-        #to be on the safe side run a full GC
+        # to be on the safe side run a full GC
         gc.collect()
 
-        #print LP294788_ids
+        # print LP294788_ids
 
         self.assertEqual(len(t), 0)
         self.assertEqual(len(LP294788_ids), 0)
         # \\\
 
         # /// BTree keys are integers, value is a tuple having an object
         LP294788_ids = {}
         ids = {}
         for i in range(1024):
             if trandom.random() > 0.1 or not ids:
-                #add
+                # add
                 id = None
                 while id is None or id in ids:
                     id = trandom.randint(0, 1000000)
 
                 ids[id] = 1
                 t[id] = (id, ToBeDeleted(id), 'somename')
             else:
-                #del
+                # del
                 keys = list(ids.keys())
                 if keys:
                     id = trandom.choice(keys)
                     del t[id]
                     del ids[id]
 
         ids = ids.keys()
         trandom.shuffle(list(ids))
         for id in ids:
             del t[id]
         ids = None
 
-        #to be on the safe side run a full GC
+        # to be on the safe side run a full GC
         gc.collect()
 
-        #print LP294788_ids
+        # print LP294788_ids
 
         self.assertEqual(len(t), 0)
         self.assertEqual(len(LP294788_ids), 0)
         # \\\
 
-
         # /// BTree keys are objects, value is an int
         t = OOBTree()
         LP294788_ids = {}
         ids = {}
         for i in range(1024):
             if trandom.random() > 0.1 or not ids:
-                #add
+                # add
                 id = None
                 while id is None or id in ids:
                     id = ToBeDeleted(trandom.randint(0, 1000000))
 
                 ids[id] = 1
                 t[id] = 1
             else:
-                #del
+                # del
                 id = trandom.choice(list(ids.keys()))
                 del ids[id]
                 del t[id]
 
         ids = ids.keys()
         trandom.shuffle(list(ids))
         for id in ids:
             del t[id]
-        #release all refs
+        # release all refs
         ids = id = None
 
-        #to be on the safe side run a full GC
+        # to be on the safe side run a full GC
         gc.collect()
 
-        #print LP294788_ids
+        # print LP294788_ids
 
         self.assertEqual(len(t), 0)
         self.assertEqual(len(LP294788_ids), 0)
 
         # /// BTree keys are tuples having objects, value is an int
         t = OOBTree()
         LP294788_ids = {}
         ids = {}
         for i in range(1024):
             if trandom.random() > 0.1 or not ids:
-                #add
+                # add
                 id = None
                 while id is None or id in ids:
                     id = trandom.randint(0, 1000000)
                     id = (id, ToBeDeleted(id), 'somename')
 
                 ids[id] = 1
                 t[id] = 1
             else:
-                #del
+                # del
                 id = trandom.choice(list(ids.keys()))
                 del ids[id]
                 del t[id]
 
         ids = ids.keys()
         trandom.shuffle(list(ids))
         for id in ids:
             del t[id]
-        #release all refs
-        ids = id = key = None
+        # release all refs
+        ids = id = None
 
-        #to be on the safe side run a full GC
+        # to be on the safe side run a full GC
         gc.collect()
 
-        #print LP294788_ids
+        # print LP294788_ids
 
         self.assertEqual(len(t), 0)
         self.assertEqual(len(LP294788_ids), 0)
 
 
-# cmp error propagation tests
+# comparison error propagation tests
 
 
 class DoesntLikeBeingCompared:
 
-    def __cmp__(self, other):
+    def _cmp(self, other):
         raise ValueError('incomparable')
-    __lt__ = __le__ = __eq__ = __ne__ = __ge__ = __gt__ = __cmp__
+
+    __lt__ = __le__ = __eq__ = __ne__ = __ge__ = __gt__ = _cmp
+
 
 class TestCmpError(unittest.TestCase):
 
     def testFoo(self):
         from BTrees.OOBTree import OOBTree
         t = OOBTree()
         t['hello world'] = None
@@ -427,14 +426,15 @@
             self.fail('incomarable objects should not be allowed into '
                       'the tree')
 
 
 class FamilyTest(unittest.TestCase):
     def test32(self):
         from zope.interface.verify import verifyObject
+
         import BTrees
         from BTrees.IOBTree import IOTreeSet
         verifyObject(BTrees.Interfaces.IBTreeFamily, BTrees.family32)
         self.assertEqual(
             BTrees.family32.IO, BTrees.IOBTree)
         self.assertEqual(
             BTrees.family32.OI, BTrees.OIBTree)
@@ -469,14 +469,15 @@
 
         with self.assertRaises((TypeError, OverflowError)):
             s.insert(BTrees.family32.minint - 1)
         self.check_pickling(BTrees.family32)
 
     def test64(self):
         from zope.interface.verify import verifyObject
+
         import BTrees
         from BTrees.LOBTree import LOTreeSet
         verifyObject(BTrees.Interfaces.IBTreeFamily, BTrees.family64)
         self.assertEqual(
             BTrees.family64.IO, BTrees.LOBTree)
         self.assertEqual(
             BTrees.family64.OI, BTrees.OLBTree)
@@ -499,17 +500,22 @@
         s = LOTreeSet()
         s.insert(BTrees.family64.maxint)
         self.assertTrue(BTrees.family64.maxint in s)
         s = LOTreeSet()
         s.insert(BTrees.family64.minint)
         self.assertTrue(BTrees.family64.minint in s)
         s = LOTreeSet()
+
         # XXX why oh why do we expect ValueError here, but TypeError in test32?
-        self.assertRaises((TypeError, OverflowError), s.insert, BTrees.family64.maxint + 1)
-        self.assertRaises((TypeError, OverflowError), s.insert, BTrees.family64.minint - 1)
+        with self.assertRaises((TypeError, OverflowError)):
+            s.insert(BTrees.family64.maxint + 1)
+
+        with self.assertRaises((TypeError, OverflowError)):
+            s.insert(BTrees.family64.minint - 1)
+
         self.check_pickling(BTrees.family64)
 
     def check_pickling(self, family):
         # The "family" objects are singletons; they can be pickled and
         # unpickled, and the same instances will always be returned on
         # unpickling, whether from the same unpickler or different
         # unpicklers.
```

### Comparing `BTrees-5.2/src/BTrees/tests/testConflict.py` & `BTrees-6.0/src/BTrees/tests/testConflict.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE
 #
 ##############################################################################
 import unittest
 
-from .common import _skip_wo_ZODB
 from .common import ConflictTestBase
+from .common import _skip_wo_ZODB
 
 
 class NastyConfictFunctionalTests(ConflictTestBase, unittest.TestCase):
     # FUNCTESTS: Provoke various conflict scenarios using ZODB + transaction
 
     def _getTargetClass(self):
         from BTrees.OOBTree import OOBTree
@@ -28,32 +28,37 @@
         # The conflict tests tend to open two or more connections
         # and then try to commit them. A standard FileStorage
         # is not MVCC aware, and so each connection would have the same
         # instance of the storage, leading to the error
         # "Duplicate tpc_begin calls for same transaction" on commit;
         # thus we use a MVCCMappingStorage for these tests, ensuring each
         # connection has its own storage.
+        #
         # Unfortunately, it wants to acquire the identically same
-        # non-recursive lock in each of its *its* tpc_* methods, which deadlocks.
+        # non-recursive lock in each of its *its* tpc_* methods, which
+        # deadlocks.
+        #
         # The solution is to give each instance its own lock, and trust in the
-        # serialization (ordering) of the datamanager, and the fact that these tests are
-        # single-threaded.
+        # serialization (ordering) of the datamanager, and the fact that these
+        # tests are single-threaded.
         import threading
-        from ZODB.tests.MVCCMappingStorage  import MVCCMappingStorage
+
+        from ZODB.DB import DB
+        from ZODB.tests.MVCCMappingStorage import MVCCMappingStorage
+
         class _MVCCMappingStorage(MVCCMappingStorage):
             def new_instance(self):
                 inst = MVCCMappingStorage.new_instance(self)
                 inst._commit_lock = threading.Lock()
                 return inst
-        from ZODB.DB import DB
+
         self.storage = _MVCCMappingStorage()
         self.db = DB(self.storage)
         return self.db
 
-
     @_skip_wo_ZODB
     def testSimpleConflict(self):
         # Invoke conflict resolution by committing a transaction and
         # catching a conflict in the storage.
         import transaction
         self.openDB()
 
@@ -63,18 +68,18 @@
 
         r2 = self.db.open().root()
         copy = r2["t"]
         list(copy)    # unghostify
 
         self.assertEqual(t._p_serial, copy._p_serial)
 
-        t.update({1:2, 2:3})
+        t.update({1: 2, 2: 3})
         transaction.commit()
 
-        copy.update({3:4})
+        copy.update({3: 4})
         transaction.commit()
 
     # This tests a problem that cropped up while trying to write
     # testBucketSplitConflict (below):  conflict resolution wasn't
     # working at all in non-trivial cases.  Symptoms varied from
     # strange complaints about pickling (despite that the test isn't
     # doing any *directly*), thru SystemErrors from Python and
@@ -107,18 +112,18 @@
         r2 = self.db.open().root()
         copy = r2["t"]
         # Make sure all of copy is loaded.
         list(copy.values())
 
         self.assertEqual(b._p_serial, copy._p_serial)
 
-        b.update({1:2, 2:3})
+        b.update({1: 2, 2: 3})
         transaction.commit()
 
-        copy.update({3:4})
+        copy.update({3: 4})
         transaction.commit()  # if this doesn't blow up
         list(copy.values())         # and this doesn't either, then fine
 
     @_skip_wo_ZODB
     def testBucketSplitConflict(self):
         # Tests that a bucket split is viewed as a conflict.
         # It's (almost necessarily) a white-box test, and sensitive to
@@ -169,15 +174,15 @@
         # bucket 0 has 15 values: 0, 4 .. 56
         # bucket 1 has 15 values: 60, 61 .. 74
         # bucket 2 has 16 values: [75, 76 .. 81] + [84, 88 ..116]
         # bucket 3 has 20 values: 120, 124 .. 196
         state = b.__getstate__()
         # Looks like:  ((b0, 60, b1, 75, b2, 120, b3), firstbucket)
         # The next block is still verifying preconditions.
-        self.assertEqual(len(state) , 2)
+        self.assertEqual(len(state), 2)
         self.assertEqual(len(state[0]), 7)
         self.assertEqual(state[0][1], 60)
         self.assertEqual(state[0][3], 75)
         self.assertEqual(state[0][5], 120)
 
         tm1.commit()
 
@@ -243,15 +248,15 @@
             del b[k]
         # bucket 0 has 15 values: 0, 4 .. 56
         # bucket 1 has 7 values: 92, 96, 100, 104, 108, 112, 116
         # bucket 2 has 20 values: 120, 124 .. 196
         state = b.__getstate__()
         # Looks like:  ((bucket0, 60, bucket1, 120, bucket2), firstbucket)
         # The next block is still verifying preconditions.
-        self.assertEqual(len(state) , 2)
+        self.assertEqual(len(state), 2)
         self.assertEqual(len(state[0]), 5)
         self.assertEqual(state[0][1], 92)
         self.assertEqual(state[0][3], 120)
 
         tm1.commit()
 
         # In the other transaction, delete the other half of bucket 1.
@@ -547,15 +552,15 @@
         assert t.__getstate__()[0][2].keys()[0] == k
 
         tm2 = transaction.TransactionManager()
         conn2 = db.open(tm2)
 
         t[k+1] = k+1
         del conn2.root.t[k]
-        for i in range(200,300):
+        for i in range(200, 300):
             conn2.root.t[i] = i
 
         tm1.commit()
         self.assertRaises(ConflictError, tm2.commit)
         tm2.abort()
 
         k = t.__getstate__()[0][1]
```

### Comparing `BTrees-5.2/src/BTrees/tests/testPersistency.py` & `BTrees-6.0/src/BTrees/tests/testPersistency.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 # FOR A PARTICULAR PURPOSE
 #
 ##############################################################################
 
 from unittest import TestCase
 
 from ..OOBTree import OOBTree
-from .common import _skip_wo_ZODB, ZODBAccess
+from .common import ZODBAccess
+from .common import _skip_wo_ZODB
 
 
 BUCKET_SIZE = OOBTree.max_leaf_size
 
 
 class TestPersistency(ZODBAccess, TestCase):
     @_skip_wo_ZODB
```

### Comparing `BTrees-5.2/src/BTrees/tests/test_Length.py` & `BTrees-6.0/src/BTrees/tests/test_Length.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 #
 ##############################################################################
 import unittest
 
 
 _marker = object()
 
+
 class TestLength(unittest.TestCase):
 
     def _getTargetClass(self):
         from BTrees.Length import Length
         return Length
 
     def _makeOne(self, value=_marker):
```

### Comparing `BTrees-5.2/src/BTrees/tests/test_OOBTree.py` & `BTrees-6.0/src/BTrees/tests/test_OOBTree.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE
 #
 ##############################################################################
 from BTrees import OOBTree
 
-from .common import BTreeTests
 from ._test_builder import update_module
+from .common import BTreeTests
+
 
 class OOBTreeTest(BTreeTests):
 
     def test_byValue(self):
         ITEMS = [(y, x) for x, y in enumerate('abcdefghijklmnopqrstuvwxyz')]
         tree = self._makeOne(ITEMS)
         self.assertEqual(list(tree.byValue(22)),
@@ -69,37 +70,37 @@
         t[c] = 1
 
         t.clear()
 
     def testAcceptDefaultComparisonOnGet(self):
         # Issue #42
         t = self._makeOne()
+
         class C:
             pass
 
         self.assertEqual(t.get(C(), 42), 42)
         self.assertRaises(KeyError, t.__getitem__, C())
         self.assertFalse(C() in t)
 
-
     def testNewStyleClassWithCustomMetaClassAllowed(self):
         class Meta(type):
             def __lt__(cls, other):
                 return 1
 
         cls = Meta('Class', (object,), {})
         m = self._makeOne()
         m[cls] = self.getTwoValues()[0]
 
     def test_None_is_smallest(self):
         t = self._makeOne()
-        for i in range(999): # Make sure we multiple buckets
+        for i in range(999):  # Make sure we multiple buckets
             t[i] = i*i
         t[None] = -1
-        for i in range(-99, 0): # Make sure we multiple buckets
+        for i in range(-99, 0):  # Make sure we multiple buckets
             t[i] = i*i
         self.assertEqual(list(t), [None] + list(range(-99, 999)))
         self.assertEqual(list(t.values()),
                          [-1] + [i*i for i in range(-99, 999)])
         self.assertEqual(t[2], 4)
         self.assertEqual(t[-2], 4)
         self.assertEqual(t[None], -1)
@@ -107,15 +108,17 @@
         self.assertEqual(t[None], -2)
         t2 = t.__class__(t)
         del t[None]
         self.assertEqual(list(t), list(range(-99, 999)))
 
         if 'Py' in self.__class__.__name__:
             return
-        from BTrees.OOBTree import difference, union, intersection
+        from BTrees.OOBTree import difference
+        from BTrees.OOBTree import intersection
+        from BTrees.OOBTree import union
         self.assertEqual(list(difference(t2, t).items()), [(None, -2)])
         self.assertEqual(list(union(t, t2)), list(t2))
         self.assertEqual(list(intersection(t, t2)), list(t))
 
     def testDeleteNoneKey(self):
         # Check that a None key can be deleted in Python 2.
         # This doesn't work on Python 3 because None is unorderable,
@@ -130,17 +133,22 @@
         del t[None]
 
     def testUnpickleNoneKey(self):
         # All versions (py2 and py3, C and Python) can unpickle
         # data that looks like this: {None: 42}, even though None
         # is unorderable..
         # This pickle was captured in BTree/ZODB3 3.10.7
-        data = b'ccopy_reg\n__newobj__\np0\n(cBTrees.OOBTree\nOOBTree\np1\ntp2\nRp3\n((((NI42\ntp4\ntp5\ntp6\ntp7\nb.'
-
         import pickle
+
+        data = (
+            b'ccopy_reg\n__newobj__\np0\n('
+            b'cBTrees.OOBTree\nOOBTree\np1\ntp2\nRp3\n('
+            b'(((NI42\ntp4\ntp5\ntp6\ntp7\nb.'
+        )
+
         t = pickle.loads(data)
         keys = list(t)
         self.assertEqual([None], keys)
 
     def testIdentityTrumpsBrokenComparison(self):
         # Identical keys always match, even if their comparison is
         # broken. See https://github.com/zopefoundation/BTrees/issues/50
```

### Comparing `BTrees-5.2/src/BTrees/tests/test__base.py` & `BTrees-6.0/src/BTrees/tests/test__base.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,21 +25,25 @@
 class Test_Base(unittest.TestCase):
 
     def _getTargetClass(self):
         from .._base import _Base
         return _Base
 
     def _makeOne(self, items=None):
+
         class _Test(self._getTargetClass()):
             max_leaf_size = 10
             max_internal_size = 15
+
             def clear(self):
                 self._data = {}
+
             def update(self, d):
                 self._data.update(d)
+
         return _Test(items)
 
     def test_ctor_wo_items(self):
         base = self._makeOne()
         self.assertEqual(base._data, {})
 
     def test_ctor_w_items(self):
@@ -61,28 +65,28 @@
         self.assertEqual(bucket._keys, [])
         self.assertEqual(bucket._next, None)
         self.assertEqual(len(bucket), 0)
         self.assertEqual(bucket.size, 0)
 
     def test__deleteNextBucket_none(self):
         bucket = self._makeOne()
-        bucket._deleteNextBucket() # no raise
+        bucket._deleteNextBucket()  # no raise
         self.assertTrue(bucket._next is None)
 
     def test__deleteNextBucket_one(self):
         bucket1 = self._makeOne()
-        bucket2 = bucket1._next = self._makeOne()
-        bucket1._deleteNextBucket() # no raise
+        bucket1._next = self._makeOne()
+        bucket1._deleteNextBucket()  # no raise
         self.assertTrue(bucket1._next is None)
 
     def test__deleteNextBucket_two(self):
         bucket1 = self._makeOne()
         bucket2 = bucket1._next = self._makeOne()
         bucket3 = bucket2._next = self._makeOne()
-        bucket1._deleteNextBucket() # no raise
+        bucket1._deleteNextBucket()  # no raise
         self.assertTrue(bucket1._next is bucket3)
 
     def test__search_empty(self):
         bucket = self._makeOne()
         self.assertEqual(bucket._search('nonesuch'), -1)
 
     def test__search_nonempty_miss(self):
@@ -373,15 +377,15 @@
         bucket = self._makeOne()
         bucket._to_key = lambda x: x
         self.assertFalse('nonesuch' in bucket)
 
     def test___contains___filled_miss(self):
         bucket = self._makeOne()
         bucket._to_key = lambda x: x
-        KEYS = bucket._keys = ['alpha', 'bravo', 'charlie', 'delta', 'echo']
+        bucket._keys = ['alpha', 'bravo', 'charlie', 'delta', 'echo']
         self.assertFalse('nonesuch' in bucket)
 
     def test___contains___filled_hit(self):
         bucket = self._makeOne()
         bucket._to_key = lambda x: x
         KEYS = bucket._keys = ['alpha', 'bravo', 'charlie', 'delta', 'echo']
         for key in KEYS:
@@ -423,18 +427,21 @@
 
     def _getTargetClass(self):
         from .._base import Bucket
         return Bucket
 
     def _makeOne(self):
         from .._datatypes import O
+
         class _Bucket(self._getTargetClass()):
             _to_key = O()
+
             def _to_value(self, x):
                 return x
+
         return _Bucket()
 
     def test_ctor_defaults(self):
         bucket = self._makeOne()
         self.assertEqual(bucket._keys, [])
         self.assertEqual(bucket._values, [])
 
@@ -472,26 +479,30 @@
         bucket = self._makeOne()
         bucket.update({'a': 'b'})
         self.assertEqual(bucket._keys, ['a'])
         self.assertEqual(bucket._values, ['b'])
 
     def test_update_value_w_items(self):
         bucket = self._makeOne()
+
         class Foo:
             def items(self):
                 return [('a', 'b')]
+
         bucket.update(Foo())
         self.assertEqual(bucket._keys, ['a'])
         self.assertEqual(bucket._values, ['b'])
 
     def test_update_value_w_invalid_items(self):
         bucket = self._makeOne()
+
         class Foo:
             def items(self):
                 return ('a', 'b', 'c')
+
         self.assertRaises(TypeError, bucket.update, Foo())
 
     def test_update_sequence(self):
         bucket = self._makeOne()
         bucket.update([('a', 'b')])
         self.assertEqual(bucket._keys, ['a'])
         self.assertEqual(bucket._values, ['b'])
@@ -500,16 +511,18 @@
         bucket = self._makeOne()
         bucket['a'] = 'b'
         bucket.update([('a', 'c')])
         self.assertEqual(bucket['a'], 'c')
 
     def test___setitem___incomparable(self):
         bucket = self._makeOne()
+
         def _should_error():
             bucket[object()] = 'b'
+
         self.assertRaises(TypeError, _should_error)
 
     def test___setitem___comparable(self):
         bucket = self._makeOne()
         bucket['a'] = 'b'
         self.assertEqual(bucket['a'], 'b')
 
@@ -517,16 +530,18 @@
         bucket = self._makeOne()
         bucket['a'] = 'b'
         bucket['a'] = 'c'
         self.assertEqual(bucket['a'], 'c')
 
     def test___delitem___miss(self):
         bucket = self._makeOne()
+
         def _should_error():
             del bucket['nonesuch']
+
         self.assertRaises(KeyError, _should_error)
 
     def test___delitem___hit(self):
         bucket = self._makeOne()
         bucket._keys.append('a')
         bucket._values.append('b')
         del bucket['a']
@@ -559,16 +574,18 @@
         bucket = self._makeOne()
         bucket._keys.append('a')
         bucket._values.append('b')
         self.assertEqual(bucket.get('a'), 'b')
 
     def test___getitem___miss(self):
         bucket = self._makeOne()
+
         def _should_error():
             return bucket['nonesuch']
+
         self.assertRaises(KeyError, _should_error)
 
     def test___getitem___hit(self):
         bucket = self._makeOne()
         bucket._keys.append('a')
         bucket._values.append('b')
         self.assertEqual(bucket['a'], 'b')
@@ -614,23 +631,27 @@
         bucket = self._makeOne()
         self.assertEqual(bucket.keys(), [])
 
     def test_keys_filled_no_args(self):
         bucket = self._makeOne()
         for i, c in enumerate('abcdef'):
             bucket[c] = i
-        self.assertEqual(bucket.keys(),
-                         ['a', 'b', 'c', 'd', 'e', 'f'])
+        self.assertEqual(
+            bucket.keys(),
+            ['a', 'b', 'c', 'd', 'e', 'f'],
+        )
 
     def test_keys_filled_w_args(self):
         bucket = self._makeOne()
         for i, c in enumerate('abcdef'):
             bucket[c] = i
-        self.assertEqual(bucket.keys(min='b', excludemin=True,
-                                     max='f', excludemax=True), ['c', 'd', 'e'])
+        self.assertEqual(
+            bucket.keys(min='b', excludemin=True, max='f', excludemax=True),
+            ['c', 'd', 'e'],
+        )
 
     def test_iterkeys_empty_no_args(self):
         bucket = self._makeOne()
         self.assertEqual(list(bucket.iterkeys()), [])
 
     def test_iterkeys_filled_no_args(self):
         bucket = self._makeOne()
@@ -696,17 +717,18 @@
 
     def test_items_filled_w_args(self):
         bucket = self._makeOne()
         EXPECTED = []
         for i, c in enumerate('abcdef'):
             bucket[c] = i
             EXPECTED.append((c, i))
-        self.assertEqual(bucket.items(min='b', excludemin=True,
-                                       max='f', excludemax=True),
-                        EXPECTED[2:5])
+        self.assertEqual(
+            bucket.items(min='b', excludemin=True, max='f', excludemax=True),
+            EXPECTED[2:5],
+        )
 
     def test_iteritems_empty_no_args(self):
         bucket = self._makeOne()
         self.assertEqual(list(bucket.iteritems()), [])
 
     def test_iteritems_filled_no_args(self):
         bucket = self._makeOne()
@@ -718,17 +740,22 @@
 
     def test_iteritems_filled_w_args(self):
         bucket = self._makeOne()
         EXPECTED = []
         for i, c in enumerate('abcdef'):
             bucket[c] = i
             EXPECTED.append((c, i))
-        self.assertEqual(list(bucket.iteritems(min='b', excludemin=True,
-                                               max='f', excludemax=True)),
-                        EXPECTED[2:5])
+        self.assertEqual(
+            list(
+                bucket.iteritems(
+                    min='b', excludemin=True, max='f', excludemax=True,
+                )
+            ),
+            EXPECTED[2:5]
+        )
 
     def test___getstate___empty_no_next(self):
         bucket = self._makeOne()
         self.assertEqual(bucket.__getstate__(), ((),))
 
     def test___getstate___empty_w_next(self):
         bucket = self._makeOne()
@@ -754,15 +781,15 @@
 
     def test___setstate___w_non_tuple(self):
         bucket = self._makeOne()
         self.assertRaises(TypeError, bucket.__setstate__, (None,))
 
     def test___setstate___w_empty_no_next(self):
         bucket = self._makeOne()
-        bucket._next = next_b = self._makeOne()
+        bucket._next = self._makeOne()
         for i, c in enumerate('abcdef'):
             bucket[c] = i
         bucket.__setstate__(((),))
         self.assertEqual(len(bucket.keys()), 0)
         self.assertTrue(bucket._next is None)
 
     def test___setstate___w_non_empty_w_next(self):
@@ -1061,17 +1088,19 @@
     assertRaises = _assertRaises
 
     def _getTargetClass(self):
         from .._base import Set
         return Set
 
     def _makeOne(self):
+
         class _Set(self._getTargetClass()):
             def _to_key(self, x):
                 return x
+
         return _Set()
 
     def test_add_not_extant(self):
         _set = self._makeOne()
         _set.add('not_extant')
         self.assertEqual(list(_set), ['not_extant'])
 
@@ -1130,15 +1159,15 @@
 
     def test___setstate___w_non_tuple(self):
         _set = self._makeOne()
         self.assertRaises(TypeError, _set.__setstate__, (None,))
 
     def test___setstate___w_empty_no_next(self):
         _set = self._makeOne()
-        _set._next = next_s = self._makeOne()
+        _set._next = self._makeOne()
         for c in 'abcdef':
             _set.add(c)
         _set.__setstate__(((),))
         self.assertEqual(len(_set), 0)
         self.assertTrue(_set._next is None)
 
     def test___setstate___w_non_empty_w_next(self):
@@ -1260,15 +1289,15 @@
         e = self.assertRaises(BTreesConflictError,
                               _set._p_resolveConflict, s_old, s_com, s_new)
         self.assertEqual(e.reason, 12)
 
     def test__p_resolveConflict_x_on_del_first_com(self):
         from ..Interfaces import BTreesConflictError
         _set = self._makeOne()
-        s_old = (('a','b'), None)
+        s_old = (('a', 'b'), None)
         s_com = (('b',), None)
         s_new = (('a', 'b', 'c'), None)
         e = self.assertRaises(BTreesConflictError,
                               _set._p_resolveConflict, s_old, s_com, s_new)
         self.assertEqual(e.reason, 13)
 
     def test__p_resolveConflict_x_on_del_first_new(self):
@@ -1461,28 +1490,30 @@
 
     def _getTargetClass(self):
         from .._base import _Tree
         return _Tree
 
     def _makeOne(self, items=None, bucket_type=None):
         from .._base import Bucket
-        from .._datatypes import O
         from .._datatypes import Any
+        from .._datatypes import O
         if bucket_type is None:
+
             class _Bucket(Bucket):
                 _to_key = O()
 
             bucket_type = _Bucket
 
         class _Test(self._getTargetClass()):
             _to_key = O()
             _to_value = Any()
             _bucket_type = bucket_type
             max_leaf_size = 10
             max_internal_size = 15
+
         return _Test(items)
 
     def test_setdefault_miss(self):
         tree = self._makeOne()
         value = object()
         self.assertTrue(tree.setdefault('non_extant', value) is value)
         self.assertTrue('non_extant' in tree)
@@ -1516,25 +1547,29 @@
     def test_update_value_w_iteritems(self):
         tree = self._makeOne()
         tree.update({'a': 'b'})
         self.assertEqual(tree._findbucket('a')['a'], 'b')
 
     def test_update_value_w_items(self):
         tree = self._makeOne()
+
         class Foo:
             def items(self):
                 return [('a', 'b')]
+
         tree.update(Foo())
         self.assertEqual(tree._findbucket('a')['a'], 'b')
 
     def test_update_value_w_invalid_items(self):
         tree = self._makeOne()
+
         class Foo:
             def items(self):
                 return ('a', 'b', 'c')
+
         self.assertRaises(TypeError, tree.update, Foo())
 
     def test_update_sequence(self):
         tree = self._makeOne()
         tree.update([('a', 'b')])
         self.assertEqual(tree._findbucket('a')['a'], 'b')
 
@@ -1542,22 +1577,26 @@
         tree = self._makeOne()
         tree['a'] = 'b'
         tree.update([('a', 'c')])
         self.assertEqual(tree._findbucket('a')['a'], 'c')
 
     def test___setitem___incomparable(self):
         tree = self._makeOne()
+
         def _should_error():
             tree[object()] = 'b'
+
         self.assertRaises(TypeError, _should_error)
 
     def test___delitem___miss(self):
         tree = self._makeOne()
+
         def _should_error():
             del tree['a']
+
         self.assertRaises(KeyError, _should_error)
 
     def test___delitem___hit(self):
         tree = self._makeOne()
         tree['a'] = 'b'
         del tree['a']
         self.assertFalse('a' in tree)
@@ -1588,16 +1627,14 @@
         self.assertEqual(len(tree), 1)
 
     def test___len__nonempty_multiple_buckets(self):
         tree = self._makeOne()
         for i in range(100):
             tree[str(i)] = i
         self.assertEqual(len(tree), 100)
-        b_count = 0
-        bucket = tree._firstbucket
 
     def test_size_empty(self):
         tree = self._makeOne()
         self.assertEqual(tree.size, 0)
 
     def test_size_nonempty(self):
         tree = self._makeOne()
@@ -1867,41 +1904,38 @@
 
     def test__split_empty(self):
         tree = self._makeOne()
         self.assertRaises(IndexError, tree._split)
 
     def test__split_filled_empties_original(self):
         tree = self._makeOne()
-        next_t = tree._next = self._makeOne()
         for i, c in enumerate('abcdef'):
             tree[c] = i
         fb = tree._firstbucket
         new_t = tree._split()
         self.assertEqual(list(tree), [])
         self.assertTrue(tree._firstbucket is None)
         self.assertEqual(list(new_t), ['a', 'b', 'c', 'd', 'e', 'f'])
         self.assertTrue(new_t._firstbucket is fb)
 
     def test__split_filled_divides_original(self):
         tree = self._makeOne()
-        next_t = tree._next = self._makeOne()
         LETTERS = 'abcdefghijklmnopqrstuvwxyz'
         for i, c in enumerate(LETTERS):
             tree[c] = i
         fb = tree._firstbucket
         new_t = tree._split()
         # Note that original tree still links to split buckets
         self.assertEqual(''.join(list(tree)), LETTERS)
         self.assertTrue(tree._firstbucket is fb)
         self.assertEqual(''.join(list(new_t)), LETTERS[10:])
         self.assertFalse(new_t._firstbucket is fb)
 
     def test__split_filled_divides_deeper(self):
         tree = self._makeOne()
-        next_t = tree._next = self._makeOne()
         KEYS = []
         FMT = '%05d'
         for i in range(1000):
             key = FMT % i
             tree[key] = i
             KEYS.append(key)
         fb = tree._firstbucket
@@ -1934,34 +1968,34 @@
         self.assertTrue(after > before)
 
     def test__del_empties_first_bucket_not_zeroth_item(self):
         SOURCE = {'%05d' % i: i for i in range(1000)}
         tree = self._makeOne(SOURCE)
         bucket = tree._data[1].child._firstbucket
         next_b = bucket._next
-        for key in list(bucket): # don't del while iterting
+        for key in list(bucket):  # don't del while iterting
             del tree[key]
         self.assertTrue(tree._data[1].child._firstbucket is next_b)
 
     def test__del_empties_first_bucket_zeroth_item(self):
         SOURCE = {'%05d' % i: i for i in range(1000)}
         tree = self._makeOne(SOURCE)
         bucket = tree._data[0].child._firstbucket
         next_b = bucket._next
-        for key in list(bucket): # don't del while iterting
+        for key in list(bucket):  # don't del while iterting
             del tree[key]
         self.assertTrue(tree._data[0].child._firstbucket is next_b)
         self.assertTrue(tree._firstbucket is next_b)
 
     def test__del_empties_other_bucket_not_zeroth_item(self):
         SOURCE = {'%05d' % i: i for i in range(1000)}
         tree = self._makeOne(SOURCE)
         bucket = tree._data[1].child._firstbucket._next
         next_b = bucket._next
-        for key in list(bucket): # don't del while iterting
+        for key in list(bucket):  # don't del while iterting
             del tree[key]
         self.assertTrue(tree._data[1].child._firstbucket._next is next_b)
 
     def test___getstate___empty(self):
         tree = self._makeOne()
         self.assertEqual(tree.__getstate__(), None)
 
@@ -2005,17 +2039,20 @@
         self.assertEqual(tree._findbucket('a')['a'], 'b')
         self.assertTrue(len(tree._data), 1)
         self.assertTrue(tree._data[0].child is tree._firstbucket)
         self.assertTrue(tree._firstbucket._p_oid is None)
 
     def test___setstate___to_multiple_buckets(self):
         from .._base import Bucket
+
         class _Bucket(Bucket):
+
             def _to_key(self, x):
                 return x
+
         tree = self._makeOne(bucket_type=_Bucket)
         b1 = _Bucket({'a': 0, 'b': 1})
         b2 = _Bucket({'c': 2, 'd': 3})
         b1._next = b2
         tree.__setstate__(((b1, 'c', b2), b1))
         self.assertEqual(list(tree.keys()), ['a', 'b', 'c', 'd'])
         self.assertTrue(len(tree._data), 2)
@@ -2023,15 +2060,15 @@
         self.assertEqual(tree._data[0].child, b1)
         self.assertEqual(tree._data[1].key, 'c')
         self.assertEqual(tree._data[1].child, b2)
         self.assertTrue(tree._firstbucket is b1)
 
     def test__check_empty_wo_firstbucket(self):
         tree = self._makeOne()
-        tree._check() # no raise
+        tree._check()  # no raise
 
     def test__check_empty_w_firstbucket(self):
         tree = self._makeOne()
         tree._firstbucket = object()
         e = self.assertRaises(AssertionError, tree._check)
         self.assertEqual(str(e), "Empty BTree has non-NULL firstbucket")
 
@@ -2044,16 +2081,18 @@
     def test__check_nonempty_w_null_child(self):
         tree = self._makeOne({'a': 'b'})
         tree._data.append(tree._data[0].__class__('c', None))
         e = self.assertRaises(AssertionError, tree._check)
         self.assertEqual(str(e), "BTree has NULL child")
 
     def test__check_nonempty_w_heterogenous_child(self):
+
         class Other:
             pass
+
         tree = self._makeOne({'a': 'b'})
         tree._data.append(tree._data[0].__class__('c', Other()))
         e = self.assertRaises(AssertionError, tree._check)
         self.assertEqual(str(e), "BTree children have different types")
 
     def test__check_nonempty_w_empty_child(self):
         tree = self._makeOne({'a': 'b'})
@@ -2069,16 +2108,18 @@
         tree._data.append(c_first.__class__('a', c_tree))
         tree._firstbucket = object()
         e = self.assertRaises(AssertionError, tree._check)
         self.assertEqual(str(e), "BTree has firstbucket different than "
                                  "its first child's firstbucket")
 
     def test__check_nonempty_w_invalid_child(self):
+
         class Invalid:
             size = 2
+
         tree = self._makeOne({'a': 'b'})
         tree._data[0].child = Invalid()
         e = self.assertRaises(AssertionError, tree._check)
         self.assertEqual(str(e), "Incorrect child type")
 
     def test__check_branch_traverse_bucket_pointers(self):
         tree = self._makeOne()
@@ -2086,22 +2127,22 @@
         c_first = t_first._data[0]
         b_first = c_first.child
         t_second = tree.__class__({'c': 'd'})
         b_first._next = t_second._firstbucket
         tree._data.append(c_first.__class__('a', t_first))
         tree._data.append(c_first.__class__('c', t_second))
         tree._firstbucket = t_first._firstbucket
-        tree._check() #no raise
+        tree._check()  # no raise
 
     def test__check_nonempty_leaf_traverse_bucket_pointers(self):
         tree = self._makeOne({'a': 'b'})
         first = tree._data[0]
         first.child._next = b2 = first.child.__class__({'c': 'd'})
         tree._data.append(first.__class__('c', b2))
-        tree._check() #no raise
+        tree._check()  # no raise
 
     def test__p_resolveConflict_invalid_state_non_tuple(self):
         tree = self._makeOne()
         INVALID = []
         EMPTY = None
         DEGEN = (((('a', 'b'),),),)
         self.assertRaises(TypeError, tree._p_resolveConflict,
@@ -2206,39 +2247,46 @@
         return _TreeItems
 
     def _makeOne(self, firstbucket, itertype, iterargs):
         return self._getTargetClass()(firstbucket, itertype, iterargs)
 
     def _makeBucket(self, items=None):
         from .._base import Bucket
+
         class _Bucket(Bucket):
+
             def _to_key(self, k):
                 return k
+
         return _Bucket(items)
 
     def test___getitem___w_slice(self):
         ITEMS = [(y, x) for x, y in enumerate('abcdefghijklmnopqrstuvwxyz')]
         bucket = self._makeBucket(ITEMS)
         ti = self._makeOne(bucket, 'iterkeys', ())
         self.assertEqual(list(ti[0:3]), ['a', 'b', 'c'])
 
     def test___getitem___w_negative_index_le_minus_length(self):
         ITEMS = [(y, x) for x, y in enumerate('abcdefghijklmnopqrstuvwxyz')]
         bucket = self._makeBucket(ITEMS)
         ti = self._makeOne(bucket, 'iterkeys', ())
+
         def _should_error():
             return ti[-27]
+
         self.assertRaises(IndexError, _should_error)
 
     def test___getitem___w_index_gt_length(self):
         ITEMS = [(y, x) for x, y in enumerate('abcdefghijklmnopqrstuvwxyz')]
         bucket = self._makeBucket(ITEMS)
         ti = self._makeOne(bucket, 'iterkeys', ())
+
         def _should_error():
             return ti[27]
+
         self.assertRaises(IndexError, _should_error)
 
     def test___getitem___w_index_smaller_than_cursor(self):
         ITEMS = [(y, x) for x, y in enumerate('abcdefghijklmnopqrstuvwxyz')]
         bucket = self._makeBucket(ITEMS)
         ti = self._makeOne(bucket, 'iterkeys', ())
         ti[12]
@@ -2269,37 +2317,40 @@
         bucket = self._makeBucket(ITEMS)
         ti = self._makeOne(bucket, 'itervalues', ())
         self.assertEqual(list(ti), [x[1] for x in ITEMS])
 
     def test___iter___w_empty_last_bucket(self):
         ITEMS = [(y, x) for x, y in enumerate('abcdefghijklmnopqrstuvwxyz')]
         bucket1 = self._makeBucket(ITEMS)
-        bucket2 = bucket1._next = self._makeBucket()
         ti = self._makeOne(bucket1, 'iterkeys', ())
         self.assertEqual(list(ti), [x[0] for x in ITEMS])
 
 
 class TreeTests(unittest.TestCase):
 
     assertRaises = _assertRaises
 
     def _getTargetClass(self):
         from .._base import Tree
         return Tree
 
     def _makeOne(self, items=None):
         from .._base import Bucket
+
         class _Bucket(Bucket):
+
             def _to_key(self, k):
                 return k
+
         class _Test(self._getTargetClass()):
             _to_key = _to_value = lambda self, x: x
             _bucket_type = _Bucket
             max_leaf_size = 10
             max_internal_size = 15
+
         return _Test(items)
 
     def test_get_empty_miss(self):
         tree = self._makeOne()
         self.assertEqual(tree.get('nonesuch'), None)
 
     def test_get_empty_miss_w_default(self):
@@ -2321,23 +2372,27 @@
     def test_get_filled_hit(self):
         ITEMS = [(y, x) for x, y in enumerate('abcdefghijklmnopqrstuvwxyz')]
         tree = self._makeOne(ITEMS)
         self.assertEqual(tree.get('a'), 0)
 
     def test___getitem___empty_miss(self):
         tree = self._makeOne()
+
         def _should_error():
             return tree['nonesuch']
+
         self.assertRaises(KeyError, _should_error)
 
     def test___getitem___filled_miss(self):
         ITEMS = [(y, x) for x, y in enumerate('abcdefghijklmnopqrstuvwxyz')]
         tree = self._makeOne(ITEMS)
+
         def _should_error():
             return tree['nonesuch']
+
         self.assertRaises(KeyError, _should_error)
 
     def test___getitem___filled_hit(self):
         ITEMS = [(y, x) for x, y in enumerate('abcdefghijklmnopqrstuvwxyz')]
         tree = self._makeOne(ITEMS)
         self.assertEqual(tree['a'], 0)
 
@@ -2365,33 +2420,42 @@
         ITEMS = [(y, x) for x, y in enumerate('abcdefghijklmnopqrstuvwxyz')]
         tree = self._makeOne(ITEMS)
         self.assertEqual(list(tree.itervalues()), list(range(26)))
 
     def test_itervalues_filled_w_args(self):
         ITEMS = [(y, x) for x, y in enumerate('abcdefghijklmnopqrstuvwxyz')]
         tree = self._makeOne(ITEMS)
-        self.assertEqual(list(tree.itervalues(min='b', excludemin=True,
-                                             max='f', excludemax=True)),
-                         [2, 3, 4])
+        self.assertEqual(
+            list(
+                tree.itervalues(
+                    min='b', excludemin=True, max='f', excludemax=True,
+                )
+            ),
+            [2, 3, 4],
+        )
 
     def test_items_empty_no_args(self):
         tree = self._makeOne()
         self.assertEqual(list(tree.items()), [])
 
     def test_items_filled_no_args(self):
         ITEMS = [(y, x) for x, y in enumerate('abcdefghijklmnopqrstuvwxyz')]
         tree = self._makeOne(ITEMS)
         self.assertEqual(list(tree.items()), ITEMS)
 
     def test_items_filled_w_args(self):
         ITEMS = [(y, x) for x, y in enumerate('abcdefghijklmnopqrstuvwxyz')]
         tree = self._makeOne(ITEMS)
-        self.assertEqual(list(tree.items(min='b', excludemin=True,
-                                          max='f', excludemax=True)),
-                         ITEMS[2:5])
+        self.assertEqual(
+            list(
+                tree.items(
+                    min='b', excludemin=True, max='f', excludemax=True,
+                )
+            ), ITEMS[2:5]
+        )
 
     def test_iteritems_empty_no_args(self):
         tree = self._makeOne()
         self.assertEqual(list(tree.iteritems()), [])
 
     def test_iteritems_filled_no_args(self):
         ITEMS = [(y, x) for x, y in enumerate('abcdefghijklmnopqrstuvwxyz')]
@@ -2429,22 +2493,25 @@
 
     def _getTargetClass(self):
         from .._base import TreeSet
         return TreeSet
 
     def _makeOne(self, items=None):
         from .._base import Bucket
+
         class _Bucket(Bucket):
             def _to_key(self, k):
                 return k
+
         class _Test(self._getTargetClass()):
             _to_key = _to_value = lambda self, x: x
             _bucket_type = _Bucket
             max_leaf_size = 10
             max_internal_size = 15
+
         return _Test(items)
 
     def test_add_new_key(self):
         _set = self._makeOne()
         self.assertTrue(_set.add('a'))
         self.assertTrue('a' in _set)
 
@@ -2494,31 +2561,35 @@
         from .._base import set_operation
         return set_operation
 
     def _makeOne(self, func, set_type):
         return self._getTargetClass()(func, set_type)
 
     def test_it(self):
+
         class _SetType:
             pass
+
         _called_with = []
+
         def _func(*args, **kw):
             _called_with.append((args, kw))
+
         set_op = self._makeOne(_func, _SetType)
         set_op('a', b=1)
         self.assertEqual(_called_with, [((_SetType, 'a',), {'b': 1})])
 
 
 class _SetObBase:
 
     def _makeSet(self, *args):
-        return  _Set(*args)
+        return _Set(*args)
 
     def _makeMapping(self, *args, **kw):
-        return  _Mapping(*args, **kw)
+        return _Mapping(*args, **kw)
 
 
 class Test_difference(unittest.TestCase, _SetObBase):
 
     def _callFUT(self, *args, **kw):
         from .._base import difference
         return difference(*args, **kw)
@@ -2706,30 +2777,38 @@
         lhs.MERGE = lambda v1, w1, v2, w2: (v1 * w1) + (v2 * w2)
         lhs.MERGE_WEIGHT = lambda v, w: v
         lhs._mapping_type = _Mapping
         rhs = self._makeSet('a', 'b', 'c')
         self.assertRaises(TypeError, self._callFUT, lhs.__class__, lhs, rhs)
 
     def test_lhs_mapping_wo_MERGE_DEFAULT_rhs_set(self):
+
         class _MappingWoDefault(dict):
+
             def MERGE(self, v1, w1, v2, w2):
                 return (v1 * w1) + (v2 * w2)
+
             def MERGE_WEIGHT(self, v, w):
                 return v
+
         lhs = _MappingWoDefault({'a': 13, 'b': 12, 'c': 11})
         lhs._mapping_type = _MappingWoDefault
         rhs = self._makeSet('a', 'b', 'c')
         self.assertRaises(TypeError, self._callFUT, lhs.__class__, lhs, rhs)
 
     def test_lhs_mapping_wo_MERGE_rhs_mapping(self):
+
         class _MappingWoMerge(dict):
+
             def MERGE_DEFAULT(self):
                 return 1
+
             def MERGE_WEIGHT(self, v, w):
                 return v
+
         lhs = _MappingWoMerge({'a': 13, 'b': 12, 'c': 11})
         lhs._mapping_type = _MappingWoMerge
         rhs = self._makeMapping({'a': 1, 'b': 2, 'c': 3})
         self.assertRaises(TypeError, self._callFUT, lhs.__class__, lhs, rhs)
 
     def test_lhs_set_wo_MERGE_DEFAULT_rhs_mapping(self):
         lhs = self._makeSet('a', 'd')
@@ -2793,15 +2872,15 @@
         from BTrees.IIBTree import IISetPy
         lhs = IISetPy([1, 2, 3])
         rhs = IISetPy([1, 4])
         weight, result = self._callFUT(lhs.__class__, lhs, rhs)
         self.assertEqual(weight, 1)
         self.assertEqual(list(result), [1, 2, 3, 4])
 
-    #TODO:  test non-default weights
+    # TODO:  test non-default weights
 
 
 class Test_weightedIntersection(unittest.TestCase, _SetObBase):
 
     def _callFUT(self, *args, **kw):
         from .._base import weightedIntersection
         return weightedIntersection(*args, **kw)
@@ -2819,19 +2898,23 @@
 
     def test_both_mappings_but_no_merge(self):
         lhs = {'a': 13, 'b': 12, 'c': 11}
         rhs = {'b': 22, 'd': 14}
         self.assertRaises(TypeError, self._callFUT, lhs.__class__, lhs, rhs)
 
     def test_lhs_mapping_wo_MERGE_rhs_mapping(self):
+
         class _MappingWoMerge(dict):
+
             def MERGE_DEFAULT(self):
                 return 1
+
             def MERGE_WEIGHT(self, v, w):
                 return v
+
         lhs = _MappingWoMerge({'a': 13, 'b': 12, 'c': 11})
         lhs._mapping_type = _MappingWoMerge
         rhs = self._makeMapping({'a': 1, 'b': 2, 'c': 3})
         self.assertRaises(TypeError, self._callFUT, lhs.__class__, lhs, rhs)
 
     def test_lhs_set_wo_MERGE_DEFAULT_rhs_set(self):
         lhs = self._makeSet('a', 'd')
@@ -2877,15 +2960,15 @@
         from BTrees.IIBTree import IISetPy
         lhs = IISetPy([1, 2, 3])
         rhs = IISetPy([1, 4])
         weight, result = self._callFUT(lhs.__class__, lhs, rhs)
         self.assertEqual(weight, 2)
         self.assertEqual(list(result), [1])
 
-    #TODO:  test non-default weights
+    # TODO:  test non-default weights
 
 
 class Test_multiunion(unittest.TestCase, _SetObBase):
 
     def _callFUT(self, *args, **kw):
         from .._base import multiunion
         return multiunion(*args, **kw)
@@ -2925,64 +3008,86 @@
         from BTrees._base import MERGE_WEIGHT_numeric
         faux_self = object()
         self.assertEqual(MERGE_WEIGHT_numeric(faux_self, 1, 17), 17)
         self.assertEqual(MERGE_WEIGHT_numeric(faux_self, 7, 1), 7)
 
 
 class _Cache:
+
     def __init__(self):
         self._mru = []
+
     def mru(self, oid):
         self._mru.append(oid)
 
 
 class _Jar:
+
     def __init__(self):
         self._current = set()
         self._cache = _Cache()
+
     def readCurrent(self, obj):
         self._current.add(obj)
+
     def register(self, obj):
         pass
 
 
 class _Set:
+
     def __init__(self, *args, **kw):
         if len(args) == 1 and isinstance(args[0], tuple):
             keys = args[0]
         else:
             keys = set(args)
         self._keys = sorted(keys)
+
     def keys(self):
         return self._keys
+
     def __iter__(self):
         return iter(self._keys)
+
     def update(self, items):
         self._keys = sorted(self._keys + list(items))
+
+
 _Set._set_type = _Set
 
 
 class _Mapping(dict):
+
     def __init__(self, source=None):
         if source is None:
             source = {}
         self._keys = []
         self._values = []
         for k, v in sorted(source.items()):
             self._keys.append(k)
             self._values.append(v)
+
     MERGE_DEFAULT = 42
+
     def MERGE_WEIGHT(self, v, w):
         return v
+
     def MERGE(self, v1, w1, v2, w2):
         return v1 * w1 + v2 * w2
+
     def iteritems(self):
         yield from zip(self._keys, self._values)
+
     def __iter__(self):
         return iter(self._keys)
+
     def __getitem__(self, key):
         search = dict(zip(self._keys, self._values))
         return search[key]
+
     def __repr__(self):
         return repr(dict(zip(self._keys, self._values)))
+
+
 _Mapping._set_type = _Set
+
 _Mapping._mapping_type = _Mapping
```

### Comparing `BTrees-5.2/src/BTrees/tests/test__datatypes.py` & `BTrees-6.0/src/BTrees/tests/test__datatypes.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,37 +9,34 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 
 import unittest
+
 from BTrees import _datatypes
 
+
 to_ob = _datatypes.Any()
 to_int = _datatypes.I()
 to_float = _datatypes.F()
 to_long = _datatypes.L()
 to_2_bytes = _datatypes.f()
 to_6_bytes = _datatypes.s()
 
+
 class TestDatatypes(unittest.TestCase):
     def test_to_ob(self):
         for thing in "abc", 0, 1.3, (), frozenset((1, 2)), object():
             self.assertTrue(to_ob(thing) is thing)
 
     def test_to_int_w_int(self):
         self.assertEqual(to_int(3), 3)
 
-    def test_to_int_w_long_in_range(self):
-        try:
-            self.assertEqual(to_int(long(3)), 3)
-        except NameError: #Python3
-            pass
-
     def test_to_int_w_overflow(self):
         self.assertRaises(TypeError, to_int, 2**64)
 
     def test_to_int_w_invalid(self):
         self.assertRaises(TypeError, to_int, ())
 
     def test_to_float_w_float(self):
@@ -50,20 +47,14 @@
 
     def test_to_float_w_invalid(self):
         self.assertRaises(TypeError, to_float, ())
 
     def test_to_long_w_int(self):
         self.assertEqual(to_long(3), 3)
 
-    def test_to_long_w_long_in_range(self):
-        try:
-            self.assertEqual(to_long(long(3)), 3)
-        except NameError: #Python3
-            pass
-
     def test_to_long_w_overflow(self):
         self.assertRaises(TypeError, to_long, 2**64)
 
     def test_to_long_w_invalid(self):
         self.assertRaises(TypeError, to_long, ())
 
     def test_to_2_bytes_w_ok(self):
```

### Comparing `BTrees-5.2/src/BTrees/tests/test_btreesubclass.py` & `BTrees-6.0/src/BTrees/tests/test_btreesubclass.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,24 +9,28 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 import unittest
 
-from BTrees.OOBTree import OOBTree, OOBucket
+from BTrees.OOBTree import OOBTree
+from BTrees.OOBTree import OOBucket
+
 
 class B(OOBucket):
     pass
 
+
 class T(OOBTree):
     _bucket_type = B
     max_leaf_size = 2
     max_internal_size = 3
 
+
 class S(T):
     pass
 
 
 class SubclassTest(unittest.TestCase):
 
     def testSubclass(self):
```

### Comparing `BTrees-5.2/src/BTrees/tests/test_check.py` & `BTrees-6.0/src/BTrees/tests/test_check.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,130 +30,146 @@
 
     def test_classify_w_unknown(self):
         class NotClassified:
             pass
         self.assertRaises(KeyError, self._callFUT, NotClassified())
 
     def test_classify_w_bucket(self):
-        from BTrees.OOBTree import OOBucketPy
         from BTrees.check import TYPE_BUCKET
+        from BTrees.OOBTree import OOBucketPy
         kind, is_mapping = self._callFUT(OOBucketPy())
         self.assertEqual(kind, TYPE_BUCKET)
         self.assertTrue(is_mapping)
 
     def test_classify_w_set(self):
-        from BTrees.OOBTree import OOSetPy
         from BTrees.check import TYPE_BUCKET
+        from BTrees.OOBTree import OOSetPy
         kind, is_mapping = self._callFUT(OOSetPy())
         self.assertEqual(kind, TYPE_BUCKET)
         self.assertFalse(is_mapping)
 
     def test_classify_w_tree(self):
-        from BTrees.OOBTree import OOBTreePy
         from BTrees.check import TYPE_BTREE
+        from BTrees.OOBTree import OOBTreePy
         kind, is_mapping = self._callFUT(OOBTreePy())
         self.assertEqual(kind, TYPE_BTREE)
         self.assertTrue(is_mapping)
 
     def test_classify_w_treeset(self):
-        from BTrees.OOBTree import OOTreeSetPy
         from BTrees.check import TYPE_BTREE
+        from BTrees.OOBTree import OOTreeSetPy
         kind, is_mapping = self._callFUT(OOTreeSetPy())
         self.assertEqual(kind, TYPE_BTREE)
         self.assertFalse(is_mapping)
 
 
 class Test_crack_btree(unittest.TestCase):
 
     def _callFUT(self, obj, is_mapping):
         from BTrees.check import crack_btree
         return crack_btree(obj, is_mapping)
 
     def test_w_empty_tree(self):
         from BTrees.check import BTREE_EMPTY
+
         class Empty:
             def __getstate__(self):
                 return None
+
         kind, keys, kids = self._callFUT(Empty(), True)
         self.assertEqual(kind, BTREE_EMPTY)
         self.assertEqual(keys, [])
         self.assertEqual(kids, [])
 
     def test_w_degenerate_tree(self):
         from BTrees.check import BTREE_ONE
+
         class Degenerate:
             def __getstate__(self):
                 return ((('a', 1, 'b', 2),),)
+
         kind, keys, kids = self._callFUT(Degenerate(), True)
         self.assertEqual(kind, BTREE_ONE)
         self.assertEqual(keys, ('a', 1, 'b', 2))
         self.assertEqual(kids, None)
 
     def test_w_normal_tree(self):
         from BTrees.check import BTREE_NORMAL
         first_bucket = [object()] * 8
         second_bucket = [object()] * 8
+
         class Normal:
             def __getstate__(self):
                 return ((first_bucket, 'b', second_bucket), first_bucket)
+
         kind, keys, kids = self._callFUT(Normal(), True)
         self.assertEqual(kind, BTREE_NORMAL)
         self.assertEqual(keys, ['b'])
         self.assertEqual(kids, [first_bucket, second_bucket])
 
 
 class Test_crack_bucket(unittest.TestCase):
 
     def _callFUT(self, obj, is_mapping):
         from BTrees.check import crack_bucket
         return crack_bucket(obj, is_mapping)
 
     def test_w_empty_set(self):
+
         class EmptySet:
             def __getstate__(self):
                 return ([],)
+
         keys, values = self._callFUT(EmptySet(), False)
         self.assertEqual(keys, [])
         self.assertEqual(values, [])
 
     def test_w_non_empty_set(self):
+
         class NonEmptySet:
             def __getstate__(self):
                 return (['a', 'b', 'c'],)
+
         keys, values = self._callFUT(NonEmptySet(), False)
         self.assertEqual(keys, ['a', 'b', 'c'])
         self.assertEqual(values, [])
 
     def test_w_empty_mapping(self):
+
         class EmptyMapping:
             def __getstate__(self):
                 return ([], object())
+
         keys, values = self._callFUT(EmptyMapping(), True)
         self.assertEqual(keys, [])
         self.assertEqual(values, [])
 
     def test_w_non_empty_mapping(self):
+
         class NonEmptyMapping:
             def __getstate__(self):
                 return (['a', 1, 'b', 2, 'c', 3], object())
+
         keys, values = self._callFUT(NonEmptyMapping(), True)
         self.assertEqual(keys, ['a', 'b', 'c'])
         self.assertEqual(values, [1, 2, 3])
 
 
 class Test_type_and_adr(unittest.TestCase):
 
     def _callFUT(self, obj):
         from BTrees.check import type_and_adr
         return type_and_adr(obj)
 
     def test_type_and_adr_w_oid(self):
         from BTrees.utils import oid_repr
+
         class WithOid:
             _p_oid = b'DEADBEEF'
+
         t_and_a = self._callFUT(WithOid())
         self.assertTrue(t_and_a.startswith('WithOid (0x'))
         self.assertTrue(t_and_a.endswith('oid=%s)' % oid_repr(b'DEADBEEF')))
 
     def test_type_and_adr_wo_oid(self):
         class WithoutOid:
             pass
@@ -197,63 +213,35 @@
         self.assertRaises(NotImplementedError, walker.visit_bucket,
                           obj, path, parent, is_mapping, keys, kids, lo, hi)
 
     def test_walk_w_empty_bucket(self):
         from BTrees.OOBTree import OOBucket
         obj = OOBucket()
         walker = self._makeOne(obj)
-        path = '/'
-        parent = object()
-        is_mapping = True
-        keys = []
-        kids = []
-        lo = 0
-        hi = None
         self.assertRaises(NotImplementedError, walker.walk)
 
     def test_walk_w_empty_btree(self):
         from BTrees.OOBTree import OOBTree
         obj = OOBTree()
         walker = self._makeOne(obj)
-        path = '/'
-        parent = object()
-        is_mapping = True
-        keys = []
-        kids = []
-        lo = 0
-        hi = None
         self.assertRaises(NotImplementedError, walker.walk)
 
     def test_walk_w_degenerate_btree(self):
         from BTrees.OOBTree import OOBTree
         obj = OOBTree()
         obj['a'] = 1
         walker = self._makeOne(obj)
-        path = '/'
-        parent = object()
-        is_mapping = True
-        keys = []
-        kids = []
-        lo = 0
-        hi = None
         self.assertRaises(NotImplementedError, walker.walk)
 
     def test_walk_w_normal_btree(self):
         from BTrees.IIBTree import IIBTree
         obj = IIBTree()
         for i in range(1000):
             obj[i] = i
         walker = self._makeOne(obj)
-        path = '/'
-        parent = object()
-        is_mapping = True
-        keys = []
-        kids = []
-        lo = 0
-        hi = None
         self.assertRaises(NotImplementedError, walker.walk)
 
 
 class CheckerTests(unittest.TestCase):
 
     assertRaises = _assertRaises
 
@@ -264,91 +252,49 @@
     def _makeOne(self, obj):
         return self._getTargetClass()(obj)
 
     def test_walk_w_empty_bucket(self):
         from BTrees.OOBTree import OOBucket
         obj = OOBucket()
         checker = self._makeOne(obj)
-        path = '/'
-        parent = object()
-        is_mapping = True
-        keys = []
-        kids = []
-        lo = 0
-        hi = None
-        checker.check() #noraise
+        checker.check()  # noraise
 
     def test_walk_w_empty_btree(self):
         obj = _makeTree(False)
         checker = self._makeOne(obj)
-        path = '/'
-        parent = object()
-        is_mapping = True
-        keys = []
-        kids = []
-        lo = 0
-        hi = None
-        checker.check() #noraise
+        checker.check()  # noraise
 
     def test_walk_w_degenerate_btree(self):
         obj = _makeTree(False)
         obj['a'] = 1
         checker = self._makeOne(obj)
-        path = '/'
-        parent = object()
-        is_mapping = True
-        keys = []
-        kids = []
-        lo = 0
-        hi = None
-        checker.check() #noraise
+        checker.check()  # noraise
 
     def test_walk_w_normal_btree(self):
         obj = _makeTree(False)
         checker = self._makeOne(obj)
-        path = '/'
-        parent = object()
-        is_mapping = True
-        keys = []
-        kids = []
-        lo = 0
-        hi = None
-        checker.check() #noraise
+        checker.check()  # noraise
 
     def test_walk_w_key_too_large(self):
         obj = _makeTree(True)
         state = obj.__getstate__()
         # Damage an invariant by dropping the BTree key to 14.
         new_state = (state[0][0], 14, state[0][2]), state[1]
         obj.__setstate__(new_state)
         checker = self._makeOne(obj)
-        path = '/'
-        parent = object()
-        is_mapping = True
-        keys = []
-        kids = []
-        lo = 0
-        hi = None
         e = self.assertRaises(AssertionError, checker.check)
         self.assertTrue(">= upper bound" in str(e))
 
     def test_walk_w_key_too_small(self):
         obj = _makeTree(True)
         state = obj.__getstate__()
         # Damage an invariant by bumping the BTree key to 16.
         new_state = (state[0][0], 16, state[0][2]), state[1]
         obj.__setstate__(new_state)
         checker = self._makeOne(obj)
-        path = '/'
-        parent = object()
-        is_mapping = True
-        keys = []
-        kids = []
-        lo = 0
-        hi = None
         e = self.assertRaises(AssertionError, checker.check)
         self.assertTrue("< lower bound" in str(e))
 
     def test_walk_w_keys_swapped(self):
         obj = _makeTree(True)
         state = obj.__getstate__()
         # Damage an invariant by bumping the BTree key to 16.
@@ -363,21 +309,14 @@
         self.assertEqual(pairs[8], 4)
         self.assertEqual(pairs[9], 8)
         self.assertEqual(pairs[10], 5)
         self.assertEqual(pairs[11], 10)
         newpairs = pairs[:8] + (5, 10, 4, 8) + pairs[12:]
         b0.__setstate__((newpairs, nextbucket))
         checker = self._makeOne(obj)
-        path = '/'
-        parent = object()
-        is_mapping = True
-        keys = []
-        kids = []
-        lo = 0
-        hi = None
         e = self.assertRaises(AssertionError, checker.check)
         self.assertTrue("key 5 at index 4 >= key 4 at index 5" in str(e))
 
 
 class Test_check(unittest.TestCase):
 
     def _callFUT(self, tree):
@@ -396,15 +335,15 @@
         tree = OOBTree()
         for i in range(31):
             tree[i] = 2*i
         state = tree.__getstate__()
         self.assertEqual(len(state), 2)
         self.assertEqual(len(state[0]), 3)
         self.assertEqual(state[0][1], 15)
-        self._callFUT(tree)   #noraise
+        self._callFUT(tree)   # noraise
 
 
 def _makeTree(fill):
     from BTrees.OOBTree import OOBTree
     from BTrees.OOBTree import OOBTreePy
     tree = OOBTree()
     if fill:
```

### Comparing `BTrees-5.2/src/BTrees/tests/test_compile_flags.py` & `BTrees-6.0/src/BTrees/tests/test_compile_flags.py`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/src/BTrees/tests/test_dynamic_btrees.py` & `BTrees-6.0/src/BTrees/tests/test_dynamic_btrees.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,29 +7,26 @@
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE
 #
 ##############################################################################
-"""
-This module dynamically creates test modules and suites for
-all expected BTree families that do not have their own test file on disk.
-"""
-
-
-import unittest
+# Dynamically creates test modules and suites for expected BTree families
+# that do not have their own test file on disk.
 import importlib
 import sys
 import types
+import unittest
 
 from BTrees import _FAMILIES
 
 from ._test_builder import update_module
 
+
 # If there is no .py file on disk, create the module in memory.
 # This is helpful during early development. However, it
 # doesn't work with zope-testrunner's ``-m`` filter.
 _suite = unittest.TestSuite()
 for family in _FAMILIES:
     mod_qname = "BTrees.tests.test_" + family + 'BTree'
     try:
@@ -38,14 +35,16 @@
         btree = importlib.import_module("BTrees." + family + 'BTree')
         mod = types.ModuleType(mod_qname)
         update_module(vars(mod), btree)
         sys.modules[mod_qname] = mod
         globals()[mod_qname.split('.', 1)[1]] = mod
         _suite.addTest(unittest.defaultTestLoader.loadTestsFromModule(mod))
 
+
 def test_suite():
     # zope.testrunner protocol
     return _suite
 
-def load_tests(loader, standard_tests, pattern): # pylint:disable=unused-argument
+
+def load_tests(loader, standard_tests, pattern):
     # Pure unittest protocol.
     return test_suite()
```

### Comparing `BTrees-5.2/src/BTrees/tests/test_fsBTree.py` & `BTrees-6.0/src/BTrees/tests/test_fsBTree.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,27 +10,29 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 import unittest
 
 from BTrees import fsBTree
+
 from ._test_builder import update_module
 
+
 class fsBucketTests(unittest.TestCase):
 
     def _getTargetClass(self):
         return fsBTree.fsBucket
 
     def _makeOne(self, *args, **kw):
         return self._getTargetClass()(*args, **kw)
 
     def _makeBytesItems(self):
         from .._compat import _ascii
-        return[(_ascii(c*2), _ascii(c*6)) for c in 'abcdef']
+        return [(_ascii(c*2), _ascii(c*6)) for c in 'abcdef']
 
     def test_toString(self):
         bucket = self._makeOne(self._makeBytesItems())
         self.assertEqual(bucket.toString(),
                          b'aabbccddeeffaaaaaabbbbbbccccccddddddeeeeeeffffff')
 
     def test_fromString(self):
@@ -44,28 +46,29 @@
         self.assertEqual(after.__getstate__(), ((),))
 
     def test_fromString_invalid_length(self):
         bucket = self._makeOne(self._makeBytesItems())
         self.assertRaises(ValueError, bucket.fromString, b'xxx')
 
 
-
 class fsBucketPyTests(fsBucketTests):
 
     def _getTargetClass(self):
         return fsBTree.fsBucketPy
 
+
 class fsTreeTests(unittest.TestCase):
 
     def _check_sizes(self, cls):
         self.assertEqual(cls.max_leaf_size, 500)
         self.assertEqual(cls.max_internal_size, 500)
 
     def test_BTree_sizes(self):
         self._check_sizes(fsBTree.BTree)
         self._check_sizes(fsBTree.BTreePy)
 
     def test_TreeSet_sizes(self):
         self._check_sizes(fsBTree.TreeSet)
         self._check_sizes(fsBTree.TreeSetPy)
 
+
 update_module(globals(), fsBTree)
```

### Comparing `BTrees-5.2/src/BTrees/tests/test_utils.py` & `BTrees-6.0/src/BTrees/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `BTrees-5.2/src/BTrees/utils.py` & `BTrees-6.0/src/BTrees/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 def non_negative(int_val):
     if int_val < 0:
         # Coerce to non-negative.
         int_val &= 0x7FFFFFFFFFFFFFFF
     return int_val
 
 
-def positive_id(obj): # pragma: no cover
+def positive_id(obj):  # pragma: no cover
     """Return id(obj) as a non-negative integer."""
     return non_negative(id(obj))
 
 
 def oid_repr(oid):
     if isinstance(oid, bytes) and len(oid) == 8:
         # Convert to hex and strip leading zeroes.
```

### Comparing `BTrees-5.2/src/BTrees.egg-info/PKG-INFO` & `BTrees-6.0/src/BTrees.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: BTrees
-Version: 5.2
+Version: 6.0
 Summary: Scalable persistent object containers
 Home-page: https://github.com/zopefoundation/BTrees
 Author: Zope Foundation
 Author-email: zodb-dev@zope.org
 License: ZPL 2.1
 Project-URL: Documentation, https://btrees.readthedocs.io
 Project-URL: Issue Tracker, https://github.com/zopefoundation/BTrees/issues
 Project-URL: Sources, https://github.com/zopefoundation/BTrees
 Platform: any
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
+Classifier: Programming Language :: Python :: 3.13
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
 Requires-Dist: persistent>=4.1.0
 Requires-Dist: zope.interface>=5.0.0
 Provides-Extra: test
 Requires-Dist: persistent>=4.4.3; extra == "test"
 Requires-Dist: transaction; extra == "test"
 Requires-Dist: zope.testrunner; extra == "test"
@@ -77,14 +77,22 @@
 further information.
 
 
 ==================
  BTrees Changelog
 ==================
 
+6.0 (2024-05-30)
+================
+
+- Drop support for Python 3.7.
+
+- Build Windows wheels on GHA.
+
+
 5.2 (2024-02-07)
 ================
 
 - Add preliminary support for Python 3.13 as of 3.13a3.
 
 5.1 (2023-10-05)
 ================
```

### Comparing `BTrees-5.2/src/BTrees.egg-info/SOURCES.txt` & `BTrees-6.0/src/BTrees.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -4,29 +4,40 @@
 .readthedocs.yaml
 CHANGES.rst
 CONTRIBUTING.md
 COPYRIGHT.txt
 LICENSE.txt
 MANIFEST.in
 README.rst
-appveyor.yml
 buildout.cfg
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
 docs/Makefile
 docs/api.rst
 docs/changes.rst
 docs/conf.py
 docs/development.rst
 docs/index.rst
 docs/make.bat
 docs/overview.rst
 docs/requirements.txt
+docs/_build/doctest/output.txt
+docs/_build/html/_sources/api.rst.txt
+docs/_build/html/_sources/changes.rst.txt
+docs/_build/html/_sources/development.rst.txt
+docs/_build/html/_sources/index.rst.txt
+docs/_build/html/_sources/overview.rst.txt
+docs/_build/html/_static/basic.css
+docs/_build/html/_static/custom.css
+docs/_build/html/_static/placeholder.txt
+docs/_build/html/_static/pygments.css
+docs/_build/html/_static/css/badge_only.css
+docs/_build/html/_static/css/theme.css
 docs/_static/custom.css
 docs/_static/placeholder.txt
 docs/_templates/placeholder.txt
 include/persistent/persistent/_compat.h
 include/persistent/persistent/cPersistence.h
 include/persistent/persistent/ring.h
 src/BTrees/BTreeItemsTemplate.c
```

### Comparing `BTrees-5.2/tox.ini` & `BTrees-6.0/tox.ini`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,13 @@
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
@@ -17,14 +16,15 @@
     w_zodb
     w_zodb-pure
 
 [testenv]
 usedevelop = true
 pip_pre = py313: true
 deps =
+    setuptools < 69
     Sphinx
 setenv =
     pure: PURE_PYTHON=1
     !pure-!pypy3: PURE_PYTHON=0
     PYTHONFAULTHANDLER=1
     PYTHONDEVMODE=1
     ZOPE_INTERFACE_STRICT_IRO=1
@@ -68,25 +68,27 @@
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

