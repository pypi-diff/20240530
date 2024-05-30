# Comparing `tmp/AccessControl-6.3.tar.gz` & `tmp/AccessControl-7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AccessControl-6.3.tar", last modified: Mon Nov 20 07:13:19 2023, max compression
+gzip compressed data, was "AccessControl-7.0.tar", last modified: Thu May 30 08:29:13 2024, max compression
```

## Comparing `AccessControl-6.3.tar` & `AccessControl-7.0.tar`

### file list

```diff
@@ -1,105 +1,104 @@
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-11-20 07:13:19.647134 AccessControl-6.3/
--rw-r--r--   0 m.howitz   (502) staff       (20)      587 2023-11-20 07:13:19.000000 AccessControl-6.3/.coveragerc
--rwxr-xr-x   0 m.howitz   (502) staff       (20)     1994 2023-11-20 07:13:19.000000 AccessControl-6.3/.manylinux-install.sh
--rwxr-xr-x   0 m.howitz   (502) staff       (20)      509 2023-11-20 07:13:19.000000 AccessControl-6.3/.manylinux.sh
--rw-r--r--   0 m.howitz   (502) staff       (20)     7163 2023-11-20 07:13:19.000000 AccessControl-6.3/CHANGES.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      799 2023-11-20 07:13:19.000000 AccessControl-6.3/CONTRIBUTING.md
--rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-11-20 07:13:19.000000 AccessControl-6.3/COPYRIGHT.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)     1849 2023-11-20 07:13:19.000000 AccessControl-6.3/HISTORY.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2023-11-20 07:13:19.000000 AccessControl-6.3/LICENSE.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)      359 2023-11-20 07:13:19.000000 AccessControl-6.3/MANIFEST.in
--rw-r--r--   0 m.howitz   (502) staff       (20)     9766 2023-11-20 07:13:19.646986 AccessControl-6.3/PKG-INFO
--rw-r--r--   0 m.howitz   (502) staff       (20)      768 2023-11-20 07:13:19.000000 AccessControl-6.3/README.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     1804 2023-11-20 07:13:19.000000 AccessControl-6.3/appveyor.yml
--rw-r--r--   0 m.howitz   (502) staff       (20)      439 2023-11-20 07:13:19.000000 AccessControl-6.3/buildout.cfg
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-11-20 07:13:19.632435 AccessControl-6.3/docs/
--rw-r--r--   0 m.howitz   (502) staff       (20)     6187 2023-11-20 07:13:19.000000 AccessControl-6.3/docs/AccessControl.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     1090 2023-11-20 07:13:19.000000 AccessControl-6.3/docs/requestmethod.rst
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-11-20 07:13:19.628432 AccessControl-6.3/include/
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-11-20 07:13:19.632692 AccessControl-6.3/include/Acquisition/
--rw-r--r--   0 m.howitz   (502) staff       (20)     2451 2023-11-20 07:13:19.000000 AccessControl-6.3/include/Acquisition/Acquisition.h
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-11-20 07:13:19.633085 AccessControl-6.3/include/ExtensionClass/
--rw-r--r--   0 m.howitz   (502) staff       (20)     9572 2023-11-20 07:13:19.000000 AccessControl-6.3/include/ExtensionClass/ExtensionClass.h
--rw-r--r--   0 m.howitz   (502) staff       (20)     1964 2023-11-20 07:13:19.000000 AccessControl-6.3/include/ExtensionClass/_compat.h
--rw-r--r--   0 m.howitz   (502) staff       (20)      583 2023-11-20 07:13:19.647413 AccessControl-6.3/setup.cfg
--rw-r--r--   0 m.howitz   (502) staff       (20)     3613 2023-11-20 07:13:19.000000 AccessControl-6.3/setup.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-11-20 07:13:19.628804 AccessControl-6.3/src/
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-11-20 07:13:19.640257 AccessControl-6.3/src/AccessControl/
--rw-r--r--   0 m.howitz   (502) staff       (20)     2211 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/AuthEncoding.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1732 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/ImplC.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    32088 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/ImplPython.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     3805 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/Implementation.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1237 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/Owned.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     5312 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/Permission.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     5202 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/PermissionMapping.py
--rw-r--r--   0 m.howitz   (502) staff       (20)      826 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/PermissionRole.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     2876 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/Permissions.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1563 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/Role.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    13880 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/SecurityInfo.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     2463 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/SecurityManagement.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1097 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/SecurityManager.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     4882 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/SimpleObjectPolicies.py
--rw-r--r--   0 m.howitz   (502) staff       (20)      912 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/SpecialUsers.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     2328 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/User.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    17536 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/ZopeGuards.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1951 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/ZopeSecurityPolicy.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     2366 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/__init__.py
--rw-r--r--   0 m.howitz   (502) staff       (20)      738 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/_compat.h
--rw-r--r--   0 m.howitz   (502) staff       (20)    62941 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/cAccessControl.c
--rw-r--r--   0 m.howitz   (502) staff       (20)     3889 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/class_init.py
--rw-r--r--   0 m.howitz   (502) staff       (20)      104 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/configure.zcml
--rw-r--r--   0 m.howitz   (502) staff       (20)    11074 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/interfaces.py
--rw-r--r--   0 m.howitz   (502) staff       (20)      214 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/logger_wrapper.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1443 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/meta.zcml
--rw-r--r--   0 m.howitz   (502) staff       (20)     2095 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/metaconfigure.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     8617 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/owner.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1691 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/permissions.zcml
--rw-r--r--   0 m.howitz   (502) staff       (20)     3344 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/requestmethod.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    16013 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/rolemanager.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     2340 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/safe_formatter.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     7349 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/security.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     5518 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/tainted.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-11-20 07:13:19.645436 AccessControl-6.3/src/AccessControl/tests/
--rw-r--r--   0 m.howitz   (502) staff       (20)        0 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/tests/__init__.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     5168 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/tests/actual_python.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-11-20 07:13:19.645664 AccessControl-6.3/src/AccessControl/tests/mixed_module/
--rw-r--r--   0 m.howitz   (502) staff       (20)       78 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/tests/mixed_module/__init__.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-11-20 07:13:19.645829 AccessControl-6.3/src/AccessControl/tests/mixed_module/submodule/
--rw-r--r--   0 m.howitz   (502) staff       (20)       46 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/tests/mixed_module/submodule/__init__.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-11-20 07:13:19.646003 AccessControl-6.3/src/AccessControl/tests/private_module/
--rw-r--r--   0 m.howitz   (502) staff       (20)       50 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/tests/private_module/__init__.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-11-20 07:13:19.646165 AccessControl-6.3/src/AccessControl/tests/private_module/submodule/
--rw-r--r--   0 m.howitz   (502) staff       (20)       50 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/tests/private_module/submodule/__init__.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-11-20 07:13:19.646327 AccessControl-6.3/src/AccessControl/tests/public_module/
--rw-r--r--   0 m.howitz   (502) staff       (20)      125 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/tests/public_module/__init__.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-11-20 07:13:19.646515 AccessControl-6.3/src/AccessControl/tests/public_module/submodule/
--rw-r--r--   0 m.howitz   (502) staff       (20)       44 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/tests/public_module/submodule/__init__.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     6618 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/tests/testClassSecurityInfo.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     2449 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/tests/testImplementation.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     4805 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/tests/testModuleSecurity.py
--rw-r--r--   0 m.howitz   (502) staff       (20)      343 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/tests/testPermissionMapping.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     4110 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/tests/testPermissionRole.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     9361 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/tests/testSecurityManager.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    15171 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/tests/testZCML.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    33544 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/tests/testZopeGuards.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    25448 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/tests/testZopeSecurityPolicy.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     9056 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/tests/test_owner.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     5411 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/tests/test_requestmethod.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     4708 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/tests/test_rolemanager.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     9743 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/tests/test_safe_formatter.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     2138 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/tests/test_safeiter.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    12667 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/tests/test_tainted.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     6446 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/tests/test_userfolder.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    22853 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/tests/test_users.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1224 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/unauthorized.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    17049 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/userfolder.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    15399 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl/users.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-11-20 07:13:19.641616 AccessControl-6.3/src/AccessControl.egg-info/
--rw-r--r--   0 m.howitz   (502) staff       (20)     9766 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl.egg-info/PKG-INFO
--rw-r--r--   0 m.howitz   (502) staff       (20)     2999 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl.egg-info/SOURCES.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl.egg-info/dependency_links.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)       67 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl.egg-info/entry_points.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl.egg-info/not-zip-safe
--rw-r--r--   0 m.howitz   (502) staff       (20)      311 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl.egg-info/requires.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)       14 2023-11-20 07:13:19.000000 AccessControl-6.3/src/AccessControl.egg-info/top_level.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)     1494 2023-11-20 07:13:19.000000 AccessControl-6.3/tox.ini
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 08:29:13.964261 AccessControl-7.0/
+-rw-r--r--   0 jens       (501) staff       (20)      608 2024-05-29 19:05:00.000000 AccessControl-7.0/.coveragerc
+-rwxr-xr-x   0 jens       (501) staff       (20)     2192 2024-05-29 19:05:00.000000 AccessControl-7.0/.manylinux-install.sh
+-rwxr-xr-x   0 jens       (501) staff       (20)      509 2024-05-29 19:05:00.000000 AccessControl-7.0/.manylinux.sh
+-rw-r--r--   0 jens       (501) staff       (20)     7628 2024-05-30 06:56:05.000000 AccessControl-7.0/CHANGES.rst
+-rw-r--r--   0 jens       (501) staff       (20)      799 2024-05-29 19:05:00.000000 AccessControl-7.0/CONTRIBUTING.md
+-rw-r--r--   0 jens       (501) staff       (20)       32 2021-11-02 08:50:53.000000 AccessControl-7.0/COPYRIGHT.txt
+-rw-r--r--   0 jens       (501) staff       (20)     1849 2021-11-02 08:50:53.000000 AccessControl-7.0/HISTORY.rst
+-rw-r--r--   0 jens       (501) staff       (20)     2070 2021-11-02 08:50:53.000000 AccessControl-7.0/LICENSE.txt
+-rw-r--r--   0 jens       (501) staff       (20)      338 2024-05-29 19:05:00.000000 AccessControl-7.0/MANIFEST.in
+-rw-r--r--   0 jens       (501) staff       (20)    10232 2024-05-30 08:29:13.964163 AccessControl-7.0/PKG-INFO
+-rw-r--r--   0 jens       (501) staff       (20)      768 2022-03-26 10:28:34.000000 AccessControl-7.0/README.rst
+-rw-r--r--   0 jens       (501) staff       (20)      439 2023-01-11 16:46:17.000000 AccessControl-7.0/buildout.cfg
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 08:29:13.949054 AccessControl-7.0/docs/
+-rw-r--r--   0 jens       (501) staff       (20)     6187 2021-11-02 08:50:53.000000 AccessControl-7.0/docs/AccessControl.rst
+-rw-r--r--   0 jens       (501) staff       (20)     1090 2021-11-02 08:50:53.000000 AccessControl-7.0/docs/requestmethod.rst
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 08:29:13.945709 AccessControl-7.0/include/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 08:29:13.949282 AccessControl-7.0/include/Acquisition/
+-rw-r--r--   0 jens       (501) staff       (20)     2451 2023-04-18 09:21:36.000000 AccessControl-7.0/include/Acquisition/Acquisition.h
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 08:29:13.949790 AccessControl-7.0/include/ExtensionClass/
+-rw-r--r--   0 jens       (501) staff       (20)     9572 2023-04-18 09:22:22.000000 AccessControl-7.0/include/ExtensionClass/ExtensionClass.h
+-rw-r--r--   0 jens       (501) staff       (20)     1964 2023-04-19 05:40:53.000000 AccessControl-7.0/include/ExtensionClass/_compat.h
+-rw-r--r--   0 jens       (501) staff       (20)      554 2024-05-30 08:29:13.964491 AccessControl-7.0/setup.cfg
+-rw-r--r--   0 jens       (501) staff       (20)     3614 2024-05-30 06:56:20.000000 AccessControl-7.0/setup.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 08:29:13.945862 AccessControl-7.0/src/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 08:29:13.957543 AccessControl-7.0/src/AccessControl/
+-rw-r--r--   0 jens       (501) staff       (20)     2211 2023-01-03 12:38:42.000000 AccessControl-7.0/src/AccessControl/AuthEncoding.py
+-rw-r--r--   0 jens       (501) staff       (20)     1732 2021-11-02 08:50:53.000000 AccessControl-7.0/src/AccessControl/ImplC.py
+-rw-r--r--   0 jens       (501) staff       (20)    32088 2023-04-18 09:53:10.000000 AccessControl-7.0/src/AccessControl/ImplPython.py
+-rw-r--r--   0 jens       (501) staff       (20)     3805 2023-01-03 12:38:42.000000 AccessControl-7.0/src/AccessControl/Implementation.py
+-rw-r--r--   0 jens       (501) staff       (20)     1237 2021-11-02 08:50:53.000000 AccessControl-7.0/src/AccessControl/Owned.py
+-rw-r--r--   0 jens       (501) staff       (20)     5312 2022-03-26 10:28:34.000000 AccessControl-7.0/src/AccessControl/Permission.py
+-rw-r--r--   0 jens       (501) staff       (20)     5202 2023-01-03 12:38:42.000000 AccessControl-7.0/src/AccessControl/PermissionMapping.py
+-rw-r--r--   0 jens       (501) staff       (20)      826 2021-11-02 08:50:53.000000 AccessControl-7.0/src/AccessControl/PermissionRole.py
+-rw-r--r--   0 jens       (501) staff       (20)     2876 2021-11-02 08:50:53.000000 AccessControl-7.0/src/AccessControl/Permissions.py
+-rw-r--r--   0 jens       (501) staff       (20)     1563 2021-11-02 08:50:53.000000 AccessControl-7.0/src/AccessControl/Role.py
+-rw-r--r--   0 jens       (501) staff       (20)    13921 2024-04-26 11:46:09.000000 AccessControl-7.0/src/AccessControl/SecurityInfo.py
+-rw-r--r--   0 jens       (501) staff       (20)     2463 2023-01-03 12:38:42.000000 AccessControl-7.0/src/AccessControl/SecurityManagement.py
+-rw-r--r--   0 jens       (501) staff       (20)     1097 2021-11-02 08:50:53.000000 AccessControl-7.0/src/AccessControl/SecurityManager.py
+-rw-r--r--   0 jens       (501) staff       (20)     4882 2023-01-03 12:38:42.000000 AccessControl-7.0/src/AccessControl/SimpleObjectPolicies.py
+-rw-r--r--   0 jens       (501) staff       (20)      912 2021-11-02 08:50:53.000000 AccessControl-7.0/src/AccessControl/SpecialUsers.py
+-rw-r--r--   0 jens       (501) staff       (20)     2328 2021-11-02 08:50:53.000000 AccessControl-7.0/src/AccessControl/User.py
+-rw-r--r--   0 jens       (501) staff       (20)    18885 2024-04-26 11:46:09.000000 AccessControl-7.0/src/AccessControl/ZopeGuards.py
+-rw-r--r--   0 jens       (501) staff       (20)     1951 2023-01-03 12:38:42.000000 AccessControl-7.0/src/AccessControl/ZopeSecurityPolicy.py
+-rw-r--r--   0 jens       (501) staff       (20)     2366 2023-10-05 09:11:59.000000 AccessControl-7.0/src/AccessControl/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)      738 2023-04-17 06:50:46.000000 AccessControl-7.0/src/AccessControl/_compat.h
+-rw-r--r--   0 jens       (501) staff       (20)    62987 2024-05-24 12:46:39.000000 AccessControl-7.0/src/AccessControl/cAccessControl.c
+-rw-r--r--   0 jens       (501) staff       (20)     3889 2023-04-17 06:50:46.000000 AccessControl-7.0/src/AccessControl/class_init.py
+-rw-r--r--   0 jens       (501) staff       (20)      104 2021-11-02 08:50:53.000000 AccessControl-7.0/src/AccessControl/configure.zcml
+-rw-r--r--   0 jens       (501) staff       (20)    11074 2023-01-03 12:38:42.000000 AccessControl-7.0/src/AccessControl/interfaces.py
+-rw-r--r--   0 jens       (501) staff       (20)      217 2024-04-26 11:46:09.000000 AccessControl-7.0/src/AccessControl/logger_wrapper.py
+-rw-r--r--   0 jens       (501) staff       (20)     1443 2021-11-02 08:50:53.000000 AccessControl-7.0/src/AccessControl/meta.zcml
+-rw-r--r--   0 jens       (501) staff       (20)     2095 2021-11-02 08:50:53.000000 AccessControl-7.0/src/AccessControl/metaconfigure.py
+-rw-r--r--   0 jens       (501) staff       (20)     8617 2022-03-26 10:28:34.000000 AccessControl-7.0/src/AccessControl/owner.py
+-rw-r--r--   0 jens       (501) staff       (20)     1691 2021-11-02 08:50:53.000000 AccessControl-7.0/src/AccessControl/permissions.zcml
+-rw-r--r--   0 jens       (501) staff       (20)     3344 2023-01-03 12:38:42.000000 AccessControl-7.0/src/AccessControl/requestmethod.py
+-rw-r--r--   0 jens       (501) staff       (20)    16013 2023-01-03 12:38:42.000000 AccessControl-7.0/src/AccessControl/rolemanager.py
+-rw-r--r--   0 jens       (501) staff       (20)     2340 2023-10-05 09:11:59.000000 AccessControl-7.0/src/AccessControl/safe_formatter.py
+-rw-r--r--   0 jens       (501) staff       (20)     7349 2023-01-03 12:38:42.000000 AccessControl-7.0/src/AccessControl/security.py
+-rw-r--r--   0 jens       (501) staff       (20)     5518 2023-01-03 12:38:42.000000 AccessControl-7.0/src/AccessControl/tainted.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 08:29:13.962740 AccessControl-7.0/src/AccessControl/tests/
+-rw-r--r--   0 jens       (501) staff       (20)        0 2021-11-02 08:50:53.000000 AccessControl-7.0/src/AccessControl/tests/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)     6286 2024-04-26 11:46:09.000000 AccessControl-7.0/src/AccessControl/tests/actual_python.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 08:29:13.962893 AccessControl-7.0/src/AccessControl/tests/mixed_module/
+-rw-r--r--   0 jens       (501) staff       (20)       78 2021-11-02 08:50:53.000000 AccessControl-7.0/src/AccessControl/tests/mixed_module/__init__.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 08:29:13.963106 AccessControl-7.0/src/AccessControl/tests/mixed_module/submodule/
+-rw-r--r--   0 jens       (501) staff       (20)       46 2021-11-02 08:50:53.000000 AccessControl-7.0/src/AccessControl/tests/mixed_module/submodule/__init__.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 08:29:13.963307 AccessControl-7.0/src/AccessControl/tests/private_module/
+-rw-r--r--   0 jens       (501) staff       (20)       50 2021-11-02 08:50:53.000000 AccessControl-7.0/src/AccessControl/tests/private_module/__init__.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 08:29:13.963455 AccessControl-7.0/src/AccessControl/tests/private_module/submodule/
+-rw-r--r--   0 jens       (501) staff       (20)       50 2021-11-02 08:50:53.000000 AccessControl-7.0/src/AccessControl/tests/private_module/submodule/__init__.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 08:29:13.963577 AccessControl-7.0/src/AccessControl/tests/public_module/
+-rw-r--r--   0 jens       (501) staff       (20)      125 2021-11-02 08:50:53.000000 AccessControl-7.0/src/AccessControl/tests/public_module/__init__.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 08:29:13.963794 AccessControl-7.0/src/AccessControl/tests/public_module/submodule/
+-rw-r--r--   0 jens       (501) staff       (20)       44 2021-11-02 08:50:53.000000 AccessControl-7.0/src/AccessControl/tests/public_module/submodule/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)     6618 2021-11-02 08:50:53.000000 AccessControl-7.0/src/AccessControl/tests/testClassSecurityInfo.py
+-rw-r--r--   0 jens       (501) staff       (20)     2449 2023-01-03 12:38:42.000000 AccessControl-7.0/src/AccessControl/tests/testImplementation.py
+-rw-r--r--   0 jens       (501) staff       (20)     4805 2022-05-03 09:03:15.000000 AccessControl-7.0/src/AccessControl/tests/testModuleSecurity.py
+-rw-r--r--   0 jens       (501) staff       (20)      343 2021-11-02 08:50:53.000000 AccessControl-7.0/src/AccessControl/tests/testPermissionMapping.py
+-rw-r--r--   0 jens       (501) staff       (20)     4110 2023-01-03 12:38:42.000000 AccessControl-7.0/src/AccessControl/tests/testPermissionRole.py
+-rw-r--r--   0 jens       (501) staff       (20)     9361 2022-03-26 10:28:34.000000 AccessControl-7.0/src/AccessControl/tests/testSecurityManager.py
+-rw-r--r--   0 jens       (501) staff       (20)    15171 2023-01-03 12:38:42.000000 AccessControl-7.0/src/AccessControl/tests/testZCML.py
+-rw-r--r--   0 jens       (501) staff       (20)    34166 2024-04-26 11:46:09.000000 AccessControl-7.0/src/AccessControl/tests/testZopeGuards.py
+-rw-r--r--   0 jens       (501) staff       (20)    25448 2023-01-03 12:38:42.000000 AccessControl-7.0/src/AccessControl/tests/testZopeSecurityPolicy.py
+-rw-r--r--   0 jens       (501) staff       (20)     9056 2023-01-03 12:38:42.000000 AccessControl-7.0/src/AccessControl/tests/test_owner.py
+-rw-r--r--   0 jens       (501) staff       (20)     5411 2021-11-02 08:50:53.000000 AccessControl-7.0/src/AccessControl/tests/test_requestmethod.py
+-rw-r--r--   0 jens       (501) staff       (20)     4708 2021-11-02 08:50:53.000000 AccessControl-7.0/src/AccessControl/tests/test_rolemanager.py
+-rw-r--r--   0 jens       (501) staff       (20)     9743 2023-10-05 09:11:59.000000 AccessControl-7.0/src/AccessControl/tests/test_safe_formatter.py
+-rw-r--r--   0 jens       (501) staff       (20)     2138 2021-11-02 08:50:53.000000 AccessControl-7.0/src/AccessControl/tests/test_safeiter.py
+-rw-r--r--   0 jens       (501) staff       (20)    12667 2023-01-03 12:38:42.000000 AccessControl-7.0/src/AccessControl/tests/test_tainted.py
+-rw-r--r--   0 jens       (501) staff       (20)     6446 2021-11-02 08:50:53.000000 AccessControl-7.0/src/AccessControl/tests/test_userfolder.py
+-rw-r--r--   0 jens       (501) staff       (20)    22853 2023-01-03 12:38:42.000000 AccessControl-7.0/src/AccessControl/tests/test_users.py
+-rw-r--r--   0 jens       (501) staff       (20)     1224 2021-11-02 08:50:53.000000 AccessControl-7.0/src/AccessControl/unauthorized.py
+-rw-r--r--   0 jens       (501) staff       (20)    17049 2023-01-03 12:38:42.000000 AccessControl-7.0/src/AccessControl/userfolder.py
+-rw-r--r--   0 jens       (501) staff       (20)    15399 2023-01-03 12:38:42.000000 AccessControl-7.0/src/AccessControl/users.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-30 08:29:13.958407 AccessControl-7.0/src/AccessControl.egg-info/
+-rw-r--r--   0 jens       (501) staff       (20)    10232 2024-05-30 08:29:13.000000 AccessControl-7.0/src/AccessControl.egg-info/PKG-INFO
+-rw-r--r--   0 jens       (501) staff       (20)     2986 2024-05-30 08:29:13.000000 AccessControl-7.0/src/AccessControl.egg-info/SOURCES.txt
+-rw-r--r--   0 jens       (501) staff       (20)        1 2024-05-30 08:29:13.000000 AccessControl-7.0/src/AccessControl.egg-info/dependency_links.txt
+-rw-r--r--   0 jens       (501) staff       (20)       67 2024-05-30 08:29:13.000000 AccessControl-7.0/src/AccessControl.egg-info/entry_points.txt
+-rw-r--r--   0 jens       (501) staff       (20)        1 2022-03-26 10:31:42.000000 AccessControl-7.0/src/AccessControl.egg-info/not-zip-safe
+-rw-r--r--   0 jens       (501) staff       (20)      311 2024-05-30 08:29:13.000000 AccessControl-7.0/src/AccessControl.egg-info/requires.txt
+-rw-r--r--   0 jens       (501) staff       (20)       14 2024-05-30 08:29:13.000000 AccessControl-7.0/src/AccessControl.egg-info/top_level.txt
+-rw-r--r--   0 jens       (501) staff       (20)     1605 2024-05-29 19:05:00.000000 AccessControl-7.0/tox.ini
```

### Comparing `AccessControl-6.3/.coveragerc` & `AccessControl-7.0/.coveragerc`

 * *Files 22% similar despite different names*

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

### Comparing `AccessControl-6.3/.manylinux-install.sh` & `AccessControl-7.0/.manylinux-install.sh`

 * *Files 9% similar despite different names*

```diff
@@ -24,35 +24,40 @@
 ls -ld /cache/pip
 
 # We need some libraries because we build wheels from scratch:
 yum -y install libffi-devel
 
 tox_env_map() {
     case $1 in
-        *"cp37"*) echo 'py37';;
+        *"cp313"*) echo 'py313';;
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
-       [[ "${PYBIN}" == *"cp311"* ]] || \
-       [[ "${PYBIN}" == *"cp312"* ]] || \
-       [[ "${PYBIN}" == *"cp37"* ]] || \
-       [[ "${PYBIN}" == *"cp38"* ]] || \
-       [[ "${PYBIN}" == *"cp39"* ]] || \
-       [[ "${PYBIN}" == *"cp310"* ]] ; then
-        "${PYBIN}/pip" install -e /io/
-        "${PYBIN}/pip" wheel /io/ -w wheelhouse/
+       [[ "${PYBIN}" == *"cp313/"* ]] || \
+       [[ "${PYBIN}" == *"cp311/"* ]] || \
+       [[ "${PYBIN}" == *"cp312/"* ]] || \
+       [[ "${PYBIN}" == *"cp38/"* ]] || \
+       [[ "${PYBIN}" == *"cp39/"* ]] || \
+       [[ "${PYBIN}" == *"cp310/"* ]] ; then
+        if [[ "${PYBIN}" == *"cp313/"* ]] ; then
+            "${PYBIN}/pip" install --pre -e /io/
+            "${PYBIN}/pip" wheel /io/ --pre -w wheelhouse/
+        else
+            "${PYBIN}/pip" install -e /io/
+            "${PYBIN}/pip" wheel /io/ -w wheelhouse/
+        fi
         if [ `uname -m` == 'aarch64' ]; then
           cd /io/
           ${PYBIN}/pip install tox
           TOXENV=$(tox_env_map "${PYBIN}")
           ${PYBIN}/tox -e ${TOXENV}
           cd ..
         fi
```

### Comparing `AccessControl-6.3/CHANGES.rst` & `AccessControl-7.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,31 @@
 Changelog
 =========
 
 For changes before version 3.0, see ``HISTORY.rst``.
 
+7.0 (2024-05-30)
+----------------
+
+- Add preliminary support for Python 3.13 as of 3.13b1.
+
+- Remove support for Python 3.7.
+
+- Build Windows wheels on GHA.
+
+- Make dict views (`.keys()`, `.items()` and `.values()`) behave like their
+  unrestricted versions.
+  (`#147 <https://github.com/zopefoundation/AccessControl/pull/147>`_)
+
+- Make `.items()` validate each keys and values, like `.keys()` and
+  `.values()` do.
+
+- Fix build errors on recent macOS versions.
+
+
 6.3 (2023-11-20)
 ----------------
 
 - Add support for Python 3.12.
 
 
 6.2 (2023-09-04)
```

### Comparing `AccessControl-6.3/CONTRIBUTING.md` & `AccessControl-7.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/HISTORY.rst` & `AccessControl-7.0/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/LICENSE.txt` & `AccessControl-7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/PKG-INFO` & `AccessControl-7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AccessControl
-Version: 6.3
+Version: 7.0
 Summary: Security framework for Zope.
 Home-page: https://github.com/zopefoundation/AccessControl
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Project-URL: Issue Tracker, https://github.com/zopefoundation/AccessControl/issues
 Project-URL: Sources, https://github.com/zopefoundation/AccessControl
@@ -13,22 +13,22 @@
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Zope
 Classifier: Framework :: Zope :: 5
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Operating System :: OS Independent
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
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 License-File: LICENSE.txt
 Requires-Dist: Acquisition
 Requires-Dist: AuthEncoding
 Requires-Dist: BTrees
 Requires-Dist: DateTime
 Requires-Dist: ExtensionClass>=4.2.1
 Requires-Dist: Persistence>=3.0a3
@@ -69,14 +69,33 @@
 
 
 Changelog
 =========
 
 For changes before version 3.0, see ``HISTORY.rst``.
 
+7.0 (2024-05-30)
+----------------
+
+- Add preliminary support for Python 3.13 as of 3.13b1.
+
+- Remove support for Python 3.7.
+
+- Build Windows wheels on GHA.
+
+- Make dict views (`.keys()`, `.items()` and `.values()`) behave like their
+  unrestricted versions.
+  (`#147 <https://github.com/zopefoundation/AccessControl/pull/147>`_)
+
+- Make `.items()` validate each keys and values, like `.keys()` and
+  `.values()` do.
+
+- Fix build errors on recent macOS versions.
+
+
 6.3 (2023-11-20)
 ----------------
 
 - Add support for Python 3.12.
 
 
 6.2 (2023-09-04)
```

### Comparing `AccessControl-6.3/README.rst` & `AccessControl-7.0/README.rst`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/docs/AccessControl.rst` & `AccessControl-7.0/docs/AccessControl.rst`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/docs/requestmethod.rst` & `AccessControl-7.0/docs/requestmethod.rst`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/include/Acquisition/Acquisition.h` & `AccessControl-7.0/include/Acquisition/Acquisition.h`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/include/ExtensionClass/ExtensionClass.h` & `AccessControl-7.0/include/ExtensionClass/ExtensionClass.h`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/include/ExtensionClass/_compat.h` & `AccessControl-7.0/include/ExtensionClass/_compat.h`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/setup.py` & `AccessControl-7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         include_dirs=['include', 'src'],
         sources=[join('src', 'AccessControl', 'cAccessControl.c')],
         depends=[join('include', 'ExtensionClass', 'ExtensionClass.h'),
                  join('include', 'ExtensionClass', '_compat.h'),
                  join('include', 'Acquisition', 'Acquisition.h')]),
 ]
 
-version = '6.3'
+version = '7.0'
 
 
 setup(name='AccessControl',
       version=version,
       url='https://github.com/zopefoundation/AccessControl',
       project_urls={
           'Issue Tracker': ('https://github.com/zopefoundation'
@@ -56,20 +56,20 @@
           'Environment :: Web Environment',
           'Framework :: Zope',
           'Framework :: Zope :: 5',
           'License :: OSI Approved :: Zope Public License',
           'Operating System :: OS Independent',
           'Programming Language :: Python',
           'Programming Language :: Python :: 3',
-          'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
           'Programming Language :: Python :: 3.10',
           'Programming Language :: Python :: 3.11',
           'Programming Language :: Python :: 3.12',
+          'Programming Language :: Python :: 3.13',
           'Programming Language :: Python :: Implementation :: CPython',
       ],
       ext_modules=ext_modules,
       install_requires=[
           'Acquisition',
           'AuthEncoding',
           'BTrees',
@@ -85,15 +85,15 @@
           'zope.interface',
           'zope.publisher',
           'zope.schema',
           'zope.security',
           'zope.testing',
           'funcsigs;python_version<"3.3"',
       ],
-      python_requires='>=3.7',
+      python_requires='>=3.8',
       include_package_data=True,
       zip_safe=False,
       extras_require={
           'test': ['zope.testrunner'],
       },
       entry_points={
           'zodbupdate.decode': [
```

### Comparing `AccessControl-6.3/src/AccessControl/AuthEncoding.py` & `AccessControl-7.0/src/AccessControl/AuthEncoding.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/ImplC.py` & `AccessControl-7.0/src/AccessControl/ImplC.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/ImplPython.py` & `AccessControl-7.0/src/AccessControl/ImplPython.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/Implementation.py` & `AccessControl-7.0/src/AccessControl/Implementation.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/Owned.py` & `AccessControl-7.0/src/AccessControl/Owned.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/Permission.py` & `AccessControl-7.0/src/AccessControl/Permission.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/PermissionMapping.py` & `AccessControl-7.0/src/AccessControl/PermissionMapping.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/PermissionRole.py` & `AccessControl-7.0/src/AccessControl/PermissionRole.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/Permissions.py` & `AccessControl-7.0/src/AccessControl/Permissions.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/Role.py` & `AccessControl-7.0/src/AccessControl/Role.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/SecurityInfo.py` & `AccessControl-7.0/src/AccessControl/SecurityInfo.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,15 +74,16 @@
         self.names = {}
         self.roles = {}
         self._unused_protected_decorators = set()
 
     def _setaccess(self, names, access):
         for name in names:
             if self.names.get(name, access) != access:
-                LOG.warn('Conflicting security declarations for "%s"' % name)
+                LOG.warning(
+                    f'Conflicting security declarations for {name!r}')
                 self._warnings = 1
             self.names[name] = access
 
     declarePublic__roles__ = ACCESS_PRIVATE
 
     def declarePublic(self, name, *names):
         """Declare names to be publicly accessible."""
@@ -155,16 +156,16 @@
 
     def setPermissionDefault(self, permission_name, roles):
         """Declare default roles for a permission"""
         rdict = {}
         for role in roles:
             rdict[role] = 1
         if self.roles.get(permission_name, rdict) != rdict:
-            LOG.warn('Conflicting default role'
-                     'declarations for permission "%s"' % permission_name)
+            LOG.warning('Conflicting default role'
+                        ' declarations for permission "%s"' % permission_name)
             self._warnings = 1
         self.roles[permission_name] = rdict
 
     setDefaultAccess__roles__ = ACCESS_PRIVATE
 
     def setDefaultAccess(self, access):
         """Declare default attribute access policy.
@@ -244,16 +245,16 @@
         # Take care of default attribute access policy
         access = getattr(self, 'access', _marker)
         if access is not _marker:
             setattr(classobj, '__allow_access_to_unprotected_subobjects__',
                     access)
 
         if getattr(self, '_warnings', None):
-            LOG.warn('Class "%s" had conflicting '
-                     'security declarations' % classobj.__name__)
+            LOG.warning('Class "%s" had conflicting'
+                        ' security declarations' % classobj.__name__)
 
 
 class ClassSecurityInformation(ClassSecurityInfo):
     # Default policy is disallow
     access = 0
 
 
@@ -339,16 +340,16 @@
 
         # Start with default attribute access policy
         access = getattr(self, 'access', _marker)
         if access is not _marker or len(self.names):
             dict['__allow_access_to_unprotected_subobjects__'] = self
 
         if getattr(self, '_warnings', None):
-            LOG.warn('Module "%s" had conflicting '
-                     'security declarations' % dict['__name__'])
+            LOG.warning('Module "%s" had conflicting'
+                        ' security declarations' % dict['__name__'])
 
     declareProtected__roles__ = ACCESS_PRIVATE
 
     def declareProtected(self, permission_name, *names):
         """Cannot declare module names protected."""
         pass
```

### Comparing `AccessControl-6.3/src/AccessControl/SecurityManagement.py` & `AccessControl-7.0/src/AccessControl/SecurityManagement.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/SecurityManager.py` & `AccessControl-7.0/src/AccessControl/SecurityManager.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/SimpleObjectPolicies.py` & `AccessControl-7.0/src/AccessControl/SimpleObjectPolicies.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/SpecialUsers.py` & `AccessControl-7.0/src/AccessControl/SpecialUsers.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/User.py` & `AccessControl-7.0/src/AccessControl/User.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/ZopeGuards.py` & `AccessControl-7.0/src/AccessControl/ZopeGuards.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE
 #
 ##############################################################################
 
 
+import collections.abc
 import math
 import random
 import string
 from functools import reduce
 
 import RestrictedPython
 from RestrictedPython.Eval import RestrictionCapableEval
@@ -123,21 +124,26 @@
             raise
         else:
             del d[key]
             return v
     return guarded_pop
 
 
-def get_iter(c, name):
-    iter = getattr(c, name)
+def get_mapping_view(c, name):
 
-    def guarded_iter():
-        return SafeIter(iter(), c)
+    view_class = {
+        'keys': SafeKeysView,
+        'items': SafeItemsView,
+        'values': SafeValuesView,
+    }
 
-    return guarded_iter
+    def guarded_mapping_view():
+        return view_class[name](c)
+
+    return guarded_mapping_view
 
 
 def get_list_pop(lst, name):
     def guarded_pop(index=-1):
         # XXX This is not thread safe, but we don't expect
         # XXX thread interactions between python scripts <wink>
         v = guarded_getitem(lst, index)
@@ -149,26 +155,23 @@
 # See comment in SimpleObjectPolicies for an explanation of what the
 # dicts below actually mean.
 _dict_white_list = {
     'clear': 1,
     'copy': 1,
     'fromkeys': 1,
     'get': get_dict_get,
-    'items': 1,
+    'items': get_mapping_view,
+    'keys': get_mapping_view,
     'pop': get_dict_pop,
     'popitem': 1,
     'setdefault': 1,
     'update': 1,
+    'values': get_mapping_view,
 }
 
-_dict_white_list.update({
-    'keys': get_iter,
-    'values': get_iter,
-})
-
 
 def _check_dict_access(name, value):
     # Check whether value is a dict method
     self = getattr(value, '__self__', None)
     if self is None:  # item
         return 1
     # Disallow spoofing
@@ -268,14 +271,48 @@
 
     def __next__(self):
         return next(self._iter)
 
     next = __next__
 
 
+# The following three view classes are used only for mappings of type `dict`
+# (not subclasses). Therefore, the mapping does not have security assertions
+# and cannot acquire ones. As a consequence, the `guard` calls used in their
+# methods verify that the checked key or value is accessible based solely on
+# its own virtues, i.e. either because it is public or has its own security
+# assertions allowing access.
+class _SafeMappingView:
+    __allow_access_to_unprotected_subobjects__ = 1
+
+    def __iter__(self):
+        for e in super().__iter__():
+            guard(self._mapping, e)
+            yield e
+
+
+class SafeKeysView(_SafeMappingView, collections.abc.KeysView):
+    pass
+
+
+class SafeValuesView(_SafeMappingView, collections.abc.ValuesView):
+    pass
+
+
+class SafeItemsView(_SafeMappingView, collections.abc.ItemsView):
+    def __iter__(self):
+        for k, v in super().__iter__():
+            guard(self._mapping, k)
+            # When checking the value, we check the guard with index=None,
+            # not with index=k, the key name does not matter. guard just
+            # needs to verify that the value itself can be accessed.
+            guard(self._mapping, v)
+            yield k, v
+
+
 def _error(index):
     raise Unauthorized('unauthorized access to element')
 
 
 def guarded_iter(*args):
     if len(args) == 1:
         i = args[0]
```

### Comparing `AccessControl-6.3/src/AccessControl/ZopeSecurityPolicy.py` & `AccessControl-7.0/src/AccessControl/ZopeSecurityPolicy.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/__init__.py` & `AccessControl-7.0/src/AccessControl/__init__.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/_compat.h` & `AccessControl-7.0/src/AccessControl/_compat.h`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/cAccessControl.c` & `AccessControl-7.0/src/AccessControl/cAccessControl.c`

 * *Files 1% similar despite different names*

```diff
@@ -421,15 +421,15 @@
 static PyExtensionClass ZopeSecurityPolicyType = {
        PyVarObject_HEAD_INIT(NULL, 0)
 	"ZopeSecurityPolicy",			/* tp_name	*/
 	sizeof(ZopeSecurityPolicy),		/* tp_basicsize	*/
 	0,					/* tp_itemsize	*/
 	/* Standard methods 	*/
 	(destructor) ZopeSecurityPolicy_dealloc,/* tp_dealloc	*/
-	NULL,					/* tp_print	*/
+	0,  					/* tp_vectorcall_offset	*/
 	NULL,					/* tp_getattr	*/
 	NULL,					/* tp_setattr	*/
 	NULL,					/* tp_compare	*/
 	NULL,					/* tp_repr	*/
 	/* Method suites	*/
 	NULL,					/* tp_as_number	*/
 	NULL,					/* tp_as_sequence*/
@@ -480,15 +480,15 @@
 static PyExtensionClass SecurityManagerType = {
        PyVarObject_HEAD_INIT(NULL, 0)
 	"SecurityManager",			/* tp_name	*/
 	sizeof(SecurityManager),		/* tp_basicsize	*/
 	0,					/* tp_itemsize	*/
 	/* Standard methods 	*/
 	(destructor) SecurityManager_dealloc,/* tp_dealloc	*/
-	NULL,					/* tp_print	*/
+	0,  					/* tp_vectorcall_offset*/
 	NULL,					/* tp_getattr	*/
 	NULL,					/* tp_setattr	*/
 	NULL,					/* tp_compare	*/
 	NULL,					/* tp_repr	*/
 	/* Method suites	*/
 	NULL,					/* tp_as_number	*/
 	NULL,					/* tp_as_sequence*/
@@ -539,15 +539,15 @@
 static PyExtensionClass PermissionRoleType = {
        PyVarObject_HEAD_INIT(NULL, 0)
 	"PermissionRole",			/* tp_name	*/
 	sizeof(PermissionRole),			/* tp_basicsize	*/
 	0,					/* tp_itemsize	*/
 	/* Standard methods 	*/
 	(destructor) PermissionRole_dealloc,	/* tp_dealloc	*/
-	NULL,					/* tp_print	*/
+	0,  					/* tp_vectorcall_offset	*/
 	NULL,					/* tp_getattr	*/
 	NULL,					/* tp_setattr	*/
 	NULL,					/* tp_compare	*/
 	NULL,					/* tp_repr	*/
 	/* Method suites	*/
 	NULL,					/* tp_as_number	*/
 	NULL,					/* tp_as_sequence*/
@@ -609,15 +609,15 @@
 static PyExtensionClass imPermissionRoleType = {
        PyVarObject_HEAD_INIT(NULL, 0)
 	"imPermissionRole",			/* tp_name	*/
 	sizeof(imPermissionRole),		/* tp_basicsize	*/
 	0,					/* tp_itemsize	*/
 	/* Standard methods 	*/
 	(destructor) imPermissionRole_dealloc,	/* tp_dealloc	*/
-	NULL,					/* tp_print	*/
+	0,  					/* tp_vectorcall_offset	*/
 	NULL,					/* tp_getattr	*/
 	NULL,	                                /* tp_setattr	*/
 	NULL,					/* tp_compare	*/
 	NULL,					/* tp_repr	*/
 	/* Method suites	*/
 	NULL,					/* tp_as_number	*/
 	&imSequenceMethods,			/* tp_as_sequence*/
@@ -1067,15 +1067,15 @@
 
 	} /* if (roles == NULL) */
 
 	/*| # Short-circuit tests if we can
 	**| try:
 	**|    if roles is None or 'Anonymous' in roles: return 1
 	**| except TypeError:
-	**|     LOG.warn('"%s' passed as roles"
+	**|     LOG.warning('"%s' passed as roles"
 	**|		" during validation of '%s' is not a sequence." %
 	**|		('roles', name))
 	**|	raise
 	*/
 
 	if (roles == Py_None) {
 		rval = INT_FROM_LONG(1);
```

### Comparing `AccessControl-6.3/src/AccessControl/class_init.py` & `AccessControl-7.0/src/AccessControl/class_init.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/interfaces.py` & `AccessControl-7.0/src/AccessControl/interfaces.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/meta.zcml` & `AccessControl-7.0/src/AccessControl/meta.zcml`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/metaconfigure.py` & `AccessControl-7.0/src/AccessControl/metaconfigure.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/owner.py` & `AccessControl-7.0/src/AccessControl/owner.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/permissions.zcml` & `AccessControl-7.0/src/AccessControl/permissions.zcml`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/requestmethod.py` & `AccessControl-7.0/src/AccessControl/requestmethod.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/rolemanager.py` & `AccessControl-7.0/src/AccessControl/rolemanager.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/safe_formatter.py` & `AccessControl-7.0/src/AccessControl/safe_formatter.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/security.py` & `AccessControl-7.0/src/AccessControl/security.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/tainted.py` & `AccessControl-7.0/src/AccessControl/tainted.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/tests/actual_python.py` & `AccessControl-7.0/src/AccessControl/tests/actual_python.py`

 * *Files 25% similar despite different names*

```diff
@@ -119,14 +119,47 @@
     expected = {'k': [1, 3],
                 'v': [2, 4],
                 'i': [(1, 2), (3, 4)]}
     for meth, kind in methods:
         access = getattr(d, meth)
         result = sorted(access())
         assert result == expected[kind], (meth, kind, result, expected[kind])
+        assert len(access()) == len(expected[kind]), (meth, kind, "len")
+        iter_ = access()  # iterate twice on the same view
+        assert list(iter_) == list(iter_)
+
+        assert sorted([k for k in getattr(d, meth)()]) == expected[kind]
+        assert sorted(k for k in getattr(d, meth)()) == expected[kind]
+    assert {k: v for k, v in d.items()} == d
+
+    assert 1 in d
+    assert 1 in d.keys()
+    assert 2 in d.values()
+    assert (1, 2) in d.items()
+
+    assert d
+    assert d.keys()
+    assert d.values()
+    assert d.items()
+
+    empty_d = {}
+    assert not empty_d
+    assert not empty_d.keys()
+    assert not empty_d.values()
+    assert not empty_d.items()
+
+    smaller_d = {1: 2}
+    for m, _ in methods:
+        assert getattr(d, m)() != getattr(smaller_d, m)()
+        assert not getattr(d, m)() == getattr(smaller_d, m)()
+        if m != 'values':
+            assert getattr(d, m)() > getattr(smaller_d, m)()
+            assert getattr(d, m)() >= getattr(smaller_d, m)()
+            assert getattr(smaller_d, m)() < getattr(d, m)()
+            assert getattr(smaller_d, m)() <= getattr(d, m)()
 
 
 f7()
 
 
 def f8():
     import math
```

### Comparing `AccessControl-6.3/src/AccessControl/tests/testClassSecurityInfo.py` & `AccessControl-7.0/src/AccessControl/tests/testClassSecurityInfo.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/tests/testImplementation.py` & `AccessControl-7.0/src/AccessControl/tests/testImplementation.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/tests/testModuleSecurity.py` & `AccessControl-7.0/src/AccessControl/tests/testModuleSecurity.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/tests/testPermissionRole.py` & `AccessControl-7.0/src/AccessControl/tests/testPermissionRole.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/tests/testSecurityManager.py` & `AccessControl-7.0/src/AccessControl/tests/testSecurityManager.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/tests/testZCML.py` & `AccessControl-7.0/src/AccessControl/tests/testZCML.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/tests/testZopeGuards.py` & `AccessControl-7.0/src/AccessControl/tests/testZopeGuards.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,50 +254,66 @@
         try:
             pop('foo')
         finally:
             self.setSecurityManager(old)
         self.assertTrue(sm.calls)
 
     def test_keys_empty(self):
-        from AccessControl.ZopeGuards import get_iter
-        keys = get_iter({}, 'keys')
+        from AccessControl.ZopeGuards import get_mapping_view
+        keys = get_mapping_view({}, 'keys')
         self.assertEqual(list(keys()), [])
 
+    def test_kvi_len(self):
+        from AccessControl.ZopeGuards import get_mapping_view
+        for attr in ("keys", "values", "items"):
+            with self.subTest(attr):
+                view = get_mapping_view({'a': 1}, attr)
+                self.assertEqual(len(view()), 1)
+
     def test_keys_validates(self):
         sm = SecurityManager()
         old = self.setSecurityManager(sm)
         keys = guarded_getattr({GuardTestCase: 1}, 'keys')
         try:
-            next(keys())
+            next(iter(keys()))
         finally:
             self.setSecurityManager(old)
         self.assertTrue(sm.calls)
 
+    def test_items_validates(self):
+        sm = SecurityManager()
+        old = self.setSecurityManager(sm)
+        items = guarded_getattr({GuardTestCase: GuardTestCase}, 'items')
+        try:
+            next(iter(items()))
+        finally:
+            self.setSecurityManager(old)
+        self.assertEqual(len(sm.calls), 2)
+
     def test_values_empty(self):
-        from AccessControl.ZopeGuards import get_iter
-        values = get_iter({}, 'values')
+        from AccessControl.ZopeGuards import get_mapping_view
+        values = get_mapping_view({}, 'values')
         self.assertEqual(list(values()), [])
 
     def test_values_validates(self):
         sm = SecurityManager()
         old = self.setSecurityManager(sm)
         values = guarded_getattr({GuardTestCase: 1}, 'values')
         try:
-            next(values())
+            next(iter(values()))
         finally:
             self.setSecurityManager(old)
         self.assertTrue(sm.calls)
 
     def test_kvi_iteration(self):
-        from AccessControl.ZopeGuards import SafeIter
         d = dict(a=1, b=2)
         for attr in ("keys", "values", "items"):
             v = getattr(d, attr)()
-            si = SafeIter(v)
-            self.assertEqual(next(si), next(iter(v)))
+            si = guarded_getattr(d, attr)()
+            self.assertEqual(next(iter(si)), next(iter(v)))
 
 
 class TestListGuards(GuardTestCase):
 
     def test_pop_simple(self):
         from AccessControl.ZopeGuards import get_list_pop
         pop = get_list_pop(['foo', 'bar', 'baz'], 'pop')
```

### Comparing `AccessControl-6.3/src/AccessControl/tests/testZopeSecurityPolicy.py` & `AccessControl-7.0/src/AccessControl/tests/testZopeSecurityPolicy.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/tests/test_owner.py` & `AccessControl-7.0/src/AccessControl/tests/test_owner.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/tests/test_requestmethod.py` & `AccessControl-7.0/src/AccessControl/tests/test_requestmethod.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/tests/test_rolemanager.py` & `AccessControl-7.0/src/AccessControl/tests/test_rolemanager.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/tests/test_safe_formatter.py` & `AccessControl-7.0/src/AccessControl/tests/test_safe_formatter.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/tests/test_safeiter.py` & `AccessControl-7.0/src/AccessControl/tests/test_safeiter.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/tests/test_tainted.py` & `AccessControl-7.0/src/AccessControl/tests/test_tainted.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/tests/test_userfolder.py` & `AccessControl-7.0/src/AccessControl/tests/test_userfolder.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/tests/test_users.py` & `AccessControl-7.0/src/AccessControl/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/unauthorized.py` & `AccessControl-7.0/src/AccessControl/unauthorized.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/userfolder.py` & `AccessControl-7.0/src/AccessControl/userfolder.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl/users.py` & `AccessControl-7.0/src/AccessControl/users.py`

 * *Files identical despite different names*

### Comparing `AccessControl-6.3/src/AccessControl.egg-info/PKG-INFO` & `AccessControl-7.0/src/AccessControl.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AccessControl
-Version: 6.3
+Version: 7.0
 Summary: Security framework for Zope.
 Home-page: https://github.com/zopefoundation/AccessControl
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Project-URL: Issue Tracker, https://github.com/zopefoundation/AccessControl/issues
 Project-URL: Sources, https://github.com/zopefoundation/AccessControl
@@ -13,22 +13,22 @@
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Zope
 Classifier: Framework :: Zope :: 5
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Operating System :: OS Independent
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
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 License-File: LICENSE.txt
 Requires-Dist: Acquisition
 Requires-Dist: AuthEncoding
 Requires-Dist: BTrees
 Requires-Dist: DateTime
 Requires-Dist: ExtensionClass>=4.2.1
 Requires-Dist: Persistence>=3.0a3
@@ -69,14 +69,33 @@
 
 
 Changelog
 =========
 
 For changes before version 3.0, see ``HISTORY.rst``.
 
+7.0 (2024-05-30)
+----------------
+
+- Add preliminary support for Python 3.13 as of 3.13b1.
+
+- Remove support for Python 3.7.
+
+- Build Windows wheels on GHA.
+
+- Make dict views (`.keys()`, `.items()` and `.values()`) behave like their
+  unrestricted versions.
+  (`#147 <https://github.com/zopefoundation/AccessControl/pull/147>`_)
+
+- Make `.items()` validate each keys and values, like `.keys()` and
+  `.values()` do.
+
+- Fix build errors on recent macOS versions.
+
+
 6.3 (2023-11-20)
 ----------------
 
 - Add support for Python 3.12.
 
 
 6.2 (2023-09-04)
```

### Comparing `AccessControl-6.3/src/AccessControl.egg-info/SOURCES.txt` & `AccessControl-7.0/src/AccessControl.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 CHANGES.rst
 CONTRIBUTING.md
 COPYRIGHT.txt
 HISTORY.rst
 LICENSE.txt
 MANIFEST.in
 README.rst
-appveyor.yml
 buildout.cfg
 setup.cfg
 setup.py
 tox.ini
 docs/AccessControl.rst
 docs/requestmethod.rst
 include/Acquisition/Acquisition.h
```

### Comparing `AccessControl-6.3/tox.ini` & `AccessControl-7.0/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
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
     coverage
 
 [testenv]
 usedevelop = true
+pip_pre = py313: true
 deps =
+    setuptools < 69
 setenv =
     pure: PURE_PYTHON=1
     !pure-!pypy3: PURE_PYTHON=0
     py312: VIRTUALENV_PIP=23.1.2
     py312: PIP_REQUIRE_VIRTUALENV=0
 commands =
     zope-testrunner --test-path=src {posargs:-vc}
@@ -44,17 +46,18 @@
 skip_install = true
 deps =
     twine
     build
     check-manifest
     check-python-versions >= 0.20.0
     wheel
+commands_pre =
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
```

