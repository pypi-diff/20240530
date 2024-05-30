# Comparing `tmp/zope.security-6.2a1.dev0.tar.gz` & `tmp/zope.security-7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zope.security-6.2a1.dev0.tar", last modified: Thu Apr 20 06:20:43 2023, max compression
+gzip compressed data, was "zope.security-7.0.tar", last modified: Thu May 30 07:40:21 2024, max compression
```

## Comparing `zope.security-6.2a1.dev0.tar` & `zope.security-7.0.tar`

### file list

```diff
@@ -1,102 +1,126 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-20 06:20:43.534636 zope.security-6.2a1.dev0/
--rw-r--r--   0 mac        (513) staff       (20)      587 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/.coveragerc
--rwxr-xr-x   0 mac        (513) staff       (20)     2182 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/.manylinux-install.sh
--rwxr-xr-x   0 mac        (513) staff       (20)      509 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/.manylinux.sh
--rw-r--r--   0 mac        (513) staff       (20)    20556 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)      799 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/CONTRIBUTING.md
--rw-r--r--   0 mac        (513) staff       (20)       32 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/COPYRIGHT.txt
--rw-r--r--   0 mac        (513) staff       (20)     2070 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)      452 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)    23376 2023-04-20 06:20:43.534803 zope.security-6.2a1.dev0/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     1290 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/README.rst
--rw-r--r--   0 mac        (513) staff       (20)     1958 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/appveyor.yml
--rw-r--r--   0 mac        (513) staff       (20)      546 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/buildout.cfg
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-20 06:20:43.512626 zope.security-6.2a1.dev0/docs/
--rw-r--r--   0 mac        (513) staff       (20)     5588 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/Makefile
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-20 06:20:43.516872 zope.security-6.2a1.dev0/docs/api/
--rw-r--r--   0 mac        (513) staff       (20)      110 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/api/adapter.rst
--rw-r--r--   0 mac        (513) staff       (20)    23089 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/api/checker.rst
--rw-r--r--   0 mac        (513) staff       (20)     5103 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/api/decorator.rst
--rw-r--r--   0 mac        (513) staff       (20)      122 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/api/interfaces.rst
--rw-r--r--   0 mac        (513) staff       (20)      122 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/api/management.rst
--rw-r--r--   0 mac        (513) staff       (20)      134 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/api/metaconfigure.rst
--rw-r--r--   0 mac        (513) staff       (20)     3332 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/api/permission.rst
--rw-r--r--   0 mac        (513) staff       (20)      130 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/api/protectclass.rst
--rw-r--r--   0 mac        (513) staff       (20)     1003 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/api/proxy.rst
--rw-r--r--   0 mac        (513) staff       (20)      138 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/api/simplepolicies.rst
--rw-r--r--   0 mac        (513) staff       (20)      110 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/api/testing.rst
--rw-r--r--   0 mac        (513) staff       (20)     2258 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/api/zcml.rst
--rw-r--r--   0 mac        (513) staff       (20)       28 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/changes.rst
--rw-r--r--   0 mac        (513) staff       (20)     9154 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/conf.py
--rw-r--r--   0 mac        (513) staff       (20)     8157 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/example.rst
--rw-r--r--   0 mac        (513) staff       (20)    10645 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/hacking.rst
--rw-r--r--   0 mac        (513) staff       (20)      631 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/index.rst
--rw-r--r--   0 mac        (513) staff       (20)     5108 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/make.bat
--rw-r--r--   0 mac        (513) staff       (20)     4334 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/narr.rst
--rw-r--r--   0 mac        (513) staff       (20)    14695 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/docs/proxy.rst
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-20 06:20:43.503250 zope.security-6.2a1.dev0/include/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-20 06:20:43.503389 zope.security-6.2a1.dev0/include/zope.proxy/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-20 06:20:43.503526 zope.security-6.2a1.dev0/include/zope.proxy/zope/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-20 06:20:43.517207 zope.security-6.2a1.dev0/include/zope.proxy/zope/proxy/
--rw-r--r--   0 mac        (513) staff       (20)     1457 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/include/zope.proxy/zope/proxy/proxy.h
--rw-r--r--   0 mac        (513) staff       (20)      122 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/rtd.txt
--rw-r--r--   0 mac        (513) staff       (20)      595 2023-04-20 06:20:43.535422 zope.security-6.2a1.dev0/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     5837 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-20 06:20:43.504062 zope.security-6.2a1.dev0/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-20 06:20:43.517536 zope.security-6.2a1.dev0/src/zope/
--rw-r--r--   0 mac        (513) staff       (20)       56 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-20 06:20:43.527111 zope.security-6.2a1.dev0/src/zope/security/
--rw-r--r--   0 mac        (513) staff       (20)     1009 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     1684 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/_compat.py
--rw-r--r--   0 mac        (513) staff       (20)      997 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/_definitions.py
--rw-r--r--   0 mac        (513) staff       (20)    26688 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/_proxy.c
--rw-r--r--   0 mac        (513) staff       (20)    18340 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/_zope_security_checker.c
--rw-r--r--   0 mac        (513) staff       (20)     4955 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/adapter.py
--rw-r--r--   0 mac        (513) staff       (20)    36314 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/checker.py
--rw-r--r--   0 mac        (513) staff       (20)      639 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/configure.zcml
--rw-r--r--   0 mac        (513) staff       (20)     3159 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/decorator.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-20 06:20:43.527771 zope.security-6.2a1.dev0/src/zope/security/examples/
--rw-r--r--   0 mac        (513) staff       (20)     8769 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/examples/sandbox.py
--rw-r--r--   0 mac        (513) staff       (20)     6305 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/examples/sandbox_security.py
--rw-r--r--   0 mac        (513) staff       (20)      892 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/i18n.py
--rw-r--r--   0 mac        (513) staff       (20)    13752 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/interfaces.py
--rw-r--r--   0 mac        (513) staff       (20)     5115 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/management.py
--rw-r--r--   0 mac        (513) staff       (20)     1964 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/meta.zcml
--rw-r--r--   0 mac        (513) staff       (20)     8318 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/metaconfigure.py
--rw-r--r--   0 mac        (513) staff       (20)     6862 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/metadirectives.py
--rw-r--r--   0 mac        (513) staff       (20)     3531 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/permission.py
--rw-r--r--   0 mac        (513) staff       (20)     1019 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/permissions.zcml
--rw-r--r--   0 mac        (513) staff       (20)     3504 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/protectclass.py
--rw-r--r--   0 mac        (513) staff       (20)    13815 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/proxy.py
--rw-r--r--   0 mac        (513) staff       (20)     2750 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/simplepolicies.py
--rw-r--r--   0 mac        (513) staff       (20)     3209 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/testing.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-20 06:20:43.534317 zope.security-6.2a1.dev0/src/zope/security/tests/
--rw-r--r--   0 mac        (513) staff       (20)      589 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/tests/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)      856 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/tests/exampleclass.py
--rw-r--r--   0 mac        (513) staff       (20)     1560 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/tests/module.py
--rw-r--r--   0 mac        (513) staff       (20)      707 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/tests/redefineperms.zcml
--rw-r--r--   0 mac        (513) staff       (20)    18656 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/tests/test_adapter.py
--rw-r--r--   0 mac        (513) staff       (20)    87468 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/tests/test_checker.py
--rw-r--r--   0 mac        (513) staff       (20)     1373 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/tests/test_compile_flags.py
--rw-r--r--   0 mac        (513) staff       (20)     6087 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/tests/test_decorator.py
--rw-r--r--   0 mac        (513) staff       (20)     1675 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/tests/test_location.py
--rw-r--r--   0 mac        (513) staff       (20)     7424 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/tests/test_management.py
--rw-r--r--   0 mac        (513) staff       (20)    30575 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/tests/test_metaconfigure.py
--rw-r--r--   0 mac        (513) staff       (20)     7816 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/tests/test_permission.py
--rw-r--r--   0 mac        (513) staff       (20)     5544 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/tests/test_protectclass.py
--rw-r--r--   0 mac        (513) staff       (20)    65397 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/tests/test_proxy.py
--rw-r--r--   0 mac        (513) staff       (20)     2799 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/tests/test_simpleinteraction.py
--rw-r--r--   0 mac        (513) staff       (20)     4863 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/tests/test_simplepolicies.py
--rw-r--r--   0 mac        (513) staff       (20)     2760 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/tests/test_testing.py
--rw-r--r--   0 mac        (513) staff       (20)     8016 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/tests/test_zcml.py
--rw-r--r--   0 mac        (513) staff       (20)    21828 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/tests/test_zcml_functest.py
--rw-r--r--   0 mac        (513) staff       (20)     3981 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/src/zope/security/zcml.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-20 06:20:43.519863 zope.security-6.2a1.dev0/src/zope.security.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)    23376 2023-04-20 06:20:43.000000 zope.security-6.2a1.dev0/src/zope.security.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     2525 2023-04-20 06:20:43.000000 zope.security-6.2a1.dev0/src/zope.security.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2023-04-20 06:20:43.000000 zope.security-6.2a1.dev0/src/zope.security.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2023-04-20 06:20:43.000000 zope.security-6.2a1.dev0/src/zope.security.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2023-04-20 06:20:43.000000 zope.security-6.2a1.dev0/src/zope.security.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)      368 2023-04-20 06:20:43.000000 zope.security-6.2a1.dev0/src/zope.security.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2023-04-20 06:20:43.000000 zope.security-6.2a1.dev0/src/zope.security.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)     1666 2023-04-20 06:20:42.000000 zope.security-6.2a1.dev0/tox.ini
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 07:40:21.968726 zope.security-7.0/
+-rw-r--r--   0 jens       (501) staff       (20)      608 2024-05-29 19:08:50.000000 zope.security-7.0/.coveragerc
+-rwxr-xr-x   0 jens       (501) staff       (20)     2192 2024-05-29 19:08:50.000000 zope.security-7.0/.manylinux-install.sh
+-rwxr-xr-x   0 jens       (501) staff       (20)      509 2024-05-29 19:08:50.000000 zope.security-7.0/.manylinux.sh
+-rw-r--r--   0 jens       (501) staff       (20)      664 2024-05-29 19:08:50.000000 zope.security-7.0/.readthedocs.yaml
+-rw-r--r--   0 jens       (501) staff       (20)    20576 2024-05-30 06:40:44.000000 zope.security-7.0/CHANGES.rst
+-rw-r--r--   0 jens       (501) staff       (20)      799 2024-05-29 19:08:50.000000 zope.security-7.0/CONTRIBUTING.md
+-rw-r--r--   0 jens       (501) staff       (20)       32 2023-01-03 12:45:40.000000 zope.security-7.0/COPYRIGHT.txt
+-rw-r--r--   0 jens       (501) staff       (20)     2070 2023-01-03 12:45:40.000000 zope.security-7.0/LICENSE.txt
+-rw-r--r--   0 jens       (501) staff       (20)      446 2024-05-29 19:08:50.000000 zope.security-7.0/MANIFEST.in
+-rw-r--r--   0 jens       (501) staff       (20)    24338 2024-05-30 07:40:21.968651 zope.security-7.0/PKG-INFO
+-rw-r--r--   0 jens       (501) staff       (20)     1291 2024-05-24 14:22:55.000000 zope.security-7.0/README.rst
+-rw-r--r--   0 jens       (501) staff       (20)      546 2023-01-16 14:43:05.000000 zope.security-7.0/buildout.cfg
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 07:40:21.954585 zope.security-7.0/docs/
+-rw-r--r--   0 jens       (501) staff       (20)     5588 2023-01-03 12:45:40.000000 zope.security-7.0/docs/Makefile
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 07:40:21.949324 zope.security-7.0/docs/_build/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 07:40:21.954786 zope.security-7.0/docs/_build/doctest/
+-rw-r--r--   0 jens       (501) staff       (20)     1490 2024-05-29 10:22:34.000000 zope.security-7.0/docs/_build/doctest/output.txt
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 07:40:21.949366 zope.security-7.0/docs/_build/html/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 07:40:21.956027 zope.security-7.0/docs/_build/html/_sources/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 07:40:21.957825 zope.security-7.0/docs/_build/html/_sources/api/
+-rw-r--r--   0 jens       (501) staff       (20)      110 2023-01-03 12:45:40.000000 zope.security-7.0/docs/_build/html/_sources/api/adapter.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)    23089 2023-01-03 12:45:40.000000 zope.security-7.0/docs/_build/html/_sources/api/checker.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     5103 2023-01-03 12:45:40.000000 zope.security-7.0/docs/_build/html/_sources/api/decorator.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)      122 2023-01-03 12:45:40.000000 zope.security-7.0/docs/_build/html/_sources/api/interfaces.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)      122 2023-01-03 12:45:40.000000 zope.security-7.0/docs/_build/html/_sources/api/management.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)      134 2023-01-03 12:45:40.000000 zope.security-7.0/docs/_build/html/_sources/api/metaconfigure.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     3332 2023-01-03 12:45:40.000000 zope.security-7.0/docs/_build/html/_sources/api/permission.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)      130 2023-01-03 12:45:40.000000 zope.security-7.0/docs/_build/html/_sources/api/protectclass.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     1003 2023-01-03 12:45:40.000000 zope.security-7.0/docs/_build/html/_sources/api/proxy.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)      138 2023-01-03 12:45:40.000000 zope.security-7.0/docs/_build/html/_sources/api/simplepolicies.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)      110 2023-01-03 12:45:40.000000 zope.security-7.0/docs/_build/html/_sources/api/testing.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     2258 2023-01-03 12:45:40.000000 zope.security-7.0/docs/_build/html/_sources/api/zcml.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)       28 2023-01-03 12:45:40.000000 zope.security-7.0/docs/_build/html/_sources/changes.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     8157 2023-01-03 12:45:40.000000 zope.security-7.0/docs/_build/html/_sources/example.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)    10645 2023-01-03 12:45:40.000000 zope.security-7.0/docs/_build/html/_sources/hacking.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)      631 2023-01-03 12:45:40.000000 zope.security-7.0/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     4334 2023-01-03 12:45:40.000000 zope.security-7.0/docs/_build/html/_sources/narr.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)    14695 2023-01-03 12:45:40.000000 zope.security-7.0/docs/_build/html/_sources/proxy.rst.txt
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 07:40:21.959594 zope.security-7.0/docs/api/
+-rw-r--r--   0 jens       (501) staff       (20)      110 2023-01-03 12:45:40.000000 zope.security-7.0/docs/api/adapter.rst
+-rw-r--r--   0 jens       (501) staff       (20)    23089 2023-01-03 12:45:40.000000 zope.security-7.0/docs/api/checker.rst
+-rw-r--r--   0 jens       (501) staff       (20)     5103 2023-01-03 12:45:40.000000 zope.security-7.0/docs/api/decorator.rst
+-rw-r--r--   0 jens       (501) staff       (20)      122 2023-01-03 12:45:40.000000 zope.security-7.0/docs/api/interfaces.rst
+-rw-r--r--   0 jens       (501) staff       (20)      122 2023-01-03 12:45:40.000000 zope.security-7.0/docs/api/management.rst
+-rw-r--r--   0 jens       (501) staff       (20)      134 2023-01-03 12:45:40.000000 zope.security-7.0/docs/api/metaconfigure.rst
+-rw-r--r--   0 jens       (501) staff       (20)     3332 2023-01-03 12:45:40.000000 zope.security-7.0/docs/api/permission.rst
+-rw-r--r--   0 jens       (501) staff       (20)      130 2023-01-03 12:45:40.000000 zope.security-7.0/docs/api/protectclass.rst
+-rw-r--r--   0 jens       (501) staff       (20)     1003 2023-01-03 12:45:40.000000 zope.security-7.0/docs/api/proxy.rst
+-rw-r--r--   0 jens       (501) staff       (20)      138 2023-01-03 12:45:40.000000 zope.security-7.0/docs/api/simplepolicies.rst
+-rw-r--r--   0 jens       (501) staff       (20)      110 2023-01-03 12:45:40.000000 zope.security-7.0/docs/api/testing.rst
+-rw-r--r--   0 jens       (501) staff       (20)     2258 2023-01-03 12:45:40.000000 zope.security-7.0/docs/api/zcml.rst
+-rw-r--r--   0 jens       (501) staff       (20)       28 2023-01-03 12:45:40.000000 zope.security-7.0/docs/changes.rst
+-rw-r--r--   0 jens       (501) staff       (20)     9163 2023-10-05 12:07:44.000000 zope.security-7.0/docs/conf.py
+-rw-r--r--   0 jens       (501) staff       (20)     8157 2023-01-03 12:45:40.000000 zope.security-7.0/docs/example.rst
+-rw-r--r--   0 jens       (501) staff       (20)    10645 2023-01-03 12:45:40.000000 zope.security-7.0/docs/hacking.rst
+-rw-r--r--   0 jens       (501) staff       (20)      631 2023-01-03 12:45:40.000000 zope.security-7.0/docs/index.rst
+-rw-r--r--   0 jens       (501) staff       (20)     5108 2023-01-03 12:45:40.000000 zope.security-7.0/docs/make.bat
+-rw-r--r--   0 jens       (501) staff       (20)     4334 2023-01-03 12:45:40.000000 zope.security-7.0/docs/narr.rst
+-rw-r--r--   0 jens       (501) staff       (20)    14695 2023-01-03 12:45:40.000000 zope.security-7.0/docs/proxy.rst
+-rw-r--r--   0 jens       (501) staff       (20)       82 2023-10-05 12:07:44.000000 zope.security-7.0/docs/requirements.txt
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 07:40:21.949566 zope.security-7.0/include/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 07:40:21.949604 zope.security-7.0/include/zope.proxy/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 07:40:21.949643 zope.security-7.0/include/zope.proxy/zope/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 07:40:21.959723 zope.security-7.0/include/zope.proxy/zope/proxy/
+-rw-r--r--   0 jens       (501) staff       (20)     1457 2023-04-20 08:04:16.000000 zope.security-7.0/include/zope.proxy/zope/proxy/proxy.h
+-rw-r--r--   0 jens       (501) staff       (20)      646 2024-05-30 07:40:21.968942 zope.security-7.0/setup.cfg
+-rw-r--r--   0 jens       (501) staff       (20)     5915 2024-05-30 06:40:59.000000 zope.security-7.0/setup.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 07:40:21.949787 zope.security-7.0/src/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 07:40:21.959838 zope.security-7.0/src/zope/
+-rw-r--r--   0 jens       (501) staff       (20)       56 2023-01-03 12:45:40.000000 zope.security-7.0/src/zope/__init__.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 07:40:21.963994 zope.security-7.0/src/zope/security/
+-rw-r--r--   0 jens       (501) staff       (20)     1009 2023-01-03 12:45:40.000000 zope.security-7.0/src/zope/security/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)     1684 2023-01-03 12:45:40.000000 zope.security-7.0/src/zope/security/_compat.py
+-rw-r--r--   0 jens       (501) staff       (20)      997 2023-01-03 12:45:40.000000 zope.security-7.0/src/zope/security/_definitions.py
+-rw-r--r--   0 jens       (501) staff       (20)    26688 2023-04-18 06:53:23.000000 zope.security-7.0/src/zope/security/_proxy.c
+-rw-r--r--   0 jens       (501) staff       (20)    18340 2023-01-03 12:45:40.000000 zope.security-7.0/src/zope/security/_zope_security_checker.c
+-rw-r--r--   0 jens       (501) staff       (20)     4955 2023-01-03 12:45:40.000000 zope.security-7.0/src/zope/security/adapter.py
+-rw-r--r--   0 jens       (501) staff       (20)    36314 2023-01-18 07:34:11.000000 zope.security-7.0/src/zope/security/checker.py
+-rw-r--r--   0 jens       (501) staff       (20)      639 2023-01-03 12:45:40.000000 zope.security-7.0/src/zope/security/configure.zcml
+-rw-r--r--   0 jens       (501) staff       (20)     3159 2023-01-03 12:45:40.000000 zope.security-7.0/src/zope/security/decorator.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 07:40:21.964389 zope.security-7.0/src/zope/security/examples/
+-rw-r--r--   0 jens       (501) staff       (20)     8769 2023-01-03 12:45:40.000000 zope.security-7.0/src/zope/security/examples/sandbox.py
+-rw-r--r--   0 jens       (501) staff       (20)     6305 2023-01-03 12:45:40.000000 zope.security-7.0/src/zope/security/examples/sandbox_security.py
+-rw-r--r--   0 jens       (501) staff       (20)      892 2023-01-03 12:45:40.000000 zope.security-7.0/src/zope/security/i18n.py
+-rw-r--r--   0 jens       (501) staff       (20)    13752 2023-01-03 12:45:40.000000 zope.security-7.0/src/zope/security/interfaces.py
+-rw-r--r--   0 jens       (501) staff       (20)     5115 2023-01-03 12:45:40.000000 zope.security-7.0/src/zope/security/management.py
+-rw-r--r--   0 jens       (501) staff       (20)     1964 2023-01-03 12:45:40.000000 zope.security-7.0/src/zope/security/meta.zcml
+-rw-r--r--   0 jens       (501) staff       (20)     8318 2023-01-03 12:45:40.000000 zope.security-7.0/src/zope/security/metaconfigure.py
+-rw-r--r--   0 jens       (501) staff       (20)     6862 2023-01-03 12:45:40.000000 zope.security-7.0/src/zope/security/metadirectives.py
+-rw-r--r--   0 jens       (501) staff       (20)     3531 2023-01-03 12:45:40.000000 zope.security-7.0/src/zope/security/permission.py
+-rw-r--r--   0 jens       (501) staff       (20)     1019 2023-01-03 12:45:40.000000 zope.security-7.0/src/zope/security/permissions.zcml
+-rw-r--r--   0 jens       (501) staff       (20)     3504 2023-01-03 12:45:40.000000 zope.security-7.0/src/zope/security/protectclass.py
+-rw-r--r--   0 jens       (501) staff       (20)    13815 2023-04-18 06:53:23.000000 zope.security-7.0/src/zope/security/proxy.py
+-rw-r--r--   0 jens       (501) staff       (20)     2750 2023-01-03 12:45:40.000000 zope.security-7.0/src/zope/security/simplepolicies.py
+-rw-r--r--   0 jens       (501) staff       (20)     3209 2023-01-03 12:45:40.000000 zope.security-7.0/src/zope/security/testing.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 07:40:21.967422 zope.security-7.0/src/zope/security/tests/
+-rw-r--r--   0 jens       (501) staff       (20)      589 2023-01-03 12:45:40.000000 zope.security-7.0/src/zope/security/tests/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)      856 2023-01-03 12:45:40.000000 zope.security-7.0/src/zope/security/tests/exampleclass.py
+-rw-r--r--   0 jens       (501) staff       (20)     1560 2023-01-03 12:45:40.000000 zope.security-7.0/src/zope/security/tests/module.py
+-rw-r--r--   0 jens       (501) staff       (20)      707 2023-01-03 12:45:40.000000 zope.security-7.0/src/zope/security/tests/redefineperms.zcml
+-rw-r--r--   0 jens       (501) staff       (20)    18656 2023-01-03 12:45:40.000000 zope.security-7.0/src/zope/security/tests/test_adapter.py
+-rw-r--r--   0 jens       (501) staff       (20)    87468 2023-04-18 06:53:23.000000 zope.security-7.0/src/zope/security/tests/test_checker.py
+-rw-r--r--   0 jens       (501) staff       (20)     1373 2023-01-03 12:45:40.000000 zope.security-7.0/src/zope/security/tests/test_compile_flags.py
+-rw-r--r--   0 jens       (501) staff       (20)     6087 2023-01-03 12:45:40.000000 zope.security-7.0/src/zope/security/tests/test_decorator.py
+-rw-r--r--   0 jens       (501) staff       (20)     1675 2023-01-03 12:45:40.000000 zope.security-7.0/src/zope/security/tests/test_location.py
+-rw-r--r--   0 jens       (501) staff       (20)     7424 2023-01-03 12:45:40.000000 zope.security-7.0/src/zope/security/tests/test_management.py
+-rw-r--r--   0 jens       (501) staff       (20)    30575 2023-01-03 12:45:40.000000 zope.security-7.0/src/zope/security/tests/test_metaconfigure.py
+-rw-r--r--   0 jens       (501) staff       (20)     7816 2023-01-03 12:45:40.000000 zope.security-7.0/src/zope/security/tests/test_permission.py
+-rw-r--r--   0 jens       (501) staff       (20)     5544 2023-01-03 12:45:40.000000 zope.security-7.0/src/zope/security/tests/test_protectclass.py
+-rw-r--r--   0 jens       (501) staff       (20)    65397 2023-04-18 06:53:23.000000 zope.security-7.0/src/zope/security/tests/test_proxy.py
+-rw-r--r--   0 jens       (501) staff       (20)     2799 2023-01-03 12:45:40.000000 zope.security-7.0/src/zope/security/tests/test_simpleinteraction.py
+-rw-r--r--   0 jens       (501) staff       (20)     4863 2023-01-03 12:45:40.000000 zope.security-7.0/src/zope/security/tests/test_simplepolicies.py
+-rw-r--r--   0 jens       (501) staff       (20)     2760 2023-01-03 12:45:40.000000 zope.security-7.0/src/zope/security/tests/test_testing.py
+-rw-r--r--   0 jens       (501) staff       (20)     8016 2023-01-03 12:45:40.000000 zope.security-7.0/src/zope/security/tests/test_zcml.py
+-rw-r--r--   0 jens       (501) staff       (20)    21828 2023-01-03 12:45:40.000000 zope.security-7.0/src/zope/security/tests/test_zcml_functest.py
+-rw-r--r--   0 jens       (501) staff       (20)     3981 2023-01-03 12:45:40.000000 zope.security-7.0/src/zope/security/zcml.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 07:40:21.960649 zope.security-7.0/src/zope.security.egg-info/
+-rw-r--r--   0 jens       (501) staff       (20)    24338 2024-05-30 07:40:21.000000 zope.security-7.0/src/zope.security.egg-info/PKG-INFO
+-rw-r--r--   0 jens       (501) staff       (20)     3396 2024-05-30 07:40:21.000000 zope.security-7.0/src/zope.security.egg-info/SOURCES.txt
+-rw-r--r--   0 jens       (501) staff       (20)        1 2024-05-30 07:40:21.000000 zope.security-7.0/src/zope.security.egg-info/dependency_links.txt
+-rw-r--r--   0 jens       (501) staff       (20)        5 2024-05-30 07:40:21.000000 zope.security-7.0/src/zope.security.egg-info/namespace_packages.txt
+-rw-r--r--   0 jens       (501) staff       (20)        1 2023-01-03 14:40:42.000000 zope.security-7.0/src/zope.security.egg-info/not-zip-safe
+-rw-r--r--   0 jens       (501) staff       (20)      383 2024-05-30 07:40:21.000000 zope.security-7.0/src/zope.security.egg-info/requires.txt
+-rw-r--r--   0 jens       (501) staff       (20)        5 2024-05-30 07:40:21.000000 zope.security-7.0/src/zope.security.egg-info/top_level.txt
+-rw-r--r--   0 jens       (501) staff       (20)     2056 2024-05-29 19:08:50.000000 zope.security-7.0/tox.ini
```

### Comparing `zope.security-6.2a1.dev0/.coveragerc` & `zope.security-7.0/.coveragerc`

 * *Files 10% similar despite different names*

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

### Comparing `zope.security-6.2a1.dev0/.manylinux-install.sh` & `zope.security-7.0/.manylinux-install.sh`

 * *Files 8% similar despite different names*

```diff
@@ -24,34 +24,34 @@
 ls -ld /cache/pip
 
 # We need some libraries because we build wheels from scratch:
 yum -y install libffi-devel
 
 tox_env_map() {
     case $1 in
-        *"cp312"*) echo 'py312';;
-        *"cp37"*) echo 'py37';;
+        *"cp313"*) echo 'py313';;
         *"cp38"*) echo 'py38';;
         *"cp39"*) echo 'py39';;
         *"cp310"*) echo 'py310';;
         *"cp311"*) echo 'py311';;
+        *"cp312"*) echo 'py312';;
         *) echo 'py';;
     esac
 }
 
 # Compile wheels
 for PYBIN in /opt/python/*/bin; do
     if \
-       [[ "${PYBIN}" == *"cp312"* ]] || \
-       [[ "${PYBIN}" == *"cp311"* ]] || \
-       [[ "${PYBIN}" == *"cp37"* ]] || \
-       [[ "${PYBIN}" == *"cp38"* ]] || \
-       [[ "${PYBIN}" == *"cp39"* ]] || \
-       [[ "${PYBIN}" == *"cp310"* ]] ; then
-        if [[ "${PYBIN}" == *"cp312"* ]] ; then
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

### Comparing `zope.security-6.2a1.dev0/CHANGES.rst` & `zope.security-7.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 =========
  Changes
 =========
 
-6.2a1.dev0 (2023-04-20)
------------------------
+7.0 (2024-05-30)
+----------------
+
+- Add preliminary support for Python 3.13 as of 3.13b1.
+
+- Drop support for Python 3.7.
+
+- Build windows wheels on GHA.
+
+
+6.2 (2023-10-05)
+----------------
 
 - Make ``next()`` on C proxies call ``__next__`` rather than ``next`` (see
   PEP 3114), and drop support for the Python 2 ``next`` method name from
   pure-Python proxies.
 
 - Drop using ``setup_requires`` due to constant problems on GHA.
 
-- Add preliminary support for Python 3.12 as of 3.12a7 -- even though there are
-  currently tests breaking, so please do not consider it fully supported.
+- Add support for Python 3.12.
 
 
 6.1 (2023-01-18)
 ================
 
 - Remove more proxying code for names that no longer exist in Python 3.
   (`#92 <https://github.com/zopefoundation/zope.security/issues/92>`_)
```

### Comparing `zope.security-6.2a1.dev0/CONTRIBUTING.md` & `zope.security-7.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/LICENSE.txt` & `zope.security-7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/PKG-INFO` & `zope.security-7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zope.security
-Version: 6.2a1.dev0
+Version: 7.0
 Summary: Zope Security Framework
 Home-page: http://github.com/zopefoundation/zope.security
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Project-URL: Documentation, https://zopesecurity.readthedocs.io
 Project-URL: Issue Tracker, https://github.com/zopefoundation/zope.security/issues
@@ -12,32 +12,54 @@
 Keywords: zope security policy principal permission
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Framework :: Zope :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.8
+License-File: LICENSE.txt
+Requires-Dist: setuptools
+Requires-Dist: zope.component
+Requires-Dist: zope.i18nmessageid
+Requires-Dist: zope.interface
+Requires-Dist: zope.location
+Requires-Dist: zope.proxy>=5.2
+Requires-Dist: zope.schema>=4.2.0
 Provides-Extra: pytz
+Requires-Dist: pytz; extra == "pytz"
 Provides-Extra: untrustedpython
+Requires-Dist: zope.untrustedpython>=5.0.dev0; extra == "untrustedpython"
 Provides-Extra: zcml
+Requires-Dist: zope.configuration; extra == "zcml"
 Provides-Extra: test
+Requires-Dist: BTrees; extra == "test"
+Requires-Dist: zope.component; extra == "test"
+Requires-Dist: zope.configuration; extra == "test"
+Requires-Dist: zope.location; extra == "test"
+Requires-Dist: zope.testing; extra == "test"
+Requires-Dist: zope.testrunner; extra == "test"
 Provides-Extra: docs
-License-File: LICENSE.txt
+Requires-Dist: Sphinx; extra == "docs"
+Requires-Dist: repoze.sphinx.autointerface; extra == "docs"
+Requires-Dist: sphinx_rtd_theme; extra == "docs"
+Requires-Dist: zope.configuration; extra == "docs"
+Requires-Dist: zope.testing; extra == "docs"
 
 ===================
  ``zope.security``
 ===================
 
 .. image:: https://github.com/zopefoundation/zope.security/actions/workflows/tests.yml/badge.svg
         :target: https://github.com/zopefoundation/zope.security/actions/workflows/tests.yml
@@ -63,29 +85,39 @@
 
 The Security framework provides a generic mechanism to implement security
 policies on Python objects.
 
 Documentation is available at https://zopesecurity.readthedocs.io/
 
 
+
 =========
  Changes
 =========
 
-6.2a1.dev0 (2023-04-20)
------------------------
+7.0 (2024-05-30)
+----------------
+
+- Add preliminary support for Python 3.13 as of 3.13b1.
+
+- Drop support for Python 3.7.
+
+- Build windows wheels on GHA.
+
+
+6.2 (2023-10-05)
+----------------
 
 - Make ``next()`` on C proxies call ``__next__`` rather than ``next`` (see
   PEP 3114), and drop support for the Python 2 ``next`` method name from
   pure-Python proxies.
 
 - Drop using ``setup_requires`` due to constant problems on GHA.
 
-- Add preliminary support for Python 3.12 as of 3.12a7 -- even though there are
-  currently tests breaking, so please do not consider it fully supported.
+- Add support for Python 3.12.
 
 
 6.1 (2023-01-18)
 ================
 
 - Remove more proxying code for names that no longer exist in Python 3.
   (`#92 <https://github.com/zopefoundation/zope.security/issues/92>`_)
```

### Comparing `zope.security-6.2a1.dev0/README.rst` & `zope.security-7.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -24,7 +24,8 @@
         :alt: Supported Python versions
 
 
 The Security framework provides a generic mechanism to implement security
 policies on Python objects.
 
 Documentation is available at https://zopesecurity.readthedocs.io/
+
```

### Comparing `zope.security-6.2a1.dev0/buildout.cfg` & `zope.security-7.0/buildout.cfg`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/docs/Makefile` & `zope.security-7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/docs/api/checker.rst` & `zope.security-7.0/docs/_build/html/_sources/api/checker.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/docs/api/decorator.rst` & `zope.security-7.0/docs/_build/html/_sources/api/decorator.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/docs/api/permission.rst` & `zope.security-7.0/docs/_build/html/_sources/api/permission.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/docs/api/proxy.rst` & `zope.security-7.0/docs/_build/html/_sources/api/proxy.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/docs/api/zcml.rst` & `zope.security-7.0/docs/_build/html/_sources/api/zcml.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/docs/conf.py` & `zope.security-7.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 #modindex_common_prefix = []
 
 
 # -- Options for HTML output ---------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = 'default'
+html_theme = 'sphinx_rtd_theme'
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #html_theme_options = {}
 
 # Add any paths that contain custom themes here, relative to this directory.
```

### Comparing `zope.security-6.2a1.dev0/docs/example.rst` & `zope.security-7.0/docs/_build/html/_sources/example.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/docs/hacking.rst` & `zope.security-7.0/docs/_build/html/_sources/hacking.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/docs/index.rst` & `zope.security-7.0/docs/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/docs/make.bat` & `zope.security-7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/docs/narr.rst` & `zope.security-7.0/docs/_build/html/_sources/narr.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/docs/proxy.rst` & `zope.security-7.0/docs/_build/html/_sources/proxy.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/include/zope.proxy/zope/proxy/proxy.h` & `zope.security-7.0/include/zope.proxy/zope/proxy/proxy.h`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/setup.cfg` & `zope.security-7.0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-[bdist_wheel]
-universal = 0
-
 [zest.releaser]
 create-wheel = no
 
 [flake8]
 doctests = 1
 per-file-ignores = 
 	src/zope/security/__init__.py: F401
 
 [check-manifest]
 ignore = 
 	.editorconfig
 	.meta.toml
 	docs/_build/html/_sources/*
 	docs/_build/doctest/*
-	docs/_build/html/_sources/api/*
+	docs/_build/*/*/*/*/*
+	docs/_build/*/*/*/*
+	docs/_build/*/*/*
+	docs/_build/*/*
+	docs/_build/*
+	src/coverage.xml
 
 [isort]
 force_single_line = True
 combine_as_imports = True
 sections = FUTURE,STDLIB,THIRDPARTY,ZOPE,FIRSTPARTY,LOCALFOLDER
 known_third_party = docutils, pkg_resources, pytz
 known_zope =
```

### Comparing `zope.security-6.2a1.dev0/setup.py` & `zope.security-7.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     'zope.location',
     'zope.testing',
     'zope.testrunner',
 ]
 
 
 setup(name='zope.security',
-      version='6.2a1.dev0',
+      version='7.0',
       author='Zope Foundation and Contributors',
       author_email='zope-dev@zope.org',
       description='Zope Security Framework',
       long_description=(
           read('README.rst')
           + '\n\n' +
           read('CHANGES.rst')
@@ -117,19 +117,20 @@
       classifiers=[
           'Development Status :: 5 - Production/Stable',
           'Environment :: Web Environment',
           'Intended Audience :: Developers',
           'License :: OSI Approved :: Zope Public License',
           'Programming Language :: Python',
           'Programming Language :: Python :: 3',
-          'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
           'Programming Language :: Python :: 3.10',
           'Programming Language :: Python :: 3.11',
+          'Programming Language :: Python :: 3.12',
+          'Programming Language :: Python :: 3.13',
           'Programming Language :: Python :: Implementation :: CPython',
           'Programming Language :: Python :: Implementation :: PyPy',
           'Natural Language :: English',
           'Operating System :: OS Independent',
           'Topic :: Internet :: WWW/HTTP',
           'Framework :: Zope :: 3',
       ],
@@ -144,22 +145,22 @@
       packages=find_packages('src'),
       package_dir={'': 'src'},
       namespace_packages=['zope'],
       cmdclass={
           'build_ext': optional_build_ext,
       },
       ext_modules=ext_modules,
-      python_requires='>=3.7',
+      python_requires='>=3.8',
       install_requires=[
           'setuptools',
           'zope.component',
           'zope.i18nmessageid',
           'zope.interface',
           'zope.location',
-          'zope.proxy >= 4.3.0',
+          'zope.proxy >= 5.2',
           'zope.schema >= 4.2.0',
       ],
       tests_require=TESTS_REQUIRE,
       extras_require={
           'pytz': [
               "pytz"
           ],
@@ -169,14 +170,15 @@
           'zcml': [
               'zope.configuration'
           ],
           'test': TESTS_REQUIRE,
           'docs': [
               'Sphinx',
               'repoze.sphinx.autointerface',
+              'sphinx_rtd_theme',
               'zope.configuration',
               'zope.testing',
           ],
       },
       include_package_data=True,
       zip_safe=False,
       )
```

### Comparing `zope.security-6.2a1.dev0/src/zope/security/__init__.py` & `zope.security-7.0/src/zope/security/__init__.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/_compat.py` & `zope.security-7.0/src/zope/security/_compat.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/_definitions.py` & `zope.security-7.0/src/zope/security/_definitions.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/_proxy.c` & `zope.security-7.0/src/zope/security/_proxy.c`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/_zope_security_checker.c` & `zope.security-7.0/src/zope/security/_zope_security_checker.c`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/adapter.py` & `zope.security-7.0/src/zope/security/adapter.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/checker.py` & `zope.security-7.0/src/zope/security/checker.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/configure.zcml` & `zope.security-7.0/src/zope/security/configure.zcml`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/decorator.py` & `zope.security-7.0/src/zope/security/decorator.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/examples/sandbox.py` & `zope.security-7.0/src/zope/security/examples/sandbox.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/examples/sandbox_security.py` & `zope.security-7.0/src/zope/security/examples/sandbox_security.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/i18n.py` & `zope.security-7.0/src/zope/security/i18n.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/interfaces.py` & `zope.security-7.0/src/zope/security/interfaces.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/management.py` & `zope.security-7.0/src/zope/security/management.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/meta.zcml` & `zope.security-7.0/src/zope/security/meta.zcml`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/metaconfigure.py` & `zope.security-7.0/src/zope/security/metaconfigure.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/metadirectives.py` & `zope.security-7.0/src/zope/security/metadirectives.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/permission.py` & `zope.security-7.0/src/zope/security/permission.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/permissions.zcml` & `zope.security-7.0/src/zope/security/permissions.zcml`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/protectclass.py` & `zope.security-7.0/src/zope/security/protectclass.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/proxy.py` & `zope.security-7.0/src/zope/security/proxy.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/simplepolicies.py` & `zope.security-7.0/src/zope/security/simplepolicies.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/testing.py` & `zope.security-7.0/src/zope/security/testing.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/tests/__init__.py` & `zope.security-7.0/src/zope/security/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/tests/exampleclass.py` & `zope.security-7.0/src/zope/security/tests/exampleclass.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/tests/module.py` & `zope.security-7.0/src/zope/security/tests/module.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/tests/redefineperms.zcml` & `zope.security-7.0/src/zope/security/tests/redefineperms.zcml`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/tests/test_adapter.py` & `zope.security-7.0/src/zope/security/tests/test_adapter.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/tests/test_checker.py` & `zope.security-7.0/src/zope/security/tests/test_checker.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/tests/test_compile_flags.py` & `zope.security-7.0/src/zope/security/tests/test_compile_flags.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/tests/test_decorator.py` & `zope.security-7.0/src/zope/security/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/tests/test_location.py` & `zope.security-7.0/src/zope/security/tests/test_location.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/tests/test_management.py` & `zope.security-7.0/src/zope/security/tests/test_management.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/tests/test_metaconfigure.py` & `zope.security-7.0/src/zope/security/tests/test_metaconfigure.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/tests/test_permission.py` & `zope.security-7.0/src/zope/security/tests/test_permission.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/tests/test_protectclass.py` & `zope.security-7.0/src/zope/security/tests/test_protectclass.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/tests/test_proxy.py` & `zope.security-7.0/src/zope/security/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/tests/test_simpleinteraction.py` & `zope.security-7.0/src/zope/security/tests/test_simpleinteraction.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/tests/test_simplepolicies.py` & `zope.security-7.0/src/zope/security/tests/test_simplepolicies.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/tests/test_testing.py` & `zope.security-7.0/src/zope/security/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/tests/test_zcml.py` & `zope.security-7.0/src/zope/security/tests/test_zcml.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/tests/test_zcml_functest.py` & `zope.security-7.0/src/zope/security/tests/test_zcml_functest.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope/security/zcml.py` & `zope.security-7.0/src/zope/security/zcml.py`

 * *Files identical despite different names*

### Comparing `zope.security-6.2a1.dev0/src/zope.security.egg-info/PKG-INFO` & `zope.security-7.0/src/zope.security.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zope.security
-Version: 6.2a1.dev0
+Version: 7.0
 Summary: Zope Security Framework
 Home-page: http://github.com/zopefoundation/zope.security
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Project-URL: Documentation, https://zopesecurity.readthedocs.io
 Project-URL: Issue Tracker, https://github.com/zopefoundation/zope.security/issues
@@ -12,32 +12,54 @@
 Keywords: zope security policy principal permission
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Framework :: Zope :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.8
+License-File: LICENSE.txt
+Requires-Dist: setuptools
+Requires-Dist: zope.component
+Requires-Dist: zope.i18nmessageid
+Requires-Dist: zope.interface
+Requires-Dist: zope.location
+Requires-Dist: zope.proxy>=5.2
+Requires-Dist: zope.schema>=4.2.0
 Provides-Extra: pytz
+Requires-Dist: pytz; extra == "pytz"
 Provides-Extra: untrustedpython
+Requires-Dist: zope.untrustedpython>=5.0.dev0; extra == "untrustedpython"
 Provides-Extra: zcml
+Requires-Dist: zope.configuration; extra == "zcml"
 Provides-Extra: test
+Requires-Dist: BTrees; extra == "test"
+Requires-Dist: zope.component; extra == "test"
+Requires-Dist: zope.configuration; extra == "test"
+Requires-Dist: zope.location; extra == "test"
+Requires-Dist: zope.testing; extra == "test"
+Requires-Dist: zope.testrunner; extra == "test"
 Provides-Extra: docs
-License-File: LICENSE.txt
+Requires-Dist: Sphinx; extra == "docs"
+Requires-Dist: repoze.sphinx.autointerface; extra == "docs"
+Requires-Dist: sphinx_rtd_theme; extra == "docs"
+Requires-Dist: zope.configuration; extra == "docs"
+Requires-Dist: zope.testing; extra == "docs"
 
 ===================
  ``zope.security``
 ===================
 
 .. image:: https://github.com/zopefoundation/zope.security/actions/workflows/tests.yml/badge.svg
         :target: https://github.com/zopefoundation/zope.security/actions/workflows/tests.yml
@@ -63,29 +85,39 @@
 
 The Security framework provides a generic mechanism to implement security
 policies on Python objects.
 
 Documentation is available at https://zopesecurity.readthedocs.io/
 
 
+
 =========
  Changes
 =========
 
-6.2a1.dev0 (2023-04-20)
------------------------
+7.0 (2024-05-30)
+----------------
+
+- Add preliminary support for Python 3.13 as of 3.13b1.
+
+- Drop support for Python 3.7.
+
+- Build windows wheels on GHA.
+
+
+6.2 (2023-10-05)
+----------------
 
 - Make ``next()`` on C proxies call ``__next__`` rather than ``next`` (see
   PEP 3114), and drop support for the Python 2 ``next`` method name from
   pure-Python proxies.
 
 - Drop using ``setup_requires`` due to constant problems on GHA.
 
-- Add preliminary support for Python 3.12 as of 3.12a7 -- even though there are
-  currently tests breaking, so please do not consider it fully supported.
+- Add support for Python 3.12.
 
 
 6.1 (2023-01-18)
 ================
 
 - Remove more proxying code for names that no longer exist in Python 3.
   (`#92 <https://github.com/zopefoundation/zope.security/issues/92>`_)
```

### Comparing `zope.security-6.2a1.dev0/src/zope.security.egg-info/SOURCES.txt` & `zope.security-7.0/src/zope.security.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,50 @@
 .coveragerc
 .manylinux-install.sh
 .manylinux.sh
+.readthedocs.yaml
 CHANGES.rst
 CONTRIBUTING.md
 COPYRIGHT.txt
 LICENSE.txt
 MANIFEST.in
 README.rst
-appveyor.yml
 buildout.cfg
-rtd.txt
 setup.cfg
 setup.py
 tox.ini
 docs/Makefile
 docs/changes.rst
 docs/conf.py
 docs/example.rst
 docs/hacking.rst
 docs/index.rst
 docs/make.bat
 docs/narr.rst
 docs/proxy.rst
+docs/requirements.txt
+docs/_build/doctest/output.txt
+docs/_build/html/_sources/changes.rst.txt
+docs/_build/html/_sources/example.rst.txt
+docs/_build/html/_sources/hacking.rst.txt
+docs/_build/html/_sources/index.rst.txt
+docs/_build/html/_sources/narr.rst.txt
+docs/_build/html/_sources/proxy.rst.txt
+docs/_build/html/_sources/api/adapter.rst.txt
+docs/_build/html/_sources/api/checker.rst.txt
+docs/_build/html/_sources/api/decorator.rst.txt
+docs/_build/html/_sources/api/interfaces.rst.txt
+docs/_build/html/_sources/api/management.rst.txt
+docs/_build/html/_sources/api/metaconfigure.rst.txt
+docs/_build/html/_sources/api/permission.rst.txt
+docs/_build/html/_sources/api/protectclass.rst.txt
+docs/_build/html/_sources/api/proxy.rst.txt
+docs/_build/html/_sources/api/simplepolicies.rst.txt
+docs/_build/html/_sources/api/testing.rst.txt
+docs/_build/html/_sources/api/zcml.rst.txt
 docs/api/adapter.rst
 docs/api/checker.rst
 docs/api/decorator.rst
 docs/api/interfaces.rst
 docs/api/management.rst
 docs/api/metaconfigure.rst
 docs/api/permission.rst
```

### Comparing `zope.security-6.2a1.dev0/tox.ini` & `zope.security-7.0/tox.ini`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,37 @@
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
+    py313,py313-pure
     pypy3
     docs
     coverage
-    py37-watch, py311-watch
+    py38-watch, py311-watch
 
 [testenv]
 usedevelop = true
-pip_pre = py312: true
+pip_pre = py313: true
 deps =
+    setuptools < 69
     Sphinx
 setenv =
     pure: PURE_PYTHON=1
     !pure-!pypy3: PURE_PYTHON=0
     ZOPE_INTERFACE_STRICT_IRO=1
     watch: ZOPE_WATCH_CHECKERS=1
+    py312: VIRTUALENV_PIP=23.1.2
+    py312: PIP_REQUIRE_VIRTUALENV=0
 commands =
     zope-testrunner --test-path=src {posargs:-vc}
     sphinx-build -b doctest -d {envdir}/.cache/doctrees docs {envdir}/.cache/doctest
 extras =
     test
     docs
 
@@ -41,29 +44,40 @@
 setenv =
     PURE_PYTHON=1
 commands =
     mkdir -p {toxinidir}/parts/htmlcov
     coverage run -m zope.testrunner --test-path=src {posargs:-vc}
     coverage html -i
     coverage report -i -m --fail-under=99.5
+[testenv:release-check]
+description = ensure that the distribution is ready to release
+basepython = python3
+skip_install = true
+deps =
+    twine
+    build
+    check-manifest
+    check-python-versions >= 0.20.0
+    wheel
+commands_pre =
+commands =
+    check-manifest
+    check-python-versions --only setup.py,tox.ini,.github/workflows/tests.yml
+    python -m build --sdist --no-isolation
+    twine check dist/*
 
 [testenv:lint]
 basepython = python3
 skip_install = true
+deps =
+    isort
+    flake8
 commands =
     isort --check-only --diff {toxinidir}/src {toxinidir}/setup.py
     flake8 src setup.py
-    check-manifest
-    check-python-versions
-deps =
-    check-manifest
-    check-python-versions >= 0.19.1
-    wheel
-    flake8
-    isort
 
 [testenv:isort-apply]
 basepython = python3
 skip_install = true
 commands_pre =
 deps =
     isort
```

